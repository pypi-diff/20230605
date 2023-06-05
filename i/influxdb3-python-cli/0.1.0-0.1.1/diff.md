# Comparing `tmp/influxdb3-python-cli-0.1.0.tar.gz` & `tmp/influxdb3-python-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.1.0.tar", last modified: Thu Jun  1 11:19:31 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.1.1.tar", last modified: Mon Jun  5 17:39:02 2023, max compression
```

## Comparing `influxdb3-python-cli-0.1.0.tar` & `influxdb3-python-cli-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 11:19:31.000000 influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7638 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:19:31.940516 influxdb3-python-cli-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-01 11:19:17.000000 influxdb3-python-cli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:39:02.000000 influxdb3-python-cli-0.1.1/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:39:02.100865 influxdb3-python-cli-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-05 17:38:52.000000 influxdb3-python-cli-0.1.1/setup.py
```

### Comparing `influxdb3-python-cli-0.1.0/LICENSE` & `influxdb3-python-cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.1.0/PKG-INFO` & `influxdb3-python-cli-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: influxdb3-python-cli
-Version: 0.1.0
-Summary: Community Python client for InfluxDB 3.0 (CLI)
-Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
-Author: InfluxData
-Author-email: contact@influxdata.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python-cli/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python-cli/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python-cli.svg" alt="PyPI version">
@@ -37,74 +18,76 @@
     <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # influxdb3-python-cli
 ## About
