# Comparing `tmp/codcat-0.1.0.tar.gz` & `tmp/codcat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codcat-0.1.0.tar", last modified: Wed May  3 16:23:12 2023, max compression
+gzip compressed data, was "codcat-0.2.0.tar", last modified: Mon Jun  5 11:29:28 2023, max compression
```

## Comparing `codcat-0.1.0.tar` & `codcat-0.2.0.tar`

### file list

```diff
@@ -1,82 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.508141 codcat-0.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.483138 codcat-0.1.0/.dvc/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-03 16:22:58.000000 codcat-0.1.0/.dvc/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-03 16:22:58.000000 codcat-0.1.0/.dvcignore
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-05-03 16:22:58.000000 codcat-0.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-05-03 16:22:58.000000 codcat-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1662 2023-05-03 16:22:58.000000 codcat-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    13829 2023-05-03 16:22:58.000000 codcat-0.1.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-03 16:22:58.000000 codcat-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3429 2023-05-03 16:23:12.508141 codcat-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-03 16:22:58.000000 codcat-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.485139 codcat-0.1.0/codcat/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/manifest.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.488139 codcat-0.1.0/codcat/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7055 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/models/estimator.py
--rw-rw-rw-   0 root         (0) root         (0)     2888 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/pyg.py
--rw-rw-rw-   0 root         (0) root         (0)     3828 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/tok.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.490139 codcat-0.1.0/codcat/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/tokenization.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.487139 codcat-0.1.0/codcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3429 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-03 16:22:58.000000 codcat-0.1.0/codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 16:22:58.000000 codcat-0.1.0/commitlint.config.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.492139 codcat-0.1.0/comparisons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2501 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/nn.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     6812 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.493139 codcat-0.1.0/data/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-03 16:22:58.000000 codcat-0.1.0/data/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-03 16:22:58.000000 codcat-0.1.0/data/code-snippets.csv.dvc
--rw-rw-rw-   0 root         (0) root         (0)     2139 2023-05-03 16:22:58.000000 codcat-0.1.0/dvc.lock
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-05-03 16:22:58.000000 codcat-0.1.0/dvc.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.474138 codcat-0.1.0/eval/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.493139 codcat-0.1.0/eval/live/
--rw-rw-rw-   0 root         (0) root         (0)     3121 2023-05-03 16:22:58.000000 codcat-0.1.0/eval/live/metrics.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.505141 codcat-0.1.0/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)   456701 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/1-eda.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7091 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/2-preprocessing.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    25406 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/3-bagofwords-tfidf.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   118990 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/4-embeddings.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6980 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/5-sentence-transformers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6000 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/6-code25-dataset.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    26980 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/7-code-tokenize.ipynb
--rw-rw-rw-   0 root         (0) root         (0)  1223000 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/8-final-evaluations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50282 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/bigcode-datasets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17407 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/bigcode-training.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7557 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/eda-paper.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    39168 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/eval-loss.png
--rw-rw-rw-   0 root         (0) root         (0)   249107 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/filtered-umap.png
--rw-rw-rw-   0 root         (0) root         (0)   300932 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/full-umap.png
--rw-rw-rw-   0 root         (0) root         (0)    47002 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/preprocessed-dataset-final-results.json
--rw-rw-rw-   0 root         (0) root         (0)    79326 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/scc-smol-final-results.json
--rw-rw-rw-   0 root         (0) root         (0)    79017 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/train-loss.png
--rw-rw-rw-   0 root         (0) root         (0)   687147 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/umap-datasets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   159120 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/wandbplot.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-03 16:22:58.000000 codcat-0.1.0/params.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-03 16:22:58.000000 codcat-0.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 16:22:58.000000 codcat-0.1.0/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-05-03 16:22:58.000000 codcat-0.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-03 16:23:12.509141 codcat-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.507141 codcat-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.508141 codcat-0.1.0/tests/resources/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/resources/test-manifest.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_estimator.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-03 16:22:58.000000 codcat-0.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.016676 codcat-0.2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.002676 codcat-0.2.0/.dvc/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 11:29:17.000000 codcat-0.2.0/.dvc/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-05 11:29:17.000000 codcat-0.2.0/.dvcignore
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2023-06-05 11:29:17.000000 codcat-0.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-05 11:29:17.000000 codcat-0.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-06-05 11:29:17.000000 codcat-0.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    13829 2023-06-05 11:29:17.000000 codcat-0.2.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-06-05 11:29:17.000000 codcat-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-05 11:29:28.016676 codcat-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-05 11:29:17.000000 codcat-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.004676 codcat-0.2.0/codcat/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/manifest.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.005676 codcat-0.2.0/codcat/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7055 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/models/estimator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2888 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/pyg.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/tok.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.006676 codcat-0.2.0/codcat/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/utils/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/utils/tokenization.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-05 11:29:17.000000 codcat-0.2.0/codcat/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.005676 codcat-0.2.0/codcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-05 11:29:27.000000 codcat-0.2.0/codcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-05 11:29:27.000000 codcat-0.2.0/codcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 11:29:27.000000 codcat-0.2.0/codcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-05 11:29:27.000000 codcat-0.2.0/codcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 11:29:27.000000 codcat-0.2.0/codcat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-05 11:29:17.000000 codcat-0.2.0/codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-05 11:29:17.000000 codcat-0.2.0/commitlint.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.007676 codcat-0.2.0/comparisons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.007676 codcat-0.2.0/comparisons/docker/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/docker/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/docker/docker-compose.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/docker/nginx.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/nn.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2023-06-05 11:29:17.000000 codcat-0.2.0/comparisons/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.008676 codcat-0.2.0/data/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-05 11:29:17.000000 codcat-0.2.0/data/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-05 11:29:17.000000 codcat-0.2.0/data/code-snippets.csv.dvc
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-06-05 11:29:17.000000 codcat-0.2.0/dvc.lock
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-05 11:29:17.000000 codcat-0.2.0/dvc.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:27.998676 codcat-0.2.0/eval/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.008676 codcat-0.2.0/eval/live/
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2023-06-05 11:29:17.000000 codcat-0.2.0/eval/live/metrics.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.015676 codcat-0.2.0/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)   456701 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/1-eda.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7091 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/2-preprocessing.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    25406 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/3-bagofwords-tfidf.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   118990 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/4-embeddings.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6980 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/5-sentence-transformers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6000 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/6-code25-dataset.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    26980 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/7-code-tokenize.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)  1223000 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/8-final-evaluations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50282 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/bigcode-datasets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17407 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/bigcode-training.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7557 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/eda-paper.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    39168 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/eval-loss.png
+-rw-rw-rw-   0 root         (0) root         (0)   249107 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/filtered-umap.png
+-rw-rw-rw-   0 root         (0) root         (0)   300932 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/full-umap.png
+-rw-rw-rw-   0 root         (0) root         (0)    47002 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/preprocessed-dataset-final-results.json
+-rw-rw-rw-   0 root         (0) root         (0)    79326 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/scc-smol-final-results.json
+-rw-rw-rw-   0 root         (0) root         (0)    79017 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/train-loss.png
+-rw-rw-rw-   0 root         (0) root         (0)   687147 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/umap-datasets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   159120 2023-06-05 11:29:17.000000 codcat-0.2.0/notebooks/wandbplot.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-05 11:29:17.000000 codcat-0.2.0/params.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-05 11:29:17.000000 codcat-0.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-05 11:29:17.000000 codcat-0.2.0/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-06-05 11:29:17.000000 codcat-0.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-05 11:29:28.017676 codcat-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.016676 codcat-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 11:29:17.000000 codcat-0.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:29:28.016676 codcat-0.2.0/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-05 11:29:17.000000 codcat-0.2.0/tests/resources/test-manifest.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-05 11:29:17.000000 codcat-0.2.0/tests/test_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-05 11:29:17.000000 codcat-0.2.0/tests/test_estimator.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-05 11:29:17.000000 codcat-0.2.0/tests/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-05 11:29:17.000000 codcat-0.2.0/tox.ini
```

### Comparing `codcat-0.1.0/.gitignore` & `codcat-0.2.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -129,7 +129,10 @@
 .pyre/
 
 .idea/
 .vscode/
 **/.DS_Store
 **/.pyc
 /model.onnx
