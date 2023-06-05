# Comparing `tmp/timeitpoj-0.1.1.tar.gz` & `tmp/timeitpoj-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeitpoj-0.1.1.tar", max compression
+gzip compressed data, was "timeitpoj-0.1.2.tar", max compression
```

## Comparing `timeitpoj-0.1.1.tar` & `timeitpoj-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      242 2023-06-03 08:09:35.297704 timeitpoj-0.1.1/README.md
--rwxr-xr-x   0        0        0      284 2023-06-05 12:30:18.549762 timeitpoj-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-05 12:05:36.372834 timeitpoj-0.1.1/timeitpoj/__init__.py
--rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.1/timeitpoj/task_report.py
--rwxr-xr-x   0        0        0     8443 2023-06-05 12:24:38.309413 timeitpoj-0.1.1/timeitpoj/timeit.py
--rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.1/timeitpoj/utils/__init__.py
--rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.1/timeitpoj/utils/constants.py
--rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.1/timeitpoj/utils/misc.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 timeitpoj-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      242 2023-06-03 08:09:35.297704 timeitpoj-0.1.2/README.md
+-rwxr-xr-x   0        0        0      284 2023-06-05 12:42:10.358799 timeitpoj-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-05 12:05:36.372834 timeitpoj-0.1.2/timeitpoj/__init__.py
+-rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.2/timeitpoj/task_report.py
+-rwxr-xr-x   0        0        0     9594 2023-06-05 12:41:55.824777 timeitpoj-0.1.2/timeitpoj/timeit.py
+-rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.2/timeitpoj/utils/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.2/timeitpoj/utils/constants.py
+-rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.2/timeitpoj/utils/misc.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 timeitpoj-0.1.2/PKG-INFO
```

### Comparing `timeitpoj-0.1.1/timeitpoj/task_report.py` & `timeitpoj-0.1.2/timeitpoj/task_report.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.1/timeitpoj/timeit.py` & `timeitpoj-0.1.2/timeitpoj/timeit.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <https://www.gnu.org/licenses/>.
 #
 import time
 from distutils.util import strtobool
 import os
+from functools import wraps
 
 from timeitpoj.task_report import TaskReport
 from timeitpoj.utils.misc import random_task_name, reformat_units, time_to_str
 
 
 class InternalTimer:
     def __init__(self):
@@ -176,14 +177,32 @@
 
         duration, unit = reformat_units(generate_report_duration)
 
         print(f"[TIMEIT] report generation took {time_to_str(generate_report_duration)}")
 
         print_report_title_line()
 
+    @classmethod
+    def as_decorator(cls, name=None, include=False):
+        def decorator(func):
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                nonlocal name
+                if name is None:
+                    name = func.__name__
+                with cls(name) as timer:
+                    if include:
+                        return func(*args, timer=timer, **kwargs)
+                    else:
+                        return func(*args, **kwargs)
+
+            return wrapper
+
+        return decorator
+
     class __Timer:
         def __init__(self, name, internal_timer: InternalTimer, parent_timer=None):
             self.internal_timer = internal_timer
             self.start_time = None
             self.end_time = None
 
             self.name = name
@@ -243,12 +262,29 @@
         def start_timer(self):
             self.start_time = time.time()
 
         def register_task_end(self, task_report):
             self.current_task = None
             self.task_timers.append(task_report)
 
+        def function(self, name=None, include=False):
+            def decorator(func):
+                @wraps(func)
+                def wrapper(*args, **kwargs):
+                    nonlocal name
+                    if name is None:
+                        name = func.__name__
+                    with self(name) as timer:
+                        if include:
+                            return func(*args, timer=timer, **kwargs)
+                        else:
+                            return func(*args, **kwargs)
+
+                return wrapper
+
+            return decorator
+
         def __repr__(self):
             return self.__str__()
 
         def __str__(self):
             return f"Timer(name=[{self.name}], tasks={self.task_timers}, current_task=[{self.current_task}])"
```

### Comparing `timeitpoj-0.1.1/timeitpoj/utils/misc.py` & `timeitpoj-0.1.2/timeitpoj/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.1/PKG-INFO` & `timeitpoj-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeitpoj
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jari Van Melckebeke
 Author-email: jarivanmelckebeke@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

