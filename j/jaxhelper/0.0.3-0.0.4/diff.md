# Comparing `tmp/jaxhelper-0.0.3.tar.gz` & `tmp/jaxhelper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxhelper-0.0.3.tar", last modified: Mon Jun  5 13:32:38 2023, max compression
+gzip compressed data, was "jaxhelper-0.0.4.tar", last modified: Mon Jun  5 13:39:02 2023, max compression
```

## Comparing `jaxhelper-0.0.3.tar` & `jaxhelper-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.3/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/jaxhelper/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     5060 2023-06-05 13:32:21.000000 jaxhelper-0.0.3/jaxhelper/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/jaxhelper.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:32:27.000000 jaxhelper-0.0.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.4/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/jaxhelper/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5200 2023-06-05 13:38:42.000000 jaxhelper-0.0.4/jaxhelper/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/jaxhelper.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:38:48.000000 jaxhelper-0.0.4/setup.py
```

### Comparing `jaxhelper-0.0.3/PKG-INFO` & `jaxhelper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.3/README.md` & `jaxhelper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jaxhelper-0.0.3/jaxhelper/__init__.py` & `jaxhelper-0.0.4/jaxhelper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,33 +93,36 @@
     return jnp.where(jnp.isfinite(x), x, default)  # True, False | x in (NaN, Inf, -Inf)
 
 
 def dot(x, w):
     return lax.dot_general(x, w, (((x.ndim - 1,), (0,)), ((), ())), precision="fastest")
 
 
-@jax.custom_gradient
 def softmax(q: jax.Array, k: jax.Array, ctx_dims: str, scale: float) -> jax.Array:
-    lgt = jnp.einsum(f"bshf,{ctx_dims}->bhsz", q, k, precision="fastest")
-    lgt = lgt.astype(jnp.float32)
-    lgt *= scale
-    lgt = jnp.exp(lgt - lgt.max(-1, keepdims=True))
-    lgt /= lgt.sum(-1, keepdims=True)
-    lgt = lgt.astype(q.dtype)
-
-    def _grad(dy):
-        inner_lgt = lgt.astype(jnp.float32)
-        prod = inner_lgt * dy.astype(jnp.float32)
-        dlgt = prod - prod.sum(-1, keepdims=True) * inner_lgt
-        dlgt *= scale
-        dlgt = dlgt.astype(q.dtype)
-        return (jnp.einsum(f"bhsz,{ctx_dims}->bshf", dlgt, k, precision="fastest"),
-                jnp.einsum(f"bhsz,bshf->{ctx_dims}", dlgt, q, precision="fastest"))
+    @jax.custom_gradient
+    def _fn(q: jax.Array, k: jax.Array) -> jax.Array:
+        lgt = jnp.einsum(f"bshf,{ctx_dims}->bhsz", q, k, precision="fastest")
+        lgt = lgt.astype(jnp.float32)
+        lgt *= scale
+        lgt = jnp.exp(lgt - lgt.max(-1, keepdims=True))
+        lgt /= lgt.sum(-1, keepdims=True)
+        lgt = lgt.astype(q.dtype)
+
+        def _grad(dy):
+            inner_lgt = lgt.astype(jnp.float32)
+            prod = inner_lgt * dy.astype(jnp.float32)
+            dlgt = prod - prod.sum(-1, keepdims=True) * inner_lgt
+            dlgt *= scale
+            dlgt = dlgt.astype(q.dtype)
+            return (jnp.einsum(f"bhsz,{ctx_dims}->bshf", dlgt, k, precision="fastest"),
+                    jnp.einsum(f"bhsz,bshf->{ctx_dims}", dlgt, q, precision="fastest"))
 
-    return lgt, _grad
+        return lgt, _grad
+
+    return _fn(q, k)
 
 
 def to_host(k, index_fn: Callable[[jax.Array], jax.Array] = index(0)):
     return jax.device_get(map_fn(index_fn)(k))
 
 
 @map_fn
```

### Comparing `jaxhelper-0.0.3/jaxhelper.egg-info/PKG-INFO` & `jaxhelper-0.0.4/jaxhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.3/setup.py` & `jaxhelper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.jaxhelper@nestler.sh",
     name='jaxhelper',
     license='BSD',
     description='Basic tools and helpers for Jax',
-    version='0.0.3',
+    version='0.0.4',
     long_description=README,
     url='https://github.com/clashluke/jaxhelper',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

