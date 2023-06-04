# Comparing `tmp/rlenvironments-0.1.3.tar.gz` & `tmp/rlenvironments-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlenvironments-0.1.3.tar", last modified: Sun Jun  4 21:52:56 2023, max compression
+gzip compressed data, was "rlenvironments-0.1.4.tar", last modified: Sun Jun  4 21:59:27 2023, max compression
```

## Comparing `rlenvironments-0.1.3.tar` & `rlenvironments-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:52:56.751773 rlenvironments-0.1.3/
--rw-rw-rw-   0        0        0     1701 2023-06-04 21:52:56.751773 rlenvironments-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2023-06-04 21:51:04.000000 rlenvironments-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 21:52:56.743790 rlenvironments-0.1.3/rlenvironments.egg-info/
--rw-rw-rw-   0        0        0     1701 2023-06-04 21:52:56.000000 rlenvironments-0.1.3/rlenvironments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-04 21:52:56.000000 rlenvironments-0.1.3/rlenvironments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:52:56.000000 rlenvironments-0.1.3/rlenvironments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-04 21:52:56.000000 rlenvironments-0.1.3/rlenvironments.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:52:56.000000 rlenvironments-0.1.3/rlenvironments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 21:52:56.751773 rlenvironments-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1021 2023-06-04 21:52:25.000000 rlenvironments-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:59:27.210940 rlenvironments-0.1.4/
+-rw-rw-rw-   0        0        0     1809 2023-06-04 21:59:27.210940 rlenvironments-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2023-06-04 21:58:32.000000 rlenvironments-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 21:59:27.210940 rlenvironments-0.1.4/rlenvironments.egg-info/
+-rw-rw-rw-   0        0        0     1809 2023-06-04 21:59:26.000000 rlenvironments-0.1.4/rlenvironments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-04 21:59:27.000000 rlenvironments-0.1.4/rlenvironments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:59:26.000000 rlenvironments-0.1.4/rlenvironments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-04 21:59:26.000000 rlenvironments-0.1.4/rlenvironments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:59:26.000000 rlenvironments-0.1.4/rlenvironments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:59:27.210940 rlenvironments-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1021 2023-06-04 21:59:15.000000 rlenvironments-0.1.4/setup.py
```

### Comparing `rlenvironments-0.1.3/PKG-INFO` & `rlenvironments-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlenvironments
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for target seeking environment
 Home-page: https://github.com/ukoksoy/rlenvironments
 Author: Umut Koksoy
 Author-email: umutkoksoy@gmail.com
 Keywords: reinforcement-learning environment target-seeking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -47,12 +47,12 @@
 
         # Take a step in the environment
         next_state, reward, done = env.step(action)
 
         # Do something with the results
 
 
-![Output 1](./output1.png)
-![Output 2](./output2.png)
-![Output 3](./output3.png)
-![Output 4](./output4.png)
+![Output 1](rlenvironments/target_seeker/output1.png)
+![Output 2](rlenvironments/target_seeker/output2.png)
+![Output 3](rlenvironments/target_seeker/output3.png)
+![Output 4](rlenvironments/target_seeker/output4.png)
```

### Comparing `rlenvironments-0.1.3/README.md` & `rlenvironments-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 
         # Take a step in the environment
         next_state, reward, done = env.step(action)
 
         # Do something with the results
 
 
-![Output 1](./output1.png)
-![Output 2](./output2.png)
-![Output 3](./output3.png)
-![Output 4](./output4.png)
+![Output 1](rlenvironments/target_seeker/output1.png)
+![Output 2](rlenvironments/target_seeker/output2.png)
+![Output 3](rlenvironments/target_seeker/output3.png)
+![Output 4](rlenvironments/target_seeker/output4.png)
```

### Comparing `rlenvironments-0.1.3/rlenvironments.egg-info/PKG-INFO` & `rlenvironments-0.1.4/rlenvironments.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlenvironments
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for target seeking environment
 Home-page: https://github.com/ukoksoy/rlenvironments
 Author: Umut Koksoy
 Author-email: umutkoksoy@gmail.com
 Keywords: reinforcement-learning environment target-seeking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -47,12 +47,12 @@
 
         # Take a step in the environment
         next_state, reward, done = env.step(action)
 
         # Do something with the results
 
 
-![Output 1](./output1.png)
-![Output 2](./output2.png)
-![Output 3](./output3.png)
-![Output 4](./output4.png)
+![Output 1](rlenvironments/target_seeker/output1.png)
+![Output 2](rlenvironments/target_seeker/output2.png)
+![Output 3](rlenvironments/target_seeker/output3.png)
+![Output 4](rlenvironments/target_seeker/output4.png)
```

### Comparing `rlenvironments-0.1.3/setup.py` & `rlenvironments-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rlenvironments",
-    version="0.1.3",
+    version="0.1.4",
     author="Umut Koksoy",
     author_email="umutkoksoy@gmail.com",
     description="Python library for target seeking environment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ukoksoy/rlenvironments",
     packages=setuptools.find_packages(),
```

