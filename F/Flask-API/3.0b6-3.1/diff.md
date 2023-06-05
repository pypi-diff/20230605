# Comparing `tmp/Flask-API-3.0b6.tar.gz` & `tmp/Flask-API-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-API-3.0b6.tar", last modified: Fri Jun  4 21:14:38 2021, max compression
+gzip compressed data, was "Flask-API-3.1.tar", last modified: Mon Jun  5 16:49:48 2023, max compression
```

## Comparing `Flask-API-3.0b6.tar` & `Flask-API-3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.936626 Flask-API-3.0b6/
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.918574 Flask-API-3.0b6/Flask_API.egg-info/
--rw-r--r--   0 Browning   (501) staff       (20)      916 2021-06-04 21:14:38.000000 Flask-API-3.0b6/Flask_API.egg-info/PKG-INFO
--rw-r--r--   0 Browning   (501) staff       (20)     1801 2021-06-04 21:14:38.000000 Flask-API-3.0b6/Flask_API.egg-info/SOURCES.txt
--rw-r--r--   0 Browning   (501) staff       (20)        1 2021-06-04 21:14:38.000000 Flask-API-3.0b6/Flask_API.egg-info/dependency_links.txt
--rw-r--r--   0 Browning   (501) staff       (20)       11 2021-06-04 21:14:38.000000 Flask-API-3.0b6/Flask_API.egg-info/requires.txt
--rw-r--r--   0 Browning   (501) staff       (20)       26 2021-06-04 21:14:38.000000 Flask-API-3.0b6/Flask_API.egg-info/top_level.txt
--rw-r--r--   0 Browning   (501) staff       (20)     1458 2021-06-02 17:15:17.000000 Flask-API-3.0b6/LICENSE.md
--rw-r--r--   0 Browning   (501) staff       (20)      916 2021-06-04 21:14:38.936295 Flask-API-3.0b6/PKG-INFO
--rw-r--r--   0 Browning   (501) staff       (20)     4389 2021-06-02 17:15:17.000000 Flask-API-3.0b6/README.md
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.923491 Flask-API-3.0b6/flask_api/
--rw-r--r--   0 Browning   (501) staff       (20)       58 2021-06-04 21:10:34.000000 Flask-API-3.0b6/flask_api/__init__.py
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.927503 Flask-API-3.0b6/flask_api/__pycache__/
--rw-r--r--   0 Browning   (501) staff       (20)      213 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     4266 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/app.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)      922 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/compat.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     2572 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     4353 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/mediatypes.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     2204 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/negotiation.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     2560 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/parsers.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     4387 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/renderers.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     5697 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/request.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     1276 2021-06-02 18:19:53.000000 Flask-API-3.0b6/flask_api/__pycache__/response.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     2061 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     2985 2021-06-02 18:19:52.000000 Flask-API-3.0b6/flask_api/__pycache__/status.cpython-39.pyc
--rw-r--r--   0 Browning   (501) staff       (20)     4806 2021-06-04 18:54:20.000000 Flask-API-3.0b6/flask_api/app.py
--rw-r--r--   0 Browning   (501) staff       (20)      739 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/compat.py
--rw-r--r--   0 Browning   (501) staff       (20)      900 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/decorators.py
--rw-r--r--   0 Browning   (501) staff       (20)     2058 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/exceptions.py
--rw-r--r--   0 Browning   (501) staff       (20)     3686 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/mediatypes.py
--rw-r--r--   0 Browning   (501) staff       (20)     2029 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/negotiation.py
--rw-r--r--   0 Browning   (501) staff       (20)     2282 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/parsers.py
--rw-r--r--   0 Browning   (501) staff       (20)     4582 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/renderers.py
--rw-r--r--   0 Browning   (501) staff       (20)     6763 2021-06-04 21:10:22.000000 Flask-API-3.0b6/flask_api/request.py
--rw-r--r--   0 Browning   (501) staff       (20)     1268 2021-06-04 18:54:28.000000 Flask-API-3.0b6/flask_api/response.py
--rw-r--r--   0 Browning   (501) staff       (20)     1723 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/settings.py
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.915518 Flask-API-3.0b6/flask_api/static/
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.929155 Flask-API-3.0b6/flask_api/static/css/
--rw-r--r--   0 Browning   (501) staff       (20)     2764 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/css/bootstrap-tweaks.css
--rw-r--r--   0 Browning   (501) staff       (20)   118028 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/css/bootstrap.min.css
--rw-r--r--   0 Browning   (501) staff       (20)     1043 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/css/default.css
--rw-r--r--   0 Browning   (501) staff       (20)      817 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/css/prettify.css
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.930132 Flask-API-3.0b6/flask_api/static/img/
--rw-r--r--   0 Browning   (501) staff       (20)     8777 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/img/glyphicons-halflings-white.png
--rw-r--r--   0 Browning   (501) staff       (20)    12762 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/img/glyphicons-halflings.png
--rw-r--r--   0 Browning   (501) staff       (20)     1458 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/img/grid.png
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.931797 Flask-API-3.0b6/flask_api/static/js/
--rw-r--r--   0 Browning   (501) staff       (20)    25688 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/js/bootstrap.min.js
--rw-r--r--   0 Browning   (501) staff       (20)     1580 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/js/default.js
--rw-r--r--   0 Browning   (501) staff       (20)    92791 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/js/jquery-1.8.1-min.js
--rw-r--r--   0 Browning   (501) staff       (20)    13632 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/static/js/prettify-min.js
--rw-r--r--   0 Browning   (501) staff       (20)     2211 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/status.py
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.932131 Flask-API-3.0b6/flask_api/templates/
--rw-r--r--   0 Browning   (501) staff       (20)     8809 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/templates/base.html
-drwxr-xr-x   0 Browning   (501) staff       (20)        0 2021-06-04 21:14:38.935852 Flask-API-3.0b6/flask_api/tests/
--rw-r--r--   0 Browning   (501) staff       (20)      433 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/__init__.py
--rw-r--r--   0 Browning   (501) staff       (20)     6910 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_app.py
--rw-r--r--   0 Browning   (501) staff       (20)      830 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_exceptions.py
--rw-r--r--   0 Browning   (501) staff       (20)     5019 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_mediatypes.py
--rw-r--r--   0 Browning   (501) staff       (20)     3664 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_negotiation.py
--rw-r--r--   0 Browning   (501) staff       (20)     7352 2021-06-02 19:11:26.000000 Flask-API-3.0b6/flask_api/tests/test_parsers.py
--rw-r--r--   0 Browning   (501) staff       (20)     6501 2021-06-04 18:54:33.000000 Flask-API-3.0b6/flask_api/tests/test_renderers.py
--rw-r--r--   0 Browning   (501) staff       (20)     1660 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_request.py
--rw-r--r--   0 Browning   (501) staff       (20)      780 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_settings.py
--rw-r--r--   0 Browning   (501) staff       (20)     1218 2021-06-02 17:15:17.000000 Flask-API-3.0b6/flask_api/tests/test_status.py
--rw-r--r--   0 Browning   (501) staff       (20)       38 2021-06-04 21:14:38.936826 Flask-API-3.0b6/setup.cfg
--rwxr-xr-x   0 Browning   (501) staff       (20)     2481 2021-06-02 17:15:17.000000 Flask-API-3.0b6/setup.py
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.185966 Flask-API-3.1/
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.179407 Flask-API-3.1/Flask_API.egg-info/
+-rw-r--r--   0 Browning   (501) staff       (20)      909 2023-06-05 16:49:48.000000 Flask-API-3.1/Flask_API.egg-info/PKG-INFO
+-rw-r--r--   0 Browning   (501) staff       (20)     1801 2023-06-05 16:49:48.000000 Flask-API-3.1/Flask_API.egg-info/SOURCES.txt
+-rw-r--r--   0 Browning   (501) staff       (20)        1 2023-06-05 16:49:48.000000 Flask-API-3.1/Flask_API.egg-info/dependency_links.txt
+-rw-r--r--   0 Browning   (501) staff       (20)       13 2023-06-05 16:49:48.000000 Flask-API-3.1/Flask_API.egg-info/requires.txt
+-rw-r--r--   0 Browning   (501) staff       (20)       26 2023-06-05 16:49:48.000000 Flask-API-3.1/Flask_API.egg-info/top_level.txt
+-rw-r--r--   0 Browning   (501) staff       (20)     1458 2021-06-02 17:15:17.000000 Flask-API-3.1/LICENSE.md
+-rw-r--r--   0 Browning   (501) staff       (20)      909 2023-06-05 16:49:48.185813 Flask-API-3.1/PKG-INFO
+-rw-r--r--   0 Browning   (501) staff       (20)     4389 2021-06-02 17:15:17.000000 Flask-API-3.1/README.md
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.181154 Flask-API-3.1/flask_api/
+-rw-r--r--   0 Browning   (501) staff       (20)       56 2023-06-05 16:31:42.000000 Flask-API-3.1/flask_api/__init__.py
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.182722 Flask-API-3.1/flask_api/__pycache__/
+-rw-r--r--   0 Browning   (501) staff       (20)      213 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     4266 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/app.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)      922 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/compat.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     2572 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     4353 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/mediatypes.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     2204 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/negotiation.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     2560 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/parsers.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     4387 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/renderers.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     5697 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/request.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     1276 2021-06-02 18:19:53.000000 Flask-API-3.1/flask_api/__pycache__/response.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     2061 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     2985 2021-06-02 18:19:52.000000 Flask-API-3.1/flask_api/__pycache__/status.cpython-39.pyc
+-rw-r--r--   0 Browning   (501) staff       (20)     4799 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/app.py
+-rw-r--r--   0 Browning   (501) staff       (20)      657 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/compat.py
+-rw-r--r--   0 Browning   (501) staff       (20)      905 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/decorators.py
+-rw-r--r--   0 Browning   (501) staff       (20)     2020 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/exceptions.py
+-rw-r--r--   0 Browning   (501) staff       (20)     3677 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/mediatypes.py
+-rw-r--r--   0 Browning   (501) staff       (20)     1967 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/negotiation.py
+-rw-r--r--   0 Browning   (501) staff       (20)     2264 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/parsers.py
+-rw-r--r--   0 Browning   (501) staff       (20)     4477 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/renderers.py
+-rw-r--r--   0 Browning   (501) staff       (20)     6800 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/request.py
+-rw-r--r--   0 Browning   (501) staff       (20)     1214 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/response.py
+-rw-r--r--   0 Browning   (501) staff       (20)     1717 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/settings.py
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.178186 Flask-API-3.1/flask_api/static/
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.183298 Flask-API-3.1/flask_api/static/css/
+-rw-r--r--   0 Browning   (501) staff       (20)     2764 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/css/bootstrap-tweaks.css
+-rw-r--r--   0 Browning   (501) staff       (20)   118028 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/css/bootstrap.min.css
+-rw-r--r--   0 Browning   (501) staff       (20)     1043 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/css/default.css
+-rw-r--r--   0 Browning   (501) staff       (20)      817 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/css/prettify.css
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.183720 Flask-API-3.1/flask_api/static/img/
+-rw-r--r--   0 Browning   (501) staff       (20)     8777 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/img/glyphicons-halflings-white.png
+-rw-r--r--   0 Browning   (501) staff       (20)    12762 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/img/glyphicons-halflings.png
+-rw-r--r--   0 Browning   (501) staff       (20)     1458 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/img/grid.png
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.184286 Flask-API-3.1/flask_api/static/js/
+-rw-r--r--   0 Browning   (501) staff       (20)    25688 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/js/bootstrap.min.js
+-rw-r--r--   0 Browning   (501) staff       (20)     1580 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/js/default.js
+-rw-r--r--   0 Browning   (501) staff       (20)    92791 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/js/jquery-1.8.1-min.js
+-rw-r--r--   0 Browning   (501) staff       (20)    13632 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/static/js/prettify-min.js
+-rw-r--r--   0 Browning   (501) staff       (20)     2156 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/status.py
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.184412 Flask-API-3.1/flask_api/templates/
+-rw-r--r--   0 Browning   (501) staff       (20)     8809 2021-06-02 17:15:17.000000 Flask-API-3.1/flask_api/templates/base.html
+drwxr-xr-x   0 Browning   (501) staff       (20)        0 2023-06-05 16:49:48.185633 Flask-API-3.1/flask_api/tests/
+-rw-r--r--   0 Browning   (501) staff       (20)      422 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/__init__.py
+-rw-r--r--   0 Browning   (501) staff       (20)     6888 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_app.py
+-rw-r--r--   0 Browning   (501) staff       (20)      755 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_exceptions.py
+-rw-r--r--   0 Browning   (501) staff       (20)     5088 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_mediatypes.py
+-rw-r--r--   0 Browning   (501) staff       (20)     3633 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_negotiation.py
+-rw-r--r--   0 Browning   (501) staff       (20)     7320 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_parsers.py
+-rw-r--r--   0 Browning   (501) staff       (20)     6507 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_renderers.py
+-rw-r--r--   0 Browning   (501) staff       (20)     1609 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_request.py
+-rw-r--r--   0 Browning   (501) staff       (20)      726 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_settings.py
+-rw-r--r--   0 Browning   (501) staff       (20)     1164 2023-06-05 16:31:00.000000 Flask-API-3.1/flask_api/tests/test_status.py
+-rw-r--r--   0 Browning   (501) staff       (20)       38 2023-06-05 16:49:48.186009 Flask-API-3.1/setup.cfg
+-rwxr-xr-x   0 Browning   (501) staff       (20)     2424 2023-06-05 16:31:00.000000 Flask-API-3.1/setup.py
```

### Comparing `Flask-API-3.0b6/Flask_API.egg-info/PKG-INFO` & `Flask-API-3.1/Flask_API.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Flask-API
-Version: 3.0b6
+Version: 3.1
 Summary: Browsable web APIs for Flask.
 Home-page: https://flask-api.github.io/flask-api/
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
-Description: Browsable web APIs for Flask.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
+License-File: LICENSE.md
+
+Browsable web APIs for Flask.
```

### Comparing `Flask-API-3.0b6/Flask_API.egg-info/SOURCES.txt` & `Flask-API-3.1/Flask_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/LICENSE.md` & `Flask-API-3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/PKG-INFO` & `Flask-API-3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Flask-API
-Version: 3.0b6
+Version: 3.1
 Summary: Browsable web APIs for Flask.
 Home-page: https://flask-api.github.io/flask-api/
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
-Description: Browsable web APIs for Flask.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
+License-File: LICENSE.md
+
+Browsable web APIs for Flask.
```

### Comparing `Flask-API-3.0b6/README.md` & `Flask-API-3.1/README.md`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/app.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/compat.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/compat.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/exceptions.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/mediatypes.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/mediatypes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/negotiation.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/negotiation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/parsers.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/parsers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/renderers.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/renderers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/request.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/request.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/response.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/settings.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/__pycache__/status.cpython-39.pyc` & `Flask-API-3.1/flask_api/__pycache__/status.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/app.py` & `Flask-API-3.1/flask_api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import request, Flask, Blueprint
+import re
+import sys
+from itertools import chain
+
+from flask import Blueprint, Flask, request
+from werkzeug.exceptions import HTTPException
+
+from flask_api.compat import is_flask_legacy
 from flask_api.exceptions import APIException
 from flask_api.request import APIRequest
 from flask_api.response import APIResponse
 from flask_api.settings import APISettings
 from flask_api.status import HTTP_204_NO_CONTENT
-from itertools import chain
-from werkzeug.exceptions import HTTPException
-import re
-import sys
-from flask_api.compat import is_flask_legacy
-
 
 api_resources = Blueprint(
-    'flask-api', __name__,
-    url_prefix='/flask-api',
-    template_folder='templates', static_folder='static'
+    "flask-api",
+    __name__,
+    url_prefix="/flask-api",
+    template_folder="templates",
+    static_folder="static",
 )
 
 
 def urlize_quoted_links(content):
     return re.sub(r'"(https?://[^"]*)"', r'"<a href="\1">\1</a>"', content)
 
 
@@ -28,15 +29,15 @@
     request_class = APIRequest
     response_class = APIResponse
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.api_settings = APISettings(self.config)
         self.register_blueprint(api_resources)
-        self.jinja_env.filters['urlize_quoted_links'] = urlize_quoted_links
+        self.jinja_env.filters["urlize_quoted_links"] = urlize_quoted_links
 
     def preprocess_request(self):
         request.parser_classes = self.api_settings.DEFAULT_PARSERS
         request.renderer_classes = self.api_settings.DEFAULT_RENDERERS
         return super().preprocess_request()
 
     def make_response(self, rv):
@@ -45,18 +46,18 @@
         list and dict types by default.
         """
         status_or_headers = headers = None
         if isinstance(rv, tuple):
             rv, status_or_headers, headers = rv + (None,) * (3 - len(rv))
 
         if rv is None and status_or_headers == HTTP_204_NO_CONTENT:
-            rv = ''
+            rv = ""
 
         if rv is None and status_or_headers:
-            raise ValueError('View function did not return a response')
+            raise ValueError("View function did not return a response")
 
         if isinstance(status_or_headers, (dict, list)):
             headers, status_or_headers = status_or_headers, None
 
         if not isinstance(rv, self.response_class):
             if isinstance(rv, (str, bytes, bytearray, list, dict)):
                 status = status_or_headers
@@ -94,38 +95,41 @@
             blueprint_handlers = handlers.get(None, ())
         app_handlers = self.error_handler_spec[None].get(None, ())
         if is_flask_legacy():
             for typecheck, handler in chain(blueprint_handlers, app_handlers):
                 if isinstance(e, typecheck):
                     return handler(e)
         else:
-            for typecheck, handler in chain(dict(blueprint_handlers).items(),
-                    dict(app_handlers).items()):
+            for typecheck, handler in chain(
+                dict(blueprint_handlers).items(), dict(app_handlers).items()
+            ):
                 if isinstance(e, typecheck):
                     return handler(e)
 
         raise e
 
     def handle_api_exception(self, exc):
-        content = {'message': exc.detail}
+        content = {"message": exc.detail}
         status = exc.status_code
         return self.response_class(content, status=status)
 
     def create_url_adapter(self, request):
         """
         We need to override the default behavior slightly here,
         to ensure the any method-based routing takes account of
         any method overloading, so that eg PUT requests from the
         browsable API are routed to the correct view.
         """
         if request is not None:
             environ = request.environ.copy()
-            environ['REQUEST_METHOD'] = request.method
-            return self.url_map.bind_to_environ(environ,
-                server_name=self.config['SERVER_NAME'])
+            environ["REQUEST_METHOD"] = request.method
+            return self.url_map.bind_to_environ(
+                environ, server_name=self.config["SERVER_NAME"]
+            )
         # We need at the very least the server name to be set for this
         # to work.
-        if self.config['SERVER_NAME'] is not None:
+        if self.config["SERVER_NAME"] is not None:
             return self.url_map.bind(
-                self.config['SERVER_NAME'],
-                script_name=self.config['APPLICATION_ROOT'] or '/',
-                url_scheme=self.config['PREFERRED_URL_SCHEME'])
+                self.config["SERVER_NAME"],
+                script_name=self.config["APPLICATION_ROOT"] or "/",
+                url_scheme=self.config["PREFERRED_URL_SCHEME"],
+            )
```

