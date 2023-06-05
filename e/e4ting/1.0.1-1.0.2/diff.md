# Comparing `tmp/e4ting-1.0.1.tar.gz` & `tmp/e4ting-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e4ting-1.0.1.tar", last modified: Mon Jun  5 15:33:22 2023, max compression
+gzip compressed data, was "dist/e4ting-1.0.2.tar", last modified: Mon Jun  5 15:39:55 2023, max compression
```

## Comparing `e4ting-1.0.1.tar` & `e4ting-1.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 15:33:22.000000 e4ting-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/db/
--rw-r--r--   0 root         (0) root         (0)      271 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1013 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/db/utilredis.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/db/kaf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/server/
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/server/call.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/server/restful.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/server/rpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/net/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/net/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/net/iface.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/etc/
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/etc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/etc/utilyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/acl/
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/acl/base.py
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/acl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8574 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/task/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/task/master.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/task/celeryproxy.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/task/base.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/task/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/task/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting/log/
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/log/otherhandle.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-06-05 15:26:51.000000 e4ting-1.0.1/e4ting/log/general_log.py
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-05 15:33:22.000000 e4ting-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/auth/
--rwxr-xr-x   0 root         (0) root         (0)      102 2023-06-05 15:26:51.000000 e4ting-1.0.1/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12268 2023-06-05 15:26:51.000000 e4ting-1.0.1/auth/baseauth.py
--rwxr-xr-x   0 root         (0) root         (0)     1174 2023-06-05 15:26:51.000000 e4ting-1.0.1/auth/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     5005 2023-06-05 15:26:51.000000 e4ting-1.0.1/auth/authcore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/celerys/
--rwxr-xr-x   0 root         (0) root         (0)     1301 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/test.client.py
--rw-r--r--   0 root         (0) root         (0)     6445 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/wsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/celerys/tasks/
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/tasks/task.py
--rwxr-xr-x   0 root         (0) root         (0)    10115 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/tasks/server.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/tasks/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2917 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/app.py
--rwxr-xr-x   0 root         (0) root         (0)      802 2023-06-05 15:26:51.000000 e4ting-1.0.1/celerys/test.app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/url2img/
--rw-r--r--   0 root         (0) root         (0)     2102 2023-06-05 15:26:51.000000 e4ting-1.0.1/url2img/url2img.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-05 15:26:51.000000 e4ting-1.0.1/url2img/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-05 15:32:12.000000 e4ting-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/common/
--rw-r--r--   0 root         (0) root         (0)    11837 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilui.py
--rw-r--r--   0 root         (0) root         (0)    23304 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilwechat.py
--rwxr-xr-x   0 root         (0) root         (0)     2235 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/capture.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utiltask.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilparallel.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5421 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilmail.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilsamba.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilaliyun.py
--rw-r--r--   0 root         (0) root         (0)    24024 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilredis.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/weixin.py
--rwxr-xr-x   0 root         (0) root         (0)     9537 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/mongo.py
--rwxr-xr-x   0 root         (0) root         (0)    25061 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/util.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utilcache.py
--rw-r--r--   0 root         (0) root         (0)     5693 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/dbpoker.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utils.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/utildingtalk.py
--rw-r--r--   0 root         (0) root         (0)    12296 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/baserequest.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-05 15:26:51.000000 e4ting-1.0.1/common/ai.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/e4ting.egg-info/
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-05 15:33:21.000000 e4ting-1.0.1/e4ting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-05 15:33:21.000000 e4ting-1.0.1/e4ting.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 15:33:21.000000 e4ting-1.0.1/e4ting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1290 2023-06-05 15:33:21.000000 e4ting-1.0.1/e4ting.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:33:22.000000 e4ting-1.0.1/test/
--rw-r--r--   0 root         (0) root         (0)      447 2023-06-05 15:26:51.000000 e4ting-1.0.1/test/test_locals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 15:39:55.000000 e4ting-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/db/
+-rw-r--r--   0 root         (0) root         (0)      271 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/db/utilredis.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/db/kaf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/server/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/server/call.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/server/restful.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/server/rpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/net/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/net/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/net/iface.py
+-rw-r--r--   0 root         (0) root         (0)      586 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/etc/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/etc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/etc/utilyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/acl/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/acl/base.py
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/acl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/task/
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/task/master.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-06-05 15:38:41.000000 e4ting-1.0.2/e4ting/task/celeryproxy.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/task/base.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/task/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/task/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting/log/
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/log/otherhandle.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-06-05 15:26:51.000000 e4ting-1.0.2/e4ting/log/general_log.py
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-05 15:39:55.000000 e4ting-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      102 2023-06-05 15:26:51.000000 e4ting-1.0.2/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12268 2023-06-05 15:26:51.000000 e4ting-1.0.2/auth/baseauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     1174 2023-06-05 15:26:51.000000 e4ting-1.0.2/auth/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5005 2023-06-05 15:26:51.000000 e4ting-1.0.2/auth/authcore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/celerys/
+-rwxr-xr-x   0 root         (0) root         (0)     1301 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/test.client.py
+-rw-r--r--   0 root         (0) root         (0)     6445 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/wsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/celerys/tasks/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/tasks/task.py
+-rwxr-xr-x   0 root         (0) root         (0)    10115 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/tasks/server.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/tasks/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2917 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/app.py
+-rwxr-xr-x   0 root         (0) root         (0)      802 2023-06-05 15:26:51.000000 e4ting-1.0.2/celerys/test.app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/url2img/
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-06-05 15:26:51.000000 e4ting-1.0.2/url2img/url2img.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-05 15:26:51.000000 e4ting-1.0.2/url2img/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-05 15:39:12.000000 e4ting-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/common/
+-rw-r--r--   0 root         (0) root         (0)    11837 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilui.py
+-rw-r--r--   0 root         (0) root         (0)    23304 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilwechat.py
+-rwxr-xr-x   0 root         (0) root         (0)     2235 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/capture.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utiltask.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilparallel.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilmail.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilsamba.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilaliyun.py
+-rw-r--r--   0 root         (0) root         (0)    24024 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilredis.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/weixin.py
+-rwxr-xr-x   0 root         (0) root         (0)     9537 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/mongo.py
+-rwxr-xr-x   0 root         (0) root         (0)    25061 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/util.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utilcache.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/dbpoker.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/utildingtalk.py
+-rw-r--r--   0 root         (0) root         (0)    12296 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/baserequest.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-05 15:26:51.000000 e4ting-1.0.2/common/ai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-06-05 15:39:55.000000 e4ting-1.0.2/e4ting.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:39:55.000000 e4ting-1.0.2/test/
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-05 15:26:51.000000 e4ting-1.0.2/test/test_locals.py
```

### Comparing `e4ting-1.0.1/e4ting/db/utilredis.py` & `e4ting-1.0.2/e4ting/db/utilredis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/bin/env python3
 # -*- coding:utf-8 -*-
 """
     [模块名]
     Add By :antiy yuhai@antiy.cn 2023-05-18 14:34:21
 """
 from redis import Redis
