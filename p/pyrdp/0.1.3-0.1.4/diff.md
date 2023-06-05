# Comparing `tmp/pyrdp-0.1.3.tar.gz` & `tmp/pyrdp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdp-0.1.3.tar", last modified: Sun Apr 30 10:23:58 2023, max compression
+gzip compressed data, was "pyrdp-0.1.4.tar", last modified: Mon Jun  5 12:16:22 2023, max compression
```

## Comparing `pyrdp-0.1.3.tar` & `pyrdp-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-04-30 09:47:21.216851 pyrdp-0.1.3/LICENSE
--rw-r--r--   0        0        0      445 2023-04-30 10:22:49.318096 pyrdp-0.1.3/README.md
--rw-r--r--   0        0        0      455 2023-04-30 10:23:58.374588 pyrdp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2234 2023-04-30 10:13:28.330084 pyrdp-0.1.3/pyrdp/__init__.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pyrdp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 09:47:21.216851 pyrdp-0.1.4/LICENSE
+-rw-r--r--   0        0        0      445 2023-04-30 10:22:49.318096 pyrdp-0.1.4/README.md
+-rw-r--r--   0        0        0      455 2023-06-05 12:16:22.980137 pyrdp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2210 2023-06-05 12:13:11.510555 pyrdp-0.1.4/pyrdp/__init__.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pyrdp-0.1.4/PKG-INFO
```

### Comparing `pyrdp-0.1.3/LICENSE` & `pyrdp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdp-0.1.3/pyrdp/__init__.py` & `pyrdp-0.1.4/pyrdp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,19 @@
             stack.append([start_index, index_max])
             stack.append([index_max, last_index])
         else:
             indices[start_index + 1 : last_index] = False
     return points[indices]
 
 
-def rdp(points: npt.ArrayLike, epsilon: float) -> npt.ArrayLike:
+def rdp(points: npt.ArrayLike, epsilon: float) -> npt.NDArray[np.float_]:
     """Simplifies a list or an array of points using the Ramer-Douglas-Peucker
     algorithm.
 
     :param points: Array of points (Nx2)
     :param epsilon: epsilon in the rdp algorithm
 
     :return: Simplified list of points.
     """
     if not isinstance(points, np.ndarray):
-        result = _rdp(np.array(points), epsilon).tolist()
-        return result
+        return _rdp(np.array(points), epsilon)
     return _rdp(points, epsilon)
```

### Comparing `pyrdp-0.1.3/PKG-INFO` & `pyrdp-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrdp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple Rammer-Douglas-Peuker algorithm implementation.
 Author-Email: Florian Stasse <f.stasse@skipperndt.com>
 License: MIT
 Requires-Python: >=3.8
-Requires-Dist: numpy~=1.23.4
+Requires-Dist: numpy>=1.24.3
 Description-Content-Type: text/markdown
 
 # Ramer-Douglas-Peucker
 
 Ramer-Douglas-Peucker python implementation.
 
 ## Installation
```