### Comparing `Flask-API-3.0b6/flask_api/compat.py` & `Flask-API-3.1/flask_api/compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals, absolute_import
 from flask import __version__ as flask_version
 
 # Markdown is optional
 try:
     import markdown
     from markdown.extensions.toc import TocExtension
 
@@ -13,15 +11,14 @@
         of '#' style headers to <h2>.
         """
 
         extensions = [TocExtension(baselevel=2)]
         md = markdown.Markdown(extensions=extensions)
         return md.convert(text)
 
-
 except ImportError:  # pragma: no cover - markdown installed for tests
     apply_markdown = None
 
 
 def is_flask_legacy():
     v = flask_version.split(".")
     return int(v[0]) == 0 and int(v[1]) < 11
```

### Comparing `Flask-API-3.0b6/flask_api/decorators.py` & `Flask-API-3.1/flask_api/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from functools import wraps
+
 from flask import request
 
 
 def set_parsers(*parsers):
     def decorator(func):
         @wraps(func)
         def decorated_function(*args, **kwargs):
             if len(parsers) == 1 and isinstance(parsers[0], (list, tuple)):
                 request.parser_classes = parsers[0]
             else:
                 request.parser_classes = parsers
             return func(*args, **kwargs)
+
         return decorated_function
+
     return decorator
 
 
 def set_renderers(*renderers):
     def decorator(func):
         @wraps(func)
         def decorated_function(*args, **kwargs):
             if len(renderers) == 1 and isinstance(renderers[0], (list, tuple)):
                 request.renderer_classes = renderers[0]
             else:
                 request.renderer_classes = renderers
             return func(*args, **kwargs)
+
         return decorated_function
+
     return decorator
```

### Comparing `Flask-API-3.0b6/flask_api/exceptions.py` & `Flask-API-3.1/flask_api/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-from __future__ import unicode_literals
 from flask_api import status
 
 
 class APIException(Exception):
     status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
-    detail = ''
+    detail = ""
 
     def __init__(self, detail=None):
         if detail is not None:
             self.detail = detail
 
     def __str__(self):
         return self.detail
 
 
 class ParseError(APIException):
     status_code = status.HTTP_400_BAD_REQUEST
-    detail = 'Malformed request.'
+    detail = "Malformed request."
 
 
 class AuthenticationFailed(APIException):
     status_code = status.HTTP_401_UNAUTHORIZED
-    detail = 'Incorrect authentication credentials.'
+    detail = "Incorrect authentication credentials."
 
 
 class NotAuthenticated(APIException):
     status_code = status.HTTP_401_UNAUTHORIZED
-    detail = 'Authentication credentials were not provided.'
+    detail = "Authentication credentials were not provided."
 
 
 class PermissionDenied(APIException):
     status_code = status.HTTP_403_FORBIDDEN
-    detail = 'You do not have permission to perform this action.'
+    detail = "You do not have permission to perform this action."
 
 
 class NotFound(APIException):
     status_code = status.HTTP_404_NOT_FOUND
-    detail = 'This resource does not exist.'
+    detail = "This resource does not exist."
+
 
 # class MethodNotAllowed(APIException):
 #     status_code = status.HTTP_405_METHOD_NOT_ALLOWED
 #     detail = 'Request method "%s" not allowed.'
 
 #     def __init__(self, method, detail=None):
 #         self.detail = (detail or self.detail) % method
 
 
 class NotAcceptable(APIException):
     status_code = status.HTTP_406_NOT_ACCEPTABLE
-    detail = 'Could not satisfy the request Accept header.'
+    detail = "Could not satisfy the request Accept header."
 
 
 class UnsupportedMediaType(APIException):
     status_code = status.HTTP_415_UNSUPPORTED_MEDIA_TYPE
-    detail = 'Unsupported media type in the request Content-Type header.'
+    detail = "Unsupported media type in the request Content-Type header."
 
 
 class Throttled(APIException):
     status_code = status.HTTP_429_TOO_MANY_REQUESTS
-    detail = 'Request was throttled.'
+    detail = "Request was throttled."
+
 
 #     def __init__(self, wait=None, detail=None):
 #         if wait is None:
 #             self.detail = detail or self.detail
 #             self.wait = None
 #         else:
 #             format = (detail or self.detail) + ' ' + self.extra_detail
```

### Comparing `Flask-API-3.0b6/flask_api/mediatypes.py` & `Flask-API-3.1/flask_api/mediatypes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,100 @@
-# coding: utf8
-from __future__ import unicode_literals
-
-
-class MediaType(object):
+class MediaType:
     def __init__(self, media_type):
         self.main_type, self.sub_type, self.params = self._parse(media_type)
 
     @property
     def full_type(self):
-        return self.main_type + '/' + self.sub_type
+        return self.main_type + "/" + self.sub_type
 
     @property
     def precedence(self):
         """
         Precedence is determined by how specific a media type is:
 
         3. 'type/subtype; param=val'
         2. 'type/subtype'
         1. 'type/*'
         0. '*/*'
         """
-        if self.main_type == '*':
+        if self.main_type == "*":
             return 0
-        elif self.sub_type == '*':
+        elif self.sub_type == "*":
             return 1
-        elif not self.params or list(self.params.keys()) == ['q']:
+        elif not self.params or list(self.params.keys()) == ["q"]:
             return 2
         return 3
 
     def satisfies(self, other):
         """
         Returns `True` if this media type is a superset of `other`.
         Some examples of cases where this holds true:
 
         'application/json; version=1.0' >= 'application/json; version=1.0'
         'application/json'              >= 'application/json; indent=4'
         'text/*'                        >= 'text/plain'
         '*/*'                           >= 'text/plain'
         """
         for key in self.params.keys():
-            if key != 'q' and other.params.get(key, None) != self.params.get(key, None):
+            if key != "q" and other.params.get(key, None) != self.params.get(key, None):
                 return False
 
-        if self.sub_type != '*' and other.sub_type != '*' and other.sub_type != self.sub_type:
+        if (
+            self.sub_type != "*"
+            and other.sub_type != "*"
+            and other.sub_type != self.sub_type
+        ):
             return False
 
-        if self.main_type != '*' and other.main_type != '*' and other.main_type != self.main_type:
+        if (
+            self.main_type != "*"
+            and other.main_type != "*"
+            and other.main_type != self.main_type
+        ):
             return False
 
         return True
 
     def _parse(self, media_type):
         """
         Parse a media type string, like "application/json; indent=4" into a
         three-tuple, like: ('application', 'json', {'indent': 4})
         """
-        full_type, sep, param_string = media_type.partition(';')
+        full_type, sep, param_string = media_type.partition(";")
         params = {}
-        for token in param_string.strip().split(','):
-            key, sep, value = [s.strip() for s in token.partition('=')]
+        for token in param_string.strip().split(","):
+            key, sep, value = [s.strip() for s in token.partition("=")]
             if value.startswith('"') and value.endswith('"'):
                 value = value[1:-1]
             if key:
                 params[key] = value
-        main_type, sep, sub_type = [s.strip() for s in full_type.partition('/')]
+        main_type, sep, sub_type = [s.strip() for s in full_type.partition("/")]
         return (main_type, sub_type, params)
 
     def __repr__(self):
         return "<%s '%s'>" % (self.__class__.__name__, str(self))
 
     def __str__(self):
         """
         Return a canonical string representing the media type.
         Note that this ensures the params are sorted.
         """
         if self.params:
-            params_str = ', '.join([
-                '%s="%s"' % (key, val)
-                for key, val in sorted(self.params.items())
-            ])
-            return self.full_type + '; ' + params_str
+            params_str = ", ".join(
+                ['%s="%s"' % (key, val) for key, val in sorted(self.params.items())]
+            )
+            return self.full_type + "; " + params_str
         return self.full_type
 
     def __hash__(self):
         return hash(str(self))
 
     def __eq__(self, other):
         # Compare two MediaType instances, ignoring parameter ordering.
-        return (
-            self.full_type == other.full_type and self.params == other.params
-        )
+        return self.full_type == other.full_type and self.params == other.params
 
 
 def parse_accept_header(accept):
     """
     Parses the value of a clients accept header, and returns a list of sets
     of media types it included, ordered by precedence.
 
