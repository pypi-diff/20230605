# Comparing `tmp/ols_py-0.2.7.tar.gz` & `tmp/ols_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ols_py-0.2.7.tar", max compression
+gzip compressed data, was "ols_py-0.3.0.tar", max compression
```

## Comparing `ols_py-0.2.7.tar` & `ols_py-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     3406 2023-05-25 01:48:00.900427 ols_py-0.2.7/README.md
--rw-r--r--   0        0        0     2167 2023-05-25 01:48:00.900427 ols_py-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       55 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/__init__.py
--rw-r--r--   0        0        0    10705 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/client.py
--rw-r--r--   0        0        0     1596 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/instances.py
--rw-r--r--   0        0        0        0 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/py.typed
--rw-r--r--   0        0        0       89 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/__init__.py
--rw-r--r--   0        0        0      408 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/common.py
--rw-r--r--   0        0        0     4219 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/requests.py
--rw-r--r--   0        0        0     3752 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/responses.py
--rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 ols_py-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3549 2023-06-05 03:08:16.163353 ols_py-0.3.0/README.md
+-rw-r--r--   0        0        0     2286 2023-06-05 03:08:16.167353 ols_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/__init__.py
+-rw-r--r--   0        0        0    10705 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/client.py
+-rw-r--r--   0        0        0     1641 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/instances.py
+-rw-r--r--   0        0        0     2975 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_client.py
+-rw-r--r--   0        0        0       49 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_schemas/__init__.py
+-rw-r--r--   0        0        0     1118 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_schemas/responses.py
+-rw-r--r--   0        0        0        0 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/py.typed
+-rw-r--r--   0        0        0       89 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/__init__.py
+-rw-r--r--   0        0        0      408 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/common.py
+-rw-r--r--   0        0        0     4219 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/requests.py
+-rw-r--r--   0        0        0     3752 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/responses.py
+-rw-r--r--   0        0        0     4556 1970-01-01 00:00:00.000000 ols_py-0.3.0/PKG-INFO
```

### Comparing `ols_py-0.2.7/README.md` & `ols_py-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 
 **PyPI**: [https://pypi.org/project/ols-py/](https://pypi.org/project/ols-py/)
 
 ---
 
 Python client for the Ontology Lookup Service
 
-**Current status:** in development, some endpoints and schemas are not
-implemented yet.
+**Current status:**
+
+* In development, some endpoints and schemas are not implemented yet.
+* Experimental support for OLS4 instances (using the existing API) - `Ols4Client` has been tweaked
+  to match changes to the API/responses.
 
 Features:
 
 * Type annotated so you know which parameters can be used for each endpoint
 * Responses validated and parsed with [pydantic](https://github.com/pydantic/pydantic) for
   easy access to response data
```

### Comparing `ols_py-0.2.7/pyproject.toml` & `ols_py-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ols-py"
-version = "0.2.7"
+version = "0.3.0"
 description = "Python client for the Ontology Lookup Service"
 authors = [
     "Marius Mather <marius.mather@sydney.edu.au>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -28,15 +28,21 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10.1, <4.0"
 requests = ">=2.0, <3.0"
 pydantic = "^1.10.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.jupyterlab]
+optional = true
+
+[tool.poetry.group.jupyterlab.dependencies]
+jupyterlab = "^3.6"
+
+[tool.poetry.group.dev.dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-builtins = "*"
 flake8-comprehensions = "*"
 flake8-debugger = "*"
```

### Comparing `ols_py-0.2.7/src/ols_py/client.py` & `ols_py-0.3.0/src/ols_py/client.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.7/src/ols_py/instances.py` & `ols_py-0.3.0/src/ols_py/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,14 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 EBI = "https://www.ebi.ac.uk/ols/api/"
+EBI_OLS4 = "https://www.ebi.ac.uk/ols4/api/"
 TIB = "https://service.tib.eu/ts4tib/api/"
 NFDI4I = "https://service.tib.eu/ts4ing/api/"
 NFDI4Chem = "https://terminology.nfdi4chem.de/ts/api/"
 ZBMed = "https://semanticlookup.zbmed.de/ols/api/"
 Monarch = "https://ols.monarchinitiative.org/api/"
 Fraunhofer = "https://rohan.scai.fraunhofer.de/api/"
```

### Comparing `ols_py-0.2.7/src/ols_py/schemas/requests.py` & `ols_py-0.3.0/src/ols_py/schemas/requests.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.7/src/ols_py/schemas/responses.py` & `ols_py-0.3.0/src/ols_py/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.7/PKG-INFO` & `ols_py-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ols-py
-Version: 0.2.7
+Version: 0.3.0
 Summary: Python client for the Ontology Lookup Service
 Home-page: https://ahida-development.github.io/ols-py
 License: MIT
 Author: Marius Mather
 Author-email: marius.mather@sydney.edu.au
 Requires-Python: >=3.10.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -42,16 +42,19 @@
 
 **PyPI**: [https://pypi.org/project/ols-py/](https://pypi.org/project/ols-py/)
 
 ---
 
 Python client for the Ontology Lookup Service
 
-**Current status:** in development, some endpoints and schemas are not
-implemented yet.
+**Current status:**
+
+* In development, some endpoints and schemas are not implemented yet.
+* Experimental support for OLS4 instances (using the existing API) - `Ols4Client` has been tweaked
+  to match changes to the API/responses.
 
 Features:
 
 * Type annotated so you know which parameters can be used for each endpoint
 * Responses validated and parsed with [pydantic](https://github.com/pydantic/pydantic) for
   easy access to response data
```

