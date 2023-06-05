# Comparing `tmp/joltedmod-0.1.1.tar.gz` & `tmp/joltedmod-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.1.1.tar", max compression
+gzip compressed data, was "joltedmod-0.1.2.tar", max compression
```

## Comparing `joltedmod-0.1.1.tar` & `joltedmod-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.1/README.md
--rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.1/jolted_mod/__init__.py
--rw-r--r--   0        0        0     2915 2023-06-01 12:57:15.756973 joltedmod-0.1.1/jolted_mod/block.py
--rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.1/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.1/jolted_mod/cell_type.py
--rw-r--r--   0        0        0     7706 2023-06-04 20:11:48.747702 joltedmod-0.1.1/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     3885 2023-06-01 13:18:22.149509 joltedmod-0.1.1/jolted_mod/main.py
--rw-r--r--   0        0        0     4116 2023-06-01 12:22:59.233432 joltedmod-0.1.1/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      649 2023-06-04 20:13:51.947283 joltedmod-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.2/README.md
+-rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.2/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     3108 2023-06-05 06:39:34.991191 joltedmod-0.1.2/jolted_mod/block.py
+-rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.2/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.2/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0      890 2023-06-05 06:48:24.698768 joltedmod-0.1.2/jolted_mod/config.py
+-rw-r--r--   0        0        0     7706 2023-06-05 06:44:15.371897 joltedmod-0.1.2/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0     3842 2023-06-05 06:48:49.065374 joltedmod-0.1.2/jolted_mod/main.py
+-rw-r--r--   0        0        0     4110 2023-06-05 06:47:46.751477 joltedmod-0.1.2/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0      649 2023-06-05 06:49:03.034665 joltedmod-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.2/PKG-INFO
```

### Comparing `joltedmod-0.1.1/LICENSE` & `joltedmod-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.1/jolted_mod/block_factory.py` & `joltedmod-0.1.2/jolted_mod/block_factory.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.1/jolted_mod/content_generator.py` & `joltedmod-0.1.2/jolted_mod/content_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,40 +33,22 @@
         if not openai.api_key:
             raise ValueError("Environment variable OPENAI_API_KEY not set")
 
     async def create_notebook(self, config_file):
         """Create a Jupyter Notebook file from the given config file."""
         nb = nbf.v4.new_notebook()
         blocks = await self.create_content(config_file)
-        await self._generate_notebook_blocks(blocks, nb)
-        return nb
-
-    async def _generate_notebook_blocks(self, blocks, nb):
-        """Generate notebook cells from given blocks asynchronously."""
-        for block in blocks:
-            if block.cell_type == CellType.CODE:
-                new_cell = nbf.v4.new_code_cell(block.content)
-                new_cell['id'] = str(uuid.uuid4())  # Generate and set cell id
-                nb.cells.append(new_cell)
-            elif block.cell_type == CellType.MARKDOWN:
-                nb.cells.append(nbf.v4.new_markdown_cell(block.content))
+        await self._generate_notebook_cells(blocks, nb)
         return nb
 
     async def create_wiki(self, config_file):
         """Create a wiki file from the given config file."""
         blocks = await self.create_content(config_file)
         return await self._create_markdown_text(blocks)
 
-    async def _create_markdown_text(self, blocks):
-        """Create a markdown file from the given blocks."""
-        markdown_text = ""
-        for block in blocks:
-            markdown_text += (block.content)
-        return markdown_text
-
     async def create_content(self, config_file):
         """Create content for blocks from the given config file asynchronously."""
         async with aiohttp.ClientSession() as self._session:
             blocks = await self._parse_config_file(config_file)
             await self._update_context(config_file, blocks)
 
             if blocks[0].type == 'SeedBlock':
@@ -74,14 +56,34 @@
                 blocks.pop(0)
             else:
                 self.system_block = None
 
             await self._generate_all_block_content(blocks)
             return blocks
 
+
+    async def _generate_notebook_cells(self, blocks, nb):
+        """Generate notebook cells from given blocks asynchronously."""
+        for block in blocks:
+            if block.cell_type == CellType.CODE:
+                new_cell = nbf.v4.new_code_cell(block.content)
+                new_cell['id'] = str(uuid.uuid4())  # Generate and set cell id
+                nb.cells.append(new_cell)
+            elif block.cell_type == CellType.MARKDOWN:
+                nb.cells.append(nbf.v4.new_markdown_cell(block.content))
+        return nb
+
+    async def _create_markdown_text(self, blocks):
+        """Create a markdown file from the given blocks."""
+        markdown_text = ""
+        for block in blocks:
+            markdown_text += (block.content)
+        return markdown_text
+
+
     @staticmethod
     async def _update_context(config_file, blocks):
         """Update block context using the given config file asynchronously."""
         async with aiofiles.open(config_file, mode='r') as f:
             config = json.loads(await f.read())
             for block, block_config in zip(blocks, config['blocks']):
                 if 'context' in block_config and block_config['context'] is not None:
```

### Comparing `joltedmod-0.1.1/jolted_mod/main.py` & `joltedmod-0.1.2/jolted_mod/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,114 @@
-import asyncio
 from jolted_mod.template_generator import TemplateGenerator
 from jolted_mod.content_generator import ContentGenerator
 from typing import Any, Dict
 
 
-async def create_notebook_module(topic: str, identity: str = 'professor of computer science',
-                                 target_audience: str = 'first year computer science students',
-                                 model: str = 'gpt-3.5-turbo') -> Dict[str, Any]:
+async def create_notebook_module(
+    topic: str,
+    identity: str = "professor of computer science",
+    target_audience: str = "first year computer science students",
+    model: str = "gpt-3.5-turbo",
+) -> Dict[str, Any]:
     """
     Creates a notebook module based on the provided topic.
 
     Args:
         topic (str): The topic for the notebook.
         identity (str): The identity of the content creator.
         target_audience (str): The target audience of the notebook.
         model (str): The AI model used for content generation.
 
     Returns:
         Dict[str, Any]: The generated notebook content.
     """
 
     if not topic:
