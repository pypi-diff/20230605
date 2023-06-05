# Comparing `tmp/meilisearch_tui-0.7.2.tar.gz` & `tmp/meilisearch_tui-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.7.2.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.7.3.tar", max compression
```

## Comparing `meilisearch_tui-0.7.2.tar` & `meilisearch_tui-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-05-11 20:23:04.069288 meilisearch_tui-0.7.2/LICENSE
--rw-r--r--   0        0        0     2045 2023-05-11 20:23:04.069288 meilisearch_tui-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0      115 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     2776 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/main.py
--rw-r--r--   0        0        0     1908 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4548 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    29130 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     6273 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     2083 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-05 11:41:47.115452 meilisearch_tui-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2045 2023-06-05 11:41:47.115452 meilisearch_tui-0.7.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     2776 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/main.py
+-rw-r--r--   0        0        0     1908 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4518 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    28829 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     6228 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     2099 2023-06-05 11:41:47.119452 meilisearch_tui-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.3/PKG-INFO
```

### Comparing `meilisearch_tui-0.7.2/LICENSE` & `meilisearch_tui-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/README.md` & `meilisearch_tui-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/client.py` & `meilisearch_tui-0.7.3/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/config.py` & `meilisearch_tui-0.7.3/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/main.py` & `meilisearch_tui-0.7.3/meilisearch_tui/main.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.7.3/meilisearch_tui/meilisearch.css`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.7.3/meilisearch_tui/screens/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
                 config.theme = Theme.LIGHT
 
             if not config.meilisearch_url:
                 self.query_one("#server-url-error", Static).visible = True
             else:
                 try:
                     config.save()
-                    asyncio.create_task(self._success_message())
+                    await self._success_message()
                 except Exception as e:
-                    asyncio.create_task(self._error_message(f"{e}"))
+                    await self._error_message(f"{e}")
 
     def on_key(self, event: events.Key) -> None:
         if event.key == "enter":
             self.query_one("#save-setting-button", Button).press()
 
     def on_screen_resume(self, event: events.ScreenResume) -> None:
         self.query_one("#save-successful").visible = False
```

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.7.3/meilisearch_tui/screens/indexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,19 +115,19 @@
                 self.index_name_error.visible = True
                 return None
 
             try:
                 async with get_client() as client:
                     await client.create_index(self.index_name.value, self.primary_key.value)
                 self.added_index = self.index_name.value
-                asyncio.create_task(self._success_message())
+                await self._success_message()
             except MeilisearchError as e:
-                asyncio.create_task(self._error_message(f"{e}"))
+                await self._error_message(f"{e}")
             except Exception as e:
-                asyncio.create_task(self._error_message(f"An unknown error occured error: {e}"))
+                await self._error_message(f"An unknown error occured error: {e}")
 
         self.index_name.value = ""
         self.primary_key.value = ""
         self.index_name.focus()
 
     def watch_added_index(self) -> None:
         self.post_message(AddIndex.IndexAdded(self.added_index))
@@ -201,19 +201,19 @@
                 self.selected_index = "No index selected"
                 return None
 
             try:
                 async with get_client() as client:
                     index = client.index(self.selected_index)
                     await index.delete()
-                asyncio.create_task(self._success_message())
+                await self._success_message()
             except MeilisearchError as e:
-                asyncio.create_task(self._error_message(f"{e}"))
+                await self._error_message(f"{e}")
             except Exception as e:
-                asyncio.create_task(self._error_message(f"An unknown error occured error: {e}"))
+                await self._error_message(f"An unknown error occured error: {e}")
 
         self.selected_index = None
         self.post_message(DeleteIndex.IndexDeleted())
 
     async def _success_message(self) -> None:
         self.indexing_successful.visible = True
         await asyncio.sleep(5)
@@ -313,19 +313,19 @@
             try:
                 async with get_client() as client:
                     index = client.index(selected_index)
                     if data_file_path.suffix == ".json":
                         await index.add_documents_from_file_in_batches(data_file_path)
                     else:
                         await index.add_documents_from_raw_file(data_file_path)
-                asyncio.create_task(self._success_message())
+                await self._success_message()
             except MeilisearchError as e:
-                asyncio.create_task(self._error_message(f"{e}"))
+                await self._error_message(f"{e}")
             except Exception as e:
-                asyncio.create_task(self._error_message(f"An unknown error occured error: {e}"))
+                await self._error_message(f"An unknown error occured error: {e}")
 
         self.data_file.value = ""
 
     def on_key(self, event: events.Key) -> None:
         if event.key == "enter":
             self.load_data_button.press()
 
@@ -549,35 +549,31 @@
                     pagination=pagination,
                 )
 
                 async with get_client() as client:
                     index = client.index(self.selected_index)
                     await index.update_settings(settings)
             except Exception as e:
