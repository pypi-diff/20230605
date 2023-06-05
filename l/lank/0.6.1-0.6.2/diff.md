# Comparing `tmp/lank-0.6.1.tar.gz` & `tmp/lank-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lank-0.6.1.tar", last modified: Sun May 28 23:42:08 2023, max compression
+gzip compressed data, was "lank-0.6.2.tar", last modified: Mon Jun  5 01:32:41 2023, max compression
```

## Comparing `lank-0.6.1.tar` & `lank-0.6.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.783802 lank-0.6.1/
--rw-r--r--   0 shawn     (1000) shawn     (1000)       82 2023-03-18 00:58:16.000000 lank-0.6.1/.gitignore
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2486 2023-03-28 20:57:22.000000 lank-0.6.1/CHANGELOG
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1102 2022-07-10 22:31:07.000000 lank-0.6.1/LICENSE
--rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-05-28 23:42:08.783802 lank-0.6.1/PKG-INFO
--rw-r--r--   0 shawn     (1000) shawn     (1000)      352 2022-07-10 22:32:02.000000 lank-0.6.1/README.md
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.750801 lank-0.6.1/lank/
--rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2022-06-14 19:59:08.000000 lank-0.6.1/lank/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:26.000000 lank-0.6.1/lank/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)       23 2023-03-20 20:11:21.000000 lank-0.6.1/lank/__version__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1397 2023-03-20 09:45:57.000000 lank-0.6.1/lank/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      295 2022-07-01 02:40:05.000000 lank-0.6.1/lank/config.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.761801 lank-0.6.1/lank/crypto/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1285 2023-03-23 13:33:21.000000 lank-0.6.1/lank/crypto/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5119 2023-03-28 20:53:35.000000 lank-0.6.1/lank/crypto/v1.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      321 2023-03-23 15:20:04.000000 lank-0.6.1/lank/crypto/v2.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.767801 lank-0.6.1/lank/gateway/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7594 2023-05-28 23:41:18.000000 lank-0.6.1/lank/gateway/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2023-03-18 00:54:57.000000 lank-0.6.1/lank/gateway/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      846 2023-03-20 11:36:36.000000 lank-0.6.1/lank/gateway/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5715 2023-03-23 12:35:35.000000 lank-0.6.1/lank/gateway/node.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5399 2023-03-28 20:46:20.000000 lank-0.6.1/lank/gateway/peer.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)       27 2022-07-09 17:02:10.000000 lank-0.6.1/lank/name.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.769801 lank-0.6.1/lank/node/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     9199 2023-03-23 15:09:01.000000 lank-0.6.1/lank/node/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:11:43.000000 lank-0.6.1/lank/node/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1836 2023-03-20 09:47:34.000000 lank-0.6.1/lank/node/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7216 2022-07-10 18:21:31.000000 lank-0.6.1/lank/node/db.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.771802 lank-0.6.1/lank/node/patch/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2035 2022-06-16 19:44:28.000000 lank-0.6.1/lank/node/patch/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1305 2022-06-17 06:07:47.000000 lank-0.6.1/lank/node/patch/v2.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1217 2022-07-01 03:06:08.000000 lank-0.6.1/lank/node/patch/v3.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      220 2022-07-07 20:36:15.000000 lank-0.6.1/lank/node/patch/v4.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.777802 lank-0.6.1/lank/node/protocol/
--rw-r--r--   0 shawn     (1000) shawn     (1000)    24186 2023-03-28 08:23:56.000000 lank-0.6.1/lank/node/protocol/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      175 2023-03-20 06:28:41.000000 lank-0.6.1/lank/node/protocol/ack.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     6283 2023-03-28 12:30:29.000000 lank-0.6.1/lank/node/protocol/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      356 2023-03-20 07:56:21.000000 lank-0.6.1/lank/node/protocol/deny.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     9134 2023-03-22 03:33:44.000000 lank-0.6.1/lank/node/protocol/peer.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     4671 2023-03-20 09:08:41.000000 lank-0.6.1/lank/node/protocol/register.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     6406 2023-03-20 08:40:23.000000 lank-0.6.1/lank/node/protocol/sync.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.780802 lank-0.6.1/lank/peer/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2310 2023-03-28 11:33:24.000000 lank-0.6.1/lank/peer/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:11.000000 lank-0.6.1/lank/peer/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2345 2022-07-14 23:13:40.000000 lank-0.6.1/lank/peer/cmd.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.782802 lank-0.6.1/lank/peer/protocol/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     3527 2023-03-28 12:57:14.000000 lank-0.6.1/lank/peer/protocol/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2080 2023-03-28 20:50:42.000000 lank-0.6.1/lank/peer/protocol/ack.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5590 2023-03-28 13:03:53.000000 lank-0.6.1/lank/peer/protocol/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1167 2023-03-28 13:07:57.000000 lank-0.6.1/lank/peer/protocol/media.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1393 2023-03-28 11:24:26.000000 lank-0.6.1/lank/peer/protocol/wrap.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     3122 2022-06-26 01:34:59.000000 lank-0.6.1/lank/peer/test.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)    12542 2023-05-28 23:41:18.000000 lank-0.6.1/lank/registration.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      106 2023-03-20 09:47:19.000000 lank-0.6.1/lank/util.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.753801 lank-0.6.1/lank.egg-info/
--rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/PKG-INFO
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1119 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/SOURCES.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)        1 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/dependency_links.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)      119 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/entry_points.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       81 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/requires.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)        5 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/top_level.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       63 2022-06-14 21:35:01.000000 lank-0.6.1/requirements.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2023-05-28 23:42:08.783802 lank-0.6.1/setup.cfg
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1735 2023-03-20 09:31:14.000000 lank-0.6.1/setup.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.087873 lank-0.6.2/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       82 2023-03-18 00:58:16.000000 lank-0.6.2/.gitignore
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2556 2023-06-05 01:31:44.000000 lank-0.6.2/CHANGELOG
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1102 2022-07-10 22:31:07.000000 lank-0.6.2/LICENSE
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-06-05 01:32:41.087873 lank-0.6.2/PKG-INFO
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      352 2022-07-10 22:32:02.000000 lank-0.6.2/README.md
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.067873 lank-0.6.2/lank/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2022-06-14 19:59:08.000000 lank-0.6.2/lank/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:26.000000 lank-0.6.2/lank/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       23 2023-06-05 01:16:34.000000 lank-0.6.2/lank/__version__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1397 2023-03-20 09:45:57.000000 lank-0.6.2/lank/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      295 2022-07-01 02:40:05.000000 lank-0.6.2/lank/config.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.069873 lank-0.6.2/lank/crypto/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1285 2023-03-23 13:33:21.000000 lank-0.6.2/lank/crypto/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5119 2023-03-28 20:53:35.000000 lank-0.6.2/lank/crypto/v1.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      321 2023-03-23 15:20:04.000000 lank-0.6.2/lank/crypto/v2.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.073873 lank-0.6.2/lank/gateway/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7594 2023-05-28 23:41:18.000000 lank-0.6.2/lank/gateway/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2023-03-18 00:54:57.000000 lank-0.6.2/lank/gateway/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      846 2023-03-20 11:36:36.000000 lank-0.6.2/lank/gateway/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5715 2023-03-23 12:35:35.000000 lank-0.6.2/lank/gateway/node.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5399 2023-03-28 20:46:20.000000 lank-0.6.2/lank/gateway/peer.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       27 2022-07-09 17:02:10.000000 lank-0.6.2/lank/name.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.074873 lank-0.6.2/lank/node/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9199 2023-03-23 15:09:01.000000 lank-0.6.2/lank/node/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:11:43.000000 lank-0.6.2/lank/node/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1836 2023-03-20 09:47:34.000000 lank-0.6.2/lank/node/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7216 2022-07-10 18:21:31.000000 lank-0.6.2/lank/node/db.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.078873 lank-0.6.2/lank/node/patch/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2035 2022-06-16 19:44:28.000000 lank-0.6.2/lank/node/patch/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1305 2022-06-17 06:07:47.000000 lank-0.6.2/lank/node/patch/v2.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1217 2022-07-01 03:06:08.000000 lank-0.6.2/lank/node/patch/v3.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      220 2022-07-07 20:36:15.000000 lank-0.6.2/lank/node/patch/v4.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.083873 lank-0.6.2/lank/node/protocol/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)    24206 2023-06-05 01:15:17.000000 lank-0.6.2/lank/node/protocol/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      175 2023-03-20 06:28:41.000000 lank-0.6.2/lank/node/protocol/ack.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     6283 2023-03-28 12:30:29.000000 lank-0.6.2/lank/node/protocol/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      356 2023-03-20 07:56:21.000000 lank-0.6.2/lank/node/protocol/deny.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9134 2023-03-22 03:33:44.000000 lank-0.6.2/lank/node/protocol/peer.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     4671 2023-03-20 09:08:41.000000 lank-0.6.2/lank/node/protocol/register.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     6406 2023-03-20 08:40:23.000000 lank-0.6.2/lank/node/protocol/sync.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.084873 lank-0.6.2/lank/peer/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2310 2023-03-28 11:33:24.000000 lank-0.6.2/lank/peer/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:11.000000 lank-0.6.2/lank/peer/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2345 2022-07-14 23:13:40.000000 lank-0.6.2/lank/peer/cmd.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.087873 lank-0.6.2/lank/peer/protocol/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3527 2023-03-28 12:57:14.000000 lank-0.6.2/lank/peer/protocol/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2080 2023-03-28 20:50:42.000000 lank-0.6.2/lank/peer/protocol/ack.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5590 2023-03-28 13:03:53.000000 lank-0.6.2/lank/peer/protocol/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1167 2023-03-28 13:07:57.000000 lank-0.6.2/lank/peer/protocol/media.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1393 2023-03-28 11:24:26.000000 lank-0.6.2/lank/peer/protocol/wrap.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3122 2022-06-26 01:34:59.000000 lank-0.6.2/lank/peer/test.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)    12542 2023-05-28 23:41:18.000000 lank-0.6.2/lank/registration.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      106 2023-03-20 09:47:19.000000 lank-0.6.2/lank/util.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-06-05 01:32:41.068873 lank-0.6.2/lank.egg-info/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/PKG-INFO
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1119 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        1 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      119 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/entry_points.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       81 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/requires.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        5 2023-06-05 01:32:41.000000 lank-0.6.2/lank.egg-info/top_level.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       63 2022-06-14 21:35:01.000000 lank-0.6.2/requirements.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2023-06-05 01:32:41.087873 lank-0.6.2/setup.cfg
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1735 2023-03-20 09:31:14.000000 lank-0.6.2/setup.py
```

### Comparing `lank-0.6.1/CHANGELOG` & `lank-0.6.2/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Copyright (C) 2022-2023 LANNOCC (Shawn A. Wilson [lannocc@yahoo.com])
 @%@~LICENSE:MIT~@%@
 
