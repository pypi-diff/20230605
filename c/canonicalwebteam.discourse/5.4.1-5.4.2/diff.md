# Comparing `tmp/canonicalwebteam.discourse-5.4.1.tar.gz` & `tmp/canonicalwebteam.discourse-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam.discourse-5.4.1.tar", last modified: Fri Apr 21 14:02:48 2023, max compression
+gzip compressed data, was "canonicalwebteam.discourse-5.4.2.tar", last modified: Mon Jun  5 09:50:52 2023, max compression
```

## Comparing `canonicalwebteam.discourse-5.4.1.tar` & `canonicalwebteam.discourse-5.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.118363 canonicalwebteam.discourse-5.4.1/canonicalwebteam/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27552 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.118363 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/fixtures/forum_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_engage_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/canonicalwebteam/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20633 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25670 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27244 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-05 09:50:52.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 09:50:52.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:50:52.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 09:50:52.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 09:50:52.000000 canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      721 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:52.109210 canonicalwebteam.discourse-5.4.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/fixtures/forum_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/test_engage_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-05 09:50:47.000000 canonicalwebteam.discourse-5.4.2/tests/test_parser.py
```

### Comparing `canonicalwebteam.discourse-5.4.1/LICENSE` & `canonicalwebteam.discourse-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/PKG-INFO` & `canonicalwebteam.discourse-5.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.discourse
-Version: 5.4.1
+Version: 5.4.2
 Summary: Flask extension to integrate discourse content generated to docs to your website.
 Home-page: https://github.com/canonical/canonicalwebteam.discourse
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,14 +47,25 @@
 
 Once this is added you will need to add the file `document.html` to your template folder.
 
 ## Local development
 
 For local development, it's best to test this module with one of our website projects like [ubuntu.com](https://github.com/canonical-web-and-design/ubuntu.com/). For more information, follow [this guide (internal only)](https://discourse.canonical.com/t/how-to-run-our-python-modules-for-local-development/308).
 
