# Comparing `tmp/gensp-0.0.1-py3.10.egg` & `tmp/gensp-1.0.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,21 +1,19 @@
-Zip file size: 9700 bytes, number of entries: 19
--rw-r--r--  2.0 unx      432 b- defN 23-Jun-03 17:39 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      396 b- defN 23-Jun-03 17:39 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-03 17:39 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-03 17:39 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-03 17:39 EGG-INFO/not-zip-safe
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-03 17:39 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-03 17:39 EGG-INFO/top_level.txt
+Zip file size: 10584 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     1258 b- defN 23-Jun-05 11:03 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      364 b- defN 23-Jun-05 11:03 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 11:03 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 11:03 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 11:03 EGG-INFO/not-zip-safe
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 11:03 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-05 11:03 EGG-INFO/top_level.txt
 -rw-r--r--  2.0 unx       48 b- defN 23-Jun-03 17:32 generateStoredProcedure/__init__.py
--rw-r--r--  2.0 unx     1452 b- defN 23-Jun-03 17:24 generateStoredProcedure/backup.py
--rw-r--r--  2.0 unx     1592 b- defN 23-Jun-03 17:24 generateStoredProcedure/compare.py
--rw-r--r--  2.0 unx      632 b- defN 23-Jun-03 14:35 generateStoredProcedure/login.py
--rw-r--r--  2.0 unx     1464 b- defN 23-Jun-03 17:31 generateStoredProcedure/main.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-03 16:59 generateStoredProcedure/test.py
--rw-r--r--  2.0 unx      286 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1468 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/backup.cpython-310.pyc
--rw-r--r--  2.0 unx     1818 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/compare.cpython-310.pyc
--rw-r--r--  2.0 unx      829 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/login.cpython-310.pyc
--rw-r--r--  2.0 unx     1374 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/main.cpython-310.pyc
--rw-r--r--  2.0 unx      213 b- defN 23-Jun-03 17:39 generateStoredProcedure/__pycache__/test.cpython-310.pyc
-19 files, 12167 bytes uncompressed, 6840 bytes compressed:  43.8%
+-rw-r--r--  2.0 unx     1739 b- defN 23-Jun-05 09:40 generateStoredProcedure/backup.py
+-rw-r--r--  2.0 unx     1902 b- defN 23-Jun-05 10:50 generateStoredProcedure/compare.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-05 11:01 generateStoredProcedure/login.py
+-rw-r--r--  2.0 unx     1995 b- defN 23-Jun-05 10:56 generateStoredProcedure/main.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jun-05 11:03 generateStoredProcedure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1605 b- defN 23-Jun-05 11:03 generateStoredProcedure/__pycache__/backup.cpython-310.pyc
+-rw-r--r--  2.0 unx     2144 b- defN 23-Jun-05 11:03 generateStoredProcedure/__pycache__/compare.cpython-310.pyc
+-rw-r--r--  2.0 unx      830 b- defN 23-Jun-05 11:03 generateStoredProcedure/__pycache__/login.cpython-310.pyc
+-rw-r--r--  2.0 unx     1806 b- defN 23-Jun-05 11:03 generateStoredProcedure/__pycache__/main.cpython-310.pyc
+17 files, 14722 bytes uncompressed, 8050 bytes compressed:  45.3%
```

## zipnote «TEMP»/diffoscope_f3pq5tbg_/tmpdm1m5_p9_.zip

```diff
@@ -30,17 +30,14 @@
 
 Filename: generateStoredProcedure/login.py
 Comment: 
 
 Filename: generateStoredProcedure/main.py
 Comment: 
 
-Filename: generateStoredProcedure/test.py
-Comment: 
-
 Filename: generateStoredProcedure/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
 Filename: generateStoredProcedure/__pycache__/backup.cpython-310.pyc
 Comment: 
 
 Filename: generateStoredProcedure/__pycache__/compare.cpython-310.pyc
@@ -48,11 +45,8 @@
 
 Filename: generateStoredProcedure/__pycache__/login.cpython-310.pyc
 Comment: 
 
 Filename: generateStoredProcedure/__pycache__/main.cpython-310.pyc
 Comment: 
 
-Filename: generateStoredProcedure/__pycache__/test.cpython-310.pyc
-Comment: 
-
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,12 +1,43 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 0.0.1
+Version: 1.0.0
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gsp
 Author: byte
 Author-email: liufangjing_byte@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# gensp
