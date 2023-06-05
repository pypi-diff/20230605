# Comparing `tmp/mdit-py-plugins-0.3.5.tar.gz` & `tmp/mdit_py_plugins-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdit-py-plugins-0.3.5.tar", last modified: Thu Mar  2 17:42:48 2023, max compression
+gzip compressed data, was "mdit_py_plugins-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdit-py-plugins-0.3.5.tar` & `mdit_py_plugins-0.4.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     1940 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1930 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/.gitignore
--rw-r--r--   0        0        0      797 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      151 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/.readthedocs.yml
--rw-r--r--   0        0        0     3419 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/LICENSE
--rw-r--r--   0        0        0     1202 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/README.md
--rw-r--r--   0        0        0      162 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/codecov.yml
--rw-r--r--   0        0        0       22 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/__init__.py
--rw-r--r--   0        0        0     1129 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/admon/LICENSE
--rw-r--r--   0        0        0       46 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/admon/__init__.py
--rw-r--r--   0        0        0     4892 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/admon/index.py
--rw-r--r--   0        0        0      117 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/admon/port.yaml
--rw-r--r--   0        0        0     4214 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/amsmath/__init__.py
--rw-r--r--   0        0        0       47 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/anchors/__init__.py
--rw-r--r--   0        0        0     4048 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/anchors/index.py
--rw-r--r--   0        0        0       66 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/attrs/__init__.py
--rw-r--r--   0        0        0     7669 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/attrs/index.py
--rw-r--r--   0        0        0     7710 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/attrs/parse.py
--rw-r--r--   0        0        0     3345 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/colon_fence.py
--rw-r--r--   0        0        0     1073 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/container/LICENSE
--rw-r--r--   0        0        0     2533 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/container/README.md
--rw-r--r--   0        0        0       49 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/container/__init__.py
--rw-r--r--   0        0        0     5358 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/container/index.py
--rw-r--r--   0        0        0      132 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/container/port.yaml
--rw-r--r--   0        0        0     1078 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/LICENSE
--rw-r--r--   0        0        0     1273 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/README.md
--rw-r--r--   0        0        0       47 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/__init__.py
--rw-r--r--   0        0        0     7409 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/index.py
--rw-r--r--   0        0        0      132 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/port.yaml
--rw-r--r--   0        0        0       50 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/dollarmath/__init__.py
--rw-r--r--   0        0        0    11438 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/dollarmath/index.py
--rw-r--r--   0        0        0     8677 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/field_list/__init__.py
--rw-r--r--   0        0        0     1078 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/LICENSE
--rw-r--r--   0        0        0       49 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/__init__.py
--rw-r--r--   0        0        0    12594 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/index.py
--rw-r--r--   0        0        0      120 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/port.yaml
--rw-r--r--   0        0        0     1056 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/LICENSE
--rw-r--r--   0        0        0       53 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/__init__.py
--rw-r--r--   0        0        0     4130 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/index.py
--rw-r--r--   0        0        0      124 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/port.yaml
--rw-r--r--   0        0        0       51 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/myst_blocks/__init__.py
--rw-r--r--   0        0        0     4341 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/myst_blocks/index.py
--rw-r--r--   0        0        0       50 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/myst_role/__init__.py
--rw-r--r--   0        0        0     1727 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/myst_role/index.py
--rw-r--r--   0        0        0       26 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/py.typed
--rw-r--r--   0        0        0     3222 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/substitution.py
--rw-r--r--   0        0        0     5784 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/tasklists/__init__.py
--rw-r--r--   0        0        0      195 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/tasklists/port.yaml
--rw-r--r--   0        0        0     1075 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/LICENSE
--rw-r--r--   0        0        0     5191 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/README.md
--rw-r--r--   0        0        0       47 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/__init__.py
--rw-r--r--   0        0        0     9666 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/index.py
--rw-r--r--   0        0        0      245 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/port.yaml
--rw-r--r--   0        0        0     1783 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/mdit_py_plugins/wordcount/__init__.py
--rw-r--r--   0        0        0     1963 2023-03-02 17:42:44.843881 mdit-py-plugins-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      532 2023-03-02 17:42:44.847880 mdit-py-plugins-0.3.5/tox.ini
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 mdit-py-plugins-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2064 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1930 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.gitignore
+-rw-r--r--   0        0        0      811 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      155 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4946 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1202 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/README.md
+-rw-r--r--   0        0        0      162 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/codecov.yml
+-rw-r--r--   0        0        0       22 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/__init__.py
+-rw-r--r--   0        0        0     1129 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/__init__.py
+-rw-r--r--   0        0        0     6196 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/index.py
+-rw-r--r--   0        0        0      117 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/port.yaml
+-rw-r--r--   0        0        0     4588 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/amsmath/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/__init__.py
+-rw-r--r--   0        0        0     4114 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/index.py
+-rw-r--r--   0        0        0       66 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/__init__.py
+-rw-r--r--   0        0        0     7625 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/index.py
+-rw-r--r--   0        0        0     7754 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/parse.py
+-rw-r--r--   0        0        0     3955 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/colon_fence.py
+-rw-r--r--   0        0        0     1073 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/LICENSE
+-rw-r--r--   0        0        0     2533 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/README.md
+-rw-r--r--   0        0        0       49 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/__init__.py
+-rw-r--r--   0        0        0     5741 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/index.py
+-rw-r--r--   0        0        0      132 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/port.yaml
+-rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/LICENSE
+-rw-r--r--   0        0        0     1273 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/README.md
+-rw-r--r--   0        0        0       47 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/__init__.py
+-rw-r--r--   0        0        0     7438 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/index.py
+-rw-r--r--   0        0        0      132 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/port.yaml
+-rw-r--r--   0        0        0       50 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/__init__.py
+-rw-r--r--   0        0        0    12497 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/index.py
+-rw-r--r--   0        0        0     8281 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/field_list/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/__init__.py
+-rw-r--r--   0        0        0    13543 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/index.py
+-rw-r--r--   0        0        0      120 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/port.yaml
+-rw-r--r--   0        0        0     1056 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/LICENSE
+-rw-r--r--   0        0        0       53 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/__init__.py
+-rw-r--r--   0        0        0     3359 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/index.py
+-rw-r--r--   0        0        0      124 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/port.yaml
+-rw-r--r--   0        0        0       51 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/__init__.py
+-rw-r--r--   0        0        0     4568 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/index.py
+-rw-r--r--   0        0        0       50 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/__init__.py
+-rw-r--r--   0        0        0     2035 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/index.py
+-rw-r--r--   0        0        0       26 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/py.typed
+-rw-r--r--   0        0        0     3122 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/substitution.py
+-rw-r--r--   0        0        0     5766 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/port.yaml
+-rw-r--r--   0        0        0     1075 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/LICENSE
+-rw-r--r--   0        0        0     5191 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/README.md
+-rw-r--r--   0        0        0       47 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/index.py
+-rw-r--r--   0        0        0      245 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/port.yaml
+-rw-r--r--   0        0        0      364 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/utils.py
+-rw-r--r--   0        0        0     1791 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/wordcount/__init__.py
+-rw-r--r--   0        0        0     1899 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      536 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/tox.ini
+-rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 mdit_py_plugins-0.4.0/PKG-INFO
```

### Comparing `mdit-py-plugins-0.3.5/.github/workflows/tests.yml` & `mdit_py_plugins-0.4.0/.github/workflows/tests.yml`

 * *Files 15% similar despite different names*

```diff
@@ -13,61 +13,69 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
-    - uses: pre-commit/action@v2.0.0
+    - uses: pre-commit/action@v3.0.0
 
   tests:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['pypy-3.7', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['pypy-3.8', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[testing]
     - name: Run pytest
       run: |
         pytest --cov=mdit_py_plugins --cov-report=xml --cov-report=term-missing
     - name: Upload to Codecov
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
         name: mdit-py-plugins-pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
 
+  allgood:
+    runs-on: ubuntu-latest
+    needs:
+    - pre-commit
+    - tests
+    steps:
+    - run: echo "Great success!"
+
   publish:
 
     name: Publish to PyPi
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.8"
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
```

### Comparing `mdit-py-plugins-0.3.5/.gitignore` & `mdit_py_plugins-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/LICENSE` & `mdit_py_plugins-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/README.md` & `mdit_py_plugins-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/admon/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/admon/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/admon/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/index.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,169 @@
-# Process admonitions and pass to cb.
+from __future__ import annotations
 
-import math
-from typing import Callable, Optional, Tuple
+import itertools
+from typing import TYPE_CHECKING, Sequence
 
 from markdown_it import MarkdownIt
+from markdown_it.common.utils import escapeHtml
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
 
-def get_tag(params: str) -> Tuple[str, str]:
-    if not params.strip():
-        return "", ""
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
 
-    tag, *_title = params.strip().split(" ")
-    joined = " ".join(_title)
 
-    title = ""
-    if not joined:
-        title = tag.title()
-    elif joined != '""':
-        title = joined
-    return tag.lower(), title
+def myst_block_plugin(md: MarkdownIt) -> None:
+    """Parse MyST targets (``(name)=``), blockquotes (``% comment``) and block breaks (``+++``)."""
+    md.block.ruler.before(
+        "blockquote",
+        "myst_line_comment",
+        line_comment,
+        {"alt": ["paragraph", "reference", "blockquote", "list", "footnote_def"]},
+    )
+    md.block.ruler.before(
+        "hr",
+        "myst_block_break",
+        block_break,
+        {"alt": ["paragraph", "reference", "blockquote", "list", "footnote_def"]},
+    )
+    md.block.ruler.before(
+        "hr",
+        "myst_target",
+        target,
+        {"alt": ["paragraph", "reference", "blockquote", "list", "footnote_def"]},
+    )
+    md.add_render_rule("myst_target", render_myst_target)
+    md.add_render_rule("myst_line_comment", render_myst_line_comment)
+
+
+def line_comment(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
+    if is_code_block(state, startLine):
+        return False
+
+    pos = state.bMarks[startLine] + state.tShift[startLine]
+    maximum = state.eMarks[startLine]
 
+    if state.src[pos] != "%":
+        return False
 
-def validate(params: str) -> bool:
-    tag = params.strip().split(" ", 1)[-1] or ""
-    return bool(tag)
+    if silent:
+        return True
 
+    token = state.push("myst_line_comment", "", 0)
+    token.attrSet("class", "myst-line-comment")
+    token.content = state.src[pos + 1 : maximum].rstrip()
+    token.markup = "%"
+
+    # search end of block while appending lines to `token.content`
+    for nextLine in itertools.count(startLine + 1):
+        if nextLine >= endLine:
+            break
+        pos = state.bMarks[nextLine] + state.tShift[nextLine]
+        maximum = state.eMarks[nextLine]
 
-MIN_MARKERS = 3
-MARKER_STR = "!"
-MARKER_CHAR = ord(MARKER_STR)
-MARKER_LEN = len(MARKER_STR)
+        if state.src[pos] != "%":
+            break
+        token.content += "\n" + state.src[pos + 1 : maximum].rstrip()
 
+    state.line = nextLine
+    token.map = [startLine, nextLine]
+
+    return True
 
-def admonition(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
-    start = state.bMarks[startLine] + state.tShift[startLine]
-    maximum = state.eMarks[startLine]
 
-    # Check out the first character quickly, which should filter out most of non-containers
-    if ord(state.src[start]) != MARKER_CHAR:
+def block_break(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
+    if is_code_block(state, startLine):
         return False
 
-    # Check out the rest of the marker string
-    pos = start + 1
-    while pos <= maximum and MARKER_STR[(pos - start) % MARKER_LEN] == state.src[pos]:
-        pos += 1
+    pos = state.bMarks[startLine] + state.tShift[startLine]
+    maximum = state.eMarks[startLine]
+
+    marker = state.src[pos]
+    pos += 1
 
-    marker_count = math.floor((pos - start) / MARKER_LEN)
-    if marker_count < MIN_MARKERS:
+    # Check block marker
+    if marker != "+":
         return False
-    marker_pos = pos - ((pos - start) % MARKER_LEN)
-    params = state.src[marker_pos:maximum]
-    markup = state.src[start:marker_pos]
 
-    if not validate(params):
+    # markers can be mixed with spaces, but there should be at least 3 of them
+
+    cnt = 1
+    while pos < maximum:
+        ch = state.src[pos]
+        if ch != marker and ch not in ("\t", " "):
+            break
+        if ch == marker:
+            cnt += 1
+        pos += 1
+
+    if cnt < 3:
         return False
 
-    # Since start is found, we can report success here in validation mode
     if silent:
         return True
 
-    old_parent = state.parentType
-    old_line_max = state.lineMax
-    old_indent = state.blkIndent
-
-    blk_start = pos
-    while blk_start < maximum and state.src[blk_start] == " ":
-        blk_start += 1
-
-    state.parentType = "admonition"
-    state.blkIndent += blk_start - start
-
-    was_empty = False
-
-    # Search for the end of the block
-    next_line = startLine
-    while True:
-        next_line += 1
-        if next_line >= endLine:
-            # unclosed block should be autoclosed by end of document.
-            # also block seems to be autoclosed by end of parent
-            break
-        pos = state.bMarks[next_line] + state.tShift[next_line]
-        maximum = state.eMarks[next_line]
-        is_empty = state.sCount[next_line] < state.blkIndent
+    state.line = startLine + 1
 
-        # two consecutive empty lines autoclose the block
-        if is_empty and was_empty:
-            break
-        was_empty = is_empty
+    token = state.push("myst_block_break", "hr", 0)
+    token.attrSet("class", "myst-block")
+    token.content = state.src[pos:maximum].strip()
+    token.map = [startLine, state.line]
+    token.markup = marker * cnt
 
-        if pos < maximum and state.sCount[next_line] < state.blkIndent:
-            # non-empty line with negative indent should stop the block:
-            # - !!!
-            #  test
-            break
+    return True
 
-    # this will prevent lazy continuations from ever going past our end marker
-    state.lineMax = next_line
 
-    tag, title = get_tag(params)
+def target(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
+    if is_code_block(state, startLine):
+        return False
 
-    token = state.push("admonition_open", "div", 1)
-    token.markup = markup
-    token.block = True
-    token.attrs = {"class": f"admonition {tag}"}
-    token.meta = {"tag": tag}
-    token.content = title
-    token.info = params
-    token.map = [startLine, next_line]
-
-    if title:
-        title_markup = f"{markup} {tag}"
-        token = state.push("admonition_title_open", "p", 1)
-        token.markup = title_markup
-        token.attrs = {"class": "admonition-title"}
-        token.map = [startLine, startLine + 1]
-
-        token = state.push("inline", "", 0)
-        token.content = title
-        token.map = [startLine, startLine + 1]
-        token.children = []
-
-        token = state.push("admonition_title_close", "p", -1)
-        token.markup = title_markup
-
-    state.md.block.tokenize(state, startLine + 1, next_line)
-
-    token = state.push("admonition_close", "div", -1)
-    token.markup = state.src[start:pos]
-    token.block = True
-
-    state.parentType = old_parent
-    state.lineMax = old_line_max
-    state.blkIndent = old_indent
-    state.line = next_line
+    pos = state.bMarks[startLine] + state.tShift[startLine]
+    maximum = state.eMarks[startLine]
 
-    return True
+    text = state.src[pos:maximum].strip()
+    if not text.startswith("("):
+        return False
+    if not text.endswith(")="):
+        return False
+    if not text[1:-2]:
+        return False
 
+    if silent:
+        return True
 
-def admon_plugin(md: MarkdownIt, render: Optional[Callable] = None) -> None:
-    """Plugin to use
-    `python-markdown style admonitions
-    <https://python-markdown.github.io/extensions/admonition>`_.
-
-    .. code-block:: md
-
-        !!! note
-            *content*
-
-    Note, this is ported from
-    `markdown-it-admon
-    <https://github.com/commenthol/markdown-it-admon>`_.
-    """
-
-    def renderDefault(self, tokens, idx, _options, env):
-        return self.renderToken(tokens, idx, _options, env)
-
-    render = render or renderDefault
-
-    md.add_render_rule("admonition_open", render)
-    md.add_render_rule("admonition_close", render)
-    md.add_render_rule("admonition_title_open", render)
-    md.add_render_rule("admonition_title_close", render)
+    state.line = startLine + 1
 
-    md.block.ruler.before(
-        "fence",
-        "admonition",
-        admonition,
-        {"alt": ["paragraph", "reference", "blockquote", "list"]},
-    )
+    token = state.push("myst_target", "", 0)
+    token.attrSet("class", "myst-target")
+    token.content = text[1:-2]
+    token.map = [startLine, state.line]
+
+    return True
+
+
+def render_myst_target(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
+    label = tokens[idx].content
+    class_name = "myst-target"
+    target = f'<a href="#{label}">({label})=</a>'
+    return f'<div class="{class_name}">{target}</div>'
+
+
+def render_myst_line_comment(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
+    # Strip leading whitespace from all lines
+    content = "\n".join(line.lstrip() for line in tokens[idx].content.split("\n"))
+    return f"<!-- {escapeHtml(content)} -->"
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/amsmath/__init__.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/amsmath/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """An extension to capture amsmath latex environments."""
+from __future__ import annotations
+
 import re
-from typing import Callable, Optional
+from typing import TYPE_CHECKING, Callable, Optional, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
+
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 # Taken from amsmath version 2.1
 # http://anorien.csc.warwick.ac.uk/mirrors/CTAN/macros/latex/required/amsmath/amsldoc.pdf
 ENVIRONMENTS = [
     # 3.2 single equation with an automatically gen-erated number
     "equation",
     # 3.3 variation equation, used for equations that dont fit on a single line
     "multline",
@@ -43,15 +52,17 @@
 # 3.7 variants gathered, aligned,and alignedat are provided
 # whose total width is the actual width of the contents;
 # thus they can be used as a component in a containing expression
 
 RE_OPEN = re.compile(r"\\begin\{(" + "|".join(ENVIRONMENTS) + r")([\*]?)\}")
 
 
-def amsmath_plugin(md: MarkdownIt, *, renderer: Optional[Callable[[str], str]] = None):
+def amsmath_plugin(
+    md: MarkdownIt, *, renderer: Optional[Callable[[str], str]] = None
+) -> None:
     """Parses TeX math equations, without any surrounding delimiters,
     only for top-level `amsmath <https://ctan.org/pkg/amsmath>`__ environments:
 
     .. code-block:: latex
 
         \\begin{gather*}
         a_1=b_1+c_1\\\\
@@ -66,38 +77,45 @@
         "amsmath",
         amsmath_block,
         {"alt": ["paragraph", "reference", "blockquote", "list", "footnote_def"]},
     )
 
     _renderer = (lambda content: escapeHtml(content)) if renderer is None else renderer
 
-    def render_amsmath_block(self, tokens, idx, options, env):
+    def render_amsmath_block(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         content = _renderer(str(tokens[idx].content))
         return f'<div class="math amsmath">\n{content}\n</div>\n'
 
     md.add_render_rule("amsmath", render_amsmath_block)
 
 
-def match_environment(string):
+def match_environment(string: str) -> None | tuple[str, str, int]:
     match_open = RE_OPEN.match(string)
     if not match_open:
         return None
     environment = match_open.group(1)
     numbered = match_open.group(2)
     match_close = re.search(
         r"\\end\{" + environment + numbered.replace("*", r"\*") + "\\}", string
     )
     if not match_close:
         return None
     return (environment, numbered, match_close.end())
 
 
-def amsmath_block(state: StateBlock, startLine: int, endLine: int, silent: bool):
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+def amsmath_block(
+    state: StateBlock, startLine: int, endLine: int, silent: bool
+) -> bool:
+    if is_code_block(state, startLine):
         return False
 
     begin = state.bMarks[startLine] + state.tShift[startLine]
 
     outcome = match_environment(state.src[begin:])
     if not outcome:
         return False
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/anchors/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     min_level: int = 1,
     max_level: int = 2,
     slug_func: Optional[Callable[[str], str]] = None,
     permalink: bool = False,
     permalinkSymbol: str = "¶",
     permalinkBefore: bool = False,
     permalinkSpace: bool = True,
-):
+) -> None:
     """Plugin for adding header anchors, based on
     `markdown-it-anchor <https://github.com/valeriangalliat/markdown-it-anchor>`__
 
     .. code-block:: md
 
         # Title String
 
@@ -60,16 +60,16 @@
 def _make_anchors_func(
     selected_levels: List[int],
     slug_func: Callable[[str], str],
     permalink: bool,
     permalinkSymbol: str,
     permalinkBefore: bool,
     permalinkSpace: bool,
-):
-    def _anchor_func(state: StateCore):
+) -> Callable[[StateCore], None]:
+    def _anchor_func(state: StateCore) -> None:
         slugs: Set[str] = set()
         for idx, token in enumerate(state.tokens):
             if token.type != "heading_open":
                 continue
             level = int(token.tag[1])
             if level not in selected_levels:
                 continue
@@ -111,19 +111,19 @@
                         ([Token("text", "", 0, content=" ")] if permalinkSpace else [])
                         + link_tokens
                     )
 
     return _anchor_func
 
 
-def slugify(title: str):
+def slugify(title: str) -> str:
     return re.sub(r"[^\w\u4e00-\u9fff\- ]", "", title.strip().lower().replace(" ", "-"))
 
 
-def unique_slug(slug: str, slugs: set):
+def unique_slug(slug: str, slugs: Set[str]) -> str:
     uniq = slug
     i = 1
     while uniq in slugs:
         uniq = f"{slug}-{i}"
         i += 1
     slugs.add(uniq)
     return uniq
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/attrs/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import List, Optional
+from typing import List, Optional, Sequence
 
 from markdown_it import MarkdownIt
-from markdown_it.common.utils import isSpace
 from markdown_it.rules_block import StateBlock
 from markdown_it.rules_core import StateCore
 from markdown_it.rules_inline import StateInline
 from markdown_it.token import Token
 
+from mdit_py_plugins.utils import is_code_block
+
 from .parse import ParseError, parse
 
 
 def attrs_plugin(
     md: MarkdownIt,
     *,
-    after=("image", "code_inline", "link_close", "span_close"),
-    spans=False,
-    span_after="link",
-):
+    after: Sequence[str] = ("image", "code_inline", "link_close", "span_close"),
+    spans: bool = False,
+    span_after: str = "link",
+) -> None:
     """Parse inline attributes that immediately follow certain inline elements::
 
         ![alt](https://image.com){#id .a b=c}
 
     This syntax is inspired by
     `Djot spans
     <https://htmlpreview.github.io/?https://github.com/jgm/djot/blob/master/doc/syntax.html#inline-attributes>`_.
@@ -45,15 +46,15 @@
         This plugin does not support attributes after emphasis, strikethrough or text elements,
         which all require post-parse processing.
     :param spans: If True, also parse attributes after spans of text, encapsulated by `[]`.
         Note Markdown link references take precedence over this syntax.
     :param span_after: The name of an inline rule after which spans may be specified.
     """
 
-    def _attr_inline_rule(state: StateInline, silent: bool):
+    def _attr_inline_rule(state: StateInline, silent: bool) -> bool:
         if state.pending or not state.tokens:
             return False
         token = state.tokens[-1]
         if token.type not in after:
             return False
         try:
             new_pos, attrs = parse(state.src[state.pos :])
@@ -72,15 +73,15 @@
 
     if spans:
         md.inline.ruler.after(span_after, "span", _span_rule)
     if after:
         md.inline.ruler.push("attr", _attr_inline_rule)
 
 
-def attrs_block_plugin(md: MarkdownIt):
+def attrs_block_plugin(md: MarkdownIt) -> None:
     """Parse block attributes.
 
     Block attributes are attributes on a single line, with no other content.
     They attach the specified attributes to the block below them::
 
         {.a #b c=1}
         A paragraph, that will be assigned the class ``a`` and the identifier ``b``.
@@ -106,16 +107,16 @@
         level += tokens[index].nesting
         if level == 0:
             return index
         index -= 1
     return None
 
 
-def _span_rule(state: StateInline, silent: bool):
-    if state.srcCharCode[state.pos] != 0x5B:  # /* [ */
+def _span_rule(state: StateInline, silent: bool) -> bool:
+    if state.src[state.pos] != "[":
         return False
 
     maximum = state.posMax
     labelStart = state.pos + 1
     labelEnd = state.md.helpers.parseLinkLabel(state, state.pos, False)
 
     # parser failed to find ']', so it's not a valid span
@@ -135,15 +136,15 @@
 
     pos += new_pos + 1
 
     if not silent:
         state.pos = labelStart
         state.posMax = labelEnd
         token = state.push("span_open", "span", 1)
-        token.attrs = attrs
+        token.attrs = attrs  # type: ignore
         state.md.inline.tokenize(state)
         token = state.push("span_close", "span", -1)
 
     state.pos = pos
     state.posMax = maximum
     return True
 
@@ -152,32 +153,31 @@
     state: StateBlock, startLine: int, endLine: int, silent: bool
 ) -> bool:
     """Find a block of attributes.
 
     The block must be a single line that begins with a `{`, after three or less spaces,
     and end with a `}` followed by any number if spaces.
     """
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if is_code_block(state, startLine):
         return False
 
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
     # if it doesn't start with a {, it's not an attribute block
-    if state.srcCharCode[pos] != 0x7B:  # /* { */
+    if state.src[pos] != "{":
         return False
 
     # find first non-space character from the right
-    while maximum > pos and isSpace(state.srcCharCode[maximum - 1]):
+    while maximum > pos and state.src[maximum - 1] in (" ", "\t"):
         maximum -= 1
     # if it doesn't end with a }, it's not an attribute block
     if maximum <= pos:
         return False
-    if state.srcCharCode[maximum - 1] != 0x7D:  # /* } */
+    if state.src[maximum - 1] != "}":
         return False
 
     try:
         new_pos, attrs = parse(state.src[pos:maximum])
     except ParseError:
         return False
 
@@ -193,15 +193,15 @@
     token.attrs = attrs  # type: ignore
     token.map = [startLine, startLine + 1]
 
     state.line = startLine + 1
     return True
 
 
-def _attr_resolve_block_rule(state: StateCore):
+def _attr_resolve_block_rule(state: StateCore) -> None:
     """Find attribute block then move its attributes to the next block."""
     i = 0
     len_tokens = len(state.tokens)
     while i < len_tokens:
         if state.tokens[i].type != "attrs_block":
             i += 1
             continue
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/attrs/parse.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 
 REGEX_SPACE = re.compile(r"\s")
 REGEX_SPACE_PUNCTUATION = re.compile(r"[\s!\"#$%&'()*+,./;<=>?@[\]^`{|}~]")
 REGEX_KEY_CHARACTERS = re.compile(r"[a-zA-Z\d_:-]")
 
 
 class TokenState:
-    def __init__(self):
-        self._tokens = []
+    def __init__(self) -> None:
+        self._tokens: list[tuple[int, int, str]] = []
         self.start: int = 0
 
     def set_start(self, start: int) -> None:
         self.start = start
 
-    def append(self, start: int, end: int, ttype: str):
+    def append(self, start: int, end: int, ttype: str) -> None:
         self._tokens.append((start, end, ttype))
 
     def compile(self, string: str) -> dict[str, str]:
         """compile the tokens into a dictionary"""
         attributes = {}
         classes = []
         idx = 0
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/colon_fence.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/colon_fence.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Sequence
+
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml, unescapeAll
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
+
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 
-def colon_fence_plugin(md: MarkdownIt):
+def colon_fence_plugin(md: MarkdownIt) -> None:
     """This plugin directly mimics regular fences, but with `:` colons.
 
     Example::
 
         :::name
         contained text
         :::
@@ -19,35 +30,33 @@
         "colon_fence",
         _rule,
         {"alt": ["paragraph", "reference", "blockquote", "list", "footnote_def"]},
     )
     md.add_render_rule("colon_fence", _render)
 
 
-def _rule(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def _rule(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
+    if is_code_block(state, startLine):
+        return False
+
     haveEndMarker = False
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
-        return False
-
     if pos + 3 > maximum:
         return False
 
-    marker = state.srcCharCode[pos]
+    marker = state.src[pos]
 
-    # /* : */
-    if marker != 0x3A:
+    if marker != ":":
         return False
 
     # scan marker length
     mem = pos
-    pos = state.skipChars(pos, marker)
+    pos = _skipCharsStr(state, pos, marker)
 
     length = pos - mem
 
     if length < 3:
         return False
 
     markup = state.src[mem:pos]
@@ -72,22 +81,21 @@
 
         if pos < maximum and state.sCount[nextLine] < state.blkIndent:
             # non-empty line with negative indent should stop the list:
             # - ```
             #  test
             break
 
-        if state.srcCharCode[pos] != marker:
+        if state.src[pos] != marker:
             continue
 
-        if state.sCount[nextLine] - state.blkIndent >= 4:
-            # closing fence should be indented less than 4 spaces
+        if is_code_block(state, nextLine):
             continue
 
-        pos = state.skipChars(pos, marker)
+        pos = _skipCharsStr(state, pos, marker)
 
         # closing code fence must be at least as long as the opening one
         if pos - mem < length:
             continue
 
         # make sure tail has spaces only
         pos = state.skipSpaces(pos)
@@ -109,15 +117,35 @@
     token.content = state.getLines(startLine + 1, nextLine, length, True)
     token.markup = markup
     token.map = [startLine, state.line]
 
     return True
 
 
-def _render(self, tokens, idx, options, env):
+def _skipCharsStr(state: StateBlock, pos: int, ch: str) -> int:
+    """Skip character string from given position."""
+    # TODO this can be replaced with StateBlock.skipCharsStr in markdown-it-py 3.0.0
+    while True:
+        try:
+            current = state.src[pos]
+        except IndexError:
+            break
+        if current != ch:
+            break
+        pos += 1
+    return pos
+
+
+def _render(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     token = tokens[idx]
     info = unescapeAll(token.info).strip() if token.info else ""
     content = escapeHtml(token.content)
     block_name = ""
 
     if info:
         block_name = info.split()[0]
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/container/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/container/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/container/README.md` & `mdit_py_plugins-0.4.0/mdit_py_plugins/container/README.md`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/container/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/container/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """Process block-level custom containers."""
+from __future__ import annotations
+
 from math import floor
-from typing import Callable, Optional
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from markdown_it import MarkdownIt
-from markdown_it.common.utils import charCodeAt
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
+
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 
 def container_plugin(
     md: MarkdownIt,
     name: str,
     marker: str = ":",
-    validate: Optional[Callable[[str, str], bool]] = None,
-    render=None,
-):
+    validate: None | Callable[[str, str], bool] = None,
+    render: None | Callable[..., str] = None,
+) -> None:
     """Plugin ported from
     `markdown-it-container <https://github.com/markdown-it/markdown-it-container>`__.
 
     It is a plugin for creating block-level custom containers:
 
     .. code-block:: md
 
@@ -30,39 +38,50 @@
     :param name: the name of the container to parse
     :param marker: the marker character to use
     :param validate: func(marker, param) -> bool, default matches against the name
     :param render: render func
 
     """
 
-    def validateDefault(params: str, *args):
+    def validateDefault(params: str, *args: Any) -> bool:
         return params.strip().split(" ", 2)[0] == name
 
-    def renderDefault(self, tokens, idx, _options, env):
+    def renderDefault(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        _options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         # add a class to the opening tag
         if tokens[idx].nesting == 1:
             tokens[idx].attrJoin("class", name)
 
-        return self.renderToken(tokens, idx, _options, env)
+        return self.renderToken(tokens, idx, _options, env)  # type: ignore
 
     min_markers = 3
     marker_str = marker
-    marker_char = charCodeAt(marker_str, 0)
+    marker_char = marker_str[0]
     marker_len = len(marker_str)
     validate = validate or validateDefault
     render = render or renderDefault
 
-    def container_func(state: StateBlock, startLine: int, endLine: int, silent: bool):
+    def container_func(
+        state: StateBlock, startLine: int, endLine: int, silent: bool
+    ) -> bool:
+        if is_code_block(state, startLine):
+            return False
+
         auto_closed = False
         start = state.bMarks[startLine] + state.tShift[startLine]
         maximum = state.eMarks[startLine]
 
         # Check out the first character quickly,
         # this should filter out most of non-containers
-        if marker_char != state.srcCharCode[start]:
+        if marker_char != state.src[start]:
             return False
 
         # Check out the rest of the marker string
         pos = start + 1
         while pos <= maximum:
             try:
                 character = state.src[pos]
@@ -102,19 +121,18 @@
 
             if start < maximum and state.sCount[nextLine] < state.blkIndent:
                 # non-empty line with negative indent should stop the list:
                 # - ```
                 #  test
                 break
 
-            if marker_char != state.srcCharCode[start]:
+            if marker_char != state.src[start]:
                 continue
 
-            if state.sCount[nextLine] - state.blkIndent >= 4:
-                # closing fence should be indented less than 4 spaces
+            if is_code_block(state, nextLine):
                 continue
 
             pos = start + 1
             while pos <= maximum:
                 try:
                     character = state.src[pos]
                 except IndexError:
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/README.md` & `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/README.md`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/deflist/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Process definition lists."""
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
 
-def deflist_plugin(md: MarkdownIt):
+
+def deflist_plugin(md: MarkdownIt) -> None:
     """Plugin ported from
     `markdown-it-deflist <https://github.com/markdown-it/markdown-it-deflist>`__.
 
     The syntax is based on
     `pandoc definition lists <http://johnmacfarlane.net/pandoc/README.html#definition-lists>`__:
 
     .. code-block:: md
@@ -18,58 +20,60 @@
           second paragraph
 
         Term 2 with *inline markup*
         ~ Definition 2a compact style
         ~ Definition 2b
 
     """
-    isSpace = md.utils.isSpace
 
-    def skipMarker(state: StateBlock, line: int):
+    def skipMarker(state: StateBlock, line: int) -> int:
         """Search `[:~][\n ]`, returns next pos after marker on success or -1 on fail."""
         start = state.bMarks[line] + state.tShift[line]
         maximum = state.eMarks[line]
 
         if start >= maximum:
             return -1
 
         # Check bullet
-        marker = state.srcCharCode[start]
+        marker = state.src[start]
         start += 1
-        if marker != 0x7E and marker != 0x3A:  # ~ :
+        if marker != "~" and marker != ":":
             return -1
 
         pos = state.skipSpaces(start)
 
         # require space after ":"
         if start == pos:
             return -1
 
         # no empty definitions, e.g. "  : "
         if pos >= maximum:
             return -1
 
         return start
 
-    def markTightParagraphs(state: StateBlock, idx: int):
+    def markTightParagraphs(state: StateBlock, idx: int) -> None:
         level = state.level + 2
 
         i = idx + 2
         l2 = len(state.tokens) - 2
         while i < l2:
             if (
                 state.tokens[i].level == level
                 and state.tokens[i].type == "paragraph_open"
             ):
                 state.tokens[i + 2].hidden = True
                 state.tokens[i].hidden = True
                 i += 2
             i += 1
 
-    def deflist(state: StateBlock, startLine: int, endLine: int, silent: bool):
+    def deflist(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
+        if is_code_block(state, startLine):
+            return False
+
         if silent:
             # quirk: validation mode validates a dd block only, not a whole deflist
             if state.ddIndent < 0:
                 return False
             return skipMarker(state, startLine) >= 0
 
         nextLine = startLine + 1
@@ -130,21 +134,18 @@
                 offset = (
                     state.sCount[ddLine]
                     + contentStart
                     - (state.bMarks[ddLine] + state.tShift[ddLine])
                 )
 
                 while pos < maximum:
-                    ch = state.srcCharCode[pos]
-
-                    if isSpace(ch):
-                        if ch == 0x09:
-                            offset += 4 - offset % 4
-                        else:
-                            offset += 1
+                    if state.src[pos] == "\t":
+                        offset += 4 - offset % 4
+                    elif state.src[pos] == " ":
+                        offset += 1
                     else:
                         break
 
                     pos += 1
 
                 contentStart = pos
 
@@ -156,15 +157,15 @@
                 oldParentType = state.parentType
                 state.blkIndent = state.ddIndent = state.sCount[ddLine] + 2
                 state.tShift[ddLine] = contentStart - state.bMarks[ddLine]
                 state.sCount[ddLine] = offset
                 state.tight = True
                 state.parentType = "deflist"
 
-                state.md.block.tokenize(state, ddLine, endLine, True)
+                state.md.block.tokenize(state, ddLine, endLine)
 
                 # If any of list item is tight, mark list as tight
                 if not state.tight or prevEmptyEnd:
                     tight = False
 
                 # Item become loose if finish with empty line,
                 # but we should filter last element, because it means list finish
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/dollarmath/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+from __future__ import annotations
+
 import re
-from typing import Any, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml, isWhiteSpace
 from markdown_it.rules_block import StateBlock
 from markdown_it.rules_inline import StateInline
 
+from mdit_py_plugins.utils import is_code_block
+
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 
 def dollarmath_plugin(
     md: MarkdownIt,
     *,
     allow_labels: bool = True,
     allow_space: bool = True,
     allow_digits: bool = True,
+    allow_blank_lines: bool = True,
     double_inline: bool = False,
     label_normalizer: Optional[Callable[[str], str]] = None,
     renderer: Optional[Callable[[str, Dict[str, Any]], str]] = None,
     label_renderer: Optional[Callable[[str], str]] = None,
 ) -> None:
     """Plugin for parsing dollar enclosed math,
     e.g. inline: ``$a=1$``, block: ``$$b=2$$``
@@ -26,14 +36,18 @@
 
     :param allow_labels: Capture math blocks with label suffix, e.g. ``$$a=1$$ (eq1)``
     :param allow_space: Parse inline math when there is space
         after/before the opening/closing ``$``, e.g. ``$ a $``
     :param allow_digits: Parse inline math when there is a digit
         before/after the opening/closing ``$``, e.g. ``1$`` or ``$2``.
         This is useful when also using currency.
+    :param allow_blank_lines: Allow blank lines inside ``$$``. Note that blank lines are
+        not allowed in LaTeX, executablebooks/markdown-it-dollarmath, or the Github or
+        StackExchange markdown dialects. Hoever, they have special semantics if used
+        within Sphinx `..math` admonitions, so are allowed for backwards-compatibility.
     :param double_inline: Search for double-dollar math within inline contexts
     :param label_normalizer: Function to normalize the label,
         by default replaces whitespace with `-`
     :param renderer: Function to render content: `(str, {"display_mode": bool}) -> str`,
         by default escapes HTML
     :param label_renderer: Function to render labels, by default creates anchor
 
@@ -43,45 +57,72 @@
 
     md.inline.ruler.before(
         "escape",
         "math_inline",
         math_inline_dollar(allow_space, allow_digits, double_inline),
     )
     md.block.ruler.before(
-        "fence", "math_block", math_block_dollar(allow_labels, label_normalizer)
+        "fence",
+        "math_block",
+        math_block_dollar(allow_labels, label_normalizer, allow_blank_lines),
     )
 
     # TODO the current render rules are really just for testing
     # would be good to allow "proper" math rendering,
     # e.g. https://github.com/roniemartinez/latex2mathml
 
     _renderer = (
         (lambda content, _: escapeHtml(content)) if renderer is None else renderer
     )
 
+    _label_renderer: Callable[[str], str]
     if label_renderer is None:
         _label_renderer = (
             lambda label: f'<a href="#{label}" class="mathlabel" title="Permalink to this equation">¶</a>'  # noqa: E501
         )
     else:
         _label_renderer = label_renderer
 
-    def render_math_inline(self, tokens, idx, options, env) -> str:
+    def render_math_inline(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         content = _renderer(str(tokens[idx].content).strip(), {"display_mode": False})
         return f'<span class="math inline">{content}</span>'
 
-    def render_math_inline_double(self, tokens, idx, options, env) -> str:
+    def render_math_inline_double(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         content = _renderer(str(tokens[idx].content).strip(), {"display_mode": True})
         return f'<div class="math inline">{content}</div>'
 
-    def render_math_block(self, tokens, idx, options, env) -> str:
+    def render_math_block(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         content = _renderer(str(tokens[idx].content).strip(), {"display_mode": True})
         return f'<div class="math block">\n{content}\n</div>\n'
 
-    def render_math_block_label(self, tokens, idx, options, env) -> str:
+    def render_math_block_label(
+        self: RendererProtocol,
+        tokens: Sequence[Token],
+        idx: int,
+        options: OptionsDict,
+        env: EnvType,
+    ) -> str:
         content = _renderer(str(tokens[idx].content).strip(), {"display_mode": True})
         _id = tokens[idx].info
         label = _label_renderer(tokens[idx].info)
         return f'<div id="{_id}" class="math block">\n{label}\n{content}\n</div>\n'
 
     md.add_render_rule("math_inline", render_math_inline)
     md.add_render_rule("math_inline_double", render_math_inline_double)
@@ -92,15 +133,15 @@
 
 def is_escaped(state: StateInline, back_pos: int, mod: int = 0) -> bool:
     """Test if dollar is escaped."""
     # count how many \ are before the current position
     backslashes = 0
     while back_pos >= 0:
         back_pos = back_pos - 1
-        if state.srcCharCode[back_pos] == 0x5C:  # /* \ */
+        if state.src[back_pos] == "\\":
             backslashes += 1
         else:
             break
 
     if not backslashes:
         return False
 
@@ -140,21 +181,21 @@
             - check if the next character is a digit (if not allow_digits)
         - Check empty content
         """
 
         # TODO options:
         # even/odd backslash escaping
 
-        if state.srcCharCode[state.pos] != 0x24:  # /* $ */
+        if state.src[state.pos] != "$":
             return False
 
         if not allow_space:
             # whitespace not allowed straight after opening $
             try:
-                if isWhiteSpace(state.srcCharCode[state.pos + 1]):
+                if isWhiteSpace(ord(state.src[state.pos + 1])):
                     return False
             except IndexError:
                 return False
 
         if not allow_digits:
             # digit not allowed straight before opening $
             try:
@@ -163,33 +204,33 @@
             except IndexError:
                 pass
 
         if is_escaped(state, state.pos):
             return False
 
         try:
-            is_double = allow_double and state.srcCharCode[state.pos + 1] == 0x24
+            is_double = allow_double and state.src[state.pos + 1] == "$"
         except IndexError:
             return False
 
         # find closing $
         pos = state.pos + 1 + (1 if is_double else 0)
         found_closing = False
         while not found_closing:
             try:
-                end = state.srcCharCode.index(0x24, pos)
+                end = state.src.index("$", pos)
             except ValueError:
                 return False
 
             if is_escaped(state, end):
                 pos = end + 1
                 continue
 
             try:
-                if is_double and state.srcCharCode[end + 1] != 0x24:
+                if is_double and state.src[end + 1] != "$":
                     pos = end + 1
                     continue
             except IndexError:
                 return False
 
             if is_double:
                 end += 1
@@ -198,15 +239,15 @@
 
         if not found_closing:
             return False
 
         if not allow_space:
             # whitespace not allowed straight before closing $
             try:
-                if isWhiteSpace(state.srcCharCode[end - 1]):
+                if isWhiteSpace(ord(state.src[end - 1])):
                     return False
             except IndexError:
                 return False
 
         if not allow_digits:
             # digit not allowed straight after closing $
             try:
@@ -242,37 +283,34 @@
 # reversed end of block dollar equation, with equation label
 DOLLAR_EQNO_REV = re.compile(r"^\s*\)([^)$\r\n]+?)\(\s*\${2}")
 
 
 def math_block_dollar(
     allow_labels: bool = True,
     label_normalizer: Optional[Callable[[str], str]] = None,
+    allow_blank_lines: bool = False,
 ) -> Callable[[StateBlock, int, int, bool], bool]:
     """Generate block dollar rule."""
 
     def _math_block_dollar(
         state: StateBlock, startLine: int, endLine: int, silent: bool
     ) -> bool:
         # TODO internal backslash escaping
 
+        if is_code_block(state, startLine):
+            return False
+
         haveEndMarker = False
         startPos = state.bMarks[startLine] + state.tShift[startLine]
         end = state.eMarks[startLine]
 
-        # if it's indented more than 3 spaces, it should be a code block
-        if state.sCount[startLine] - state.blkIndent >= 4:
-            return False
-
         if startPos + 2 > end:
             return False
 
-        if (
-            state.srcCharCode[startPos] != 0x24
-            or state.srcCharCode[startPos + 1] != 0x24
-        ):  # /* $ */
+        if state.src[startPos] != "$" or state.src[startPos + 1] != "$":
             return False
 
         # search for end of block
         nextLine = startLine
         label = None
 
         # search for end of block on same line
@@ -295,23 +333,22 @@
                 nextLine += 1
                 if nextLine >= endLine:
                     break
 
                 start = state.bMarks[nextLine] + state.tShift[nextLine]
                 end = state.eMarks[nextLine]
 
-                if end - start < 2:
-                    continue
-
                 lineText = state.src[start:end]
 
                 if lineText.strip().endswith("$$"):
                     haveEndMarker = True
                     end = end - 2 - (len(lineText) - len(lineText.strip()))
                     break
+                if lineText.strip() == "" and not allow_blank_lines:
+                    break  # blank lines are not allowed within $$
 
                 # reverse the line and match
                 if allow_labels:
                     eqnoMatch = DOLLAR_EQNO_REV.match(lineText[::-1])
                     if eqnoMatch:
                         haveEndMarker = True
                         label = eqnoMatch.group(1)[::-1]
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/field_list/__init__.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/field_list/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Field list plugin"""
 from contextlib import contextmanager
-from typing import Optional, Tuple
+from typing import Iterator, Optional, Tuple
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
 
-def fieldlist_plugin(md: MarkdownIt):
+
+def fieldlist_plugin(md: MarkdownIt) -> None:
     """Field lists are mappings from field names to field bodies, based on the
     `reStructureText syntax
     <https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#field-lists>`_.
 
     .. code-block:: md
 
         :name *markup*:
@@ -81,27 +83,28 @@
     if not name_text.strip():
         return -1, ""
 
     return pos + name_length + 1, name_text
 
 
 @contextmanager
-def set_parent_type(state: StateBlock, name: str):
+def set_parent_type(state: StateBlock, name: str) -> Iterator[None]:
     """Temporarily set parent type to `name`"""
     oldParentType = state.parentType
     state.parentType = name
     yield
     state.parentType = oldParentType
 
 
-def _fieldlist_rule(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def _fieldlist_rule(
+    state: StateBlock, startLine: int, endLine: int, silent: bool
+) -> bool:
     # adapted from markdown_it/rules_block/list.py::list_block
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if is_code_block(state, startLine):
         return False
 
     posAfterName, name_text = parseNameMarker(state, startLine)
     if posAfterName < 0:
         return False
 
     # For validation mode we can terminate immediately
@@ -134,21 +137,21 @@
                 state.sCount[nextLine]
                 + posAfterName
                 - (state.bMarks[startLine] + state.tShift[startLine])
             )
 
             # find indent to start of body on first line
             while pos < maximum:
-                ch = state.srcCharCode[pos]
+                ch = state.src[pos]
 
-                if ch == 0x09:  # \t
+                if ch == "\t":
                     first_line_body_indent += (
                         4 - (first_line_body_indent + state.bsCount[nextLine]) % 4
                     )
-                elif ch == 0x20:  # \s
+                elif ch == " ":
                     first_line_body_indent += 1
                 else:
                     break
 
                 pos += 1
 
             contentStart = pos
@@ -191,24 +194,19 @@
                 if has_first_line and block_indent < first_line_body_indent:
                     # this is a hack to get the first line to render correctly
                     # we temporarily "shift" it to the left by the difference
                     # between the first line indent and the block indent
                     # and replace the "hole" left with space,
                     # so that src indexes still match
                     diff = first_line_body_indent - block_indent
-                    state._src = (
+                    state.src = (
                         state.src[: contentStart - diff]
                         + " " * diff
                         + state.src[contentStart:]
                     )
-                    state.srcCharCode = (
-                        state.srcCharCode[: contentStart - diff]
-                        + tuple([0x20] * diff)
-                        + state.srcCharCode[contentStart:]
-                    )
 
                 state.tShift[startLine] = contentStart - diff - state.bMarks[startLine]
                 state.sCount[startLine] = first_line_body_indent - diff
                 state.blkIndent = block_indent
 
                 state.md.block.tokenize(state, startLine, endLine)
 
@@ -222,16 +220,15 @@
 
             contentStart = state.bMarks[startLine]
 
             # Try to check if list is terminated or continued.
             if state.sCount[nextLine] < state.blkIndent:
                 break
 
-            # if it's indented more than 3 spaces, it should be a code block
-            if state.sCount[startLine] - state.blkIndent >= 4:
+            if is_code_block(state, startLine):
                 break
 
             # get next field item
             posAfterName, name_text = parseNameMarker(state, startLine)
             if posAfterName < 0:
                 break
 
@@ -240,20 +237,18 @@
         listLines[1] = nextLine
         state.line = nextLine
 
     return True
 
 
 @contextmanager
-def temp_state_changes(state: StateBlock, startLine: int):
+def temp_state_changes(state: StateBlock, startLine: int) -> Iterator[None]:
     """Allow temporarily changing certain state attributes."""
     oldTShift = state.tShift[startLine]
     oldSCount = state.sCount[startLine]
     oldBlkIndent = state.blkIndent
-    oldSrc = state._src
-    oldSrcCharCode = state.srcCharCode
+    oldSrc = state.src
     yield
     state.blkIndent = oldBlkIndent
     state.tShift[startLine] = oldTShift
     state.sCount[startLine] = oldSCount
-    state._src = oldSrc
-    state.srcCharCode = oldSrcCharCode
+    state.src = oldSrc
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/footnote/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# Process footnotes
-#
+"""Process footnotes"""
+from __future__ import annotations
 
-from typing import List, Optional
+from typing import TYPE_CHECKING, List, Optional, Sequence
 
 from markdown_it import MarkdownIt
-from markdown_it.common.utils import isSpace
 from markdown_it.helpers import parseLinkLabel
 from markdown_it.rules_block import StateBlock
+from markdown_it.rules_core import StateCore
 from markdown_it.rules_inline import StateInline
 from markdown_it.token import Token
 
+from mdit_py_plugins.utils import is_code_block
 
-def footnote_plugin(md: MarkdownIt):
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.utils import EnvType, OptionsDict
+
+
+def footnote_plugin(md: MarkdownIt) -> None:
     """Plugin ported from
     `markdown-it-footnote <https://github.com/markdown-it/markdown-it-footnote>`__.
 
     It is based on the
     `pandoc definition <http://johnmacfarlane.net/pandoc/README.html#footnotes>`__:
 
     .. code-block:: md
@@ -50,41 +56,44 @@
     md.add_render_rule("footnote_caption", render_footnote_caption)
     md.add_render_rule("footnote_anchor_name", render_footnote_anchor_name)
 
 
 # ## RULES ##
 
 
-def footnote_def(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def footnote_def(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     """Process footnote block definition"""
 
+    if is_code_block(state, startLine):
+        return False
+
     start = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
     # line should be at least 5 chars - "[^x]:"
     if start + 4 > maximum:
         return False
 
-    if state.srcCharCode[start] != 0x5B:  # /* [ */
+    if state.src[start] != "[":
         return False
-    if state.srcCharCode[start + 1] != 0x5E:  # /* ^ */
+    if state.src[start + 1] != "^":
         return False
 
     pos = start + 2
     while pos < maximum:
-        if state.srcCharCode[pos] == 0x20:
+        if state.src[pos] == " ":
             return False
-        if state.srcCharCode[pos] == 0x5D:  # /* ] */
+        if state.src[pos] == "]":
             break
         pos += 1
 
     if pos == start + 2:  # no empty footnote labels
         return False
     pos += 1
-    if pos >= maximum or state.srcCharCode[pos] != 0x3A:  # /* : */
+    if pos >= maximum or state.src[pos] != ":":
         return False
     if silent:
         return True
     pos += 1
 
     label = state.src[start + 2 : pos - 2]
     state.env.setdefault("footnotes", {}).setdefault("refs", {})[":" + label] = -1
@@ -104,21 +113,20 @@
     initial = offset = (
         state.sCount[startLine]
         + pos
         - (state.bMarks[startLine] + state.tShift[startLine])
     )
 
     while pos < maximum:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        if isSpace(ch):
-            if ch == 0x09:
-                offset += 4 - offset % 4
-            else:
-                offset += 1
+        if ch == "\t":
+            offset += 4 - offset % 4
+        elif ch == " ":
+            offset += 1
 
         else:
             break
 
         pos += 1
 
     state.tShift[startLine] = pos - posAfterColon
@@ -127,15 +135,15 @@
     state.bMarks[startLine] = posAfterColon
     state.blkIndent += 4
     state.parentType = "footnote"
 
     if state.sCount[startLine] < state.blkIndent:
         state.sCount[startLine] += state.blkIndent
 
-    state.md.block.tokenize(state, startLine, endLine, True)
+    state.md.block.tokenize(state, startLine, endLine)
 
     state.parentType = oldParentType
     state.blkIndent -= 4
     state.tShift[startLine] = oldTShift
     state.sCount[startLine] = oldSCount
     state.bMarks[startLine] = oldBMark
 
@@ -145,25 +153,25 @@
     state.level -= 1
     token.level = state.level
     state.tokens.append(token)
 
     return True
 
 
-def footnote_inline(state: StateInline, silent: bool):
+def footnote_inline(state: StateInline, silent: bool) -> bool:
     """Process inline footnotes (^[...])"""
 
     maximum = state.posMax
     start = state.pos
 
     if start + 2 >= maximum:
         return False
-    if state.srcCharCode[start] != 0x5E:  # /* ^ */
+    if state.src[start] != "^":
         return False
-    if state.srcCharCode[start + 1] != 0x5B:  # /* [ */
+    if state.src[start + 1] != "[":
         return False
 
     labelStart = start + 2
     labelEnd = parseLinkLabel(state, start + 1)
 
     # parser failed to find ']', so it's not a valid note
     if labelEnd < 0:
@@ -187,38 +195,38 @@
         refs[footnoteId] = {"content": state.src[labelStart:labelEnd], "tokens": tokens}
 
     state.pos = labelEnd + 1
     state.posMax = maximum
     return True
 
 
-def footnote_ref(state: StateInline, silent: bool):
+def footnote_ref(state: StateInline, silent: bool) -> bool:
     """Process footnote references ([^...])"""
 
     maximum = state.posMax
     start = state.pos
 
     # should be at least 4 chars - "[^x]"
     if start + 3 > maximum:
         return False
 
     if "footnotes" not in state.env or "refs" not in state.env["footnotes"]:
         return False
-    if state.srcCharCode[start] != 0x5B:  # /* [ */
+    if state.src[start] != "[":
         return False
-    if state.srcCharCode[start + 1] != 0x5E:  # /* ^ */
+    if state.src[start + 1] != "^":
         return False
 
     pos = start + 2
     while pos < maximum:
-        if state.srcCharCode[pos] == 0x20:
+        if state.src[pos] == " ":
             return False
-        if state.srcCharCode[pos] == 0x0A:
+        if state.src[pos] == "\n":
             return False
-        if state.srcCharCode[pos] == 0x5D:  # /* ] */
+        if state.src[pos] == "]":
             break
         pos += 1
 
     if pos == start + 2:  # no empty footnote labels
         return False
     if pos >= maximum:
         return False
@@ -246,15 +254,15 @@
         token.meta = {"id": footnoteId, "subId": footnoteSubId, "label": label}
 
     state.pos = pos
     state.posMax = maximum
     return True
 
 
-def footnote_tail(state: StateBlock, *args, **kwargs):
+def footnote_tail(state: StateCore) -> None:
     """Post-processing step, to move footnote tokens to end of the token stream.
 
     Also removes un-referenced tokens.
     """
 
     insideRef = False
     refTokens = {}
@@ -347,37 +355,55 @@
     state.tokens.append(token)
 
 
 ########################################
 # Renderer partials
 
 
-def render_footnote_anchor_name(self, tokens, idx, options, env):
+def render_footnote_anchor_name(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     n = str(tokens[idx].meta["id"] + 1)
     prefix = ""
 
     doc_id = env.get("docId", None)
     if isinstance(doc_id, str):
         prefix = f"-{doc_id}-"
 
     return prefix + n
 
 
-def render_footnote_caption(self, tokens, idx, options, env):
+def render_footnote_caption(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     n = str(tokens[idx].meta["id"] + 1)
 
     if tokens[idx].meta.get("subId", -1) > 0:
         n += ":" + str(tokens[idx].meta["subId"])
 
     return "[" + n + "]"
 
 
-def render_footnote_ref(self, tokens, idx, options, env):
-    ident = self.rules["footnote_anchor_name"](tokens, idx, options, env)
-    caption = self.rules["footnote_caption"](tokens, idx, options, env)
+def render_footnote_ref(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
+    ident: str = self.rules["footnote_anchor_name"](tokens, idx, options, env)  # type: ignore[attr-defined]
+    caption: str = self.rules["footnote_caption"](tokens, idx, options, env)  # type: ignore[attr-defined]
     refid = ident
 
     if tokens[idx].meta.get("subId", -1) > 0:
         refid += ":" + str(tokens[idx].meta["subId"])
 
     return (
         '<sup class="footnote-ref"><a href="#fn'
@@ -386,44 +412,74 @@
         + refid
         + '">'
         + caption
         + "</a></sup>"
     )
 
 
-def render_footnote_block_open(self, tokens, idx, options, env):
+def render_footnote_block_open(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     return (
         (
             '<hr class="footnotes-sep" />\n'
             if options.xhtmlOut
             else '<hr class="footnotes-sep">\n'
         )
         + '<section class="footnotes">\n'
         + '<ol class="footnotes-list">\n'
     )
 
 
-def render_footnote_block_close(self, tokens, idx, options, env):
+def render_footnote_block_close(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     return "</ol>\n</section>\n"
 
 
-def render_footnote_open(self, tokens, idx, options, env):
-    ident = self.rules["footnote_anchor_name"](tokens, idx, options, env)
+def render_footnote_open(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
+    ident: str = self.rules["footnote_anchor_name"](tokens, idx, options, env)  # type: ignore[attr-defined]
 
     if tokens[idx].meta.get("subId", -1) > 0:
         ident += ":" + tokens[idx].meta["subId"]
 
     return '<li id="fn' + ident + '" class="footnote-item">'
 
 
-def render_footnote_close(self, tokens, idx, options, env):
+def render_footnote_close(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
     return "</li>\n"
 
 
-def render_footnote_anchor(self, tokens, idx, options, env):
-    ident = self.rules["footnote_anchor_name"](tokens, idx, options, env)
+def render_footnote_anchor(
+    self: RendererProtocol,
+    tokens: Sequence[Token],
+    idx: int,
+    options: OptionsDict,
+    env: EnvType,
+) -> str:
+    ident: str = self.rules["footnote_anchor_name"](tokens, idx, options, env)  # type: ignore[attr-defined]
 
     if tokens[idx].meta["subId"] > 0:
         ident += ":" + str(tokens[idx].meta["subId"])
 
     # ↩ with escape code to prevent display as Apple Emoji on iOS
     return ' <a href="#fnref' + ident + '" class="footnote-backref">\u21a9\uFE0E</a>'
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/front_matter/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,127 @@
-# Process front matter and pass to cb
-from math import floor
-
+"""Process front matter."""
 from markdown_it import MarkdownIt
-from markdown_it.common.utils import charCodeAt
 from markdown_it.rules_block import StateBlock
 
+from mdit_py_plugins.utils import is_code_block
+
 
-def front_matter_plugin(md: MarkdownIt):
+def front_matter_plugin(md: MarkdownIt) -> None:
     """Plugin ported from
     `markdown-it-front-matter <https://github.com/ParkSB/markdown-it-front-matter>`__.
 
     It parses initial metadata, stored between opening/closing dashes:
 
     .. code-block:: md
 
         ---
         valid-front-matter: true
         ---
 
     """
-    frontMatter = make_front_matter_rule()
     md.block.ruler.before(
         "table",
         "front_matter",
-        frontMatter,
+        _front_matter_rule,
         {"alt": ["paragraph", "reference", "blockquote", "list"]},
     )
 
 
-def make_front_matter_rule():
+def _front_matter_rule(
+    state: StateBlock, startLine: int, endLine: int, silent: bool
+) -> bool:
+    marker_chr = "-"
     min_markers = 3
-    marker_str = "-"
-    marker_char = charCodeAt(marker_str, 0)
-    marker_len = len(marker_str)
-
-    def frontMatter(state: StateBlock, startLine: int, endLine: int, silent: bool):
-        auto_closed = False
-        start = state.bMarks[startLine] + state.tShift[startLine]
-        maximum = state.eMarks[startLine]
-        src_len = len(state.src)
-
-        # Check out the first character of the first line quickly,
-        # this should filter out non-front matter
-        if startLine != 0 or marker_char != state.srcCharCode[0]:
-            return False
-
-        # Check out the rest of the marker string
-        # while pos <= 3
-        pos = start + 1
-        while pos <= maximum and pos < src_len:
-            if marker_str[(pos - start) % marker_len] != state.src[pos]:
-                break
-            pos += 1
 
-        marker_count = floor((pos - start) / marker_len)
+    auto_closed = False
+    start = state.bMarks[startLine] + state.tShift[startLine]
+    maximum = state.eMarks[startLine]
+    src_len = len(state.src)
+
+    # Check out the first character of the first line quickly,
+    # this should filter out non-front matter
+    if startLine != 0 or state.src[0] != marker_chr:
+        return False
+
+    # Check out the rest of the marker string
+    # while pos <= 3
+    pos = start + 1
+    while pos <= maximum and pos < src_len:
+        if state.src[pos] != marker_chr:
+            break
+        pos += 1
 
-        if marker_count < min_markers:
-            return False
+    marker_count = pos - start
 
-        pos -= (pos - start) % marker_len
+    if marker_count < min_markers:
+        return False
 
-        # Since start is found, we can report success here in validation mode
-        if silent:
-            return True
-
-        # Search for the end of the block
-        nextLine = startLine
-
-        while True:
-            nextLine += 1
-            if nextLine >= endLine:
-                # unclosed block should be autoclosed by end of document.
-                return False
+    # Since start is found, we can report success here in validation mode
+    if silent:
+        return True
 
-            if state.src[start:maximum] == "...":
-                break
+    # Search for the end of the block
+    nextLine = startLine
 
-            start = state.bMarks[nextLine] + state.tShift[nextLine]
-            maximum = state.eMarks[nextLine]
+    while True:
+        nextLine += 1
+        if nextLine >= endLine:
+            # unclosed block should be autoclosed by end of document.
+            return False
 
-            if start < maximum and state.sCount[nextLine] < state.blkIndent:
-                # non-empty line with negative indent should stop the list:
-                # - ```
-                #  test
-                break
+        if state.src[start:maximum] == "...":
+            break
 
-            if marker_char != state.srcCharCode[start]:
-                continue
+        start = state.bMarks[nextLine] + state.tShift[nextLine]
+        maximum = state.eMarks[nextLine]
 
-            if state.sCount[nextLine] - state.blkIndent >= 4:
-                # closing fence should be indented less than 4 spaces
-                continue
-
-            pos = start + 1
-            while pos < maximum:
-                if marker_str[(pos - start) % marker_len] != state.src[pos]:
-                    break
-                pos += 1
-
-            # closing code fence must be at least as long as the opening one
-            if floor((pos - start) / marker_len) < marker_count:
-                continue
-
-            # make sure tail has spaces only
-            pos -= (pos - start) % marker_len
-            pos = state.skipSpaces(pos)
+        if start < maximum and state.sCount[nextLine] < state.blkIndent:
+            # non-empty line with negative indent should stop the list:
+            # - ```
+            #  test
+            break
 
-            if pos < maximum:
-                continue
+        if state.src[start] != marker_chr:
+            continue
 
-            # found!
-            auto_closed = True
-            break
+        if is_code_block(state, nextLine):
+            continue
 
-        old_parent = state.parentType
-        old_line_max = state.lineMax
-        state.parentType = "container"
-
-        # this will prevent lazy continuations from ever going past our end marker
-        state.lineMax = nextLine
-
-        token = state.push("front_matter", "", 0)
-        token.hidden = True
-        token.markup = marker_str * min_markers
-        token.content = state.src[
-            state.bMarks[startLine + 1] : state.eMarks[nextLine - 1]
-        ]
-        token.block = True
-
-        state.parentType = old_parent
-        state.lineMax = old_line_max
-        state.line = nextLine + (1 if auto_closed else 0)
-        token.map = [startLine, state.line]
+        pos = start + 1
+        while pos < maximum:
+            if state.src[pos] != marker_chr:
+                break
+            pos += 1
 
-        return True
+        # closing code fence must be at least as long as the opening one
+        if (pos - start) < marker_count:
+            continue
+
+        # make sure tail has spaces only
+        pos = state.skipSpaces(pos)
+
+        if pos < maximum:
+            continue
+
+        # found!
+        auto_closed = True
+        break
+
+    old_parent = state.parentType
+    old_line_max = state.lineMax
+    state.parentType = "container"
+
+    # this will prevent lazy continuations from ever going past our end marker
+    state.lineMax = nextLine
+
+    token = state.push("front_matter", "", 0)
+    token.hidden = True
+    token.markup = marker_chr * min_markers
+    token.content = state.src[state.bMarks[startLine + 1] : state.eMarks[nextLine - 1]]
+    token.block = True
+
+    state.parentType = old_parent
+    state.lineMax = old_line_max
+    state.line = nextLine + (1 if auto_closed else 0)
+    token.map = [startLine, state.line]
 
-    return frontMatter
+    return True
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/myst_role/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import re
+from typing import TYPE_CHECKING, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml
 from markdown_it.rules_inline import StateInline
 
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 VALID_NAME_PATTERN = re.compile(r"^\{([a-zA-Z0-9\_\-\+\:]+)\}")
 
 
-def myst_role_plugin(md: MarkdownIt):
+def myst_role_plugin(md: MarkdownIt) -> None:
     """Parse ``{role-name}`content```"""
     md.inline.ruler.before("backticks", "myst_role", myst_role)
     md.add_render_rule("myst_role", render_myst_role)
 
 
-def myst_role(state: StateInline, silent: bool):
+def myst_role(state: StateInline, silent: bool) -> bool:
     # check name
     match = VALID_NAME_PATTERN.match(state.src[state.pos :])
     if not match:
         return False
     name = match.group(1)
 
     # check for starting backslash escape
     try:
-        if state.srcCharCode[state.pos - 1] == 0x5C:  # /* \ */
+        if state.src[state.pos - 1] == "\\":
             # escaped (this could be improved in the case of edge case '\\{')
             return False
     except IndexError:
         pass
 
     # scan opening tick length
     start = pos = state.pos + match.end()
@@ -52,11 +58,17 @@
         token.content = content
 
     state.pos = pos + match.end() + 1
 
     return True
 
 
-def render_myst_role(self, tokens, idx, options, env):
+def render_myst_role(
+    self: "RendererProtocol",
+    tokens: Sequence["Token"],
+    idx: int,
+    options: "OptionsDict",
+    env: "EnvType",
+) -> str:
     token = tokens[idx]
     name = token.meta.get("name", "unknown")
     return f'<code class="myst role">{{{name}}}[{escapeHtml(token.content)}]</code>'
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/substitution.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/substitution.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 from markdown_it.rules_inline import StateInline
 
+from mdit_py_plugins.utils import is_code_block
+
 
 def substitution_plugin(
     md: MarkdownIt, start_delimiter: str = "{", end_delimiter: str = "}"
-):
+) -> None:
     """A plugin to create substitution tokens.
 
     These, token should be handled by the renderer.
 
     Example::
 
         {{ block }}
 
         a {{ inline }} b
 
     """
 
-    start_char = ord(start_delimiter)
-    end_char = ord(end_delimiter)
-
-    def _substitution_inline(state: StateInline, silent: bool):
+    def _substitution_inline(state: StateInline, silent: bool) -> bool:
         try:
             if (
-                state.srcCharCode[state.pos] != start_char
-                or state.srcCharCode[state.pos + 1] != start_char
+                state.src[state.pos] != start_delimiter
+                or state.src[state.pos + 1] != start_delimiter
             ):
                 return False
         except IndexError:
             return False
 
         pos = state.pos + 2
         found_closing = False
         while True:
             try:
-                end = state.srcCharCode.index(end_char, pos)
+                end = state.src.index(end_delimiter, pos)
             except ValueError:
                 return False
             try:
-                if state.srcCharCode[end + 1] == end_char:
+                if state.src[end + 1] == end_delimiter:
                     found_closing = True
                     break
             except IndexError:
                 return False
             pos = end + 2
 
         if not found_closing:
@@ -62,22 +61,21 @@
         token.attrSet("text", text)
         token.markup = f"{start_delimiter}{end_delimiter}"
 
         return True
 
     def _substitution_block(
         state: StateBlock, startLine: int, endLine: int, silent: bool
-    ):
+    ) -> bool:
+        if is_code_block(state, startLine):
+            return False
+
         startPos = state.bMarks[startLine] + state.tShift[startLine]
         end = state.eMarks[startLine]
 
-        # if it's indented more than 3 spaces, it should be a code block
-        if state.sCount[startLine] - state.blkIndent >= 4:
-            return False
-
         lineText = state.src[startPos:end].strip()
 
         try:
             if (
                 lineText[0] != start_delimiter
                 or lineText[1] != start_delimiter
                 or lineText[-1] != end_delimiter
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/tasklists/__init__.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,34 +11,35 @@
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+from __future__ import annotations
 
 import re
-from typing import List
 from uuid import uuid4
 
 from markdown_it import MarkdownIt
+from markdown_it.rules_core import StateCore
 from markdown_it.token import Token
 
 # Regex string to match a whitespace character, as specified in
 # https://github.github.com/gfm/#whitespace-character
 # (spec version 0.29-gfm (2019-04-06))
 _GFM_WHITESPACE_RE = r"[ \t\n\v\f\r]"
 
 
 def tasklists_plugin(
     md: MarkdownIt,
     enabled: bool = False,
     label: bool = False,
     label_after: bool = False,
-):
+) -> None:
     """Plugin for building task/todo lists out of markdown lists with items starting with [ ] or [x]
     .. Nothing else
 
     For example::
        - [ ] An item that needs doing
        - [x] An item that is complete
 
@@ -49,104 +50,102 @@
     :param label: True wraps the rendered list items in a <label> element for UX purposes,
     :param label_after: True adds the <label> element after the checkbox.
     """
     disable_checkboxes = not enabled
     use_label_wrapper = label
     use_label_after = label_after
 
-    def fcn(state):
-        tokens: List[Token] = state.tokens
+    def fcn(state: StateCore) -> None:
+        tokens = state.tokens
         for i in range(2, len(tokens) - 1):
             if is_todo_item(tokens, i):
-                todoify(tokens[i], tokens[i].__class__)
+                todoify(tokens[i])
                 tokens[i - 2].attrSet(
                     "class",
                     "task-list-item" + (" enabled" if not disable_checkboxes else ""),
                 )
                 tokens[parent_token(tokens, i - 2)].attrSet(
                     "class", "contains-task-list"
                 )
 
     md.core.ruler.after("inline", "github-tasklists", fcn)
 
-    def parent_token(tokens, index):
+    def parent_token(tokens: list[Token], index: int) -> int:
         target_level = tokens[index].level - 1
         for i in range(1, index + 1):
             if tokens[index - i].level == target_level:
                 return index - i
         return -1
 
-    def is_todo_item(tokens, index):
+    def is_todo_item(tokens: list[Token], index: int) -> bool:
         return (
             is_inline(tokens[index])
             and is_paragraph(tokens[index - 1])
             and is_list_item(tokens[index - 2])
             and starts_with_todo_markdown(tokens[index])
         )
 
-    def todoify(token: Token, token_constructor):
+    def todoify(token: Token) -> None:
         assert token.children is not None
-        token.children.insert(0, make_checkbox(token, token_constructor))
+        token.children.insert(0, make_checkbox(token))
         token.children[1].content = token.children[1].content[3:]
         token.content = token.content[3:]
 
         if use_label_wrapper:
             if use_label_after:
                 token.children.pop()
 
                 # Replaced number generator from original plugin with uuid.
                 checklist_id = f"task-item-{uuid4()}"
                 token.children[0].content = (
                     token.children[0].content[0:-1] + f' id="{checklist_id}">'
                 )
-                token.children.append(
-                    after_label(token.content, checklist_id, token_constructor)
-                )
+                token.children.append(after_label(token.content, checklist_id))
             else:
-                token.children.insert(0, begin_label(token_constructor))
-                token.children.append(end_label(token_constructor))
+                token.children.insert(0, begin_label())
+                token.children.append(end_label())
 
-    def make_checkbox(token, token_constructor):
-        checkbox = token_constructor("html_inline", "", 0)
+    def make_checkbox(token: Token) -> Token:
+        checkbox = Token("html_inline", "", 0)
         disabled_attr = 'disabled="disabled"' if disable_checkboxes else ""
         if token.content.startswith("[ ] "):
             checkbox.content = (
                 '<input class="task-list-item-checkbox" '
                 f'{disabled_attr} type="checkbox">'
             )
         elif token.content.startswith("[x] ") or token.content.startswith("[X] "):
             checkbox.content = (
                 '<input class="task-list-item-checkbox" checked="checked" '
                 f'{disabled_attr} type="checkbox">'
             )
         return checkbox
 
-    def begin_label(token_constructor):
-        token = token_constructor("html_inline", "", 0)
+    def begin_label() -> Token:
+        token = Token("html_inline", "", 0)
         token.content = "<label>"
         return token
 
-    def end_label(token_constructor):
-        token = token_constructor("html_inline", "", 0)
+    def end_label() -> Token:
+        token = Token("html_inline", "", 0)
         token.content = "</label>"
         return token
 
-    def after_label(content, checkbox_id, token_constructor):
-        token = token_constructor("html_inline", "", 0)
+    def after_label(content: str, checkbox_id: str) -> Token:
+        token = Token("html_inline", "", 0)
         token.content = (
             f'<label class="task-list-item-label" for="{checkbox_id}">{content}</label>'
         )
-        token.attrs = [{"for": checkbox_id}]
+        token.attrs = {"for": checkbox_id}
         return token
 
-    def is_inline(token):
+    def is_inline(token: Token) -> bool:
         return token.type == "inline"
 
-    def is_paragraph(token):
+    def is_paragraph(token: Token) -> bool:
         return token.type == "paragraph_open"
 
-    def is_list_item(token):
+    def is_list_item(token: Token) -> bool:
         return token.type == "list_item_open"
 
-    def starts_with_todo_markdown(token):
+    def starts_with_todo_markdown(token: Token) -> bool:
         # leading whitespace in a list item is already trimmed off by markdown-it
-        return re.match(rf"\[[ xX]]{_GFM_WHITESPACE_RE}+", token.content)
+        return re.match(rf"\[[ xX]]{_GFM_WHITESPACE_RE}+", token.content) is not None
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/LICENSE` & `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/README.md` & `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/README.md`

 * *Files identical despite different names*

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/texmath/index.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+from __future__ import annotations
+
 import re
-from typing import Optional
+from typing import TYPE_CHECKING, Any, Callable, Match, Sequence, TypedDict
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import charCodeAt
 
+if TYPE_CHECKING:
+    from markdown_it.renderer import RendererProtocol
+    from markdown_it.rules_block import StateBlock
+    from markdown_it.rules_inline import StateInline
+    from markdown_it.token import Token
+    from markdown_it.utils import EnvType, OptionsDict
+
 
-def texmath_plugin(md: MarkdownIt, delimiters="dollars", macros: Optional[dict] = None):
+def texmath_plugin(
+    md: MarkdownIt, delimiters: str = "dollars", macros: Any = None
+) -> None:
     """Plugin ported from
     `markdown-it-texmath <https://github.com/goessner/markdown-it-texmath>`__.
 
     It parses TeX math equations set inside opening and closing delimiters:
 
     .. code-block:: md
 
@@ -22,74 +33,101 @@
 
     if delimiters in rules:
         for rule_inline in rules[delimiters]["inline"]:
             md.inline.ruler.before(
                 "escape", rule_inline["name"], make_inline_func(rule_inline)
             )
 
-            def render_math_inline(self, tokens, idx, options, env):
+            def render_math_inline(
+                self: RendererProtocol,
+                tokens: Sequence[Token],
+                idx: int,
+                options: OptionsDict,
+                env: EnvType,
+            ) -> str:
                 return rule_inline["tmpl"].format(  # noqa: B023
                     render(tokens[idx].content, False, macros)
                 )
 
             md.add_render_rule(rule_inline["name"], render_math_inline)
 
         for rule_block in rules[delimiters]["block"]:
             md.block.ruler.before(
                 "fence", rule_block["name"], make_block_func(rule_block)
             )
 
-            def render_math_block(self, tokens, idx, options, env):
+            def render_math_block(
+                self: RendererProtocol,
+                tokens: Sequence[Token],
+                idx: int,
+                options: OptionsDict,
+                env: EnvType,
+            ) -> str:
                 return rule_block["tmpl"].format(  # noqa: B023
                     render(tokens[idx].content, True, macros), tokens[idx].info
                 )
 
             md.add_render_rule(rule_block["name"], render_math_block)
 
 
-def applyRule(rule, string: str, begin, inBlockquote):
+class _RuleDictReqType(TypedDict):
+    name: str
+    rex: re.Pattern[str]
+    tmpl: str
+    tag: str
+
+
+class RuleDictType(_RuleDictReqType, total=False):
+    # Note in Python 3.10+ could use Req annotation
+    pre: Any
+    post: Any
+
+
+def applyRule(
+    rule: RuleDictType, string: str, begin: int, inBlockquote: bool
+) -> None | Match[str]:
     if not (
         string.startswith(rule["tag"], begin)
         and (rule["pre"](string, begin) if "pre" in rule else True)
     ):
-        return False
+        return None
 
-    match = rule["rex"].match(string[begin:])  # type: re.Match
+    match = rule["rex"].match(string[begin:])
 
     if not match or match.start() != 0:
-        return False
+        return None
 
     lastIndex = match.end() + begin - 1
     if "post" in rule and not (
         rule["post"](string, lastIndex)  # valid post-condition
         # remove evil blockquote bug (https:#github.com/goessner/mdmath/issues/50)
         and (not inBlockquote or "\n" not in match.group(1))
     ):
-        return False
+        return None
     return match
 
 
-def make_inline_func(rule):
-    def _func(state, silent):
+def make_inline_func(rule: RuleDictType) -> Callable[[StateInline, bool], bool]:
+    def _func(state: StateInline, silent: bool) -> bool:
         res = applyRule(rule, state.src, state.pos, False)
         if res:
             if not silent:
                 token = state.push(rule["name"], "math", 0)
                 token.content = res[1]  # group 1 from regex ..
                 token.markup = rule["tag"]
 
             state.pos += res.end()
 
         return bool(res)
 
     return _func
 
 
-def make_block_func(rule):
-    def _func(state, begLine, endLine, silent):
+def make_block_func(rule: RuleDictType) -> Callable[[StateBlock, int, int, bool], bool]:
+    def _func(state: StateBlock, begLine: int, endLine: int, silent: bool) -> bool:
         begin = state.bMarks[begLine] + state.tShift[begLine]
         res = applyRule(rule, state.src, begin, state.parentType == "blockquote")
         if res:
             if not silent:
                 token = state.push(rule["name"], "math", 0)
                 token.block = True
                 token.content = res[1]
@@ -102,39 +140,37 @@
             while line < endLine:
                 if endpos >= state.bMarks[line] and endpos <= state.eMarks[line]:
                     # line for end of block math found ...
                     state.line = line + 1
                     break
                 line += 1
 
-            state.pos = begin + res.end()
-
         return bool(res)
 
     return _func
 
 
-def dollar_pre(str, beg):
-    prv = charCodeAt(str[beg - 1], 0) if beg > 0 else False
+def dollar_pre(src: str, beg: int) -> bool:
+    prv = charCodeAt(src[beg - 1], 0) if beg > 0 else False
     return (
         (not prv) or prv != 0x5C and (prv < 0x30 or prv > 0x39)  # no backslash,
     )  # no decimal digit .. before opening '$'
 
 
-def dollar_post(string, end):
+def dollar_post(src: str, end: int) -> bool:
     try:
-        nxt = string[end + 1] and charCodeAt(string[end + 1], 0)
+        nxt = src[end + 1] and charCodeAt(src[end + 1], 0)
     except IndexError:
         return True
     return (
         (not nxt) or (nxt < 0x30) or (nxt > 0x39)
     )  # no decimal digit .. after closing '$'
 
 
-def render(tex, displayMode, macros):
+def render(tex: str, displayMode: bool, macros: Any) -> str:
     return tex
     # TODO better HTML renderer port for math
     # try:
     #     res = katex.renderToString(tex,{throwOnError:False,displayMode,macros})
     # except:
     #     res = tex+": "+err.message.replace("<","&lt;")
     # return res
@@ -145,15 +181,16 @@
 #     return texmath;
 # }
 
 
 # All regexes areg global (g) and sticky (y), see:
 # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/sticky
 
-rules: dict = {
+
+rules: dict[str, dict[str, list[RuleDictType]]] = {
     "brackets": {
         "inline": [
             {
                 "name": "math_inline",
                 "rex": re.compile(r"^\\\((.+?)\\\)", re.DOTALL),
                 "tmpl": "<eq>{0}</eq>",
                 "tag": "\\(",
```

### Comparing `mdit-py-plugins-0.3.5/mdit_py_plugins/wordcount/__init__.py` & `mdit_py_plugins-0.4.0/mdit_py_plugins/wordcount/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def wordcount_plugin(
     md: MarkdownIt,
     *,
     per_minute: int = 200,
     count_func: Callable[[str], int] = basic_count,
     store_text: bool = False,
-):
+) -> None:
     """Plugin for computing and storing the word count.
 
     Stores in the ``env`` e.g.::
 
         env["wordcount"] = {
           "words": 200
           "minutes": 1,
```

### Comparing `mdit-py-plugins-0.3.5/pyproject.toml` & `mdit_py_plugins-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 authors = [{name = "Chris Sewell", email = "chrisj_sewell@hotmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
 ]
 keywords = ["markdown", "markdown-it", "lexer", "parser", "development"]
-requires-python = ">=3.7"
-dependencies = ["markdown-it-py>=1.0.0,<3.0.0"]
+requires-python = ">=3.8"
+dependencies = ["markdown-it-py>=1.0.0,<4.0.0"]
 
 [project.urls]
 Homepage = "https://github.com/executablebooks/mdit-py-plugins"
 Documentation = "https://mdit-py-plugins.readthedocs.io"
 
 [project.optional-dependencies]
 code_style = ["pre-commit"]
 testing = [
     "coverage",
     "pytest",
     "pytest-cov",
     "pytest-regressions",
 ]
 rtd = [
-    "attrs",
-    "myst-parser~=0.16.1",
-    "sphinx-book-theme~=0.1.0",
+    "myst-parser",
+    "sphinx-book-theme",
 ]
 
 [tool.flit.module]
 name = "mdit_py_plugins"
 
 [tool.flit.sdist]
 exclude = [
@@ -64,9 +63,8 @@
 extend-select = ["B0", "C4", "ICN", "ISC", "N", "RUF", "SIM"]
 extend-ignore = ["E731", "N802", "N803", "N806"]
 
 [tool.mypy]
 show_error_codes = true
 warn_unused_ignores = true
 warn_redundant_casts = true
-no_implicit_optional = true
-strict_equality = true
+strict = true
```

### Comparing `mdit-py-plugins-0.3.5/tox.ini` & `mdit_py_plugins-0.4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # To use tox, see https://tox.readthedocs.io
 # Simply pip or conda install tox
 # If you use conda, you may also want to install tox-conda
 # then run `tox` or `tox -- {pytest args}`
 # run in parallel using `tox -p`
 [tox]
-envlist = py37
+envlist = py38
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310}]
+[testenv:py{37,38,39,310,311}]
 extras = testing
 commands = pytest {posargs}
 
 [testenv:docs-{update,clean}]
 extras = rtd
 whitelist_externals = rm
 commands =
```

### Comparing `mdit-py-plugins-0.3.5/PKG-INFO` & `mdit_py_plugins-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: mdit-py-plugins
-Version: 0.3.5
+Version: 0.4.0
 Summary: Collection of plugins for markdown-it-py
 Keywords: markdown,markdown-it,lexer,parser,development
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
-Requires-Dist: markdown-it-py>=1.0.0,<3.0.0
+Requires-Dist: markdown-it-py>=1.0.0,<4.0.0
 Requires-Dist: pre-commit ; extra == "code_style"
-Requires-Dist: attrs ; extra == "rtd"
-Requires-Dist: myst-parser~=0.16.1 ; extra == "rtd"
-Requires-Dist: sphinx-book-theme~=0.1.0 ; extra == "rtd"
+Requires-Dist: myst-parser ; extra == "rtd"
+Requires-Dist: sphinx-book-theme ; extra == "rtd"
 Requires-Dist: coverage ; extra == "testing"
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
 Project-URL: Documentation, https://mdit-py-plugins.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/mdit-py-plugins
 Provides-Extra: code_style
```

