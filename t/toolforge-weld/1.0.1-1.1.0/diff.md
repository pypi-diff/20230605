# Comparing `tmp/toolforge-weld-1.0.1.tar.gz` & `tmp/toolforge-weld-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-1.0.1.tar", last modified: Thu May 25 13:02:57 2023, max compression
+gzip compressed data, was "toolforge-weld-1.1.0.tar", last modified: Mon Jun  5 17:51:10 2023, max compression
```

## Comparing `toolforge-weld-1.0.1.tar` & `toolforge-weld-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:02:57.555288 toolforge-weld-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/tests/test_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2998 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3021 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-25 13:02:47.000000 toolforge-weld-1.0.1/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:02:57.559289 toolforge-weld-1.0.1/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 13:02:57.000000 toolforge-weld-1.0.1/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-25 13:02:57.000000 toolforge-weld-1.0.1/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 13:02:57.000000 toolforge-weld-1.0.1/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-25 13:02:57.000000 toolforge-weld-1.0.1/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 13:02:57.000000 toolforge-weld-1.0.1/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.107992 toolforge-weld-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7555 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-1.0.1/LICENSE` & `toolforge-weld-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/PKG-INFO` & `toolforge-weld-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.0.1
+Version: 1.1.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.0.1/setup.py` & `toolforge-weld-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from pathlib import Path
+
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="1.0.1",
+    version="1.1.0",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
-    long_description=(this_directory / 'README.md').read_text(),
-    long_description_content_type='text/markdown',
+    long_description=(this_directory / "README.md").read_text(),
+    long_description_content_type="text/markdown",
     install_requires=["python-dateutil", "PyYAML", "requests"],
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: System Administrators',
-        'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
-        'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3',
-        'Typing :: Typed',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: System Administrators",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3",
+        "Typing :: Typed",
     ],
     python_requires=">=3.7",
 )
```

### Comparing `toolforge-weld-1.0.1/tests/test_api_client.py` & `toolforge-weld-1.1.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/tests/test_kubernetes_config.py` & `toolforge-weld-1.1.0/tests/test_kubernetes_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,32 +41,50 @@
             }
         ],
         "apiVersion": "v1",
     }
 
 
 @pytest.fixture
-def tmp_kubeconfig(tmp_path) -> Path:
+def tmp_kubeconfig(tmp_path: Path) -> Path:
     path = tmp_path / "dummy_file.yaml"
     return path
 
 
