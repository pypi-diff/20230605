# Comparing `tmp/joltedmod-0.1.2.tar.gz` & `tmp/joltedmod-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.1.2.tar", max compression
+gzip compressed data, was "joltedmod-0.1.3.tar", max compression
```

## Comparing `joltedmod-0.1.2.tar` & `joltedmod-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.2/README.md
--rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.2/jolted_mod/__init__.py
--rw-r--r--   0        0        0     3108 2023-06-05 06:39:34.991191 joltedmod-0.1.2/jolted_mod/block.py
--rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.2/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.2/jolted_mod/cell_type.py
--rw-r--r--   0        0        0      890 2023-06-05 06:48:24.698768 joltedmod-0.1.2/jolted_mod/config.py
--rw-r--r--   0        0        0     7706 2023-06-05 06:44:15.371897 joltedmod-0.1.2/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     3842 2023-06-05 06:48:49.065374 joltedmod-0.1.2/jolted_mod/main.py
--rw-r--r--   0        0        0     4110 2023-06-05 06:47:46.751477 joltedmod-0.1.2/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      649 2023-06-05 06:49:03.034665 joltedmod-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.3/README.md
+-rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.3/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     3108 2023-06-05 06:39:34.991191 joltedmod-0.1.3/jolted_mod/block.py
+-rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.3/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.3/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0      890 2023-06-05 06:48:24.698768 joltedmod-0.1.3/jolted_mod/config.py
+-rw-r--r--   0        0        0     7706 2023-06-05 06:44:15.371897 joltedmod-0.1.3/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0     4014 2023-06-05 07:00:49.244856 joltedmod-0.1.3/jolted_mod/main.py
+-rw-r--r--   0        0        0     7264 2023-06-05 07:04:40.600941 joltedmod-0.1.3/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0      649 2023-06-05 07:07:18.545347 joltedmod-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.3/PKG-INFO
```

### Comparing `joltedmod-0.1.2/LICENSE` & `joltedmod-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.2/jolted_mod/block.py` & `joltedmod-0.1.3/jolted_mod/block.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.2/jolted_mod/block_factory.py` & `joltedmod-0.1.3/jolted_mod/block_factory.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.2/jolted_mod/config.py` & `joltedmod-0.1.3/jolted_mod/config.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.2/jolted_mod/content_generator.py` & `joltedmod-0.1.3/jolted_mod/content_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.2/jolted_mod/main.py` & `joltedmod-0.1.3/jolted_mod/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict
 
 
 async def create_notebook_module(
     topic: str,
     identity: str = "professor of computer science",
     target_audience: str = "first year computer science students",
+    is_code: bool = True,
     model: str = "gpt-3.5-turbo",
 ) -> Dict[str, Any]:
     """
     Creates a notebook module based on the provided topic.
 
     Args:
         topic (str): The topic for the notebook.
@@ -23,29 +24,30 @@
     """
 
     if not topic:
         raise ValueError("Topic cannot be empty")
 
     # Generate the template
     template_generator = TemplateGenerator(topic, identity, target_audience)
