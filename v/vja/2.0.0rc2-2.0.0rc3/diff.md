# Comparing `tmp/vja-2.0.0rc2.tar.gz` & `tmp/vja-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0rc2.tar", last modified: Fri Jun  2 20:48:02 2023, max compression
+gzip compressed data, was "vja-2.0.0rc3.tar", last modified: Mon Jun  5 19:00:43 2023, max compression
```

## Comparing `vja-2.0.0rc2.tar` & `vja-2.0.0rc3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.571430 vja-2.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 20:48:02.571430 vja-2.0.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-02 20:48:02.571430 vja-2.0.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-02 20:47:19.000000 vja-2.0.0rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.568430 vja-2.0.0rc2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     9956 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.570430 vja-2.0.0rc2/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17963 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3878 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     5756 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/project_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10416 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.571430 vja-2.0.0rc2/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-05 19:00:43.198216 vja-2.0.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 19:00:43.198216 vja-2.0.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-05 18:59:55.000000 vja-2.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.195471 vja-2.0.0rc3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)    10103 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17977 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5756 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/project_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0rc2/PKG-INFO` & `vja-2.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc2/setup.py` & `vja-2.0.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/tests/conftest.py` & `vja-2.0.0rc3/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 def _login_as_test_user():
     run_vja('vja logout')
     run_vja('vja --username=test --password=test user show')
 
 
 def _create_project_and_task():
     run_vja('vja project add test-project')
-    run_vja('vja project add child --parent-project-id=2')
-    run_vja('vja project add grand-child --parent-project-id=3')
-    run_vja('vja add At least one task --force-create --priority=5 --due-date=today --label=my_tag --favorite=True --project-id=1')
-    run_vja('vja add Task in subproject --force-create --project-id=4')
+    run_vja('vja project add child --parent-project=test-project')
+    run_vja('vja project add grand-child --parent-project=child')
+    run_vja('vja add At least one task --force-create --priority=5 --due-date=today --label=my_tag --favorite=True --project-id=test-project')
+    run_vja('vja add Task in subproject --force-create --project-id=grand-child')
     run_vja('vja add A task without a label --force-create')
 
 
 def run_vja(command):
     result = subprocess.run(command.split(), capture_output=True, check=False)
     if result.returncode:
         print(f'!!! Non-zero result ({result.returncode}) from command {command}')