+### Running tests, linting and formatting
+
+Tests can be run with [Tox](https://tox.wiki/en/latest/):
+
+``` bash
+pip3 install tox  # Install tox
+tox               # Run tests
+tox -e lint       # Check the format of Python code
+tox -e format     # Reformat the Python code
+```
+
 ## Instructions for Engage pages extension
 
 Because you are viewing a protected topic, you must provide `api_key` and `api_username`. You also need an index topic id, which you can get from discourse.ubuntu.com. Your index topic must contain a metadata section. Visit the EngageParser for more information about the structure. You are encouraged to use an blueprint name that does not collide with existent blueprints. The templates must match the ones provided in the parameters indicated.
 
 Here is an example of an implementation:
 
 ```python
```

### Comparing `canonicalwebteam.discourse-5.4.1/README.md` & `canonicalwebteam.discourse-5.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 
 Once this is added you will need to add the file `document.html` to your template folder.
 
 ## Local development
 
 For local development, it's best to test this module with one of our website projects like [ubuntu.com](https://github.com/canonical-web-and-design/ubuntu.com/). For more information, follow [this guide (internal only)](https://discourse.canonical.com/t/how-to-run-our-python-modules-for-local-development/308).
 
+### Running tests, linting and formatting
+
+Tests can be run with [Tox](https://tox.wiki/en/latest/):
+
+``` bash
+pip3 install tox  # Install tox
+tox               # Run tests
+tox -e lint       # Check the format of Python code
+tox -e format     # Reformat the Python code
+```
+
 ## Instructions for Engage pages extension
 
 Because you are viewing a protected topic, you must provide `api_key` and `api_username`. You also need an index topic id, which you can get from discourse.ubuntu.com. Your index topic must contain a metadata section. Visit the EngageParser for more information about the structure. You are encouraged to use an blueprint name that does not collide with existent blueprints. The templates must match the ones provided in the parameters indicated.
 
 Here is an example of an implementation:
 
 ```python
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/app.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         @self.blueprint.route("/sitemap.txt")
         def sitemap_view():
             """
             Show a list of all URLs in the URL map
             """
 
-            self.parser.ensure_parsed()
+            self.parser.parse()
 
             urls = []
 
             for key, value in self.parser.url_map.items():
                 if type(key) is str:
                     urls.append(flask.request.host_url.strip("/") + key)
 
@@ -48,15 +48,15 @@
 
         @self.blueprint.route("/sitemap.xml")
         def sitemap_xml():
             """
             Show a list of all URLs in the URL map
             """
 
-            self.parser.ensure_parsed()
+            self.parser.parse()
             pages = []
 
             for key, value in self.parser.url_map.items():
                 if type(key) is str:
                     try:
                         response = parser.api.get_topic(str(value))
                         last_updated = response["post_stream"]["posts"][0][
@@ -156,15 +156,15 @@
         def document_view(path=""):
             """
             A Flask view function to serve
             topics pulled from Discourse as documentation pages.
             """
             docs_version = ""
             path = "/" + path
-            self.parser.ensure_parsed()
+            self.parser.parse()
 
             if path == "/":
                 document = self.parser.parse_topic(self.parser.index_topic)
             else:
                 try:
                     topic_id, docs_version = self.parser.resolve_path(path)
                 except RedirectFoundError as redirect:
@@ -235,15 +235,15 @@
         def document_view(path=""):
             """
             A Flask view function to serve
             topics pulled from Discourse as documentation pages.
             """
 
             path = "/" + path
-            self.parser.ensure_parsed()
+            self.parser.parse()
 
             if path == "/":
                 document = self.parser.parse_topic(self.parser.index_topic)
             else:
                 try:
                     topic_id = self.parser.resolve_path(path)
                 except RedirectFoundError as redirect:
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/exceptions.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/exceptions.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/models.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/models.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/base_parser.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/base_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,15 +475,15 @@
         <p>Content</p>
         <h2>Next heading</h2>
 
         and `title_text` is "My heading", then it will return:
 
         <p>Content</p>
         """
-        heading = soup.find(HEADER_REGEX, text=title_text)
+        heading = soup.find(HEADER_REGEX, string=title_text)
 
         if not heading:
             return None
 
         heading_tag = heading.name
         section_soup = BeautifulSoup()
         for sibling in list(heading.next_siblings):
@@ -497,15 +497,15 @@
     def _get_preamble(self, soup, break_on_title):
         """
         Given a BeautifulSoup HTML document,
         separate out the HTML at the start, up to
         the heading defined in `break_on_title`,
         and return it as a BeautifulSoup object
         """
-        heading = soup.find(HEADER_REGEX, text=break_on_title)
+        heading = soup.find(HEADER_REGEX, string=break_on_title)
 
         if not heading:
             return soup
         # get all the previous contents, reversing order on insert
         preamble_soup = BeautifulSoup()
         for sibling in list(heading.previous_siblings):
             preamble_soup.insert(0, sibling)
@@ -610,15 +610,16 @@
                 <div class="p-notification__response">
                     <p class="u-no-padding--top u-no-margin--bottom">
                         Content
                     </p>
                 </div>
             </div>
         """
-        for note_string in soup.findAll(text=re.compile("ⓘ ")):
+
+        for note_string in soup.find_all(string=re.compile("ⓘ ")):
             first_paragraph = note_string.parent
             blockquote = first_paragraph.parent
             last_paragraph = blockquote.findChildren(recursive=False)[-1]
 
             if first_paragraph.name == "p" and blockquote.name == "blockquote":
                 # Remove extra padding/margin
                 first_paragraph.attrs["class"] = "u-no-padding--top"
@@ -754,15 +755,15 @@
         from the following Markdown:
 
         > :construction: **NOTE TO EDITORS** :construction:
         >
         > ...
         """
 
-        notes_to_editors_text = soup.find_all(text="NOTE TO EDITORS")
+        notes_to_editors_text = soup.find_all(string="NOTE TO EDITORS")
 
         for text in notes_to_editors_text:
             # If this section is of the expected HTML format,
             # we should find the <aside> container 4 levels up from
             # the "NOTE TO EDITORS" text
             container = text.parent.parent.parent.parent
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/docs.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,14 @@
         # Tutorials
         self.tutorials_url_map = {}
         self.tutorials_index_topic_id = tutorials_index_topic_id
         self.tutorials_url_prefix = tutorials_url_prefix
 
         return super().__init__(api, index_topic_id, url_prefix)
 
-    def ensure_parsed(self) -> bool:
-        """
-        Ensure that we have parsed the cooked post into parts.
-
-        returns True if it's already parsed, or False if we needed to parse.
-        """
-        if self.index_topic is not None:
-            return True
-        self.parse()
-        return False
-
     def parse(self):
         """
         Get the index topic and split it into:
         - navigation
         - index document content
         - URL map
         - redirects map
@@ -810,15 +799,15 @@
             if value == "true":
                 return True
             elif value == "false":
                 return False
             else:
                 return value
 
-        heading = index_soup.find(re.compile("^h[1-6]$"), text=section_name)
+        heading = index_soup.find(re.compile("^h[1-6]$"), string=section_name)
 
         if not heading:
             return None
 
         metadata_soup = heading.findNext("div", {"class": "md-table"})
 
         metadata_object = {}
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/tutorials.py` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam/discourse/parsers/tutorials.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,14 @@
 
 class TutorialParser(BaseParser):
     def __init__(self, api, index_topic_id, url_prefix):
         self.tutorials = None
         self.errors = []
         return super().__init__(api, index_topic_id, url_prefix)
 
-    def ensure_parsed(self) -> bool:
-        """
-        Ensure that we have parsed the cooked post into parts.
-
-        returns True if it's already parsed, or False if we needed to parse.
-        """
-        if self.index_topic is not None:
-            return True
-        self.parse()
-        return False
-
     def parse(self):
         """
         Get the index topic and split it into:
         - navigation
         - index document content
         - URL map
         - redirects map
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/PKG-INFO` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.discourse
-Version: 5.4.1
+Version: 5.4.2
 Summary: Flask extension to integrate discourse content generated to docs to your website.
 Home-page: https://github.com/canonical/canonicalwebteam.discourse
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,14 +47,25 @@
 
 Once this is added you will need to add the file `document.html` to your template folder.
 
 ## Local development
 
 For local development, it's best to test this module with one of our website projects like [ubuntu.com](https://github.com/canonical-web-and-design/ubuntu.com/). For more information, follow [this guide (internal only)](https://discourse.canonical.com/t/how-to-run-our-python-modules-for-local-development/308).
 
+### Running tests, linting and formatting
+
+Tests can be run with [Tox](https://tox.wiki/en/latest/):
+
+``` bash
+pip3 install tox  # Install tox
+tox               # Run tests
+tox -e lint       # Check the format of Python code
+tox -e format     # Reformat the Python code
+```
+
 ## Instructions for Engage pages extension
 
 Because you are viewing a protected topic, you must provide `api_key` and `api_username`. You also need an index topic id, which you can get from discourse.ubuntu.com. Your index topic must contain a metadata section. Visit the EngageParser for more information about the structure. You are encouraged to use an blueprint name that does not collide with existent blueprints. The templates must match the ones provided in the parameters indicated.
 
 Here is an example of an implementation:
 
 ```python
```

### Comparing `canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/SOURCES.txt` & `canonicalwebteam.discourse-5.4.2/canonicalwebteam.discourse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/setup.py` & `canonicalwebteam.discourse-5.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 setup(
     name="canonicalwebteam.discourse",
-    version="5.4.1",
+    version="5.4.2",
     author="Canonical webteam",
     author_email="webteam@canonical.com",
     url="https://github.com/canonical/canonicalwebteam.discourse",
     description=(
         "Flask extension to integrate discourse content generated "
         "to docs to your website."
     ),
@@ -16,15 +16,12 @@
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "Flask>=1.0.2",
         "beautifulsoup4",
         "humanize",
         "lxml",
+        "requests",
         "python-dateutil",
         "validators",
     ],
-    tests_require=[
-        "vcrpy-unittest",
-        "httpretty",
-    ],
 )
```

### Comparing `canonicalwebteam.discourse-5.4.1/tests/fixtures/forum_mock.py` & `canonicalwebteam.discourse-5.4.2/tests/fixtures/forum_mock.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/tests/test_engage_pages.py` & `canonicalwebteam.discourse-5.4.2/tests/test_engage_pages.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/tests/test_models.py` & `canonicalwebteam.discourse-5.4.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.1/tests/test_parser.py` & `canonicalwebteam.discourse-5.4.2/tests/test_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import unittest
-from unittest.mock import MagicMock, patch
+from unittest.mock import MagicMock
 import warnings
 
 from bs4 import BeautifulSoup
 import httpretty
 import requests
 
 from canonicalwebteam.discourse.models import DiscourseAPI
 from canonicalwebteam.discourse.parsers.base_parser import BaseParser
 from canonicalwebteam.discourse.parsers.docs import DocParser
-from canonicalwebteam.discourse.parsers.tutorials import TutorialParser
 
 EXAMPLE_CONTENT = """
 <p>Some homepage content</p>
 <h2>Navigation</h2>
 
 <details>
   <summary>Navigation items</summary>
@@ -133,58 +132,14 @@
                 },
             }
         )
 
         self.assertEqual("/t/sample--text/1", parsed_topic["topic_path"])
 
 
