# Comparing `tmp/ivt-0.1.0.tar.gz` & `tmp/ivt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivt-0.1.0.tar", last modified: Mon Jun  5 10:06:23 2023, max compression
+gzip compressed data, was "ivt-0.1.1.tar", last modified: Mon Jun  5 11:04:25 2023, max compression
```

## Comparing `ivt-0.1.0.tar` & `ivt-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1123 2023-06-05 09:53:24.916313 ivt-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2097 2022-12-26 08:46:33.368156 ivt-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.0/LICENSE
--rw-r--r--   0        0        0     2262 2023-01-27 21:22:24.586035 ivt-0.1.0/README.md
--rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.0/docs/_templates/page.html
--rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.0/docs/conf.py
--rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.0/docs/core_install.rst
--rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.0/docs/core_intro.rst
--rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.0/docs/forward_intro.rst
--rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.0/docs/index.rst
--rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.0/docs/inverse_intro.rst
--rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.0/docs/plugin_refs.rst
--rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.0/docs/teaser.png
--rw-r--r--   0        0        0      269 2023-06-05 10:03:08.765120 ivt-0.1.0/ivt/__init__.py
--rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.0/ivt/config.py
--rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.0/ivt/connector.py
--rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.0/ivt/connectors/__init__.py
--rw-r--r--   0        0        0    14092 2023-06-05 09:53:24.918811 ivt-0.1.0/ivt/connectors/psdr_jit_connector.py
--rw-r--r--   0        0        0     3170 2023-06-05 09:53:24.919311 ivt-0.1.0/ivt/io.py
--rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.0/ivt/loss.py
--rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.0/ivt/model.py
--rw-r--r--   0        0        0     2417 2023-06-05 09:53:24.920312 ivt-0.1.0/ivt/parameter.py
--rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.0/ivt/renderer.py
--rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.0/ivt/sampling.py
--rw-r--r--   0        0        0     5729 2023-06-05 09:53:24.921811 ivt-0.1.0/ivt/scene.py
--rw-r--r--   0        0        0     3221 2023-06-05 09:53:24.922311 ivt-0.1.0/ivt/transform.py
--rw-r--r--   0        0        0      469 2023-06-05 10:02:03.225503 ivt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 ivt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-05 09:53:24.916313 ivt-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2097 2022-12-26 08:46:33.368156 ivt-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.1/LICENSE
+-rw-r--r--   0        0        0      776 2023-06-05 10:57:06.577472 ivt-0.1.1/README.md
+-rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.1/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.1/docs/_templates/page.html
+-rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.1/docs/core_install.rst
+-rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.1/docs/core_intro.rst
+-rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.1/docs/forward_intro.rst
+-rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.1/docs/inverse_intro.rst
+-rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.1/docs/plugin_refs.rst
+-rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.1/docs/teaser.png
+-rw-r--r--   0        0        0      269 2023-06-05 11:03:32.115809 ivt-0.1.1/ivt/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.1/ivt/config.py
+-rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.1/ivt/connector.py
+-rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.1/ivt/connectors/__init__.py
+-rw-r--r--   0        0        0    14092 2023-06-05 09:53:24.918811 ivt-0.1.1/ivt/connectors/psdr_jit_connector.py
+-rw-r--r--   0        0        0     3170 2023-06-05 09:53:24.919311 ivt-0.1.1/ivt/io.py
+-rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.1/ivt/loss.py
+-rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.1/ivt/model.py
+-rw-r--r--   0        0        0     2417 2023-06-05 09:53:24.920312 ivt-0.1.1/ivt/parameter.py
+-rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.1/ivt/renderer.py
+-rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.1/ivt/sampling.py
+-rw-r--r--   0        0        0     5729 2023-06-05 09:53:24.921811 ivt-0.1.1/ivt/scene.py
+-rw-r--r--   0        0        0     3221 2023-06-05 09:53:24.922311 ivt-0.1.1/ivt/transform.py
+-rw-r--r--   0        0        0      440 2023-06-05 10:20:47.334303 ivt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 ivt-0.1.1/PKG-INFO
```

### Comparing `ivt-0.1.0/.github/workflows/python-publish.yml` & `ivt-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/.gitignore` & `ivt-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/LICENSE` & `ivt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/docs/_static/theme_overrides.css` & `ivt-0.1.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/docs/conf.py` & `ivt-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/docs/index.rst` & `ivt-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/docs/teaser.png` & `ivt-0.1.1/docs/teaser.png`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/connector.py` & `ivt-0.1.1/ivt/connector.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/connectors/psdr_jit_connector.py` & `ivt-0.1.1/ivt/connectors/psdr_jit_connector.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/io.py` & `ivt-0.1.1/ivt/io.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/loss.py` & `ivt-0.1.1/ivt/loss.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/model.py` & `ivt-0.1.1/ivt/model.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/parameter.py` & `ivt-0.1.1/ivt/parameter.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/renderer.py` & `ivt-0.1.1/ivt/renderer.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/sampling.py` & `ivt-0.1.1/ivt/sampling.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/scene.py` & `ivt-0.1.1/ivt/scene.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.0/ivt/transform.py` & `ivt-0.1.1/ivt/transform.py`

 * *Files identical despite different names*