+
+[![Coverage Status](https://coveralls.io/repos/github/yourusername/yourproject/badge.svg?branch=master)](https://github.com/zerobyte1o1/gensp?branch=main)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+> 比对postgres数据库备份的数据，得出新增的存储过程，目前不支持更新和删除，所有数据库备份区别都以新增的格式输出成存储过程。
+
+## Installation
+
+```
+pip install gensp
+```
+
+## Usage example
+
+```
+gensp help          # 帮助
+gensp login         # 配置数据库链接信息
+gensp backup        # 备份数据库
+gensp compare       # 比较两次数据库备份，并生成存储过程
+gensp clear         # 清理本地数据库备份
+```
+
+
+## Release History
+
+* v0.0.1
+    * ADD: Initial version
+
+#
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.py
 generateStoredProcedure/__init__.py
 generateStoredProcedure/backup.py
 generateStoredProcedure/compare.py
 generateStoredProcedure/login.py
 generateStoredProcedure/main.py
-generateStoredProcedure/test.py
 gensp.egg-info/PKG-INFO
 gensp.egg-info/SOURCES.txt
 gensp.egg-info/dependency_links.txt
 gensp.egg-info/entry_points.txt
 gensp.egg-info/requires.txt
 gensp.egg-info/top_level.txt
```

## generateStoredProcedure/backup.py

```diff
@@ -1,51 +1,60 @@
 import time
 import psycopg2
 import os
 import yaml
-# 数据库连接字符串
 
 
+# 数据库连接字符串
 def conn_postgres(database):
     rootPath = os.path.dirname(os.path.abspath(__file__))
     configPath = os.path.join(rootPath, "env.yaml")
     env = yaml.safe_load(open(configPath))
     try:
         conn = psycopg2.connect(
             host=env["login"]["host"],
             port=env["login"]["port"],
             database=database,
             user=env["login"]["user"],
             password=env["login"]["password"]
         )
     except psycopg2.Error as e:
-        print("Warning: Failed to connect to database.\nError message: ",e)
+        print("Warning: Failed to connect to database.\nError message: ", e)
         conn = None
     return conn
 
+
 def get_backup(database):
-# 获取数据库中的所有表
-    conn=conn_postgres(database)
+    # 获取数据库中的所有表
+    conn = conn_postgres(database)
     if conn is None:
         return
     cur = conn.cursor()
-    cur.execute("SELECT table_name FROM information_schema.tables WHERE table_schema='public' AND table_type='BASE TABLE'")
+    cur.execute(
+        "SELECT table_name FROM information_schema.tables WHERE table_schema='public' AND table_type='BASE TABLE'")
     table_names = cur.fetchall()
     cur.close()
-    print(table_names)
     # 创建备份文件名
-    backup_file_name = 'backup_' + str(int(time.time()*1000)) + '.sql'
+    backup_file_name = 'backup_' + str(int(time.time() * 1000)) + '.sql'
 
     # 将每个表备份到备份文件中
     cur = conn.cursor()
     with open(backup_file_name, 'w') as backup_file:
         for table in table_names:
-            cur.copy_to(backup_file, table[0], sep='|')
+            cur.execute("SELECT * FROM " + table[0])
+            rows = cur.fetchall()
+            for row in rows:
+                backup_file.write(table[0] + '|' + '|'.join(map(str, row)) + '\n')
+
+    # 需要修改成提张表存入一个文件下，从而降低时间复杂度。
+
+
     conn.commit()
     cur.close()
 
     # 关闭数据库连接
     conn.close()
+    print('\033[32m·\033[0m生成备份成功: ' + database)
 
 
 if __name__ == '__main__':
-    conn_postgres("teamtest_scm")
+    get_backup("teamtest_scm")
```

## generateStoredProcedure/compare.py

```diff
@@ -1,60 +1,62 @@
-
 import difflib
 import os
 
+
 def compare_files(file1, file2):
     with open(file1, 'r') as f1, open(file2, 'r') as f2:
         diff = difflib.unified_diff(f1.readlines(), f2.readlines())
         return ''.join(diff)
 
+
 def generate_procedure(file1, file2):
     diff = compare_files(file1, file2)
     lines = diff.split('\n')
     insert_lines = []
     delete_lines = []
-    insert_query=[]
-    delete_query=[]
+    insert_query = []
+    delete_query = []
     for line in lines:
-        # print(line+"\n")
         if line.startswith('+'):
             insert_lines.append(line[1:])
         elif line.startswith('-'):
             delete_lines.append(line[1:])
     for insert_line in insert_lines[1:]:
         values = insert_line.split('|')
-        for i in range(len(values)):
-            if isinstance(values[i], str):
-                values[i] = "'{}'".format(values[i])
-        insert_query.append('INSERT INTO table_name VALUES ({})'.format(', '.join(values)))
+        values2=values[1:]
+        for i in range(len(values2)):
+            if isinstance(values2[i], str):
+                values2[i] = "'{}'".format(values2[i])
+        insert_query.append('INSERT INTO {} VALUES ({})'.format(values[0],', '.join(values2)))
 
     # 删除先不写了，用不上
     procedure = '''\
-CREATE OR REPLACE FUNCTION restore_backup()
-RETURNS void AS $$
+CREATE OR REPLACE FUNCTION restore_backup(numbegin NUMERIC,numend NUMERIC)
+RETURNS NUMERIC AS $$
+DECLARE a int DEFAULT 1;
+DECLARE
 BEGIN
-    {};
+    a:=numbegin;
+    while a < numend LOOP
+        {};
+        a = a + 1 ;
+    END LOOP;
 END;
 $$ LANGUAGE plpgsql;
-'''.format(';\n    '.join(insert_query))
+SELECT restore_backup(0,2);
+'''.format(';\n        '.join(insert_query))
     with open('restore_backup.sql', 'w') as f:
         f.write(procedure)
     return procedure
 
+
 def run_compare():
     backup_files = [f for f in os.listdir('.') if f.startswith('backup_')]
+    if len(backup_files) < 2:
+        print('\033[33m·\033[0m数据库备份数量不够2个，请先gensp backup备份数据库')
     file1 = backup_files[0]
     file2 = backup_files[1]
     # 比较时间戳
     if int(file1.split('_')[1].split('.')[0]) > int(file2.split('_')[1].split('.')[0]):
         file1, file2 = file2, file1
     procedure = generate_procedure(file1, file2)
-    print(procedure)
-
-
-    
- 
-
-
-
-
-
+    print(procedure)
```

## generateStoredProcedure/login.py

```diff
@@ -1,23 +1,22 @@
- 
 import yaml
 from backup import conn_postgres
 
+
 def login():
     with open('env.yaml', 'r') as f:
         env = yaml.safe_load(f)
     host = input('\033[34m·\033[0mhost: ').strip()
     port = input('\033[34m·\033[0mport: ').strip()
     username = input('\033[34m·\033[0musername: ').strip()
     password = input('\033[34m·\033[0mpassword: ').strip()
     env['login']['host'] = host
     env['login']['port'] = port
-    env['login']['username'] = username
+    env['login']['user'] = username
     env['login']['password'] = password
     with open('env.yaml', 'w') as f:
         yaml.dump(env, f)
     conn_postgres('postgres')
 
 
 if __name__ == '__main__':
-
-    login()
+    login()
```

## generateStoredProcedure/main.py

```diff
@@ -1,42 +1,53 @@
- 
 import sys
 from login import login
 from backup import get_backup
 from compare import run_compare
 import os
+
+
 def main():
     if len(sys.argv) == 2:
         if sys.argv[1] == 'login':
             login()
         elif sys.argv[1] == 'backup':
             file_number = 0
             for file in os.listdir():
                 if file.startswith('backup_') and file.endswith('.sql'):
                     file_number += 1
-            print('\033[32m·\033[0m已存在备份数量: '+str(file_number))
+            print('\033[32m·\033[0m已存在备份数量: ' + str(file_number))
             if file_number >= 2:
                 print('\033[33m·\033[0m备份数量已满，请执行gsp compare生成存储过程，或执行gsp clear清空备份')
                 sys.exit()
-            database_name=input('\033[34m·\033[0mdatabase: ').strip()
+            database_name = input('\033[34m·\033[0mdatabase: ').strip()
+            print('\033[32m·\033[0m备份中……')
             get_backup(database_name)
         elif sys.argv[1] == 'compare':
             print('\033[32m·\033[0m生成存储过程如下: ')
             run_compare()
         elif sys.argv[1] == 'clear':
             for file in os.listdir():
                 if file.startswith('backup_') and file.endswith('.sql'):
                     os.remove(file)
             print('\033[32m·\033[0mcompleted!')
+        elif sys.argv[1] == 'help':
+            print('\033[32m·\033[0m参数介绍：')
+            print('\033[32m·\033[0mlogin：注册数据库基本信息')
+            print('\033[32m·\033[0mbackup：备份数据库')
+            print('\033[32m·\033[0mcompare：比较备份并生成存储过程')
+            print('\033[32m·\033[0mclear：清除本地数据库备份')
+            print('\033[32m·\033[0mhelp：帮助')
         elif sys.argv[1] == 'lasttime':
             with open('restore_backup.sql', 'r') as f:
                 content = f.read()
                 print(content)
 
 
 
         else:
             print("\033[31m·\033Invalid argument")
     else:
         print("\033[31m·\033Invalid number of arguments")
 
 
+if __name__ == '__main__':
+    main()
```

## generateStoredProcedure/__pycache__/backup.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun  3 09:24:31 2023 UTC, .py size: 1452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,14 +1,14 @@
-00000000: 6f0d 0d0a 0000 0000 cf06 7b64 ac05 0000  o.........{d....
+00000000: 6f0d 0d0a 0000 0000 273d 7d64 cb06 0000  o.......'=}d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 8400 5a04 6404 6405 8400 5a05 6506  d...Z.d.d...Z.e.
-00000060: 6406 6b02 7222 6504 6407 8301 0100 6401  d.k.r"e.d.....d.
+00000060: 6406 6b02 7222 6505 6407 8301 0100 6401  d.k.r"e.d.....d.
 00000070: 5300 6401 5300 2908 e900 0000 004e 6301  S.d.S.)......Nc.
 00000080: 0000 0000 0000 0000 0000 0006 0000 000a  ................
 00000090: 0000 0043 0000 0073 a200 0000 7400 6a01  ...C...s....t.j.
 000000a0: a002 7400 6a01 a003 7404 a101 a101 7d01  ..t.j...t.....}.
 000000b0: 7400 6a01 a005 7c01 6401 a102 7d02 7406  t.j...|.d...}.t.
 000000c0: a007 7408 7c02 8301 a101 7d03 7a1d 7409  ..t.|.....}.z.t.
 000000d0: 6a0a 7c03 6402 1900 6403 1900 7c03 6402  j.|.d...d...|.d.
@@ -41,52 +41,61 @@
 00000280: 6767 2f67 656e 6572 6174 6553 746f 7265  gg/generateStore
 00000290: 6450 726f 6365 6475 7265 2f62 6163 6b75  dProcedure/backu
 000002a0: 702e 7079 da0d 636f 6e6e 5f70 6f73 7467  p.py..conn_postg
 000002b0: 7265 7308 0000 0073 2400 0000 1401 0e01  res....s$.......
 000002c0: 0e01 0201 0401 0a01 0a01 0201 0a01 0a01  ................
 000002d0: 08fb 040a 10fd 0a01 0e01 0401 0880 02fd  ................
 000002e0: 7219 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000002f0: 0000 0700 0000 0800 0000 4300 0000 73c6  ..........C...s.
-00000300: 0000 0074 007c 0083 017d 017c 0164 0075  ...t.|...}.|.d.u
+000002f0: 0000 0900 0000 0b00 0000 4300 0000 7300  ..........C...s.
+00000300: 0100 0074 007c 0083 017d 017c 0164 0075  ...t.|...}.|.d.u
 00000310: 0072 0a64 0053 007c 01a0 01a1 007d 027c  .r.d.S.|.....}.|
 00000320: 02a0 0264 01a1 0101 007c 02a0 03a1 007d  ...d.....|.....}
-00000330: 037c 02a0 04a1 0001 0074 057c 0383 0101  .|.......t.|....
-00000340: 0064 0274 0674 0774 08a0 08a1 0064 0314  .d.t.t.t.....d..
-00000350: 0083 0183 0117 0064 0417 007d 047c 01a0  .......d...}.|..
-00000360: 01a1 007d 0274 097c 0464 0583 028f 177d  ...}.t.|.d.....}
-00000370: 057c 0344 005d 0c7d 067c 026a 0a7c 057c  .|.D.].}.|.j.|.|
-00000380: 0664 0619 0064 0764 088d 0301 0071 3957  .d...d.d.....q9W
-00000390: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-000003a0: 5077 0101 0001 0001 0059 0001 007c 01a0  Pw.......Y...|..
-000003b0: 0ba1 0001 007c 02a0 04a1 0001 007c 01a0  .....|.......|..
-000003c0: 04a1 0001 0064 0053 0029 094e 7a68 5345  .....d.S.).NzhSE
-000003d0: 4c45 4354 2074 6162 6c65 5f6e 616d 6520  LECT table_name 
-000003e0: 4652 4f4d 2069 6e66 6f72 6d61 7469 6f6e  FROM information
-000003f0: 5f73 6368 656d 612e 7461 626c 6573 2057  _schema.tables W
-00000400: 4845 5245 2074 6162 6c65 5f73 6368 656d  HERE table_schem
-00000410: 613d 2770 7562 6c69 6327 2041 4e44 2074  a='public' AND t
-00000420: 6162 6c65 5f74 7970 653d 2742 4153 4520  able_type='BASE 
-00000430: 5441 424c 4527 5a07 6261 636b 7570 5f69  TABLE'Z.backup_i
-00000440: e803 0000 7a04 2e73 716c da01 7772 0100  ....z..sql..wr..
-00000450: 0000 fa01 7c29 01da 0373 6570 290c 7219  ....|)...sep).r.
-00000460: 0000 005a 0663 7572 736f 72da 0765 7865  ...Z.cursor..exe
-00000470: 6375 7465 5a08 6665 7463 6861 6c6c da05  cuteZ.fetchall..
-00000480: 636c 6f73 6572 1300 0000 da03 7374 72da  closer......str.
-00000490: 0369 6e74 da04 7469 6d65 720f 0000 005a  .int..timer....Z
-000004a0: 0763 6f70 795f 746f 5a06 636f 6d6d 6974  .copy_toZ.commit
-000004b0: 2907 7207 0000 0072 1500 0000 da03 6375  ).r....r......cu
-000004c0: 725a 0b74 6162 6c65 5f6e 616d 6573 5a10  rZ.table_namesZ.
-000004d0: 6261 636b 7570 5f66 696c 655f 6e61 6d65  backup_file_name
-000004e0: 5a0b 6261 636b 7570 5f66 696c 65da 0574  Z.backup_file..t
-000004f0: 6162 6c65 7217 0000 0072 1700 0000 7218  abler....r....r.
-00000500: 0000 00da 0a67 6574 5f62 6163 6b75 7019  .....get_backup.
-00000510: 0000 0073 2400 0000 0802 0801 0401 0801  ...s$...........
-00000520: 0a01 0801 0801 0801 1c02 0803 0c01 0801  ................
-00000530: 1601 02ff 1cff 0803 0801 0c03 7224 0000  ............r$..
-00000540: 00da 085f 5f6d 6169 6e5f 5f5a 0c74 6561  ...__main__Z.tea
-00000550: 6d74 6573 745f 7363 6d29 0772 2100 0000  mtest_scm).r!...
-00000560: 7210 0000 0072 0800 0000 720e 0000 0072  r....r....r....r
-00000570: 1900 0000 7224 0000 00da 085f 5f6e 616d  ....r$.....__nam
-00000580: 655f 5f72 1700 0000 7217 0000 0072 1700  e__r....r....r..
-00000590: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000005a0: 3e01 0000 0073 1200 0000 0800 0801 0801  >....s..........
-000005b0: 0801 0804 0811 0819 0c01 04ff            ............
+00000330: 037c 02a0 04a1 0001 0064 0274 0574 0674  .|.......d.t.t.t
+00000340: 07a0 07a1 0064 0314 0083 0183 0117 0064  .....d.........d
+00000350: 0417 007d 047c 01a0 01a1 007d 0274 087c  ...}.|.....}.t.|
+00000360: 0464 0583 028f 327d 057c 0344 005d 277d  .d....2}.|.D.]'}
+00000370: 067c 02a0 0264 067c 0664 0719 0017 00a1  .|...d.|.d......
+00000380: 0101 007c 02a0 03a1 007d 077c 0744 005d  ...|.....}.|.D.]
+00000390: 157d 087c 05a0 097c 0664 0719 0064 0817  .}.|...|.d...d..
+000003a0: 0064 08a0 0a74 0b74 057c 0883 02a1 0117  .d...t.t.|......
+000003b0: 0064 0917 00a1 0101 0071 4671 3557 0064  .d.......qFq5W.d
+000003c0: 0004 0004 0083 0301 006e 0831 0073 6777  .........n.1.sgw
+000003d0: 0101 0001 0001 0059 0001 007c 01a0 0ca1  .......Y...|....
+000003e0: 0001 007c 02a0 04a1 0001 007c 01a0 04a1  ...|.......|....
+000003f0: 0001 0074 0d64 0a7c 0017 0083 0101 0064  ...t.d.|.......d
+00000400: 0053 0029 0b4e 7a68 5345 4c45 4354 2074  .S.).NzhSELECT t
+00000410: 6162 6c65 5f6e 616d 6520 4652 4f4d 2069  able_name FROM i
+00000420: 6e66 6f72 6d61 7469 6f6e 5f73 6368 656d  nformation_schem
+00000430: 612e 7461 626c 6573 2057 4845 5245 2074  a.tables WHERE t
+00000440: 6162 6c65 5f73 6368 656d 613d 2770 7562  able_schema='pub
+00000450: 6c69 6327 2041 4e44 2074 6162 6c65 5f74  lic' AND table_t
+00000460: 7970 653d 2742 4153 4520 5441 424c 4527  ype='BASE TABLE'
+00000470: 5a07 6261 636b 7570 5f69 e803 0000 7a04  Z.backup_i....z.
+00000480: 2e73 716c da01 777a 0e53 454c 4543 5420  .sql..wz.SELECT 
+00000490: 2a20 4652 4f4d 2072 0100 0000 fa01 7cda  * FROM r......|.
+000004a0: 010a 751f 0000 001b 5b33 326d c2b7 1b5b  ..u.....[32m...[
+000004b0: 306d e794 9fe6 8890 e5a4 87e4 bbbd e688  0m..............
+000004c0: 90e5 8a9f 3a20 290e 7219 0000 005a 0663  ....: ).r....Z.c
+000004d0: 7572 736f 72da 0765 7865 6375 7465 5a08  ursor..executeZ.
+000004e0: 6665 7463 6861 6c6c da05 636c 6f73 65da  fetchall..close.
+000004f0: 0373 7472 da03 696e 74da 0474 696d 6572  .str..int..timer
+00000500: 0f00 0000 da05 7772 6974 6572 0d00 0000  ......writer....
+00000510: da03 6d61 705a 0663 6f6d 6d69 7472 1300  ..mapZ.commitr..
+00000520: 0000 2909 7207 0000 0072 1500 0000 da03  ..).r....r......
+00000530: 6375 725a 0b74 6162 6c65 5f6e 616d 6573  curZ.table_names
+00000540: 5a10 6261 636b 7570 5f66 696c 655f 6e61  Z.backup_file_na
+00000550: 6d65 5a0b 6261 636b 7570 5f66 696c 65da  meZ.backup_file.
+00000560: 0574 6162 6c65 5a04 726f 7773 da03 726f  .tableZ.rows..ro
+00000570: 7772 1700 0000 7217 0000 0072 1800 0000  wr....r....r....
+00000580: da0a 6765 745f 6261 636b 7570 1a00 0000  ..get_backup....
+00000590: 7330 0000 0008 0208 0104 0108 0104 0102  s0..............
+000005a0: 0104 ff08 0208 011c 0208 030c 0108 0112  ................
+000005b0: 0108 0108 0128 0102 ff02 fd1c ff08 0a08  .....(..........
+000005c0: 0108 0310 0172 2700 0000 da08 5f5f 6d61  .....r'.....__ma
+000005d0: 696e 5f5f 5a0c 7465 616d 7465 7374 5f73  in__Z.teamtest_s
+000005e0: 636d 2907 7221 0000 0072 1000 0000 7208  cm).r!...r....r.
+000005f0: 0000 0072 0e00 0000 7219 0000 0072 2700  ...r....r....r'.
+00000600: 0000 da08 5f5f 6e61 6d65 5f5f 7217 0000  ....__name__r...
+00000610: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000620: da08 3c6d 6f64 756c 653e 0100 0000 7312  ..<module>....s.
+00000630: 0000 0008 0008 0108 0108 0108 0408 1208  ................
+00000640: 210c 0104 ff                             !....
```

## generateStoredProcedure/__pycache__/compare.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun  3 09:24:41 2023 UTC, .py size: 1592 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d906 7b64 3806 0000  o.........{d8...
+00000000: 6f0d 0d0a 0000 0000 724d 7d64 6e07 0000  o.......rM}dn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6404 6405 8400 5a03 6406  d...Z.d.d...Z.d.
 00000050: 6407 8400 5a04 6401 5300 2908 e900 0000  d...Z.d.S.).....
 00000060: 004e 6302 0000 0000 0000 0000 0000 0005  .Nc.............
 00000070: 0000 0009 0000 0043 0000 0073 8600 0000  .......C...s....
@@ -23,92 +23,112 @@
 00000160: 0000 00fa 4462 7569 6c64 2f62 6469 7374  ....Dbuild/bdist
 00000170: 2e6d 6163 6f73 782d 3133 2e32 2d61 726d  .macosx-13.2-arm
 00000180: 3634 2f65 6767 2f67 656e 6572 6174 6553  64/egg/generateS
 00000190: 746f 7265 6450 726f 6365 6475 7265 2f63  toredProcedure/c
 000001a0: 6f6d 7061 7265 2e70 79da 0d63 6f6d 7061  ompare.py..compa
 000001b0: 7265 5f66 696c 6573 0500 0000 7308 0000  re_files....s...
 000001c0: 0018 0114 0108 0152 fe72 0f00 0000 6302  .......R.r....c.
-000001d0: 0000 0000 0000 0000 0000 000e 0000 0008  ................
-000001e0: 0000 0043 0000 0073 1601 0000 7400 7c00  ...C...s....t.|.
+000001d0: 0000 0000 0000 0000 0000 000f 0000 0009  ................
+000001e0: 0000 0043 0000 0073 2801 0000 7400 7c00  ...C...s(...t.|.
 000001f0: 7c01 8302 7d02 7c02 a001 6401 a101 7d03  |...}.|...d...}.
 00000200: 6700 7d04 6700 7d05 6700 7d06 6700 7d07  g.}.g.}.g.}.g.}.
 00000210: 7c03 4400 5d1f 7d08 7c08 a002 6402 a101  |.D.].}.|...d...
 00000220: 7225 7c04 a003 7c08 6403 6400 8502 1900  r%|...|.d.d.....
 00000230: a101 0100 7114 7c08 a002 6404 a101 7233  ....q.|...d...r3
 00000240: 7c05 a003 7c08 6403 6400 8502 1900 a101  |...|.d.d.......
 00000250: 0100 7114 7c04 6403 6400 8502 1900 4400  ..q.|.d.d.....D.
-00000260: 5d2b 7d09 7c09 a001 6405 a101 7d0a 7404  ]+}.|...d...}.t.
-00000270: 7405 7c0a 8301 8301 4400 5d12 7d0b 7406  t.|.....D.].}.t.
-00000280: 7c0a 7c0b 1900 7407 8302 7259 6406 a008  |.|...t...rYd...
-00000290: 7c0a 7c0b 1900 a101 7c0a 7c0b 3c00 7147  |.|.....|.|.<.qG
-000002a0: 7c06 a003 6407 a008 6408 a009 7c0a a101  |...d...d...|...
-000002b0: a101 a101 0100 713a 6409 a008 640a a009  ......q:d...d...
-000002c0: 7c06 a101 a101 7d0c 740a 640b 640c 8302  |.....}.t.d.d...
-000002d0: 8f0e 7d0d 7c0d a00b 7c0c a101 0100 5700  ..}.|...|.....W.
-000002e0: 6400 0400 0400 8303 0100 7c0c 5300 3100  d.........|.S.1.
-000002f0: 7384 7701 0100 0100 0100 5900 0100 7c0c  s.w.......Y...|.
-00000300: 5300 290d 4eda 010a fa01 2be9 0100 0000  S.).N.....+.....
-00000310: fa01 2dfa 017c 7a04 277b 7d27 7a22 494e  ..-..|z.'{}'z"IN
-00000320: 5345 5254 2049 4e54 4f20 7461 626c 655f  SERT INTO table_
-00000330: 6e61 6d65 2056 414c 5545 5320 287b 7d29  name VALUES ({})
-00000340: 7a02 2c20 7a67 4352 4541 5445 204f 5220  z., zgCREATE OR 
-00000350: 5245 504c 4143 4520 4655 4e43 5449 4f4e  REPLACE FUNCTION
-00000360: 2072 6573 746f 7265 5f62 6163 6b75 7028   restore_backup(
-00000370: 290a 5245 5455 524e 5320 766f 6964 2041  ).RETURNS void A
-00000380: 5320 2424 0a42 4547 494e 0a20 2020 207b  S $$.BEGIN.    {
-00000390: 7d3b 0a45 4e44 3b0a 2424 204c 414e 4755  };.END;.$$ LANGU
-000003a0: 4147 4520 706c 7067 7371 6c3b 0a7a 063b  AGE plpgsql;.z.;
-000003b0: 0a20 2020 207a 1272 6573 746f 7265 5f62  .    z.restore_b
-000003c0: 6163 6b75 702e 7371 6cda 0177 290c 720f  ackup.sql..w).r.
-000003d0: 0000 00da 0573 706c 6974 da0a 7374 6172  .....split..star
-000003e0: 7473 7769 7468 da06 6170 7065 6e64 da05  tswith..append..
-000003f0: 7261 6e67 65da 036c 656e da0a 6973 696e  range..len..isin
-00000400: 7374 616e 6365 da03 7374 72da 0666 6f72  stance..str..for
-00000410: 6d61 7472 0700 0000 7204 0000 00da 0577  matr....r......w
-00000420: 7269 7465 290e 7208 0000 0072 0900 0000  rite).r....r....
-00000430: 720c 0000 00da 056c 696e 6573 5a0c 696e  r......linesZ.in
-00000440: 7365 7274 5f6c 696e 6573 5a0c 6465 6c65  sert_linesZ.dele
-00000450: 7465 5f6c 696e 6573 5a0c 696e 7365 7274  te_linesZ.insert
-00000460: 5f71 7565 7279 5a0c 6465 6c65 7465 5f71  _queryZ.delete_q
-00000470: 7565 7279 da04 6c69 6e65 5a0b 696e 7365  uery..lineZ.inse
-00000480: 7274 5f6c 696e 65da 0676 616c 7565 73da  rt_line..values.
-00000490: 0169 da09 7072 6f63 6564 7572 65da 0166  .i..procedure..f
-000004a0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-000004b0: 1267 656e 6572 6174 655f 7072 6f63 6564  .generate_proced
-000004c0: 7572 650a 0000 0073 3800 0000 0a01 0a01  ure....s8.......
-000004d0: 0401 0401 0401 0401 0801 0a02 1401 0a01  ................
-000004e0: 1201 0280 1001 0a01 1001 0e01 1201 0280  ................
-000004f0: 1801 0203 0c07 02f9 0c08 0c01 0aff 0402  ................
-00000500: 10fe 0402 7225 0000 0063 0000 0000 0000  ....r%...c......
-00000510: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00000520: 0000 737c 0000 0064 0164 0284 0074 00a0  ..s|...d.d...t..
-00000530: 0164 03a1 0144 0083 017d 007c 0064 0419  .d...D...}.|.d..
-00000540: 007d 017c 0064 0519 007d 0274 027c 01a0  .}.|.d...}.t.|..
-00000550: 0364 06a1 0164 0519 00a0 0364 03a1 0164  .d...d.....d...d
-00000560: 0419 0083 0174 027c 02a0 0364 06a1 0164  .....t.|...d...d
-00000570: 0519 00a0 0364 03a1 0164 0419 0083 016b  .....d...d.....k
-00000580: 0472 337c 027c 0102 027d 017d 0274 047c  .r3|.|...}.}.t.|
-00000590: 017c 0283 027d 0374 057c 0383 0101 0064  .|...}.t.|.....d
-000005a0: 0053 0029 074e 6301 0000 0000 0000 0000  .S.).Nc.........
-000005b0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-000005c0: 1a00 0000 6700 7c00 5d09 7d01 7c01 a000  ....g.|.].}.|...
-000005d0: 6400 a101 7202 7c01 9102 7102 5300 2901  d...r.|...q.S.).
-000005e0: 5a07 6261 636b 7570 5f29 0172 1700 0000  Z.backup_).r....
-000005f0: 2902 da02 2e30 7224 0000 0072 0d00 0000  )....0r$...r....
-00000600: 720d 0000 0072 0e00 0000 da0a 3c6c 6973  r....r......<lis
-00000610: 7463 6f6d 703e 2c00 0000 7302 0000 001a  tcomp>,...s.....
-00000620: 007a 1f72 756e 5f63 6f6d 7061 7265 2e3c  .z.run_compare.<
-00000630: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000640: 703e da01 2e72 0100 0000 7212 0000 00da  p>...r....r.....
-00000650: 015f 2906 da02 6f73 da07 6c69 7374 6469  ._)...os..listdi
-00000660: 72da 0369 6e74 7216 0000 0072 2500 0000  r..intr....r%...
-00000670: da05 7072 696e 7429 045a 0c62 6163 6b75  ..print).Z.backu
-00000680: 705f 6669 6c65 7372 0800 0000 7209 0000  p_filesr....r...
-00000690: 0072 2300 0000 720d 0000 0072 0d00 0000  .r#...r....r....
-000006a0: 720e 0000 00da 0b72 756e 5f63 6f6d 7061  r......run_compa
-000006b0: 7265 2b00 0000 730e 0000 0014 0108 0108  re+...s.........
-000006c0: 0138 020a 010a 010c 0172 2e00 0000 2905  .8.......r....).
-000006d0: 7205 0000 0072 2a00 0000 720f 0000 0072  r....r*...r....r
-000006e0: 2500 0000 722e 0000 0072 0d00 0000 720d  %...r....r....r.
-000006f0: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
-00000700: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
-00000710: 0801 0801 0802 0805 0c21                 .........!
+00000260: 5d34 7d09 7c09 a001 6405 a101 7d0a 7c0a  ]4}.|...d...}.|.
+00000270: 6403 6400 8502 1900 7d0b 7404 7405 7c0b  d.d.....}.t.t.|.
+00000280: 8301 8301 4400 5d12 7d0c 7406 7c0b 7c0c  ....D.].}.t.|.|.
+00000290: 1900 7407 8302 725f 6406 a008 7c0b 7c0c  ..t...r_d...|.|.
+000002a0: 1900 a101 7c0b 7c0c 3c00 714d 7c06 a003  ....|.|.<.qM|...
+000002b0: 6407 a008 7c0a 6408 1900 6409 a009 7c0b  d...|.d...d...|.
+000002c0: a101 a102 a101 0100 713a 640a a008 640b  ........q:d...d.
+000002d0: a009 7c06 a101 a101 7d0d 740a 640c 640d  ..|.....}.t.d.d.
+000002e0: 8302 8f0e 7d0e 7c0e a00b 7c0d a101 0100  ....}.|...|.....
+000002f0: 5700 6400 0400 0400 8303 0100 7c0d 5300  W.d.........|.S.
+00000300: 3100 738d 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00000310: 7c0d 5300 290e 4eda 010a fa01 2be9 0100  |.S.).N.....+...
+00000320: 0000 fa01 2dfa 017c 7a04 277b 7d27 7a1a  ....-..|z.'{}'z.
+00000330: 494e 5345 5254 2049 4e54 4f20 7b7d 2056  INSERT INTO {} V
+00000340: 414c 5545 5320 287b 7d29 7201 0000 007a  ALUES ({})r....z
+00000350: 022c 2061 1701 0000 4352 4541 5445 204f  ., a....CREATE O
+00000360: 5220 5245 504c 4143 4520 4655 4e43 5449  R REPLACE FUNCTI
+00000370: 4f4e 2072 6573 746f 7265 5f62 6163 6b75  ON restore_backu
+00000380: 7028 6e75 6d62 6567 696e 204e 554d 4552  p(numbegin NUMER
+00000390: 4943 2c6e 756d 656e 6420 4e55 4d45 5249  IC,numend NUMERI
+000003a0: 4329 0a52 4554 5552 4e53 204e 554d 4552  C).RETURNS NUMER
+000003b0: 4943 2041 5320 2424 0a44 4543 4c41 5245  IC AS $$.DECLARE
+000003c0: 2061 2069 6e74 2044 4546 4155 4c54 2031   a int DEFAULT 1
+000003d0: 3b0a 4445 434c 4152 450a 4245 4749 4e0a  ;.DECLARE.BEGIN.
+000003e0: 2020 2020 613a 3d6e 756d 6265 6769 6e3b      a:=numbegin;
+000003f0: 0a20 2020 2077 6869 6c65 2061 203c 206e  .    while a < n
+00000400: 756d 656e 6420 4c4f 4f50 0a20 2020 2020  umend LOOP.     
+00000410: 2020 207b 7d3b 0a20 2020 2020 2020 2061     {};.        a
+00000420: 203d 2061 202b 2031 203b 0a20 2020 2045   = a + 1 ;.    E
+00000430: 4e44 204c 4f4f 503b 0a45 4e44 3b0a 2424  ND LOOP;.END;.$$
+00000440: 204c 414e 4755 4147 4520 706c 7067 7371   LANGUAGE plpgsq
+00000450: 6c3b 0a53 454c 4543 5420 7265 7374 6f72  l;.SELECT restor
+00000460: 655f 6261 636b 7570 2830 2c32 293b 0a7a  e_backup(0,2);.z
+00000470: 0a3b 0a20 2020 2020 2020 207a 1272 6573  .;.        z.res
+00000480: 746f 7265 5f62 6163 6b75 702e 7371 6cda  tore_backup.sql.
+00000490: 0177 290c 720f 0000 00da 0573 706c 6974  .w).r......split
+000004a0: da0a 7374 6172 7473 7769 7468 da06 6170  ..startswith..ap
+000004b0: 7065 6e64 da05 7261 6e67 65da 036c 656e  pend..range..len
+000004c0: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
+000004d0: 72da 0666 6f72 6d61 7472 0700 0000 7204  r..formatr....r.
+000004e0: 0000 00da 0577 7269 7465 290f 7208 0000  .....write).r...
+000004f0: 0072 0900 0000 720c 0000 00da 056c 696e  .r....r......lin
+00000500: 6573 5a0c 696e 7365 7274 5f6c 696e 6573  esZ.insert_lines
+00000510: 5a0c 6465 6c65 7465 5f6c 696e 6573 5a0c  Z.delete_linesZ.
+00000520: 696e 7365 7274 5f71 7565 7279 5a0c 6465  insert_queryZ.de
+00000530: 6c65 7465 5f71 7565 7279 da04 6c69 6e65  lete_query..line
+00000540: 5a0b 696e 7365 7274 5f6c 696e 65da 0676  Z.insert_line..v
+00000550: 616c 7565 735a 0776 616c 7565 7332 da01  aluesZ.values2..
+00000560: 69da 0970 726f 6365 6475 7265 da01 6672  i..procedure..fr
+00000570: 0d00 0000 720d 0000 0072 0e00 0000 da12  ....r....r......
+00000580: 6765 6e65 7261 7465 5f70 726f 6365 6475  generate_procedu
+00000590: 7265 0b00 0000 733a 0000 000a 010a 0104  re....s:........
+000005a0: 0104 0104 0104 0108 010a 0114 010a 0112  ................
+000005b0: 0102 8010 010a 010c 0110 010e 0112 0102  ................
+000005c0: 801e 0102 030c 0e02 f20c 0f0c 010a ff04  ................
+000005d0: 0210 fe04 0272 2500 0000 6300 0000 0000  .....r%...c.....
+000005e0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+000005f0: 0000 0073 9000 0000 6401 6402 8400 7400  ...s....d.d...t.
+00000600: a001 6403 a101 4400 8301 7d00 7402 7c00  ..d...D...}.t.|.
+00000610: 8301 6404 6b00 7214 7403 6405 8301 0100  ..d.k.r.t.d.....
+00000620: 7c00 6406 1900 7d01 7c00 6407 1900 7d02  |.d...}.|.d...}.
+00000630: 7404 7c01 a005 6408 a101 6407 1900 a005  t.|...d...d.....
+00000640: 6403 a101 6406 1900 8301 7404 7c02 a005  d...d.....t.|...
+00000650: 6408 a101 6407 1900 a005 6403 a101 6406  d...d.....d...d.
+00000660: 1900 8301 6b04 723d 7c02 7c01 0202 7d01  ....k.r=|.|...}.
+00000670: 7d02 7406 7c01 7c02 8302 7d03 7403 7c03  }.t.|.|...}.t.|.
+00000680: 8301 0100 6400 5300 2909 4e63 0100 0000  ....d.S.).Nc....
+00000690: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+000006a0: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
+000006b0: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
+000006c0: 0253 0029 015a 0762 6163 6b75 705f 2901  .S.).Z.backup_).
+000006d0: 7217 0000 0029 02da 022e 3072 2400 0000  r....)....0r$...
+000006e0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+000006f0: 0a3c 6c69 7374 636f 6d70 3e35 0000 0073  .<listcomp>5...s
+00000700: 0200 0000 1a00 7a1f 7275 6e5f 636f 6d70  ......z.run_comp
+00000710: 6172 652e 3c6c 6f63 616c 733e 2e3c 6c69  are.<locals>.<li
+00000720: 7374 636f 6d70 3eda 012e e902 0000 0075  stcomp>........u
+00000730: 4e00 0000 1b5b 3333 6dc2 b71b 5b30 6de6  N....[33m...[0m.
+00000740: 95b0 e68d aee5 ba93 e5a4 87e4 bbbd e695  ................
+00000750: b0e9 878f e4b8 8de5 a49f 32e4 b8aa efbc  ..........2.....
+00000760: 8ce8 afb7 e585 8867 656e 7370 2062 6163  .......gensp bac
+00000770: 6b75 70e5 a487 e4bb bde6 95b0 e68d aee5  kup.............
+00000780: ba93 7201 0000 0072 1200 0000 da01 5f29  ..r....r......_)
+00000790: 07da 026f 73da 076c 6973 7464 6972 721a  ...os..listdirr.
+000007a0: 0000 00da 0570 7269 6e74 da03 696e 7472  .....print..intr
+000007b0: 1600 0000 7225 0000 0029 045a 0c62 6163  ....r%...).Z.bac
+000007c0: 6b75 705f 6669 6c65 7372 0800 0000 7209  kup_filesr....r.
+000007d0: 0000 0072 2300 0000 720d 0000 0072 0d00  ...r#...r....r..
+000007e0: 0000 720e 0000 00da 0b72 756e 5f63 6f6d  ..r......run_com
+000007f0: 7061 7265 3400 0000 7312 0000 0014 010c  pare4...s.......
+00000800: 0108 0108 0108 0138 020a 010a 010c 0172  .......8.......r
+00000810: 2f00 0000 2905 7205 0000 0072 2b00 0000  /...).r....r+...
+00000820: 720f 0000 0072 2500 0000 722f 0000 0072  r....r%...r/...r
+00000830: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000840: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000850: 0073 0a00 0000 0800 0801 0803 0806 0c29  .s.............)
```

## generateStoredProcedure/__pycache__/login.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun  3 06:35:17 2023 UTC, .py size: 632 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 25df 7a64 7802 0000  o.......%.zdx...
+00000000: 6f0d 0d0a 0000 0000 0450 7d64 7302 0000  o........P}ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 8400 5a03 6504 6405 6b02  ..d.d...Z.e.d.k.
 00000050: 7217 6503 8300 0100 6401 5300 6401 5300  r.e.....d.S.d.S.
 00000060: 2906 e900 0000 004e 2901 da0d 636f 6e6e  )......N)...conn
 00000070: 5f70 6f73 7467 7265 7363 0000 0000 0000  _postgresc......
@@ -25,28 +25,28 @@
 00000180: 0000 1b5b 3334 6dc2 b71b 5b30 6d68 6f73  ...[34m...[0mhos
 00000190: 743a 2075 1100 0000 1b5b 3334 6dc2 b71b  t: u.....[34m...
 000001a0: 5b30 6d70 6f72 743a 2075 1500 0000 1b5b  [0mport: u.....[
 000001b0: 3334 6dc2 b71b 5b30 6d75 7365 726e 616d  34m...[0musernam
 000001c0: 653a 2075 1500 0000 1b5b 3334 6dc2 b71b  e: u.....[34m...
 000001d0: 5b30 6d70 6173 7377 6f72 643a 20da 056c  [0mpassword: ..l
 000001e0: 6f67 696e da04 686f 7374 da04 706f 7274  ogin..host..port
-000001f0: da08 7573 6572 6e61 6d65 da08 7061 7373  ..username..pass
-00000200: 776f 7264 da01 775a 0870 6f73 7467 7265  word..wZ.postgre
-00000210: 7329 07da 046f 7065 6eda 0479 616d 6c5a  s)...open..yamlZ
-00000220: 0973 6166 655f 6c6f 6164 da05 696e 7075  .safe_load..inpu
-00000230: 74da 0573 7472 6970 da04 6475 6d70 7202  t..strip..dumpr.
-00000240: 0000 0029 06da 0166 da03 656e 7672 0500  ...)...f..envr..
-00000250: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000260: 00a9 0072 1100 0000 fa42 6275 696c 642f  ...r.....Bbuild/
-00000270: 6264 6973 742e 6d61 636f 7378 2d31 332e  bdist.macosx-13.
-00000280: 322d 6172 6d36 342f 6567 672f 6765 6e65  2-arm64/egg/gene
-00000290: 7261 7465 5374 6f72 6564 5072 6f63 6564  rateStoredProced
-000002a0: 7572 652f 6c6f 6769 6e2e 7079 7204 0000  ure/login.pyr...
-000002b0: 0005 0000 0073 1e00 0000 0c01 0c01 1cff  .....s..........
-000002c0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000002d0: 0c01 0e01 1cff 0c02 7204 0000 00da 085f  ........r......_
-000002e0: 5f6d 6169 6e5f 5f29 0572 0b00 0000 5a06  _main__).r....Z.
-000002f0: 6261 636b 7570 7202 0000 0072 0400 0000  backupr....r....
-00000300: da08 5f5f 6e61 6d65 5f5f 7211 0000 0072  ..__name__r....r
-00000310: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
-00000320: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
-00000330: 0008 010c 0108 0208 100a 0204 fe         .............
+000001f0: da04 7573 6572 da08 7061 7373 776f 7264  ..user..password
+00000200: da01 775a 0870 6f73 7467 7265 7329 07da  ..wZ.postgres)..
+00000210: 046f 7065 6eda 0479 616d 6c5a 0973 6166  .open..yamlZ.saf
+00000220: 655f 6c6f 6164 da05 696e 7075 74da 0573  e_load..input..s
+00000230: 7472 6970 da04 6475 6d70 7202 0000 0029  trip..dumpr....)
+00000240: 06da 0166 da03 656e 7672 0500 0000 7206  ...f..envr....r.
+00000250: 0000 00da 0875 7365 726e 616d 6572 0800  .....usernamer..
+00000260: 0000 a900 7212 0000 00fa 4262 7569 6c64  ....r.....Bbuild
+00000270: 2f62 6469 7374 2e6d 6163 6f73 782d 3133  /bdist.macosx-13
+00000280: 2e32 2d61 726d 3634 2f65 6767 2f67 656e  .2-arm64/egg/gen
+00000290: 6572 6174 6553 746f 7265 6450 726f 6365  erateStoredProce
+000002a0: 6475 7265 2f6c 6f67 696e 2e70 7972 0400  dure/login.pyr..
+000002b0: 0000 0500 0000 731e 0000 000c 010c 011c  ......s.........
+000002c0: ff0c 020c 010c 010c 010c 010c 010c 010c  ................
+000002d0: 010c 010e 011c ff0c 0272 0400 0000 da08  .........r......
+000002e0: 5f5f 6d61 696e 5f5f 2905 720b 0000 005a  __main__).r....Z
+000002f0: 0662 6163 6b75 7072 0200 0000 7204 0000  .backupr....r...
+00000300: 00da 085f 5f6e 616d 655f 5f72 1200 0000  ...__name__r....
+00000310: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000320: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
+00000330: 0000 0800 0c01 0803 0810 0a01 04ff       ..............
```

## generateStoredProcedure/__pycache__/main.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun  3 09:31:59 2023 UTC, .py size: 1464 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,86 +1,113 @@
-00000000: 6f0d 0d0a 0000 0000 8f08 7b64 b805 0000  o.........{d....
+00000000: 6f0d 0d0a 0000 0000 df4e 7d64 cb07 0000  o........N}d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6401 6c06  d.l.m.Z...d.d.l.
-00000060: 5a06 6405 6406 8400 5a07 6401 5300 2907  Z.d.d...Z.d.S.).
-00000070: e900 0000 004e 2901 da05 6c6f 6769 6e29  .....N)...login)
-00000080: 01da 0a67 6574 5f62 6163 6b75 7029 01da  ...get_backup)..
-00000090: 0b72 756e 5f63 6f6d 7061 7265 6300 0000  .run_comparec...
-000000a0: 0000 0000 0000 0000 0005 0000 0008 0000  ................
-000000b0: 0043 0000 0073 6e01 0000 7400 7401 6a02  .C...sn...t.t.j.
-000000c0: 8301 6401 6b02 72b1 7401 6a02 6402 1900  ..d.k.r.t.j.d...
-000000d0: 6403 6b02 7213 7403 8300 0100 6400 5300  d.k.r.t.....d.S.
-000000e0: 7401 6a02 6402 1900 6404 6b02 7251 6405  t.j.d...d.k.rQd.
-000000f0: 7d00 7404 a005 a100 4400 5d10 7d01 7c01  }.t.....D.].}.|.
-00000100: a006 6406 a101 7230 7c01 a007 6407 a101  ..d...r0|...d...
-00000110: 7230 7c00 6402 3700 7d00 7120 7408 6408  r0|.d.7.}.q t.d.
-00000120: 7409 7c00 8301 1700 8301 0100 7c00 6401  t.|.........|.d.
-00000130: 6b05 7245 7408 6409 8301 0100 7401 a00a  k.rEt.d.....t...
-00000140: a100 0100 740b 640a 8301 a00c a100 7d02  ....t.d.......}.
-00000150: 740d 7c02 8301 0100 6400 5300 7401 6a02  t.|.....d.S.t.j.
-00000160: 6402 1900 640b 6b02 7261 7408 640c 8301  d...d.k.rat.d...
-00000170: 0100 740e 8300 0100 6400 5300 7401 6a02  ..t.....d.S.t.j.
-00000180: 6402 1900 640d 6b02 7284 7404 a005 a100  d...d.k.r.t.....
-00000190: 4400 5d11 7d01 7c01 a006 6406 a101 727d  D.].}.|...d...r}
-000001a0: 7c01 a007 6407 a101 727d 7404 a00f 7c01  |...d...r}t...|.
-000001b0: a101 0100 716c 7408 640e 8301 0100 6400  ....qlt.d.....d.
-000001c0: 5300 7401 6a02 6402 1900 640f 6b02 72ab  S.t.j.d...d.k.r.
-000001d0: 7410 6410 6411 8302 8f11 7d03 7c03 a011  t.d.d.....}.|...
-000001e0: a100 7d04 7408 7c04 8301 0100 5700 6400  ..}.t.|.....W.d.
-000001f0: 0400 0400 8303 0100 6400 5300 3100 73a4  ........d.S.1.s.
-00000200: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-00000210: 7408 6412 8301 0100 6400 5300 7408 6413  t.d.....d.S.t.d.
-00000220: 8301 0100 6400 5300 2914 4ee9 0200 0000  ....d.S.).N.....
-00000230: e901 0000 0072 0200 0000 da06 6261 636b  .....r......back
-00000240: 7570 7201 0000 005a 0762 6163 6b75 705f  upr....Z.backup_
-00000250: 7a04 2e73 716c 7522 0000 001b 5b33 326d  z..sqlu"....[32m
-00000260: c2b7 1b5b 306d e5b7 b2e5 ad98 e59c a8e5  ...[0m..........
-00000270: a487 e4bb bde6 95b0 e987 8f3a 2075 6700  ...........: ug.
-00000280: 0000 1b5b 3333 6dc2 b71b 5b30 6de5 a487  ...[33m...[0m...
-00000290: e4bb bde6 95b0 e987 8fe5 b7b2 e6bb a1ef  ................
-000002a0: bc8c e8af b7e6 89a7 e8a1 8c67 7370 2063  ...........gsp c
-000002b0: 6f6d 7061 7265 e794 9fe6 8890 e5ad 98e5  ompare..........
-000002c0: 82a8 e8bf 87e7 a88b efbc 8ce6 8896 e689  ................
-000002d0: a7e8 a18c 6773 7020 636c 6561 72e6 b885  ....gsp clear...
-000002e0: e7a9 bae5 a487 e4bb bd75 1500 0000 1b5b  .........u.....[
-000002f0: 3334 6dc2 b71b 5b30 6d64 6174 6162 6173  34m...[0mdatabas
-00000300: 653a 20da 0763 6f6d 7061 7265 7525 0000  e: ..compareu%..
-00000310: 001b 5b33 326d c2b7 1b5b 306d e794 9fe6  ..[32m...[0m....
-00000320: 8890 e5ad 98e5 82a8 e8bf 87e7 a88b e5a6  ................
-00000330: 82e4 b88b 3a20 da05 636c 6561 7275 1500  ....: ..clearu..
-00000340: 0000 1b5b 3332 6dc2 b71b 5b30 6d63 6f6d  ...[32m...[0mcom
-00000350: 706c 6574 6564 215a 086c 6173 7474 696d  pleted!Z.lasttim
-00000360: 657a 1272 6573 746f 7265 5f62 6163 6b75  ez.restore_backu
-00000370: 702e 7371 6cda 0172 7518 0000 001b 5b33  p.sql..ru.....[3
-00000380: 316d c2b7 1b49 6e76 616c 6964 2061 7267  1m...Invalid arg
-00000390: 756d 656e 7475 2300 0000 1b5b 3331 6dc2  umentu#....[31m.
-000003a0: b71b 496e 7661 6c69 6420 6e75 6d62 6572  ..Invalid number
-000003b0: 206f 6620 6172 6775 6d65 6e74 7329 12da   of arguments)..
-000003c0: 036c 656e da03 7379 73da 0461 7267 7672  .len..sys..argvr
-000003d0: 0200 0000 da02 6f73 da07 6c69 7374 6469  ......os..listdi
-000003e0: 72da 0a73 7461 7274 7377 6974 68da 0865  r..startswith..e
-000003f0: 6e64 7377 6974 68da 0570 7269 6e74 da03  ndswith..print..
-00000400: 7374 72da 0465 7869 74da 0569 6e70 7574  str..exit..input
-00000410: da05 7374 7269 7072 0300 0000 7204 0000  ..stripr....r...
-00000420: 00da 0672 656d 6f76 65da 046f 7065 6eda  ...remove..open.
-00000430: 0472 6561 6429 055a 0b66 696c 655f 6e75  .read).Z.file_nu
-00000440: 6d62 6572 da04 6669 6c65 5a0d 6461 7461  mber..fileZ.data
-00000450: 6261 7365 5f6e 616d 65da 0166 da07 636f  base_name..f..co
-00000460: 6e74 656e 74a9 0072 1d00 0000 fa41 6275  ntent..r.....Abu
-00000470: 696c 642f 6264 6973 742e 6d61 636f 7378  ild/bdist.macosx
-00000480: 2d31 332e 322d 6172 6d36 342f 6567 672f  -13.2-arm64/egg/
-00000490: 6765 6e65 7261 7465 5374 6f72 6564 5072  generateStoredPr
-000004a0: 6f63 6564 7572 652f 6d61 696e 2e70 79da  ocedure/main.py.
-000004b0: 046d 6169 6e07 0000 0073 3e00 0000 0e01  .main....s>.....
-000004c0: 0e01 0a01 0e01 0401 0c01 1401 0801 0280  ................
-000004d0: 1001 0801 0801 0801 0c01 0c01 0e01 0801  ................
-000004e0: 0a01 0e01 0c01 1401 0a01 0280 0c01 0e01  ................
-000004f0: 0c01 0801 0a01 22fe 0c07 0c02 721f 0000  ......".....r...
-00000500: 0029 0872 0c00 0000 7202 0000 0072 0700  .).r....r....r..
-00000510: 0000 7203 0000 0072 0800 0000 7204 0000  ..r....r....r...
-00000520: 0072 0e00 0000 721f 0000 0072 1d00 0000  .r....r....r....
-00000530: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000540: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000550: 0000 0801 0c01 0c01 0c01 0801 0c01       ..............
+00000060: 5a06 6405 6406 8400 5a07 6508 6407 6b02  Z.d.d...Z.e.d.k.
+00000070: 7227 6507 8300 0100 6401 5300 6401 5300  r'e.....d.S.d.S.
+00000080: 2908 e900 0000 004e 2901 da05 6c6f 6769  )......N)...logi
+00000090: 6e29 01da 0a67 6574 5f62 6163 6b75 7029  n)...get_backup)
+000000a0: 01da 0b72 756e 5f63 6f6d 7061 7265 6300  ...run_comparec.
+000000b0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
+000000c0: 0000 0043 0000 0073 b801 0000 7400 7401  ...C...s....t.t.
+000000d0: 6a02 8301 6401 6b02 72d6 7401 6a02 6402  j...d.k.r.t.j.d.
+000000e0: 1900 6403 6b02 7213 7403 8300 0100 6400  ..d.k.r.t.....d.
+000000f0: 5300 7401 6a02 6402 1900 6404 6b02 7255  S.t.j.d...d.k.rU
+00000100: 6405 7d00 7404 a005 a100 4400 5d10 7d01  d.}.t.....D.].}.
+00000110: 7c01 a006 6406 a101 7230 7c01 a007 6407  |...d...r0|...d.
+00000120: a101 7230 7c00 6402 3700 7d00 7120 7408  ..r0|.d.7.}.q t.
+00000130: 6408 7409 7c00 8301 1700 8301 0100 7c00  d.t.|.........|.
+00000140: 6401 6b05 7245 7408 6409 8301 0100 7401  d.k.rEt.d.....t.
+00000150: a00a a100 0100 740b 640a 8301 a00c a100  ......t.d.......
+00000160: 7d02 7408 640b 8301 0100 740d 7c02 8301  }.t.d.....t.|...
+00000170: 0100 6400 5300 7401 6a02 6402 1900 640c  ..d.S.t.j.d...d.
+00000180: 6b02 7265 7408 640d 8301 0100 740e 8300  k.ret.d.....t...
+00000190: 0100 6400 5300 7401 6a02 6402 1900 640e  ..d.S.t.j.d...d.
+000001a0: 6b02 7288 7404 a005 a100 4400 5d11 7d01  k.r.t.....D.].}.
+000001b0: 7c01 a006 6406 a101 7281 7c01 a007 6407  |...d...r.|...d.
+000001c0: a101 7281 7404 a00f 7c01 a101 0100 7170  ..r.t...|.....qp
+000001d0: 7408 640f 8301 0100 6400 5300 7401 6a02  t.d.....d.S.t.j.
+000001e0: 6402 1900 6410 6b02 72a9 7408 6411 8301  d...d.k.r.t.d...
+000001f0: 0100 7408 6412 8301 0100 7408 6413 8301  ..t.d.....t.d...
+00000200: 0100 7408 6414 8301 0100 7408 6415 8301  ..t.d.....t.d...
+00000210: 0100 7408 6416 8301 0100 6400 5300 7401  ..t.d.....d.S.t.
+00000220: 6a02 6402 1900 6417 6b02 72d0 7410 6418  j.d...d.k.r.t.d.
+00000230: 6419 8302 8f11 7d03 7c03 a011 a100 7d04  d.....}.|.....}.
+00000240: 7408 7c04 8301 0100 5700 6400 0400 0400  t.|.....W.d.....
+00000250: 8303 0100 6400 5300 3100 73c9 7701 0100  ....d.S.1.s.w...
+00000260: 0100 0100 5900 0100 6400 5300 7408 641a  ....Y...d.S.t.d.
+00000270: 8301 0100 6400 5300 7408 641b 8301 0100  ....d.S.t.d.....
+00000280: 6400 5300 291c 4ee9 0200 0000 e901 0000  d.S.).N.........
+00000290: 0072 0200 0000 da06 6261 636b 7570 7201  .r......backupr.
+000002a0: 0000 005a 0762 6163 6b75 705f 7a04 2e73  ...Z.backup_z..s
+000002b0: 716c 7522 0000 001b 5b33 326d c2b7 1b5b  qlu"....[32m...[
+000002c0: 306d e5b7 b2e5 ad98 e59c a8e5 a487 e4bb  0m..............
+000002d0: bde6 95b0 e987 8f3a 2075 6700 0000 1b5b  .......: ug....[
+000002e0: 3333 6dc2 b71b 5b30 6de5 a487 e4bb bde6  33m...[0m.......
+000002f0: 95b0 e987 8fe5 b7b2 e6bb a1ef bc8c e8af  ................
+00000300: b7e6 89a7 e8a1 8c67 7370 2063 6f6d 7061  .......gsp compa
+00000310: 7265 e794 9fe6 8890 e5ad 98e5 82a8 e8bf  re..............
+00000320: 87e7 a88b efbc 8ce6 8896 e689 a7e8 a18c  ................
+00000330: 6773 7020 636c 6561 72e6 b885 e7a9 bae5  gsp clear.......
+00000340: a487 e4bb bd75 1500 0000 1b5b 3334 6dc2  .....u.....[34m.
+00000350: b71b 5b30 6d64 6174 6162 6173 653a 2075  ..[0mdatabase: u
+00000360: 1a00 0000 1b5b 3332 6dc2 b71b 5b30 6de5  .....[32m...[0m.
+00000370: a487 e4bb bde4 b8ad e280 a6e2 80a6 da07  ................
+00000380: 636f 6d70 6172 6575 2500 0000 1b5b 3332  compareu%....[32
+00000390: 6dc2 b71b 5b30 6de7 949f e688 90e5 ad98  m...[0m.........
+000003a0: e582 a8e8 bf87 e7a8 8be5 a682 e4b8 8b3a  ...............:
+000003b0: 20da 0563 6c65 6172 7515 0000 001b 5b33   ..clearu.....[3
+000003c0: 326d c2b7 1b5b 306d 636f 6d70 6c65 7465  2m...[0mcomplete
+000003d0: 6421 da04 6865 6c70 751a 0000 001b 5b33  d!..helpu.....[3
+000003e0: 326d c2b7 1b5b 306d e58f 82e6 95b0 e4bb  2m...[0m........
+000003f0: 8be7 bb8d efbc 9a75 2e00 0000 1b5b 3332  .......u.....[32
+00000400: 6dc2 b71b 5b30 6d6c 6f67 696e efbc 9ae6  m...[0mlogin....
+00000410: b3a8 e586 8ce6 95b0 e68d aee5 ba93 e59f  ................
+00000420: bae6 9cac e4bf a1e6 81af 7523 0000 001b  ..........u#....
+00000430: 5b33 326d c2b7 1b5b 306d 6261 636b 7570  [32m...[0mbackup
+00000440: efbc 9ae5 a487 e4bb bde6 95b0 e68d aee5  ................
+00000450: ba93 7536 0000 001b 5b33 326d c2b7 1b5b  ..u6....[32m...[
+00000460: 306d 636f 6d70 6172 65ef bc9a e6af 94e8  0mcompare.......
+00000470: be83 e5a4 87e4 bbbd e5b9 b6e7 949f e688  ................
+00000480: 90e5 ad98 e582 a8e8 bf87 e7a8 8b75 2e00  .............u..
+00000490: 0000 1b5b 3332 6dc2 b71b 5b30 6d63 6c65  ...[32m...[0mcle
+000004a0: 6172 efbc 9ae6 b885 e999 a4e6 9cac e59c  ar..............
+000004b0: b0e6 95b0 e68d aee5 ba93 e5a4 87e4 bbbd  ................
+000004c0: 7518 0000 001b 5b33 326d c2b7 1b5b 306d  u.....[32m...[0m
+000004d0: 6865 6c70 efbc 9ae5 b8ae e58a a95a 086c  help.........Z.l
+000004e0: 6173 7474 696d 657a 1272 6573 746f 7265  asttimez.restore
+000004f0: 5f62 6163 6b75 702e 7371 6cda 0172 7518  _backup.sql..ru.
+00000500: 0000 001b 5b33 316d c2b7 1b49 6e76 616c  ....[31m...Inval
+00000510: 6964 2061 7267 756d 656e 7475 2300 0000  id argumentu#...
+00000520: 1b5b 3331 6dc2 b71b 496e 7661 6c69 6420  .[31m...Invalid 
+00000530: 6e75 6d62 6572 206f 6620 6172 6775 6d65  number of argume
+00000540: 6e74 7329 12da 036c 656e da03 7379 73da  nts)...len..sys.
+00000550: 0461 7267 7672 0200 0000 da02 6f73 da07  .argvr......os..
+00000560: 6c69 7374 6469 72da 0a73 7461 7274 7377  listdir..startsw
+00000570: 6974 68da 0865 6e64 7377 6974 68da 0570  ith..endswith..p
+00000580: 7269 6e74 da03 7374 72da 0465 7869 74da  rint..str..exit.
+00000590: 0569 6e70 7574 da05 7374 7269 7072 0300  .input..stripr..
+000005a0: 0000 7204 0000 00da 0672 656d 6f76 65da  ..r......remove.
+000005b0: 046f 7065 6eda 0472 6561 6429 055a 0b66  .open..read).Z.f
+000005c0: 696c 655f 6e75 6d62 6572 da04 6669 6c65  ile_number..file
+000005d0: 5a0d 6461 7461 6261 7365 5f6e 616d 65da  Z.database_name.
+000005e0: 0166 da07 636f 6e74 656e 74a9 0072 1e00  .f..content..r..
+000005f0: 0000 fa41 6275 696c 642f 6264 6973 742e  ...Abuild/bdist.
+00000600: 6d61 636f 7378 2d31 332e 322d 6172 6d36  macosx-13.2-arm6
+00000610: 342f 6567 672f 6765 6e65 7261 7465 5374  4/egg/generateSt
+00000620: 6f72 6564 5072 6f63 6564 7572 652f 6d61  oredProcedure/ma
+00000630: 696e 2e70 79da 046d 6169 6e08 0000 0073  in.py..main....s
+00000640: 4e00 0000 0e01 0e01 0a01 0e01 0401 0c01  N...............
+00000650: 1401 0801 0280 1001 0801 0801 0801 0c01  ................
+00000660: 0801 0c01 0e01 0801 0a01 0e01 0c01 1401  ................
+00000670: 0a01 0280 0c01 0e01 0801 0801 0801 0801  ................
+00000680: 0801 0c01 0e01 0c01 0801 0a01 22fe 0c07  ............"...
+00000690: 0c02 7220 0000 00da 085f 5f6d 6169 6e5f  ..r .....__main_
+000006a0: 5f29 0972 0d00 0000 7202 0000 0072 0700  _).r....r....r..
+000006b0: 0000 7203 0000 0072 0800 0000 7204 0000  ..r....r....r...
+000006c0: 0072 0f00 0000 7220 0000 00da 085f 5f6e  .r....r .....__n
+000006d0: 616d 655f 5f72 1e00 0000 721e 0000 0072  ame__r....r....r
+000006e0: 1e00 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
+000006f0: 6c65 3e01 0000 0073 1200 0000 0800 0c01  le>....s........
+00000700: 0c01 0c01 0801 0803 082c 0a01 04ff       .........,....
```

