# Comparing `tmp/streamlit-lottie-0.0.3.tar.gz` & `tmp/streamlit-lottie-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-lottie-0.0.3.tar", last modified: Wed Dec  1 20:31:00 2021, max compression
+gzip compressed data, was "streamlit-lottie-0.0.4.tar", last modified: Mon Jun  5 13:42:32 2023, max compression
```

## Comparing `streamlit-lottie-0.0.3.tar` & `streamlit-lottie-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-12-01 20:31:00.243542 streamlit-lottie-0.0.3/
--rw-rw-rw-   0        0        0       53 2021-06-22 21:47:03.000000 streamlit-lottie-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3103 2021-12-01 20:31:00.241546 streamlit-lottie-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2056 2021-12-01 20:17:13.000000 streamlit-lottie-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2021-12-01 20:31:00.243542 streamlit-lottie-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1000 2021-06-22 21:47:03.000000 streamlit-lottie-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-01 20:30:59.948816 streamlit-lottie-0.0.3/streamlit_lottie/
--rw-rw-rw-   0        0        0     2371 2021-12-01 20:29:18.000000 streamlit-lottie-0.0.3/streamlit_lottie/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-01 20:30:59.942815 streamlit-lottie-0.0.3/streamlit_lottie/frontend/
-drwxrwxrwx   0        0        0        0 2021-12-01 20:31:00.035406 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/
--rw-rw-rw-   0        0        0     1047 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2113 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/index.html
--rw-rw-rw-   0        0        0      663 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/precache-manifest.15a63a0b1cb400a23885f1155cca2d92.js
--rw-rw-rw-   0        0        0     1183 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2021-12-01 20:30:59.944815 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2021-12-01 20:31:00.050977 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/css/
--rw-rw-rw-   0        0        0      153 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/css/main.885a514a.chunk.css
--rw-rw-rw-   0        0        0      352 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/css/main.885a514a.chunk.css.map
-drwxrwxrwx   0        0        0        0 2021-12-01 20:31:00.239557 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/
--rw-rw-rw-   0        0        0   728742 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/2.73b50dd7.chunk.js
--rw-rw-rw-   0        0        0     1653 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/2.73b50dd7.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2567736 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/2.73b50dd7.chunk.js.map
--rw-rw-rw-   0        0        0     1363 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/main.f28122a4.chunk.js
--rw-rw-rw-   0        0        0     4396 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/main.f28122a4.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-rw-rw-   0        0        0     8317 2021-12-01 20:30:07.000000 streamlit-lottie-0.0.3/streamlit_lottie/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxrwxrwx   0        0        0        0 2021-12-01 20:30:59.986822 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/
--rw-rw-rw-   0        0        0     3103 2021-12-01 20:30:59.000000 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2021-12-01 20:30:59.000000 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-01 20:30:59.000000 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2021-12-01 20:30:59.000000 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2021-12-01 20:30:59.000000 streamlit-lottie-0.0.3/streamlit_lottie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:42:32.455405 streamlit-lottie-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-05 13:42:32.455405 streamlit-lottie-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:42:32.455405 streamlit-lottie-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:42:32.455405 streamlit-lottie-0.0.4/streamlit_lottie/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/streamlit_lottie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/streamlit_lottie/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-05 13:42:05.000000 streamlit-lottie-0.0.4/streamlit_lottie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:42:32.455405 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-05 13:42:32.000000 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 13:42:32.000000 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:42:32.000000 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 13:42:32.000000 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 13:42:32.000000 streamlit-lottie-0.0.4/streamlit_lottie.egg-info/top_level.txt
```

### Comparing `streamlit-lottie-0.0.3/setup.py` & `streamlit-lottie-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from os.path import dirname
-from os.path import join
-import setuptools
-
-
-def readme() -> str:
-    """Utility function to read the README file.
-    Used for the long_description.  It's nice, because now 1) we have a top
-    level README file and 2) it's easier to type in the README file than to put
-    a raw string in below.
-    :return: content of README.md
-    """
-    return open(join(dirname(__file__), "README.md")).read()
-
-
-setuptools.setup(
-    name="streamlit-lottie",
-    version="0.0.3",
-    author="Fanilo ANDRIANASOLO",
-    author_email="andfanilo@gmail.com",
-    description="A Streamlit custom component to load Lottie animations",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/andfanilo/streamlit-lottie",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    classifiers=[],
-    python_requires=">=3.6",
-    install_requires=[
-        "streamlit >= 0.63",
-    ],
-)
+from os.path import dirname
+from os.path import join
+import setuptools
+
+
+def readme() -> str:
+    """Utility function to read the README file.
+    Used for the long_description.  It's nice, because now 1) we have a top
+    level README file and 2) it's easier to type in the README file than to put
+    a raw string in below.
+    :return: content of README.md
+    """
+    return open(join(dirname(__file__), "README.md")).read()
+
+
+setuptools.setup(
+    name="streamlit-lottie",
+    version="0.0.4",
+    author="Fanilo ANDRIANASOLO",
+    author_email="contact@andfanilo.com",
+    description="A Streamlit custom component to load Lottie animations",
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/andfanilo/streamlit-lottie",
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    classifiers=[],
+    python_requires=">=3.6",
+    install_requires=[
+        "streamlit >= 0.63",
+    ],
+)
```