-from lib import util
-# from lib.etc import MyRds
+from e4ting import util
+# from e4ting.etc import MyRds
 
 # r = MyRds()
 
 class RedisDB:
     def __init__(self, db, ip="", port=6379):
         self.ip = ip
         self.port = int(port)
```

### Comparing `e4ting-1.0.1/e4ting/db/kaf.py` & `e4ting-1.0.2/e4ting/db/kaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 """
 import sys,os
 import json,time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 
-from lib import log
-from lib import util
+from e4ting import log
+from e4ting import util
 from confluent_kafka import Consumer
 
 
 class Kafka:
 
     def __init__(self, ignore=True):
         self.ignore = ignore   # 是否忽略pull的报错
```

### Comparing `e4ting-1.0.1/e4ting/server/call.py` & `e4ting-1.0.2/e4ting/server/call.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 import sys,os
 import json,time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 
-from lib import log
+from e4ting import log
 import xmlrpc.client
 
 
 def client(server="http://localhost:8080"):
     # Create an XML-RPC client
     proxy = xmlrpc.client.ServerProxy(server)
     return proxy
```

### Comparing `e4ting-1.0.1/e4ting/server/restful.py` & `e4ting-1.0.2/e4ting/server/restful.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 
 import importlib
 import importlib.util
 import pkgutil
 
-from lib import log,util
+from e4ting import log,util
 
 from flask_restful import Resource
 
 @util.redef_return(ret=None)
 def find_api_class(module):
     for item_name in dir(module):
         item = getattr(module, item_name)
```

### Comparing `e4ting-1.0.1/e4ting/server/rpc.py` & `e4ting-1.0.2/e4ting/server/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys,os
 import json,time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 from functools  import partial
 
-from lib import log
+from e4ting import log
 
 from xmlrpc.server import SimpleXMLRPCServer
 from socketserver import ThreadingMixIn
 
 
 class ThreadXMLRPCServer(ThreadingMixIn, SimpleXMLRPCServer):
     pass
```

### Comparing `e4ting-1.0.1/e4ting/net/iface.py` & `e4ting-1.0.2/e4ting/net/iface.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 """
 import sys,os
 import json,time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 
