# Comparing `tmp/cashare-0.0.2.tar.gz` & `tmp/cashare-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashare-0.0.2.tar", last modified: Mon May 29 07:53:30 2023, max compression
+gzip compressed data, was "cashare-0.0.5.tar", last modified: Mon Jun  5 12:03:44 2023, max compression
```

## Comparing `cashare-0.0.2.tar` & `cashare-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:53:30.637090 cashare-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      164 2023-05-29 07:53:30.637090 cashare-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:53:30.627089 cashare-0.0.2/cashare/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.2/cashare/__init__.py
--rw-rw-rw-   0        0        0     3269 2023-05-29 07:12:13.000000 cashare-0.0.2/cashare/day_data.py
--rw-rw-rw-   0        0        0       58 2023-03-25 03:03:24.000000 cashare-0.0.2/cashare/dname.py
--rw-rw-rw-   0        0        0     4312 2023-05-29 07:12:13.000000 cashare-0.0.2/cashare/minute_data.py
--rw-rw-rw-   0        0        0      441 2023-05-29 07:12:14.000000 cashare-0.0.2/cashare/stock_list.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:53:30.635097 cashare-0.0.2/cashare.egg-info/
--rw-rw-rw-   0        0        0      164 2023-05-29 07:53:30.000000 cashare-0.0.2/cashare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-29 07:53:30.000000 cashare-0.0.2/cashare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:53:30.000000 cashare-0.0.2/cashare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-29 07:53:30.000000 cashare-0.0.2/cashare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 07:53:30.000000 cashare-0.0.2/cashare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 07:53:30.638060 cashare-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-05-29 07:12:13.000000 cashare-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.864579 cashare-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      164 2023-06-05 12:03:44.863582 cashare-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.854606 cashare-0.0.5/cashare/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.5/cashare/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/day_data.py
+-rw-rw-rw-   0        0        0       61 2023-06-04 12:22:16.000000 cashare-0.0.5/cashare/dname.py
+-rw-rw-rw-   0        0        0     4343 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/minute_data.py
+-rw-rw-rw-   0        0        0      445 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/stock_list.py
+-rw-rw-rw-   0        0        0      438 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/stock_now.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.862585 cashare-0.0.5/cashare.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 12:03:44.864579 cashare-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-06-05 12:03:20.000000 cashare-0.0.5/setup.py
```

### Comparing `cashare-0.0.2/cashare/day_data.py` & `cashare-0.0.5/cashare/day_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import httpx
-from dname import url1
+from cashare.dname import url1
 import datetime
 import pandas as pd
 import dateutil.relativedelta
 import time
 
 def daily_data(sk_code,token,end_date=str(datetime.date.today().strftime('%Y-%m-%d')),start_date='19000101',x=5000, y=5000):
     if start_date > (datetime.date.today().strftime('%Y-%m-%d')):
@@ -76,15 +76,15 @@
             df = df.append(lsss, ignore_index=True)
             time.sleep(0.2)
             # print(df)
     df.drop_duplicates(subset='date', keep='first', inplace =True, ignore_index = True)#去重
     return df
 
 if __name__ == '__main__':
-    df = daily_data(sk_code="aapl", token='g0ad8f825bad3234af22d39de80f717db93', start_date='2022-04-02',
+    df = daily_data(sk_code="aapl", token='y0ad8f825bad3234ada0ab7ff56e1925372', start_date='2012-04-02',
                     end_date='2023-05-02')
     print(df)
     pass
```

### Comparing `cashare-0.0.2/cashare/minute_data.py` & `cashare-0.0.5/cashare/minute_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import httpx
-from dname import url1
+from cashare.dname import url1
 import datetime
 import pandas as pd
 import dateutil.relativedelta
 import time
 def m_data(sk_code,type,token,end_date=str(datetime.date.today().strftime('%Y-%m-%d')),start_date='19000101',):
 
 
@@ -84,27 +84,28 @@
 
 def url_get(url_list):
     import pandas as pd
     df = pd.DataFrame(data=None)
     for item in url_list:
         # print(item)
         r = httpx.get(item,timeout=30)
+        # print(r.json())
         if pd.DataFrame(r.json()).empty:
            pass
         else:
             lsss = pd.DataFrame(r.json()).sort_values(by='date')  # 进行升序排序
             df = df.append(lsss, ignore_index=True)
             time.sleep(0.2)
             # print(df)
     df.drop_duplicates(subset='date', keep='first', inplace =True, ignore_index = True)#去重
     # df.to_csv("34343.csv")
     return df
 
 if __name__ == '__main__':
 
-    # df=m_data(sk_code="aapl",token='g0ad8f825bad3234af22d39de80f717db93',type='30min',start_date='2023-03-02',end_date='2023-05-02')
-    # print(df)
+    df=m_data(sk_code="aapl",token='y0ad8f825bad3234ada0ab7ff56e1925372',type='30min',start_date='2022-03-02',end_date='2023-05-02')
+    print(df)
     pass
```