@@ -101,11 +102,11 @@
 
     [
         set([<MediaType "application/xml">, <MediaType "application/json">]),
         set([<MediaType "*/*">])
     ]
     """
     ret = [set(), set(), set(), set()]
-    for token in accept.split(','):
+    for token in accept.split(","):
         media_type = MediaType(token.strip())
         ret[3 - media_type.precedence].add(media_type)
     return [media_types for media_types in ret if media_types]
```

### Comparing `Flask-API-3.0b6/flask_api/negotiation.py` & `Flask-API-3.1/flask_api/negotiation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# coding: utf8
-from __future__ import unicode_literals
 from flask import request
+
 from flask_api import exceptions
 from flask_api.mediatypes import MediaType, parse_accept_header
 
 
-class BaseNegotiation(object):
+class BaseNegotiation:
     def select_parser(self, parsers):
         msg = '`select_parser()` method must be implemented for class "%s"'
         raise NotImplementedError(msg % self.__class__.__name__)
 
     def select_renderer(self, renderers):
         msg = '`select_renderer()` method must be implemented for class "%s"'
         raise NotImplementedError(msg % self.__class__.__name__)
@@ -32,15 +31,15 @@
         raise exceptions.UnsupportedMediaType()
 
     def select_renderer(self, renderers):
         """
         Determine which renderer to use for rendering the response body.
         Returns a two-tuple of (renderer, content type).
         """
-        accept_header = request.headers.get('Accept', '*/*')
+        accept_header = request.headers.get("Accept", "*/*")
 
         for client_media_types in parse_accept_header(accept_header):
             for renderer in renderers:
                 server_media_type = MediaType(renderer.media_type)
                 for client_media_type in client_media_types:
                     if client_media_type.satisfies(server_media_type):
                         if server_media_type.precedence > client_media_type.precedence:
```

### Comparing `Flask-API-3.0b6/flask_api/parsers.py` & `Flask-API-3.1/flask_api/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask_api import exceptions
+import json
+
 from werkzeug.formparser import MultiPartParser as WerkzeugMultiPartParser
 from werkzeug.formparser import default_stream_factory
 from werkzeug.urls import url_decode_stream
-import json
+
+from flask_api import exceptions
 
 
-class BaseParser(object):
+class BaseParser:
     media_type = None
     handles_file_uploads = False  # If set then 'request.files' will be populated.
-    handles_form_data = False     # If set then 'request.form' will be populated.
+    handles_form_data = False  # If set then 'request.form' will be populated.
 
     def parse(self, stream, media_type, **options):
         msg = '`parse()` method must be implemented for class "%s"'
         raise NotImplementedError(msg % self.__class__.__name__)
 
 
 class JSONParser(BaseParser):
-    media_type = 'application/json'
+    media_type = "application/json"
 
     def parse(self, stream, media_type, **options):
-        data = stream.read().decode('utf-8')
+        data = stream.read().decode("utf-8")
         try:
             return json.loads(data)
         except ValueError as exc:
-            msg = 'JSON parse error - %s' % str(exc)
+            msg = "JSON parse error - %s" % str(exc)
             raise exceptions.ParseError(msg)
 
 
 class MultiPartParser(BaseParser):
-    media_type = 'multipart/form-data'
+    media_type = "multipart/form-data"
     handles_file_uploads = True
     handles_form_data = True
 
     def parse(self, stream, media_type, **options):
-        boundary = media_type.params.get('boundary')
+        boundary = media_type.params.get("boundary")
         if boundary is None:
-            msg = 'Multipart message missing boundary in Content-Type header'
+            msg = "Multipart message missing boundary in Content-Type header"
             raise exceptions.ParseError(msg)
-        boundary = boundary.encode('ascii')
+        boundary = boundary.encode("ascii")
 
-        content_length = options.get('content_length')
-        assert content_length is not None, 'MultiPartParser.parse() requires `content_length` argument'
+        content_length = options.get("content_length")
+        assert (
+            content_length is not None
+        ), "MultiPartParser.parse() requires `content_length` argument"
 
         buffer_size = content_length
         while buffer_size % 4 or buffer_size < 1024:
             buffer_size += 1
-        multipart_parser = WerkzeugMultiPartParser(default_stream_factory, buffer_size=buffer_size)
+        multipart_parser = WerkzeugMultiPartParser(
+            default_stream_factory, buffer_size=buffer_size
+        )
 
         try:
             return multipart_parser.parse(stream, boundary, content_length)
         except ValueError as exc:
-            msg = 'Multipart parse error - %s' % str(exc)
+            msg = "Multipart parse error - %s" % str(exc)
             raise exceptions.ParseError(msg)
 
 
 class URLEncodedParser(BaseParser):
-    media_type = 'application/x-www-form-urlencoded'
+    media_type = "application/x-www-form-urlencoded"
     handles_form_data = True
 
     def parse(self, stream, media_type, **options):
         return url_decode_stream(stream)
```

### Comparing `Flask-API-3.0b6/flask_api/renderers.py` & `Flask-API-3.1/flask_api/renderers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,98 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import request, render_template, current_app
-from flask.globals import _request_ctx_stack
-from flask_api.mediatypes import MediaType
-from flask_api.compat import apply_markdown
-import json
 import pydoc
 import re
 
+from flask import current_app, render_template, request
+from flask.globals import _request_ctx_stack
+
+from flask_api.compat import apply_markdown
+from flask_api.mediatypes import MediaType
+
 
 def dedent(content):
     """
     Remove leading indent from a block of text.
     Used when generating descriptions from docstrings.
 
     Note that python's `textwrap.dedent` doesn't quite cut it,
     as it fails to dedent multiline docstrings that include
     unindented text on the initial line.
     """
-    whitespace_counts = [len(line) - len(line.lstrip(' '))
-                         for line in content.splitlines()[1:] if line.lstrip()]
+    whitespace_counts = [
+        len(line) - len(line.lstrip(" "))
+        for line in content.splitlines()[1:]
+        if line.lstrip()
+    ]
 
     # unindent the content if needed
     if whitespace_counts:
-        whitespace_pattern = '^' + (' ' * min(whitespace_counts))
-        content = re.sub(re.compile(whitespace_pattern, re.MULTILINE), '', content)
+        whitespace_pattern = "^" + (" " * min(whitespace_counts))
+        content = re.sub(re.compile(whitespace_pattern, re.MULTILINE), "", content)
 
     return content.strip()
 
 
 def convert_to_title(name):
-    for char in ['-', '_', '.']:
-        name = name.replace(char, ' ')
+    for char in ["-", "_", "."]:
+        name = name.replace(char, " ")
     return name.capitalize()
 
 
-class BaseRenderer(object):
+class BaseRenderer:
     media_type = None
-    charset = 'utf-8'
+    charset = "utf-8"
     handles_empty_responses = False
 
     def render(self, data, media_type, **options):
         msg = '`render()` method must be implemented for class "%s"'
         raise NotImplementedError(msg % self.__class__.__name__)
 
 
 class JSONRenderer(BaseRenderer):
-    media_type = 'application/json'
+    media_type = "application/json"
     charset = None
 
     def render(self, data, media_type, **options):
         # Requested indentation may be set in the Accept header.
         try:
-            indent = max(min(int(media_type.params['indent']), 8), 0)
+            indent = max(min(int(media_type.params["indent"]), 8), 0)
         except (KeyError, ValueError, TypeError):
             indent = None
         # Indent may be set explicitly, eg when rendered by the browsable API.
-        indent = options.get('indent', indent)
-        return json.dumps(data, cls=current_app.json_encoder, ensure_ascii=False, indent=indent)
+        indent = options.get("indent", indent)
+        return current_app.json.dumps(
+            data, ensure_ascii=False, indent=indent
+        )
 
 
-class HTMLRenderer(object):
-    media_type = 'text/html'
-    charset = 'utf-8'
+class HTMLRenderer:
+    media_type = "text/html"
+    charset = "utf-8"
 
     def render(self, data, media_type, **options):
         return data.encode(self.charset)
 
 
 class BrowsableAPIRenderer(BaseRenderer):
-    media_type = 'text/html'
+    media_type = "text/html"
     handles_empty_responses = True
-    template = 'base.html'
+    template = "base.html"
 
     def render(self, data, media_type, **options):
         # Render the content as it would have been if the client
         # had requested 'Accept: */*'.
         available_renderers = [
-            renderer for renderer in request.renderer_classes
+            renderer
+            for renderer in request.renderer_classes
             if not issubclass(renderer, BrowsableAPIRenderer)
         ]
-        assert available_renderers, 'BrowsableAPIRenderer cannot be the only renderer'
+        assert available_renderers, "BrowsableAPIRenderer cannot be the only renderer"
         mock_renderer = available_renderers[0]()
         mock_media_type = MediaType(mock_renderer.media_type)
-        if data == '' and not mock_renderer.handles_empty_responses:
+        if data == "" and not mock_renderer.handles_empty_responses:
             mock_content = None
         else:
             text = mock_renderer.render(data, mock_media_type, indent=4)
             mock_content = self._html_escape(text)
 
         # Determine the allowed methods on this view.
         adapter = _request_ctx_stack.top.url_adapter
@@ -100,36 +105,32 @@
             if apply_markdown:
                 view_description = dedent(view_description)
                 view_description = apply_markdown(view_description)
             else:  # pragma: no cover - markdown installed for tests
                 view_description = dedent(view_description)
                 view_description = pydoc.html.preformat(view_description)
 
-        status = options['status']
-        headers = options['headers']
-        headers['Content-Type'] = str(mock_media_type)
+        status = options["status"]
+        headers = options["headers"]
+        headers["Content-Type"] = str(mock_media_type)
 
         from flask_api import __version__
 
         context = {
-            'status': status,
-            'headers': headers,
-            'content': mock_content,
-            'allowed_methods': allowed_methods,
-            'view_name': convert_to_title(view_name),
-            'view_description': view_description,
-            'version': __version__
+            "status": status,
+            "headers": headers,
+            "content": mock_content,
+            "allowed_methods": allowed_methods,
+            "view_name": convert_to_title(view_name),
+            "view_description": view_description,
+            "version": __version__,
         }
         return render_template(self.template, **context)
 
     @staticmethod
     def _html_escape(text):
-        escape_table = [
-            ("&", "&amp;"),
-            ("<", "&lt;"),
-            (">", "&gt;")
-        ]
+        escape_table = [("&", "&amp;"), ("<", "&lt;"), (">", "&gt;")]
 
         for char, replacement in escape_table:
             text = text.replace(char, replacement)
 
         return text
```

### Comparing `Flask-API-3.0b6/flask_api/request.py` & `Flask-API-3.1/flask_api/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# coding: utf8
-from __future__ import unicode_literals
+import io
+
 from flask import Request
-from flask_api.negotiation import DefaultNegotiation
-from flask_api.settings import default_settings
 from werkzeug.datastructures import MultiDict
 from werkzeug.urls import url_decode_stream
 from werkzeug.wsgi import get_content_length
-import io
+
+from flask_api.negotiation import DefaultNegotiation
+from flask_api.settings import default_settings
 
 
 class APIRequest(Request):
     parser_classes = default_settings.DEFAULT_PARSERS
     renderer_classes = default_settings.DEFAULT_RENDERERS
     negotiator_class = DefaultNegotiation
     empty_data_class = MultiDict
 
     # Request parsing...
 
     @property
     def data(self):
-        if not hasattr(self, '_data'):
+        if not hasattr(self, "_data"):
             self._parse()
         return self._data
 
     @property
     def form(self):
-        if not hasattr(self, '_form'):
+        if not hasattr(self, "_form"):
             self._parse()
         return self._form
 
     @property
     def files(self):
-        if not hasattr(self, '_files'):
+        if not hasattr(self, "_files"):
             self._parse()
         return self._files
 
     def _parse(self):
         """
         Parse the body of the request, using whichever parser satisfies the
         client 'Content-Type' header.
