# Comparing `tmp/purplecaffeine-0.1.0.tar.gz` & `tmp/purplecaffeine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purplecaffeine-0.1.0.tar", last modified: Fri May 19 19:15:18 2023, max compression
+gzip compressed data, was "purplecaffeine-0.1.1.tar", last modified: Mon Jun  5 16:55:27 2023, max compression
```

## Comparing `purplecaffeine-0.1.0.tar` & `purplecaffeine-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.142857 purplecaffeine-0.1.0/purplecaffeine/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.146857 purplecaffeine-0.1.0/purplecaffeine/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/helpers/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.146857 purplecaffeine-0.1.0/purplecaffeine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/purplecaffeine/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.146857 purplecaffeine-0.1.0/purplecaffeine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-19 19:15:18.000000 purplecaffeine-0.1.0/purplecaffeine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-19 19:15:18.000000 purplecaffeine-0.1.0/purplecaffeine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:15:18.000000 purplecaffeine-0.1.0/purplecaffeine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-19 19:15:18.000000 purplecaffeine-0.1.0/purplecaffeine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 19:15:18.000000 purplecaffeine-0.1.0/purplecaffeine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/helpers/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/test_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:18.150857 purplecaffeine-0.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 19:15:08.000000 purplecaffeine-0.1.0/tests/utils/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/helpers/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/purplecaffeine/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/purplecaffeine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 16:55:26.000000 purplecaffeine-0.1.1/purplecaffeine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:55:27.025554 purplecaffeine-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/helpers/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/test_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:27.021554 purplecaffeine-0.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 16:55:19.000000 purplecaffeine-0.1.1/tests/utils/test_json.py
```

### Comparing `purplecaffeine-0.1.0/PKG-INFO` & `purplecaffeine-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.1.0
+Version: 0.1.1
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -26,15 +26,15 @@
 
 ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
 [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
 [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/IceKhan13/purplecaffeine/blob/main/LICENSE)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
 
-![Logo](./docs/images/readme_logo.png)
+![Logo](https://raw.githubusercontent.com/IceKhan13/purplecaffeine/main/docs/images/readme_logo.png)
 
 Tracking experiments and programs is known problem in scientific community.
 This project is aimed to create simple general interface to track quantum experiments, store and search them in an easy way.
 
 ### Table of Contents
 
 ##### For Users
@@ -53,26 +53,26 @@
 ### Quickstart
 
 ```python
 from qiskit.circuit.random import random_circuit
 from qiskit.quantum_info.random import random_pauli
 from qiskit.primitives import Estimator
 
-from purplecaffeine.core import Trial, LocalBackend
+from purplecaffeine.core import Trial, LocalStorage
 
 n_qubits = 4
 depth = 3
 shots = 2000
 
 circuit = random_circuit(n_qubits, depth)
 obs = random_pauli(n_qubits)
 
-local_backend = LocalBackend("./")
+local_storage = LocalStorage("./")
 
-with Trial("Example trial", backend=local_backend) as trial:
+with Trial("Example trial", storage=local_storage) as trial:
     # track some parameters
     trial.add_parameter("estimator", "qiskit.primitives.Estimator")
     trial.add_parameter("depth", depth)
     trial.add_parameter("n_qubits", n_qubits)
     trial.add_parameter("shots", shots)
     
     # track objects of interest
```

### Comparing `purplecaffeine-0.1.0/README.md` & `purplecaffeine-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
 [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
 [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/IceKhan13/purplecaffeine/blob/main/LICENSE)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
 
-![Logo](./docs/images/readme_logo.png)
+![Logo](https://raw.githubusercontent.com/IceKhan13/purplecaffeine/main/docs/images/readme_logo.png)
 
 Tracking experiments and programs is known problem in scientific community.
 This project is aimed to create simple general interface to track quantum experiments, store and search them in an easy way.
 
 ### Table of Contents
 
 ##### For Users
@@ -30,26 +30,26 @@
 ### Quickstart
 
 ```python
 from qiskit.circuit.random import random_circuit
 from qiskit.quantum_info.random import random_pauli
 from qiskit.primitives import Estimator
 
-from purplecaffeine.core import Trial, LocalBackend
+from purplecaffeine.core import Trial, LocalStorage
 
 n_qubits = 4
 depth = 3
 shots = 2000
 
 circuit = random_circuit(n_qubits, depth)
 obs = random_pauli(n_qubits)
 
-local_backend = LocalBackend("./")
+local_storage = LocalStorage("./")
 
-with Trial("Example trial", backend=local_backend) as trial:
+with Trial("Example trial", storage=local_storage) as trial:
     # track some parameters
     trial.add_parameter("estimator", "qiskit.primitives.Estimator")
     trial.add_parameter("depth", depth)
     trial.add_parameter("n_qubits", n_qubits)
     trial.add_parameter("shots", shots)
     
     # track objects of interest
```

### Comparing `purplecaffeine-0.1.0/purplecaffeine/helpers/conf.py` & `purplecaffeine-0.1.1/purplecaffeine/helpers/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,25 @@
 from typing import List, Any
 
 
 class Configuration:
     """Configuration list."""
 
     MAX_SIZE: float = 5e6
-    API_HTTP: str = "http"
-    API_URL: str = "127.0.0.1"
-    API_PORT: str = "8000"
     API_TRIAL_ENDPOINT: str = "api/trials"
-    API_FULL_URL: str = f"{API_HTTP}://{API_URL}:{API_PORT}/{API_TRIAL_ENDPOINT}"
+    API_TOKEN_ENDPOINT: str = "api/token"
     API_HEADERS: dict = {
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     API_TIMEOUT: int = 30
 
     @classmethod
     def all(cls) -> List[Any]:
         """Returns all Configurations."""
         return [
             Configuration.MAX_SIZE,
-            Configuration.API_HTTP,
-            Configuration.API_URL,
-            Configuration.API_PORT,
             Configuration.API_TRIAL_ENDPOINT,
-            Configuration.API_FULL_URL,
+            Configuration.API_TOKEN_ENDPOINT,
             Configuration.API_HEADERS,
             Configuration.API_TIMEOUT,
         ]
```

### Comparing `purplecaffeine-0.1.0/purplecaffeine/utils/json.py` & `purplecaffeine-0.1.1/purplecaffeine/utils/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 
 
 # pylint: disable=no-else-return, import-outside-toplevel, cyclic-import
 class TrialEncoder(RuntimeEncoder):
     """Json encoder for trial."""
 
     def default(self, obj: Any) -> Any:
-        from purplecaffeine.core import BaseBackend
+        from purplecaffeine.core import BaseStorage
 
         if isinstance(obj, Backend):
             return {
                 "__type__": "Backend",
                 "__value__": pickle.dumps(obj),
             }
-        elif isinstance(obj, BaseBackend):
-            return {"__type__": "PurpleCaffeineBackend"}
+        elif isinstance(obj, BaseStorage):
+            return {"__type__": "PurpleCaffeineStorage"}
         return super().default(obj)
 
 
 class TrialDecoder(RuntimeDecoder):
     """Json decoder for trial."""
 
     def object_hook(self, obj: Any) -> Any:
         if "__type__" in obj:
             obj_type = obj["__type__"]
 
             if obj_type == "Backend":
                 return pickle.loads(obj["__value__"])
-            elif obj_type == "PurpleCaffeineBackend":
+            elif obj_type == "PurpleCaffeineStorage":
                 # we should not recover trial backend
                 return None
             return super().object_hook(obj)
         return obj
```

### Comparing `purplecaffeine-0.1.0/purplecaffeine.egg-info/PKG-INFO` & `purplecaffeine-0.1.1/purplecaffeine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.1.0
+Version: 0.1.1
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -26,15 +26,15 @@
 
 ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
 [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
 [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/IceKhan13/purplecaffeine/blob/main/LICENSE)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
 
-![Logo](./docs/images/readme_logo.png)
+![Logo](https://raw.githubusercontent.com/IceKhan13/purplecaffeine/main/docs/images/readme_logo.png)
 
 Tracking experiments and programs is known problem in scientific community.
 This project is aimed to create simple general interface to track quantum experiments, store and search them in an easy way.
 
 ### Table of Contents
 
 ##### For Users
@@ -53,26 +53,26 @@
 ### Quickstart
 
 ```python
 from qiskit.circuit.random import random_circuit
 from qiskit.quantum_info.random import random_pauli
 from qiskit.primitives import Estimator
 
-from purplecaffeine.core import Trial, LocalBackend
+from purplecaffeine.core import Trial, LocalStorage
 
 n_qubits = 4
 depth = 3
 shots = 2000
 
 circuit = random_circuit(n_qubits, depth)
 obs = random_pauli(n_qubits)
 
-local_backend = LocalBackend("./")
+local_storage = LocalStorage("./")
 
-with Trial("Example trial", backend=local_backend) as trial:
+with Trial("Example trial", storage=local_storage) as trial:
     # track some parameters
     trial.add_parameter("estimator", "qiskit.primitives.Estimator")
     trial.add_parameter("depth", depth)
     trial.add_parameter("n_qubits", n_qubits)
     trial.add_parameter("shots", shots)
     
     # track objects of interest
```

### Comparing `purplecaffeine-0.1.0/purplecaffeine.egg-info/SOURCES.txt` & `purplecaffeine-0.1.1/purplecaffeine.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 README.md
 setup.py
 purplecaffeine/__init__.py
 purplecaffeine/core.py
+purplecaffeine/exception.py
 purplecaffeine.egg-info/PKG-INFO
 purplecaffeine.egg-info/SOURCES.txt
 purplecaffeine.egg-info/dependency_links.txt
 purplecaffeine.egg-info/requires.txt
 purplecaffeine.egg-info/top_level.txt
 purplecaffeine/helpers/__init__.py
 purplecaffeine/helpers/conf.py
 purplecaffeine/utils/__init__.py
 purplecaffeine/utils/json.py
 tests/__init__.py
-tests/test_backend.py
+tests/test_storage.py
 tests/test_trial.py
 tests/helpers/__init__.py
 tests/helpers/test_conf.py
 tests/utils/__init__.py
 tests/utils/test_json.py
```

### Comparing `purplecaffeine-0.1.0/setup.py` & `purplecaffeine-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.1.0/tests/helpers/test_conf.py` & `purplecaffeine-0.1.1/tests/helpers/test_conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,16 @@
 class TestConf(TestCase):
     """TestConf."""
 
     def test_conf(self):
         """Test conf access variables."""
         self.assertTrue(isinstance(Configuration.MAX_SIZE, float))
         self.assertTrue(Configuration.MAX_SIZE > 1000000)
-        self.assertTrue(Configuration.API_HTTP == "http")
-        self.assertTrue(Configuration.API_URL == "127.0.0.1")
-        self.assertTrue(Configuration.API_PORT == "8000")
         self.assertTrue(Configuration.API_TRIAL_ENDPOINT == "api/trials")
-        self.assertTrue(
-            Configuration.API_FULL_URL == "http://127.0.0.1:8000/api/trials"
-        )
+        self.assertTrue(Configuration.API_TOKEN_ENDPOINT == "api/token")
         self.assertTrue(
             Configuration.API_HEADERS
             == {"Accept": "application/json", "Content-Type": "application/json"}
         )
         self.assertTrue(Configuration.API_TIMEOUT == 30)
 
         self.assertTrue(isinstance(Configuration.all(), list))
```

### Comparing `purplecaffeine-0.1.0/tests/test_trial.py` & `purplecaffeine-0.1.1/tests/test_trial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Tests for Trial."""
 import os
 import shutil
 from pathlib import Path
 from typing import Optional
-from unittest import TestCase, skip
+from unittest import TestCase
 
 import numpy as np
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import XGate
 from qiskit.quantum_info import Operator
 
-from purplecaffeine import Trial, LocalBackend, ApiBackend, BaseBackend as TrialBackend
+from purplecaffeine import Trial, LocalStorage, BaseStorage as TrialStorage
 
 
 def dummy_trial(
-    name: Optional[str] = "test_trial", backend: Optional[TrialBackend] = None
+    name: Optional[str] = "test_trial", storage: Optional[TrialStorage] = None
 ):
     """Returns dummy trial for tests.
 
     Returns:
         dummy trial
     """
-    trial = Trial(name=name, backend=backend)
+    trial = Trial(name=name, storage=storage)
+    trial.add_description("Short desc")
     trial.add_metric("test_metric", 42)
     trial.add_parameter("test_parameter", "parameter")
     trial.add_circuit("test_circuit", QuantumCircuit(2))
     trial.add_operator("test_operator", Operator(XGate()))
     trial.add_text("test_text", "text")
     trial.add_array("test_array", np.array([42]))
     trial.add_tag("qiskit")
@@ -38,62 +39,48 @@
 
     def setUp(self) -> None:
         """SetUp Trial object."""
         current_directory = os.path.dirname(os.path.abspath(__file__))
         self.save_path = os.path.join(current_directory, "resources")
         if not os.path.exists(self.save_path):
             Path(self.save_path).mkdir(parents=True, exist_ok=True)
-        self.local_backend = LocalBackend(path=self.save_path)
+        self.local_storage = LocalStorage(path=self.save_path)
 
     def test_trial_context(self):
         """Test train context."""
         uuid = "some_uuid"
-        with Trial(name="test_trial", backend=self.local_backend, uuid=uuid) as trial:
+        with Trial(name="test_trial", storage=self.local_storage, uuid=uuid) as trial:
             trial.add_metric("test_metric", 42)
         trial.read(trial_id=uuid)
         self.assertTrue(os.path.isfile(os.path.join(self.save_path, f"{uuid}.json")))
         self.assertEqual(trial.metrics, [["test_metric", 42]])
 
     def test_add_trial(self):
         """Test adding stuff into Trial."""
         trial = dummy_trial()
 
+        self.assertEqual(trial.description, "Short desc")
         self.assertEqual(trial.metrics, [["test_metric", 42]])
         self.assertEqual(trial.parameters, [["test_parameter", "parameter"]])
         self.assertEqual(trial.circuits, [["test_circuit", QuantumCircuit(2)]])
         self.assertEqual(trial.operators, [["test_operator", Operator(XGate())]])
         self.assertEqual(trial.texts, [["test_text", "text"]])
         self.assertEqual(trial.arrays, [["test_array", np.array([42])]])
         self.assertEqual(trial.tags, ["qiskit", "test"])
 
     def test_save_read_local_trial(self):
         """Test save and read Trial locally."""
-        trial = dummy_trial(backend=self.local_backend)
+        trial = dummy_trial(storage=self.local_storage)
         trial.save()
 
         self.assertTrue(
             os.path.isfile(os.path.join(self.save_path, f"{trial.uuid}.json"))
         )
         recovered = trial.read(trial_id=trial.uuid)
-        self.assertEqual(recovered.metrics, [["test_metric", 42]])
-        self.assertEqual(recovered.parameters, [["test_parameter", "parameter"]])
-        self.assertEqual(recovered.circuits, [["test_circuit", QuantumCircuit(2)]])
-        self.assertEqual(recovered.operators, [["test_operator", Operator(XGate())]])
-        self.assertEqual(recovered.texts, [["test_text", "text"]])
-        self.assertEqual(recovered.arrays, [["test_array", np.array([42])]])
-        self.assertEqual(recovered.tags, ["qiskit", "test"])
-
-    @skip("Remote call")
-    def test_save_read_api_trial(self):
-        """Test save and read Trial remotely."""
-        backend = ApiBackend(username="", password="", host="")
-        trial = dummy_trial(backend=backend)
-        trial.save()
-
-        recovered = trial.read(trial_id="1")
+        self.assertEqual(recovered.description, "Short desc")
         self.assertEqual(recovered.metrics, [["test_metric", 42]])
         self.assertEqual(recovered.parameters, [["test_parameter", "parameter"]])
         self.assertEqual(recovered.circuits, [["test_circuit", QuantumCircuit(2)]])
         self.assertEqual(recovered.operators, [["test_operator", Operator(XGate())]])
         self.assertEqual(recovered.texts, [["test_text", "text"]])
         self.assertEqual(recovered.arrays, [["test_array", np.array([42])]])
         self.assertEqual(recovered.tags, ["qiskit", "test"])
@@ -106,14 +93,15 @@
         self.assertTrue(
             os.path.isfile(os.path.join(self.save_path, f"{trial.uuid}.json"))
         )
         # Import
         new_trial = Trial("test_import").import_from_shared_file(
             os.path.join(self.save_path, f"{trial.uuid}.json")
         )
+        self.assertEqual(new_trial.description, "Short desc")
         self.assertEqual(new_trial.metrics, [["test_metric", 42]])
         self.assertEqual(new_trial.parameters, [["test_parameter", "parameter"]])
         self.assertEqual(new_trial.circuits, [["test_circuit", QuantumCircuit(2)]])
         self.assertEqual(new_trial.operators, [["test_operator", Operator(XGate())]])
         self.assertEqual(new_trial.texts, [["test_text", "text"]])
         self.assertEqual(new_trial.arrays, [["test_array", np.array([42])]])
         self.assertEqual(new_trial.tags, ["qiskit", "test"])
```

### Comparing `purplecaffeine-0.1.0/tests/utils/test_json.py` & `purplecaffeine-0.1.1/tests/utils/test_json.py`

 * *Files identical despite different names*

