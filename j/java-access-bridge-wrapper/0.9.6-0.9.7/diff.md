# Comparing `tmp/java-access-bridge-wrapper-0.9.6.tar.gz` & `tmp/java-access-bridge-wrapper-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java-access-bridge-wrapper-0.9.6.tar", max compression
+gzip compressed data, was "java-access-bridge-wrapper-0.9.7.tar", max compression
```

## Comparing `java-access-bridge-wrapper-0.9.6.tar` & `java-access-bridge-wrapper-0.9.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2021-06-15 06:20:32.304687 java-access-bridge-wrapper-0.9.6/LICENSE
--rw-r--r--   0        0        0     1044 2023-03-23 11:07:46.297694 java-access-bridge-wrapper-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3134 2022-01-05 10:23:23.675337 java-access-bridge-wrapper-0.9.6/README.md
--rw-r--r--   0        0        0    20563 2023-03-23 09:33:01.253323 java-access-bridge-wrapper-0.9.6/src/JABWrapper/context_tree.py
--rw-r--r--   0        0        0     5587 2023-03-23 08:15:42.443278 java-access-bridge-wrapper-0.9.6/src/JABWrapper/jab_types.py
--rw-r--r--   0        0        0    79824 2023-03-23 11:05:14.142027 java-access-bridge-wrapper-0.9.6/src/JABWrapper/jab_wrapper.py
--rw-r--r--   0        0        0     1735 2023-03-22 10:51:00.086202 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/actions_parser.py
--rw-r--r--   0        0        0     2063 2023-03-22 10:51:00.087212 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/hypertext_parser.py
--rw-r--r--   0        0        0     1408 2023-03-22 10:51:00.088200 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/icon_parser.py
--rw-r--r--   0        0        0     1522 2023-03-22 10:51:00.088200 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/keybind_parser.py
--rw-r--r--   0        0        0       75 2022-01-05 10:23:23.684438 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/parser_if.py
--rw-r--r--   0        0        0      666 2023-03-22 10:51:00.089213 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/selection_parser.py
--rw-r--r--   0        0        0     1283 2023-03-22 10:51:00.090210 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/table_parser.py
--rw-r--r--   0        0        0     4509 2023-03-22 10:51:00.091202 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/text_parser.py
--rw-r--r--   0        0        0      895 2023-03-22 10:51:00.092203 java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/value_parser.py
--rw-r--r--   0        0        0     1604 2022-08-16 09:00:48.398750 java-access-bridge-wrapper-0.9.6/src/JABWrapper/utils.py
--rw-r--r--   0        0        0     4221 2023-03-23 11:09:59.019307 java-access-bridge-wrapper-0.9.6/setup.py
--rw-r--r--   0        0        0     4246 2023-03-23 11:09:59.020306 java-access-bridge-wrapper-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-06-15 06:20:32.304687 java-access-bridge-wrapper-0.9.7/LICENSE
+-rw-r--r--   0        0        0     1044 2023-03-23 11:30:16.095093 java-access-bridge-wrapper-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3134 2022-01-05 10:23:23.675337 java-access-bridge-wrapper-0.9.7/README.md
+-rw-r--r--   0        0        0    20563 2023-03-23 09:33:01.253323 java-access-bridge-wrapper-0.9.7/src/JABWrapper/context_tree.py
+-rw-r--r--   0        0        0     5587 2023-03-23 08:15:42.443278 java-access-bridge-wrapper-0.9.7/src/JABWrapper/jab_types.py
+-rw-r--r--   0        0        0    79823 2023-03-23 11:29:14.267282 java-access-bridge-wrapper-0.9.7/src/JABWrapper/jab_wrapper.py
+-rw-r--r--   0        0        0     1735 2023-03-22 10:51:00.086202 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/actions_parser.py
+-rw-r--r--   0        0        0     2063 2023-03-22 10:51:00.087212 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/hypertext_parser.py
+-rw-r--r--   0        0        0     1408 2023-03-22 10:51:00.088200 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/icon_parser.py
+-rw-r--r--   0        0        0     1522 2023-03-22 10:51:00.088200 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/keybind_parser.py
+-rw-r--r--   0        0        0       75 2022-01-05 10:23:23.684438 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/parser_if.py
+-rw-r--r--   0        0        0      666 2023-03-22 10:51:00.089213 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/selection_parser.py
+-rw-r--r--   0        0        0     1283 2023-03-22 10:51:00.090210 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/table_parser.py
+-rw-r--r--   0        0        0     4509 2023-03-22 10:51:00.091202 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/text_parser.py
+-rw-r--r--   0        0        0      895 2023-03-22 10:51:00.092203 java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/value_parser.py
+-rw-r--r--   0        0        0     1604 2022-08-16 09:00:48.398750 java-access-bridge-wrapper-0.9.7/src/JABWrapper/utils.py
+-rw-r--r--   0        0        0     4221 2023-03-23 11:30:45.836911 java-access-bridge-wrapper-0.9.7/setup.py
+-rw-r--r--   0        0        0     4246 2023-03-23 11:30:45.836911 java-access-bridge-wrapper-0.9.7/PKG-INFO
```

### Comparing `java-access-bridge-wrapper-0.9.6/LICENSE` & `java-access-bridge-wrapper-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/pyproject.toml` & `java-access-bridge-wrapper-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "java-access-bridge-wrapper"
-version = "0.9.6"
+version = "0.9.7"
 description = "Python wrapper for the Windows Java Access Bridge"
 license = "Apache-2.0"
 readme = "README.md"
 authors = [
 	"Robocorp <support@robocorp.com>",
 ]
 repository = "https://github.com/robocorp/java-access-bridge-wrapper.git"
