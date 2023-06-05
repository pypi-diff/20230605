# Comparing `tmp/ar_ex_sys_worker-1.6.32-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.33-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16333 bytes, number of entries: 11
+Zip file size: 16330 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    29391 b- defN 23-Jun-05 08:45 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19943 b- defN 23-Jun-05 08:45 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    29452 b- defN 23-Jun-05 10:29 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19901 b- defN 23-Jun-05 10:30 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Jun-05 08:49 ar_ex_sys_worker-1.6.32.dist-info/RECORD
-11 files, 64210 bytes uncompressed, 14617 bytes compressed:  77.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/RECORD
+11 files, 64229 bytes uncompressed, 14614 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.32.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.33.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.32.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.33.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.32.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.33.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.32.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.33.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.32.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -488,15 +488,16 @@
             return
         if signal_id.strip() == 'this carrier was not found':
             self.delete_act_from_send_reports(record_id)
             return {'error': {f'Act has not been delivered cos {signal_id}. '
                               f'Deleted from log...'}}
         if not self.is_valid_uuid(signal_id):
             return {'error': f'act not found in signall_id ({signal_id})'}
-        self.delete_act(signal_id)
+        self.delete_act_from_send_reports(record_id)
+        return self.delete_act(signal_id)
 
     def act_update_work(self, record_id, car_number, transporter_inn,
                         trash_cat,
                         trash_type, comment):
         signal_id = self.extract_act_ex_id(record_id)
         if not signal_id:
             return
```

## ar_external_sys_worker/mixins.py

```diff
@@ -219,15 +219,14 @@
 class SignallGetCarriersPO:
     headers = None
     get_carriers_po_link = None
 
     def get_carriers_po(self):
         if not self.get_carriers_po_link:
             return {'error': 'There are not link for route get_carriers'}
-        print(self.get_carriers_po_link)
         response = requests.get(self.get_carriers_po_link,
                                 headers=self.headers)
         return response
 
 
 class SignAllCarsGetter:
     headers = None
```

## Comparing `ar_ex_sys_worker-1.6.32.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.33.dist-info/LICENSE`

 * *Files identical despite different names*

