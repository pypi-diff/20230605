# Comparing `tmp/ar_ex_sys_worker-1.6.31-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16332 bytes, number of entries: 11
+Zip file size: 16333 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    28877 b- defN 23-Jun-05 08:37 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19993 b- defN 23-Jun-05 08:37 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    29391 b- defN 23-Jun-05 08:45 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19943 b- defN 23-Jun-05 08:45 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 08:38 ar_ex_sys_worker-1.6.31.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Jun-05 08:38 ar_ex_sys_worker-1.6.31.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 08:38 ar_ex_sys_worker-1.6.31.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 08:38 ar_ex_sys_worker-1.6.31.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Jun-05 08:38 ar_ex_sys_worker-1.6.31.dist-info/RECORD
-11 files, 63746 bytes uncompressed, 14616 bytes compressed:  77.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/RECORD
+11 files, 64210 bytes uncompressed, 14617 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.31.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.32.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.31.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.32.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.31.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.32.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.31.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.32.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.31.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -451,15 +451,16 @@
                            'package': act['package_name']},
         }
         act_json = json.dumps(data)
         return act_json
 
 
 class SignAllActsWorkerToken(mixins.TokenAuth, SignallActWorker,
-                             mixins.TokenDBAuth, mixins.SignallActDBDeletter,
+                             mixins.TokenDBAuth,
+                             mixins.SignallActDBDeletter,
                              mixins.ExSysActIdExtractor,
                              mixins.SignallActUpdater,
                              mixins.SignallActDeletter):
     def __init__(self, sql_shell, trash_cats_list, time_start, platform_id,
                  acts_limit=5, gravity_ip=None, gravity_port=8080, test=False,
                  mutex=None):
         super().__init__(sql_shell, trash_cats_list, time_start, acts_limit,
@@ -477,14 +478,26 @@
             self.link_host = 'https://signalltestdev.qodex.tech'
         self.signall_update_act_link = self.get_full_endpoint(
                 '/v1/gravity/update_act/{}')
         self.signal_del_act_url = self.get_full_endpoint(
             "/v1/acts/delete_act_by_id/{}"
         )
 
+    def del_act(self, record_id):
+        signal_id = self.extract_act_ex_id(record_id)
+        if not signal_id:
+            return
+        if signal_id.strip() == 'this carrier was not found':
+            self.delete_act_from_send_reports(record_id)
+            return {'error': {f'Act has not been delivered cos {signal_id}. '
+                              f'Deleted from log...'}}
+        if not self.is_valid_uuid(signal_id):
+            return {'error': f'act not found in signall_id ({signal_id})'}
+        self.delete_act(signal_id)
+
     def act_update_work(self, record_id, car_number, transporter_inn,
                         trash_cat,
                         trash_type, comment):
         signal_id = self.extract_act_ex_id(record_id)
         if not signal_id:
             return
         if signal_id.strip() == 'this carrier was not found':
@@ -571,15 +584,14 @@
                  **kwargs):
         self.sql_shell = sql_shell
         self.login = login
         self.password = password
         if test:
             self.link_host = 'https://signalltestdev.qodex.tech'
         self.headers = self.get_headers()
-        self.working_link = self.get_full_endpoint(self.del_act_url)
 
     def work(self, act_number):
         print(f"DEL ACT #{act_number}")
         response = self.delete_act(act_number)
         print(f"SIGNALL RESULT:{response.json()}")
         response = self.delete_act_from_send_reports(act_number)
         print(f"DB RESULT:{response}")
```

## ar_external_sys_worker/mixins.py

```diff
@@ -179,15 +179,14 @@
             "transporter_name": "",
             "waste_category": 'tko'
 
         }
 
 
 class SignallActDeletter:
-    del_act_url = '/v1/acts/delete_act_by_id/{}'
     headers = None
     working_link = None
     signal_del_act_url = None
 
     def delete_act(self, signall_act_id):
         return requests.delete(self.signal_del_act_url.format(signall_act_id),
                                headers=self.headers)
```

## Comparing `ar_ex_sys_worker-1.6.31.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.32.dist-info/LICENSE`

 * *Files identical despite different names*