```

### Comparing `java-access-bridge-wrapper-0.9.6/README.md` & `java-access-bridge-wrapper-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/context_tree.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/context_tree.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/jab_types.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/jab_types.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/jab_wrapper.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/jab_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
     def set_hwnd(self, hwnd: wintypes.HWND) -> None:
         self._hwnd = hwnd
 
     def set_context(self, vm_id: c_long, context: JavaObject) -> None:
         self._vmID = vm_id
         self.context = context
 
-    def get_expected_windows_handle(self) -> wintypes.HWND:
+    def get_current_windows_handle(self) -> wintypes.HWND:
         return self._hwnd
 
     def release_object(self, context: JavaObject) -> None:
         """
         Release the java object received via the API.
 
         Mainly used to release the events received via the Windows event system.
```

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/actions_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/actions_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/hypertext_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/hypertext_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/icon_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/icon_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/keybind_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/keybind_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/selection_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/selection_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/table_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/table_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/text_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/text_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/parsers/value_parser.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/parsers/value_parser.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/src/JABWrapper/utils.py` & `java-access-bridge-wrapper-0.9.7/src/JABWrapper/utils.py`

 * *Files identical despite different names*

### Comparing `java-access-bridge-wrapper-0.9.6/setup.py` & `java-access-bridge-wrapper-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.7.6" and sys_platform == "win32" or python_version > "3.7.6" and python_version < "3.8.1" and sys_platform == "win32" or python_version > "3.8.1" and sys_platform == "win32"': ['pywin32>=300,<304']}
 
 setup_kwargs = {
     'name': 'java-access-bridge-wrapper',
-    'version': '0.9.6',
+    'version': '0.9.7',
     'description': 'Python wrapper for the Windows Java Access Bridge',
     'long_description': '[![Version](https://img.shields.io/pypi/v/java-access-bridge-wrapper.svg?label=version)](https://pypi.org/project/java-access-bridge-wrapper/)\n[![License](https://img.shields.io/pypi/l/java-access-bridge-wrapper.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)\n\n# Introduction\n\nPython wrapper around the Java Access Bridge / Windows Access Bridge.\n\n# Prerequisites\n\n* 64-bit Windows\n* Java >= 8 (https://docs.aws.amazon.com/corretto/latest/corretto-8-ug/downloads-list.html)\n* Python >= 3.7 (https://www.python.org/downloads/release/python-375/)\n\nEnable the Java Access Bridge in windows\n\n    C:\\path\\to\\java\\bin\\jabswitch -enable\n\n# Install\n\n    pip install java-access-bridge-wrapper\n\n# How to use\n\nImport the Java Access Bridge (JAB) wrapper and optionally the context tree\n\n    from JABWrapper.jab_wrapper import JavaAccessBridgeWrapper\n    from JABWrapper.context_tree import ContextNode, ContextTree, SearchElement\n\nThe JAB creates an virtual GUI window when it is opened. For the JAB to operate and receive events from the GUI, the calling code needs to implement the windows\nmessage pump and call it in a loop. The JABWrapper object needs to be in the same thread.\n\nThis can be achieved for example by starting the message pump in a separate thread, where the JAB object is also initialized.\n\n    GetMessage = ctypes.windll.user32.GetMessageW\n    TranslateMessage = ctypes.windll.user32.TranslateMessage\n    DispatchMessage = ctypes.windll.user32.DispatchMessageW\n\n    def pump_background(pipe: queue.Queue):\n        try:\n            jab_wrapper = JavaAccessBridgeWrapper()\n            pipe.put(jab_wrapper)\n            message = byref(wintypes.MSG())\n            while GetMessage(message, 0, 0, 0) > 0:\n                TranslateMessage(message)\n                logging.debug("Dispatching msg={}".format(repr(message)))\n                DispatchMessage(message)\n        except Exception as err:\n            pipe.put(None)\n\n    def main():\n        pipe = queue.Queue()\n            thread = threading.Thread(target=pump_background, daemon=True, args=[pipe])\n            thread.start()\n            jab_wrapper = pipe.get()\n            if not jab_wrapper:\n                raise Exception("Failed to initialize Java Access Bridge Wrapper")\n            time.sleep(0.1) # Wait until the initial messages are parsed, before accessing frames\n\n    if __name__ == "__main__":\n        main()\n\nOnce the JABWrapper object is initialized, attach to some frame and optionally create the context tree to get the element tree of the application.\n\n    jab_wrapper.switch_window_by_title("Frame title")\n    context_tree = ContextTree(jab_wrapper)\n\n# Development\n\n## Development prerequisites\n\n* Install poetry: https://python-poetry.org/docs/\n\n## Test\n\nRun test script against simple Swing application\n\nset environment variable\n\n    set RC_JAVA_ACCESS_BRIDGE_DLL="C:\\path\\to\\Java\\bin\\WindowsAccessBridge-64.dll"\n\nRun test with poetry\n\n    poetry run python tests\\test.py\n\n## Packaging\n\n    poetry build\n    poetry publish\n\n## TODO:\n\n* Support for 32-bit Java Access Bridge version\n* Implement rest of the utility functions to the JABWrapper\n',
     'author': 'Robocorp',
     'author_email': 'support@robocorp.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/robocorp/java-access-bridge-wrapper.git',
```

### Comparing `java-access-bridge-wrapper-0.9.6/PKG-INFO` & `java-access-bridge-wrapper-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: java-access-bridge-wrapper
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python wrapper for the Windows Java Access Bridge
 Home-page: https://github.com/robocorp/java-access-bridge-wrapper.git
 License: Apache-2.0
 Author: Robocorp
 Author-email: support@robocorp.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