+/comparisons/mlruns/
+/mlruns/
+/comparisons/docker/minio/
```

### Comparing `codcat-0.1.0/.gitlab-ci.yml` & `codcat-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/.pre-commit-config.yaml` & `codcat-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/.pylintrc` & `codcat-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/LICENSE` & `codcat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/PKG-INFO` & `codcat-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codcat
-Version: 0.1.0
+Version: 0.2.0
 Summary: Code snippets language classification tool
 Author-email: Konstantin Templin <1qnbhd@gmail.com>
 Maintainer-email: Konstantin Templin <1qnbhd@gmail.com>
 License: MIT
 Project-URL: Repository, https://gitlab.com/codcat/codcat
 Keywords: code,snippets,classification,language,NLP,ML
 Classifier: Intended Audience :: Science/Research
```

### Comparing `codcat-0.1.0/README.md` & `codcat-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/cli.py` & `codcat-0.2.0/codcat/cli.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/downloader.py` & `codcat-0.2.0/codcat/downloader.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/models/estimator.py` & `codcat-0.2.0/codcat/models/estimator.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/pyg.py` & `codcat-0.2.0/codcat/pyg.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/tok.py` & `codcat-0.2.0/codcat/tok.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/utils/dataset.py` & `codcat-0.2.0/codcat/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat/utils/tokenization.py` & `codcat-0.2.0/codcat/utils/tokenization.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/codcat.egg-info/PKG-INFO` & `codcat-0.2.0/codcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codcat
-Version: 0.1.0
+Version: 0.2.0
 Summary: Code snippets language classification tool
 Author-email: Konstantin Templin <1qnbhd@gmail.com>
 Maintainer-email: Konstantin Templin <1qnbhd@gmail.com>
 License: MIT
 Project-URL: Repository, https://gitlab.com/codcat/codcat
 Keywords: code,snippets,classification,language,NLP,ML
 Classifier: Intended Audience :: Science/Research