+@pytest.fixture
+def tmp_token(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> str:
+    token = "asdf"
+
+    token_file = tmp_path / "token"
+    token_file.write_text(token)
+
+    monkeypatch.setattr(
+        toolforge_weld.kubernetes_config,
+        "CONTAINER_SERVICE_ACCOUNT_TOKEN_FILE",
+        token_file,
+    )
+
+    return token
+
+
 def test_kubeconfig_load_loads_from_given_path(tmp_kubeconfig: Path):
     tmp_kubeconfig.write_text(yaml.dump(get_dummy_kubeconfig_data()))
 
     my_kubeconfig = Kubeconfig.load(path=tmp_kubeconfig)
 
     assert (
         my_kubeconfig.client_cert_file
         == tmp_kubeconfig.parent.parent / ".toolskube/client.crt"
     )
     assert (
         my_kubeconfig.client_key_file
         == tmp_kubeconfig.parent.parent / ".toolskube/client.key"
     )
+    assert my_kubeconfig.ca_file is None
+    assert my_kubeconfig.token is None
     assert my_kubeconfig.current_namespace == "tool-wm-lol"
     assert (
         my_kubeconfig.current_server == "https://k8s.tools.eqiad1.wikimedia.cloud:6443"
     )
 
 
 def test_kubeconfig_load_loads_from_user_home(
@@ -115,7 +133,22 @@
         my_kubeconfig.client_key_file
         == tmp_kubeconfig.parent.parent / ".toolskube/client.key"
     )
     assert my_kubeconfig.current_namespace == "tool-wm-lol"
     assert (
         my_kubeconfig.current_server == "https://k8s.tools.eqiad1.wikimedia.cloud:6443"
     )
+
+
+def test_kubeconfig_load_from_token_file(tmp_token: str):
+    my_kubeconfig = Kubeconfig.from_container_service_account(namespace="tf-public")
+
+    assert my_kubeconfig.token == tmp_token
+    assert (
+        str(my_kubeconfig.ca_file)
+        == "/var/run/secrets/kubernetes.io/serviceaccount/ca.crt"
+    )
+    assert my_kubeconfig.current_server == "https://kubernetes.default.svc"
+    assert my_kubeconfig.current_namespace == "tf-public"
+
+    assert my_kubeconfig.client_cert_file is None
+    assert my_kubeconfig.client_key_file is None
```

### Comparing `toolforge-weld-1.0.1/toolforge_weld/api_client.py` & `toolforge-weld-1.1.0/toolforge_weld/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, Callable, Optional
 
 import requests
 import urllib3
 
 import toolforge_weld
-from toolforge_weld.kubernetes_config import Kubeconfig
+from toolforge_weld.kubernetes_config import Kubeconfig, ToolforgeKubernetesConfigError
 
 
 # TODO: these are available natively starting with python 3.9
 # but toolforge bastions run python 3.7 as of this writing
 def _removesuffix(input_string: str, suffix: str) -> str:
     if suffix and input_string.endswith(suffix):
         return input_string[: -len(suffix)]  # noqa: E203
@@ -36,24 +36,34 @@
         exception_handler: Optional[Callable[..., BaseException]] = None,
     ):
         self.exception_handler = exception_handler
         self.timeout = timeout
         self.server = server
         self.session = requests.Session()
 
-        self.session.cert = (
-            str(kubeconfig.client_cert_file),
-            str(kubeconfig.client_key_file),
-        )
-
-        self.session.verify = False
-
-        # T253412: Disable warnings about unverifed TLS certs when talking to the
-        # Kubernetes API endpoint
-        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        if kubeconfig.client_cert_file and kubeconfig.client_key_file:
+            self.session.cert = (
+                str(kubeconfig.client_cert_file),
+                str(kubeconfig.client_key_file),
+            )
+        elif kubeconfig.token:
+            self.session.headers["Authorization"] = f"Bearer {kubeconfig.token}"
+        else:
+            raise ToolforgeKubernetesConfigError(
+                "Kubernetes configuration is missing authentication details"
+            )
+
+        if kubeconfig.ca_file:
+            self.session.verify = str(kubeconfig.ca_file)
+        else:
+            self.session.verify = False
+
+            # T253412: Disable warnings about unverifed TLS certs when talking to the
+            # Kubernetes API endpoint
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
         self.session.headers[
             "User-Agent"
         ] = f"{user_agent} toolforge_weld/{toolforge_weld.__version__} python-requests/{requests.__version__}"
 
     def _make_request(self, method: str, url: str, **kwargs) -> requests.Response:
         try:
```

### Comparing `toolforge-weld-1.0.1/toolforge_weld/errors.py` & `toolforge-weld-1.1.0/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/toolforge_weld/kubernetes.py` & `toolforge-weld-1.1.0/toolforge_weld/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/toolforge_weld/kubernetes_config.py` & `toolforge-weld-1.1.0/toolforge_weld/kubernetes_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,51 +12,70 @@
     """Base class for exceptions related to the Kubernetes config."""
 
 
 class KubernetesConfigFileNotFoundException(ToolforgeKubernetesConfigError):
     """Raised when a Kubernetes client is attempted to be created but the configuration file does not exist."""
 
 
+CONTAINER_SERVICE_ACCOUNT_TOKEN_FILE = Path(
+    "/var/run/secrets/kubernetes.io/serviceaccount/token"
+)
+CONTAINER_CA_FILE = Path("/var/run/secrets/kubernetes.io/serviceaccount/ca.crt")
+CONTAINER_API_SERVER_URL = "https://kubernetes.default.svc"
+
+
 @dataclass(frozen=True)
 class Kubeconfig:
