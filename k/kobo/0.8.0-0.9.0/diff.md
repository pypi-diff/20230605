# Comparing `tmp/kobo-0.8.0.tar.bz2` & `tmp/kobo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-bzip2 compressed data, block size = 900k
+gzip compressed data, was "dist/kobo-0.9.0.tar", last modified: Sun Jan 13 22:56:04 2019, max compression
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-Bzip2File
+GzipFile
```

## Comparing `kobo-0.8.0.tar` & `kobo-0.9.0.tar`

### file list

```diff
@@ -1,269 +1,275 @@
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    26436 2018-05-22 23:00:52.000000 kobo-0.8.0/LICENSE
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     2181 2018-11-28 03:17:09.000000 kobo-0.8.0/setup.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      305 2018-11-28 03:23:25.000000 kobo-0.8.0/PKG-INFO
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      813 2018-05-22 23:00:52.000000 kobo-0.8.0/COPYING
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      453 2018-05-22 23:00:52.000000 kobo-0.8.0/INSTALL
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6082 2018-11-26 06:05:49.000000 kobo-0.8.0/README.md
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      839 2018-11-26 05:58:39.000000 kobo-0.8.0/Makefile
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      625 2018-05-22 23:00:52.000000 kobo-0.8.0/AUTHORS
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/tests/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3623 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/rpc.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     7694 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_types.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12526 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_main.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     4407 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_plugins.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8259 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_taskbase.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     2873 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_tback.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2906 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_middleware.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      627 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_decorators.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    17131 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_view_log.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1927 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_utf8_chunk.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1024 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_fields.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1678 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_tail.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1307 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_http.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     5486 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_conf.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1379 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/utils.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13398 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_xmlrpc_client.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      111 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/chunks_file
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)    17143 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_shortcuts.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3190 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_logger.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1990 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_hardlink.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      418 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/hub_urls.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     9320 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_pkgset.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    38612 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_xmlrpc_worker.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/tests/plugins/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      108 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/plugins/plug_working.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/plugins/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      132 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/plugins/plug_broken.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/__init__.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)    10984 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_rpmlib.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5078 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_task_logs.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/tests/fields_test/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/tests/fields_test/fixtures/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      149 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/fields_test/fixtures/initial_data.json
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     3177 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/fields_test/tests.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       23 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/fields_test/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      327 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/fields_test/models.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      205 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/fields_test/settings.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1353 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/settings.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    31288 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_taskmanager.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/tests/data/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1592 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/data/dummy-basesystem-10.0-6.noarch.rpm
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2099 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/data/dummy-AdobeReader_enu-9.5.1-1.nosrc.rpm
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1814 2018-05-22 23:00:52.000000 kobo-0.8.0/tests/data/dummy-basesystem-10.0-6.src.rpm
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      573 2018-11-26 05:58:39.000000 kobo-0.8.0/tests/test_log.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      298 2018-11-26 05:58:39.000000 kobo-0.8.0/MANIFEST.in
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     9352 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/types.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/xmlrpc/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      128 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/xmlrpc/apps.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4499 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/hub/xmlrpc/client.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1108 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/xmlrpc/auth.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      110 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/xmlrpc/system.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8410 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/hub/xmlrpc/worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       48 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/xmlrpc/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1188 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/forms.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/static/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/static/kobo/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/static/kobo/css/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4095 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/css/screen.css
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/static/kobo/img/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      201 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-first.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      191 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-prev.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      204 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-last-disabled.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      201 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-first-disabled.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      204 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-last.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      194 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-prev-disabled.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      191 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-next.png
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      282 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/img/list-next-disabled.png
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/static/kobo/js/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1770 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/static/kobo/js/log_watcher.js
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1100 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/admin.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/task/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      652 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/task/log.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2810 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/task/detail.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      483 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/task/list.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      888 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/task/list_include.html
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/arch/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      425 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/arch/detail.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      223 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/arch/list.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      310 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/arch/list_include.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1122 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/pagination.html
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/worker/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1278 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/worker/detail.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      227 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/worker/list.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      891 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/worker/list_include.html
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/user/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      928 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/user/detail.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      223 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/user/list.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      772 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/user/list_include.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      285 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/500.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      330 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/base.html.example
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      199 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/404.html
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/channel/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      440 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/channel/detail.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      229 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/channel/list.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      328 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/channel/list_include.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1586 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/layout.html
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/templates/auth/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      726 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/templates/auth/login.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8803 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/views.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/urls/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      310 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/auth.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      607 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/user.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      770 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/channel.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      997 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/task.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      583 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/arch.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      739 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/urls/__init__.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/migrations/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1367 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/migrations/0002_auto_20150722_0612.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      658 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/migrations/0003_auto_20160202_0647.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5311 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/migrations/0001_initial.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/migrations/__init__.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/fixtures/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1827 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/fixtures/data.json
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/hub/sql/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       95 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/sql/task.postgresql.sql
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      232 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/menu.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      725 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/decorators.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1055 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      997 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hub/middleware.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    37360 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/hub/models.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4381 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/http.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5885 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/plugins.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/client/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      959 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/constants.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      777 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/default.conf
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/client/commands/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1005 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_cancel_tasks.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1386 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_enable_worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2482 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_watch_log.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1036 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_shutdown_worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      950 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_add_user.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1234 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_resubmit_tasks.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2419 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_create_task.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      975 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_worker_info.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      647 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_watch_tasks.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1390 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_disable_worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      742 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_list_workers.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2410 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/commands/cmd_list_tasks.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4837 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/task_watcher.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      433 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/main.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12914 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/client/__init__.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/xmlrpc/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      166 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/admin.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6236 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/views.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2560 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/auth.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/xmlrpc/migrations/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      814 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/migrations/0001_initial.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/migrations/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4143 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/decorators.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3747 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/dispatcher.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/xmlrpc/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      505 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/django/xmlrpc/models.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2278 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/forms.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/views/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3238 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/views/generic.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/views/__init__.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/upload/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      405 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/admin.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      165 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/urls.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2595 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/views.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1016 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/xmlrpc.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2969 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/upload/models.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/menu/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      305 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/menu/context_processors.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    11042 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/menu/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      695 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/menu/middleware.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6430 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/fields.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/auth/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       40 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/admin.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      159 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/apps.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/django/auth/migrations/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      521 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/migrations/0002_LongnameUser.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2847 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/migrations/0001_initial.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/migrations/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1587 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/krb5.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       56 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      512 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/middleware.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2630 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/django/auth/models.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    10815 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/tback.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/worker/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1107 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/default.conf
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3167 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/main.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3727 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/task.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2426 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/logger.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      184 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/__init__.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/worker/tasks/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      568 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/tasks/task_shutdown_worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/worker/tasks/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    19597 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/worker/taskmanager.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    11766 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/conf.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12171 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/cli.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5691 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/log.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8167 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/pkgset.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4488 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/threads.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13992 2018-11-26 05:58:39.000000 kobo-0.8.0/kobo/shortcuts.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13201 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/rpmlib.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    25773 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/xmlrpc.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      309 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/exceptions.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2084 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/decorators.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8699 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/process.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/__init__.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     3204 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/notification.py
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/hub/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/hub/xmlrpc/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      521 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/xmlrpc/urls.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/xmlrpc/__init__.py.template
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/hub/templates/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      117 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/templates/index.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      604 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/templates/base.html
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      329 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/__project_name__.wsgi
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5516 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/settings.py.template
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      546 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/manage.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1906 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/urls.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1407 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/menu.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1292 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/__project_name__-httpd.conf
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/__init__.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1031 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/hub/settings_local.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      988 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/task___project_name__.py.template
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/client/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      879 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/client/__project_name__.conf
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/client/commands/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/client/commands/__init__.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/client/__init__.py.template
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1829 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/client/__project_name__
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/worker/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1251 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/worker/__project_name__.conf
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/worker/__init__.py.template
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/worker/tasks/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/worker/tasks/__init__.py.template
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1493 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/worker/__project_name__
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1235 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/client@cmd___project_name__.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1083 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/cli@cmd___project_name__.py.template
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/cli/
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/templates/cli/commands/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/cli/commands/__init__.py.template
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/cli/__init__.py.template
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1463 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/templates/cli/__project_name__
-drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2018-11-28 03:23:25.000000 kobo-0.8.0/kobo/admin/commands/
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      817 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_worker_task.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1347 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_hub.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      845 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_client.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      826 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_cli_command.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      839 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_client_command.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      660 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_worker.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      778 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/commands/cmd_start_cli.py
--rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      134 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/kobo-admin
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3779 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/admin/__init__.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     7224 2018-05-22 23:00:52.000000 kobo-0.8.0/kobo/hardlink.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    26436 2019-01-04 04:23:14.000000 kobo-0.9.0/LICENSE
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     2181 2019-01-13 22:49:38.000000 kobo-0.9.0/setup.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      305 2019-01-13 22:56:04.000000 kobo-0.9.0/PKG-INFO
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      813 2019-01-04 04:23:14.000000 kobo-0.9.0/COPYING
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      453 2019-01-04 04:23:14.000000 kobo-0.9.0/INSTALL
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6435 2019-01-13 22:50:02.000000 kobo-0.9.0/README.md
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      839 2019-01-04 04:23:24.000000 kobo-0.9.0/Makefile
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      625 2019-01-04 04:23:14.000000 kobo-0.9.0/AUTHORS
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/tests/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3623 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/rpc.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     7694 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_types.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12526 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_main.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     4407 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_plugins.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      262 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_xmlrpc_system.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8259 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_taskbase.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     2873 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_tback.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2906 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_middleware.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    53193 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_models.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2087 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_xmlrpc_auth.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      627 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_decorators.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    16473 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_view_log.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1927 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_utf8_chunk.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     9020 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_forms.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1024 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_fields.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1678 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_tail.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1307 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_http.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     5486 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_conf.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1926 2019-01-07 04:44:11.000000 kobo-0.9.0/tests/utils.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13398 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_xmlrpc_client.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      111 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/chunks_file
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)    17143 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_shortcuts.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2965 2019-01-13 22:21:10.000000 kobo-0.9.0/tests/test_logger.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1990 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_hardlink.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     7885 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_views.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      664 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/hub_urls.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     9320 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_pkgset.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    38612 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_xmlrpc_worker.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/tests/plugins/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      108 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/plugins/plug_working.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/plugins/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      132 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/plugins/plug_broken.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/__init__.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)    10984 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_rpmlib.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5078 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_task_logs.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      830 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_task_shutdown_worker.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/tests/fields_test/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/tests/fields_test/fixtures/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      149 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/fields_test/fixtures/initial_data.json
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     3177 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/fields_test/tests.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       23 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/fields_test/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      327 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/fields_test/models.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      205 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/fields_test/settings.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1475 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/settings.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    32408 2019-01-13 22:23:11.000000 kobo-0.9.0/tests/test_taskmanager.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/tests/data/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1592 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/data/dummy-basesystem-10.0-6.noarch.rpm
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2099 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/data/dummy-AdobeReader_enu-9.5.1-1.nosrc.rpm
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1814 2019-01-04 04:23:14.000000 kobo-0.9.0/tests/data/dummy-basesystem-10.0-6.src.rpm
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      573 2019-01-04 04:23:24.000000 kobo-0.9.0/tests/test_log.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      298 2019-01-04 04:23:24.000000 kobo-0.9.0/MANIFEST.in
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     9352 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/types.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/xmlrpc/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      128 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/xmlrpc/apps.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4499 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/xmlrpc/client.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1108 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/xmlrpc/auth.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      110 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/xmlrpc/system.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8410 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/xmlrpc/worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       48 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/xmlrpc/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1188 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/forms.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/static/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/static/kobo/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/static/kobo/css/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4095 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/css/screen.css
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/static/kobo/img/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      201 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-first.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      191 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-prev.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      204 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-last-disabled.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      201 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-first-disabled.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      204 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-last.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      194 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-prev-disabled.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      191 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-next.png
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      282 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/static/kobo/img/list-next-disabled.png
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/static/kobo/js/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1770 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/static/kobo/js/log_watcher.js
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1100 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/admin.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/task/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      652 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/templates/task/log.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2810 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/task/detail.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      483 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/task/list.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      888 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/task/list_include.html
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/arch/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      425 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/arch/detail.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      223 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/arch/list.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      310 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/arch/list_include.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1122 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/pagination.html
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/worker/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1278 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/worker/detail.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      227 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/worker/list.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      891 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/worker/list_include.html
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/user/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      928 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/user/detail.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      223 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/user/list.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      772 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/user/list_include.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      285 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/500.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      330 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/base.html.example
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      199 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/404.html
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/channel/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      440 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/channel/detail.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      229 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/channel/list.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      328 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/channel/list_include.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1586 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/layout.html
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/templates/auth/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      726 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/templates/auth/login.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8803 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/views.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/urls/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      310 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/auth.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      607 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/user.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      770 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/channel.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      997 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/task.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      583 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/arch.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      739 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/urls/__init__.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/migrations/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1367 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/migrations/0002_auto_20150722_0612.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      658 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/migrations/0003_auto_20160202_0647.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5311 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/migrations/0001_initial.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/migrations/__init__.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/fixtures/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1827 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/fixtures/data.json
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/hub/sql/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       95 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/sql/task.postgresql.sql
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      232 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/menu.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      725 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/decorators.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1055 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/hub/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      997 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/middleware.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    37360 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hub/models.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4381 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/http.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5885 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/plugins.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/client/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      959 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/client/constants.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      777 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/client/default.conf
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/client/commands/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1005 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_cancel_tasks.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1386 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_enable_worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2482 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_watch_log.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1036 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_shutdown_worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      950 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_add_user.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1234 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_resubmit_tasks.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2419 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/client/commands/cmd_create_task.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      975 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_worker_info.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/client/commands/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      647 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_watch_tasks.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1390 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_disable_worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      742 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_list_workers.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2410 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/commands/cmd_list_tasks.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4837 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/task_watcher.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      433 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/client/main.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12914 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/client/__init__.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/xmlrpc/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      166 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/admin.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6236 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/views.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2560 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/xmlrpc/auth.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/xmlrpc/migrations/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      884 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/migrations/0001_initial.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/xmlrpc/migrations/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4143 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/decorators.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3747 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/dispatcher.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/xmlrpc/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      505 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/xmlrpc/models.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2278 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/forms.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/views/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3238 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/views/generic.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/views/__init__.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/upload/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      405 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/upload/admin.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      165 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/upload/urls.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2595 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/upload/views.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1016 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/upload/xmlrpc.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/upload/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2969 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/upload/models.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/menu/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      305 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/menu/context_processors.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    11042 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/menu/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      695 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/menu/middleware.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     6430 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/fields.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/auth/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       40 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/admin.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      159 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/apps.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/django/auth/migrations/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      521 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/django/auth/migrations/0002_LongnameUser.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2847 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/migrations/0001_initial.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/migrations/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1587 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/krb5.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       56 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      512 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/middleware.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2630 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/django/auth/models.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    10815 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/tback.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/worker/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1107 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/worker/default.conf
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3167 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/worker/main.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3711 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/worker/task.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2405 2019-01-13 22:23:01.000000 kobo-0.9.0/kobo/worker/logger.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      184 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/worker/__init__.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/worker/tasks/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      567 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/worker/tasks/task_shutdown_worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/worker/tasks/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    18239 2019-01-13 22:23:11.000000 kobo-0.9.0/kobo/worker/taskmanager.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    11766 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/conf.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    12171 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/cli.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5691 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/log.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8167 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/pkgset.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     4488 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/threads.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13992 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/shortcuts.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    13201 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/rpmlib.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)    25983 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/xmlrpc.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      309 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/exceptions.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     2084 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/decorators.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     8699 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/process.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/__init__.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     3204 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/notification.py
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/hub/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/hub/xmlrpc/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      521 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/xmlrpc/urls.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/xmlrpc/__init__.py.template
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/hub/templates/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      117 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/templates/index.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      604 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/templates/hub/templates/base.html
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      329 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/__project_name__.wsgi
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     5516 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/settings.py.template
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      546 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/manage.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1906 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/templates/hub/urls.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1407 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/menu.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1292 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/__project_name__-httpd.conf
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/__init__.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1031 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/hub/settings_local.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      988 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/task___project_name__.py.template
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/client/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      879 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/client/__project_name__.conf
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/client/commands/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/client/commands/__init__.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/client/__init__.py.template
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1829 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/client/__project_name__
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/worker/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1251 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/worker/__project_name__.conf
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/worker/__init__.py.template
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/worker/tasks/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/worker/tasks/__init__.py.template
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1493 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/worker/__project_name__
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1235 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/client@cmd___project_name__.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1083 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/cli@cmd___project_name__.py.template
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/cli/
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/templates/cli/commands/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/cli/commands/__init__.py.template
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/cli/__init__.py.template
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)     1463 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/templates/cli/__project_name__
+drwxrwxr-x   0 rmcgover (20551) rmcgover (20551)        0 2019-01-13 22:56:04.000000 kobo-0.9.0/kobo/admin/commands/
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      817 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_worker_task.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     1347 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_hub.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      845 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_client.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      826 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_cli_command.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/commands/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      839 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_client_command.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      660 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_worker.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      778 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/commands/cmd_start_cli.py
+-rwxrwxr-x   0 rmcgover (20551) rmcgover (20551)      134 2019-01-04 04:23:14.000000 kobo-0.9.0/kobo/admin/kobo-admin
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     3779 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/admin/__init__.py
+-rw-rw-r--   0 rmcgover (20551) rmcgover (20551)     7224 2019-01-04 04:23:24.000000 kobo-0.9.0/kobo/hardlink.py
```

### Comparing `kobo-0.8.0/LICENSE` & `kobo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/setup.py` & `kobo-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 packages = sorted(packages)
 for package in package_data.keys():
     package_data[package] = sorted(package_data[package])
 
 
 setup(
     name            = "kobo",
-    version         = "0.8.0",
+    version         = "0.9.0",
     description     = "A pile of python modules used by Red Hat release engineering to build their tools",
     url             = "https://github.com/release-engineering/kobo/",
     author          = "Red Hat, Inc.",
     author_email    = "dmach@redhat.com",
     license         = "LGPLv2.1",
 
     packages        = packages,
```

### Comparing `kobo-0.8.0/COPYING` & `kobo-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/README.md` & `kobo-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,24 @@
 
 Please submit pull requests against https://github.com/release-engineering/kobo.
 
 
 Changelog
 =========
 
+kobo 0.9.0
+----------
+
+### BUG FIXES
+
+- Fixed LoggingThread on Python 3 ([#66](https://github.com/release-engineering/kobo/issues/66))
+- Fixed `kobo.django.xmlrpc` migrations for Django 2.x
+- Fixed some exceptions discarded without logging ([#32](https://github.com/release-engineering/kobo/issues/32))
+- Fixed some reliability issues in `kobo.xmlrpc`
+
 kobo 0.8.0
 ----------
 
 ### FEATURES & IMPROVEMENTS
 
 - Improved Python 3 compatibility
 - Improved Django 2.0 compatibility
```

### Comparing `kobo-0.8.0/Makefile` & `kobo-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/AUTHORS` & `kobo-0.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/rpc.py` & `kobo-0.9.0/tests/rpc.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_types.py` & `kobo-0.9.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_main.py` & `kobo-0.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_plugins.py` & `kobo-0.9.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_taskbase.py` & `kobo-0.9.0/tests/test_taskbase.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_tback.py` & `kobo-0.9.0/tests/test_tback.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_middleware.py` & `kobo-0.9.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_decorators.py` & `kobo-0.9.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_view_log.py` & `kobo-0.9.0/tests/test_view_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-import sys
-import os
-import json
 import gc
 import itertools
-import six
+import json
 import locale
+import os
 
 from tempfile import TemporaryFile
 from gzip import GzipFile
 from io import BytesIO
 from shutil import rmtree
+
 import mock
+import six
 
 import django
 import django.conf
 import django.test
-from django.test.utils import get_runner
+
+from django.http import HttpResponse
 
 # Only for Django >= 1.7
 if 'setup' in dir(django):
     # This has to happen before below imports because they have a hard requirement
     # on settings being loaded before import.
     django.setup()
 
-from kobo.hub.models import Task, Arch, Channel, TASK_STATES
-from kobo.hub import views
 from django.contrib.auth.models import User
 
-from .utils import DjangoRunner
+from kobo.hub.models import Task, Arch, Channel, TASK_STATES
+
+from .utils import DjangoRunner, profile
 
 runner = DjangoRunner()
 setup_module = runner.start
 teardown_module = runner.stop
 
-
-# Run test with KOBO_MEMORY_PROFILER=1 to generate memory usage reports from
-# tests annotated with @profile.
-#
-# The point of the memory profiler with this test is to prove that requesting
-# a log doesn't require loading the entire log into memory.  When using the
-# profiler, you'll want to verify that the peak memory usage shows no significant
-# increase in the tests dealing with big logs.
-if os.environ.get('KOBO_MEMORY_PROFILER', '0') == '1':
-    from memory_profiler import profile
-else:
-    # If memory_profiler is disabled, this is a no-op decorator
-    def profile(fn):
-        return fn
-
-
 TASK_ID = 123
 
 
 def tiny_log_content():
     """Returns very small log content.  Particularly, small enough that
     gzip-compressing will *increase* the content size."""
     return 'hi!'
@@ -253,20 +238,21 @@
             content = str(content, encoding=response.charset)
         self.assertTrue(content.startswith('<!DOCTYPE html'))
         self.assertTrue(big_log_content()[-2000:] in content)
 
     @profile
     def test_view_zipped_big_html_context(self):
         """Verify the context passed into HTML template contains correct values."""
-        with mock.patch('kobo.hub.views.render_to_response') as render_to_response:
-            response = render_to_response.return_value.render.return_value
-            response.status_code = 200
+        def render(*args, **kwargs):
+            return HttpResponse(status=200)
+
+        with mock.patch('kobo.hub.views.render_to_response', side_effect=render) as render_mock:
             self.get_log('zipped_big.log')
 
-        mock_call = render_to_response.mock_calls[0]
+        mock_call = render_mock.mock_calls[0]
 
         # make sure we're looking at the right call
         self.assertEqual(mock_call[0], '')
 
         call_args = mock_call[1]
         (template_name, context) = call_args
```

### Comparing `kobo-0.8.0/tests/test_utf8_chunk.py` & `kobo-0.9.0/tests/test_utf8_chunk.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_fields.py` & `kobo-0.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_tail.py` & `kobo-0.9.0/tests/test_tail.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_http.py` & `kobo-0.9.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_conf.py` & `kobo-0.9.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_xmlrpc_client.py` & `kobo-0.9.0/tests/test_xmlrpc_client.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_shortcuts.py` & `kobo-0.9.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_logger.py` & `kobo-0.9.0/tests/test_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import time
 
-import six
 import unittest2 as unittest
-import pytest
+
+from six import BytesIO
 
 from mock import Mock
-from six.moves import StringIO
 
 from kobo.worker.logger import LoggingThread, LoggingIO
 from .utils import ArgumentIsInstanceOf
 
 
 class TestLoggingThread(unittest.TestCase):
 
-    @pytest.mark.xfail(six.PY3, reason='Check issue #66 for more info (https://git.io/fxSc6).')
     def test_upload_task_log_on_stop(self):
         mock_hub = Mock()
         thread = LoggingThread(mock_hub, 9999)
         thread.daemon = True
 
         thread.start()
         self.assertTrue(thread.is_alive())
@@ -27,17 +25,16 @@
 
         thread.write('This is a log message!')
         mock_hub.upload_task_log.assert_not_called()
 
         thread.stop()
         self.assertFalse(thread.is_alive())
         self.assertFalse(thread._running)
-        mock_hub.upload_task_log.assert_called_once_with(ArgumentIsInstanceOf(StringIO), 9999, 'stdout.log', append=True)
+        mock_hub.upload_task_log.assert_called_once_with(ArgumentIsInstanceOf(BytesIO), 9999, 'stdout.log', append=True)
 
-    @pytest.mark.xfail(six.PY3, reason='Check issue #66 for more info (https://git.io/fxSc6).')
     def test_upload_task_log_after_some_time(self):
         mock_hub = Mock()
         thread = LoggingThread(mock_hub, 9999)
         thread.daemon = True
 
         thread.start()
 
@@ -46,15 +43,15 @@
 
         for i in range(5):
             thread.write('%d - This is a very long message to be written in the log\n' % (i + 1))
             mock_hub.upload_task_log.assert_not_called()
 
         # let the thread running for a while
         time.sleep(.1)
-        mock_hub.upload_task_log.assert_called_once_with(ArgumentIsInstanceOf(StringIO), 9999, 'stdout.log', append=True)
+        mock_hub.upload_task_log.assert_called_once_with(ArgumentIsInstanceOf(BytesIO), 9999, 'stdout.log', append=True)
 
         thread.stop()
         self.assertFalse(thread.is_alive())
         self.assertFalse(thread._running)
 
 
 class TestLoggingIO(unittest.TestCase):
```

### Comparing `kobo-0.8.0/tests/test_hardlink.py` & `kobo-0.9.0/tests/test_hardlink.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_pkgset.py` & `kobo-0.9.0/tests/test_pkgset.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_xmlrpc_worker.py` & `kobo-0.9.0/tests/test_xmlrpc_worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_rpmlib.py` & `kobo-0.9.0/tests/test_rpmlib.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_task_logs.py` & `kobo-0.9.0/tests/test_task_logs.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/fields_test/tests.py` & `kobo-0.9.0/tests/fields_test/tests.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/settings.py` & `kobo-0.9.0/tests/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 
 # The middleware and apps below are the bare minimum required
 # to let kobo.hub load successfully
 
 MIDDLEWARE_CLASSES = (
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
+    'kobo.django.auth.middleware.LimitedRemoteUserMiddleware',
     'kobo.hub.middleware.WorkerMiddleware',
 )
 
 INSTALLED_APPS = (
     'django.contrib.contenttypes',
+    'django.contrib.admin',
     'django.contrib.auth',
+    'django.contrib.sessions',
     'kobo.hub',
 )
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': 'testdatabase',
```

### Comparing `kobo-0.8.0/tests/test_taskmanager.py` & `kobo-0.9.0/tests/test_taskmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import errno
 import os
 import signal
+import logging
 
 import django
 import pytest
 import six
 
 # Only for Django >= 1.7
 if 'setup' in dir(django):
@@ -746,14 +747,42 @@
                 os_mock.setpgrp.assert_called_once()
                 os_mock._exit.assert_called_once()
                 signal_mock.signal.assert_called()
 
         t = Task.objects.get(id=t.id)
         self.assertEqual(t.state, TASK_STATES['CLOSED'])
 
+    def test_fork_task_logs_exceptions(self):
+        """Exceptions from the child within fork_task are logged."""
+
+        t = Task.objects.create(
+            worker=self._worker.worker,
+            arch=self._arch,
+            channel=self._channel,
+            owner=self._user,
+            method='DummyForegroundTask',
+            state=TASK_STATES['OPEN'],
+        )
+
+        logger = Mock()
+
+        with patch('kobo.worker.taskmanager.HubProxy') as hub_mock:
+            # Arrange for close_task call to fail (at end of task)
+            hub_mock.return_value.worker.close_task.side_effect = RuntimeError("simulated error")
+
+            tm = TaskManager(conf={'worker': self._worker}, logger=logger)
+            task_info = t.export(False)
+
+            with patch('kobo.worker.taskmanager.os', fork=Mock(return_value=0)) as os_mock:
+                os_mock.devnull = os.devnull
+                tm.fork_task(task_info)
+
+        # It should have logged something about the failure to close the task.
+        logger.log.assert_called_with(logging.CRITICAL, 'Error running forked task', exc_info=1)
+
     @patch('kobo.worker.taskmanager.HubProxy', HubProxyMock)
     def test_run_task_runs_foreground_task(self):
         t = Task.objects.create(
             worker=self._worker.worker,
             arch=self._arch,
             channel=self._channel,
             owner=self._user,
```

### Comparing `kobo-0.8.0/tests/data/dummy-basesystem-10.0-6.noarch.rpm` & `kobo-0.9.0/tests/data/dummy-basesystem-10.0-6.noarch.rpm`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/data/dummy-AdobeReader_enu-9.5.1-1.nosrc.rpm` & `kobo-0.9.0/tests/data/dummy-AdobeReader_enu-9.5.1-1.nosrc.rpm`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/data/dummy-basesystem-10.0-6.src.rpm` & `kobo-0.9.0/tests/data/dummy-basesystem-10.0-6.src.rpm`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/tests/test_log.py` & `kobo-0.9.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/types.py` & `kobo-0.9.0/kobo/types.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/xmlrpc/client.py` & `kobo-0.9.0/kobo/hub/xmlrpc/client.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/xmlrpc/auth.py` & `kobo-0.9.0/kobo/hub/xmlrpc/auth.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/xmlrpc/worker.py` & `kobo-0.9.0/kobo/hub/xmlrpc/worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/forms.py` & `kobo-0.9.0/kobo/hub/forms.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/static/kobo/css/screen.css` & `kobo-0.9.0/kobo/hub/static/kobo/css/screen.css`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/static/kobo/js/log_watcher.js` & `kobo-0.9.0/kobo/hub/static/kobo/js/log_watcher.js`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/admin.py` & `kobo-0.9.0/kobo/hub/admin.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/task/log.html` & `kobo-0.9.0/kobo/hub/templates/task/log.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/task/detail.html` & `kobo-0.9.0/kobo/hub/templates/task/detail.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/task/list_include.html` & `kobo-0.9.0/kobo/hub/templates/task/list_include.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/pagination.html` & `kobo-0.9.0/kobo/hub/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/worker/detail.html` & `kobo-0.9.0/kobo/hub/templates/worker/detail.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/worker/list_include.html` & `kobo-0.9.0/kobo/hub/templates/worker/list_include.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/user/detail.html` & `kobo-0.9.0/kobo/hub/templates/user/detail.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/user/list_include.html` & `kobo-0.9.0/kobo/hub/templates/user/list_include.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/layout.html` & `kobo-0.9.0/kobo/hub/templates/layout.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/templates/auth/login.html` & `kobo-0.9.0/kobo/hub/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/views.py` & `kobo-0.9.0/kobo/hub/views.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/urls/user.py` & `kobo-0.9.0/kobo/hub/urls/user.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/urls/channel.py` & `kobo-0.9.0/kobo/hub/urls/channel.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/urls/task.py` & `kobo-0.9.0/kobo/hub/urls/task.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/urls/arch.py` & `kobo-0.9.0/kobo/hub/urls/arch.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/urls/worker.py` & `kobo-0.9.0/kobo/hub/urls/worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/migrations/0002_auto_20150722_0612.py` & `kobo-0.9.0/kobo/hub/migrations/0002_auto_20150722_0612.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/migrations/0003_auto_20160202_0647.py` & `kobo-0.9.0/kobo/hub/migrations/0003_auto_20160202_0647.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/migrations/0001_initial.py` & `kobo-0.9.0/kobo/hub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/fixtures/data.json` & `kobo-0.9.0/kobo/hub/fixtures/data.json`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/decorators.py` & `kobo-0.9.0/kobo/hub/decorators.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/__init__.py` & `kobo-0.9.0/kobo/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/middleware.py` & `kobo-0.9.0/kobo/hub/middleware.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hub/models.py` & `kobo-0.9.0/kobo/hub/models.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/http.py` & `kobo-0.9.0/kobo/http.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/plugins.py` & `kobo-0.9.0/kobo/plugins.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/constants.py` & `kobo-0.9.0/kobo/client/constants.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/default.conf` & `kobo-0.9.0/kobo/client/default.conf`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_cancel_tasks.py` & `kobo-0.9.0/kobo/client/commands/cmd_cancel_tasks.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_enable_worker.py` & `kobo-0.9.0/kobo/client/commands/cmd_enable_worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_watch_log.py` & `kobo-0.9.0/kobo/client/commands/cmd_watch_log.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_shutdown_worker.py` & `kobo-0.9.0/kobo/client/commands/cmd_shutdown_worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_add_user.py` & `kobo-0.9.0/kobo/client/commands/cmd_add_user.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_resubmit_tasks.py` & `kobo-0.9.0/kobo/client/commands/cmd_resubmit_tasks.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_create_task.py` & `kobo-0.9.0/kobo/client/commands/cmd_create_task.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_worker_info.py` & `kobo-0.9.0/kobo/client/commands/cmd_worker_info.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_watch_tasks.py` & `kobo-0.9.0/kobo/client/commands/cmd_watch_tasks.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_disable_worker.py` & `kobo-0.9.0/kobo/client/commands/cmd_disable_worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_list_workers.py` & `kobo-0.9.0/kobo/client/commands/cmd_list_workers.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/commands/cmd_list_tasks.py` & `kobo-0.9.0/kobo/client/commands/cmd_list_tasks.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/task_watcher.py` & `kobo-0.9.0/kobo/client/task_watcher.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/client/__init__.py` & `kobo-0.9.0/kobo/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/xmlrpc/views.py` & `kobo-0.9.0/kobo/django/xmlrpc/views.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/xmlrpc/auth.py` & `kobo-0.9.0/kobo/django/xmlrpc/auth.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/xmlrpc/migrations/0001_initial.py` & `kobo-0.9.0/kobo/django/xmlrpc/migrations/0001_initial.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,11 +15,12 @@
         migrations.CreateModel(
             name='XmlRpcLog',
             fields=[
                 ('id', models.AutoField(verbose_name='ID', serialize=False, auto_created=True, primary_key=True)),
                 ('dt_inserted', models.DateTimeField(auto_now_add=True)),
                 ('method', models.CharField(max_length=255)),
                 ('args', models.TextField(blank=True)),
-                ('user', models.ForeignKey(blank=True, to=settings.AUTH_USER_MODEL, null=True)),
+                ('user', models.ForeignKey(blank=True, to=settings.AUTH_USER_MODEL, null=True,
+                                           on_delete=models.SET_NULL)),
             ],
         ),
     ]
```

### Comparing `kobo-0.8.0/kobo/django/xmlrpc/decorators.py` & `kobo-0.9.0/kobo/django/xmlrpc/decorators.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/xmlrpc/dispatcher.py` & `kobo-0.9.0/kobo/django/xmlrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/forms.py` & `kobo-0.9.0/kobo/django/forms.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/views/generic.py` & `kobo-0.9.0/kobo/django/views/generic.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/upload/views.py` & `kobo-0.9.0/kobo/django/upload/views.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/upload/xmlrpc.py` & `kobo-0.9.0/kobo/django/upload/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/upload/models.py` & `kobo-0.9.0/kobo/django/upload/models.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/menu/__init__.py` & `kobo-0.9.0/kobo/django/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/menu/middleware.py` & `kobo-0.9.0/kobo/django/menu/middleware.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/fields.py` & `kobo-0.9.0/kobo/django/fields.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/auth/migrations/0002_LongnameUser.py` & `kobo-0.9.0/kobo/django/auth/migrations/0002_LongnameUser.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/auth/migrations/0001_initial.py` & `kobo-0.9.0/kobo/django/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/auth/krb5.py` & `kobo-0.9.0/kobo/django/auth/krb5.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/auth/middleware.py` & `kobo-0.9.0/kobo/django/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/django/auth/models.py` & `kobo-0.9.0/kobo/django/auth/models.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/tback.py` & `kobo-0.9.0/kobo/tback.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/worker/default.conf` & `kobo-0.9.0/kobo/worker/default.conf`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/worker/main.py` & `kobo-0.9.0/kobo/worker/main.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/worker/task.py` & `kobo-0.9.0/kobo/worker/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
-
 from __future__ import print_function
+
 import copy
 import signal
 
+from kobo.client.constants import TASK_STATES
 from kobo.plugins import Plugin
 from kobo.shortcuts import force_list
-from kobo.client.constants import TASK_STATES
 
 
 __all__ = (
     "TaskBase",
     "FailTaskException",
 )
 
@@ -22,15 +22,15 @@
 
 
 class TaskBase(Plugin):
     """Base class for all tasks."""
     enabled = True
 
     def __init__(self, hub, conf, task_id, args):
-        self._hub = hub            # created by taskmanager
+        self._hub = hub  # created by taskmanager
         self._conf = conf
         self._task_id = task_id
         self._task_info = self.hub.worker.get_task(self.task_id)
         self._task_manager = None  # created by taskmanager (only for foreground tasks)
         self._args = args
         self._subtask_list = []
         self.result = ""
@@ -114,15 +114,15 @@
 
         self.hub.worker.wait(self.task_id, subtasks)
 
         finished = []
         while True:
             (finished, unfinished) = self.hub.worker.check_wait(self.task_id)
 
-            if len(unfinished) == 0:
+            if not unfinished:
                 # all done
                 break
 
             # sleep
             signal.pause()
             # wake up on signal to check the status
```

### Comparing `kobo-0.8.0/kobo/worker/logger.py` & `kobo-0.9.0/kobo/worker/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 
-import six
 import threading
 import time
-import six.moves.queue
-from six.moves import StringIO
+
+import six
+
+from six.moves import queue
 from six.moves.xmlrpc_client import Fault
+from six import BytesIO
 
 
 __all__ = (
     "LoggingThread",
     "LoggingIO",
 )
 
@@ -17,15 +19,15 @@
 class LoggingThread(threading.Thread):
     """Send stdout data to hub in a background thread."""
 
     def __init__(self, hub, task_id, *args, **kwargs):
         threading.Thread.__init__(self, *args, **kwargs)
         self._hub = hub
         self._task_id = task_id
-        self._queue = six.moves.queue.Queue()
+        self._queue = queue.Queue()
         self._event = threading.Event()
         self._running = True
         self._send_time = 0
         self._send_data = ""
 
     def run(self):
         """Send queue content to hub."""
@@ -33,29 +35,29 @@
             if self._queue.empty():
                 self._event.wait(5)
 
             self._event.clear()
             while True:
                 try:
                     self._send_data += self._queue.get_nowait()
-                except six.moves.queue.Empty:
+                except queue.Empty:
                     break
 
             if not self._send_data:
                 continue
 
             now = int(time.time())
             if self._running and len(self._send_data) < 1200 and now - self._send_time < 5:
                 continue
 
             if isinstance(self._send_data, six.text_type):
                 self._send_data = self._send_data.encode('utf-8')
 
             try:
-                self._hub.upload_task_log(StringIO(self._send_data), self._task_id, "stdout.log", append=True)
+                self._hub.upload_task_log(BytesIO(self._send_data), self._task_id, "stdout.log", append=True)
                 self._send_time = now
                 self._send_data = ""
             except Fault:
                 continue
 
     def write(self, data):
         """Add data to the queue and set the event for sending queue content."""
```

### Comparing `kobo-0.8.0/kobo/worker/tasks/task_shutdown_worker.py` & `kobo-0.9.0/kobo/worker/tasks/task_shutdown_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-
 from kobo.worker import TaskBase
 from kobo.exceptions import ShutdownException
 
 
 class ShutdownWorker(TaskBase):
     enabled = True
```

### Comparing `kobo-0.8.0/kobo/worker/taskmanager.py` & `kobo-0.9.0/kobo/worker/taskmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,36 +41,39 @@
         "dt_finished": datetime or None,
         "priority": int,
         "weight": int,
     }
 """
 
 from __future__ import absolute_import
+
+import datetime
 import errno
 import os
-import sys
 import signal
+import sys
 import time
-import datetime
-from six.moves.xmlrpc_client import Fault, ProtocolError
+
 from six.moves import StringIO
+from six.moves.xmlrpc_client import Fault, ProtocolError
+
+import six
 
 import kobo.conf
-import kobo.worker.logger
 import kobo.log
 import kobo.tback
+import kobo.worker.logger
+
 from kobo.client import HubProxy
+from kobo.client.constants import TASK_STATES
 from kobo.exceptions import ShutdownException
-
-from kobo.process import kill_process_group, get_process_status
 from kobo.plugins import PluginContainer
+from kobo.process import kill_process_group, get_process_status
 
 from .task import FailTaskException
-from kobo.client.constants import TASK_STATES
-import six
 
 
 __all__ = (
     "TaskContainer",
     "TaskManager",
     "Fault",
     "ProtocolError",
@@ -98,18 +101,18 @@
         # update data from another config
         if conf is not None:
             self.conf.load_from_conf(conf)
 
         # update data from kwargs
         self.conf.load_from_dict(kwargs)
 
-        self.pid_dict = {}      # { task_id: pid }
-        self.task_dict = {}     # { task_id: { task information obtained from self.hub.get_worker_tasks() } }
+        self.pid_dict = {}  # { task_id: pid }
+        self.task_dict = {}  # { task_id: { task information obtained from self.hub.get_worker_tasks() } }
 
-        self.locked = False     # if task manager is locked, it waits until tasks finish and exits
+        self.locked = False # if task manager is locked, it waits until tasks finish and exits
 
         self.task_container = TaskContainer()
 
         # self.hub (xml-rpc hub client) is created here
         self.hub = HubProxy(conf, client_type="worker", logger=self._logger, **kwargs)
         # worker information obtained from hub
         self.worker_info = self.hub.worker.get_worker_info()
@@ -121,30 +124,26 @@
 
     def sleep(self):
         """Sleep between polls."""
         time.sleep(self.conf.get("SLEEP_TIME", 20))
 
     def update_worker_info(self):
         """Update worker_info dictionary."""
-
         self.log_debug("Updating worker info.")
+
         try:
-            self.worker_info = self.hub.worker.update_worker(self.worker_info["enabled"], self.worker_info["ready"], len(self.pid_dict))
+            self.worker_info = self.hub.worker.update_worker(
+                self.worker_info["enabled"],
+                self.worker_info["ready"],
+                len(self.pid_dict)
+            )
         except ProtocolError as ex:
             self.log_error("Cannot update worker info: %s" % ex)
             return
 
-#    def check_version(self):
-#        """Check if worker version matches with hub."""
-#        hub_version = self.worker_info.get("hub_version", None)
-#        if hub_version is not None and not self.locked:
-#            if str(self.version) != str(hub_version):
-#                self.logger.error("Invalid version detected [worker=%s, hub=%s]." % (self.version, hub_version))
-#                self.lock()
-
     def wakeup_task(self, task_info):
         # alert is set in hub.worker.get_worker_tasks() when the task is supposed to wake up
         if task_info.get("alert", False):
             try:
                 os.kill(self.pid_dict[task_info["id"]], signal.SIGUSR2)
             except OSError as ex:
                 self.log_error("Cannot wake up task %s: %s" % (self._task_str(task_info), ex))
@@ -164,23 +163,23 @@
         timeout_list = []
         finished_tasks = set()
 
         for task_info in self.hub.worker.get_worker_tasks():
             self.log_debug("Checking task: %s." % self._task_str(task_info))
 
             if task_info["state"] == TASK_STATES["OPEN"] and task_info["id"] not in self.pid_dict:
-                # an interrupted task appears to be open, but running task manager doesn't track it in it's pid list
-                # this happens after a power outage, for example
+                # an interrupted task appears to be open, but running task manager doesn't track it
+                # in it's pid list this happens after a power outage, for example
                 interrupted_list.append(task_info["id"])
                 finished_tasks.add(task_info["id"])
                 continue
 
             if task_info["timeout"] is not None:
                 time_delta = datetime.datetime.now() - datetime.datetime(*time.strptime(task_info["dt_started"], "%Y-%m-%d %H:%M:%S")[0:6])
-                #time_delta = datetime.datetime.now() - datetime.datetime.strptime(task_info["dt_started"], "%Y-%m-%d %H:%M:%S") #for Python2.5+
+
                 if time_delta.seconds >= (int(task_info["timeout"])):
                     timeout_list.append(task_info["id"])
                     finished_tasks.add(task_info["id"])
                     continue
 
             task_list[task_info["id"]] = task_info
             self.wakeup_task(task_info)
@@ -255,39 +254,40 @@
         for task_id in sorted(finished_tasks):
             task_info = self.hub.worker.get_task(task_id)
             self.finish_task(task_info)
 
         self.update_worker_info()
 
     def get_next_task(self):
-        """ """
+        """Takes new task."""
         if not self.worker_info["enabled"]:
             self.log_info("Worker is disabled.")
             return
 
         if not self.worker_info["ready"]:
             self.log_info("Worker is not ready to take another task.")
             return
 
         if self.locked:
             task_list = self.hub.worker.get_worker_tasks()
-            if len(task_list) == 0:
+
+            if not task_list:
                 raise ShutdownException()
 
             awaited_task_list = self.hub.worker.get_awaited_tasks(task_list)
-            self.log_debug("Current awaited tasks: %r" % [ task_info["id"] for task_info in awaited_task_list ])
+            self.log_debug("Current awaited tasks: %r" % [ti["id"] for ti in awaited_task_list])
 
             # process assigned tasks first
             for task_info in awaited_task_list:
                 self.take_task(task_info)
 
             return
 
         assigned_task_list = self.hub.worker.get_tasks_to_assign()
-        self.log_debug("Current assigned tasks: %r" % [ task_info["id"] for task_info in assigned_task_list ])
+        self.log_debug("Current assigned tasks: %r" % [ti["id"] for ti in assigned_task_list])
 
         # process assigned tasks first
         for task_info in assigned_task_list:
             self.take_task(task_info)
 
     def take_task(self, task_info):
         """Attempt to open the specified task. Return True on success, False otherwise."""
@@ -324,15 +324,14 @@
                 result = True
             except (ShutdownException, KeyboardInterrupt):
                 raise
             except Fault as ex:
                 reason = "[%s] %s" % (ex.faultCode, ex.faultString)
             except Exception as ex:
                 # TODO: log proper error message
-#                self.logger.error("[%s] %s" % (ex.faultCode, ex.faultString))
                 reason = "%s" % ex
 
         if not result:
             self.log_error("Cannot open task %s: %s" % (self._task_str(task_info), reason))
             return
 
         self.worker_info["current_load"] += TaskClass.weight
@@ -364,14 +363,17 @@
             signal.signal(signal.SIGUSR2, lambda *args: None)
 
             # set a default handler for SIGTERM
             signal.signal(signal.SIGTERM, signal.SIG_DFL)
 
             # run the task
             self.run_task(task_info)
+        except Exception:
+            self.log_critical("Error running forked task", exc_info=1)
+            # don't bother raising since we're about to exit
         finally:
             # die
             os._exit(os.EX_OK)
 
     def run_task(self, task_info):
         TaskClass = self.task_container[task_info["method"]]
 
@@ -427,18 +429,20 @@
         if failed:
             hub.worker.fail_task(task.task_id, task.result)
         else:
             hub.worker.close_task(task.task_id, task.result)
 
     def finish_task(self, task_info):
         TaskClass = self.task_container[task_info["method"]]
+
         try:
             TaskClass.cleanup(self.hub, self.conf, task_info)
         except:
             self.log_critical(kobo.tback.get_exception())
+
         try:
             TaskClass.notification(self.hub, self.conf, task_info)
         except:
             self.log_critical(kobo.tback.get_exception())
 
     def is_finished_task(self, task_id):
         """Determine if task has finished.
@@ -461,42 +465,29 @@
             prefix = "Task #%s" % task_id
             self.log_info(get_process_status(status, prefix))
             return True
 
         return False
 
     def cleanup_task(self, task_id):
-        """Cleanup after the task.
-          - kill child processes
-        """
-
-        # clean up stray subtasks
-#        self.logger.debug("cleanup_task: Trying to terminate task with SIGTERM: %s [#%s] (pid: %s)" % (self.task_dict[task_id]["method"], task_id, self.pid_dict[task_id]))
+        """Cleanup after the task. Kill child processes."""
 
         try:
-#            success = kill_process_group(self.pid_dict[task_id])
             success = kill_process_group(self.pid_dict[task_id], logger=self._logger)
         except IOError as ex:
             # proc file doesn"t exist -> process was already killed
             success = True
 
         if not success:
-#            self.logger.debug("cleanup_task: Trying to terminate task with SIGKILL: %s [#%s] (pid: %s)" % (self.task_dict[task_id]["method"], task_id, self.pid_dict[task_id]))
             try:
-#                success = kill_process_group(self.pid_dict[task_id], signal.SIGKILL, timeout=2)
                 success = kill_process_group(self.pid_dict[task_id], signal.SIGKILL, timeout=2, logger=self._logger)
             except IOError:
                 # proc file doesn"t exist -> process was already killed
                 success = True
 
-#        if success:
-#            self.logger.info("cleanup_task: Task terminated: %s [#%s] (pid: %s)" % (self.task_dict[task_id]["method"], task_id, self.pid_dict[task_id]))
-#        else:
-#            self.logger.error("cleanup_task: Task NOT terminated: %s [#%s] (pid: %s)" % (self.task_dict[task_id]["method"], task_id, self.pid_dict[task_id]))
-
         return success
 
     def shutdown(self):
         """Terminate all tasks and exit."""
         for task_id, task_info in six.iteritems(self.task_dict):
             try:
                 TaskClass = self.task_container[task_info["method"]]
```

### Comparing `kobo-0.8.0/kobo/conf.py` & `kobo-0.9.0/kobo/conf.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/cli.py` & `kobo-0.9.0/kobo/cli.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/log.py` & `kobo-0.9.0/kobo/log.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/pkgset.py` & `kobo-0.9.0/kobo/pkgset.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/threads.py` & `kobo-0.9.0/kobo/threads.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/shortcuts.py` & `kobo-0.9.0/kobo/shortcuts.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/rpmlib.py` & `kobo-0.9.0/kobo/rpmlib.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/xmlrpc.py` & `kobo-0.9.0/kobo/xmlrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,17 +531,20 @@
 
         if sys.version_info[:2] < (2, 7):
             host, extra_headers, x509 = self.get_host_info(host)
             conn = TimeoutHTTPS(host, None, **(x509 or {}))
             conn.set_timeout(self.timeout)
             return conn
         else:
+            CONNECTION_LOCK.acquire()
+            self._connection = (None, None) # this disables connection caching which causes a race condition when running in threads
             conn = xmlrpclib.SafeTransport.make_connection(self, host)
             if self.timeout:
                 conn.timeout = self.timeout
+            CONNECTION_LOCK.release()
             return conn
 
     # override the appropriate request method
     if hasattr(xmlrpclib.Transport, "single_request"):
         # python 2.7+
         single_request = CookieTransport._single_request
     else:
@@ -575,21 +578,20 @@
 
             for i in range(self.retry_count + 1):
                 try:
                     result = transport_class.request(self, *args, **kwargs)
                     return result
                 except KeyboardInterrupt:
                     raise
-                except (socket.error, socket.herror, socket.gaierror, socket.timeout) as ex:
+                except (socket.error, socket.herror, socket.gaierror, socket.timeout, httplib.CannotSendRequest) as ex:
                     if i >= self.retry_count:
                         raise
                     retries_left = self.retry_count - i
                     retries = "%d %s left" % (retries_left, retries_left == 1 and "retry" or "retries") # 1 retry left / X retries left
                     print("XML-RPC connection to %s failed: %s, %s" % (args[0], ex.args[1:], retries), file=sys.stderr)
-                    raise
                     time.sleep(self.retry_timeout)
 
     RetryTransportClass.__name__ = transport_class.__name__
     RetryTransportClass.__doc__ = transport_class.__name__
     return RetryTransportClass
```

### Comparing `kobo-0.8.0/kobo/decorators.py` & `kobo-0.9.0/kobo/decorators.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/process.py` & `kobo-0.9.0/kobo/process.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/notification.py` & `kobo-0.9.0/kobo/notification.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/xmlrpc/urls.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/xmlrpc/urls.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/templates/base.html` & `kobo-0.9.0/kobo/admin/templates/hub/templates/base.html`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/settings.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/settings.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/manage.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/manage.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/urls.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/urls.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/menu.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/menu.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/__project_name__-httpd.conf` & `kobo-0.9.0/kobo/admin/templates/hub/__project_name__-httpd.conf`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/hub/settings_local.py.template` & `kobo-0.9.0/kobo/admin/templates/hub/settings_local.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/task___project_name__.py.template` & `kobo-0.9.0/kobo/admin/templates/task___project_name__.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/client/__project_name__.conf` & `kobo-0.9.0/kobo/admin/templates/client/__project_name__.conf`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/client/__project_name__` & `kobo-0.9.0/kobo/admin/templates/client/__project_name__`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/worker/__project_name__.conf` & `kobo-0.9.0/kobo/admin/templates/worker/__project_name__.conf`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/worker/__project_name__` & `kobo-0.9.0/kobo/admin/templates/worker/__project_name__`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/client@cmd___project_name__.py.template` & `kobo-0.9.0/kobo/admin/templates/client@cmd___project_name__.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/cli@cmd___project_name__.py.template` & `kobo-0.9.0/kobo/admin/templates/cli@cmd___project_name__.py.template`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/templates/cli/__project_name__` & `kobo-0.9.0/kobo/admin/templates/cli/__project_name__`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_worker_task.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_worker_task.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_hub.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_hub.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_client.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_client.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_cli_command.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_cli_command.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_client_command.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_client_command.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_worker.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_worker.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/commands/cmd_start_cli.py` & `kobo-0.9.0/kobo/admin/commands/cmd_start_cli.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/admin/__init__.py` & `kobo-0.9.0/kobo/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `kobo-0.8.0/kobo/hardlink.py` & `kobo-0.9.0/kobo/hardlink.py`

 * *Files identical despite different names*