@@ -53,131 +53,138 @@
         except Exception as e:
             # Ensure that accessing `request.data` again does not reraise
             # the exception, so that eg exceptions can handle properly.
             self._set_empty_data()
             raise e from None
 
         if parser.handles_file_uploads:
-            assert isinstance(ret, tuple) and len(ret) == 2, 'Expected a two-tuple of (data, files)'
+            assert (
+                isinstance(ret, tuple) and len(ret) == 2
+            ), "Expected a two-tuple of (data, files)"
             self._data, self._files = ret
         else:
             self._data = ret
             self._files = self.empty_data_class()
 
         self._form = self._data if parser.handles_form_data else self.empty_data_class()
 
     def _get_parser_options(self):
         """
         Any additional information to pass to the parser.
         """
-        return {'content_length': self.content_length}
+        return {"content_length": self.content_length}
 
     def _set_empty_data(self):
         """
         If the request does not contain data then return an empty representation.
         """
         self._data = self.empty_data_class()
         self._form = self.empty_data_class()
         self._files = self.empty_data_class()
 
     # Content negotiation...
 
     @property
     def accepted_renderer(self):
-        if not hasattr(self, '_accepted_renderer'):
+        if not hasattr(self, "_accepted_renderer"):
             self._perform_content_negotiation()
         return self._accepted_renderer
 
     @property
     def accepted_media_type(self):
-        if not hasattr(self, '_accepted_media_type'):
+        if not hasattr(self, "_accepted_media_type"):
             self._perform_content_negotiation()
         return self._accepted_media_type
 
     def _perform_content_negotiation(self):
         """
         Determine which of the available renderers should be used for
         rendering the response content, based on the client 'Accept' header.
         """
         negotiator = self.negotiator_class()
         renderers = [renderer() for renderer in self.renderer_classes]
-        self._accepted_renderer, self._accepted_media_type = negotiator.select_renderer(renderers)
+        self._accepted_renderer, self._accepted_media_type = negotiator.select_renderer(
+            renderers
+        )
 
     # Method and content type overloading.
 
     @property
     def method(self):
-        if not hasattr(self, '_method'):
+        if not hasattr(self, "_method"):
             self._perform_method_overloading()
         return self._method
 
     @method.setter
     def method(self, value):
         self._method = value
 
     @property
     def content_type(self):
-        if not hasattr(self, '_content_type'):
+        if not hasattr(self, "_content_type"):
             self._perform_method_overloading()
         return self._content_type
 
     @property
     def content_length(self):
-        if not hasattr(self, '_content_length'):
+        if not hasattr(self, "_content_length"):
             self._perform_method_overloading()
         return self._content_length
 
     @property
     def stream(self):
-        if not hasattr(self, '_stream'):
+        if not hasattr(self, "_stream"):
             self._perform_method_overloading()
         return self._stream
 
     def _perform_method_overloading(self):
         """
         Perform method and content type overloading.
 
         Provides support for browser PUT, PATCH, DELETE & other requests,
-        by specifing a '_method' form field.
+        by specifying a '_method' form field.
 
         Also provides support for browser non-form requests (eg JSON),
-        by specifing '_content' and '_content_type' form fields.
+        by specifying '_content' and '_content_type' form fields.
         """
-        if not hasattr(self, '_method'):
+        if not hasattr(self, "_method"):
             self.method = super().method
         self._stream = super().stream
-        self._content_type = self.headers.get('Content-Type')
+        self._content_type = self.headers.get("Content-Type")
         self._content_length = get_content_length(self.environ)
 
-        if (self._method == 'POST' and self._content_type == 'application/x-www-form-urlencoded'):
+        if (
+            self._method == "POST"
+            and self._content_type == "application/x-www-form-urlencoded"
+        ):
             # Read the request data, then push it back onto the stream again.
             body = self.get_data()
             data = url_decode_stream(io.BytesIO(body))
             self._stream = io.BytesIO(body)
-            if '_method' in data:
+            if "_method" in data:
                 # Support browser forms with PUT, PATCH, DELETE & other methods.
-                self._method = data['_method']
-            if '_content' in data and '_content_type' in data:
+                self._method = data["_method"]
+            if "_content" in data and "_content_type" in data:
                 # Support browser forms with non-form data, such as JSON.
-                body = data['_content'].encode('utf8')
+                body = data["_content"].encode("utf8")
                 self._stream = io.BytesIO(body)
-                self._content_type = data['_content_type']
+                self._content_type = data["_content_type"]
                 self._content_length = len(body)
 
     # Misc...
 
     @property
     def full_path(self):
         """
         Werzueg's full_path implementation always appends '?', even when the
         query string is empty.  Let's fix that.
         """
         if not self.query_string:
             return self.path
-        return self.path + '?' + self.query_string.decode()
+        return self.path + "?" + self.query_string.decode()
 
     # @property
     # def auth(self):
     #     if not has_attribute(self, '_auth'):
     #         self._authenticate()
     #     return self._auth
```

### Comparing `Flask-API-3.0b6/flask_api/response.py` & `Flask-API-3.1/flask_api/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import request, Response
+from flask import Response, request
 
 
 class APIResponse(Response):
 
     api_return_types = (list, dict)
 
     def __init__(self, content=None, *args, **kwargs):
         super().__init__(None, *args, **kwargs)
 
         media_type = None
-        if isinstance(content, self.api_return_types) or content == '':
+        if isinstance(content, self.api_return_types) or content == "":
             renderer = request.accepted_renderer
-            if content != '' or renderer.handles_empty_responses:
+            if content != "" or renderer.handles_empty_responses:
                 media_type = request.accepted_media_type
                 options = self.get_renderer_options()
                 content = renderer.render(content, media_type, **options)
                 if self.status_code == 204:
                     self.status_code = 200
 
         # From `werkzeug.wrappers.BaseResponse`
@@ -25,15 +23,15 @@
             content = []
         if isinstance(content, (str, bytes, bytearray)):
             self.set_data(content)
         else:
             self.response = content
 
         if media_type is not None:
-            self.headers['Content-Type'] = str(media_type)
+            self.headers["Content-Type"] = str(media_type)
 
     def get_renderer_options(self):
         return {
-            'status': self.status,
-            'status_code': self.status_code,
-            'headers': self.headers
+            "status": self.status,
+            "status_code": self.status_code,
+            "headers": self.headers,
         }
```

### Comparing `Flask-API-3.0b6/flask_api/settings.py` & `Flask-API-3.1/flask_api/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 
 def import_from_string(val, setting_name):
     """
     Attempt to import a class from a string representation.
     """
     try:
         # Nod to tastypie's use of importlib.
-        parts = val.split('.')
-        module_path, class_name = '.'.join(parts[:-1]), parts[-1]
+        parts = val.split(".")
+        module_path, class_name = ".".join(parts[:-1]), parts[-1]
         module = importlib.import_module(module_path)
         return getattr(module, class_name)
     except ImportError as exc:
         format = "Could not import '%s' for API setting '%s'. %s."
         msg = format % (val, setting_name, exc)
         raise ImportError(msg)
 
 
-class APISettings(object):
+class APISettings:
     def __init__(self, user_config=None):
         self.user_config = user_config or {}
 
     @property
     def DEFAULT_PARSERS(self):
         default = [
-            'flask_api.parsers.JSONParser',
-            'flask_api.parsers.URLEncodedParser',
-            'flask_api.parsers.MultiPartParser'
+            "flask_api.parsers.JSONParser",
+            "flask_api.parsers.URLEncodedParser",
+            "flask_api.parsers.MultiPartParser",
         ]