```

### Comparing `vja-2.0.0rc2/tests/test_basic.py` & `vja-2.0.0rc3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/tests/test_command.py` & `vja-2.0.0rc3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/tests/test_query.py` & `vja-2.0.0rc3/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,16 @@
         assert len(data) == 0
 
     def test_task_filter_base_project(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--base-project=test-project'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all(i['project']['title'] == 'test-project' or i['project']['title'] == 'grand-child' for i in data)
+        assert any(i['project']['title'] == 'test-project' for i in data)
+        assert any(i['project']['title'] == 'grand-child' for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--project=Not created'])
         data = json.loads(res.output)
         assert len(data) == 0
 
     def test_task_filter_priority(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--priority=eq 5'])
         data = json.loads(res.output)
@@ -185,15 +187,15 @@
         assert len(data) > 0
         assert all(i['priority'] > 4 for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--priority=gt 5'])
         data = json.loads(res.output)
         assert len(data) == 0
 
     def test_task_filter_title(self, runner):
-        res = invoke(runner, ['ls', '--jsonvja', '--title=At least one'])
+        res = invoke(runner, ['ls', '--jsonvja', '--title=at least one'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all('At least one task' in i['title'] for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--title=Not created'])
         data = json.loads(res.output)
         assert len(data) == 0
```

### Comparing `vja-2.0.0rc2/vja/apiclient.py` & `vja-2.0.0rc3/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/authenticate.py` & `vja-2.0.0rc3/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/cli.py` & `vja-2.0.0rc3/vja/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,20 +96,20 @@
 # projects
 @cli.group('project', help='Subcommand: project (see help)')
 def project_group():
     pass
 
 
 @project_group.command('add', help='Add project with title')
-@click.option('parent_project_id', '-o', '--parent-project-id', '--parent_project_id', type=click.INT,
-              help='Create project as child of parent project id')
+@click.option('parent_project', '-o', '--parent-project', '--parent_project',
+              help='Create project as child of parent project. May be given by id or title of parent-project.')
 @click.argument('title', nargs=-1, required=True)
 @with_application
-def project_add(application, title, parent_project_id=None):
-    project = application.command_service.add_project(parent_project_id, " ".join(title))
+def project_add(application, title, parent_project=None):
+    project = application.command_service.add_project(parent_project, " ".join(title))
     click.echo(f'Created project {project.id}')
 
 
 @project_group.command('ls', help='Print projects ... (id; title; description; parent_project_id)')
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
```

### Comparing `vja-2.0.0rc2/vja/config.py` & `vja-2.0.0rc3/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/filter.py` & `vja-2.0.0rc3/vja/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def _create_upper_project_filter(value):
     if str(value).isdigit():
         return lambda x: x.project.id == int(value) or any(ancestor.id == int(value) for ancestor in x.project.ancestor_projects)
     return lambda x: x.project.title == value or any(ancestor.title == value for ancestor in x.project.ancestor_projects)
 
 
 def _create_title_filter(value):
-    return lambda x: bool(re.search(re.compile(value), x.title))
+    return lambda x: bool(re.search(re.compile(value, re.IGNORECASE), x.title))
 
 
 def _create_priority_filter(value):
     return _create_general_filter([f'priority {value}'])
 
 
 def _create_urgency_filter(value):
```

### Comparing `vja-2.0.0rc2/vja/model.py` & `vja-2.0.0rc3/vja/model.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/output.py` & `vja-2.0.0rc3/vja/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 BUCKET_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20} {x.is_done_bucket:2} {x.limit:3} {x.count_tasks:5}'
 
 LABEL_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20}'
 
 TASK_LIST_FORMAT_DEFAULT = '{x.id:5} ({x.priority}) {"*" if x.is_favorite else " "} {x.title:50.50} ' \
                            '{x.due_date.strftime("%a %d.%m %H:%M") if x.due_date else "":15.15} ' \
-                           '{"R" if x.reminders else " "} {x.project.title:20.20} ' \
-                           '{x.labels:20.20} {x.urgency:3.1f}'
+                           '{"A" if x.reminders else " "}{"R" if x.repeat_after else " "}{"D" if x.description else " "} ' \
+                           '{x.project.title:20.20} {x.labels:20.20} {x.urgency:3.1f}'
 
 logger = logging.getLogger(__name__)
 
 
 class Output:
 
     def user(self, user: User, is_json, is_jsonvja):
```

### Comparing `vja-2.0.0rc2/vja/parse.py` & `vja-2.0.0rc3/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/project_service.py` & `vja-2.0.0rc3/vja/project_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/service_command.py` & `vja-2.0.0rc3/vja/service_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 
 from vja import VjaError
 from vja.apiclient import ApiClient
-from vja.model import Label
+from vja.model import Label, Project
 from vja.parse import parse_date_arg_to_iso, parse_json_date, parse_date_arg_to_timedelta, datetime_to_isoformat
 from vja.project_service import ProjectService
 from vja.task_service import TaskService
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,17 +21,24 @@
         self._api_client.authenticate(True, username, password, totp_passcode)
 
     def logout(self):
         self._api_client.logout()
         logger.info('Logged out')
 
     # project
-    def add_project(self, parent_project_id, title):
+    def add_project(self, parent_project, title):
+        if parent_project:
+            if str(parent_project).isdigit():
+                parent_project_id = parent_project
+            else:
+                parent_project_id = self._project_service.find_project_by_title(parent_project).id
+        else:
+            parent_project_id = None
         project_json = self._api_client.put_project(parent_project_id, title)
-        return self._project_service.find_project_by_id(project_json['id'])
+        return Project.from_json(project_json, [])
 
     # label
     def add_label(self, title):
         label_json = self._api_client.put_label(title)
         return Label.from_json(label_json)
 
     # tasks
```

### Comparing `vja-2.0.0rc2/vja/service_query.py` & `vja-2.0.0rc3/vja/service_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/task_service.py` & `vja-2.0.0rc3/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja/urgency.py` & `vja-2.0.0rc3/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc2/vja.egg-info/PKG-INFO` & `vja-2.0.0rc3/vja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc2/vja.egg-info/SOURCES.txt` & `vja-2.0.0rc3/vja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

