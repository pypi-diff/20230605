# Comparing `tmp/rdflib_ocdm-0.2.0.tar.gz` & `tmp/rdflib_ocdm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.2.0.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.2.1.tar", max compression
```

## Comparing `rdflib_ocdm-0.2.0.tar` & `rdflib_ocdm-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      497 2023-05-11 11:41:27.372364 rdflib_ocdm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.2.0/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.2.0/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5349 2023-04-14 08:28:09.422946 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3589 2023-05-11 10:55:37.891219 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4600 2023-04-18 15:55:19.068117 rdflib_ocdm-0.2.0/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     7604 2023-04-19 10:32:08.234267 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.2.0/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2259 2023-05-11 11:36:15.565333 rdflib_ocdm-0.2.0/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.2.0/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.2.0/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.2.0/README.md
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.0/setup.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-06-05 16:08:39.917692 rdflib_ocdm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.2.1/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.2.1/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5348 2023-06-05 21:03:43.220445 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3529 2023-06-05 21:22:26.205708 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4612 2023-06-05 21:12:44.765077 rdflib_ocdm-0.2.1/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     7604 2023-06-05 21:16:39.230517 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.2.1/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2259 2023-05-11 11:36:15.565333 rdflib_ocdm-0.2.1/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.2.1/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.2.1/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.2.1/README.md
+-rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.1/setup.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.1/PKG-INFO
```

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             raise ValueError("new_value must be a non negative integer!")
         file_path: str = self._get_prov_path()
         self.__initialize_file_if_not_existing(file_path, entity_name)
         with open(file_path, 'r', encoding='utf8') as file:
             data = json.load(file)
         with open(file_path, 'w', encoding='utf8') as outfile:
             data[entity_name] = new_value
-            outfile.write(data)
+            json.dump(obj=data, fp=outfile, ensure_ascii=False, indent=False)
 
     def read_counter(self, entity_name: str) -> int:
         """
         It allows to read the counter value of provenance entities.
 
         :param entity_name: The entity name
         :type entity_name: str
@@ -95,16 +95,15 @@
 
     def __initialize_file_if_not_existing(self, file_path: str, entity_name: str):
         entity_name = str(entity_name)
         if not os.path.exists(os.path.dirname(file_path)):
             os.makedirs(os.path.dirname(file_path))
         if not os.path.isfile(file_path):
             with open(file_path, 'w', encoding='utf8') as outfile:
-                json_object = json.dumps({entity_name: 0}, ensure_ascii=False, indent=None)
-                outfile.write(json_object)
+                json.dump({entity_name: 0}, ensure_ascii=False, indent=None, fp=outfile)
 
     def _read_number(self, file_path: str, entity_name: str) -> int:
         self.__initialize_file_if_not_existing(file_path, entity_name)
         with open(file_path, 'r', encoding='utf8') as file:
             data = json.load(file)
             if entity_name in data:
                 self.prov_files[entity_name] = data[entity_name]
```

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,12 +77,11 @@
         """
         It allows to increment the counter value of graph and provenance entities by one unit.
 
         :param entity_name: The entity name
         :type entity_name: str
         :return: The newly-updated (already incremented) counter value.
         """
-        entity_name = urllib.parse.quote(str(entity_name))
         cur_count = self.read_counter(entity_name)
         count = cur_count + 1
         self.set_counter(count, entity_name)
         return count
```

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/ocdm_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     
     def get_entity(self, res: str) -> Optional[ProvEntity]:
         return self.provenance.get_entity(res)
     
     def commit_changes(self):
         self.__merge_index = dict()
         self.__entity_index = dict()
-        self.preexisting_finished()
+        self.preexisting_graph = deepcopy(self)
     
     def get_provenance_graphs(self) -> ConjunctiveGraph:
         prov_g = ConjunctiveGraph()
         for _, prov_entity in self.provenance.res_to_entity.items():
             for triple in prov_entity.g.triples((None, None, None)):
                 prov_g.add((triple[0], triple[1], triple[2], URIRef(prov_entity.prov_subject + '/prov/')))
         return prov_g
```

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/storer.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/rdflib_ocdm/support.py` & `rdflib_ocdm-0.2.1/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/README.md` & `rdflib_ocdm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.0/setup.py` & `rdflib_ocdm-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['oc-ocdm>=7.1.7,<8.0.0', 'rdflib>=6.2.0,<7.0.0', 'sparqlwrapper>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rdflib-ocdm',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/rdflib-ocdm)\n\n# rdflib-ocdm\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdflib_ocdm-0.2.0/PKG-INFO` & `rdflib_ocdm-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

