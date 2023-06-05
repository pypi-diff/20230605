# Comparing `tmp/mlx2md-0.1.1.tar.gz` & `tmp/mlx2md-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx2md-0.1.1.tar", last modified: Mon Jun  5 13:21:21 2023, max compression
+gzip compressed data, was "mlx2md-0.1.2.tar", last modified: Mon Jun  5 15:10:22 2023, max compression
```

## Comparing `mlx2md-0.1.1.tar` & `mlx2md-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:21:21.402130 mlx2md-0.1.1/
--rw-rw-rw-   0        0        0      580 2023-06-05 13:21:21.402130 mlx2md-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-05 13:15:20.000000 mlx2md-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 13:21:21.393754 mlx2md-0.1.1/mlx2md/
--rw-rw-rw-   0        0        0      115 2023-06-05 12:51:18.000000 mlx2md-0.1.1/mlx2md/__init__.py
--rw-rw-rw-   0        0        0     6946 2023-06-05 12:39:23.000000 mlx2md-0.1.1/mlx2md/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:21:21.401619 mlx2md-0.1.1/mlx2md.egg-info/
--rw-rw-rw-   0        0        0      580 2023-06-05 13:21:21.000000 mlx2md-0.1.1/mlx2md.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-05 13:21:21.000000 mlx2md-0.1.1/mlx2md.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:21:21.000000 mlx2md-0.1.1/mlx2md.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 13:21:21.000000 mlx2md-0.1.1/mlx2md.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 13:21:21.402130 mlx2md-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-06-05 13:21:13.000000 mlx2md-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:10:22.588768 mlx2md-0.1.2/
+-rw-rw-rw-   0        0        0     6391 2023-06-05 15:10:22.588768 mlx2md-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5768 2023-06-05 13:27:49.000000 mlx2md-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:10:22.575267 mlx2md-0.1.2/mlx2md/
+-rw-rw-rw-   0        0        0      115 2023-06-05 12:51:18.000000 mlx2md-0.1.2/mlx2md/__init__.py
+-rw-rw-rw-   0        0        0     6946 2023-06-05 12:39:23.000000 mlx2md-0.1.2/mlx2md/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:10:22.588768 mlx2md-0.1.2/mlx2md.egg-info/
+-rw-rw-rw-   0        0        0     6391 2023-06-05 15:10:22.000000 mlx2md-0.1.2/mlx2md.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-05 15:10:22.000000 mlx2md-0.1.2/mlx2md.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:10:22.000000 mlx2md-0.1.2/mlx2md.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 15:10:22.000000 mlx2md-0.1.2/mlx2md.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:10:22.588768 mlx2md-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-06-05 15:09:58.000000 mlx2md-0.1.2/setup.py
```

### Comparing `mlx2md-0.1.1/mlx2md/__main__.py` & `mlx2md-0.1.2/mlx2md/__main__.py`

 * *Files identical despite different names*

### Comparing `mlx2md-0.1.1/setup.py` & `mlx2md-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from setuptools import setup
 
+def readme():
+    with open('README.md') as f:
+        return f.read()
+
 setup(
     name='mlx2md',
-    version='0.1.1',    
+    version='0.1.2',    
     description='Matlab mlx to Markdown format converter',
     url='https://github.com/alient12/mlx2md',
     author='Ali Entezari',
     author_email='ali_ent12@yahoo.com',
     license='BSD 2-clause',
     packages=['mlx2md'],
+    long_description=readme(),
+    long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
```

