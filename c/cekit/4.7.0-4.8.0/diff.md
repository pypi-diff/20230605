# Comparing `tmp/cekit-4.7.0.tar.gz` & `tmp/cekit-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cekit-4.7.0.tar", last modified: Fri May 19 09:36:55 2023, max compression
+gzip compressed data, was "cekit-4.8.0.tar", last modified: Mon Jun  5 06:38:02 2023, max compression
```

## Comparing `cekit-4.7.0.tar` & `cekit-4.8.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.515787 cekit-4.7.0/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-05-19 09:36:54.000000 cekit-4.7.0/LICENSE
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-05-19 09:36:54.000000 cekit-4.7.0/MANIFEST.in
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-05-19 09:36:55.515787 cekit-4.7.0/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-05-19 09:36:54.000000 cekit-4.7.0/README.rst
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.513787 cekit-4.7.0/cekit/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builder.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/builders/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/buildah.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     9671 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/docker_builder.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    21904 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/podman.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/cache/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/artifact.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cekit_types.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    15244 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2408 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/config.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/crypto.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/descriptor/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     6611 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1367 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/env.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1174 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/execute.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/image.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/label.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/module.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/modules.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/overrides.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     6338 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/packages.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/port.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    24929 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/resource.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/run.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/volume.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/errors.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/generator/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    27118 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/behave.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/docker.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/legacy_version.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    13990 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/log.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/template_helper.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/templates/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/help.jinja
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/template.jinja
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.515787 cekit-4.7.0/cekit/test/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/behave_runner.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/behave_tester.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/collector.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    22126 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/tools.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/version.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.513787 cekit-4.7.0/cekit.egg-info/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/entry_points.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/requires.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/top_level.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-05-19 09:36:54.000000 cekit-4.7.0/requirements.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      339 2023-05-19 09:36:55.515787 cekit-4.7.0/setup.cfg
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-05-19 09:36:54.000000 cekit-4.7.0/setup.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-06-05 06:38:01.000000 cekit-4.8.0/LICENSE
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-06-05 06:38:01.000000 cekit-4.8.0/MANIFEST.in
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-06-05 06:38:02.641619 cekit-4.8.0/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-06-05 06:38:01.000000 cekit-4.8.0/README.rst
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.639619 cekit-4.8.0/cekit/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builder.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.639619 cekit-4.8.0/cekit/builders/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builders/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builders/buildah.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     9442 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builders/docker_builder.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    21904 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builders/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/builders/podman.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/cekit/cache/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/cache/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/cache/artifact.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/cache/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/cekit_types.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    15304 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2290 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/config.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/crypto.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/cekit/descriptor/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6579 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1367 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/env.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1174 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/execute.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/image.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/label.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/module.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/modules.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/overrides.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6338 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/packages.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/port.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    25109 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/resource.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/run.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/descriptor/volume.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/errors.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/cekit/generator/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    27221 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/behave.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/docker.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/legacy_version.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    14205 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/generator/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/log.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/template_helper.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/cekit/templates/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/templates/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/templates/help.jinja
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/templates/template.jinja
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.640619 cekit-4.8.0/cekit/test/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/test/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/test/behave_runner.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/test/behave_tester.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/test/collector.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    21957 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/tools.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-06-05 06:38:01.000000 cekit-4.8.0/cekit/version.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-06-05 06:38:02.639619 cekit-4.8.0/cekit.egg-info/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/entry_points.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/requires.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-06-05 06:38:02.000000 cekit-4.8.0/cekit.egg-info/top_level.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-06-05 06:38:01.000000 cekit-4.8.0/requirements.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      339 2023-06-05 06:38:02.641619 cekit-4.8.0/setup.cfg
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-06-05 06:38:01.000000 cekit-4.8.0/setup.py
```

### Comparing `cekit-4.7.0/LICENSE` & `cekit-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/PKG-INFO` & `cekit-4.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.7.0
+Version: 4.8.0
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.7.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.8.0.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.7.0/cekit/builder.py` & `cekit-4.8.0/cekit/builder.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/builders/buildah.py` & `cekit-4.8.0/cekit/builders/buildah.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/builders/docker_builder.py` & `cekit-4.8.0/cekit/builders/docker_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,37 +106,33 @@
                 build_log.append(messages)
 
                 layer_id_match = re.search(r"^---> ([\w]{12})$", messages)
 
                 if layer_id_match:
                     docker_layer_ids.append(layer_id_match.group(1))
 