+saw_060423_1 - Fix registration that was broken in the last release.
+
 saw_032823_1 - Lots of work on gateway/peer. Begin some crypto upgrades.
 
 saw_032123_2 - Fixes for the last commit.
 
 saw_032123_1 - Upate GetHistory message to allow for filtering by name.
 
 saw_032023_5 - Registration upgraded. Note that peer stuff is still broken.
```

### Comparing `lank-0.6.1/LICENSE` & `lank-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/PKG-INFO` & `lank-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lank
-Version: 0.6.1
+Version: 0.6.2
 Summary: Listening Anchor Nodes for K
 Home-page: https://github.com/lannocc/lank
 Author: LANNOCC (Shawn A. Wilson)
 Author-email: lannocc@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lank-0.6.1/lank/cmd.py` & `lank-0.6.2/lank/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/crypto/__init__.py` & `lank-0.6.2/lank/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/crypto/v1.py` & `lank-0.6.2/lank/crypto/v1.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/gateway/__init__.py` & `lank-0.6.2/lank/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/gateway/cmd.py` & `lank-0.6.2/lank/gateway/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/gateway/node.py` & `lank-0.6.2/lank/gateway/node.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/gateway/peer.py` & `lank-0.6.2/lank/gateway/peer.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/__init__.py` & `lank-0.6.2/lank/node/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/cmd.py` & `lank-0.6.2/lank/node/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/db.py` & `lank-0.6.2/lank/node/db.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/patch/__init__.py` & `lank-0.6.2/lank/node/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/patch/v2.py` & `lank-0.6.2/lank/node/patch/v2.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/patch/v3.py` & `lank-0.6.2/lank/node/patch/v3.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/protocol/__init__.py` & `lank-0.6.2/lank/node/protocol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             else: # just an echo from another node?
                 pass
 
         elif master.ldb.get_label_by_name(msg.label):
             reply = ReservationCancel(msg.label, True)
 
         else:
