# Comparing `tmp/rbx-3.1.0.dev26.tar.gz` & `tmp/rbx-3.1.0.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbx-3.1.0.dev26.tar", last modified: Thu May 25 11:59:24 2023, max compression
+gzip compressed data, was "rbx-3.1.0.dev27.tar", last modified: Mon Jun  5 14:56:26 2023, max compression
```

## Comparing `rbx-3.1.0.dev26.tar` & `rbx-3.1.0.dev27.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/keystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/buildtools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx/buildtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/buildtools/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/adsquare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/broadsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/oxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/uslicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/queues/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/utils/mdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.760772 rbx-3.1.0.dev27/rbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/auth/keystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-05 14:56:25.000000 rbx-3.1.0.dev27/rbx/buildtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/buildtools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/tasks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/tasks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/buildtools/tasks/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/adsquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/broadsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/oxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/clients/uslicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/gcp/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.764772 rbx-3.1.0.dev27/rbx/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/geo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/geo/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/geo/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/rbx/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/manifest/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/rbx/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/queues/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/queues/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/rbx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/utils/mdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/rbx/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-05 14:56:06.000000 rbx-3.1.0.dev27/rbx/web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:56:26.760772 rbx-3.1.0.dev27/rbx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 14:56:26.000000 rbx-3.1.0.dev27/rbx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:56:26.768772 rbx-3.1.0.dev27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-05 14:56:25.000000 rbx-3.1.0.dev27/setup.py
```

### Comparing `rbx-3.1.0.dev26/LICENSE` & `rbx-3.1.0.dev27/LICENSE`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/PKG-INFO` & `rbx-3.1.0.dev27/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.1.0.dev26
+Version: 3.1.0.dev27
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.1.0.dev26/rbx/auth/decorators.py` & `rbx-3.1.0.dev27/rbx/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/auth/keystore.py` & `rbx-3.1.0.dev27/rbx/auth/keystore.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/aws/s3.py` & `rbx-3.1.0.dev27/rbx/aws/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             raise AWSException(e)
 
     def copy(self, filename, key, content_type="binary/octet-stream", download=False):
         """Copy a file to the given S3 key.
 
         The filename will be read, so filename is expected to be the path to the file itself.
 
-        When download is True,  we add the "ContentDisposition: attachment" header so that it makes
+        When download is True, we add the "ContentDisposition: attachment" header so that it makes
         browsers download the file when accessed directly.
         """
         content_type = (
             content_type or "binary/octet-stream"
         )  # Content-Type cannot be None
         options = {"ContentType": content_type}
         if download:
@@ -146,17 +146,26 @@
             if error_code == "404":
                 return
             else:
                 logger.error(e)
         else:
             return object
 
-    def save(self, fileobj, key, content_type="binary/octet-stream"):
-        """Save a file-like object to the given S3 key."""
+    def save(self, fileobj, key, content_type="binary/octet-stream", download=False):
+        """Save a file-like object to the given S3 key.
+
+        When download is True, we add the "ContentDisposition: attachment" header so that it makes
+        browsers download the file when accessed directly.
+        """
+        content_type = (
+            content_type or "binary/octet-stream"
+        )  # Content-Type cannot be None
         options = {"ContentType": content_type}
+        if download:
+            options["ContentDisposition"] = "attachment"
 
         try:
             self.bucket.upload_fileobj(fileobj, self.prefix + key, ExtraArgs=options)
         except ValueError as e:
             raise AWSException(e)
         except botocore.exceptions.ClientError as e:
             logger.error(e, extra=e.response)
```

### Comparing `rbx-3.1.0.dev26/rbx/buildtools/tasks/deploy.py` & `rbx-3.1.0.dev27/rbx/buildtools/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/buildtools/tasks/image.py` & `rbx-3.1.0.dev27/rbx/buildtools/tasks/image.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/buildtools/tasks/misc.py` & `rbx-3.1.0.dev27/rbx/buildtools/tasks/misc.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/__init__.py` & `rbx-3.1.0.dev27/rbx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/adsquare.py` & `rbx-3.1.0.dev27/rbx/clients/adsquare.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/broadsign.py` & `rbx-3.1.0.dev27/rbx/clients/broadsign.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/oxr.py` & `rbx-3.1.0.dev27/rbx/clients/oxr.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/panels.py` & `rbx-3.1.0.dev27/rbx/clients/panels.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/reporting.py` & `rbx-3.1.0.dev27/rbx/clients/reporting.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/retry.py` & `rbx-3.1.0.dev27/rbx/clients/retry.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/clients/uslicer.py` & `rbx-3.1.0.dev27/rbx/clients/uslicer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/exceptions.py` & `rbx-3.1.0.dev27/rbx/exceptions.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/gcp/cloud_tasks.py` & `rbx-3.1.0.dev27/rbx/gcp/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/gcp/pubsub.py` & `rbx-3.1.0.dev27/rbx/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/gcp/storage.py` & `rbx-3.1.0.dev27/rbx/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/geo/__init__.py` & `rbx-3.1.0.dev27/rbx/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/geo/cli.py` & `rbx-3.1.0.dev27/rbx/geo/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/geo/maps.py` & `rbx-3.1.0.dev27/rbx/geo/maps.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/geo/packer.py` & `rbx-3.1.0.dev27/rbx/geo/packer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/logging.py` & `rbx-3.1.0.dev27/rbx/logging.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/manifest/cli.py` & `rbx-3.1.0.dev27/rbx/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/manifest/processor.py` & `rbx-3.1.0.dev27/rbx/manifest/processor.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/manifest/utils.py` & `rbx-3.1.0.dev27/rbx/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/queues/__init__.py` & `rbx-3.1.0.dev27/rbx/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/queues/jobs.py` & `rbx-3.1.0.dev27/rbx/queues/jobs.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/queues/scheduler.py` & `rbx-3.1.0.dev27/rbx/queues/scheduler.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/utils/__init__.py` & `rbx-3.1.0.dev27/rbx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx/web/handlers.py` & `rbx-3.1.0.dev27/rbx/web/handlers.py`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx.egg-info/PKG-INFO` & `rbx-3.1.0.dev27/rbx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.1.0.dev26
+Version: 3.1.0.dev27
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.1.0.dev26/rbx.egg-info/SOURCES.txt` & `rbx-3.1.0.dev27/rbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/rbx.egg-info/requires.txt` & `rbx-3.1.0.dev27/rbx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.1.0.dev26/setup.py` & `rbx-3.1.0.dev27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 STORAGE = ["google-cloud-storage>=2.1,<3"]
 TASKS = ["google-cloud-tasks>=2.7,<3"]
 
 
 setup(
     name="rbx",
-    version="3.1.0.dev26",
+    version="3.1.0.dev27",
     license="Apache 2.0",
     description="Scoota Platform utilities",
     long_description="A collection of common tools for Scoota services.",
     url="http://scoota.com/",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

