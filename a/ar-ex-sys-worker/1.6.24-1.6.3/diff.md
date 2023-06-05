# Comparing `tmp/ar_ex_sys_worker-1.6.24-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16237 bytes, number of entries: 11
+Zip file size: 16290 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    27525 b- defN 23-May-12 05:03 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19928 b- defN 23-May-25 14:07 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    28707 b- defN 23-Jun-05 07:54 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19950 b- defN 23-Jun-05 07:54 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/RECORD
-11 files, 62329 bytes uncompressed, 14521 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 07:57 ar_ex_sys_worker-1.6.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      343 b- defN 23-Jun-05 07:57 ar_ex_sys_worker-1.6.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 07:57 ar_ex_sys_worker-1.6.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 07:57 ar_ex_sys_worker-1.6.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 23-Jun-05 07:57 ar_ex_sys_worker-1.6.3.dist-info/RECORD
+11 files, 63527 bytes uncompressed, 14584 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.24.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.24.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.3.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.24.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.24.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.24.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -451,15 +451,17 @@
                            'package': act['package_name']},
         }
         act_json = json.dumps(data)
         return act_json
 
 
 class SignAllActsWorkerToken(mixins.TokenAuth, SignallActWorker,
-                             mixins.TokenDBAuth, mixins.SignallActDBDeletter):
+                             mixins.TokenDBAuth, mixins.SignallActDBDeletter,
+                             mixins.ExSysActIdExtractor,
+                             mixins.SignallActUpdater,):
     def __init__(self, sql_shell, trash_cats_list, time_start, platform_id,
                  acts_limit=5, gravity_ip=None, gravity_port=8080, test=False,
                  mutex=None):
         super().__init__(sql_shell, trash_cats_list, time_start, acts_limit,
                          auto_auth=False, mutex=mutex)
         self.platform_id = platform_id
         self.gravity_ip = gravity_ip
@@ -468,17 +470,39 @@
             s.connect(("8.8.8.8", 80))
             self.gravity_ip = s.getsockname()[0]
         self.gravity_port = gravity_port
         platform_info = self.get_platform_info()[0]
         self.inn, self.kpp = platform_info['inn'], platform_info['kpp']
         if test:
             self.link_host = 'https://signalltestdev.qodex.tech'
+        self.signall_update_act_link = self.get_full_endpoint(
+                '/v1/gravity/update_act/{}')
+
+    def act_update_work(self, record_id, car_number, transporter_inn,
+                        trash_cat,
+                        trash_type, comment):
+        signal_id = self.extract_act_ex_id(record_id)
+        if not signal_id:
+            return
+        if signal_id.strip() == 'this carrier was not found':
+            self.delete_act_from_send_reports(record_id)
+            return {
+                'error': {f'Act has not been delivered cos {signal_id}. '
+                          f'Deleted from log...'}}
+        if not self.is_valid_uuid(signal_id):
+            return {'error': f'act not found in signall_id ({signal_id})'}
+        return self.update_act(
+            signall_id=signal_id,
+            car_number=car_number,
+            transporter_inn=transporter_inn,
+            trash_cat=trash_cat,
+            trash_type=trash_type,
+            comment=comment)
 
     def resend_unget_acts(self):
-        print("Resending acts")
         self.mutex.acquire()
         unsend_acts = self.get_unget_by_signall_acts()
         if not unsend_acts:
             self.mutex.release()
             return
         for act in unsend_acts:
             self.delete_act_from_send_reports(act['local_id'])
@@ -562,25 +586,27 @@
             self.delete_act_from_send_reports(act['local_id'])
 
 class SignallActUpdater(mixins.SignallMixin, DataWorker,
                         mixins.ExSysActIdExtractor,
                         mixins.SignallActUpdater,
                         mixins.SignallActDBDeletter):
     def __init__(self, sql_shell, login=None, password=None, test=False,
+                 platform_id = None,
                  **kwargs):
+        self.platform_id = platform_id
         self.sql_shell = sql_shell
         self.login = login
         self.password = password
         self.headers = self.get_headers()
         if test:
             self.link_host = "https://signalltestdev.qodex.tech"
         self.working_link = self.get_full_endpoint(
             '/v1/gravity/update_act/{}')
 
-    def work(self, record_id, car_number, transporter_inn, trash_cat,
+    def act_update_work(self, record_id, car_number, transporter_inn, trash_cat,
              trash_type, comment):
         signal_id = self.extract_act_ex_id(record_id)
         if not signal_id:
             return
         if signal_id.strip() == 'this carrier was not found':
             self.delete_act_from_send_reports(record_id)
             return {'error': {f'Act has not been delivered cos {signal_id}. '
```

## ar_external_sys_worker/mixins.py

```diff
@@ -195,26 +195,26 @@
         return requests.delete(
             self.working_link.format(id_),
             headers=self.headers)
 
 
 class SignallActUpdater:
     headers = None
-    working_link = None
+    signall_update_act_link = None
 
     def update_act(self, signall_id, car_number, transporter_inn, trash_cat,
                    trash_type, comment):
         data_json = {
             'carrier': transporter_inn,
             'comment': comment,
             'trash_cat': trash_cat,
             'trash_type': trash_type,
             'car_number': car_number}
         data_json = json.dumps(data_json)
-        response = requests.post(self.working_link.format(signall_id),
+        response = requests.post(self.signall_update_act_link.format(signall_id),
                                  headers=self.headers,
                                  data=data_json)
         return response
 
 
 class SignallGetCarriersPO:
     headers = None
```

## Comparing `ar_ex_sys_worker-1.6.24.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.6.24.dist-info/RECORD` & `ar_ex_sys_worker-1.6.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/main.py,sha256=06JgXXUu4RQ69guazXnYhKIAJmHhm4Z1SXaqs1PAfbg,27525
-ar_external_sys_worker/mixins.py,sha256=UXagTBmWlwPwMVhgjZk8WKIShc__Lm9q4r7AsswA-uQ,19928
+ar_external_sys_worker/main.py,sha256=LMc9ljc1_HTZcxBTjXmTBTOoeFA8qlLrULsYXrQfsAw,28707
+ar_external_sys_worker/mixins.py,sha256=lWm8xT9MjOXZ97L-3H8eYJ_5mPFvUYiiaGy3qXuYjRU,19950
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/tests/main_test.py,sha256=eOqy3_5sPoq7knV5fjESJ6FVWEXehwSOLTd8qXckdXw,11225
 ar_external_sys_worker/tests/mixins_test.py,sha256=NTPOm74h7bL5ra_acU3AxLgDhn75waGOGKtbkkGSxoc,1107
-ar_ex_sys_worker-1.6.24.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.6.24.dist-info/METADATA,sha256=PWrcruNxZHmfsYYBjG2TEctqKdIQnx0NhTYC-TfLacs,344
-ar_ex_sys_worker-1.6.24.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ar_ex_sys_worker-1.6.24.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.6.24.dist-info/RECORD,,
+ar_ex_sys_worker-1.6.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.6.3.dist-info/METADATA,sha256=pleGVL03mPwSHsr1l4t3G4s2KOCVyaIf7reXRXYlgSc,343
+ar_ex_sys_worker-1.6.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_ex_sys_worker-1.6.3.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.6.3.dist-info/RECORD,,
```

