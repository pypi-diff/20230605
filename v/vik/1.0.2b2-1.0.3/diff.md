# Comparing `tmp/vik-1.0.2b2.tar.gz` & `tmp/vik-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vik-1.0.2b2.tar", last modified: Fri Feb 10 17:59:35 2023, max compression
+gzip compressed data, was "vik-1.0.3.tar", last modified: Mon Jun  5 07:17:13 2023, max compression
```

## Comparing `vik-1.0.2b2.tar` & `vik-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 debill    (1000) debill    (1000)        0 2023-02-10 17:59:35.446210 vik-1.0.2b2/
--rw-r--r--   0 debill    (1000) debill    (1000)    35149 2023-02-10 15:12:18.000000 vik-1.0.2b2/LICENSE
--rw-r--r--   0 debill    (1000) debill    (1000)       16 2023-02-10 14:29:12.000000 vik-1.0.2b2/MANIFEST.in
--rw-r--r--   0 debill    (1000) debill    (1000)      896 2023-02-10 17:59:35.446210 vik-1.0.2b2/PKG-INFO
--rw-r--r--   0 debill    (1000) debill    (1000)      606 2023-02-10 16:11:53.000000 vik-1.0.2b2/README.md
--rw-r--r--   0 debill    (1000) debill    (1000)       81 2023-02-06 17:10:18.000000 vik-1.0.2b2/pyproject.toml
--rw-r--r--   0 debill    (1000) debill    (1000)      545 2023-02-10 17:59:35.446210 vik-1.0.2b2/setup.cfg
-drwxr-xr-x   0 debill    (1000) debill    (1000)        0 2023-02-10 17:59:35.446210 vik-1.0.2b2/vik/
--rw-r--r--   0 debill    (1000) debill    (1000)      731 2023-02-06 15:30:56.000000 vik-1.0.2b2/vik/.vimrc
--rw-r--r--   0 debill    (1000) debill    (1000)        0 2023-02-09 17:40:52.000000 vik-1.0.2b2/vik/__init__.py
--rwxr-xr-x   0 debill    (1000) debill    (1000)      814 2023-02-10 17:59:14.000000 vik-1.0.2b2/vik/vik.py
-drwxr-xr-x   0 debill    (1000) debill    (1000)        0 2023-02-10 17:59:35.446210 vik-1.0.2b2/vik.egg-info/
--rw-r--r--   0 debill    (1000) debill    (1000)      896 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/PKG-INFO
--rw-r--r--   0 debill    (1000) debill    (1000)      256 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/SOURCES.txt
--rw-r--r--   0 debill    (1000) debill    (1000)        1 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/dependency_links.txt
--rw-r--r--   0 debill    (1000) debill    (1000)       37 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/entry_points.txt
--rw-r--r--   0 debill    (1000) debill    (1000)       11 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/requires.txt
--rw-r--r--   0 debill    (1000) debill    (1000)        4 2023-02-10 17:59:35.000000 vik-1.0.2b2/vik.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.832357 vik-1.0.3/
+-rw-rw-rw-   0        0        0    35149 2023-03-25 15:10:13.000000 vik-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-06-05 07:14:54.000000 vik-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      953 2023-06-05 07:17:13.832357 vik-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-03-25 15:10:13.000000 vik-1.0.3/README.md
+-rw-rw-rw-   0        0        0       81 2023-03-25 15:10:13.000000 vik-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      573 2023-06-05 07:17:13.832357 vik-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.800358 vik-1.0.3/vik/
+-rw-rw-rw-   0        0        0      807 2023-06-05 07:11:34.000000 vik-1.0.3/vik/.vimrc
+-rw-rw-rw-   0        0        0        0 2023-03-25 15:10:13.000000 vik-1.0.3/vik/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-03-25 15:10:13.000000 vik-1.0.3/vik/vik.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.832357 vik-1.0.3/vik.egg-info/
+-rw-rw-rw-   0        0        0      953 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/top_level.txt
```

### Comparing `vik-1.0.2b2/LICENSE` & `vik-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vik-1.0.2b2/README.md` & `vik-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vik-1.0.2b2/vik/.vimrc` & `vik-1.0.3/vik/.vimrc`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 set nocompatible
 set noswapfile
 set nobackup
 
 set belloff=all
 
+let &t_EI = "\e[2 q"
+let &t_SI = "\e[6 q"
+
+syntax on
+set filetype=markdown
+
 set ignorecase
 set smartcase
 
 set tabstop=2
 set shiftwidth=2
 set softtabstop=2
 set expandtab
```

### Comparing `vik-1.0.2b2/vik/vik.py` & `vik-1.0.3/vik/vik.py`

 * *Files identical despite different names*

