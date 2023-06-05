# Comparing `tmp/blurry_cli-0.2.1.tar.gz` & `tmp/blurry_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.2.1.tar", max compression
+gzip compressed data, was "blurry_cli-0.3.0.tar", max compression
```

## Comparing `blurry_cli-0.2.1.tar` & `blurry_cli-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/LICENSE
--rw-r--r--   0        0        0     1784 2023-04-16 22:37:50.018954 blurry_cli-0.2.1/README.md
--rw-r--r--   0        0        0     8177 2023-04-16 23:06:33.073434 blurry_cli-0.2.1/blurry/__init__.py
--rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/__main__.py
--rw-r--r--   0        0        0      527 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/async_typer.py
--rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/constants.py
--rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.2.1/blurry/images.py
--rw-r--r--   0        0        0     6514 2023-04-16 22:37:50.018954 blurry_cli-0.2.1/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-15 17:13:08.997639 blurry_cli-0.2.1/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0     1995 2023-04-23 22:31:36.524446 blurry_cli-0.2.1/blurry/open_graph.py
--rw-r--r--   0        0        0      189 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0     1145 2023-04-23 21:40:44.156168 blurry_cli-0.2.1/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      644 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1471 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/py.typed
--rw-r--r--   0        0        0     2042 2023-04-09 23:10:30.264113 blurry_cli-0.2.1/blurry/settings.py
--rw-r--r--   0        0        0     1546 2023-04-23 21:51:14.275747 blurry_cli-0.2.1/blurry/sitemap.py
--rw-r--r--   0        0        0      636 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/types.py
--rw-r--r--   0        0        0     3722 2023-04-23 21:40:44.156168 blurry_cli-0.2.1/blurry/utils.py
--rw-r--r--   0        0        0     1988 2023-04-23 22:52:11.247417 blurry_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 blurry_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1782 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/README.md
+-rw-r--r--   0        0        0     8177 2023-04-16 23:06:33.073434 blurry_cli-0.3.0/blurry/__init__.py
+-rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.3.0/blurry/__main__.py
+-rw-r--r--   0        0        0      526 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/async_typer.py
+-rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.3.0/blurry/constants.py
+-rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.3.0/blurry/images.py
+-rw-r--r--   0        0        0     6819 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1649 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/markdown/renderer_functions/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/markdown/renderer_functions/render_video.py
+-rw-r--r--   0        0        0     1995 2023-04-23 22:31:36.524446 blurry_cli-0.3.0/blurry/open_graph.py
+-rw-r--r--   0        0        0      189 2023-04-16 22:37:50.025621 blurry_cli-0.3.0/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.3.0/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1146 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.3.0/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-16 22:37:50.025621 blurry_cli-0.3.0/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      683 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1509 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.3.0/blurry/py.typed
+-rw-r--r--   0        0        0     2122 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/settings.py
+-rw-r--r--   0        0        0     1546 2023-04-23 21:51:14.275747 blurry_cli-0.3.0/blurry/sitemap.py
+-rw-r--r--   0        0        0      777 2023-06-04 15:53:32.861954 blurry_cli-0.3.0/blurry/types.py
+-rw-r--r--   0        0        0     3722 2023-04-23 21:40:44.156168 blurry_cli-0.3.0/blurry/utils.py
+-rw-r--r--   0        0        0     2034 2023-06-04 15:55:48.693891 blurry_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 blurry_cli-0.3.0/PKG-INFO
```

### Comparing `blurry_cli-0.2.1/LICENSE` & `blurry_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/README.md` & `blurry_cli-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Contributing
 
 Contributions are welcome!
 Check out [the contribution docs](https://github.com/blurry-dev/blurry/blob/main/CONTRIBUTING.md) to get started.
 
 ## Standing on the shoulders of giants
 
-Blurry stitches together high-quality libraries:
+Blurry blends together high-quality libraries:
 
 - [Mistune](https://mistune.readthedocs.io/) to convert Markdown to HTML
 - [Jinja](https://jinja.palletsprojects.com/) for HTML templating
 - [LiveReload](https://livereload.readthedocs.io/) for an HTTP server with automatic browser reloading
 - [Typer](https://typer.tiangolo.com/) for its CLI interface
 - [ImageMagick](https://imagemagick.org/index.php) to resize and convert images
```

### Comparing `blurry_cli-0.2.1/blurry/__init__.py` & `blurry_cli-0.3.0/blurry/__init__.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/blurry/async_typer.py` & `blurry_cli-0.3.0/blurry/async_typer.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from typer import Typer
 
 
 class AsyncTyper(Typer):
     def async_command(self, *args, **kwargs):
         def decorator(async_func):
-
             # Convert async function to synchronous
             @wraps(async_func)
             def sync_func(*_args, **_kwargs):
                 return asyncio.run(async_func(*_args, **_kwargs))
 
             # Register synchronous function
             self.command(*args, **kwargs)(sync_func)
```

### Comparing `blurry_cli-0.2.1/blurry/images.py` & `blurry_cli-0.3.0/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/blurry/markdown/__init__.py` & `blurry_cli-0.3.0/blurry/markdown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,78 +12,81 @@
 from mistune.plugins.table import table
 from mistune.plugins.task_lists import task_lists
 from mistune.plugins.url import url
 from mistune.util import escape
 from wand.image import Image
 
 from .front_matter import parse_front_matter
+from .renderer_functions.render_video import render_video
 from blurry.images import add_image_width_to_path
 from blurry.images import generate_sizes_string
 from blurry.images import generate_srcset_string
 from blurry.images import get_widths_for_image_width
-from blurry.images import THUMBNAIL_WIDTH
 from blurry.plugins import discovered_markdown_plugins
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import SETTINGS
+from blurry.types import is_str
 from blurry.utils import build_path_to_url
 from blurry.utils import content_path_to_url
 from blurry.utils import convert_relative_path_in_markdown_to_relative_build_path
 from blurry.utils import path_to_url_pathname
 from blurry.utils import remove_lazy_loading_from_first_image
 from blurry.utils import resolve_relative_path_in_markdown
 
 CONTENT_DIR = get_content_directory()
+THUMBNAIL_WIDTH = SETTINGS.get("THUMBNAIL_WIDTH")
 
 
 class BlurryRenderer(mistune.HTMLRenderer):
     """Renderer that converts relative content URLs to build URLs."""
 
     filepath: Path
 
     def image(self, alt, url, title=None) -> str:
         # Improve images:
         # - Converts relative paths to web server paths
         # - Convert to <picture> tag with AVIF <source>
         # - Adds srcset & sizes attributes
         # - Adds width & height attributes
         src = self.safe_url(url)
+
         attributes: dict[str, str] = {
             "alt": alt,
             "src": src,
             "loading": "lazy",
         }
         source_tag = ""
 
-        if title:
-            attributes["title"] = escape(title)
-
         # Make local images responsive
         if src.startswith("."):
             # Convert relative path to URL pathname
             absolute_path = resolve_relative_path_in_markdown(src, self.filepath)
-            img_extension = absolute_path.suffix
+            extension = absolute_path.suffix.removeprefix(".")
             src = path_to_url_pathname(absolute_path)
             attributes["src"] = src
 
+            if extension.lower() in SETTINGS.get("VIDEO_EXTENSIONS"):
+                return render_video(src, absolute_path, extension, title=alt)
+
             # Tailor srcset and sizes to image width
             with Image(filename=str(absolute_path)) as img:
                 image_width = img.width
                 attributes["width"] = image_width
                 attributes["height"] = img.height
 
-            if img_extension in [".webp", ".gif"]:
+            if extension in ["webp", "gif"]:
                 source_tag = ""
             else:
                 image_widths = get_widths_for_image_width(image_width)
 
                 attributes["sizes"] = generate_sizes_string(image_widths)
                 attributes["srcset"] = generate_srcset_string(src, image_widths)
                 avif_srcset = generate_srcset_string(
-                    src.replace(img_extension, ".avif"), image_widths
+                    src.replace(extension, "avif"), image_widths
                 )
                 source_tag = '<source srcset="{}" sizes="{}" />'.format(
                     avif_srcset, attributes["sizes"]
                 )
 
         attributes_str = " ".join(
             f'{name}="{value}"' for name, value in attributes.items()
@@ -149,18 +152,21 @@
     # Add filepath to the renderer to resolve relative paths
     if not is_blurry_renderer(markdown.renderer):
         raise Exception(
             f"Markdown renderer is not BlurryRenderer {repr(markdown.renderer)}"
         )
     markdown.renderer.filepath = filepath
     initial_state = BlockState()
-    initial_state.env["__file__"] = str(filepath)
+    initial_state.env["__file__"] = str(filepath)  # type: ignore
     markdown_text, state = parse_front_matter(markdown, state=initial_state)
     html, state = markdown.parse(markdown_text, state=state)
 
+    if not is_str(html):
+        raise Exception(f"Expected html to be a string but got: {type(html)}")
+
     # Post-process HTML
     html = remove_lazy_loading_from_first_image(html)
 
     # Seed front_matter with schema_data from config file
     front_matter: dict[str, Any] = dict(SETTINGS.get("SCHEMA_DATA", {}))
     front_matter.update(state.env.get("front_matter", {}))
```

### Comparing `blurry_cli-0.2.1/blurry/markdown/front_matter.py` & `blurry_cli-0.3.0/blurry/markdown/front_matter.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,9 +44,9 @@
 
 def parse_front_matter(_: Markdown, state: BlockState) -> tuple[str, BlockState]:
     filepath = state.env.get("__file__")
     if not isinstance(filepath, str):
         raise Exception(f"Count not find filepath {filepath}")
     file_contents = Path(filepath).read_text()
     markdown_text, front_matter = get_data(file_contents)
-    state.env["front_matter"] = front_matter
+    state.env["front_matter"] = front_matter  # type: ignore
     return markdown_text, state
```

### Comparing `blurry_cli-0.2.1/blurry/open_graph.py` & `blurry_cli-0.3.0/blurry/open_graph.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/blurry/plugins/html_plugins/minify_html_plugin.py` & `blurry_cli-0.3.0/blurry/plugins/html_plugins/minify_html_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import htmlmin
 import re
+
+import htmlmin
 from selectolax.parser import HTMLParser
 
 from blurry.types import TemplateContext
 
 
 def minify_css(css: str) -> str:
     minified_css = css.strip()
```

### Comparing `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.3.0/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.3.0/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from re import Match
-from mistune import InlineState, InlineParser, Markdown
+
+from mistune import InlineParser
+from mistune import InlineState
+from mistune import Markdown
 
 EM_DASH_PATTERN = r"---"
 EN_DASH_PATTERN = r"--"
 
 
 def parse_em_dash(_: InlineParser, match: Match, state: InlineState):
     pos = match.end()
```

### Comparing `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.3.0/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import importlib
 import inspect
 import re
-import importlib
 
-from mistune import Markdown, BlockState, BlockParser
+from mistune import BlockParser
+from mistune import BlockState
+from mistune import Markdown
 
 PYTHON_CODE_PATTERN = r"[\s]*@(?P<language>[a-z]+)<(?P<path>.+)>"
 
 
 def parse_python_code(_: BlockParser, match: re.Match, state: BlockState):
     language = match.group("language")
     path = match.group("path")
```

### Comparing `blurry_cli-0.2.1/blurry/settings.py` & `blurry_cli-0.3.0/blurry/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     DEV_HOST: str
     DEV_PORT: int
     DOMAIN: str
     IMAGE_WIDTHS: list[int]
     MAXIMUM_IMAGE_WIDTH: int
     THUMBNAIL_WIDTH: int
+    VIDEO_EXTENSIONS: list[str]
     USE_HTTP: bool
     RUNSERVER: bool
     FRONTMATTER_NON_SCHEMA_VARIABLE_PREFIX: str
 
 
 SETTINGS: Settings = {
     "AVIF_COMPRESSION_QUALITY": 90,
@@ -33,14 +34,15 @@
     "DEV_HOST": "127.0.0.1",
     "DEV_PORT": 8000,
     "DOMAIN": "example.com",
     # Sizes adapted from: https://link.medium.com/UqzDeLKwyeb
     "IMAGE_WIDTHS": [360, 640, 768, 1024, 1366, 1600, 1920],
     "MAXIMUM_IMAGE_WIDTH": 1920,
     "THUMBNAIL_WIDTH": 250,
+    "VIDEO_EXTENSIONS": ["mp4", "webm", "mkv"],
     "USE_HTTP": False,
     "RUNSERVER": False,
     "FRONTMATTER_NON_SCHEMA_VARIABLE_PREFIX": "~",
     "TEMPLATE_SCHEMA_TYPES": {},
 }
 
 try:
```

### Comparing `blurry_cli-0.2.1/blurry/sitemap.py` & `blurry_cli-0.3.0/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/blurry/types.py` & `blurry_cli-0.3.0/blurry/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any
+from typing import TypeGuard
 
 
 @dataclass
 class MarkdownFileData:
     body: str
     front_matter: dict[str, Any]
     path: Path
@@ -23,7 +24,13 @@
     ORGANIZATION = "Organization"
     PERSON = "Person"
 
 
 DirectoryFileData = dict[Path, list[MarkdownFileData]]
 
 TemplateContext = dict[str, Any]
+
+
+def is_str(value: Any) -> TypeGuard[str]:
+    if isinstance(value, str):
+        return True
+    return False
```

### Comparing `blurry_cli-0.2.1/blurry/utils.py` & `blurry_cli-0.3.0/blurry/utils.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.1/pyproject.toml` & `blurry_cli-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.2.1"
+version = "0.3.0"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
@@ -22,31 +22,33 @@
     "LICENSE",
 ]
 packages = [
     { include = "blurry" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-PyLD = "^2.0.3"
-mistune = "^3.0.0rc5"
 Jinja2 = "^3.0.0"
-livereload = "^2.6.3"
-typer = "^0.6.1"
+PyLD = "^2.0.3"
 Wand = "^0.6.6"
-toml = "^0.10.2"
+ffmpeg-python = "^0.2.0"
 htmlmin = "^0.1.12"
-selectolax = "^0.3.6"
+livereload = "^2.6.3"
+mistune = "^3.0.0rc5"
+python = "^3.10"
 rich = "^13.3.3"
+selectolax = "^0.3.6"
+toml = "^0.10.2"
+typer = "^0.6.1"
 
 [tool.poetry.dev-dependencies]
+black = "^22.10.0"
+pyright = "^1.1.311"
 pytest = "^6.2.2"
-pytest-watch = "^4.2.0"
 pytest-cov = "^2.11.1"
-black = "^22.10.0"
+pytest-watch = "^4.2.0"
 
 [tool.poetry.scripts]
 blurry = 'blurry:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `blurry_cli-0.2.1/PKG-INFO` & `blurry_cli-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
@@ -20,14 +20,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management 
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML 
 Classifier: Topic :: Text Processing :: Markup :: Markdown 
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: PyLD (>=2.0.3,<3.0.0)
 Requires-Dist: Wand (>=0.6.6,<0.7.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: htmlmin (>=0.1.12,<0.2.0)
 Requires-Dist: livereload (>=2.6.3,<3.0.0)
 Requires-Dist: mistune (>=3.0.0rc5,<4.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: selectolax (>=0.3.6,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
@@ -59,15 +60,15 @@
 ## Contributing
 
 Contributions are welcome!
 Check out [the contribution docs](https://github.com/blurry-dev/blurry/blob/main/CONTRIBUTING.md) to get started.
 
 ## Standing on the shoulders of giants
 
-Blurry stitches together high-quality libraries:
+Blurry blends together high-quality libraries:
 
 - [Mistune](https://mistune.readthedocs.io/) to convert Markdown to HTML
 - [Jinja](https://jinja.palletsprojects.com/) for HTML templating
 - [LiveReload](https://livereload.readthedocs.io/) for an HTTP server with automatic browser reloading
 - [Typer](https://typer.tiangolo.com/) for its CLI interface
 - [ImageMagick](https://imagemagick.org/index.php) to resize and convert images
```