-from lib import log
-from lib import util
+from e4ting import log
+from e4ting import util
 
 def cat(fname):
     return open(fname).read().strip()
 
 class IFace():
     """网卡列表原生操作，不依赖第三方库"""
     def __init__(self, name):
```

### Comparing `e4ting-1.0.1/e4ting/__init__.py` & `e4ting-1.0.2/e4ting/__init__.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/etc/__init__.py` & `e4ting-1.0.2/e4ting/etc/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 import sys, os
 import json, time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 
-from lib import util
+from e4ting import util
 
 class Setting():
     def __init__(self):
         # 配置有可能发生变化，应该时刻保持最新
         pass
 
     @classmethod
```

### Comparing `e4ting-1.0.1/e4ting/etc/utilyaml.py` & `e4ting-1.0.2/e4ting/etc/utilyaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         return ret
 
     def __getattr__(self, attr):
         return self.sec.get(attr)
 
     def __setattr__(self, attr, value):
-        from lib import log
+        from e4ting import log
         log.info("{self.etc} [{self.section}] {attr} = {value}".format(self=self, attr=attr, value=value))
         self.sec.update({attr : value})
         self.etc.content.update({self.section : self.sec})
         self.etc.save()
 
     def __repr__(self):
         return "[{self.etc.yaml_path}]-[{self.section}]:{keys}".format(self=self,keys=self.keys())
```

### Comparing `e4ting-1.0.1/e4ting/acl/base.py` & `e4ting-1.0.2/e4ting/acl/base.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/util.py` & `e4ting-1.0.2/e4ting/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     import sys
     path, args, kwargs = params
     # log.info(os.path.join(path, "opt/rh/rh-python38/root/usr/local/lib64/python3.8/site-packages"))
     # log.info(sys.executable)
     # log.info(os.path.exists(sys.executable))
     # with chroot(path):
     # sys.path.append(os.path.join(path, "opt/rh/rh-python38/root/usr/local/lib64/python3.8/site-packages"))
-    # sys.path.append(os.path.join(path, "opt/rh/rh-python38/root/usr/local/lib/python3.8/site-packages"))
+    # sys.path.append(os.path.join(path, "opt/rh/rh-python38/root/usr/local/e4ting/python3.8/site-packages"))
     for _ in path:
         sys.path.append(_)
     ret = sys.otherfunc(*args, **kwargs)
     return ret
 
 def get_root(name, python):
     cmd = """docker inspect -f "/proc/{{.State.Pid}}/root" %(name)s""" % dict(name=name)
```

### Comparing `e4ting-1.0.1/e4ting/task/master.py` & `e4ting-1.0.2/e4ting/task/master.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 
 import consul
 import uuid
 import json
 