-        val = self.user_config.get('DEFAULT_PARSERS', default)
-        return perform_imports(val, 'DEFAULT_PARSERS')
+        val = self.user_config.get("DEFAULT_PARSERS", default)
+        return perform_imports(val, "DEFAULT_PARSERS")
 
     @property
     def DEFAULT_RENDERERS(self):
         default = [
-            'flask_api.renderers.JSONRenderer',
-            'flask_api.renderers.BrowsableAPIRenderer'
+            "flask_api.renderers.JSONRenderer",
+            "flask_api.renderers.BrowsableAPIRenderer",
         ]
-        val = self.user_config.get('DEFAULT_RENDERERS', default)
-        return perform_imports(val, 'DEFAULT_RENDERERS')
+        val = self.user_config.get("DEFAULT_RENDERERS", default)
+        return perform_imports(val, "DEFAULT_RENDERERS")
 
 
 default_settings = APISettings()
```

### Comparing `Flask-API-3.0b6/flask_api/static/css/bootstrap-tweaks.css` & `Flask-API-3.1/flask_api/static/css/bootstrap-tweaks.css`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/css/bootstrap.min.css` & `Flask-API-3.1/flask_api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/css/default.css` & `Flask-API-3.1/flask_api/static/css/default.css`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/css/prettify.css` & `Flask-API-3.1/flask_api/static/css/prettify.css`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/img/glyphicons-halflings-white.png` & `Flask-API-3.1/flask_api/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/img/glyphicons-halflings.png` & `Flask-API-3.1/flask_api/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/img/grid.png` & `Flask-API-3.1/flask_api/static/img/grid.png`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/js/bootstrap.min.js` & `Flask-API-3.1/flask_api/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/js/default.js` & `Flask-API-3.1/flask_api/static/js/default.js`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/js/jquery-1.8.1-min.js` & `Flask-API-3.1/flask_api/static/js/jquery-1.8.1-min.js`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/static/js/prettify-min.js` & `Flask-API-3.1/flask_api/static/js/prettify-min.js`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/status.py` & `Flask-API-3.1/flask_api/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# coding: utf8
 """
 Descriptive HTTP status codes, for code readability.
 
 See RFC 2616 and RFC 6585.
 
 RFC 2616: http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html
 RFC 6585: http://tools.ietf.org/html/rfc6585
 """
-from __future__ import unicode_literals
 
 
 def is_informational(code):
     return code >= 100 and code <= 199
 
 
 def is_success(code):
```

### Comparing `Flask-API-3.0b6/flask_api/templates/base.html` & `Flask-API-3.1/flask_api/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-API-3.0b6/flask_api/tests/test_app.py` & `Flask-API-3.1/flask_api/tests/test_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import abort, make_response, request, jsonify
-from flask_api.decorators import set_renderers
-from flask_api import exceptions, renderers, status, FlaskAPI
 import json
 import unittest
 
+from flask import abort, jsonify, make_response, request
+
+from flask_api import FlaskAPI, exceptions, renderers, status
+from flask_api.decorators import set_renderers
 
 app = FlaskAPI(__name__)
-app.config['TESTING'] = True
+app.config["TESTING"] = True
 
 
 class JSONVersion1(renderers.JSONRenderer):
     media_type = 'application/json; api-version="1.0"'
 
 
 class JSONVersion2(renderers.JSONRenderer):
@@ -28,164 +27,166 @@
         self.message = message
         if status_code is not None:
             self.status_code = status_code
         self.payload = payload
 
     def to_dict(self):
         rv = dict(self.payload or ())
-        rv['message'] = self.message
+        rv["message"] = self.message
         return rv
 
 
 @app.errorhandler(InvalidUsage)
 def handle_invalid_usage(error):
     response = jsonify(error.to_dict())
     response.status_code = error.status_code
     return response
 
 
-@app.route('/set_status_and_headers/')
+@app.route("/set_status_and_headers/")
 def set_status_and_headers():
-    headers = {'Location': 'http://example.com/456'}
-    return {'example': 'content'}, status.HTTP_201_CREATED, headers
+    headers = {"Location": "http://example.com/456"}
+    return {"example": "content"}, status.HTTP_201_CREATED, headers
 
 
-@app.route('/set_headers/')
+@app.route("/set_headers/")
 def set_headers():
-    headers = {'Location': 'http://example.com/456'}
-    return {'example': 'content'}, headers
+    headers = {"Location": "http://example.com/456"}
+    return {"example": "content"}, headers
 
 
-@app.route('/make_response_view/')
+@app.route("/make_response_view/")
 def make_response_view():
-    response = make_response({'example': 'content'})
-    response.headers['Location'] = 'http://example.com/456'
+    response = make_response({"example": "content"})
+    response.headers["Location"] = "http://example.com/456"
     return response
 
 
-@app.route('/none_204_response/')
+@app.route("/none_204_response/")
 def none_204_response():
     return None, status.HTTP_204_NO_CONTENT
 
 
-@app.route('/none_200_response/')
+@app.route("/none_200_response/")
 def none_200_response():
     return None, status.HTTP_200_OK
 
 
-@app.route('/api_exception/')
+@app.route("/api_exception/")
 def api_exception():
     raise exceptions.PermissionDenied()
 
 
-@app.route('/custom_exception/')
+@app.route("/custom_exception/")
 def custom_exception():
-    raise InvalidUsage('Invalid usage test.', status_code=410)
+    raise InvalidUsage("Invalid usage test.", status_code=410)
 
 
-@app.route('/custom_exception_no_code/')
+@app.route("/custom_exception_no_code/")
 def custom_exception_no_status_code():
-    raise InvalidUsage('Invalid usage test.')
+    raise InvalidUsage("Invalid usage test.")
 
 
-@app.route('/abort_view/')
+@app.route("/abort_view/")
 def abort_view():
     abort(status.HTTP_403_FORBIDDEN)
 
 
-@app.route('/options/')
+@app.route("/options/")
 def options_view():
     return {}
 
 
-@app.route('/accepted_media_type/')
+@app.route("/accepted_media_type/")
 @set_renderers([JSONVersion2, JSONVersion1])
 def accepted_media_type():
-    return {'accepted_media_type': str(request.accepted_media_type)}
+    return {"accepted_media_type": str(request.accepted_media_type)}
 
 
 class AppTests(unittest.TestCase):
     def test_set_status_and_headers(self):
         with app.test_client() as client:
-            response = client.get('/set_status_and_headers/')
+            response = client.get("/set_status_and_headers/")
             self.assertEqual(response.status_code, status.HTTP_201_CREATED)
-            self.assertEqual(response.headers['Location'], 'http://example.com/456')
-            self.assertEqual(response.content_type, 'application/json')
+            self.assertEqual(response.headers["Location"], "http://example.com/456")
+            self.assertEqual(response.content_type, "application/json")
             expected = '{"example": "content"}'
-            self.assertEqual(response.get_data().decode('utf8'), expected)
+            self.assertEqual(response.get_data().decode("utf8"), expected)
 
     def test_set_headers(self):
         with app.test_client() as client:
-            response = client.get('/set_headers/')
+            response = client.get("/set_headers/")
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Location'], 'http://example.com/456')
-            self.assertEqual(response.content_type, 'application/json')
+            self.assertEqual(response.headers["Location"], "http://example.com/456")
+            self.assertEqual(response.content_type, "application/json")
             expected = '{"example": "content"}'
-            self.assertEqual(response.get_data().decode('utf8'), expected)
+            self.assertEqual(response.get_data().decode("utf8"), expected)
 
     def test_make_response(self):
         with app.test_client() as client:
-            response = client.get('/make_response_view/')
-            self.assertEqual(response.content_type, 'application/json')
-            self.assertEqual(response.headers['Location'], 'http://example.com/456')
-            self.assertEqual(response.content_type, 'application/json')
+            response = client.get("/make_response_view/")
+            self.assertEqual(response.content_type, "application/json")
+            self.assertEqual(response.headers["Location"], "http://example.com/456")
+            self.assertEqual(response.content_type, "application/json")
             expected = '{"example": "content"}'
-            self.assertEqual(response.get_data().decode('utf8'), expected)
+            self.assertEqual(response.get_data().decode("utf8"), expected)
 
     def test_none_204_response(self):
         with app.test_client() as client:
-            response = client.get('/none_204_response/')
+            response = client.get("/none_204_response/")
             self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
-            expected = ''
-            self.assertEqual(response.get_data().decode('utf8'), expected)
+            expected = ""
+            self.assertEqual(response.get_data().decode("utf8"), expected)
 
     def test_none_200_response(self):
         with app.test_client() as client:
             with self.assertRaises(ValueError):
-                client.get('/none_200_response/')
+                client.get("/none_200_response/")
 
     def test_api_exception(self):
         with app.test_client() as client:
-            response = client.get('/api_exception/')
+            response = client.get("/api_exception/")
             self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
-            self.assertEqual(response.content_type, 'application/json')
-            expected = '{"message": "You do not have permission to perform this action."}'
-            self.assertEqual(response.get_data().decode('utf8'), expected)
+            self.assertEqual(response.content_type, "application/json")
+            expected = (
+                '{"message": "You do not have permission to perform this action."}'
+            )
+            self.assertEqual(response.get_data().decode("utf8"), expected)
 
     def test_custom_exception(self):
         with app.test_client() as client:
-            response = client.get('/custom_exception/')
+            response = client.get("/custom_exception/")
             self.assertEqual(response.status_code, status.HTTP_410_GONE)
-            self.assertEqual(response.content_type, 'application/json')
+            self.assertEqual(response.content_type, "application/json")
 
     def test_custom_exception_default_code(self):
         with app.test_client() as client:
-            response = client.get('/custom_exception_no_code/')
+            response = client.get("/custom_exception_no_code/")
             self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
-            self.assertEqual(response.content_type, 'application/json')
+            self.assertEqual(response.content_type, "application/json")
 
     def test_abort_view(self):
         with app.test_client() as client:
-            response = client.get('/abort_view/')
+            response = client.get("/abort_view/")
             self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
     def test_options_view(self):
         with app.test_client() as client:
-            response = client.options('/options/')
+            response = client.options("/options/")
         # Errors if `response.response` is `None`
         response.get_data()
 
     def test_accepted_media_type_property(self):
         with app.test_client() as client:
             # Explicitly request the "api-version 1.0" renderer.
-            headers = {'Accept': 'application/json; api-version="1.0"'}
-            response = client.get('/accepted_media_type/', headers=headers)
-            data = json.loads(response.get_data().decode('utf8'))
-            expected = {'accepted_media_type': 'application/json; api-version="1.0"'}
+            headers = {"Accept": 'application/json; api-version="1.0"'}
+            response = client.get("/accepted_media_type/", headers=headers)
+            data = json.loads(response.get_data().decode("utf8"))
+            expected = {"accepted_media_type": 'application/json; api-version="1.0"'}
             self.assertEqual(data, expected)
 
             # Request the default renderer, which is "api-version 2.0".
-            headers = {'Accept': '*/*'}
-            response = client.get('/accepted_media_type/', headers=headers)
-            data = json.loads(response.get_data().decode('utf8'))
-            expected = {'accepted_media_type': 'application/json; api-version="2.0"'}
+            headers = {"Accept": "*/*"}
+            response = client.get("/accepted_media_type/", headers=headers)
+            data = json.loads(response.get_data().decode("utf8"))
+            expected = {"accepted_media_type": 'application/json; api-version="2.0"'}
             self.assertEqual(data, expected)
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_exceptions.py` & `Flask-API-3.1/flask_api/tests/test_exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask_api import exceptions
-from flask_api import status
 import unittest
 
+from flask_api import exceptions, status
+
 
 class Conflict(exceptions.APIException):
     status_code = status.HTTP_409_CONFLICT
-    detail = 'Could not update the resource'
+    detail = "Could not update the resource"
 
 
 class TestExceptions(unittest.TestCase):
     def test_custom_exception(self):
         try:
             raise Conflict()
         except Conflict as exc:
