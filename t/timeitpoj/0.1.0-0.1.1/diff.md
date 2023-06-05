# Comparing `tmp/timeitpoj-0.1.0.tar.gz` & `tmp/timeitpoj-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeitpoj-0.1.0.tar", max compression
+gzip compressed data, was "timeitpoj-0.1.1.tar", max compression
```

## Comparing `timeitpoj-0.1.0.tar` & `timeitpoj-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      242 2023-06-03 08:09:35.297704 timeitpoj-0.1.0/README.md
--rwxr-xr-x   0        0        0      284 2023-06-05 12:17:24.511204 timeitpoj-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-05 12:05:36.372834 timeitpoj-0.1.0/timeitpoj/__init__.py
--rwxr-xr-x   0        0        0     4514 2023-06-03 10:40:22.974268 timeitpoj-0.1.0/timeitpoj/task_report.py
--rwxr-xr-x   0        0        0     8423 2023-06-03 08:09:35.298285 timeitpoj-0.1.0/timeitpoj/timeit.py
--rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.0/timeitpoj/utils/__init__.py
--rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.0/timeitpoj/utils/constants.py
--rwxr-xr-x   0        0        0     1131 2023-06-03 08:09:35.298660 timeitpoj-0.1.0/timeitpoj/utils/misc.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 timeitpoj-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      242 2023-06-03 08:09:35.297704 timeitpoj-0.1.1/README.md
+-rwxr-xr-x   0        0        0      284 2023-06-05 12:30:18.549762 timeitpoj-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-05 12:05:36.372834 timeitpoj-0.1.1/timeitpoj/__init__.py
+-rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.1/timeitpoj/task_report.py
+-rwxr-xr-x   0        0        0     8443 2023-06-05 12:24:38.309413 timeitpoj-0.1.1/timeitpoj/timeit.py
+-rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.1/timeitpoj/utils/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.1/timeitpoj/utils/constants.py
+-rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.1/timeitpoj/utils/misc.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 timeitpoj-0.1.1/PKG-INFO
```

### Comparing `timeitpoj-0.1.0/timeitpoj/task_report.py` & `timeitpoj-0.1.1/timeitpoj/task_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
-from utils import constants
-from utils.misc import reformat_units, format_percentage, time_to_str
+from timeitpoj.utils import constants
+from timeitpoj.utils.misc import reformat_units, format_percentage, time_to_str
 
 PADDING_SECONDS = len("seconds")
 
 
 class TaskReport:
     def __init__(self,
                  name: str,
```

### Comparing `timeitpoj-0.1.0/timeitpoj/timeit.py` & `timeitpoj-0.1.1/timeitpoj/timeit.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <https://www.gnu.org/licenses/>.
 #
 import time
 from distutils.util import strtobool
 import os
 
-from task_report import TaskReport
-from utils.misc import random_task_name, reformat_units, time_to_str
+from timeitpoj.task_report import TaskReport
+from timeitpoj.utils.misc import random_task_name, reformat_units, time_to_str
 
 
 class InternalTimer:
     def __init__(self):
         self.start_time = None
         self.end_time = None
```

### Comparing `timeitpoj-0.1.0/timeitpoj/utils/misc.py` & `timeitpoj-0.1.1/timeitpoj/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from utils import constants
+from timeitpoj.utils import constants
 
 
 def reformat_units(value: float, start_unit="seconds"):
     unit_order = ["seconds", "milliseconds", "microseconds", "nanoseconds"]
     unit_index = unit_order.index(start_unit)
 
     while value < 0.1 and unit_index < len(unit_order) - 1:
```

### Comparing `timeitpoj-0.1.0/PKG-INFO` & `timeitpoj-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeitpoj
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Jari Van Melckebeke
 Author-email: jarivanmelckebeke@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

