# Comparing `tmp/collectd-dbod-1.1.tar.gz` & `tmp/collectd-dbod-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collectd-dbod-1.1.tar", last modified: Wed May 26 06:25:38 2021, max compression
+gzip compressed data, was "dist/collectd-dbod-1.9.tar", last modified: Mon Jun  5 12:15:23 2023, max compression
```

## Comparing `collectd-dbod-1.1.tar` & `collectd-dbod-1.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-26 06:25:38.000000 collectd-dbod-1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-26 06:25:38.000000 collectd-dbod-1.1/test/
--rw-rw-rw-   0 root         (0) root         (0)    15306 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_slave.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_collectd_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    18117 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_collectd_plugin_ping.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_collectd_plugin_entities_malformed.py
--rw-rw-rw-   0 root         (0) root         (0)    14330 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_collectd_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    20289 2021-05-26 06:25:34.000000 collectd-dbod-1.1/test/test_dbod_instances.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2021-05-26 06:25:38.000000 collectd-dbod-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      361 2021-05-26 06:25:38.000000 collectd-dbod-1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13291 2021-05-26 06:25:34.000000 collectd-dbod-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/
--rw-rw-rw-   0 root         (0) root         (0)    10990 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_instances.py
--rw-rw-rw-   0 root         (0) root         (0)     6359 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_ping.py
--rw-rw-rw-   0 root         (0) root         (0)     3907 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_slave.py
--rw-rw-rw-   0 root         (0) root         (0)     2137 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      361 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      572 2021-05-26 06:25:38.000000 collectd-dbod-1.1/src/collectd_dbod.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      738 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_entities_malformed.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2021-05-26 06:25:34.000000 collectd-dbod-1.1/src/dbod_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2021-05-26 06:25:34.000000 collectd-dbod-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:15:23.000000 collectd-dbod-1.9/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-05 12:15:23.000000 collectd-dbod-1.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      948 2023-06-05 12:15:20.000000 collectd-dbod-1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/
+-rw-r--r--   0 root         (0) root         (0)    12288 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_innodb_cluster_ping.py
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_entities_malformed.py
+-rw-r--r--   0 root         (0) root         (0)    15280 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_instances.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_ping.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_slave.py
+-rw-r--r--   0 root         (0) root         (0)     6421 2023-06-05 12:15:20.000000 collectd-dbod-1.9/src/dbod_replication.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:15:23.000000 collectd-dbod-1.9/src/collectd_dbod.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:15:23.000000 collectd-dbod-1.9/test/
+-rw-r--r--   0 root         (0) root         (0)    10899 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_collectd_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_collectd_plugin_entities_malformed.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_collectd_plugin_ping.py
+-rw-r--r--   0 root         (0) root         (0)    15306 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_slave.py
+-rw-r--r--   0 root         (0) root         (0)    21928 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_instances.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-05 12:15:20.000000 collectd-dbod-1.9/test/test_dbod_collectd_plugin.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-05 12:15:23.000000 collectd-dbod-1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    13131 2023-06-05 12:15:20.000000 collectd-dbod-1.9/README.md
```

### Comparing `collectd-dbod-1.1/test/test_dbod_slave.py` & `collectd-dbod-1.9/test/test_dbod_slave.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/test/test_dbod_collectd_plugin.py` & `collectd-dbod-1.9/test/test_dbod_collectd_plugin.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/test/test_dbod_collectd_plugin_ping.py` & `collectd-dbod-1.9/test/test_dbod_collectd_plugin_ping.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/test/test_dbod_collectd_plugin_entities_malformed.py` & `collectd-dbod-1.9/test/test_dbod_collectd_plugin_entities_malformed.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/test/test_dbod_collectd_helpers.py` & `collectd-dbod-1.9/test/test_dbod_collectd_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,63 @@
+#!/usr/bin/python3
+
 from dbod_helpers import DbodCollectdHelper, \
     DbodConfigException
 from mock import MagicMock, call
 from pytest import raises
 import pytest
-import apacheconfig
 import requests
 import json
 import dbod_helpers
 import dbod_instances
-
+import yaml
+import platform
+PYTHON_VERSION = platform.python_version()
+from pkg_resources import parse_version as version
+import cerndb
+from  pathlib import Path
+import builtins
 
 @pytest.fixture
-def helper_mocks(mocker, httpserver):
+def helper_mocks(mocker):
     """
     Mock all external libraries calls
     """
-    mocker.patch('apacheconfig.make_loader')
-    loader_mock = MagicMock()
-    apacheconfig.make_loader.return_value.__enter__.return_value = loader_mock
-    loader_mock.load.return_value = {"api": {
-        "cachefile": "/some/cache/file.json",
-        "host": httpserver.url,
-        "host_metadata_endpoint": "test/host",
-        "entity_endpoint": "v1/instance",
-        "user": "dbod_api",
-        "password": "pass-api"
-        }}
-    mocker.patch('dbod_helpers.gethostname', create=True)
 
+    mocker.patch('pathlib.Path.exists')
+    path_mock = MagicMock()
+    Path.exists = path_mock
+    #Patch https://gitlab.cern.ch/db/python3-cerndb/-/blob/master/cerndb/config/__init__.py#L41
+    path_mock.return_value = True
+    mocker.patch('builtins.open')
+    open_mock = MagicMock()
+    builtins.open = open_mock
+    #Patch https://gitlab.cern.ch/db/python3-cerndb/-/blob/master/cerndb/config/__init__.py#L52
+    open_mock.return_value.__enter__.return_value = ('''
+            api:
+              cachefile: /some/cache/file.json
+              host: https://some-url.cern.ch
+              entity_endpoint: api/v1/instance
+              cluster_member_endpoint: qa/api/v1/cluster-member
+              user: dbod-api
+              password: pass-api
+            mysql:
+              user: uu
+              password: uu
+            dbmon:
+              user: uu
+              password: uu
+            dbod_database:
+              db_name: itcore
+              db_account: DBONDEMAND
+              db_pwd: 12131
+            influx2:
+              client: /path/to/influx/client
+            ''')
+    mocker.patch('dbod_helpers.gethostname', create=True)
     dbod_helpers.gethostname.return_value = "dbod-test1.cern.ch"
     # Mock requests
     mocker.patch("requests.get")
     requests.get.return_value.status_code = 200
     # Mock instance
     mocker.patch('dbod_instances.DbodInstance.__init__')
     mocker.patch('dbod_instances.MySQLDbodInstance.__init__')
@@ -39,318 +65,220 @@
     mocker.patch('dbod_instances.InfluxDbodInstance.__init__')
     mocker.patch('dbod_instances.MalformedDbodInstance.__init__')
     dbod_instances.MySQLDbodInstance.__init__.return_value = None
     dbod_instances.PostgresDbodInstance.__init__.return_value = None
     dbod_instances.InfluxDbodInstance.__init__.return_value = None
     dbod_instances.MalformedDbodInstance.__init__.return_value = None
     dbod_instances.DbodInstance.__init__.return_value = None
-    config = mocker.patch("dbod_helpers.ConfigParser")
-    config.return_value.get.return_value = "uu"
 
-    return {"loader_mock": loader_mock,
-            "httpserver": httpserver,
-            "requests": requests}
+    return {"open_mock": open_mock}
 
 
-def test_dbod_helper_reads_config(mocker, tmpdir, helper_mocks):
+def test_dbod_helper_reads_config(mocker, helper_mocks):
     """
     Test a method to get the "source of truth"
-    May it be JSON from the disk or API call
     """
     # Test configuration was read
     h = DbodCollectdHelper()
-    apacheconfig.make_loader.return_value.__enter__. \
-        return_value.load.assert_called_with("/etc/dbod/core.conf")
-    assert h.config == apacheconfig.make_loader.return_value.__enter__. \
-        return_value.load.return_value
     assert h.cachefile == "/some/cache/file.json"
