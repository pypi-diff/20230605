# Comparing `tmp/helloPypi-topic-0.0.5.tar.gz` & `tmp/helloPypi-topic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloPypi-topic-0.0.5.tar", last modified: Sun Jun  4 20:11:37 2023, max compression
+gzip compressed data, was "helloPypi-topic-0.0.6.tar", last modified: Sun Jun  4 22:47:24 2023, max compression
```

## Comparing `helloPypi-topic-0.0.5.tar` & `helloPypi-topic-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/PKG-INFO
-drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.865241 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      241 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/top_level.txt
-drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.865241 helloPypi-topic-0.0.5/myhellopackage/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       79 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/channel.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       41 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/hello.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      218 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/setup.py
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 22:47:24.240295 helloPypi-topic-0.0.6/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 22:47:24.240295 helloPypi-topic-0.0.6/PKG-INFO
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 22:47:24.236295 helloPypi-topic-0.0.6/helloPypi_topic.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 22:47:24.000000 helloPypi-topic-0.0.6/helloPypi_topic.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      241 2023-06-04 22:47:24.000000 helloPypi-topic-0.0.6/helloPypi_topic.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-04 22:47:24.000000 helloPypi-topic-0.0.6/helloPypi_topic.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2023-06-04 22:47:24.000000 helloPypi-topic-0.0.6/helloPypi_topic.egg-info/top_level.txt
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 22:47:24.240295 helloPypi-topic-0.0.6/myhellopackage/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 22:46:14.000000 helloPypi-topic-0.0.6/myhellopackage/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       79 2023-06-04 22:46:14.000000 helloPypi-topic-0.0.6/myhellopackage/channel.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       41 2023-06-04 22:46:14.000000 helloPypi-topic-0.0.6/myhellopackage/hello.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-04 22:47:24.240295 helloPypi-topic-0.0.6/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      218 2023-06-04 22:47:23.000000 helloPypi-topic-0.0.6/setup.py
```

