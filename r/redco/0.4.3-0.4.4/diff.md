# Comparing `tmp/redco-0.4.3.tar.gz` & `tmp/redco-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.3.tar", last modified: Mon May 29 23:46:07 2023, max compression
+gzip compressed data, was "redco-0.4.4.tar", last modified: Mon Jun  5 13:15:21 2023, max compression
```

## Comparing `redco-0.4.3.tar` & `redco-0.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.3/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-29 23:46:07.370000 redco-0.4.3/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.3/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.360000 redco-0.4.3/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.3/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.3/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5546 2023-05-29 00:52:43.000000 redco-0.4.3/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.3/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.3/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4274 2023-05-29 01:02:59.000000 redco-0.4.3/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.3/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.3/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12139 2023-05-29 01:12:09.000000 redco-0.4.3/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.3/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.360000 redco-0.4.3/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-29 23:46:06.000000 redco-0.4.3/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-29 23:46:06.000000 redco-0.4.3/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-29 23:46:07.370000 redco-0.4.3/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-29 23:46:04.000000 redco-0.4.3/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.4/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-05 13:15:21.670000 redco-0.4.4/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.4/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.4/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.4/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.4/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5546 2023-05-29 00:52:43.000000 redco-0.4.4/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.4/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.4/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.4/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4263 2023-06-02 00:28:54.000000 redco-0.4.4/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.4/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.670000 redco-0.4.4/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.4/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12128 2023-06-02 00:28:54.000000 redco-0.4.4/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.4/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-05 13:15:21.660000 redco-0.4.4/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-06-05 13:15:21.000000 redco-0.4.4/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-06-05 13:15:21.670000 redco-0.4.4/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-06-05 13:12:00.000000 redco-0.4.4/setup.py
```

### Comparing `redco-0.4.3/LICENSE` & `redco-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/PKG-INFO` & `redco-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.3
+Version: 0.4.4
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.3/README.md` & `redco-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/__init__.py` & `redco-0.4.4/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/datasets/__init__.py` & `redco-0.4.4/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/datasets/dataset.py` & `redco-0.4.4/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/datasets/jsonl_dataset.py` & `redco-0.4.4/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/__init__.py` & `redco-0.4.4/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/data_utils.py` & `redco-0.4.4/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/deployer.py` & `redco-0.4.4/redco/deployers/deployer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/log_utils.py` & `redco-0.4.4/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.4/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.4/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.4/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/deployers/opt_utils.py` & `redco-0.4.4/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/predictors/__init__.py` & `redco-0.4.4/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/predictors/predictor.py` & `redco-0.4.4/redco/predictors/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from functools import partial
 import numpy as np
-
 import jax
 from jax.experimental.pjit import pjit
-from jax.experimental.pjit import PartitionSpec as P
+from jax.sharding import PartitionSpec as P
 from flax.core.frozen_dict import freeze
-
 from .utils import \
     add_idxes, collate_fn_wrapper, pred_fn_wrapper, default_output_fn
 
 
 class Predictor:
     def __init__(self,
                  deployer,
```

### Comparing `redco-0.4.3/redco/predictors/utils.py` & `redco-0.4.4/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/trainers/__init__.py` & `redco-0.4.4/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco/trainers/trainer.py` & `redco-0.4.4/redco/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from functools import partial
 import json
 import numpy as np
-
 import jax
 from jax.experimental.pjit import pjit
-from jax.experimental.pjit import PartitionSpec as P
+from jax.sharding import PartitionSpec as P
 from flax.jax_utils import replicate
 from flax.training.train_state import TrainState
 from flax.traverse_util import flatten_dict
 from flax.core.frozen_dict import freeze
-
 from .utils import default_train_step, default_eval_step
 from ..predictors import Predictor
 
 
 class Trainer:
     def __init__(self,
                  deployer,
```

### Comparing `redco-0.4.3/redco/trainers/utils.py` & `redco-0.4.4/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/redco.egg-info/PKG-INFO` & `redco-0.4.4/redco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.3
+Version: 0.4.4
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.3/redco.egg-info/SOURCES.txt` & `redco-0.4.4/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.3/setup.py` & `redco-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.3",
+    version="0.4.4",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