-            self.assertEqual(str(exc), 'Could not update the resource')
+            self.assertEqual(str(exc), "Could not update the resource")
             self.assertEqual(exc.status_code, 409)
 
     def test_override_exception_detail(self):
         try:
-            raise Conflict('A widget with this id already exists')
+            raise Conflict("A widget with this id already exists")
         except Conflict as exc:
-            self.assertEqual(str(exc), 'A widget with this id already exists')
+            self.assertEqual(str(exc), "A widget with this id already exists")
             self.assertEqual(exc.status_code, 409)
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_mediatypes.py` & `Flask-API-3.1/flask_api/tests/test_mediatypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,126 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask_api.mediatypes import MediaType, parse_accept_header
 import unittest
 
+from flask_api.mediatypes import MediaType, parse_accept_header
+
 
 class MediaTypeParsingTests(unittest.TestCase):
     def test_media_type_with_params(self):
-        media = MediaType('application/xml; schema=foobar, q=0.5')
+        media = MediaType("application/xml; schema=foobar, q=0.5")
         self.assertEqual(str(media), 'application/xml; q="0.5", schema="foobar"')
-        self.assertEqual(media.main_type, 'application')
-        self.assertEqual(media.sub_type, 'xml')
-        self.assertEqual(media.full_type, 'application/xml')
-        self.assertEqual(media.params, {'schema': 'foobar', 'q': '0.5'})
+        self.assertEqual(media.main_type, "application")
+        self.assertEqual(media.sub_type, "xml")
+        self.assertEqual(media.full_type, "application/xml")
+        self.assertEqual(media.params, {"schema": "foobar", "q": "0.5"})
         self.assertEqual(media.precedence, 3)
-        self.assertEqual(repr(media), '<MediaType \'application/xml; q="0.5", schema="foobar"\'>')
+        self.assertEqual(
+            repr(media), '<MediaType \'application/xml; q="0.5", schema="foobar"\'>'
+        )
 
     def test_media_type_with_q_params(self):
-        media = MediaType('application/xml; q=0.5')
+        media = MediaType("application/xml; q=0.5")
         self.assertEqual(str(media), 'application/xml; q="0.5"')
-        self.assertEqual(media.main_type, 'application')
-        self.assertEqual(media.sub_type, 'xml')
-        self.assertEqual(media.full_type, 'application/xml')
-        self.assertEqual(media.params, {'q': '0.5'})
+        self.assertEqual(media.main_type, "application")
+        self.assertEqual(media.sub_type, "xml")
+        self.assertEqual(media.full_type, "application/xml")
+        self.assertEqual(media.params, {"q": "0.5"})
         self.assertEqual(media.precedence, 2)
 
     def test_media_type_without_params(self):
-        media = MediaType('application/xml')
-        self.assertEqual(str(media), 'application/xml')
-        self.assertEqual(media.main_type, 'application')
-        self.assertEqual(media.sub_type, 'xml')
-        self.assertEqual(media.full_type, 'application/xml')
+        media = MediaType("application/xml")
+        self.assertEqual(str(media), "application/xml")
+        self.assertEqual(media.main_type, "application")
+        self.assertEqual(media.sub_type, "xml")
+        self.assertEqual(media.full_type, "application/xml")
         self.assertEqual(media.params, {})
         self.assertEqual(media.precedence, 2)
 
     def test_media_type_with_wildcard_sub_type(self):
-        media = MediaType('application/*')
-        self.assertEqual(str(media), 'application/*')
-        self.assertEqual(media.main_type, 'application')
-        self.assertEqual(media.sub_type, '*')
-        self.assertEqual(media.full_type, 'application/*')
+        media = MediaType("application/*")
+        self.assertEqual(str(media), "application/*")
+        self.assertEqual(media.main_type, "application")
+        self.assertEqual(media.sub_type, "*")
+        self.assertEqual(media.full_type, "application/*")
         self.assertEqual(media.params, {})
         self.assertEqual(media.precedence, 1)
 
     def test_media_type_with_wildcard_main_type(self):
-        media = MediaType('*/*')
-        self.assertEqual(str(media), '*/*')
-        self.assertEqual(media.main_type, '*')
-        self.assertEqual(media.sub_type, '*')
-        self.assertEqual(media.full_type, '*/*')
+        media = MediaType("*/*")
+        self.assertEqual(str(media), "*/*")
+        self.assertEqual(media.main_type, "*")
+        self.assertEqual(media.sub_type, "*")
+        self.assertEqual(media.full_type, "*/*")
         self.assertEqual(media.params, {})
         self.assertEqual(media.precedence, 0)
 
 
 class MediaTypeMatchingTests(unittest.TestCase):
     def test_media_type_includes_params(self):
-        media_type = MediaType('application/json')
-        other = MediaType('application/json; version=1.0')
+        media_type = MediaType("application/json")
+        other = MediaType("application/json; version=1.0")
         self.assertTrue(media_type.satisfies(other))
 
     def test_media_type_missing_params(self):
-        media_type = MediaType('application/json; version=1.0')
-        other = MediaType('application/json')
+        media_type = MediaType("application/json; version=1.0")
+        other = MediaType("application/json")
         self.assertFalse(media_type.satisfies(other))
 
     def test_media_type_matching_params(self):
-        media_type = MediaType('application/json; version=1.0')
-        other = MediaType('application/json; version=1.0')
+        media_type = MediaType("application/json; version=1.0")
+        other = MediaType("application/json; version=1.0")
         self.assertTrue(media_type.satisfies(other))
 
     def test_media_type_non_matching_params(self):
-        media_type = MediaType('application/json; version=1.0')
-        other = MediaType('application/json; version=2.0')
+        media_type = MediaType("application/json; version=1.0")
+        other = MediaType("application/json; version=2.0")
         self.assertFalse(media_type.satisfies(other))
 
     def test_media_type_main_type_match(self):
-        media_type = MediaType('image/*')
-        other = MediaType('image/png')
+        media_type = MediaType("image/*")
+        other = MediaType("image/png")
         self.assertTrue(media_type.satisfies(other))
 
     def test_media_type_sub_type_mismatch(self):
-        media_type = MediaType('image/jpeg')
-        other = MediaType('image/png')
+        media_type = MediaType("image/jpeg")
+        other = MediaType("image/png")
         self.assertFalse(media_type.satisfies(other))
 
     def test_media_type_wildcard_match(self):
-        media_type = MediaType('*/*')
-        other = MediaType('image/png')
+        media_type = MediaType("*/*")
+        other = MediaType("image/png")
         self.assertTrue(media_type.satisfies(other))
 
     def test_media_type_wildcard_mismatch(self):
-        media_type = MediaType('image/*')
-        other = MediaType('audio/*')
+        media_type = MediaType("image/*")
+        other = MediaType("audio/*")
         self.assertFalse(media_type.satisfies(other))
 
 
 class AcceptHeaderTests(unittest.TestCase):
     def test_parse_simple_accept_header(self):
-        parsed = parse_accept_header('*/*, application/json')
-        self.assertEqual(parsed, [
-            set([MediaType('application/json')]),
-            set([MediaType('*/*')])
-        ])
+        parsed = parse_accept_header("*/*, application/json")
+        self.assertEqual(
+            parsed, [set([MediaType("application/json")]), set([MediaType("*/*")])]
+        )
 
     def test_parse_complex_accept_header(self):
         """
         The accept header should be parsed into a list of sets of MediaType.
         The list is an ordering of precedence.
 
         Note that we disregard 'q' values when determining precedence, and
         instead differentiate equal values by using the server preference.
         """
-        header = 'application/xml; schema=foo, application/json; q=0.9, application/xml, */*'
+        header = (
+            "application/xml; schema=foo, application/json; q=0.9, application/xml, */*"
+        )
         parsed = parse_accept_header(header)
-        self.assertEqual(parsed, [
-            set([MediaType('application/xml; schema=foo')]),
-            set([MediaType('application/json; q=0.9'), MediaType('application/xml')]),
-            set([MediaType('*/*')]),
-        ])
+        self.assertEqual(
+            parsed,
+            [
+                set([MediaType("application/xml; schema=foo")]),
+                set(
+                    [MediaType("application/json; q=0.9"), MediaType("application/xml")]
+                ),
+                set([MediaType("*/*")]),
+            ],
+        )
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_negotiation.py` & `Flask-API-3.1/flask_api/tests/test_negotiation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,94 @@
-# coding: utf8
-from __future__ import unicode_literals
 import unittest
+
 import flask_api
 from flask_api import exceptions
 from flask_api.negotiation import BaseNegotiation, DefaultNegotiation
 
-
 app = flask_api.FlaskAPI(__name__)
 
 
-class JSON(object):
-    media_type = 'application/json'
+class JSON:
+    media_type = "application/json"
 
 
-class HTML(object):
-    media_type = 'application/html'
+class HTML:
+    media_type = "application/html"
 
 
-class URLEncodedForm(object):
-    media_type = 'application/x-www-form-urlencoded'
+class URLEncodedForm:
+    media_type = "application/x-www-form-urlencoded"
 
 
 class TestRendererNegotiation(unittest.TestCase):
     def test_select_renderer_client_preference(self):
         negotiation = DefaultNegotiation()
         renderers = [JSON, HTML]
-        headers = {'Accept': 'application/html'}
+        headers = {"Accept": "application/html"}
         with app.test_request_context(headers=headers):
             renderer, media_type = negotiation.select_renderer(renderers)
             self.assertEqual(renderer, HTML)
-            self.assertEqual(str(media_type), 'application/html')
+            self.assertEqual(str(media_type), "application/html")
 
     def test_select_renderer_no_accept_header(self):
         negotiation = DefaultNegotiation()
         renderers = [JSON, HTML]
         with app.test_request_context():
             renderer, media_type = negotiation.select_renderer(renderers)
             self.assertEqual(renderer, JSON)
-            self.assertEqual(str(media_type), 'application/json')
+            self.assertEqual(str(media_type), "application/json")
 
     def test_select_renderer_server_preference(self):
         negotiation = DefaultNegotiation()
         renderers = [JSON, HTML]
-        headers = {'Accept': '*/*'}
+        headers = {"Accept": "*/*"}
         with app.test_request_context(headers=headers):
             renderer, media_type = negotiation.select_renderer(renderers)
             self.assertEqual(renderer, JSON)
-            self.assertEqual(str(media_type), 'application/json')
+            self.assertEqual(str(media_type), "application/json")
 
     def test_select_renderer_failed(self):
         negotiation = DefaultNegotiation()
         renderers = [JSON, HTML]
-        headers = {'Accept': 'application/xml'}
+        headers = {"Accept": "application/xml"}
         with app.test_request_context(headers=headers):
             with self.assertRaises(exceptions.NotAcceptable):
                 renderer, media_type = negotiation.select_renderer(renderers)
 
     def test_renderer_negotiation_not_implemented(self):
         negotiation = BaseNegotiation()
         with self.assertRaises(NotImplementedError) as context:
             negotiation.select_renderer([])
         msg = str(context.exception)
-        expected = '`select_renderer()` method must be implemented for class "BaseNegotiation"'
+        expected = (
+            '`select_renderer()` method must be implemented for class "BaseNegotiation"'
+        )
         self.assertEqual(msg, expected)
 
 
 class TestParserNegotiation(unittest.TestCase):
     def test_select_parser(self):
         negotiation = DefaultNegotiation()
         parsers = [JSON, URLEncodedForm]
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
         with app.test_request_context(headers=headers):
             renderer, media_type = negotiation.select_parser(parsers)
             self.assertEqual(renderer, URLEncodedForm)
-            self.assertEqual(str(media_type), 'application/x-www-form-urlencoded')
+            self.assertEqual(str(media_type), "application/x-www-form-urlencoded")
 
     def test_select_parser_failed(self):
         negotiation = DefaultNegotiation()
         parsers = [JSON, URLEncodedForm]