-    assert h.api_url == helper_mocks["httpserver"].url
-    assert h.api_user == "dbod_api"
-    assert h.api_password == "pass-api"
+    assert h.api_url == 'https://some-url.cern.ch'
+    assert h.api_user == 'dbod-api'
+    assert h.api_password == 'pass-api'
+    assert h.user == 'uu'
+
 
 
-def test_dbod_helper_reads_config_malformed(mocker, tmpdir, helper_mocks):
+def test_dbod_helper_reads_config_malformed(mocker, helper_mocks):
     """
     Test a method to get the "source of truth"
-    May it be JSON from the disk or API call
+    May it be YAML from the disk
     """
     # Test configuration was read
-    helper_mocks["loader_mock"].load.return_value = {"t": {}}
+    helper_mocks["open_mock"].return_value.__enter__.return_value  = ('''a''')
     with raises(DbodConfigException) as exc:
         DbodCollectdHelper()
-    assert str(exc.value) == "Error in DBOD config file " \
-        "(/etc/dbod/core.conf): missing key 'api'"
+    assert str(exc.value) == "Error in DBOD config file (config.yaml):" \
+                             " missing key 'api'"
     ##########################################################
-    helper_mocks["loader_mock"].load.return_value = {"api": {}}
+    helper_mocks["open_mock"].return_value.__enter__.return_value = ('''
+            api:
+            ''')
     with raises(DbodConfigException) as exc:
         DbodCollectdHelper()
-    assert str(exc.value) == "Error in DBOD config file " \
-        "(/etc/dbod/core.conf): missing key 'cachefile'"
+    assert str(exc.value) == "Error in DBOD config file (config.yaml): missing nested key"
 
     ##########################################################
-    helper_mocks["loader_mock"].load.return_value = {"api": {
-        "cachefile": "/some/cache/file.json",
-        "host": "127.0.0.0"
-        }}
-    with raises(DbodConfigException) as exc:
-        DbodCollectdHelper()
-    assert str(exc.value) == "Error in DBOD config file " \
-        "(/etc/dbod/core.conf): missing key 'host_metadata_endpoint'"
-    ##########################################################
-    helper_mocks["loader_mock"].load.return_value = {"api": {
-        "cachefile": "/some/cache/file.json",
-        "host": "127.0.0.0",
-        "host_metadata_endpoint": "/end/point"
-        }}
+
+    helper_mocks["open_mock"].return_value.__enter__.return_value = ('''
+            api:
+              cachefile: /some/cache/file.json
+              host: https://some-url.cern.ch
+            ''')
     with raises(DbodConfigException) as exc:
         DbodCollectdHelper()
-    assert str(exc.value) == "Error in DBOD config file " \
-        "(/etc/dbod/core.conf): missing key 'entity_endpoint'"
+    assert str(exc.value) == "Error in DBOD config file (config.yaml): " \
+                             "missing key 'entity_endpoint'"
     ##########################################################
-    helper_mocks["loader_mock"].load.side_effect = \
-        apacheconfig.error.ConfigFileReadError("sth wrong")
+    helper_mocks["open_mock"].return_value.__enter__.side_effect =  FileNotFoundError("sth wrong")
     with raises(DbodConfigException) as exc:
         DbodCollectdHelper()
     assert str(exc.value) == "sth wrong"
 
 
-def test_get_instances_from_get(mocker, tmpdir, helper_mocks):
-    """
-    Test get_instances calls api to get a list of instances
-        if it fails, it reads entities.json
-        Then it creates a list of DbodInstance object
-        which is returned
-    """
-    # Everything ok - status code 200
-    mocker.patch('dbod_helpers.open')
-    requests.get.return_value.json.return_value = \
-        {"response": [
-            {"instance": "1", "db_type": "MYSQL", "state": "RUNNING"},
-            {"instance": "2", "db_type": "InfluxDB", "state": "RUNNING"},
-            {"instance": "3", "db_type": "MYSQL", "state": "RUNNING"},
-            {"instance": "4", "db_type": "PG", "state": "RUNNING"}
-        ]}
-    h = DbodCollectdHelper()
-    h.user = "user"
-    h.password = "pass"
-    assert h.host_metadata_endpoint == "test/host"
-    instances = h.get_instances()
-    dbod_helpers.gethostname.assert_called()
-    requests.get.assert_called_with("%s/test/host/dbod-test1"
-                                    % h.api_url)
-    requests.get.return_value.json.assert_called()
-    dbod_helpers.open.assert_not_called()
-    # ############ MYSQL INSTANCES #####################
-    assert dbod_instances.MySQLDbodInstance.__init__. \
-        mock_calls \
-        == [call({"instance": "1", "db_type": "MYSQL", "state": "RUNNING"},
-                 user="user", password="pass"),
-            call({"instance": "3", "db_type": "MYSQL", "state": "RUNNING"},
-                 user="user", password="pass")]
-    # ############ POSTGRES INSTANCES #####################
-    assert dbod_instances.PostgresDbodInstance.__init__. \
-        mock_calls \
-        == [call({"instance": "4", "db_type": "PG", "state": "RUNNING"},
-                 user="user", password="pass")]
-    # ############ INFLUXDB INSTANCES #####################
-    assert dbod_instances.InfluxDbodInstance.__init__. \
-        mock_calls \
-        == [call({"instance": "2", "db_type": "InfluxDB", "state": "RUNNING"},
-                 user="user", password="pass")]
-    # ########## SUPER CALLS
-    assert len(instances) == 4
-
-
 @pytest.fixture
 def instances_from_json(helper_mocks, mocker):
     requests.get.return_value.status_code = 404
 
     mocker.patch('dbod_helpers.open')
     mocker.patch('json.load')
     json.load.return_value = [
-            {"instance": "1", "db_type": "PG", "state": "RUNNING"},
-            {"instance": "2", "db_type": "MYSQL", "state": "RUNNING"},
-            {"instance": "3", "db_type": "InfluxDB", "state": "RUNNING"}
+            {"instance": "1", "type": "PG", "state": "RUNNING"},
+            {"instance": "2", "type": "MYSQL", "state": "RUNNING"},
+            {"instance": "3", "type": "InfluxDB", "state": "RUNNING"}
         ]
 
     open_file = MagicMock()
     dbod_helpers.open.return_value.__enter__.return_value = open_file
 
-
 def test_get_instances_from_json(mocker, tmpdir, instances_from_json):
     """
-    API call failed - use entities.json
+    use entities.json
     """
 
     h = DbodCollectdHelper()
     instances = h.get_instances()
     json.load.assert_called_with(
         dbod_helpers.open.return_value.__enter__.return_value)
     dbod_helpers.open.assert_called_with(h.cachefile)
     assert dbod_instances.MySQLDbodInstance.__init__. \
-        mock_calls == [call({"instance": "2", "db_type": "MYSQL", "state": "RUNNING"},
-                            user="uu", password="uu")]
+        mock_calls == [call({"instance": "2", "type": "MYSQL", "state": "RUNNING"},
+                            influx2_client="/path/to/influx/client", user="uu", password="uu")]
     assert dbod_instances.PostgresDbodInstance.__init__. \
-        mock_calls == [call({"instance": "1", "db_type": "PG", "state": "RUNNING"},
-                            user="uu", password="uu")]
+        mock_calls == [call({"instance": "1", "type": "PG", "state": "RUNNING"},
+                            influx2_client="/path/to/influx/client", user="uu", password="uu")]
     assert dbod_instances.InfluxDbodInstance.__init__. \
-        mock_calls == [call({"instance": "3", "db_type": "InfluxDB", "state": "RUNNING"},
-                            user="uu", password="uu")]
+        mock_calls == [call({"instance": "3", "type": "InfluxDB", "state": "RUNNING"},
+                            influx2_client="/path/to/influx/client", user="uu", password="uu")]
     assert len(instances) == 3
 