```

### Comparing `codcat-0.1.0/codcat.egg-info/SOURCES.txt` & `codcat-0.2.0/codcat.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 codcat/utils/tokenization.py
 codcat/utils/types.py
 comparisons/__init__.py
 comparisons/nn.py
 comparisons/requirements.txt
 comparisons/tools.py
 comparisons/train.py
+comparisons/docker/Dockerfile
+comparisons/docker/docker-compose.yml
+comparisons/docker/nginx.conf
 data/.gitignore
 data/code-snippets.csv.dvc
 eval/live/metrics.json
 notebooks/1-eda.ipynb
 notebooks/2-preprocessing.ipynb
 notebooks/3-bagofwords-tfidf.ipynb
 notebooks/4-embeddings.ipynb
```

### Comparing `codcat-0.1.0/comparisons/nn.py` & `codcat-0.2.0/comparisons/nn.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/comparisons/tools.py` & `codcat-0.2.0/comparisons/tools.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/comparisons/train.py` & `codcat-0.2.0/comparisons/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import os
 import time
+import traceback
 import warnings
 from collections import defaultdict
 from itertools import chain
+from urllib.parse import urlparse
 
+import mlflow
 from lightgbm import LGBMClassifier
+from mlflow.models import infer_signature
 from nltk import (
     TweetTokenizer,
     word_tokenize,
 )
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_extraction.text import (
     CountVectorizer,
@@ -25,16 +30,16 @@
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import LabelEncoder
 from sklearn.svm import SVC
 from tqdm.auto import tqdm
 from xgboost import XGBClassifier
 
-from comparisons.nn import SimpleTransformersWrapper
-from comparisons.tools import (
+from codcat.comparisons.nn import SimpleTransformersWrapper
+from codcat.comparisons.tools import (
     FastTextVectorizer,
     SentenceTransformerVectorizer,
 )
 
 estimators = {}
 
 
@@ -170,52 +175,93 @@
     le = LabelEncoder()
     y_train_labeled = le.fit_transform(y_train)
 
     pbar = tqdm(estimators.items())
 
     try:
         for name, estimator in pbar:
-            pbar.set_description("Fitting %s" % name)
-            estimator.fit(X_train, y_train_labeled)
-            for dataset_name, X, L in chain([("", X_test, y_test)], datasets):
-                encoded_L = le.transform(L)
-                start = time.time()
-                y_pred = estimator.predict(X)
-                results[name]["time-1sample"] = (time.time() - start) / len(X)
-                f1 = f1_score(encoded_L, y_pred, average="macro")
-                accuracy = accuracy_score(encoded_L, y_pred)
-                precision = precision_score(
-                    encoded_L, y_pred, average="weighted"
-                )
-                recall = recall_score(encoded_L, y_pred, average="weighted")
-
-                postfix = f"-{dataset_name}" if dataset_name else ""
-                results[name][f"f1{postfix}"] = f1
-                results[name][f"accuracy{postfix}"] = accuracy
-                results[name][f"precision{postfix}"] = precision
-                results[name][f"recall{postfix}"] = recall
-                results[name][
-                    f"classification-report{postfix}"
-                ] = classification_report(encoded_L, y_pred, output_dict=True)
-
-                print("-" * 80)
-                print(name)
-                print(classification_report(encoded_L, y_pred))
-                print("-" * 80)
+            with mlflow.start_run(nested=True):
+                pbar.set_description("Fitting %s" % name)
+                estimator.fit(X_train, y_train_labeled)
+                for dataset_name, X, L in chain(
+                    [("", X_test, y_test)], datasets
+                ):
+                    encoded_L = le.transform(L)
+                    start = time.time()
+                    y_pred = estimator.predict(X)
+                    results[name]["time-1sample"] = (time.time() - start) / len(
+                        X
+                    )
+                    f1 = f1_score(encoded_L, y_pred, average="macro")
+                    accuracy = accuracy_score(encoded_L, y_pred)
+                    precision = precision_score(
+                        encoded_L, y_pred, average="weighted"
+                    )
+                    recall = recall_score(encoded_L, y_pred, average="weighted")
+
+                    postfix = f"-{dataset_name}" if dataset_name else ""
+                    results[name][f"f1{postfix}"] = f1
+                    results[name][f"accuracy{postfix}"] = accuracy
+                    results[name][f"precision{postfix}"] = precision
+                    results[name][f"recall{postfix}"] = recall
+                    results[name][
+                        f"classification-report{postfix}"
+                    ] = classification_report(
+                        encoded_L, y_pred, output_dict=True
+                    )
+
+                    mlflow.log_param("model", name)
+                    mlflow.log_metric("f1", f1)
+                    mlflow.log_metric("accuracy", accuracy)
+                    mlflow.log_metric("recall", recall)
+                    mlflow.log_metric("precision", precision)
+
+                    signature = infer_signature(X_train, y_pred)
+                    tracking_url_type_store = urlparse(
+                        mlflow.get_tracking_uri()
+                    ).scheme
+
+                    # Model registry does not work with file store
+                    if tracking_url_type_store != "file":
+                        # Register the model
+                        # There are other ways to use the Model Registry, which depends on the use case,
+                        # please refer to the doc for more information:
+                        # https://mlflow.org/docs/latest/model-registry.html#api-workflow
+                        mlflow.sklearn.log_model(
+                            estimator,
+                            "model",
+                            registered_model_name=name,
+                            signature=signature,
+                        )
+                    else:
+                        mlflow.sklearn.log_model(
+                            estimator, "model", signature=signature
+                        )
+
+                    print("-" * 80)
+                    print(name)
+                    print(classification_report(encoded_L, y_pred))
+                    print("-" * 80)
     except Exception as e:
         print(e)
 
     return results
 
 
 if __name__ == "__main__":
     import pandas as pd
     from sklearn.model_selection import train_test_split
 
     # train = pd.read_csv('../notebooks/train.csv')
+    mlflow_tracking_uri = os.getenv(
+        "MLFLOW_TRACKING_URI", "http://localhost:5000"
+    )
+    mlflow.set_tracking_uri(mlflow_tracking_uri)
+    mlflow.set_experiment("ModelComparisons")
+
     # test = pd.read_csv('../notebooks/test.csv')
     train = pd.read_json("../notebooks/train-code25.json")
     test = pd.read_json("../notebooks/test-code25.json")
 
     # test = pd.read_csv('../notebooks/test-preprocessed.csv')
     # train, test = train_test_split(train, random_state=42)
     X_train, y_train = train["code"], train["language"]
```

### Comparing `codcat-0.1.0/dvc.lock` & `codcat-0.2.0/dvc.lock`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/dvc.yaml` & `codcat-0.2.0/dvc.yaml`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/eval/live/metrics.json` & `codcat-0.2.0/eval/live/metrics.json`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/1-eda.ipynb` & `codcat-0.2.0/notebooks/1-eda.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/2-preprocessing.ipynb` & `codcat-0.2.0/notebooks/2-preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/3-bagofwords-tfidf.ipynb` & `codcat-0.2.0/notebooks/3-bagofwords-tfidf.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/4-embeddings.ipynb` & `codcat-0.2.0/notebooks/4-embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/5-sentence-transformers.ipynb` & `codcat-0.2.0/notebooks/5-sentence-transformers.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/6-code25-dataset.ipynb` & `codcat-0.2.0/notebooks/6-code25-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/7-code-tokenize.ipynb` & `codcat-0.2.0/notebooks/7-code-tokenize.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/8-final-evaluations.ipynb` & `codcat-0.2.0/notebooks/8-final-evaluations.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/bigcode-datasets.ipynb` & `codcat-0.2.0/notebooks/bigcode-datasets.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/bigcode-training.ipynb` & `codcat-0.2.0/notebooks/bigcode-training.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/eda-paper.ipynb` & `codcat-0.2.0/notebooks/eda-paper.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/eval-loss.png` & `codcat-0.2.0/notebooks/eval-loss.png`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/filtered-umap.png` & `codcat-0.2.0/notebooks/filtered-umap.png`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/full-umap.png` & `codcat-0.2.0/notebooks/full-umap.png`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/preprocessed-dataset-final-results.json` & `codcat-0.2.0/notebooks/preprocessed-dataset-final-results.json`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/scc-smol-final-results.json` & `codcat-0.2.0/notebooks/scc-smol-final-results.json`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/train-loss.png` & `codcat-0.2.0/notebooks/train-loss.png`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/umap-datasets.ipynb` & `codcat-0.2.0/notebooks/umap-datasets.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/notebooks/wandbplot.ipynb` & `codcat-0.2.0/notebooks/wandbplot.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/pyproject.toml` & `codcat-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/tests/test_downloader.py` & `codcat-0.2.0/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/tests/test_estimator.py` & `codcat-0.2.0/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `codcat-0.1.0/tox.ini` & `codcat-0.2.0/tox.ini`

 * *Files identical despite different names*