-            reservation = (msg.uuid, self.sock, master.now())
+            reservation = (msg.uuid, self.addr, master.now())
             master.reservations[msg.label] = reservation
             await master.broadcast_nodes(msg, skip=self)
             if not self.node_uuid: reply = msg
 
         return reply
 
     async def reservation_cancel(self, master, msg):
@@ -381,23 +381,24 @@
             return NodeIsIsolated()
 
         if msg.label not in master.reservations:
             return ReservationRequired(msg.label)
 
         reservation = master.reservations[msg.label]
         res_uuid = reservation[0]
-        res_sock = reservation[1]
+        res_addr = reservation[1]
 
-        #FIXME sock
-        #if res_sock != self.sock: # imposter
-        #    return ReservationRequired(msg.label)
+        #FIXME enable imposter checks?
 
         #if res_uuid != msg.uuid: # imposter
         #    return ReservationRequired(msg.label)
 
+        #if res_addr != self.addr: # imposter
+        #    return ReservationRequired(msg.label)
+
         crypto = get_crypto(msg.version)
         pub_key = crypto.load_public_key(msg.key_pair_pem)
         data = crypto.get_register_message(msg.label, msg.time_nonce)
 
         if not crypto.verify(pub_key, data, msg.signature):
             return SignatureFailure(msg.uuid)