-class TestDocParserEnsureParsed(unittest.TestCase):
-    def test_ensure_parsed(self):
-        """Ensure parsed will call parse if and only if index_topic is None."""
-        discourse_api = DiscourseAPI("https://base.url", session=MagicMock())
-
-        parser = DocParser(
-            api=discourse_api,
-            index_topic_id=1,
-            url_prefix="/",
-        )
-        with patch.object(parser, "parse", autospec=True) as mock_parse:
-            self.assertIsNone(parser.index_topic)
-            parsed_already_first = parser.ensure_parsed()
-            self.assertFalse(parsed_already_first)
-            mock_parse.assert_called_once_with()
-            mock_parse.reset_mock()
-            parser.index_topic = object()
-            parsed_already_second = parser.ensure_parsed()
-            self.assertTrue(parsed_already_second)
-            mock_parse.assert_not_called()
-
-
-class TestTutorialParser(unittest.TestCase):
-    def test_ensure_parsed(self):
-        """Ensure parsed will call parse if and only if index_topic is None."""
-        discourse_api = DiscourseAPI("https://base.url", session=MagicMock())
-
-        parser = TutorialParser(
-            api=discourse_api,
-            index_topic_id=1,
-            url_prefix="/",
-        )
-        with patch.object(parser, "parse", autospec=True) as mock_parse:
-            self.assertIsNone(parser.index_topic)
-            parsed_already_first = parser.ensure_parsed()
-            self.assertFalse(parsed_already_first)
-            mock_parse.assert_called_once_with()
-            mock_parse.reset_mock()
-            parser.index_topic = object()
-            parsed_already_second = parser.ensure_parsed()
-            self.assertTrue(parsed_already_second)
-            mock_parse.assert_not_called()
-
-
 class TestDocParser(unittest.TestCase):
     def setUp(self):
         # Suppress annoying warnings from HTTPretty
         # See: https://github.com/gabrielfalcao/HTTPretty/issues/368
         warnings.filterwarnings(
             "ignore", category=ResourceWarning, message="unclosed.*"
         )
```