-    path: Path
     current_server: str
-    client_cert_file: Path
-    client_key_file: Path
     current_namespace: str
 
+    client_cert_file: Optional[Path] = None
+    client_key_file: Optional[Path] = None
+    token: Optional[str] = None
+    ca_file: Optional[Path] = None
+
     @classmethod
-    def from_path(cls, path: Path):
+    def from_path(cls, path: Path) -> "Kubeconfig":
         data = yaml.safe_load(path.read_text())
         current_context = _find_cfg_obj(data, "contexts", data["current-context"])
         current_cluster = _find_cfg_obj(data, "clusters", current_context["cluster"])
         current_user = _find_cfg_obj(data, "users", current_context["user"])
         return cls(
-            path=path,
             current_server=current_cluster["server"],
             # TODO: handle when the contents of the cert are embedded in the kubeconfig
             client_cert_file=_resolve_file_path(
                 path.parent, current_user["client-certificate"]
             ),
             # TODO: handle when the contents of the key are embedded in the kubeconfig
             client_key_file=_resolve_file_path(path.parent, current_user["client-key"]),
             current_namespace=current_context["namespace"],
         )
 
     @classmethod
-    def load(cls, path: Optional[Path] = None):
+    def load(cls, path: Optional[Path] = None) -> "Kubeconfig":
         """Load the kubeconfig file from the given path or environment and standard locations."""
         if path is None:
             path = locate_config_file()
 
         if not path.exists():
             raise KubernetesConfigFileNotFoundException(str(path.resolve()))
 
         return cls.from_path(path=path)
 
+    @classmethod
+    def from_container_service_account(cls, *, namespace: str) -> "Kubeconfig":
+        token = CONTAINER_SERVICE_ACCOUNT_TOKEN_FILE.read_text()
+
+        return cls(
+            current_server=CONTAINER_API_SERVER_URL,
+            token=token,
+            ca_file=CONTAINER_CA_FILE,
+            current_namespace=namespace,
+        )
+
 
 def locate_config_file() -> Path:
     """Attempt to locate the Kubernetes config file for this user.
 
     Don't use directly, only public for backwards compatibility.
     """
     return Path(os.getenv("KUBECONFIG", "~/.kube/config")).expanduser()
@@ -78,13 +97,12 @@
         return input_path
     return (base / input_path).resolve()
 
 
 def fake_kube_config() -> Kubeconfig:
     """Creates a fake Kubeconfig object for testing purposes."""
     return Kubeconfig(
-        path=Path("dummy/path"),
         current_server="https://example.org/",
         current_namespace="tool-test",
         client_cert_file=Path("/tmp/fake.crt"),
         client_key_file=Path("/tmp/fake.key"),
     )
```

### Comparing `toolforge-weld-1.0.1/toolforge_weld/logs/__init__.py` & `toolforge-weld-1.1.0/toolforge_weld/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-1.1.0/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/toolforge_weld/logs/source.py` & `toolforge-weld-1.1.0/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.0.1/toolforge_weld.egg-info/PKG-INFO` & `toolforge-weld-1.1.0/toolforge_weld.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.0.1
+Version: 1.1.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.0.1/toolforge_weld.egg-info/SOURCES.txt` & `toolforge-weld-1.1.0/toolforge_weld.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 tests/test_api_client.py
+tests/test_config.py
 tests/test_kubernetes.py
 tests/test_kubernetes_config.py
 tests/test_utils.py
 toolforge_weld/__init__.py
 toolforge_weld/api_client.py
+toolforge_weld/config.py
 toolforge_weld/errors.py
 toolforge_weld/kubernetes.py
 toolforge_weld/kubernetes_config.py
 toolforge_weld/py.typed
 toolforge_weld/utils.py
 toolforge_weld.egg-info/PKG-INFO
 toolforge_weld.egg-info/SOURCES.txt
```