```

### Comparing `lank-0.6.1/lank/node/protocol/base.py` & `lank-0.6.2/lank/node/protocol/base.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/protocol/peer.py` & `lank-0.6.2/lank/node/protocol/peer.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/protocol/register.py` & `lank-0.6.2/lank/node/protocol/register.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/node/protocol/sync.py` & `lank-0.6.2/lank/node/protocol/sync.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/__init__.py` & `lank-0.6.2/lank/peer/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/cmd.py` & `lank-0.6.2/lank/peer/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/protocol/__init__.py` & `lank-0.6.2/lank/peer/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/protocol/ack.py` & `lank-0.6.2/lank/peer/protocol/ack.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/protocol/base.py` & `lank-0.6.2/lank/peer/protocol/base.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/protocol/media.py` & `lank-0.6.2/lank/peer/protocol/media.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/protocol/wrap.py` & `lank-0.6.2/lank/peer/protocol/wrap.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/peer/test.py` & `lank-0.6.2/lank/peer/test.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank/registration.py` & `lank-0.6.2/lank/registration.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/lank.egg-info/PKG-INFO` & `lank-0.6.2/lank.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lank
-Version: 0.6.1
+Version: 0.6.2
 Summary: Listening Anchor Nodes for K
 Home-page: https://github.com/lannocc/lank
 Author: LANNOCC (Shawn A. Wilson)
 Author-email: lannocc@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lank-0.6.1/lank.egg-info/SOURCES.txt` & `lank-0.6.2/lank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lank-0.6.1/setup.py` & `lank-0.6.2/setup.py`

 * *Files identical despite different names*