-        headers = {'Content-Type': 'application/xml'}
+        headers = {"Content-Type": "application/xml"}
         with app.test_request_context(headers=headers):
             with self.assertRaises(exceptions.UnsupportedMediaType):
                 renderer, media_type = negotiation.select_parser(parsers)
 
     def test_parser_negotiation_not_implemented(self):
         negotiation = BaseNegotiation()
         with self.assertRaises(NotImplementedError) as context:
             negotiation.select_parser([])
         msg = str(context.exception)
-        expected = '`select_parser()` method must be implemented for class "BaseNegotiation"'
+        expected = (
+            '`select_parser()` method must be implemented for class "BaseNegotiation"'
+        )
         self.assertEqual(msg, expected)
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_parsers.py` & `Flask-API-3.1/flask_api/tests/test_parsers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import request
-from flask_api import exceptions, parsers, status, mediatypes, FlaskAPI
-from flask_api.decorators import set_parsers
 import io
 import json
 import unittest
 
+from flask import request
+
+from flask_api import FlaskAPI, exceptions, mediatypes, parsers, status
+from flask_api.decorators import set_parsers
 
 app = FlaskAPI(__name__)
 
 
-@app.route('/', methods=['POST'])
+@app.route("/", methods=["POST"])
 def data():
     return {
-        'data': request.data,
-        'form': request.form,
-        'files': dict([
-            (key, {'name': val.filename, 'contents': val.read().decode('utf8')})
-            for key, val in request.files.items()
-        ])
+        "data": request.data,
+        "form": request.form,
+        "files": dict(
+            [
+                (key, {"name": val.filename, "contents": val.read().decode("utf8")})
+                for key, val in request.files.items()
+            ]
+        ),
     }
 
 
 class ParserTests(unittest.TestCase):
     def test_valid_json(self):
         parser = parsers.JSONParser()
         stream = io.BytesIO(b'{"key": 1, "other": "two"}')
-        data = parser.parse(stream, 'application/json')
+        data = parser.parse(stream, "application/json")
         self.assertEqual(data, {"key": 1, "other": "two"})
 
     def test_invalid_json(self):
         parser = parsers.JSONParser()
         stream = io.BytesIO(b'{key: 1, "other": "two"}')
         with self.assertRaises(exceptions.ParseError) as context:
-            parser.parse(stream, mediatypes.MediaType('application/json'))
+            parser.parse(stream, mediatypes.MediaType("application/json"))
         detail = str(context.exception)
-        expected_pypy = 'JSON parse error - Key name must be string at char: line 1 column 2 (char 1)'
-        expected_py3 = 'JSON parse error - Expecting property name enclosed in double quotes: line 1 column 2 (char 1)'
+        expected_pypy = "JSON parse error - Key name must be string at char: line 1 column 2 (char 1)"
+        expected_py3 = "JSON parse error - Expecting property name enclosed in double quotes: line 1 column 2 (char 1)"
         self.assertIn(detail, (expected_pypy, expected_py3))
 
     def test_invalid_multipart(self):
         parser = parsers.MultiPartParser()
-        stream = io.BytesIO(b'invalid')
+        stream = io.BytesIO(b"invalid")
         media_type = mediatypes.MediaType('multipart/form-data; boundary="foo"')
         with self.assertRaises(exceptions.ParseError) as context:
-            parser.parse(stream, media_type, content_length=len('invalid'))
-        self.assertIn('Multipart parse error', str(context.exception))
+            parser.parse(stream, media_type, content_length=len("invalid"))
+        self.assertIn("Multipart parse error", str(context.exception))
 
     def test_invalid_multipart_no_boundary(self):
         parser = parsers.MultiPartParser()
-        stream = io.BytesIO(b'invalid')
+        stream = io.BytesIO(b"invalid")
         with self.assertRaises(exceptions.ParseError) as context:
-            parser.parse(stream, mediatypes.MediaType('multipart/form-data'))
+            parser.parse(stream, mediatypes.MediaType("multipart/form-data"))
         detail = str(context.exception)
-        expected = 'Multipart message missing boundary in Content-Type header'
+        expected = "Multipart message missing boundary in Content-Type header"
         self.assertEqual(detail, expected)
 
     def test_renderer_negotiation_not_implemented(self):
         parser = parsers.BaseParser()
         with self.assertRaises(NotImplementedError) as context:
             parser.parse(None, None)
         msg = str(context.exception)
         expected = '`parse()` method must be implemented for class "BaseParser"'
         self.assertEqual(msg, expected)
 
     def test_accessing_json(self):
         with app.test_client() as client:
-            data = json.dumps({'example': 'example'})
-            response = client.post('/', data=data, content_type='application/json')
+            data = json.dumps({"example": "example"})
+            response = client.post("/", data=data, content_type="application/json")
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
-            expected = {
-                "data": {"example": "example"},
-                "form": {},
-                "files": {}
-            }
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
+            expected = {"data": {"example": "example"}, "form": {}, "files": {}}
             self.assertEqual(data, expected)
 
     def test_accessing_url_encoded(self):
         with app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.post('/', data=data)
