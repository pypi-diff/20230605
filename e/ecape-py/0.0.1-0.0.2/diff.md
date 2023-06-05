# Comparing `tmp/ecape_py-0.0.1.tar.gz` & `tmp/ecape_py-0.0.2.tar.gz`

## Comparing `ecape_py-0.0.1.tar` & `ecape_py-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/14fdf6e3251c6ab
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/2d141dda1a739d15
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/31634853e8e0a225
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/3683ab3a17443b35
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/4db88cbd806badf
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/5c62f748d7fd567a
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/5e12cf61d3a116b9
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/6363b2cac1df1527
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/74e8f76bbb787d8
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/897f9277732a0ba2
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/94b2a1ecdf3977a9
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/95304718c7671c57
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/9fcb0f13d38946e5
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/aa6f8456b6a5ad1d
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/b05b33f966cc0171
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/b5d24510ee3adaad
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/b94394e8a03833b7
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/c7863ed84ddd0c76
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/cf5c01c84f813c6e
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/d7b13f6506fa03c5
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/ea4340c60e00c60b
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/eac032f871d52a99
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/f3ba9fbe5f6ccc67
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.ruff_cache/content/fd55c4f84d7ea348
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape_py-0.0.1/src/ecape_py/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape_py-0.0.1/src/ecape_py/__init__.py
--rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 ecape_py-0.0.1/src/ecape_py/ecape.py
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/.coverage
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/intarg.txt
--rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/mseo.txt
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/ncape.txt
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/sounding.txt
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/test_ecape.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/__init___py.html
--rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/d_0e2659fc066377d6___init___py.html
--rw-r--r--   0        0        0    99333 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/d_0e2659fc066377d6_ecape_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/status.json
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/style.css
--rw-r--r--   0        0        0    58645 2020-02-02 00:00:00.000000 ecape_py-0.0.1/tests/htmlcov/test_ecape_py.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ecape_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape_py-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ecape_py-0.0.1/README.md
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ecape_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 ecape_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/14fdf6e3251c6ab
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/2d141dda1a739d15
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/31634853e8e0a225
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/3683ab3a17443b35
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/4db88cbd806badf
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/5c62f748d7fd567a
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/5e12cf61d3a116b9
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/6363b2cac1df1527
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/74e8f76bbb787d8
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/897f9277732a0ba2
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/94b2a1ecdf3977a9
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/95304718c7671c57
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/9fcb0f13d38946e5
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/aa6f8456b6a5ad1d
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/b05b33f966cc0171
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/b5d24510ee3adaad
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/b94394e8a03833b7
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/c7863ed84ddd0c76
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/cf5c01c84f813c6e
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/d7b13f6506fa03c5
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/ea4340c60e00c60b
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/eac032f871d52a99
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/f3ba9fbe5f6ccc67
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.ruff_cache/content/fd55c4f84d7ea348
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape_py-0.0.2/src/ecape_py/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape_py-0.0.2/src/ecape_py/__init__.py
+-rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 ecape_py-0.0.2/src/ecape_py/ecape.py
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/.coverage
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/intarg.txt
+-rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/mseo.txt
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/ncape.txt
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/sounding.txt
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/test_ecape.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/__init___py.html
+-rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/d_0e2659fc066377d6___init___py.html
+-rw-r--r--   0        0        0    99333 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/d_0e2659fc066377d6_ecape_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/status.json
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/style.css
+-rw-r--r--   0        0        0    58645 2020-02-02 00:00:00.000000 ecape_py-0.0.2/tests/htmlcov/test_ecape_py.html
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape_py-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ecape_py-0.0.2/README.md
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ecape_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ecape_py-0.0.2/PKG-INFO
```

### Comparing `ecape_py-0.0.1/.ruff_cache/content/2d141dda1a739d15` & `ecape_py-0.0.2/.ruff_cache/content/2d141dda1a739d15`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/31634853e8e0a225` & `ecape_py-0.0.2/.ruff_cache/content/31634853e8e0a225`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/5e12cf61d3a116b9` & `ecape_py-0.0.2/.ruff_cache/content/5e12cf61d3a116b9`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/6363b2cac1df1527` & `ecape_py-0.0.2/.ruff_cache/content/6363b2cac1df1527`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/897f9277732a0ba2` & `ecape_py-0.0.2/.ruff_cache/content/897f9277732a0ba2`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/94b2a1ecdf3977a9` & `ecape_py-0.0.2/.ruff_cache/content/94b2a1ecdf3977a9`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/95304718c7671c57` & `ecape_py-0.0.2/.ruff_cache/content/95304718c7671c57`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/9fcb0f13d38946e5` & `ecape_py-0.0.2/.ruff_cache/content/9fcb0f13d38946e5`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/aa6f8456b6a5ad1d` & `ecape_py-0.0.2/.ruff_cache/content/aa6f8456b6a5ad1d`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/b05b33f966cc0171` & `ecape_py-0.0.2/.ruff_cache/content/b05b33f966cc0171`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/b94394e8a03833b7` & `ecape_py-0.0.2/.ruff_cache/content/b94394e8a03833b7`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/c7863ed84ddd0c76` & `ecape_py-0.0.2/.ruff_cache/content/c7863ed84ddd0c76`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/cf5c01c84f813c6e` & `ecape_py-0.0.2/.ruff_cache/content/cf5c01c84f813c6e`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/d7b13f6506fa03c5` & `ecape_py-0.0.2/.ruff_cache/content/d7b13f6506fa03c5`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/ea4340c60e00c60b` & `ecape_py-0.0.2/.ruff_cache/content/ea4340c60e00c60b`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/eac032f871d52a99` & `ecape_py-0.0.2/.ruff_cache/content/eac032f871d52a99`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/f3ba9fbe5f6ccc67` & `ecape_py-0.0.2/.ruff_cache/content/f3ba9fbe5f6ccc67`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/.ruff_cache/content/fd55c4f84d7ea348` & `ecape_py-0.0.2/.ruff_cache/content/fd55c4f84d7ea348`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/src/ecape_py/ecape.py` & `ecape_py-0.0.2/src/ecape_py/ecape.py`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/.coverage` & `ecape_py-0.0.2/tests/.coverage`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/intarg.txt` & `ecape_py-0.0.2/tests/intarg.txt`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/mseo.txt` & `ecape_py-0.0.2/tests/mseo.txt`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/ncape.txt` & `ecape_py-0.0.2/tests/ncape.txt`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/sounding.txt` & `ecape_py-0.0.2/tests/sounding.txt`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/test_ecape.py` & `ecape_py-0.0.2/tests/test_ecape.py`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/__init___py.html` & `ecape_py-0.0.2/tests/htmlcov/__init___py.html`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/coverage_html.js` & `ecape_py-0.0.2/tests/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/d_0e2659fc066377d6___init___py.html` & `ecape_py-0.0.2/tests/htmlcov/d_0e2659fc066377d6___init___py.html`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/d_0e2659fc066377d6_ecape_py.html` & `ecape_py-0.0.2/tests/htmlcov/d_0e2659fc066377d6_ecape_py.html`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/favicon_32.png` & `ecape_py-0.0.2/tests/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/index.html` & `ecape_py-0.0.2/tests/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/keybd_closed.png` & `ecape_py-0.0.2/tests/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/keybd_open.png` & `ecape_py-0.0.2/tests/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/status.json` & `ecape_py-0.0.2/tests/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/style.css` & `ecape_py-0.0.2/tests/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/tests/htmlcov/test_ecape_py.html` & `ecape_py-0.0.2/tests/htmlcov/test_ecape_py.html`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/LICENSE.txt` & `ecape_py-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape_py-0.0.1/pyproject.toml` & `ecape_py-0.0.2/pyproject.toml`

 * *Files identical despite different names*

