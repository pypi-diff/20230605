# Comparing `tmp/lana-0.1.6.tar.gz` & `tmp/lana-0.1.7.tar.gz`

## Comparing `lana-0.1.6.tar` & `lana-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 lana-0.1.6/Cargo.toml
--rw-r--r--   0      501       20      726 2023-05-31 13:58:49.000000 lana-0.1.6/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.6/LICENSE
--rw-r--r--   0      501       20      640 2023-05-30 15:23:21.000000 lana-0.1.6/README.md
--rw-r--r--   0      501       20      475 2023-05-30 15:56:16.000000 lana-0.1.6/examples/competition.py
--rw-r--r--   0      501       20     5243 2023-05-31 15:01:48.000000 lana-0.1.6/examples/example.ipynb
--rw-r--r--   0      501       20      509 2023-05-31 16:27:08.000000 lana-0.1.6/lana/__init__.py
--rw-r--r--   0      501       20      651 2023-05-30 15:32:41.000000 lana-0.1.6/pyproject.toml
--rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.6/src/lib.rs
--rw-r--r--   0      501       20     5173 2023-05-31 16:19:08.000000 lana-0.1.6/src/matrix.rs
--rw-r--r--   0      501       20      885 2023-05-30 13:33:31.000000 lana-0.1.6/test/test_matrix.py
--rw-r--r--   0      501       20     9870 2023-05-31 13:57:32.000000 lana-0.1.6/Cargo.lock
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lana-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 lana-0.1.7/Cargo.toml
+-rw-r--r--   0      501       20      726 2023-05-31 13:58:49.000000 lana-0.1.7/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.7/LICENSE
+-rw-r--r--   0      501       20      668 2023-06-05 09:03:25.000000 lana-0.1.7/README.md
+-rw-r--r--   0      501       20      475 2023-05-30 15:56:16.000000 lana-0.1.7/examples/competition.py
+-rw-r--r--   0      501       20     5447 2023-05-31 16:32:18.000000 lana-0.1.7/examples/example.ipynb
+-rw-r--r--   0      501       20     1088 2023-06-05 09:10:03.000000 lana-0.1.7/lana/__init__.py
+-rw-r--r--   0      501       20      651 2023-05-30 15:32:41.000000 lana-0.1.7/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.7/src/lib.rs
+-rw-r--r--   0      501       20     5173 2023-05-31 16:19:08.000000 lana-0.1.7/src/matrix.rs
+-rw-r--r--   0      501       20      885 2023-05-30 13:33:31.000000 lana-0.1.7/test/test_matrix.py
+-rw-r--r--   0      501       20     9870 2023-06-05 09:45:53.000000 lana-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 lana-0.1.7/PKG-INFO
```

### Comparing `lana-0.1.6/.gitignore` & `lana-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.1.6/LICENSE` & `lana-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.6/README.md` & `lana-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Lana 🧶
 
 [![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
 
-**L***inear* **a***lgebra* *for* **n***octurnal and* **a***dventurous data scientists.*
+**L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists.*
 
 ## Install 
 
 ```console
 pip install lana
 ```
 
@@ -14,16 +14,16 @@
 
 ```python
 from lana import Matrix
 
 zeros = Matrix.zeros((3,3))
 print(zeros)
 print(f"shape: {zeros.shape}, type: {type(zeros)}")
-print(zeros[0], zeros[0][0])
+print(zeros.to_list()[0], zeros.to_list()[0][0])
 
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
-for rows in mat:
+for rows in mat.to_list():
     print(rows, type(rows))
 ```
```

### Comparing `lana-0.1.6/examples/example.ipynb` & `lana-0.1.7/examples/example.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859068627450981%*

 * *Differences: {"'cells'": "{1: {'source': ['from lana import Matrix, inject']}, 4: {'execution_count': 3}, 6: "*

 * *            "{'outputs': {0: {'text': ['Matrix([[0, 0, 0],\\n', '       [0, 0, 0]])\\n']}}, "*

 * *            "'source': ['c = Matrix.matrix(inject(zeros.to_list()[0:2]))\\n', 'print(c)']}, 8: "*

 * *            "{'execution_count': 10}, 10: {'execution_count': 11}, 12: {'execution_count': 12}, "*

 * *            "14: {'execution_count': 13}, 15: {'execution_count': 14}, 16: {'execution_count': "*

 * *            "15}, insert: [( […]*

```diff
@@ -10,15 +10,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lana import Matrix"
+                "from lana import Matrix, inject"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -47,15 +47,15 @@
                 "print(zeros)\n",
                 "print(f\"type: {type(zeros)}\")\n",
                 "print(f\"shape: {zeros.shape}\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[0.0, 0.0, 0.0] <class 'list'>\n",
@@ -67,43 +67,61 @@
             "source": [
                 "for row in zeros.to_list():\n",
                 "    print(row, type(row))"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Matrix([[0]])\n"
+                    ]
+                }
+            ],
+            "source": [
+                "## sub-matrix\n",
+                "b = Matrix.matrix(inject(zeros.to_list()[0:2][0][0]))\n",
+                "print(b)"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[0.0, 0.0, 0.0] <class 'list'> 0.0 <class 'float'>\n",
-                        "[0.0, 0.0, 0.0] <class 'list'> 0.0 <class 'float'>\n",
-                        "[0.0, 0.0, 0.0] <class 'list'> 0.0 <class 'float'>\n"
+                        "Matrix([[0, 0, 0],\n",
+                        "       [0, 0, 0]])\n"
                     ]
                 }
             ],
             "source": [
-                "for row in zeros:\n",
-                "    print(row, type(row), row[0], type(row[0]))"
+                "c = Matrix.matrix(inject(zeros.to_list()[0:2]))\n",
+                "print(c)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Eye"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[1, 0, 0],\n",
@@ -127,15 +145,15 @@
             "metadata": {},
             "source": [
                 "### Ones"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[1, 1, 1],\n",
@@ -159,15 +177,15 @@
             "metadata": {},
             "source": [
                 "### Matrix"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[1, 2, 3],\n",
@@ -191,15 +209,15 @@
             "metadata": {},
             "source": [
                 "### Operations"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[3, 3, 3],\n",
@@ -212,15 +230,15 @@
                 "b = Matrix.matrix([[2,2,2],[2,2,2]])\n",
                 "c = a + b\n",
                 "print(c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[2, 2, 2],\n",
@@ -231,15 +249,15 @@
             "source": [
                 "d = c - a\n",
                 "print(d)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix([[-2, -2, -2],\n",
```

### Comparing `lana-0.1.6/pyproject.toml` & `lana-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.1.6/src/matrix.rs` & `lana-0.1.7/src/matrix.rs`

 * *Files identical despite different names*

### Comparing `lana-0.1.6/test/test_matrix.py` & `lana-0.1.7/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `lana-0.1.6/Cargo.lock` & `lana-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "pyo3",
  "rayon",
 ]
 
 [[package]]
 name = "libc"
```

### Comparing `lana-0.1.6/PKG-INFO` & `lana-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Experimental Linear Algebra library written in Rust
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/marcosalvalaggio/lana
 
 ## Lana 🧶
 
 [![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
 
-**L***inear* **a***lgebra* *for* **n***octurnal and* **a***dventurous data scientists.*
+**L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists.*
 
 ## Install 
 
 ```console
 pip install lana
 ```
 
@@ -28,17 +28,17 @@
 
 ```python
 from lana import Matrix
 
 zeros = Matrix.zeros((3,3))
 print(zeros)
 print(f"shape: {zeros.shape}, type: {type(zeros)}")
-print(zeros[0], zeros[0][0])
+print(zeros.to_list()[0], zeros.to_list()[0][0])
 
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
-for rows in mat:
+for rows in mat.to_list():
     print(rows, type(rows))
 ```
```

