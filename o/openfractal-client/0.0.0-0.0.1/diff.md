# Comparing `tmp/openfractal_client-0.0.0.tar.gz` & `tmp/openfractal_client-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.0.0.tar", last modified: Mon Jun  5 21:28:35 2023, max compression
+gzip compressed data, was "openfractal_client-0.0.1.tar", last modified: Mon Jun  5 21:47:45 2023, max compression
```

## Comparing `openfractal_client-0.0.0.tar` & `openfractal_client-0.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/.github/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)        9 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/CODEOWNERS
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     5202 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      333 2023-06-05 13:38:23.000000 openfractal_client-0.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      104 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/SECURITY.md
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/.github/workflows/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1119 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/workflows/code-check.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1397 2023-06-05 16:33:55.000000 openfractal_client-0.0.0/.github/workflows/doc.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1366 2023-06-05 21:23:36.000000 openfractal_client-0.0.0/.github/workflows/docker.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3112 2023-06-05 17:37:51.000000 openfractal_client-0.0.0/.github/workflows/release.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1055 2023-06-05 16:20:43.000000 openfractal_client-0.0.0/.github/workflows/test.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      477 2023-06-05 13:35:03.000000 openfractal_client-0.0.0/.gitignore
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       32 2023-06-05 13:34:51.000000 openfractal_client-0.0.0/CHANGELOG.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     2607 2023-06-05 17:03:50.000000 openfractal_client-0.0.0/Dockerfile
--rw-rw-r--   0 hadim     (1000) hadim     (1000)    11315 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/LICENSE
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3220 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/PKG-INFO
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1834 2023-06-05 21:00:45.000000 openfractal_client-0.0.0/README.md
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/docker/
--rwxrwxr-x   0 hadim     (1000) hadim     (1000)     1191 2023-06-05 20:57:48.000000 openfractal_client-0.0.0/docker/entrypoint.sh
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      695 2023-06-05 21:23:27.000000 openfractal_client-0.0.0/docker-compose.yml
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/docs/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       21 2023-06-05 13:33:33.000000 openfractal_client-0.0.0/docs/index.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       20 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/docs/license.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      746 2023-06-05 13:59:38.000000 openfractal_client-0.0.0/env.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1690 2023-06-05 21:00:48.000000 openfractal_client-0.0.0/mkdocs.yml
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/openfractal_client/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       34 2023-06-05 13:36:33.000000 openfractal_client-0.0.0/openfractal_client/__init__.py
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      229 2023-06-05 13:36:59.000000 openfractal_client-0.0.0/openfractal_client/_version.py
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/openfractal_client.egg-info/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3220 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/PKG-INFO
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      651 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)        1 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       19 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/top_level.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1885 2023-06-05 21:28:31.000000 openfractal_client-0.0.0/pyproject.toml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       38 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/setup.cfg
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/tests/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       49 2023-06-05 13:35:24.000000 openfractal_client-0.0.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.399504 openfractal_client-0.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.399504 openfractal_client-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/openfractal_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-05 21:47:45.000000 openfractal_client-0.0.1/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 21:47:45.000000 openfractal_client-0.0.1/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:47:45.000000 openfractal_client-0.0.1/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:47:45.000000 openfractal_client-0.0.1/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:47:45.403504 openfractal_client-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 21:45:20.000000 openfractal_client-0.0.1/tests/test_import.py
```

### Comparing `openfractal_client-0.0.0/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.0.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/code-check.yml` & `openfractal_client-0.0.1/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/doc.yml` & `openfractal_client-0.0.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/docker.yml` & `openfractal_client-0.0.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/release.yml` & `openfractal_client-0.0.1/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -91,12 +91,19 @@
 
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
+      - name: Build Changelog
+        id: github_release
+        uses: mikepenz/release-changelog-builder-action@v4
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          outputFile: CHANGELOGS.md
+
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
-          body: "See [CHANGELOGS.md](https://github.com/datamol-io/datamol/blob/main/CHANGELOG.md)."
+          body: ${{steps.github_release.outputs.changelog}}
```

### Comparing `openfractal_client-0.0.0/.github/workflows/test.yml` & `openfractal_client-0.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/Dockerfile` & `openfractal_client-0.0.1/Dockerfile`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM ghcr.io/mamba-org/micromamba:1.4-jammy-cuda-12.1.1
+FROM ghcr.io/mamba-org/micromamba:1.4-jammy
 
 ARG DEBIAN_FRONTEND=noninteractive
 
 ENV LC_ALL=C.UTF-8
 ENV LANG=C.UTF-8
 
 # Set the build arg to ENV so they are available at runtime.
@@ -30,19 +30,14 @@
     htop libsm6 libxrender1 git gettext-base tzdata \
     libxml2 libaio-dev nano && \
     apt clean
 
 # Switch back to regular user
 USER $MAMBA_USER
 
-# If the base image ships with CUDA, we need to make sure
-# CONDA_OVERRIDE_CUDA is set so micromamba can find the right virtual
-# packages `__cuda` and so allow the installation of CUDA packages such as `pytorch-gpu`.
-ENV CONDA_OVERRIDE_CUDA=$CUDA_VERSION
-
 RUN mkdir -p $MAMBA_ROOT_PREFIX
 
 # Configure base micromamba
 RUN micromamba config append channels conda-forge && \
     micromamba config set show_banner false && \
     micromamba config set auto_activate_base true && \
     micromamba config set channel_priority strict && \
```

### Comparing `openfractal_client-0.0.0/LICENSE` & `openfractal_client-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/PKG-INFO` & `openfractal_client-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal_client
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,12 +58,12 @@
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/README.md` & `openfractal_client-0.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,12 +30,12 @@
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/docker/entrypoint.sh` & `openfractal_client-0.0.1/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/docker-compose.yml` & `openfractal_client-0.0.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/env.yml` & `openfractal_client-0.0.1/env.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/mkdocs.yml` & `openfractal_client-0.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.0.1/openfractal_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal-client
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,12 +58,12 @@
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/openfractal_client.egg-info/SOURCES.txt` & `openfractal_client-0.0.1/openfractal_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .gitignore
-CHANGELOG.md
+CHANGELOGS.md
 Dockerfile
 LICENSE
 README.md
 docker-compose.yml
 env.yml
 mkdocs.yml
 pyproject.toml
```

### Comparing `openfractal_client-0.0.0/pyproject.toml` & `openfractal_client-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openfractal_client"
 description = "A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation."
 authors = [{ name = "Hadrien Mary", email = "hadrien@valencediscovery.com" }]
 readme = "README.md"
-# dynamic = ["version"]
-version = "0.0.0"
+dynamic = ["version"]
 requires-python = ">=3.9"
 license = { text = "Apache" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
```