-    tutorial_template = template_generator.save_tutorial_template_to_file(
-        "tutorial_template.json"
+    tutorial_template = template_generator.save_template_to_file(
+        "tutorial_template.json", code=is_code, template_type="notebook"
     )
 
     # Generate cell content using the ContentGenerator
     cg = ContentGenerator(model=model)
     tutorial_content = await cg.create_notebook("tutorial_template.json")
 
     return tutorial_content
 
 
 async def create_wiki_module(
     topic: str,
     identity: str = "professor of computer science",
     target_audience: str = "first year computer science students",
+    is_code: bool = True,
     model: str = "gpt-3.5-turbo",
 ) -> str:
     """
     Creates a wiki module based on the provided topic.
 
     Args:
         topic (str): The topic for the wiki.
@@ -58,27 +60,30 @@
     """
 
     if not topic:
         raise ValueError("Topic cannot be empty")
 
     # Generate the template
     template_generator = TemplateGenerator(topic, identity, target_audience)
-    wiki_template = template_generator.save_wiki_template_to_file("wiki_template.json")
+    wiki_template = template_generator.save_template_to_file(
+        "wiki_template.json", code=is_code, template_type="wiki"
+    )
 
     # Generate cell content using the ContentGenerator
     cg = ContentGenerator(model=model)
     wiki_content = await cg.create_wiki("wiki_template.json")
 
     return wiki_content
 
 
 async def create_curriculum(
     curriculum_data: Dict[str, Any],
     identity: str = "Professor of Computer Science",
     target_audience: str = "first year computer science students",
+    is_code: bool = True,
     model: str = "gpt-3.5-turbo",
 ) -> Dict[str, Any]:
     """
     Creates a curriculum based on the provided curriculum data.
 
     Args:
         curriculum_data (Dict[str, Any]): The curriculum data containing topics and subtopics.
@@ -97,18 +102,18 @@
 
     curriculum = {}
     for topic_index, topic in enumerate(curriculum_data["topics"]):
         topic_name = topic["name"]
         topic_content = {}
         for subtopic_index, subtopic in enumerate(topic["subtopics"]):
             tutorial_content = await create_notebook_module(
-                subtopic, identity, target_audience, model
+                subtopic, identity, target_audience, is_code, model
             )
             wiki_content = await create_wiki_module(
-                subtopic, identity, target_audience, model
+                subtopic, identity, target_audience, is_code, model
             )
             topic_content[subtopic] = {
                 "tutorial": tutorial_content,
                 "wiki": wiki_content,
             }
         curriculum[topic_name] = topic_content
     return curriculum
```

### Comparing `joltedmod-0.1.2/jolted_mod/template_generator.py` & `joltedmod-0.1.3/jolted_mod/template_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,192 @@
 import json
 
 
 class TemplateGenerator:
-
     def __init__(self, topic, identity, target_audience):
         self.topic = topic
         self.identity = identity
         self.target_audience = target_audience
 
-    def generate_tutorial_template(self):
+    def generate_tutorial_code_template(self):
         template = {
             "blocks": [
                 {
                     "type": "SeedBlock",
                     "identity": self.identity,
                     "topic": self.topic,
-                    "target_audience": self.target_audience
+                    "target_audience": self.target_audience,
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a metaphor without code",
                     "target_audience": self.target_audience,
                     "context": None,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a concrete code example that's thoroughly commented",
                     "target_audience": self.target_audience,
                     "context": 1,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "KnowledgeTestingBlock",
                     "n": 1,
                     "question_type": "programming problem",
                     "topic": self.topic,
                     "target_audience": self.target_audience,
                     "context": None,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "KnowledgeTestingBlock",
                     "n": 1,
                     "question_type": "programming problem",
                     "topic": self.topic,
                     "target_audience": self.target_audience,
                     "cell_type": "CODE",
-                    "context": 3
-                }
+                    "context": 3,
+                },
             ]
         }
         return template
 
-    def generate_wiki_template(self):
+    def generate_wiki_code_template(self):
         template = {
             "blocks": [
                 {
                     "type": "SeedBlock",
                     "identity": self.identity,
                     "topic": self.topic,
-                    "target_audience": self.target_audience
+                    "target_audience": self.target_audience,
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a metaphor without code",
                     "target_audience": self.target_audience,
                     "context": None,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a concrete code example that's thoroughly commented",
                     "target_audience": self.target_audience,
                     "context": 1,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "3 example use cases",
                     "target_audience": self.target_audience,
                     "context": None,
-                    "cell_type": "MARKDOWN"
+                    "cell_type": "MARKDOWN",
                 },
                 {
                     "type": "KnowledgeTestingBlock",
                     "n": 5,
                     "question_type": "multiple choice",
                     "topic": self.topic,
                     "target_audience": self.target_audience,
                     "context": None,
-                    "cell_type": "MARKDOWN"
-                }
+                    "cell_type": "MARKDOWN",
+                },
             ]
         }
         return template
 
-    def save_tutorial_template_to_file(self, file_path):
-        template = self.generate_tutorial_template()
-        with open(file_path, 'w') as f:
-            json.dump(template, f, indent=2)
+    def generate_tutorial_noncode_template(self):
+        template = {
+            "blocks": [
+                {
+                    "type": "SeedBlock",
+                    "identity": self.identity,
+                    "topic": self.topic,
+                    "target_audience": self.target_audience,
+                },
+                {
+                    "type": "ExplanatoryBlock",
+                    "topic": self.topic,
+                    "method_of_teaching": "a metaphor",
+                    "target_audience": self.target_audience,
+                    "context": None,
+                    "cell_type": "MARKDOWN",
+                },
+                {
+                    "type": "ExplanatoryBlock",
+                    "topic": self.topic,
+                    "method_of_teaching": "a concrete example that's thoroughly explained based on the previous metaphor",
+                    "target_audience": self.target_audience,
+                    "context": 1,
+                    "cell_type": "MARKDOWN",
+                },
+                {
+                    "type": "KnowledgeTestingBlock",
+                    "n": 1,
+                    "question_type": "essay question",
+                    "topic": self.topic,
+                    "target_audience": self.target_audience,
+                    "context": None,
+                    "cell_type": "MARKDOWN",
+                },
+            ]
+        }
+        return template
+
+    def generate_wiki_noncode_template(self):
+        template = {
+            "blocks": [
+                {
+                    "type": "SeedBlock",
+                    "identity": self.identity,
+                    "topic": self.topic,
+                    "target_audience": self.target_audience,
+                },
+                {
+                    "type": "ExplanatoryBlock",
+                    "topic": self.topic,
+                    "method_of_teaching": "a metaphor",
+                    "target_audience": self.target_audience,
+                    "context": None,
+                    "cell_type": "MARKDOWN",
+                },
+                {
+                    "type": "ExplanatoryBlock",
+                    "topic": self.topic,
+                    "method_of_teaching": "a concrete example that's thoroughly explained based on the previous metaphor",
+                    "target_audience": self.target_audience,
+                    "context": 1,
+                    "cell_type": "MARKDOWN",
+                },
+                {
+                    "type": "KnowledgeTestingBlock",
+                    "n": 1,
+                    "question_type": "essay question",
+                    "topic": self.topic,
+                    "target_audience": self.target_audience,
+                    "context": None,
+                    "cell_type": "MARKDOWN",
+                },
+            ]
+        }
+        return template
+
+    def save_template_to_file(self, file_path, code=True, template_type="notebook"):
+        if code:
+            if template_type == "notebook":
+                template = self.generate_tutorial_code_template()
+            elif template_type == "wiki":
+                template = self.generate_wiki_code_template()
+        else:
+            if template_type == "notebook":
+                template = self.generate_tutorial_noncode_template()
+            elif template_type == "wiki":
+                template = self.generate_wiki_noncode_template()
 
-    def save_wiki_template_to_file(self, file_path):
-        template = self.generate_wiki_template()
-        with open(file_path, 'w') as f:
+        with open(file_path, "w") as f:
             json.dump(template, f, indent=2)
```

### Comparing `joltedmod-0.1.2/pyproject.toml` & `joltedmod-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.1.2"
+version = "0.1.3"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
 license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
```

### Comparing `joltedmod-0.1.2/PKG-INFO` & `joltedmod-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joltedmod
-Version: 0.1.2
+Version: 0.1.3
 Summary: JoltEd self-documenting learning module
 License: MIT
 Author: Nathan Laundry
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