-This repository contains an extention to the influxdb 3.0 python client libary. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
+This repository contains a CLI extension to the [influxdb 3.0 python client library](https://github.com/InfluxCommunity/influxdb3-python). While this code is built on officially supported APIs, the library and CLI here are not officially support by InfluxData. 
 
 ## Install
-To install only the client:
+To install the CLI, enter the following command in your terminal:
 
 ```bash
-python3 -m pip install pyinflux3
+python3 -m pip install influxdb3-python-cli
 ```
 
-To install the client and CLI:
 
-```bash
-sudo python3 -m pip install "pyinflux3[cli]"
-```
+### Scope and privileges
 
-***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
+Python provides the following methods for installing packages within a specific scope:
 
-## Add a Config
+- To isolate the CLI (and its dependencies) to your project directory, install the CLI in a _virtual environment_. [See how to create and use a `venv` or `conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-serverless/query-data/execute-queries/flight-sql/python/#create-a-python-virtual-environment).
+- To install the client to a user-specific directory (without administrative rights), pass the `--user` flag in the `pip` command.
+- To install the client in your system-wide path, use `sudo` with admin privileges.
 
-To configure `pyinflux3` and the CLI, do one of the following:
+## Add a config
 
-You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
+To configure the CLI, do _one_ of the following:
 
-```json
-{
-    "my-config": {
-        "database": "your-database",
-        "host": "your-host",
-        "token": "your-token",
-        "org": "your-org-id",
-        "active": true
-    }
-}
-```
+- Use the `influx3 config` command to create or modify config--for example:
 
-
-- Use the `config` command to create or modify a config:
-
-    ```
+    ```bash
     influx3 config \
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
+    
+  The output is the configuration in a `config.json` file.
+
+- In your editor, create or edit the `config.json` file, and then save it to the directory where you're using the `influx3` command--for example:
+
+    ```json
+    {
+        "my-config": {
+            "database": "your-database",
+            "host": "your-host",
+            "token": "your-token",
+            "org": "your-org-id",
+            "active": true
+        }
+    }
+    ```
 
-If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
+If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
-## Run as a Command
+## Run as a command
 
 ```
 influx3 sql "select * from anomalies"
 ```
 
 ```
 influx3 write testmes f=7 
 ```
 
-## Query and Write Interactively
+## Query and write interactively
 
 In your terminal, enter the following command:
 
 ```
 influx3
 ```
 
@@ -148,26 +131,37 @@
 ```
 (>) write 
 home,room=kitchen temp=70.5,hum=80
 ```
 
 To exit a prompt, enter `exit`.
 
-## Write from a File
+## Write from a file
+
+The InfluxDB CLI and client library can write data from a CSV file.
+The CSV file must contain the following:
+
+- A header row with column names
+- A column that contains a timestamp for each row
+
+The following CLI options specify how data is parsed:
 
-Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
 * `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
+The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
+
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 ## Client library
-The underlining client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
+
+The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
-If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. 
+
+When developing a new feature for the CLI or the client library, make sure to test your feature in both for breaking changes.
 
 #
```

#### html2text {}

```diff
@@ -1,55 +1,57 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.0 Summary:
-Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
-InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
-contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
-# influxdb3-python-cli ## About This repository contains an extention to the
-influxdb 3.0 python client libary. While this code is built on officially
-supported APIs, the library and CLI here are not officially support by Influx
-Data. ## Install To install only the client: ```bash python3 -m pip install
-pyinflux3 ``` To install the client and CLI: ```bash sudo python3 -m pip
-install "pyinflux3[cli]" ``` ***Note: Use sudo if you would like to directly
-install the client onto your path. Otherwise use the `--user` flag.** ## Add a
-Config To configure `pyinflux3` and the CLI, do one of the following: You can
-drop a config file called `config.json` in the directory where you are running
-the `influx3` command: ```json { "my-config": { "database": "your-database",
-"host": "your-host", "token": "your-token", "org": "your-org-id", "active":
-true } } ``` - Use the `config` command to create or modify a config: ```
-influx3 config \ --name="my-config" \ --database="" \ --host="us-east-1-
-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` If you are running
-against InfluxDB Cloud Serverless, then use the _bucket name_ as the database
-in your configuration. ## Run as a Command ``` influx3 sql "select * from
-anomalies" ``` ``` influx3 write testmes f=7 ``` ## Query and Write
-Interactively In your terminal, enter the following command: ``` influx3 ```
-`influx3` displays the `(>)` interactive prompt and waits for input. ```
-Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt. ``` (>) sql
-``` At the `(sql >)` prompt, enter your query statement: ``` (sql >) select *
-from home ``` The `influx3` CLI displays query results in Markdown table
-format--for example: ``` | | co | hum | room | temp | time | |----:|-----:|----
---:|:------------|-------:|:------------------------------| | 0 | 0 | 35.9 |
-Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09
-08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>) write ``` At
-the `(write >)` prompt, enter line protocol data. ``` (>) write
-home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
-from a File Both the InfluxDB CLI and Client libary support writing from a CSV
-file. The CSV file must have a header row with the column names. The there must
-be a column containing a timestamp. Here are the parse options: * `--file` -
-The path to the csv file. * `--time` - The name of the column containing the
-timestamp. * `--measurement` - The name of the measurment to store the CSV data
-under. (Currently only supports user specified string) * `--tags` - (optional)
-Specify an array of column names to use as tags. (Currently only supports user
-specified strings) for example: `--tags=host,region` ```bash influx3 write_csv
---file ./Examples/example.csv --measurement table2 --time Date --tags
-host,region ``` ## Client library The underlining client library is also
+# influxdb3-python-cli ## About This repository contains a CLI extension to the
+[influxdb 3.0 python client library](https://github.com/InfluxCommunity/
+influxdb3-python). While this code is built on officially supported APIs, the
+library and CLI here are not officially support by InfluxData. ## Install To
+install the CLI, enter the following command in your terminal: ```bash python3
+-m pip install influxdb3-python-cli ``` ### Scope and privileges Python
+provides the following methods for installing packages within a specific scope:
+- To isolate the CLI (and its dependencies) to your project directory, install
+the CLI in a _virtual environment_. [See how to create and use a `venv` or
+`conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-
+serverless/query-data/execute-queries/flight-sql/python/#create-a-python-
+virtual-environment). - To install the client to a user-specific directory
+(without administrative rights), pass the `--user` flag in the `pip` command. -
+To install the client in your system-wide path, use `sudo` with admin
+privileges. ## Add a config To configure the CLI, do _one_ of the following: -
+Use the `influx3 config` command to create or modify config--for example:
+```bash influx3 config \ --name="my-config" \ --database="" \ --host="us-east-
+1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The output is the
+configuration in a `config.json` file. - In your editor, create or edit the
+`config.json` file, and then save it to the directory where you're using the
+`influx3` command--for example: ```json { "my-config": { "database": "your-
+database", "host": "your-host", "token": "your-token", "org": "your-org-id",
+"active": true } } ``` If you're running the CLI against InfluxDB Cloud
+Serverless, replace `your-database` in the examples with your Cloud Serverless
+_bucket name_. ## Run as a command ``` influx3 sql "select * from anomalies"
+``` ``` influx3 write testmes f=7 ``` ## Query and write interactively In your
+terminal, enter the following command: ``` influx3 ``` `influx3` displays the `
+(>)` interactive prompt and waits for input. ``` Welcome to my IOx CLI. (>) ```
+To query, type `sql` at the prompt. ``` (>) sql ``` At the `(sql >)` prompt,
+enter your query statement: ``` (sql >) select * from home ``` The `influx3`
+CLI displays query results in Markdown table format--for example: ``` | | co |
+hum | room | temp | time | |----:|-----:|------:|:------------|-------:|:------
+------------------------| | 0 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 |
+| 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:50 | ``` To write, type
+`write` at the `(>)` prompt. ``` (>) write ``` At the `(write >)` prompt, enter
+line protocol data. ``` (>) write home,room=kitchen temp=70.5,hum=80 ``` To
+exit a prompt, enter `exit`. ## Write from a file The InfluxDB CLI and client
+library can write data from a CSV file. The CSV file must contain the
+following: - A header row with column names - A column that contains a
+timestamp for each row The following CLI options specify how data is parsed: *
+`--file` - The path to the csv file. * `--time` - The name of the column
+containing the timestamp. * `--measurement` - The name of the measurment to
+store the CSV data under. (Currently only supports user specified string) * `--
+tags` - (optional) Specify an array of column names to use as tags. (Currently
+only supports user specified strings) for example: `--tags=host,region` The
+following example shows how to write CSV data from the [`./Examples/
+example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/
+main/Examples/example.csv) to InfluxDB (as line protocol): ```bash influx3
+write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags
+host,region ``` ## Client library The underlying client library is also
 available for use in your own code: https://github.com/InfluxCommunity/
-influxdb3-python ## Contribution If you are working on a new feature for either
-the CLI or the Client Libary please make sure you test both for breaking
+influxdb3-python ## Contribution When developing a new feature for the CLI or
+the client library, make sure to test your feature in both for breaking
 changes. #
```

### Comparing `influxdb3-python-cli-0.1.0/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -37,74 +37,76 @@
     <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # influxdb3-python-cli
 ## About
-This repository contains an extention to the influxdb 3.0 python client libary. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
+This repository contains a CLI extension to the [influxdb 3.0 python client library](https://github.com/InfluxCommunity/influxdb3-python). While this code is built on officially supported APIs, the library and CLI here are not officially support by InfluxData. 
 
 ## Install
-To install only the client:
+To install the CLI, enter the following command in your terminal:
 
 ```bash
-python3 -m pip install pyinflux3
+python3 -m pip install influxdb3-python-cli
 ```
 
-To install the client and CLI:
 
-```bash
-sudo python3 -m pip install "pyinflux3[cli]"
-```
-
-***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
+### Scope and privileges
 
-## Add a Config
+Python provides the following methods for installing packages within a specific scope:
 
-To configure `pyinflux3` and the CLI, do one of the following:
+- To isolate the CLI (and its dependencies) to your project directory, install the CLI in a _virtual environment_. [See how to create and use a `venv` or `conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-serverless/query-data/execute-queries/flight-sql/python/#create-a-python-virtual-environment).
+- To install the client to a user-specific directory (without administrative rights), pass the `--user` flag in the `pip` command.
+- To install the client in your system-wide path, use `sudo` with admin privileges.
 
-You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
+## Add a config
 
-```json
-{
-    "my-config": {
-        "database": "your-database",
-        "host": "your-host",
-        "token": "your-token",
-        "org": "your-org-id",
-        "active": true
-    }
-}
-```
+To configure the CLI, do _one_ of the following:
 
+- Use the `influx3 config` command to create or modify config--for example:
 
-- Use the `config` command to create or modify a config:
-
-    ```
+    ```bash
     influx3 config \
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
+    
+  The output is the configuration in a `config.json` file.
 
-If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
+- In your editor, create or edit the `config.json` file, and then save it to the directory where you're using the `influx3` command--for example:
 
-## Run as a Command
+    ```json
+    {
+        "my-config": {
+            "database": "your-database",
+            "host": "your-host",
+            "token": "your-token",
+            "org": "your-org-id",
+            "active": true
+        }
+    }
+    ```
+
+If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
+
+## Run as a command
 
 ```
 influx3 sql "select * from anomalies"
 ```
 
 ```
 influx3 write testmes f=7 
 ```
 
-## Query and Write Interactively
+## Query and write interactively
 
 In your terminal, enter the following command:
 
 ```
 influx3
 ```
 
@@ -148,26 +150,37 @@
 ```
 (>) write 
 home,room=kitchen temp=70.5,hum=80
 ```
 
 To exit a prompt, enter `exit`.
 
-## Write from a File
+## Write from a file
+
+The InfluxDB CLI and client library can write data from a CSV file.
+The CSV file must contain the following:
+
+- A header row with column names
+- A column that contains a timestamp for each row
+
+The following CLI options specify how data is parsed:
 
-Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
 * `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
+The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
+
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 ## Client library
-The underlining client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
+
+The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
-If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. 
+
+When developing a new feature for the CLI or the client library, make sure to test your feature in both for breaking changes.
 
 #
```

#### html2text {}

```diff
@@ -1,55 +1,67 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.1.1 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown License-File: LICENSE
                                  [Your Image]
  [PyPI_version] [PyPI_downloads] [Lint_Code_Base] [Lint_Code_Base] [Community
                                     Slack]
-# influxdb3-python-cli ## About This repository contains an extention to the
-influxdb 3.0 python client libary. While this code is built on officially
-supported APIs, the library and CLI here are not officially support by Influx
-Data. ## Install To install only the client: ```bash python3 -m pip install
-pyinflux3 ``` To install the client and CLI: ```bash sudo python3 -m pip
-install "pyinflux3[cli]" ``` ***Note: Use sudo if you would like to directly
-install the client onto your path. Otherwise use the `--user` flag.** ## Add a
-Config To configure `pyinflux3` and the CLI, do one of the following: You can
-drop a config file called `config.json` in the directory where you are running
-the `influx3` command: ```json { "my-config": { "database": "your-database",
-"host": "your-host", "token": "your-token", "org": "your-org-id", "active":
-true } } ``` - Use the `config` command to create or modify a config: ```
-influx3 config \ --name="my-config" \ --database="" \ --host="us-east-1-
-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` If you are running
-against InfluxDB Cloud Serverless, then use the _bucket name_ as the database
-in your configuration. ## Run as a Command ``` influx3 sql "select * from
-anomalies" ``` ``` influx3 write testmes f=7 ``` ## Query and Write
-Interactively In your terminal, enter the following command: ``` influx3 ```
-`influx3` displays the `(>)` interactive prompt and waits for input. ```
-Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt. ``` (>) sql
-``` At the `(sql >)` prompt, enter your query statement: ``` (sql >) select *
-from home ``` The `influx3` CLI displays query results in Markdown table
-format--for example: ``` | | co | hum | room | temp | time | |----:|-----:|----
---:|:------------|-------:|:------------------------------| | 0 | 0 | 35.9 |
-Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09
-08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>) write ``` At
-the `(write >)` prompt, enter line protocol data. ``` (>) write
-home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
-from a File Both the InfluxDB CLI and Client libary support writing from a CSV
-file. The CSV file must have a header row with the column names. The there must
-be a column containing a timestamp. Here are the parse options: * `--file` -
-The path to the csv file. * `--time` - The name of the column containing the
-timestamp. * `--measurement` - The name of the measurment to store the CSV data
-under. (Currently only supports user specified string) * `--tags` - (optional)
-Specify an array of column names to use as tags. (Currently only supports user
-specified strings) for example: `--tags=host,region` ```bash influx3 write_csv
---file ./Examples/example.csv --measurement table2 --time Date --tags
-host,region ``` ## Client library The underlining client library is also
+# influxdb3-python-cli ## About This repository contains a CLI extension to the
+[influxdb 3.0 python client library](https://github.com/InfluxCommunity/
+influxdb3-python). While this code is built on officially supported APIs, the
+library and CLI here are not officially support by InfluxData. ## Install To
+install the CLI, enter the following command in your terminal: ```bash python3
+-m pip install influxdb3-python-cli ``` ### Scope and privileges Python
+provides the following methods for installing packages within a specific scope:
+- To isolate the CLI (and its dependencies) to your project directory, install
+the CLI in a _virtual environment_. [See how to create and use a `venv` or
+`conda` Python virtual environment](https://docs.influxdata.com/influxdb/cloud-
+serverless/query-data/execute-queries/flight-sql/python/#create-a-python-
+virtual-environment). - To install the client to a user-specific directory
+(without administrative rights), pass the `--user` flag in the `pip` command. -
+To install the client in your system-wide path, use `sudo` with admin
+privileges. ## Add a config To configure the CLI, do _one_ of the following: -
+Use the `influx3 config` command to create or modify config--for example:
+```bash influx3 config \ --name="my-config" \ --database="" \ --host="us-east-
+1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The output is the
+configuration in a `config.json` file. - In your editor, create or edit the
+`config.json` file, and then save it to the directory where you're using the
+`influx3` command--for example: ```json { "my-config": { "database": "your-
+database", "host": "your-host", "token": "your-token", "org": "your-org-id",
+"active": true } } ``` If you're running the CLI against InfluxDB Cloud
+Serverless, replace `your-database` in the examples with your Cloud Serverless
+_bucket name_. ## Run as a command ``` influx3 sql "select * from anomalies"
+``` ``` influx3 write testmes f=7 ``` ## Query and write interactively In your
+terminal, enter the following command: ``` influx3 ``` `influx3` displays the `
+(>)` interactive prompt and waits for input. ``` Welcome to my IOx CLI. (>) ```
+To query, type `sql` at the prompt. ``` (>) sql ``` At the `(sql >)` prompt,
+enter your query statement: ``` (sql >) select * from home ``` The `influx3`
+CLI displays query results in Markdown table format--for example: ``` | | co |
+hum | room | temp | time | |----:|-----:|------:|:------------|-------:|:------
+------------------------| | 0 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 |
+| 1 | 0 | 35.9 | Kitchen | 21 | 2023-03-09 08:00:50 | ``` To write, type
+`write` at the `(>)` prompt. ``` (>) write ``` At the `(write >)` prompt, enter
+line protocol data. ``` (>) write home,room=kitchen temp=70.5,hum=80 ``` To
+exit a prompt, enter `exit`. ## Write from a file The InfluxDB CLI and client
+library can write data from a CSV file. The CSV file must contain the
+following: - A header row with column names - A column that contains a
+timestamp for each row The following CLI options specify how data is parsed: *
+`--file` - The path to the csv file. * `--time` - The name of the column
+containing the timestamp. * `--measurement` - The name of the measurment to
+store the CSV data under. (Currently only supports user specified string) * `--
+tags` - (optional) Specify an array of column names to use as tags. (Currently
+only supports user specified strings) for example: `--tags=host,region` The
+following example shows how to write CSV data from the [`./Examples/
+example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/
+main/Examples/example.csv) to InfluxDB (as line protocol): ```bash influx3
+write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags
+host,region ``` ## Client library The underlying client library is also
 available for use in your own code: https://github.com/InfluxCommunity/
-influxdb3-python ## Contribution If you are working on a new feature for either
-the CLI or the Client Libary please make sure you test both for breaking
+influxdb3-python ## Contribution When developing a new feature for the CLI or
+the client library, make sure to test your feature in both for breaking
 changes. #
```

### Comparing `influxdb3-python-cli-0.1.0/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.1.1/influxdb_cli/influx3.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         self._write_prompt_session = PromptSession(lexer=None)
 
     def do_sql(self, arg):
         if self._configurations == {}:
             print("can't query, no active configs")
             return
         try: 
-            reader = self.influxdb_client.query(query=arg, language="sql")
-            table = reader.read_all()
+            table = self.influxdb_client.query(query=arg, language="sql")
             print(table.to_pandas().to_markdown())
         except Exception as e:
             print(e)
 
     def do_write(self, arg):
         if self._configurations == {}:
             print("can't write, no active configs")
```

### Comparing `influxdb3-python-cli-0.1.0/setup.py` & `influxdb3-python-cli-0.1.1/setup.py`

 * *Files identical despite different names*