-                asyncio.create_task(
-                    self._error_message(f"An error occurred saving the settings: {e}")
-                )
+                await self._error_message(f"An error occurred saving the settings: {e}")
                 return
 
         if button_id == "reset-settings-button" and self.selected_index:
             try:
                 async with get_client() as client:
                     index = client.index(self.selected_index)
                     await index.reset_settings()
             except Exception as e:
-                asyncio.create_task(
-                    self._error_message(f"An error occurred resetting the settings: {e}")
-                )
+                await self._error_message(f"An error occurred resetting the settings: {e}")
                 return
 
-        asyncio.create_task(self._load_settings())
+        await self._load_settings()
         self.settings_saved = True
 
     async def watch_selected_index(self) -> None:
-        asyncio.create_task(self._load_settings())
+        await self._load_settings()
 
     def watch_settings_saved(self) -> None:
         if self.settings_saved:
             self.post_message(EditMeilisearchSettings.SettingsSaved(True))
 
         self.settings_saved = False
 
@@ -648,15 +644,15 @@
         return self.query_one("#edit-settings", VerticalScroll)
 
     @cached_property
     def edit_meilisearch_settings(self) -> EditMeilisearchSettings:
         return self.query_one(EditMeilisearchSettings)
 
     async def watch_selected_index(self) -> None:
-        asyncio.create_task(self.load_settings())
+        await self.load_settings()
         self.edit_meilisearch_settings.selected_index = self.selected_index
 
     def watch_edit_view(self) -> None:
         if self.edit_view:
             self.view_settings.display = False
             self.edit_settings_container.display = True
         else:
@@ -664,15 +660,15 @@
             self.edit_settings_container.display = False
 
     async def on_edit_meilisearch_settings_settings_saved(
         self, event: EditMeilisearchSettings.SettingsSaved
     ) -> None:
         if event.settings_saved:
             self.edit_view = False
-            asyncio.create_task(self.load_settings())
+            await self.load_settings()
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         button_id = event.button.id
 
         if button_id == "edit-settings-button":
             self.edit_view = True
```

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.7.3/meilisearch_tui/screens/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import asyncio
 from functools import cached_property
 
 from aiocache import cached
 from meilisearch_python_async.errors import MeilisearchCommunicationError
 from meilisearch_python_async.models.search import SearchResults
 from textual import events
 from textual.app import ComposeResult
@@ -102,25 +101,25 @@
         self.index_name.update(f"Searching index: {self.selected_index}")
         self.search_input.value = ""
         self.results.update("")
 
     async def on_input_changed(self, message: Input.Changed) -> None:
         self.limit = 20
         if message.value:
-            asyncio.create_task(self.search(message.value))
+            await self.search(message.value)
         else:
             self.results.update("")
             self.load_more_button.visible = False
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         button_id = event.button.id
 
         if button_id == "load-more-button":
             self.limit += 20
-            asyncio.create_task(self.search(self.search_input.value))
+            await self.search(self.search_input.value)
 
     @cached(ttl=10)
     async def search(self, search: str) -> None:
         if not self.selected_index and search == self.search_input.value:
             self.results.update("Error: No index provided")
             return
```

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/utils.py` & `meilisearch_tui-0.7.3/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.7.3/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.7.3/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.7.3/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.7.3/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.2/pyproject.toml` & `meilisearch_tui-0.7.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.7.2"
+version = "0.7.3"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -17,31 +17,30 @@
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-meilisearch-python-async = "1.2.2"
-textual = "0.24.1"
+meilisearch-python-async = "1.3.0"
+textual = "0.27.0"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
 aiocache = "0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
 mypy = "1.3.0"
-pre-commit = "3.3.1"
+pre-commit = "3.3.2"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
-pytest-cov = "4.0.0"
-ruff = "0.0.265"
-tox = "4.5.1"
+pytest-cov = "4.1.0"
+ruff = "0.0.270"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 meilisearch = "meilisearch_tui.__main__:main"
@@ -84,11 +83,12 @@
 addopts = "--cov=meilisearch_tui --cov-report term-missing"
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
 
 [tool.ruff]
-select = ["E", "F", "T201", "T203", "I001"]
+select = ["E", "F", "UP", "I001", "T201", "T203"]
 ignore = ["E501"]
 line-length = 100
+target-version = "py38"
 fix = true
```

### Comparing `meilisearch_tui-0.7.2/PKG-INFO` & `meilisearch_tui-0.7.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.7.2
+Version: 0.7.3
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,21 +12,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiocache (==0.12.1)
-Requires-Dist: meilisearch-python-async (==1.2.2)
-Requires-Dist: textual (==0.24.1)
+Requires-Dist: meilisearch-python-async (==1.3.0)
+Requires-Dist: textual (==0.27.0)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
 
 # Meilisearch TUI
```