+            data = {"example": "example"}
+            response = client.post("/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
             expected = {
                 "data": {"example": "example"},
                 "form": {"example": "example"},
-                "files": {}
+                "files": {},
             }
             self.assertEqual(data, expected)
 
     def test_accessing_multipart(self):
         with app.test_client() as client:
-            data = {'example': 'example', 'upload': (io.BytesIO(b'file contents'), 'name.txt')}
-            response = client.post('/', data=data)
+            data = {
+                "example": "example",
+                "upload": (io.BytesIO(b"file contents"), "name.txt"),
+            }
+            response = client.post("/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
             expected = {
                 "data": {"example": "example"},
                 "form": {"example": "example"},
-                "files": {"upload": {"name": "name.txt", "contents": "file contents"}}
+                "files": {"upload": {"name": "name.txt", "contents": "file contents"}},
             }
             self.assertEqual(data, expected)
 
 
 class OverrideParserSettings(unittest.TestCase):
     def setUp(self):
         class CustomParser1(parsers.BaseParser):
-            media_type = '*/*'
+            media_type = "*/*"
 
             def parse(self, stream, media_type, content_length=None):
-                return 'custom parser 1'
+                return "custom parser 1"
 
         class CustomParser2(parsers.BaseParser):
-            media_type = '*/*'
+            media_type = "*/*"
 
             def parse(self, stream, media_type, content_length=None):
-                return 'custom parser 2'
+                return "custom parser 2"
 
         app = FlaskAPI(__name__)
-        app.config['DEFAULT_PARSERS'] = [CustomParser1]
+        app.config["DEFAULT_PARSERS"] = [CustomParser1]
 
-        @app.route('/custom_parser_1/', methods=['POST'])
+        @app.route("/custom_parser_1/", methods=["POST"])
         def custom_parser_1():
-            return {'data': request.data}
+            return {"data": request.data}
 
-        @app.route('/custom_parser_2/', methods=['POST'])
+        @app.route("/custom_parser_2/", methods=["POST"])
         @set_parsers([CustomParser2])
         def custom_parser_2():
-            return {'data': request.data}
+            return {"data": request.data}
 
-        @app.route('/custom_parser_2_as_args/', methods=['POST'])
+        @app.route("/custom_parser_2_as_args/", methods=["POST"])
         @set_parsers(CustomParser2, CustomParser1)
         def custom_parser_2_as_args():
-            return {'data': request.data}
+            return {"data": request.data}
 
         self.app = app
 
     def test_overridden_parsers_with_settings(self):
         with self.app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.post('/custom_parser_1/', data=data)
+            data = {"example": "example"}
+            response = client.post("/custom_parser_1/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
             expected = {
                 "data": "custom parser 1",
             }
             self.assertEqual(data, expected)
 
     def test_overridden_parsers_with_decorator(self):
         with self.app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.post('/custom_parser_2/', data=data)
+            data = {"example": "example"}
+            response = client.post("/custom_parser_2/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
             expected = {
                 "data": "custom parser 2",
             }
             self.assertEqual(data, expected)
 
     def test_overridden_parsers_with_decorator_as_args(self):
         with self.app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.post('/custom_parser_2_as_args/', data=data)
+            data = {"example": "example"}
+            response = client.post("/custom_parser_2_as_args/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/json')
-            data = json.loads(response.get_data().decode('utf8'))
+            self.assertEqual(response.headers["Content-Type"], "application/json")
+            data = json.loads(response.get_data().decode("utf8"))
             expected = {
                 "data": "custom parser 2",
             }
             self.assertEqual(data, expected)
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_renderers.py` & `Flask-API-3.1/flask_api/tests/test_renderers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,172 @@
-# coding: utf8
-from __future__ import unicode_literals
+import unittest
 from datetime import datetime
-from flask.json import JSONEncoder
-from flask_api import renderers, status, FlaskAPI
+
+from flask.json.provider import DefaultJSONProvider
+
+from flask_api import FlaskAPI, renderers, status
 from flask_api.decorators import set_renderers
 from flask_api.mediatypes import MediaType
-import unittest
 
 
 class RendererTests(unittest.TestCase):
     def _make_app(self):
         app = FlaskAPI(__name__)
 
-        @app.route('/_love', methods=['GET'])
+        @app.route("/_love", methods=["GET"])
         def love():
             return {"test": "I <3 Python"}
 
         return app
 
     def test_render_json(self):
         app = self._make_app()
         renderer = renderers.JSONRenderer()
         with app.app_context():
-            content = renderer.render({'example': 'example'}, MediaType('application/json'))
+            content = renderer.render(
+                {"example": "example"}, MediaType("application/json")
+            )
         expected = '{"example": "example"}'
         self.assertEqual(content, expected)
 
     def test_render_json_with_indent(self):
         app = self._make_app()
         renderer = renderers.JSONRenderer()
         with app.app_context():
-            content = renderer.render({'example': 'example'}, MediaType('application/json; indent=4'))
+            content = renderer.render(
+                {"example": "example"}, MediaType("application/json; indent=4")
+            )
         expected = '{\n    "example": "example"\n}'
         self.assertEqual(content, expected)
 
     def test_render_json_with_custom_encoder(self):
-        class CustomJsonEncoder(JSONEncoder):
+        class CustomJsonProvider(DefaultJSONProvider):
             def default(self, o):
                 if isinstance(o, datetime):
                     return o.isoformat()
                 return super().default(o)
 
         app = self._make_app()
-        app.json_encoder = CustomJsonEncoder
+        app.json = CustomJsonProvider(app)
         renderer = renderers.JSONRenderer()
         date = datetime(2017, 10, 5, 15, 22)
         with app.app_context():
-            content = renderer.render(date, MediaType('application/json'))
+            content = renderer.render(date, MediaType("application/json"))
         self.assertEqual(content, '"{}"'.format(date.isoformat()))
 
     def test_render_browsable_encoding(self):
         app = FlaskAPI(__name__)
 
-        @app.route('/_love', methods=['GET'])
+        @app.route("/_love", methods=["GET"])
         def love():
             return {"test": "I <3 Python"}
 
         with app.test_client() as client:
-            response = client.get('/_love', headers={"Accept": "text/html"})
+            response = client.get("/_love", headers={"Accept": "text/html"})
             html = str(response.get_data())
-            self.assertTrue('I &lt;3 Python' in html)
-            self.assertTrue('<h1>Love</h1>' in html)
-            self.assertTrue('/_love' in html)
+            self.assertTrue("I &lt;3 Python" in html)
+            self.assertTrue("<h1>Love</h1>" in html)
+            self.assertTrue("/_love" in html)
 
     def test_render_browsable_encoding_with_markdown(self):
         app = FlaskAPI(__name__)
 
-        @app.route('/_foo', methods=['GET'])
+        @app.route("/_foo", methods=["GET"])
         def foo():
             """Bar:
-              - `qux`
+            - `qux`
             """
             return {"test": "I <3 Python"}
 
         with app.test_client() as client:
-            response = client.get('/_foo', headers={"Accept": "text/html"})
+            response = client.get("/_foo", headers={"Accept": "text/html"})
             html = str(response.get_data())
             print(html)
-            self.assertTrue('<h1>Foo</h1>' in html)
-            self.assertTrue('<p>Bar:' in html)
-            self.assertTrue('<code>qux</code>' in html)
+            self.assertTrue("<h1>Foo</h1>" in html)
+            self.assertTrue("<p>Bar:" in html)
+            self.assertTrue("<code>qux</code>" in html)
 
     def test_render_browsable_linking(self):
         app = FlaskAPI(__name__)
 
-        @app.route('/_happiness', methods=['GET'])
+        @app.route("/_happiness", methods=["GET"])
         def happiness():
-            return {"url": "http://example.org",
-                    "a tag": "<br />"}
+            return {"url": "http://example.org", "a tag": "<br />"}
 
         with app.test_client() as client:
-            response = client.get('/_happiness',
-                                  headers={"Accept": "text/html"})
+            response = client.get("/_happiness", headers={"Accept": "text/html"})
             html = str(response.get_data())
-            self.assertTrue('<a href="http://example.org">http://example.org</a>' in html)
-            self.assertTrue('&lt;br /&gt;'in html)
-            self.assertTrue('<h1>Happiness</h1>' in html)
-            self.assertTrue('/_happiness' in html)
+            self.assertTrue(
+                '<a href="http://example.org">http://example.org</a>' in html
+            )
+            self.assertTrue("&lt;br /&gt;" in html)
+            self.assertTrue("<h1>Happiness</h1>" in html)
+            self.assertTrue("/_happiness" in html)
 
     def test_renderer_negotiation_not_implemented(self):
         renderer = renderers.BaseRenderer()
         with self.assertRaises(NotImplementedError) as context:
             renderer.render(None, None)
         msg = str(context.exception)
         expected = '`render()` method must be implemented for class "BaseRenderer"'
         self.assertEqual(msg, expected)
 
 
 class OverrideParserSettings(unittest.TestCase):
     def setUp(self):
         class CustomRenderer1(renderers.BaseRenderer):
-            media_type = 'application/example1'
+            media_type = "application/example1"
 
             def render(self, data, media_type, **options):
-                return 'custom renderer 1'
+                return "custom renderer 1"
 
         class CustomRenderer2(renderers.BaseRenderer):
-            media_type = 'application/example2'
+            media_type = "application/example2"
 
             def render(self, data, media_type, **options):
-                return 'custom renderer 2'
+                return "custom renderer 2"
 
         app = FlaskAPI(__name__)
-        app.config['DEFAULT_RENDERERS'] = [CustomRenderer1]
-        app.config['PROPAGATE_EXCEPTIONS'] = True
+        app.config["DEFAULT_RENDERERS"] = [CustomRenderer1]
+        app.config["PROPAGATE_EXCEPTIONS"] = True
 
-        @app.route('/custom_renderer_1/', methods=['GET'])
+        @app.route("/custom_renderer_1/", methods=["GET"])
         def custom_renderer_1():
-            return {'data': 'example'}
+            return {"data": "example"}
 
-        @app.route('/custom_renderer_2/', methods=['GET'])
+        @app.route("/custom_renderer_2/", methods=["GET"])
         @set_renderers([CustomRenderer2])
         def custom_renderer_2():
-            return {'data': 'example'}
+            return {"data": "example"}
 
-        @app.route('/custom_renderer_2_as_args/', methods=['GET'])
+        @app.route("/custom_renderer_2_as_args/", methods=["GET"])
         @set_renderers(CustomRenderer2)
         def custom_renderer_2_as_args():
-            return {'data': 'example'}
+            return {"data": "example"}
 
         self.app = app
 
     def test_overridden_parsers_with_settings(self):
         with self.app.test_client() as client:
-            response = client.get('/custom_renderer_1/')
+            response = client.get("/custom_renderer_1/")
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/example1')
-            data = response.get_data().decode('utf8')
+            self.assertEqual(response.headers["Content-Type"], "application/example1")
+            data = response.get_data().decode("utf8")
             self.assertEqual(data, "custom renderer 1")
 
     def test_overridden_parsers_with_decorator(self):
         with self.app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.get('/custom_renderer_2/', data=data)
+            data = {"example": "example"}
+            response = client.get("/custom_renderer_2/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/example2')
-            data = response.get_data().decode('utf8')
+            self.assertEqual(response.headers["Content-Type"], "application/example2")
+            data = response.get_data().decode("utf8")
             self.assertEqual(data, "custom renderer 2")
 
     def test_overridden_parsers_with_decorator_as_args(self):
         with self.app.test_client() as client:
-            data = {'example': 'example'}
-            response = client.get('/custom_renderer_2_as_args/', data=data)
+            data = {"example": "example"}
+            response = client.get("/custom_renderer_2_as_args/", data=data)
             self.assertEqual(response.status_code, status.HTTP_200_OK)
-            self.assertEqual(response.headers['Content-Type'], 'application/example2')
-            data = response.get_data().decode('utf8')
+            self.assertEqual(response.headers["Content-Type"], "application/example2")
+            data = response.get_data().decode("utf8")
             self.assertEqual(data, "custom renderer 2")
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_request.py` & `Flask-API-3.1/flask_api/tests/test_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask import request
-from flask_api import exceptions
-import flask_api
 import io
 import unittest
 
+from flask import request
+
+import flask_api
+from flask_api import exceptions
+
 app = flask_api.FlaskAPI(__name__)
 
 
 class MediaTypeParsingTests(unittest.TestCase):
     def test_json_request(self):
         kwargs = {
-            'method': 'PUT',
-            'input_stream': io.BytesIO(b'{"key": 1, "other": "two"}'),
-            'content_type': 'application/json'
+            "method": "PUT",
+            "input_stream": io.BytesIO(b'{"key": 1, "other": "two"}'),
+            "content_type": "application/json",
         }
         with app.test_request_context(**kwargs):
             self.assertEqual(request.data, {"key": 1, "other": "two"})
 
     def test_invalid_content_type_request(self):
         kwargs = {
-            'method': 'PUT',
-            'input_stream': io.BytesIO(b'Cannot parse this content type.'),
-            'content_type': 'text/plain'
+            "method": "PUT",
+            "input_stream": io.BytesIO(b"Cannot parse this content type."),
+            "content_type": "text/plain",
         }
         with app.test_request_context(**kwargs):
             with self.assertRaises(exceptions.UnsupportedMediaType):
                 request.data
 
     def test_no_content_request(self):
         """
         Ensure that requests with no data do not populate the
         `.data`, `.form` or `.files` attributes.
         """
-        with app.test_request_context(method='PUT'):
+        with app.test_request_context(method="PUT"):
             self.assertFalse(request.data)
 
-        with app.test_request_context(method='PUT'):
+        with app.test_request_context(method="PUT"):
             self.assertFalse(request.form)
 
-        with app.test_request_context(method='PUT'):
+        with app.test_request_context(method="PUT"):
             self.assertFalse(request.files)
 
     def test_encode_request(self):
         """
         Ensure that `.full_path` is correctly decoded in python 3
         """
-        with app.test_request_context(method='GET', path='/?a=b'):
-            self.assertEqual(request.full_path, '/?a=b')
+        with app.test_request_context(method="GET", path="/?a=b"):
+            self.assertEqual(request.full_path, "/?a=b")
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_settings.py` & `Flask-API-3.1/flask_api/tests/test_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask_api.settings import APISettings
 import unittest
 
+from flask_api.settings import APISettings
+
 
 class SettingsTests(unittest.TestCase):
     def test_bad_import(self):
-        settings = APISettings({'DEFAULT_PARSERS': 'foobarz.FailedImport'})
+        settings = APISettings({"DEFAULT_PARSERS": "foobarz.FailedImport"})
         with self.assertRaises(ImportError) as context:
             settings.DEFAULT_PARSERS
         msg = str(context.exception)
         excepted_py2 = (
             "Could not import 'foobarz.FailedImport' for API setting "
             "'DEFAULT_PARSERS'. No module named foobarz."
         )
```

### Comparing `Flask-API-3.0b6/flask_api/tests/test_status.py` & `Flask-API-3.1/flask_api/tests/test_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# coding: utf8
-from __future__ import unicode_literals
-from flask_api import status
 import unittest
 
+from flask_api import status
+
 
 class TestStatus(unittest.TestCase):
     def test_status_categories(self):
         self.assertFalse(status.is_informational(99))
         self.assertTrue(status.is_informational(100))
         self.assertTrue(status.is_informational(199))
         self.assertFalse(status.is_informational(200))
```

### Comparing `Flask-API-3.0b6/setup.py` & `Flask-API-3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+#!/usr/bin/env python3
 
-from __future__ import print_function
-from setuptools import setup
-import re
 import os
+import re
 import sys
 
+from setuptools import setup
 
-name = 'Flask-API'
-package = 'flask_api'
-description = 'Browsable web APIs for Flask.'
-url = 'https://flask-api.github.io/flask-api/'
-author = 'Tom Christie'
-author_email = 'tom@tomchristie.com'
-license = 'BSD'
-install_requires = ['Flask >= 2.0']
+name = "Flask-API"
+package = "flask_api"
+description = "Browsable web APIs for Flask."
+url = "https://flask-api.github.io/flask-api/"
+author = "Tom Christie"
+author_email = "tom@tomchristie.com"
+license = "BSD"
+install_requires = ["Flask >= 2.0.0"]
 
 long_description = """Browsable web APIs for Flask."""
 
 
 def get_version(package):
     """
     Return package version as listed in `__version__` in `init.py`.
     """
-    init_py = open(os.path.join(package, '__init__.py')).read()
-    return re.search("^__version__ = ['\"]([^'\"]+)['\"]", init_py, re.MULTILINE).group(1)
+    init_py = open(os.path.join(package, "__init__.py")).read()
+    return re.search("^__version__ = ['\"]([^'\"]+)['\"]", init_py, re.MULTILINE).group(
+        1
+    )
 
 
 def get_packages(package):
     """
     Return root package and all sub-packages.
     """
-    return [dirpath
-            for dirpath, dirnames, filenames in os.walk(package)
-            if os.path.exists(os.path.join(dirpath, '__init__.py'))]
+    return [
+        dirpath
+        for dirpath, dirnames, filenames in os.walk(package)
+        if os.path.exists(os.path.join(dirpath, "__init__.py"))
+    ]
 
 
 def get_package_data(package):
     """
     Return all files under the root package, that are not in a
     package themselves.
     """
-    walk = [(dirpath.replace(package + os.sep, '', 1), filenames)
-            for dirpath, dirnames, filenames in os.walk(package)
-            if not os.path.exists(os.path.join(dirpath, '__init__.py'))]
+    walk = [
+        (dirpath.replace(package + os.sep, "", 1), filenames)
+        for dirpath, dirnames, filenames in os.walk(package)
+        if not os.path.exists(os.path.join(dirpath, "__init__.py"))
+    ]
 
     filepaths = []
     for base, filenames in walk:
-        filepaths.extend([os.path.join(base, filename)
-                          for filename in filenames])
+        filepaths.extend([os.path.join(base, filename) for filename in filenames])
     return {package: filepaths}
 
+
 setup(
     name=name,
     version=get_version(package),
     url=url,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     packages=get_packages(package),
     package_data=get_package_data(package),
     install_requires=install_requires,
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Web Environment',
-        'Framework :: Flask',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Internet :: WWW/HTTP',
-    ]
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Flask",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Internet :: WWW/HTTP",
+    ],
 )
```