-        except requests.ConnectionError as ex:
+        except requests.ConnectionError:
             exception_chain = traceback.format_exc()
-            # TODO: exc_info should probably be True rather than 1.
             LOGGER.debug(
                 "Caught ConnectionError attempting to communicate with Docker ",
-                exc_info=1,
+                exc_info=True,
             )
 
             if "PermissionError" in exception_chain:
                 message = (
                     "Unable to contact docker daemon. Is it correctly setup?\n"
                     "See https://developer.fedoraproject.org/tools/docker/docker-installation.html and "
                     "http://www.projectatomic.io/blog/2015/08/why-we-dont-let-non-root-users-run-docker-in-centos-fedora-or-rhel"
                 )
             elif "FileNotFoundError" in exception_chain:
                 message = "Unable to contact docker daemon. Is it started?"
             else:
                 message = "Unknown ConnectionError from docker ; is the daemon started and correctly setup?"
 
-            # Work-around for python 3 code - replicate exception(...) from None
-            cekit_exception = CekitError(message, ex)
-            cekit_exception.__cause__ = None
-            raise cekit_exception
+            raise CekitError(message) from None
 
         except Exception as ex:
             msg = "Image build failed, see logs above."
             if len(docker_layer_ids) >= 2:
                 LOGGER.error(
                     "You can look inside the failed image by running "
                     "'docker run --rm -ti {} bash'".format(docker_layer_ids[-1])
@@ -147,15 +143,15 @@
                 msg = (
                     "Image build failed with a yum error and you don't "
                     "have any yum repository configured, please check "
                     "your image/module descriptor for proper repository "
                     "definitions."
                 )
 
-            raise CekitError(msg, ex)
+            raise CekitError(msg) from ex
 
         return docker_layer_ids[-1]
 
     def _squash(self, docker_client, image_id):
         LOGGER.info("Squashing image {}...".format(image_id))
 
         squash = Squash(
@@ -205,15 +201,15 @@
             client = APIClientClass(**params)
         except docker.errors.DockerException as e:
             LOGGER.error(
                 "Could not create Docker client, please make sure that you "
                 "specified valid parameters in the 'DOCKER_HOST' environment variable, "
                 "examples: 'unix:///var/run/docker.sock', 'tcp://192.168.22.33:1234'"
             )
-            raise CekitError("Error while creating the Docker client", e)
+            raise CekitError("Error while creating the Docker client") from e
 
         if client and self._valid_docker_connection(client):
             LOGGER.debug("Docker client ready and working")
             LOGGER.debug(client.version())
             return client
 
         LOGGER.error(
```

### Comparing `cekit-4.7.0/cekit/builders/osbs.py` & `cekit-4.8.0/cekit/builders/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/builders/podman.py` & `cekit-4.8.0/cekit/builders/podman.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/cache/artifact.py` & `cekit-4.8.0/cekit/cache/artifact.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/cache/cli.py` & `cekit-4.8.0/cekit/cache/cli.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/cli.py` & `cekit-4.8.0/cekit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,16 +480,18 @@
         ]
 
         for directory in directories_to_clean:
             if os.path.exists(directory):
                 LOGGER.debug("Removing dirty directory: '{}'".format(directory))
                 try:
                     shutil.rmtree(directory)
-                except Exception:
-                    raise CekitError("Unable to clean directory '{}'".format(directory))
+                except Exception as ex:
+                    raise CekitError(
+                        "Unable to clean directory '{}'".format(directory)
+                    ) from ex
 
     def run(self, clazz: Type["Command"]):
         """Main application entry"""
 
         self.init()
         self.configure()
         self.cleanup()
```

### Comparing `cekit-4.7.0/cekit/config.py` & `cekit-4.8.0/cekit/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,17 +44,14 @@
         cls.cfg["common"] = cls.cfg.get("common", {})
         cls.cfg["common"]["work_dir"] = cls.cfg.get("common").get(
             "work_dir", default_work_dir
         )
         cls.cfg["common"]["redhat"] = yaml.safe_load(
             cls.cfg.get("common", {}).get("redhat", "False")
         )
-        cls.cfg["common"]["fetch_url_domains"] = cls.cfg.get("common").get(
-            "fetch_url_domains"
-        )
 
     @classmethod
     def get(cls, *args) -> Optional[str]:
         """Returns key value located by path of *args,
         None if Key doesn't exists,
 
         Args:
```

### Comparing `cekit-4.7.0/cekit/crypto.py` & `cekit-4.8.0/cekit/crypto.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/__init__.py` & `cekit-4.8.0/cekit/descriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/base.py` & `cekit-4.8.0/cekit/descriptor/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
                 schema_data=self.schema,
                 allow_assertions=True,
             )
 
             core.validate(raise_exception=True)
         except SchemaError as ex:
             raise CekitError(
-                "Cannot validate schema: {}".format(self.__class__.__name__), ex
-            )
+                "Cannot validate schema: {}".format(self.__class__.__name__)
+            ) from ex
 
     @classmethod
     def to_yaml(cls, representer: yaml.representer.BaseRepresenter, node) -> yaml.Node:
         return representer.represent_data(node._descriptor)
 
     def write(self, path: str) -> None:
         directory = os.path.dirname(path)
@@ -91,18 +91,17 @@
         Args:
           descriptor - a cekit descriptor
         """
         try:
             _merge_descriptors(self, descriptor)
             return self
         except KeyError as ex:
-            logger.debug(ex, exc_info=True)
             raise CekitError(
                 "Cannot merge descriptors, see log message for more information"
-            )
+            ) from ex
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self["name"] == other["name"]
         return NotImplemented
 
     def __ne__(self, other):
```

### Comparing `cekit-4.7.0/cekit/descriptor/env.py` & `cekit-4.8.0/cekit/descriptor/env.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/execute.py` & `cekit-4.8.0/cekit/descriptor/execute.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/image.py` & `cekit-4.8.0/cekit/descriptor/image.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/label.py` & `cekit-4.8.0/cekit/descriptor/label.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/module.py` & `cekit-4.8.0/cekit/descriptor/module.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/modules.py` & `cekit-4.8.0/cekit/descriptor/modules.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/osbs.py` & `cekit-4.8.0/cekit/descriptor/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/overrides.py` & `cekit-4.8.0/cekit/descriptor/overrides.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/packages.py` & `cekit-4.8.0/cekit/descriptor/packages.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/port.py` & `cekit-4.8.0/cekit/descriptor/port.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/resource.py` & `cekit-4.8.0/cekit/descriptor/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 import shutil
+from abc import abstractmethod
 from typing import Any, Dict, Optional, overload
 
 from cekit.cekit_types import _T, PathType
 from cekit.config import Config
 from cekit.crypto import SUPPORTED_HASH_ALGORITHMS, check_sum
 from cekit.descriptor import Descriptor
 from cekit.errors import CekitError
@@ -191,30 +192,35 @@
         """
         Make sure that the 'dest' value, if provided, does end with a single slash.
         """
 
         if descriptor.get("dest") is not None:
             descriptor["dest"] = os.path.normpath(descriptor.get("dest")) + "/"
 
+    @abstractmethod
     def _get_default_name_value(self, descriptor: RawResourceDescriptor) -> str:
         """
         Returns default identifier value for particular class.
 
         This method must be overridden in classes extending Resource.
         Returned should be a string that will be be a unique identifier
         of the resource across thw whole image.
         """
-        # TODO: This is an abstract method, and hence should return NotImplementedError()
-        return None
+        raise NotImplementedError(
+            "Implement _get_default_name_value() for Resource: "
+            + self.__module__
+            + "."
+            + type(self).__name__
+        )
 
     def _get_default_target_value(self, descriptor: RawResourceDescriptor) -> str:
         return os.path.basename(descriptor.get("name"))
 
+    @abstractmethod
     def _copy_impl(self, target: PathType) -> PathType:
-        # TODO: Return value is never used.
         raise NotImplementedError(
             "Implement _copy_impl() for Resource: "
             + self.__module__
             + "."
             + type(self).__name__
         )
 
@@ -255,16 +261,16 @@
             )
 
             if self.description:
                 logger.info(self.description)
 
             # exception is fatal we be logged before Cekit dies
             raise CekitError(
-                "Error copying resource: '%s'. See logs for more info." % self.name, ex
-            )
+                "Error copying resource: '%s'. See logs for more info." % self.name
+            ) from ex
 
         if set(SUPPORTED_HASH_ALGORITHMS).intersection(self) and not self.__verify(
             target
         ):
             raise CekitError("Artifact checksum verification failed!")
 
         return target