-        raise ValueError('Topic cannot be empty')
+        raise ValueError("Topic cannot be empty")
 
     # Generate the template
     template_generator = TemplateGenerator(topic, identity, target_audience)
     tutorial_template = template_generator.save_tutorial_template_to_file(
-        'tutorial_template.json')
+        "tutorial_template.json"
+    )
 
     # Generate cell content using the ContentGenerator
     cg = ContentGenerator(model=model)
-    tutorial_content = await cg.create_notebook('tutorial_template.json')
+    tutorial_content = await cg.create_notebook("tutorial_template.json")
 
     return tutorial_content
 
 
-async def create_wiki_module(topic: str, identity: str = 'professor of computer science',
-                             target_audience: str = 'first year computer science students',
-                             model: str = 'gpt-3.5-turbo') -> str:
+async def create_wiki_module(
+    topic: str,
+    identity: str = "professor of computer science",
+    target_audience: str = "first year computer science students",
+    model: str = "gpt-3.5-turbo",
+) -> str:
     """
     Creates a wiki module based on the provided topic.
 
     Args:
         topic (str): The topic for the wiki.
         identity (str): The identity of the content creator.
         target_audience (str): The target audience of the wiki.
         model (str): The AI model used for content generation.
 
     Returns:
         str: The generated wiki content in markdown format.
     """
 
     if not topic:
-        raise ValueError('Topic cannot be empty')
+        raise ValueError("Topic cannot be empty")
 
     # Generate the template
     template_generator = TemplateGenerator(topic, identity, target_audience)
-    wiki_template = template_generator.save_wiki_template_to_file(
-        'wiki_template.json')
+    wiki_template = template_generator.save_wiki_template_to_file("wiki_template.json")
 
     # Generate cell content using the ContentGenerator
     cg = ContentGenerator(model=model)
-    wiki_content = await cg.create_wiki('wiki_template.json')
+    wiki_content = await cg.create_wiki("wiki_template.json")
 
     return wiki_content
 
 
-async def create_curriculum(curriculum_data: Dict[str, Any], identity: str = 'Professor of Computer Science',
-                            target_audience: str = 'first year computer science students',
-                            model: str = 'gpt-3.5-turbo') -> Dict[str, Any]:
+async def create_curriculum(
+    curriculum_data: Dict[str, Any],
+    identity: str = "Professor of Computer Science",
+    target_audience: str = "first year computer science students",
+    model: str = "gpt-3.5-turbo",
+) -> Dict[str, Any]:
     """
     Creates a curriculum based on the provided curriculum data.
 
     Args:
         curriculum_data (Dict[str, Any]): The curriculum data containing topics and subtopics.
         identity (str): The identity of the content creator.
         target_audience (str): The target audience of the curriculum.
         model (str): The AI model used for content generation.
 
     Returns:
         Dict[str, Any]: The generated curriculum.
     """
 
-    if 'topics' not in curriculum_data:
+    if "topics" not in curriculum_data:
         raise ValueError(
-            "The curriculum data must contain a 'topics' key with a list of topics.")
+            "The curriculum data must contain a 'topics' key with a list of topics."
+        )
 
     curriculum = {}
-    for topic_index, topic in enumerate(curriculum_data['topics']):
-        topic_name = topic['name']
+    for topic_index, topic in enumerate(curriculum_data["topics"]):
+        topic_name = topic["name"]
         topic_content = {}
-        for subtopic_index, subtopic in enumerate(topic['subtopics']):
-            tutorial_content = await create_notebook_module(subtopic, identity, target_audience, model)
-            wiki_content = await create_wiki_module(subtopic, identity, target_audience, model)
+        for subtopic_index, subtopic in enumerate(topic["subtopics"]):
+            tutorial_content = await create_notebook_module(
+                subtopic, identity, target_audience, model
+            )
+            wiki_content = await create_wiki_module(
+                subtopic, identity, target_audience, model
+            )
             topic_content[subtopic] = {
-                "tutorial": tutorial_content, "wiki": wiki_content}
+                "tutorial": tutorial_content,
+                "wiki": wiki_content,
+            }
         curriculum[topic_name] = topic_content
     return curriculum
```

### Comparing `joltedmod-0.1.1/jolted_mod/template_generator.py` & `joltedmod-0.1.2/jolted_mod/template_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     "cell_type": "MARKDOWN"
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a concrete code example that's thoroughly commented",
                     "target_audience": self.target_audience,
-                    "context": None,
+                    "context": 1,
                     "cell_type": "MARKDOWN"
                 },
                 {
                     "type": "KnowledgeTestingBlock",
                     "n": 1,
                     "question_type": "programming problem",
                     "topic": self.topic,
@@ -73,15 +73,15 @@
                     "cell_type": "MARKDOWN"
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "a concrete code example that's thoroughly commented",
                     "target_audience": self.target_audience,
-                    "context": None,
+                    "context": 1,
                     "cell_type": "MARKDOWN"
                 },
                 {
                     "type": "ExplanatoryBlock",
                     "topic": self.topic,
                     "method_of_teaching": "3 example use cases",
                     "target_audience": self.target_audience,
```

### Comparing `joltedmod-0.1.1/pyproject.toml` & `joltedmod-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.1.1"
+version = "0.1.2"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
 license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
```

### Comparing `joltedmod-0.1.1/PKG-INFO` & `joltedmod-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joltedmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: JoltEd self-documenting learning module
 License: MIT
 Author: Nathan Laundry
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

