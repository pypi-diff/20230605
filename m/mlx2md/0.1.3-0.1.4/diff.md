# Comparing `tmp/mlx2md-0.1.3.tar.gz` & `tmp/mlx2md-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx2md-0.1.3.tar", last modified: Mon Jun  5 15:33:14 2023, max compression
+gzip compressed data, was "mlx2md-0.1.4.tar", last modified: Mon Jun  5 15:39:22 2023, max compression
```

## Comparing `mlx2md-0.1.3.tar` & `mlx2md-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:14.933995 mlx2md-0.1.3/
--rw-rw-rw-   0        0        0     6810 2023-06-05 15:33:14.933995 mlx2md-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5983 2023-06-05 15:31:55.000000 mlx2md-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:14.915134 mlx2md-0.1.3/mlx2md/
--rw-rw-rw-   0        0        0      115 2023-06-05 12:51:18.000000 mlx2md-0.1.3/mlx2md/__init__.py
--rw-rw-rw-   0        0        0     6946 2023-06-05 12:39:23.000000 mlx2md-0.1.3/mlx2md/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:14.926480 mlx2md-0.1.3/mlx2md.egg-info/
--rw-rw-rw-   0        0        0     6810 2023-06-05 15:33:14.000000 mlx2md-0.1.3/mlx2md.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-05 15:33:14.000000 mlx2md-0.1.3/mlx2md.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:33:14.000000 mlx2md-0.1.3/mlx2md.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 15:33:14.000000 mlx2md-0.1.3/mlx2md.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:33:14.933995 mlx2md-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-06-05 15:22:02.000000 mlx2md-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:22.758935 mlx2md-0.1.4/
+-rw-rw-rw-   0        0        0     6830 2023-06-05 15:39:22.758935 mlx2md-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6003 2023-06-05 15:39:05.000000 mlx2md-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:22.745285 mlx2md-0.1.4/mlx2md/
+-rw-rw-rw-   0        0        0      115 2023-06-05 12:51:18.000000 mlx2md-0.1.4/mlx2md/__init__.py
+-rw-rw-rw-   0        0        0     6946 2023-06-05 12:39:23.000000 mlx2md-0.1.4/mlx2md/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:22.756425 mlx2md-0.1.4/mlx2md.egg-info/
+-rw-rw-rw-   0        0        0     6830 2023-06-05 15:39:22.000000 mlx2md-0.1.4/mlx2md.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-05 15:39:22.000000 mlx2md-0.1.4/mlx2md.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:39:22.000000 mlx2md-0.1.4/mlx2md.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 15:39:22.000000 mlx2md-0.1.4/mlx2md.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:39:22.758935 mlx2md-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-06-05 15:39:09.000000 mlx2md-0.1.4/setup.py
```

### Comparing `mlx2md-0.1.3/PKG-INFO` & `mlx2md-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx2md
-Version: 0.1.3
+Version: 0.1.4
 Summary: Matlab mlx to Markdown format converter
 Home-page: https://github.com/alient12/mlx2md
 Author: Ali Entezari
 Author-email: ali_ent12@yahoo.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -346,18 +346,18 @@
   s^4 + 57.99 s^3 + 1045 s^2 + 7085 s + 2.75e04
  
 Continuous-time transfer function.
 
 
 ```
 
-![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://github.com/alient12/mlx2md/blob/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
+![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
 
 
-![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://github.com/alient12/mlx2md/blob/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
+![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
 
 **k_new** *(1x5) double*:
 
 ```
 	1.0e+05 *
 
    -0.4437   -0.0698    0.0336    0.0010    1.5698
```

### Comparing `mlx2md-0.1.3/README.md` & `mlx2md-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -325,18 +325,18 @@
   s^4 + 57.99 s^3 + 1045 s^2 + 7085 s + 2.75e04
  
 Continuous-time transfer function.
 
 
 ```
 
-![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://github.com/alient12/mlx2md/blob/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
+![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
 
 
-![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://github.com/alient12/mlx2md/blob/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
+![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
 
 **k_new** *(1x5) double*:
 
 ```
 	1.0e+05 *
 
    -0.4437   -0.0698    0.0336    0.0010    1.5698
```

### Comparing `mlx2md-0.1.3/mlx2md/__main__.py` & `mlx2md-0.1.4/mlx2md/__main__.py`

 * *Files identical despite different names*

### Comparing `mlx2md-0.1.3/mlx2md.egg-info/PKG-INFO` & `mlx2md-0.1.4/mlx2md.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx2md
-Version: 0.1.3
+Version: 0.1.4
 Summary: Matlab mlx to Markdown format converter
 Home-page: https://github.com/alient12/mlx2md
 Author: Ali Entezari
 Author-email: ali_ent12@yahoo.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -346,18 +346,18 @@
   s^4 + 57.99 s^3 + 1045 s^2 + 7085 s + 2.75e04
  
 Continuous-time transfer function.
 
 
 ```
 
-![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://github.com/alient12/mlx2md/blob/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
+![f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/f2f9fc6b-fe2d-4f3d-8e79-70d7d3815b4f.png)
 
 
-![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://github.com/alient12/mlx2md/blob/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
+![008281e5-ffe8-4a76-96dc-74eab0b4808b.png](https://raw.githubusercontent.com/alient12/mlx2md/master/resources/008281e5-ffe8-4a76-96dc-74eab0b4808b.png)
 
 **k_new** *(1x5) double*:
 
 ```
 	1.0e+05 *
 
    -0.4437   -0.0698    0.0336    0.0010    1.5698
```

### Comparing `mlx2md-0.1.3/setup.py` & `mlx2md-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name='mlx2md',
-    version='0.1.3',    
+    version='0.1.4',    
     description='Matlab mlx to Markdown format converter',
     url='https://github.com/alient12/mlx2md',
     author='Ali Entezari',
     author_email='ali_ent12@yahoo.com',
     license='BSD 2-clause',
     packages=['mlx2md'],
     long_description=readme(),
```

