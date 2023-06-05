# Comparing `tmp/configzen-0.2.3.tar.gz` & `tmp/configzen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.3.tar", max compression
+gzip compressed data, was "configzen-0.2.4.tar", max compression
```

## Comparing `configzen-0.2.3.tar` & `configzen-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.3/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.3/configzen/__main__.py
--rw-r--r--   0        0        0    67072 2023-06-05 06:56:38.878732 configzen-0.2.3/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.3/configzen/errors.py
--rw-r--r--   0        0        0    30567 2023-06-05 06:53:19.290433 configzen-0.2.3/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.3/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.3/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.3/LICENSE
--rw-r--r--   0        0        0     1154 2023-06-05 06:58:57.556277 configzen-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.3/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.4/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.4/configzen/__main__.py
+-rw-r--r--   0        0        0    68063 2023-06-05 07:06:03.591411 configzen-0.2.4/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.4/configzen/errors.py
+-rw-r--r--   0        0        0    30567 2023-06-05 06:53:19.290433 configzen-0.2.4/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.4/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.4/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1154 2023-06-05 07:06:36.501662 configzen-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.4/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.4/PKG-INFO
```

### Comparing `configzen-0.2.3/configzen/__main__.py` & `configzen-0.2.4/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/configzen/config.py` & `configzen-0.2.4/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,49 @@
         The loaded configuration.
         """
         dict_config = self.load_into_dict(blob, ac_parser=ac_parser, **kwargs)
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
-    def _preload_into_dict(
+    async def async_load_into(
+        self,
+        config_class: type[ConfigModelT],
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration into a `ConfigModel` subclass asynchronously.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        dict_config = await self.load_into_dict_async(
+            blob,
+            ac_parser=ac_parser,
+            **kwargs
+        )
+        if dict_config is None:
+            dict_config = {}
+        return config_class.parse_obj(dict_config)
+
+    def _load_into_dict_impl(
         self,
         blob: str,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
         if ac_parser is None:
             ac_parser = self.ac_parser
@@ -726,15 +760,15 @@
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        loaded = self._preload_into_dict(blob, ac_parser, **kwargs)
+        loaded = self._load_into_dict_impl(blob, ac_parser, **kwargs)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
         return loaded
 
     async def load_into_dict_async(
         self,
         blob: str,
@@ -756,15 +790,15 @@
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        loaded = self._preload_into_dict(blob, ac_parser, **kwargs)
+        loaded = self._load_into_dict_impl(blob, ac_parser, **kwargs)
         if preprocess:
             loaded = await self.processor_class(self, loaded).preprocess_async()
         return loaded
 
     def dump_config(
         self,
         config: ConfigModelT,
@@ -1066,15 +1100,15 @@
             async with self.open_resource_async(**kwargs) as fp:
                 blob = await fp.read()
         except FileNotFoundError:
             if self.create_if_missing:
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 await self.write_async(blob, **(create_kwargs or {}))
-        return self.load_into(config_class, blob, **self.load_options)
+        return await self.async_load_into(config_class, blob, **self.load_options)
 
     async def write_async(
         self,
         blob: str,
         **kwargs: Any,
     ) -> int:
         """
```

### Comparing `configzen-0.2.3/configzen/errors.py` & `configzen-0.2.4/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/configzen/processor.py` & `configzen-0.2.4/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/configzen/typedefs.py` & `configzen-0.2.4/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/LICENSE` & `configzen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/pyproject.toml` & `configzen-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.3"
+version = "0.2.4"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.3/README.md` & `configzen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.3/PKG-INFO` & `configzen-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.3
+Version: 0.2.4
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

