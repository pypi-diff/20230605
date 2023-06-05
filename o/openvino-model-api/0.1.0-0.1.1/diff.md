# Comparing `tmp/openvino_model_api-0.1.0.tar.gz` & `tmp/openvino_model_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino_model_api-0.1.0.tar", last modified: Thu Jun  1 19:25:24 2023, max compression
+gzip compressed data, was "openvino_model_api-0.1.1.tar", last modified: Mon Jun  5 10:38:12 2023, max compression
```

## Comparing `openvino_model_api-0.1.0.tar` & `openvino_model_api-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-01 19:25:24.374454 openvino_model_api-0.1.0/
--rw-rw-r--   0 wov       (1000) wov       (1000)      447 2023-06-01 19:25:24.374454 openvino_model_api-0.1.0/PKG-INFO
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-01 19:25:24.374454 openvino_model_api-0.1.0/openvino_model_api.egg-info/
--rw-rw-r--   0 wov       (1000) wov       (1000)      447 2023-06-01 19:25:24.000000 openvino_model_api-0.1.0/openvino_model_api.egg-info/PKG-INFO
--rw-rw-r--   0 wov       (1000) wov       (1000)     2996 2023-06-01 19:25:24.000000 openvino_model_api-0.1.0/openvino_model_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)       37 2023-06-01 19:25:24.000000 openvino_model_api-0.1.0/openvino_model_api.egg-info/dependency_links.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)      222 2023-06-01 19:25:24.000000 openvino_model_api-0.1.0/openvino_model_api.egg-info/requires.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)        9 2023-06-01 19:25:24.000000 openvino_model_api-0.1.0/openvino_model_api.egg-info/top_level.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)       38 2023-06-01 19:25:24.374454 openvino_model_api-0.1.0/setup.cfg
--rwxrwxr-x   0 wov       (1000) wov       (1000)     2049 2023-05-31 13:56:17.000000 openvino_model_api-0.1.0/setup.py
+drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/
+-rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/PKG-INFO
+drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/openvino_model_api.egg-info/
+-rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/PKG-INFO
+-rw-rw-r--   0 wov       (1000) wov       (1000)     2996 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)        1 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)      157 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/requires.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)        9 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/top_level.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)       38 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/setup.cfg
+-rwxrwxr-x   0 wov       (1000) wov       (1000)     1636 2023-06-05 10:34:46.000000 openvino_model_api-0.1.1/setup.py
```

### Comparing `openvino_model_api-0.1.0/openvino_model_api.egg-info/SOURCES.txt` & `openvino_model_api-0.1.1/openvino_model_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvino_model_api-0.1.0/setup.py` & `openvino_model_api-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,62 +11,35 @@
  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 """
 
-"""
-Use this script to create a wheel for Open Model Zoo
-model API. The installation of wheel is described in
-`<omz_dir>/demos/README.md`
-"""
-
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 SETUP_DIR = Path(__file__).resolve().parent
 
-with open(SETUP_DIR / "requirements.txt") as f:
-    INSTALL_REQUIRES = f.read().splitlines()
-
-with open(SETUP_DIR / "requirements_ovms.txt") as f:
-    OVMS_REQUIRES = f.read().splitlines()
-
-packages = find_packages(str(SETUP_DIR))
-package_dir = {"openvino": str(SETUP_DIR / "openvino")}
-
-TESTS_REQUIRE = [
-    "pytest",
-    "parameterized",
-    "google-api-python-client",
-    "onnx",
-    "tensorflow",
-    "torch",
-    "torchvision",
-    "protobuf~=3.20",
-]
-
-EXTRAS_REQUIRE = {
-    "ovms": OVMS_REQUIRES,
-    "tests": TESTS_REQUIRE,
-}
-
 setup(
     name="openvino_model_api",
-    version="0.1.0",
-    author="Intel Corporation",
-    license="OSI Approved :: Apache Software License",
-    url="https://github.com/openvinotoolkit/model_api",
+    version="0.1.1",
     description="Model API: model wrappers and pipelines for inference with OpenVINO",
-    python_requires=">=3.7",
+    author="Intel(R) Corporation",
+    url="https://github.com/openvinotoolkit/model_api",
+    packages=find_packages(SETUP_DIR),
+    package_dir={"openvino": str(SETUP_DIR / "openvino")},
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
     ],
-    packages=packages,
-    package_dir=package_dir,
-    install_requires=INSTALL_REQUIRES,
-    extras_require=EXTRAS_REQUIRE,
-    dependency_links=["https://download.pytorch.org/whl/cpu"],
+    license="OSI Approved :: Apache Software License",
+    python_requires=">=3.7",
+    install_requires=(SETUP_DIR / "requirements.txt").read_text(),
+    extras_require={
+        "ovms": (SETUP_DIR / "requirements_ovms.txt").read_text(),
+        "tests": ["pytest", "openvino-dev[onnx,pytorch,tensorflow2]"],
+    },
+    long_description=(SETUP_DIR.parents[1] / "README.md").read_text(),
+    long_description_content_type="text/markdown",
 )
```

