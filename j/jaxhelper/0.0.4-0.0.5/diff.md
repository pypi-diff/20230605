# Comparing `tmp/jaxhelper-0.0.4.tar.gz` & `tmp/jaxhelper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxhelper-0.0.4.tar", last modified: Mon Jun  5 13:39:02 2023, max compression
+gzip compressed data, was "jaxhelper-0.0.5.tar", last modified: Mon Jun  5 14:03:51 2023, max compression
```

## Comparing `jaxhelper-0.0.4.tar` & `jaxhelper-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.4/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/jaxhelper/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     5200 2023-06-05 13:38:42.000000 jaxhelper-0.0.4/jaxhelper/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/jaxhelper.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:39:02.000000 jaxhelper-0.0.4/jaxhelper.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:39:02.321727 jaxhelper-0.0.4/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:38:48.000000 jaxhelper-0.0.4/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 14:03:51.581464 jaxhelper-0.0.5/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 14:03:51.581464 jaxhelper-0.0.5/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.5/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 14:03:51.581464 jaxhelper-0.0.5/jaxhelper/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5197 2023-06-05 14:03:40.000000 jaxhelper-0.0.5/jaxhelper/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 14:03:51.581464 jaxhelper-0.0.5/jaxhelper.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 14:03:51.000000 jaxhelper-0.0.5/jaxhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 14:03:51.000000 jaxhelper-0.0.5/jaxhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 14:03:51.000000 jaxhelper-0.0.5/jaxhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 14:03:51.000000 jaxhelper-0.0.5/jaxhelper.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 14:03:51.581464 jaxhelper-0.0.5/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 14:03:40.000000 jaxhelper-0.0.5/setup.py
```

### Comparing `jaxhelper-0.0.4/PKG-INFO` & `jaxhelper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.4/README.md` & `jaxhelper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jaxhelper-0.0.4/jaxhelper/__init__.py` & `jaxhelper-0.0.5/jaxhelper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
               dot_fn: Callable = multi_dot):
     ctx_dims = f'{"b" * (context.ndim > 2)}zhf'
 
     @remat
     def _fn(h, c, qk, kk, vk, pk, pb):
 
         q, k, v = [x.reshape(*x.shape[:-1], heads, -1).astype(jnp.bfloat16)  #
-                   for x in multi_dot((h, qk), (c, vk), (c, kk))]
+                   for x in dot_fn((h, qk), (c, vk), (c, kk))]
 
         def _attn(carry: jax.Array, idx: jax.Array) -> Tuple[jax.Array, None]:
             lq = lax.dynamic_slice_in_dim(q, idx * chunk, chunk, q.ndim - 3)
             tmp = jnp.einsum(f"bhsz,{ctx_dims}->bshf", softmax(lq, k, ctx_dims, scale), v, precision="fastest")
             carry = lax.dynamic_update_slice_in_dim(carry, tmp, idx * chunk, 1)
             return carry, None
```

### Comparing `jaxhelper-0.0.4/jaxhelper.egg-info/PKG-INFO` & `jaxhelper-0.0.5/jaxhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.4/setup.py` & `jaxhelper-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.jaxhelper@nestler.sh",
     name='jaxhelper',
     license='BSD',
     description='Basic tools and helpers for Jax',
-    version='0.0.4',
+    version='0.0.5',
     long_description=README,
     url='https://github.com/clashluke/jaxhelper',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

