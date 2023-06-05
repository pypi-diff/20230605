# Comparing `tmp/hkfdb-3.4.tar.gz` & `tmp/hkfdb-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.4.tar", last modified: Sun Jun  4 18:37:45 2023, max compression
+gzip compressed data, was "hkfdb-3.4.2.tar", last modified: Mon Jun  5 05:24:32 2023, max compression
```

## Comparing `hkfdb-3.4.tar` & `hkfdb-3.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.987755 hkfdb-3.4/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-06-04 18:37:45.987486 hkfdb-3.4/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.986526 hkfdb-3.4/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   106397 2023-06-04 18:34:32.000000 hkfdb-3.4/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.987308 hkfdb-3.4/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-04 18:37:45.987801 hkfdb-3.4/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-06-04 18:37:07.000000 hkfdb-3.4/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.232151 hkfdb-3.4.2/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4.2/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-05 05:24:32.231992 hkfdb-3.4.2/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.230877 hkfdb-3.4.2/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   107582 2023-06-05 05:21:10.000000 hkfdb-3.4.2/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4.2/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.231817 hkfdb-3.4.2/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-05 05:24:32.000000 hkfdb-3.4.2/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 05:24:32.232199 hkfdb-3.4.2/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      763 2023-06-05 05:23:11.000000 hkfdb-3.4.2/setup.py
```

### Comparing `hkfdb-3.4/LICENSE` & `hkfdb-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4/PKG-INFO` & `hkfdb-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4
+Version: 3.4.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.4/README.md` & `hkfdb-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4/hkfdb/Database.py` & `hkfdb-3.4.2/hkfdb/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,15 @@
                     roll_diff_dict = {}
 
                     for expiry_date in expiry_dates:
                         try:
                             exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
                                                     (df['current_month_expiry_date_diff'] == rolling_day) &
                                                     (df['current_month'] == True)].reset_index(drop=True).sort_values(
-                                by=['datetime']).at[0, 'date']
+                                by=['datetime'], ascending=False).at[0, 'date']
 
                             df_roll = df[(df['date'] == exact_rolling_date)].copy()
                             df_roll = df_roll.sort_values(by=['datetime']).reset_index(drop=True)
 
                             roll_diff_dict[expiry_date] = {}
 
                             roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
@@ -413,25 +413,46 @@
                     expiry_dates = list(df['expiry_date'].unique())
                     expiry_dates.sort()
                     # print(expiry_dates)
 
                     # Calculate roll diff
                     roll_diff_dict = {}
 
+                    df.to_csv('df.csv')
+
                     for expiry_date in expiry_dates:
+
                         try:
+
+
+                            # print(expiry_date)
+                            #
+                            # print(df[(df['expiry_date'] == expiry_date) &
+                            #                         (df['current_month_expiry_date_diff'] == rolling_day) &
+                            #                         (df['current_month'] == True)].sort_values(by=['datetime'], ascending=False))
+                            #
+                            # exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
+                            #                         (df['current_month_expiry_date_diff'] == rolling_day) &
+                            #                         (df['current_month'] == True)].sort_values(by=['datetime'], ascending=False).reset_index(drop=True).reset_index(drop=True).at[0, 'date']
+
                             exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
                                                     (df['current_month_expiry_date_diff'] == rolling_day) &
-                                                    (df['current_month'] == True)].sort_values(by=['datetime']).reset_index(drop=True).reset_index(drop=True).at[0, 'date']
+                                                    (df['current_month'] == True)].sort_values(by=['datetime'],
+                                                                                               ascending=False).reset_index(
+                                                                            drop=True).reset_index(drop=True).at[0, 'date']
+                                # Sorting Reverse because get later date to make sure it is RTH trading date
+
+
 
                             df_roll = df[(df['date'] == exact_rolling_date)].copy()
                             df_roll = df_roll[df_roll['time'] == rolling_time].sort_values(by=['expiry_date']).reset_index(drop=True)
 
                             roll_diff_dict[expiry_date] = {}
 
+
                             if len(df_roll) == 2:
                                 roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
                                 roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
                                 roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
                                 roll_diff_dict[expiry_date]['rolling_time'] = rolling_time
 
                             else:
@@ -439,20 +460,23 @@
                                 df_roll = df[(df['date'] == exact_rolling_date) & (df['RTH'] == True)].copy()
                                 df_roll = df_roll.sort_values(by=['time', 'expiry_date']).reset_index(drop=True)
                                 df_roll = df_roll.tail(2).sort_values(by=['expiry_date']).reset_index(drop=True)
                                 roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
                                 roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
                                 roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
                                 roll_diff_dict[expiry_date]['rolling_time'] = df_roll.at[0, 'time']
+
                         except:
                             pass
 
+
                     df = df.reset_index(drop=True)
                     df['roll_diff'] = 0
 
+
                     for expiry_date in roll_diff_dict.keys():
                         d = roll_diff_dict[expiry_date]['rolling_day']
                         t = roll_diff_dict[expiry_date]['rolling_time']
                         diff = roll_diff_dict[expiry_date]['roll_diff']
 
                         condition = (df['date'] == d) & (df['time'] == t) & (df['current_month'] == False)
                         indices = df[condition].index[0]
```

### Comparing `hkfdb-3.4/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.4.2/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4
+Version: 3.4.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.4/setup.py` & `hkfdb-3.4.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.4",
+    version="3.4.2",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