-from lib import log
+from e4ting import log
 
 class Scheduler:
     def __init__(self, consul_host, consul_port, task_prefix):
         self.consul_client = consul.Consul(host=consul_host, port=consul_port, token="")
         self.task_prefix = task_prefix
 
     def submit_task(self, task_func, task_args, task_id = str(uuid.uuid4())):
```

### Comparing `e4ting-1.0.1/e4ting/task/celeryproxy.py` & `e4ting-1.0.2/e4ting/task/celeryproxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys,os
 import json,time
 from pdb import set_trace as strace
 from traceback  import format_exc as dumpstack
 from textwrap import dedent
 from functools import partial
 
-from lib import log
+from e4ting import log
 
 
 def imports(app):
     globals()["app"] = app
     for mod in app.conf['include']:
         try:
             exec('from {mod} import *'.format(mod=mod), globals())
```

### Comparing `e4ting-1.0.1/e4ting/task/base.py` & `e4ting-1.0.2/e4ting/task/base.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/task/worker.py` & `e4ting-1.0.2/e4ting/task/worker.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/log/__init__.py` & `e4ting-1.0.2/e4ting/log/__init__.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/log/otherhandle.py` & `e4ting-1.0.2/e4ting/log/otherhandle.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting/log/general_log.py` & `e4ting-1.0.2/e4ting/log/general_log.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/auth/baseauth.py` & `e4ting-1.0.2/auth/baseauth.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/auth/__main__.py` & `e4ting-1.0.2/auth/__main__.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/auth/authcore.py` & `e4ting-1.0.2/auth/authcore.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/test.client.py` & `e4ting-1.0.2/celerys/test.client.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/__init__.py` & `e4ting-1.0.2/celerys/__init__.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/wsapp.py` & `e4ting-1.0.2/celerys/wsapp.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/tasks/task.py` & `e4ting-1.0.2/celerys/tasks/task.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/tasks/server.py` & `e4ting-1.0.2/celerys/tasks/server.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/app.py` & `e4ting-1.0.2/celerys/app.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/celerys/test.app.py` & `e4ting-1.0.2/celerys/test.app.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/url2img/url2img.py` & `e4ting-1.0.2/url2img/url2img.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/setup.py` & `e4ting-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def run(self):
         install.run(self)
         # 添加命令
         print("打包完成")
 
 setup(
     name='e4ting',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages() + [ "e4ting.acl.models" ],
     package_data={
         'e4ting.acl.models': ['admin.policy', 'admin.model'],
     },
     include_package_data=True,
     # packages=find_packages(),  #  找到目录下所有的包
     # 需要的依赖包list
```

### Comparing `e4ting-1.0.1/common/utilui.py` & `e4ting-1.0.2/common/utilui.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilwechat.py` & `e4ting-1.0.2/common/utilwechat.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/capture.py` & `e4ting-1.0.2/common/capture.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utiltask.py` & `e4ting-1.0.2/common/utiltask.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilparallel.py` & `e4ting-1.0.2/common/utilparallel.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilmail.py` & `e4ting-1.0.2/common/utilmail.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilsamba.py` & `e4ting-1.0.2/common/utilsamba.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilaliyun.py` & `e4ting-1.0.2/common/utilaliyun.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilredis.py` & `e4ting-1.0.2/common/utilredis.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/weixin.py` & `e4ting-1.0.2/common/weixin.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/mongo.py` & `e4ting-1.0.2/common/mongo.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/util.py` & `e4ting-1.0.2/common/util.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utilcache.py` & `e4ting-1.0.2/common/utilcache.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/dbpoker.py` & `e4ting-1.0.2/common/dbpoker.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utils.py` & `e4ting-1.0.2/common/utils.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/utildingtalk.py` & `e4ting-1.0.2/common/utildingtalk.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/baserequest.py` & `e4ting-1.0.2/common/baserequest.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/common/ai.py` & `e4ting-1.0.2/common/ai.py`

 * *Files identical despite different names*

### Comparing `e4ting-1.0.1/e4ting.egg-info/SOURCES.txt` & `e4ting-1.0.2/e4ting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