-
 def test_get_instances_instance_raises_exception(
         mocker, tmpdir, instances_from_json):
     """
     When DbodInstance creation raises exception - we should get
         MalformedDbodInstance
     """
     dbod_instances.MySQLDbodInstance.__init__.side_effect = \
         dbod_helpers.EntityMalformedException("sth wrong")
     h = DbodCollectdHelper()
     instances = h.get_instances()
     assert dbod_instances.MalformedDbodInstance.__init__. \
-        mock_calls == [call({"instance": "2", "db_type": "MYSQL", "state": "RUNNING"},
+        mock_calls == [call({"instance": "2", "type": "MYSQL", "state": "RUNNING"},
                             user="uu", password="uu")]
     assert len(instances) == 3
     assert isinstance(instances[1], dbod_instances.MalformedDbodInstance)
 
-
 def test_get_instances_request_raises_exception_use_json(
         mocker, tmpdir, instances_from_json):
     requests.get.side_effect = requests.ConnectionError("Something wrong")
     h = DbodCollectdHelper()
     instances = h.get_instances()
     json.load.assert_called_with(
         dbod_helpers.open.return_value.__enter__.return_value)
     assert len(instances) == 3
 
 
-def test_get_instances_db_type_missing(mocker, tmpdir, helper_mocks):
+
+def test_get_instances_type_missing(mocker, tmpdir, instances_from_json):
     """
-    Test get_instances calls api to get a list of instances
-        if it fails, it reads entities.json
+    Test get_instances reading entities.json and failing with type missing
         Then it creates a list of DbodInstance object
         which is returned
     """
-    # Everything ok - status code 200
     mocker.patch('dbod_helpers.open')
-    requests.get.return_value.json.return_value = \
-        {"response": [
-            {"instance": "1", "db_type": "MYSQL", "state": "RUNNING"},
-            {"instance": "2", "db_type": "InfluxDB", "state": "RUNNING"},
-            {"instance": "3", "db_type": "MYSQL", "state": "RUNNING"},
+    mocker.patch('json.load')
+    json.load.return_value = [
+            {"instance": "1", "type": "MYSQL", "state": "RUNNING"},
+            {"instance": "2", "type": "InfluxDB", "state": "RUNNING"},
+            {"instance": "3", "type": "MYSQL", "state": "RUNNING"},
             {"instance": "4", "state": "RUNNING"}
-        ]}
+        ]
+
+    open_file = MagicMock()
+    dbod_helpers.open.return_value.__enter__.return_value = open_file
     h = DbodCollectdHelper()
     instances = h.get_instances()
     assert len(instances) == 4
     assert dbod_instances.MalformedDbodInstance.__init__. \
         mock_calls == [call({"instance": "4", "state": "RUNNING"},
                             password='uu', user='uu')]
     assert isinstance(instances[3], dbod_instances.MalformedDbodInstance)
 
 
-def test_init_opens_and_reads_dbod_sensor_config(mocker):
-    """
-    /etc/dbod/sensors/dbod_sensor.ini holds credentials
-    to get to each of the databases, for now we'll use this file.
-    Maybe it could be read from core.conf?
-    """
-    mocker.patch("apacheconfig.make_loader")
-    mock_config_parser = mocker.patch('dbod_helpers.ConfigParser')
-    mock_config_parser.return_value.get.side_effect = ["user", "pass"]
-    helper = DbodCollectdHelper()
-    mock_config_parser.assert_called()
-    mock_config_parser.return_value.read.assert_called_with(
-        "/etc/dbod/sensors/dbod_sensor.ini")
-    mock_config_parser.return_value.get.mock_calls == [
-        call("mysql", "user"), call("mysql", "password")]
-    assert helper.user == "user"
-    assert helper.password == "pass"
-    ######################################################
-    # It should raise DbodConfigException on any problems
-    ######################################################
-    try:
-        from ConfigParser import NoOptionError
-    except ImportError: # Python 3
-        from configparser import NoOptionError
-    mock_config_parser.return_value.get.side_effect = \
-        NoOptionError("pro", "section")
-    with raises(DbodConfigException) as exc:
-        helper = DbodCollectdHelper()
-    assert "Error reading /etc/dbod/sensors/dbod_sensor.ini: "\
-        in str(exc.value)
-
-
 @pytest.mark.parametrize(
-    "state,api_url,endpoint,dbname,status_code,current_state",
+    "state,api_url,endpoint,id,status_code,current_state",
     [("STOPPED", "api.cern.ch:3", "api/test", "db1",
       204, "RUNNING"),
      ("RUNNING", "a.c/232", "api/ent", "db2",
       204, "RUNNING"),
      ("BUSY", "test-api:33", "api/entities", "db3",
       200, "RUNNING"),
-     ("RUNNING", "test-api:33", "api/entities", "db6",
-      200, "JOB_PENDING"),
      ("RUNNING", "test-api:33", "api/entities", "db5",
       200, "AWAITING_APPROVAL"),
      ("BUSY", "test-api:33", "api/entities", "db4",
       200, "MAINTENANCE"),
      ])
-def test_update_state(mocker, state, api_url, endpoint, dbname,
-                       status_code, current_state):
+def test_update_state(mocker, state, api_url, endpoint, id,
+                       status_code, current_state,test_entities_file_name):
     init = mocker.patch('dbod_helpers.DbodCollectdHelper.__init__')
     init.return_value = None
     helper = DbodCollectdHelper()
     helper.api_url = api_url
-    helper.entity_endpoint = endpoint
+    helper.instance_endpoint = endpoint
     helper.api_user = "user"
     helper.api_password = "pass"
+    helper.cachefile = test_entities_file_name
 
     import requests
     import collectd
     mocker.resetall()
     requests.put.reset_mock()
 
     class Instance:
         pass
     instance = Instance()
-    instance.db_name = dbname
+    instance.id = id
+    instance.db_name = id
     instance.state = current_state
-    expected_url = "%s/%s/%s" % (api_url, endpoint, dbname)
+    expected_url = "%s/%s/%s" % (api_url, endpoint, id)
     requests.put.return_value.status_code = status_code
     helper.update_state(instance, state)
 
-    if current_state in ["JOB_PENDING", "AWAITING_APPROVAL", "MAINTENANCE"]:
+    if current_state in ["AWAITING_APPROVAL", "MAINTENANCE"]:
         requests.put.assert_not_called()
         collectd.debug.assert_called_with(
             "Not updating state of %s. Instance state: %s"
-            % (dbname, current_state))
+            % (instance.db_name, current_state))
     elif current_state == state:
         requests.put.assert_not_called()
         collectd.debug("Instance %s state [%s] has not changed"
                         % (instance.db_name, instance.state))
     else:
         collectd.debug("Updating %s instance state to: %s"
                         % (instance.db_name, instance.state))
-        if hasattr(instance, 'id'):
-            expected_url = "%s/%s/%s" % (api_url,
+        expected_url = "%s/%s/%s" % (api_url,
                                     endpoint,
                                     instance.id)
-        else:
-            expected_url = "%s/%s/%s" % (api_url,
-                                    endpoint,
-                                    instance.db_name)
 
         data_to_post = {"state": state}
+        headers={'auth': '{ "admin" : true , "groups" : [ ] , "owner" : "collectd" }'}
         requests.put.assert_called_with(
             expected_url,
+            headers=headers,
             auth=(helper.api_user, helper.api_password),
             json=data_to_post,
             verify=False
             )
         if status_code != 204:
             collectd.error.assert_called_with(
-                "Failed updating state of %s. Response code %s, url %s, self.api_url %s, self.entity_endpoint %s, "
-                % (dbname, status_code, expected_url, api_url, endpoint))
+                "Failed updating state of %s. Response code %s, url %s, self.api_url %s, self.instance_endpoint %s, headers %s"
+                % (instance.db_name, status_code, expected_url, api_url, endpoint, headers))
```

### Comparing `collectd-dbod-1.1/test/test_dbod_instances.py` & `collectd-dbod-1.9/test/test_dbod_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,25 @@
     MySQLDbodInstance, PostgresDbodInstance, InfluxDbodInstance, \
     MalformedDbodInstance, StatusCodeException
 from hypothesis import given, strategies as st, settings, HealthCheck
 from pytest import raises
 from mock import MagicMock, call
 import dbod_instances
 import pytest
+import subprocess
+
+
+class FakePopen(object):
+    def __init__(self, args, stdout=None):
+        super().__init__()
+        self.args = args
+        self.stdout = stdout
+
+    def communicate(self):
+        return "OK"
 
 
 @pytest.fixture
 def instance():
     """
     Dummy implementation of DbodInstance
     """
@@ -217,17 +228,16 @@
         "INSERT INTO collectd_ping VALUES ({0});"
     assert PostgresDbodInstance.ping_select_query ==\
         "SELECT * FROM collectd_ping;"
     assert PostgresDbodInstance.ping_create_query is None
     assert PostgresDbodInstance.ping_delete_query ==\
         "DELETE FROM collectd_ping;"
     assert PostgresDbodInstance.slave_lag_query ==\
-        "SELECT extract(epoch from now() - " \
-        "pg_last_xact_replay_timestamp()) AS time_lag;"
-
+        "SELECT CASE WHEN pg_last_wal_receive_lsn() = pg_last_wal_replay_lsn() THEN 0::int ELSE " \
+                "EXTRACT(EPOCH FROM now() - pg_last_xact_replay_timestamp())::int END AS time_lag;"
 
 @pytest.mark.parametrize(
     "user,password,host,port",
     [
         ("user1", "pass1", "host-dbod1.cern.ch", "6060"),
         ("user2", "pass333", "host-dbod2.cern.ch", "60"),
         ("user3", "pass324", "host-dbod3.cern.ch", "16060")
@@ -256,15 +266,15 @@
     ############################################
     p.connect()
 
     psycopg2.connect.assert_called_with(
         database="dod_dbmon",
         user=p.user,
         password=p.password,
-        host=p.instance,
+        host="/var/lib/pgsql/",
         port=p.port)
     assert p.connection == connect_result
     ############################################
     # Execute
     ############################################
     cursor = MagicMock()
     connect_result.cursor.return_value = cursor
@@ -401,14 +411,18 @@
     i = instance(test_instance1)
     with raises(AttributeError):
         i.user
     with raises(AttributeError):
         i.password
 
 
+######################################################
+# InfluxDB
+######################################################
+
 def test_influx_instance_has_plugin_queries():
     """
     InfluxDbodInstance should have:
         - ping_insert_query
         - ping_select_query
         - ping_create_query
     """
@@ -417,21 +431,21 @@
     assert InfluxDbodInstance.ping_select_query ==\
         "q=select * from collectd_ping order by time desc limit 1"
     assert InfluxDbodInstance.ping_create_query is None
     assert InfluxDbodInstance.ping_delete_query is None
 
 
 @pytest.mark.parametrize(
-    "user,password,instance,port,status_code",
+    "user,password,instance,port,status_code,db_version,bindir",
     [
-        ("user1", "pass1", "host-dbod1.cern.ch", "6060", 200),
-        ("user2", "pass333", "host-dbod2.cern.ch", "60", 200),
-        ("user3", "pass324", "host-dbod3.cern.ch", "16060", 203)
+        ("user1", "pass1", "host-dbod1.cern.ch", "6060", 200, "1.8.2", "/usr/local/influxdb/influxdb-2.0.4"),
+        ("user2", "pass333", "host-dbod2.cern.ch", "60", 200, "2.0.4", "/usr/local/influxdb/influxdb-2.0.4"),
+        ("user3", "pass324", "host-dbod3.cern.ch", "16060", 203, "1.7.3", "/usr/local/influxdb/influxdb-2.0.4")
     ])
-def test_influx_instance(mocker, user, password, instance, port, status_code):
+def test_influx_instance(mocker, user, password, instance, port, status_code, db_version, bindir):
     """
     Test Influx instance, it should have
         - connect()
         - insert(table, )
         - select()
         - create()
     It uses HTTP API to manipulat the data!
@@ -445,59 +459,79 @@
     init.return_value = None
 
     p = InfluxDbodInstance()
     mocker.patch.object(p, 'user', user, create=True)
     mocker.patch.object(p, 'password', password, create=True)
     mocker.patch.object(p, 'instance', instance, create=True)
     mocker.patch.object(p, 'port', port, create=True)
+    mocker.patch.object(p, 'db_version', db_version, create=True)
+    mocker.patch.object(p, 'bindir', bindir, create=True)
     ############################
     # Connect, shouldn't do anything
     ############################
     p.connect()
     requests.assert_not_called()
     p.execute("query")
     requests.assert_not_called()
     p.create("query")
     requests.assert_not_called()
 
     ######################################
     # select()
     ######################################
-    if status_code == 200:
-        result = p.select("my query")
-        assert result == 12345
+    if db_version[0] == "1":
+        if status_code == 200:
+            result = p.select("my query")
+            assert result == 12345
+        else:
+            with raises(StatusCodeException) as exc:
+                p.select("my query")
+            assert "Error executing GET statement on %s instance."\
+                " Response code was: %s" % (p.instance, status_code)\
+                in str(exc.value)
+        url = "https://%s:%s/query?db=dod_dbmon" % (instance, port)
+        requests.get.assert_called_with(
+            url, auth=(user, password), params="my query",
+            verify=False, timeout=10)
     else:
-        with raises(StatusCodeException) as exc:
-            p.select("my query")
-        assert "Error executing GET statement on %s instance."\
-            " Response code was: %s" % (p.instance, status_code)\
-            in str(exc.value)
-    url = "https://%s:%s/query?db=dod_dbmon" % (instance, port)
-    requests.get.assert_called_with(
-        url, auth=(user, password), params="my query",
-        verify=False, timeout=10)
+        def fake_communicate(a):
+            return "OK"
+        subprocess.Popen = FakePopen
+        subprocess.Popen.communicate = fake_communicate
+        stdout = "12345"
+        stderr = None
+        if stderr:
+            with raises(StatusCodeException) as exc:
+                p.select("my query")
+            assert "Error pinging instance %s. Response code was: %s"\
+                % (p.instance, "err")
+        else:
+            assert stdout == "12345"
 
     ######################################
     # insert()
     ######################################
     # In case of insert 204 is the proper code
     status_code += 4
     requests.post.return_value.status_code = status_code
-    if status_code == 204:
-        p.insert("my query")
-    else:
-        with raises(StatusCodeException) as exc:
+    if db_version[0] == "1":
+        if status_code == 204:
             p.insert("my query")
-        assert "Error executing POST statement on %s instance."\
-            " Response code was: %s" % (p.instance, status_code)\
-            in str(exc.value)
-    url = "https://%s:%s/write?db=dod_dbmon" % (instance, port)
-    requests.post.assert_called_with(
-        url, auth=(user, password), data="my query",
-        verify=False, timeout=10)
+        else:
+            with raises(StatusCodeException) as exc:
+                p.insert("my query")
+            assert "Error executing POST statement on %s instance."\
+                " Response code was: %s" % (p.instance, status_code)\
+                in str(exc.value)
+        url = "https://%s:%s/write?db=dod_dbmon" % (instance, port)
+        requests.post.assert_called_with(
+            url, auth=(user, password), data="my query",
+            verify=False, timeout=10)
+    else:
+        p.insert("my query value=%s" % status_code)
 
 
 def test_dbod_instance_has_get_replication_lag(mocker):
     """
     The basic implementation of get_replication_lag should just call select
     with slave_query
     """
@@ -563,15 +597,17 @@
             "db_type": st.sampled_from(["PG", "MYSQL", "InfluxDB"]),
             "port": st.integers(1000, 3000),
             "socket": st.sampled_from(["/var/lib/mysql.socket",
                                        "/tmp/some.socket"]),
             "class": st.just("TEST"),
             "attributes": st.just({}),
             "active": st.booleans(),
-            "state": st.sampled_from(["RUNNING", "BUSY", "STOPPED"])
+            "state": st.sampled_from(["RUNNING", "BUSY", "STOPPED"]),
+            "version": st.sampled_from(["1.7.3", "1.8.2", "2.0.4"]),
+            "bindir": st.just("/usr/local/influxdb/influxdb-2.0.4")
             }
         )
     # Simulate missing attributes
     notifications = st.dictionaries(
         keys=st.just("notifications"),
         values=st.sampled_from(["true", "false"])
     )
@@ -598,18 +634,19 @@
     as it comes from DBOD API or entities.json
     """
     mocker.resetall()
     class TestInstance(DbodInstance):
         def connect(self):
             pass
 
-    # Fill missing pieces, that we're not interested in in this test
+    # Fill missing pieces, that we're not interested in this test
     # api_dict will randomly make them empty or not defined
     api_dict["attributes"]["notifications"] = "true"
-
+    api_dict["cluster_type"] = None
+    api_dict["role"] = None
     t = TestInstance(api_dict)
 
     try:
         # If attribute defined in the dict, assert that object attribute is
         # set to proper value
         seconds = api_dict['attributes']['monit_notif_max_lag_seconds']
         assert t.max_lag_seconds == seconds
```

### Comparing `collectd-dbod-1.1/README.md` & `collectd-dbod-1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 `read` method calls `get_instances` method of `DbodCollectdHelper`. This one makes a call to the API to get instances on the current host. If the API call fails, it takes this data from a locally stored copy `entities.json`.
 
 ---
 #### DbodCollectdHelper
 
 A class defined in `dbod_collectd_helpers` module.
 
-In `__init__` we read two config files - `/etc/dbod/core.conf` and `/etc/dbod/sensors/dbod_sensor.ini` - probably we could unify to reading just the first one. From the second one we take only the password to `dod_dbmon` account.
+In `__init__` we read two config files - `/etc/dbod/conf/core.conf`. 
 
 `DbodCollectdHelper` has two methods - `get_instances()` and `update_status()`.
 
 **`get_instances`** - queries DBOD API using REST, or if DBOD API is unavailable it uses the content of cached `entities.json`. This method is called on every call to `read` by collectd.
 
 **`update_status`** - this one uses DBOD API to update instance status. If there was a problem with an instance, status can be changed changed to `BUSY` or `STOPPED` etc..
```

### Comparing `collectd-dbod-1.1/src/dbod_instances.py` & `collectd-dbod-1.9/src/dbod_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,338 +1,265 @@
+"""Update instance status, get list of instances on a host
+
+Raises:
+    DbodConfigException: Missing configuration in  /etc/dbod/conf/core.conf
 """
-DBOD instances
-"""
+import json
+from socket import gethostname
 
-from distutils.util import strtobool
-from abc import ABCMeta, abstractmethod
 import requests
-import psycopg2
-import pymysql
-
-try:
-    from itertools import izip as zip  # pylint: disable=redefined-builtin
-except ImportError:  # Python 3.x
-    pass
-
+from dbod_instances import EntityMalformedException, MalformedDbodInstance, \
+    instance_types
+import collectd  # pylint: disable=import-error
 
-# compatible with Python 2 *and* 3:
-ABC = ABCMeta('ABC', (object,), {'__slots__': ()})
+import platform
+PYTHON_VERSION = platform.python_version()
+from pkg_resources import parse_version as version
 
+if version(PYTHON_VERSION) >= version("3.0"):
+    from cerndb.config import Config
+else:
+    try:
+        from ConfigParser import ConfigParser
+    except ImportError:
+        from configparser import ConfigParser
+    import apacheconfig
 
-# Python 2 - 3 compatibility
-try:
-    basestring
-except NameError:
-    basestring = (str, bytes)  # pylint: disable=invalid-name
 
 
-class EntityMalformedException(Exception):
-    """
-    Raised when there is missing information in the metadata
-    returned by the DBOD API
-    """
+class DbodConfigException(Exception):
+    """Raised when the config is missing or malformed."""
 
 
-class DbodInstance(ABC):
-    # pylint: disable=too-many-instance-attributes
-    # All of the attributes are considered necessary
+class DbodCollectdHelper:
+    """Class mostly used in performing operations with DBOD API."""
 
-    """
-    Represents DBOD instance and is created from dictionary
-        returned by a DBOD API call
-    """
-    STOPPED = "STOPPED"
-    RUNNING = "RUNNING"
-    BUSY = "BUSY"
+    # pylint: disable=unsubscriptable-object, too-many-instance-attributes
+    # pylint: disable=import-outside-toplevel
+    def __init__(self):
+        if version(PYTHON_VERSION) >= version("3.0"):
+            """Use cerndb-config"""
 
-    def __init__(self, api_dict, user=None, password=None):
-        """
-        Takes dictionary as it was returned by the DBOD API
-            and fills instance attributes
-        user - since user/password doesn't come from the API information
-            we nedd separate args to set them
-
-        Raises:
-            EntityMalformedException - when one of the necessary attributes is
-                not present in the dictionary.
-        """
-        self.connection = None
-        if user:
-            self.user = user
-        if password:
-            self.password = password
-        try:
-            self.instance = "dbod-%s.cern.ch" \
-                % (api_dict["db_name"].replace("_", "-"))
-            #check if we use the old api:
-            if "db_type" in api_dict:
-                self.db_type = api_dict["db_type"]
-                self.active = api_dict["active"]
-            else: 
-                self.id = api_dict["id"]
-                self.db_type = api_dict["type"]
-                self.active = (api_dict["status"] == "ACTIVE")
-            self.port = api_dict["port"]
-            self.socket = api_dict["socket"]
-            self.category = api_dict["class"]
-            self.notification = api_dict["attributes"]["notifications"]
-            self.state = api_dict["state"]
-            self.db_name = api_dict["db_name"]
-        except KeyError as e:
-            raise EntityMalformedException(
-                "Attribute %s missing from the metadata! (DBOD API)"
-                % e.args[0])
-
-        #####################################
-        # Change attribute types
-        #####################################
-        try:
-            self.port = int(self.port)
-        except ValueError as e:
-            raise EntityMalformedException(
-                "Attribute port has incorrect value! (DBOD API metadata): %s"
-                % (e))
-        if isinstance(self.notification, basestring):
             try:
-                self.notification = bool(strtobool(self.notification))
-            except ValueError as e:
-                raise EntityMalformedException(
-                    "Attribute notifications has incorrect value! "
-                    "(DBOD API metadata): %s" % (e))
-
-        ########################################
-        # If slave was not defined, use False
-        ########################################
-        try:
-            self.slave = api_dict["attributes"]["slave"]
-            if isinstance(self.slave, basestring):
+                self.config = Config( module_name="collectd-dbod")
+            except Exception as e:
+                raise DbodConfigException(e)
+            ##################################################
+            # Get interesting info from the config file /etc/collectd-dbod/config.yaml
+            ##################################################
+            try:
+                self.cachefile = self.config['api']['cachefile']
+                self.api_url = self.config['api']['host']
+                self.instance_endpoint = \
+                    self.config['api']['entity_endpoint']
+                self.api_user = self.config['api']['user']
+                self.api_password = self.config['api']['password']
+                self.user = self.config['dbmon']['user']
+                self.password = self.config['dbmon']['password']
+                self.influx2_client = self.config['influx2']['client']
+                self.cluster_member_endpoint = self.config['api']['cluster_member_endpoint']
+
+            except KeyError as e:
+                raise DbodConfigException(
+                    "Error in DBOD config file (%s): missing key '%s'"
+                    % ('config.yaml', e.args[0]))
+
+            except TypeError as e:
+                raise DbodConfigException(
+                    "Error in DBOD config file (%s): missing nested key"
+                    % ('config.yaml'))
+
+        else:
+            """Regethostnamead DBOD config file."""
+            from apacheconfig import make_loader
+            config_file = "/etc/dbod/conf/core.conf"
+            ##################################################
+            # Load DBOD config file to get api endpoints and
+            # cachefile location
+            ##################################################
+            with make_loader() as loader:
                 try:
-                    self.slave = bool(strtobool(self.slave))
-                except ValueError as e:
-                    raise EntityMalformedException(
-                        "Attribute slave has incorrect value! "
-                        "(DBOD API metadata): %s" % (e))
-        except KeyError:
-            self.slave = False
-
-        #############################################################
-        # If slave monit_notif_max_lag_seconds is not defined, use 0
-        #############################################################
-        try:
-            self.max_lag_seconds = \
-                api_dict["attributes"]["monit_notif_max_lag_seconds"]
-        except KeyError:
-            self.max_lag_seconds = 300
-
-    @abstractmethod
-    def connect(self):
-        """Connect to an instance."""
-
-    def disconnect(self):
-        """
-        Default implementation that works for both
-            Postgres and MySQL library
-        """
-        self.connection.close()
-
-    def execute(self, statement):
-        """
-        Default implementation that works for both
-            Postgres and MySQL library
-        """
-        cursor = self.connection.cursor()
-        cursor.execute(statement)
-        self.connection.commit()
-        cursor.close()
-
-    def select(self, statement):
-        """
-        Default implementation that works for both
-            Postgres and MySQL library
-        For now it can select only one value!
-        """
-        cursor = self.connection.cursor()
-        cursor.execute(statement)
-        results = cursor.fetchall()
-        cursor.close()
-        return results[0][0]
-
-    def insert(self, query):
-        """
-        By default it just executes, maybe for InfluxDB
-        we need to override it, to be seen...
-        """
-        self.execute(query)
-
-    def create(self, query):
-        """
-        Same as 'insert'. To be verified if needed at all
-        """
-        self.execute(query)
-
-    def get_replication_lag(self):
-        """
-        Unfortunately we need a separate function for that.
-        This is because while in Postgres, we can get this info with
-        a select statement, in mysql we have to run 'SHOW SLAVE STATUS'.
-        Show slave status, doesn't allow for easy filtering for the info that
-        we're interested with, so we have to do it in Python.
-
-        Implementation in the base class is the one that will be used in
-        Postgres. Also, future release (8.0) of mysql has a table
-        that can be selected for this info, then we can remove this method
-        and use plain select
-        """
-        return self.select(self.slave_lag_query)  # pylint: disable=no-member
-
-
-class MySQLDbodInstance(DbodInstance):
-    """Represents a MySQL instance."""
-    ping_insert_query = "INSERT INTO collectd_ping VALUES ({0});"
-    ping_select_query = "SELECT * FROM collectd_ping;"
-    ping_create_query = None
-    ping_delete_query = "DELETE FROM collectd_ping;"
-    slave_lag_query = "SHOW SLAVE STATUS"
-
-    def connect(self):
-        self.connection = pymysql.connect(
-            unix_socket=self.socket,
-            user=self.user,
-            passwd=self.password,
-            db="dod_dbmon",
-            port=self.port,
-            connect_timeout=10)
-
-    def create(self, query):
-        pass
-
-    def get_replication_lag(self):
-        """
-        SHOW SLAVE STATUS, then we have to process what we get
-        from this statement to get the interesting bit - Seconds_Behind_Master
-        """
-        cursor = self.connection.cursor()
-        cursor.execute(self.slave_lag_query)
-        results = cursor.fetchone()
-        self.connection.commit()
-        cursor.close()
-        column_names = [desc[0] for desc in cursor.description]
-        results = dict(zip(column_names, results))
-        return results['Seconds_Behind_Master']
-
-
-class PostgresDbodInstance(DbodInstance):
-    """Represents a Postgresql instance. Is a subclass of DbodInstance"""
-    ping_insert_query = "INSERT INTO collectd_ping VALUES ({0});"
-    ping_select_query = "SELECT * FROM collectd_ping;"
-    ping_create_query = None
-    ping_delete_query = "DELETE FROM collectd_ping;"
-    slave_lag_query = "SELECT extract(epoch from now() - " \
-        "pg_last_xact_replay_timestamp()) AS time_lag;"
-
-    def connect(self):
-        """
-        Connect to the database using psycopg2
-        """
-        self.connection = psycopg2.connect(
-            database="dod_dbmon",
-            user=self.user,
-            password=self.password,
-            host=self.instance,
-            port=self.port
-        )
-
-    def create(self, query):
-        pass
-
-
-class StatusCodeException(Exception):
-    """
-    Raised when using InfluxDbodInstance, and result
-    code was different than 200
-    """
-
-
-class InfluxDbodInstance(DbodInstance):
-    """Represents a InfluxDB instance. Is a subclass of DbodInstance"""
-    ping_insert_query = "collectd_ping,measurement=ping value={0}"
-    ping_select_query = "q=select * from collectd_ping order by "\
-        "time desc limit 1"
-    ping_create_query = None
-    ping_delete_query = None
-
-    def connect(self):
-        """
-        Since we access InfluxDB with HTTP API there is no point
-        in doing anything in the connect method
-        """
-
-    def select(self, statement):
-        """
-        HTTP API query
-        """
-        url = "https://%s:%s/query?db=dod_dbmon" % (self.instance, self.port)
-        response = requests.get(
-            url, auth=(self.user, self.password), params=statement,
-            verify=False, timeout=10)  # nosec
-        if response.status_code != 200:
-            raise StatusCodeException(
-                "Error executing GET statement on %s instance. Response "
-                "code was: %s" % (self.instance, response.status_code))
-        return response.json()["results"][0]["series"][0]["values"][0][2]
-
-    def insert(self, query):
-        """
-        Influx uses HTTP API to write, here we POST to the influx write URL
+                    self.config = loader.load(config_file)
+                except apacheconfig.error.ConfigFileReadError as e:
+                    raise DbodConfigException(e)
+            ##################################################
+            # Get interesting info from the config file
+            ##################################################
+            try:
+                self.cachefile = self.config['api']['cachefile']
+                self.api_url = self.config['api']['host']
+                self.instance_endpoint = \
+                    self.config['api']['entity_endpoint']
+                self.api_user = self.config['api']['user']
+                self.api_password = self.config['api']['password']
+                self.user = self.config['dbmon']['user']
+                self.password = self.config['dbmon']['password']
+                self.influx2_client = self.config['influx2']['client']
+                self.cluster_member_endpoint = \
+                    self.config['api']['cluster_member_endpoint']
+
+            except KeyError as e:
+                raise DbodConfigException(
+                    "Error in DBOD config file (%s): missing key '%s'"
+                    % (config_file, e.args[0]))
+
+
+    def get_instances(self):
+        """
+        Get running instances in the node using entities.json
+        Returns:
+            entities data as a dict (from /etc/dbod/conf/cache/entities.json)
+        """
+        ###################################
+        # Get data from the cache: /etc/dbod/conf/cache/entities.json
+        ###################################
+        with open(self.cachefile) as f:
+            data = json.load(f)
+
+        ######################################
+        # Create Instances from the response
+        ######################################
+        instances = []
+
+        for instance_dict in data:
+            # If creating DbodInstance raises exception, we either
+            # pass it further or ignore it - depends on the metric!
+            try:
+                #####################################################
+                # Create instances based on the db_type attribute
+                #####################################################
+                # Dynamically decide which instance
+                # to create based on the db_type
+                if instance_dict['state'] != 'MAINTENANCE':
+                    try:
+                        type = instance_dict['type']
+                        instances.append(
+                            instance_types[type](instance_dict,
+                              user=self.user,
+                              password=self.password,
+                              influx2_client=self.influx2_client
+                        ))
+
+                    except KeyError:
+                        # Missing db_type
+                        instances.append(
+                            MalformedDbodInstance(instance_dict,
+                                                  user=self.user,
+                                                  password=self.password))
+            except EntityMalformedException:
+                # Create MalformedDbodInstance
+                instances.append(MalformedDbodInstance(
+                    instance_dict, user=self.user, password=self.password))
+        return instances
+
+    def write_to_cache(self,db_name, key, value):
+        with open(self.cachefile,'r') as f:
+            data = json.load(f)
+        for instance_dict in data:
+            if instance_dict['name'] == db_name:
+                instance_dict[key] = value
+                break
+        with open(self.cachefile,'w') as f:
+            json.dump(data,f,indent=2,separators=(',', ': '))
+
+    def update_state(self, instance, state):
+        """
+        instance - one of DbodInstance
+        state - DbodInstance.STOPPED or DbodInstance.RUNNING for now
+
+        update instance state in DBOD API
+        """
+
+        if instance.state == state:
+            collectd.debug("Instance %s state [%s] has not changed from [%s]"
+                           % (instance.db_name, instance.state, state))
+        else:
+            collectd.debug("Updating %s instance state to: %s"
+                           % (instance.db_name, state))
+            url = "%s/%s/%s" % (self.api_url,
+                                self.instance_endpoint,
+                                instance.id)
+            # check the actual current value
+            request = requests.get(url)
+            # If status code != 200 there was an issue connecting to the DBOD api
+            if request.status_code != 200:
+                collectd.error("Failed getting current state of %s. Response code %s, url %s, self.api_url %s, self.instance_endpoint %s"
+                               % (instance.db_name, request.status_code, url, self.api_url, self.instance_endpoint))
+                # we then consider that the cache is good
+                current_state = instance.state
+            else:
+               current_state = request.json()["response"][0]['state']
+            # if the new instance state is one of these don't update
+            if current_state in ["AWAITING_APPROVAL","MAINTENANCE", "TO_BE_DELETED"]:
+                collectd.debug("Not updating state of %s. Instance state: %s"
+                           % (instance.db_name, instance.state))
+            elif current_state == state:
+                collectd.debug("Instance %s state [%s] has not changed, but the cache needs to be updated"
+                           % (instance.db_name, current_state))
+                self.write_to_cache(instance.db_name, 'state', state)
+            else:
+                headers = {'auth': '{ "admin" : true , "groups" : [ ] , "owner" : "collectd" }' }
+                response = requests.put(
+                url, headers=headers,
+                auth=(self.api_user, self.api_password),
+                json={"state": state},
+                verify=False)  # nosec
+                if response.status_code != 204:
+                    collectd.error("Failed updating state of %s. Response code %s, url %s, self.api_url %s, self.instance_endpoint %s, headers %s"
+                               % (instance.db_name, response.status_code, url, self.api_url, self.instance_endpoint, headers))
+                #also update the cache (DBOD-2744)
+                self.write_to_cache(instance.db_name,'state', state)
+
+    def update_instance_role(self, instance, role):
+        """
+        instance - one of DbodInstance
+        role - PRIMARY or REPLICA for now
+        update instance role in DBOD API
         """
-        url = "https://%s:%s/write?db=dod_dbmon" % (self.instance, self.port)
-        response = requests.post(
-            url, auth=(self.user, self.password), data=query,
-            verify=False, timeout=10)  # nosec
-        if response.status_code != 204:
-            raise StatusCodeException(
-                "Error executing POST statement on %s instance. Response "
-                "code was: %s" % (self.instance, response.status_code))
-
-    def execute(self, statement):
-        pass
 
-    def create(self, query):
-        pass
+        collectd.debug("Updating %s instance role to: %s"
+                       % (instance, role))
 
-    def disconnect(self):
-        """
-        Also, here we won't do anything
+        try:
+            role_id = 1 if role == 'PRIMARY' else 2
+            request_dict = {"instance_id": instance, "role_id": role_id}
+            body = json.dumps(request_dict)
+            headers = {'Content-Type': 'application/json',
+                       'auth': '{ "admin" : true , "groups" : [ ] , "owner" : "collectd-agent" }'}
+            url = '{base_path}/{cluster_member_endpoint}'.format(base_path=self.api_url,cluster_member_endpoint=self.cluster_member_endpoint)
+            response = requests.put(url, data=body, headers=headers, auth=(self.api_user, self.api_password))
+
+            if response.status_code == 200:
+                collectd.debug(
+                    "Instance  {node}  {role} attribute updated successfully".format(node=instance,
+                                                                                          role=role))
+            else:
+                collectd.error("DBOD api returned code: {code}".format(code=response.status_code))
+        except Exception as e:
+            collectd.error("There was an error while updating {node} role. Error: {err}".format(node=instance, err=e))
+
+
+    def update_instance_attribute(self, instance_name, attribute, value):
+        """
+        :param self:
+        :param instance_name:
+        :param attribute:
+        :return:
         """
+        collectd.debug("Updating {} '{}' attribute".format(instance_name, attribute))
 
-
-class MalformedDbodInstance(DbodInstance):
-    """Represents a malformed instance, i.e. an instance that has some missing
-    information in it's description (in entities.json). For example, such
-    missing information makes connecting impossible."""
-    # pylint: disable=super-init-not-called
-    def __init__(self, api_dict, user=None, password=None):
-        """
-        Don't call parent class constructor, keep the dict, to see
-            what was missing
-        """
-        self.api_dict = api_dict
         try:
-            self.state = api_dict["state"]
-        except KeyError:
-            self.state = "UNKNOWN"
-
-    def connect(self):
-        pass
-
-    def execute(self, statement):
-        pass
-
-    def disconnect(self):
-        pass
-
-
-instance_types = {    # pylint: disable=invalid-name
-    "PG": PostgresDbodInstance,
-    "MYSQL": MySQLDbodInstance,
-    "InfluxDB": InfluxDbodInstance
-}
+            body = value
+            headers = {'Content-Type': 'text/html; charset=utf-8',
+                       'auth': '{ "admin" : true , "groups" : [ ] , "owner" : "collectd-agent" }'}
+            url = '{base_path}/{entity_endpoint}/{node}/attribute/{attr}'.format(base_path=self.api_url, entity_endpoint=self.instance_endpoint,node=instance_name,
+                                                                   attr=attribute)
+            response = requests.put(url, data=body, headers=headers, auth=(self.api_user, self.api_password))
+
+            if response.status_code == 200:
+                collectd.debug(
+                    "Instance  {node}  {attribute} attribute updated successfully".format(node=instance_name,
+                                                                                          attribute=attribute))
+            else:
+                collectd.error("DBOD api returned code: {code}".format(code=response.status_code))
+        except Exception as e:
+            collectd.error("There was an error while updating {node} attribute. Error: {err}".format(node=instance_name, err=e))
```

### Comparing `collectd-dbod-1.1/src/dbod_ping.py` & `collectd-dbod-1.9/src/dbod_ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
                         "INFO", instance.db_name,
                         "-1", "Instance not active."))
                 continue
 
             # Skip slave instances
             if instance.slave:
                 continue
-
+            elif instance.cluster_type == 'InnoDB':
+                continue
             try:
                 collectd.debug("%s, name: %s"
                                % (type(instance).__name__, instance.db_name))
                 # Iterate over all instances
                 ##############################
                 # Connect to the database
                 ##############################
```

### Comparing `collectd-dbod-1.1/src/dbod_slave.py` & `collectd-dbod-1.9/src/dbod_slave.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,77 +10,95 @@
 class DbodSlavePlugin(DbodCollectdPlugin):
     """
     DBOD slave plugin
     """
 
     log_dispatch = "| dbod_slave | {} | {:10} | [{}] | {}"
 
+    def repl_lag_check(self,instance):
+
+        collectd.debug("dbod_slave - checking replica {} replication lag".format(
+                        instance.db_name))
+        try:
+            instance.connect()
+            seconds = instance.get_replication_lag()
+            # Compare the lag with the max_lag_seconds
+            collectd.debug(
+                "dbod_slave - comparing current lag ({}) with max_lag ({})".format(seconds, instance.max_lag_seconds))
+            if type(seconds) is int:
+                if seconds > instance.max_lag_seconds:
+                    collectd.error(
+                        self.log_dispatch.format(
+                            "ERROR", instance.db_name, "1",
+                            "Instance lags {} seconds behind master".format(seconds)))
+                    self.dispatch([1], instance.notification,
+                                  self.log_dispatch.format(
+                                      "ERROR", instance.db_name,
+                                      "-1", "Notifications disabled"),
+                                  plugin_instance=instance.db_name)
+                    self.helper.update_state(instance, DbodInstance.BUSY)
+                else:
+                    self.dispatch([0], instance.notification,
+                                  self.log_dispatch.format(
+                                      "INFO", instance.db_name,
+                                      "-1", "Notifications disabled"),
+                                  plugin_instance=instance.db_name)
+                    self.helper.update_state(instance,
+                                         DbodInstance.RUNNING)
+            else:
+                collectd.error(
+                    self.log_dispatch.format(
+                        "ERROR", instance.db_name, "1",
+                        "Instance lag seconds behind primary is NULL"
+                        ))
+                self.dispatch([1], instance.notification,
+                              self.log_dispatch.format(
+                                  "ERROR", instance.db_name,
+                                  "-1", "Notifications disabled"),
+                              plugin_instance=instance.db_name)
+                self.helper.update_state(instance, DbodInstance.BUSY)
+        except Exception as exc:
+            # Catch all exception and dispatch error
+            collectd.error(
+                self.log_dispatch.format(
+                    "ERROR", instance.db_name, "1",
+                    "Exception: {}" .format(exc)))
+            self.dispatch([1], instance.notification,
+                          self.log_dispatch.format(
+                              "ERROR", instance.db_name,
+                              "-1", "Notifications disabled"),
+                          plugin_instance=instance.db_name)
+            self.helper.update_state(instance, DbodInstance.STOPPED)
+        finally:
+            try:
+                # Close connection to the database
+                instance.disconnect()
+            except Exception as exc:
+                # We catch all exceptions - maybe the plugin
+                # wasn't able to connect to the instance at all?
+                collectd.warning(
+                    self.log_dispatch.format(
+                        "WARNING", instance.db_name, "",
+                        "Not able to disconnect: {}".format(exc)))
+
     def read(self):
         """
         Call super - this will refresh list of instances from the Dbod API
         Then iterate over the list of instances, and check if they are slave
         """
         super(DbodSlavePlugin, self).read()
         for instance in self.instances:
             # MalformedDbodInstance means broken data in DBOD API
             # this is handled by another collectd plugin
+            # Catch all exception and dispatch error
             if isinstance(instance, MalformedDbodInstance):
                 continue
-
+            if instance.cluster_type == 'InnoDB':
+                continue
             if instance.slave:
                 collectd.debug("-------")
+                collectd.debug("dbod_slave - instance {} is a replica".format(instance.db_name))
+                self.repl_lag_check(instance)
 
-                collectd.debug("dbod_slave - instance %s is slave"
-                               % instance.db_name)
-                try:
-                    instance.connect()
-                    seconds = instance.get_replication_lag()
-                    # Compare the lag with the max_lag_seconds
-                    collectd.debug(
-                        "Comparing current lag (%s) with max_lag (%s)"
-                        % (seconds, instance.max_lag_seconds))
-                    if seconds > instance.max_lag_seconds:
-                        collectd.error(
-                            self.log_dispatch.format(
-                                "ERROR", instance.db_name, "1",
-                                "Instance lags %s seconds behind master"
-                                % seconds))
-                        self.dispatch([1], instance.notification,
-                                      self.log_dispatch.format(
-                                          "ERROR", instance.db_name,
-                                          "-1", "Notifications disabled"),
-                                      plugin_instance=instance.db_name)
-                        self.helper.update_state(instance, DbodInstance.BUSY)
-                    else:
-                        self.dispatch([0], instance.notification,
-                                      self.log_dispatch.format(
-                                          "INFO", instance.db_name,
-                                          "-1", "Notifications disabled"),
-                                      plugin_instance=instance.db_name)
-                        self.helper.update_state(instance,
-                                                 DbodInstance.RUNNING)
-                except Exception as exc:
-                    # Catch all exception and dispatch error
-                    collectd.error(
-                        self.log_dispatch.format(
-                            "ERROR", instance.db_name, "1",
-                            "Exception: %s" % exc))
-                    self.dispatch([1], instance.notification,
-                                  self.log_dispatch.format(
-                                      "ERROR", instance.db_name,
-                                      "-1", "Notifications disabled"),
-                                  plugin_instance=instance.db_name)
-                    self.helper.update_state(instance, DbodInstance.STOPPED)
-                finally:
-                    try:
-                        # Close connection to the database
-                        instance.disconnect()
-                    except Exception as exc:
-                        # We catch all exceptions - maybe the plugin
-                        # wasn't able to connect to the instance at all?
-                        collectd.warning(
-                            self.log_dispatch.format(
-                                "WARNING", instance.db_name, "",
-                                "Not able to disconnect: %s" % exc))
 
 
 DbodSlavePlugin()
```

### Comparing `collectd-dbod-1.1/src/dbod_plugin.py` & `collectd-dbod-1.9/src/dbod_plugin.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/src/collectd_dbod.egg-info/SOURCES.txt` & `collectd-dbod-1.9/src/collectd_dbod.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 README.md
 setup.cfg
 setup.py
 src/dbod_entities_malformed.py
 src/dbod_helpers.py
+src/dbod_innodb_cluster_ping.py
 src/dbod_instances.py
 src/dbod_ping.py
 src/dbod_plugin.py
+src/dbod_replication.py
 src/dbod_slave.py
 src/collectd_dbod.egg-info/PKG-INFO
 src/collectd_dbod.egg-info/SOURCES.txt
 src/collectd_dbod.egg-info/dependency_links.txt
 src/collectd_dbod.egg-info/requires.txt
 src/collectd_dbod.egg-info/top_level.txt
 test/test_dbod_collectd_helpers.py
```

### Comparing `collectd-dbod-1.1/src/dbod_entities_malformed.py` & `collectd-dbod-1.9/src/dbod_entities_malformed.py`

 * *Files identical despite different names*

### Comparing `collectd-dbod-1.1/setup.py` & `collectd-dbod-1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 setup.py configuration
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='collectd-dbod',
-    version='1.1',
+    version='1.9',
     description='Collectd plugins for DBoD',
     author='Damian Moskalik',
     author_email='damian.moskalik@cern.ch',
     url='https://gitlab.cern.ch/db/collectd/collectd-dbod',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[
         'dbod_entities_malformed',
         'dbod_helpers',
         'dbod_ping',
         'dbod_plugin',
         'dbod_instances',
-        'dbod_slave'
-        ],
+        'dbod_slave',
+        'dbod_innodb_cluster_ping',
+        'dbod_replication'
+    ],
     install_requires=[
+        "cerndb-base",
         "apacheconfig",
         "requests",
         "psycopg2-binary",
         "psycopg2",
         "six",
-        "pymysql"
+        "pymysql",
+        "setuptools"
     ],
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
     ]
 )
```