@@ -376,18 +382,17 @@
             # file - try to fetch the 'path' artifact from cacher
             # even if it was not defined as 'url'.
             if cache:
                 try:
                     self._download_file(self.path, target)
                     return target
                 except Exception as ex:
-                    logger.exception(ex)
                     raise CekitError(
                         "Could not download resource '%s' from cache" % self.name
-                    )
+                    ) from ex
             else:
                 raise CekitError(
                     "Could not copy resource '%s', "
                     "source path does not exist. "
                     "Make sure you provided correct path" % self.name
                 )
 
@@ -588,14 +593,17 @@
                 logger.debug(str(e))
                 logger.warning(
                     "Could not download artifact '{}' from Brew".format(self.name)
                 )
 
         raise CekitError("Artifact {} could not be found".format(self.name))
 
+    def _get_default_name_value(self, descriptor: RawResourceDescriptor) -> str:
+        return ""
+
 
 class _ImageContentResource(Resource):
     """
     Class to cover artifacts that should be fetched from images.
 
     Main purpose of this type of resources are artifacts built as
     part of multi-stage builds. Other use case is where the artifact
```

### Comparing `cekit-4.7.0/cekit/descriptor/run.py` & `cekit-4.8.0/cekit/descriptor/run.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/descriptor/volume.py` & `cekit-4.8.0/cekit/descriptor/volume.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/generator/base.py` & `cekit-4.8.0/cekit/generator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import tempfile
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 from urllib.parse import urlparse
 
 import yaml
 
 from jinja2 import Environment, FileSystemLoader
-from packaging.version import InvalidVersion, Version
+from packaging.version import InvalidVersion, Version, _BaseVersion
 from packaging.version import parse as parse_version
 
 from cekit.cekit_types import PathType
 from cekit.config import Config
 from cekit.descriptor import (
     Env,
     Image,
@@ -25,14 +25,15 @@
     Modules,
     Overrides,
     Repository,
     Resource,
 )
 from cekit.errors import CekitError
 from cekit.generator import legacy_version
+from cekit.generator.legacy_version import LegacyVersion
 from cekit.template_helper import TemplateHelper
 from cekit.tools import DependencyDefinition, Map, download_file, load_descriptor
 from cekit.version import __version__ as cekit_version
 
 if TYPE_CHECKING:
     from cekit.descriptor.modules import Install
 
@@ -528,15 +529,15 @@
             if ex.response.status_code == 401:
                 LOGGER.error(
                     (
                         "You are not authorized to use {} ODCS service. "
                         "Are you sure you have a valid Kerberos session?"
                     ).format(odcs_service_type)
                 )
-            raise CekitError("Could not create ODCS compose", ex)
+            raise CekitError("Could not create ODCS compose") from ex
 
         compose_id = compose.get("id", None)
 
         if not compose_id:
             raise CekitError(
                 "Invalid response from ODCS service: no compose id found: {}".format(
                     compose
@@ -727,31 +728,35 @@
         if version in modules:
             raise CekitError(
                 "Module '{}' with version '{}' already exists in module registry".format(
                     module.name, version
                 )
             )
 
-        default_version: Version = parse_version(self._defaults.get(module.name))
-        try:
-            current_version: Version = parse_version(version)
-            # This if block is only for Python3.6 compatibility which still might return
-            # a LegacyVersion and not throw an exception. LegacyVersion does not have
-            # that field so can be used to differentiate.
-            if not hasattr(current_version, "major"):
-                raise InvalidVersion
-            # If current module version is newer, we need to make it the new default
-            if current_version > default_version:
-                self._defaults[module.name] = version
-        except InvalidVersion:
-            LOGGER.error(
-                f"Module's '{module.name}' version '{version}' does not follow PEP 440 versioning scheme "
-                "(https://www.python.org/dev/peps/pep-0440) which should be followed in modules."
-            )
-
-            if legacy_version.parse(version) > legacy_version.parse(
-                self._defaults.get(module.name)
-            ):
-                self._defaults[module.name] = version
+        current_version: _BaseVersion = internal_parse_version(version, module.name)
+        default_version: _BaseVersion = internal_parse_version(
+            self._defaults.get(module.name), module.name
+        )
+
+        # If current module version is newer, we need to make it the new default
+        if current_version > default_version:
+            self._defaults[module.name] = version
 
         # Finally add the module to registry
         modules[version] = module
+
+
+def internal_parse_version(version: str, module_name: str) -> _BaseVersion:
+    try:
+        result: Version = parse_version(version)
+        # This if block is only for Python3.6 compatibility which still might return
+        # a LegacyVersion and not throw an exception. LegacyVersion does not have
+        # that field so can be used to differentiate.
+        if not hasattr(result, "major"):
+            raise InvalidVersion
+    except InvalidVersion:
+        LOGGER.error(
+            f"Module's '{module_name}' version '{version}' does not follow PEP 440 versioning "
+            "scheme (https://www.python.org/dev/peps/pep-0440) which should be followed in modules."
+        )
+        result: LegacyVersion = legacy_version.parse(version)
+    return result
```

### Comparing `cekit-4.7.0/cekit/generator/docker.py` & `cekit-4.8.0/cekit/generator/docker.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/generator/legacy_version.py` & `cekit-4.8.0/cekit/generator/legacy_version.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/generator/osbs.py` & `cekit-4.8.0/cekit/generator/osbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             descriptor_path, target, container_file, overrides
         )
 
     def init(self):
         super(OSBSGenerator, self).init()
 
         self._prepare_osbs_config_file(yaml.safe_dump, "container.yaml")
-        # TODO: Why do we use file.write here and yaml.dump above?
+        # As the CVP gating.yaml might use non-standard yaml format use file.write not yaml.dump
         self._prepare_osbs_config_file(
             lambda contents, file, **kwargs: file.write(contents), "gating.yaml"
         )
 
     def generate(self):
         # If extra directory exists (by default named 'osbs_extra') next to
         # the image descriptor, copy it contents to the target directory.
@@ -229,14 +229,18 @@
                             )
                         )
                         # OSBS by default downloads all artifacts to artifacts/<target_path>
                         artifact["target"] = os.path.join(
                             "artifacts", artifact["target"]
                         )
                     except Exception:
+                        logger.debug(
+                            "Caught exception when processing PlainResource",
+                            exc_info=True,
+                        )
                         logger.warning(
                             "Plain artifact {} could not be found in Brew, trying to handle it using lookaside cache".format(
                                 artifact["name"]
                             )
                         )
                         artifact.copy(target_dir)
                         # TODO: This is ugly, rewrite this!
```

### Comparing `cekit-4.7.0/cekit/log.py` & `cekit-4.8.0/cekit/log.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/template_helper.py` & `cekit-4.8.0/cekit/template_helper.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/templates/help.jinja` & `cekit-4.8.0/cekit/templates/help.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/templates/template.jinja` & `cekit-4.8.0/cekit/templates/template.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/test/behave_runner.py` & `cekit-4.8.0/cekit/test/behave_runner.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/test/behave_tester.py` & `cekit-4.8.0/cekit/test/behave_tester.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/test/collector.py` & `cekit-4.8.0/cekit/test/collector.py`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/cekit/tools.py` & `cekit-4.8.0/cekit/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     if "-" == descriptor:
         descriptor = click.get_text_stream("stdin").read()
         logger.debug("Read from stdin: {}".format(descriptor))
 
     try:
         data = yaml.safe_load(descriptor)
     except Exception as ex:
-        raise CekitError("Cannot load descriptor", ex)
+        raise CekitError("Cannot load descriptor") from ex
 
     if isinstance(data, str):
         logger.debug("Reading descriptor from '{}' file...".format(descriptor))
 
         if os.path.exists(descriptor):
             with open(descriptor, "r") as fh:
                 return yaml.safe_load(fh)
@@ -200,30 +200,24 @@
         "call",
         "--json-output",
         "listArchives",
         "checksum={}".format(md5),
         "type=maven",
     ]
 
-    logger.debug("Executing '{}'.".format(" ".join(list_archives_cmd)))
     try:
-        result = subprocess.run(
-            list_archives_cmd, capture_output=True, check=True, text=True
-        )
-    except subprocess.CalledProcessError as ex:
-        logger.error(
-            "{} Command stdout is '{}' with stderr '{}'".format(
-                ex, ex.stdout, ex.stderr
-            )
-        )
-        if ex.output is not None and "AuthError" in ex.output:
+        result = run_wrapper(list_archives_cmd, capture_output=True, check=True)
+    except CekitError as ex:
+        # noinspection PyTypeChecker
+        nested: subprocess.CalledProcessError = ex.__cause__
+        if nested.output is not None and "AuthError" in nested.output:
             logger.warning(
                 "Brew authentication failed, please make sure you have a valid Kerberos ticket"
             )
-        raise CekitError("Could not fetch archives for checksum {}".format(md5), ex)
+        raise CekitError(f"Could not fetch archives for checksum {md5}") from ex
 
     archives = yaml.safe_load(result.stdout)
 
     if not archives:
         raise CekitError(
             "Artifact with md5 checksum {} could not be found in Brew".format(md5)
         )
@@ -371,15 +365,15 @@
         )
     except subprocess.CalledProcessError as ex:
         logger.error(
             "{} Command stdout is '{}' with stderr '{}'".format(
                 ex, ex.stdout, ex.stderr
             )
         )
-        raise CekitError(exception_message, ex)
+        raise CekitError(exception_message) from ex
     if result.stdout:
         result.stdout = result.stdout.strip()
     if result.stderr:
         result.stderr = result.stderr.strip()
     return result
```

### Comparing `cekit-4.7.0/cekit.egg-info/PKG-INFO` & `cekit-4.8.0/cekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.7.0
+Version: 4.8.0
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.7.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.8.0.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.7.0/cekit.egg-info/SOURCES.txt` & `cekit-4.8.0/cekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/requirements.txt` & `cekit-4.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.7.0/setup.py` & `cekit-4.8.0/setup.py`

 * *Files identical despite different names*

