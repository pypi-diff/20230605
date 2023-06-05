# Comparing `tmp/tarentula-4.3.3.tar.gz` & `tmp/tarentula-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarentula-4.3.3.tar", max compression
+gzip compressed data, was "tarentula-4.3.4.tar", max compression
```

## Comparing `tarentula-4.3.3.tar` & `tarentula-4.3.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    34551 2022-08-01 15:50:17.808633 tarentula-4.3.3/LICENSE
--rw-r--r--   0        0        0    14926 2022-12-14 09:57:46.491146 tarentula-4.3.3/README.md
--rw-r--r--   0        0        0      541 2022-12-15 10:44:53.689237 tarentula-4.3.3/pyproject.toml
--rw-r--r--   0        0        0       76 2022-12-14 10:46:14.379027 tarentula-4.3.3/tarentula/__init__.py
--rw-r--r--   0        0        0    11897 2022-12-15 10:40:11.315657 tarentula-4.3.3/tarentula/cli.py
--rw-r--r--   0        0        0     1731 2022-08-01 15:50:17.812633 tarentula-4.3.3/tarentula/config_file_reader.py
--rw-r--r--   0        0        0     2714 2022-08-01 15:50:17.812633 tarentula-4.3.3/tarentula/count.py
--rw-r--r--   0        0        0     8176 2022-09-01 09:12:56.068432 tarentula-4.3.3/tarentula/datashare_client.py
--rw-r--r--   0        0        0     7852 2022-09-01 09:42:34.053840 tarentula-4.3.3/tarentula/download.py
--rw-r--r--   0        0        0     7812 2022-12-14 10:14:07.888588 tarentula-4.3.3/tarentula/export_by_query.py
--rw-r--r--   0        0        0     2375 2022-08-01 15:50:17.812633 tarentula-4.3.3/tarentula/graph_realtime.py
--rw-r--r--   0        0        0      958 2022-12-15 10:40:22.351714 tarentula-4.3.3/tarentula/logger.py
--rw-r--r--   0        0        0     2435 2022-08-01 15:50:17.812633 tarentula-4.3.3/tarentula/tag_cleaning_by_query.py
--rw-r--r--   0        0        0     5087 2022-10-14 16:58:17.052207 tarentula-4.3.3/tarentula/tagging.py
--rw-r--r--   0        0        0     4868 2022-12-15 10:34:49.958238 tarentula-4.3.3/tarentula/tagging_by_query.py
--rw-r--r--   0        0        0    16076 1970-01-01 00:00:00.000000 tarentula-4.3.3/setup.py
--rw-r--r--   0        0        0    15446 1970-01-01 00:00:00.000000 tarentula-4.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-08-01 15:50:17.808633 tarentula-4.3.4/LICENSE
+-rw-r--r--   0        0        0    19487 2023-06-05 12:24:17.517076 tarentula-4.3.4/README.md
+-rw-r--r--   0        0        0      580 2023-06-05 12:33:13.411113 tarentula-4.3.4/pyproject.toml
+-rw-r--r--   0        0        0       76 2022-12-14 10:46:14.379027 tarentula-4.3.4/tarentula/__init__.py
+-rw-r--r--   0        0        0     3717 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/aggregate.py
+-rw-r--r--   0        0        0    16649 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/cli.py
+-rw-r--r--   0        0        0     1040 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/command.py
+-rw-r--r--   0        0        0     1773 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/config_file_reader.py
+-rw-r--r--   0        0        0     1822 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/count.py
+-rw-r--r--   0        0        0    10601 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/datashare_client.py
+-rw-r--r--   0        0        0     7274 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/download.py
+-rw-r--r--   0        0        0     7266 2023-06-05 12:29:27.894104 tarentula-4.3.4/tarentula/export_by_query.py
+-rw-r--r--   0        0        0     2474 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/graph_realtime.py
+-rw-r--r--   0        0        0      964 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/logger.py
+-rw-r--r--   0        0        0     3666 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/metadata_fields.py
+-rw-r--r--   0        0        0     2574 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tag_cleaning_by_query.py
+-rw-r--r--   0        0        0     5234 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tagging.py
+-rw-r--r--   0        0        0     4979 2023-06-05 12:24:17.517076 tarentula-4.3.4/tarentula/tagging_by_query.py
+-rw-r--r--   0        0        0    20739 1970-01-01 00:00:00.000000 tarentula-4.3.4/setup.py
+-rw-r--r--   0        0        0    20007 1970-01-01 00:00:00.000000 tarentula-4.3.4/PKG-INFO
```

### Comparing `tarentula-4.3.3/LICENSE` & `tarentula-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tarentula-4.3.3/README.md` & `tarentula-4.3.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,46 +19,64 @@
   --syslog-port         INTEGER 514         Syslog port
   --syslog-facility     TEXT    local7      Syslog facility
   --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler
   --help                                    Show this message and exit
   --version                                 Show the installed version of Tarentula
 
 Commands:
+  aggregate
   count
   clean-tags-by-query
   download
   export-by-query
+  list-metadata
   tagging
   tagging-by-query
 ```
 
 ---
 <!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->
 
+- [Installation](#installation)
 - [Usage](#usage)
   - [Cookbook 👩‍🍳](#cookbook-)
   - [Count](#count)
   - [Clean Tags by Query](#clean-tags-by-query)
   - [Download](#download)
   - [Export by Query](#export-by-query)
   - [Tagging](#tagging)
     - [CSV formats](#csv-formats)
   - [Tagging by Query](#tagging-by-query)
+  - [Aggregate](#aggregate)
   - [Following your changes](#following-your-changes)
 - [Configuration File](#configuration-file)
 - [Testing](#testing)
 - [Releasing](#releasing)
   - [1. Create a new release](#1-create-a-new-release)
   - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)
   - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)
   - [4. Push your changes on Github](#4-push-your-changes-on-github)
 
 <!-- /TOC -->
 ---
 
+## Installation
+
+You can insatll Datashare Tarentula with your favorite package manager:
+
+```
+pip3 install --user tarentula
+```
+
+Or alternativly with Docker:
+
+```
+docker run icij/datashare-tarentula
+```
+
 ## Usage
 
 Datashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.
 
 ### Cookbook 👩‍🍳
 
 To learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.
@@ -137,14 +155,17 @@
                                   separatesemicolons: key1=val1;key2=val2;...
 
   --path-format TEXT              Downloaded document path template
   --scroll TEXT                   Scroll duration
   --source TEXT                   A comma-separated list of field to include
                                   in the downloaded document from the index
 
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
   --sort-by TEXT                  Field to use to sort results
   --order-by [asc|desc]           Order to use to sort results
   --once / --not-once             Download file only once
   --traceback / --no-traceback    Display a traceback in case of error
   --progressbar / --no-progressbar
                                   Display a progressbar
   --raw-file / --no-raw-file      Download raw file from Datashare
@@ -182,14 +203,17 @@
 
   --sort-by TEXT                  Field to use to sort results
   --order-by [asc|desc]           Order to use to sort results
   --traceback / --no-traceback    Display a traceback in case of error
   --progressbar / --no-progressbar
                                   Display a progressbar
   --type [Document|NamedEntity]   Type of indexed documents to download
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
   --size INTEGER                  Size of the scroll request that powers the
                                   operation.
 
   --query-field / --no-query-field
                                   Add the query to the export CSV
   --help                          Show this message and exit.
 ```
@@ -261,14 +285,88 @@
   --progressbar / --no-progressbar      Display a progressbar
   --wait-for-completion / --no-wait-for-completion
                                         Create a Elasticsearch task to perform the
                                           updateasynchronously
   --help                                Show this message and exit
 ```
 
+
+### List Metadata
+
+You can list the metadata from the mapping, optionally counting the number of occurrences of each field in the index, with the `--count` parameter. Counting the fields is disabled by default.
+
+It includes a `--filter_by` parameter to narrow retrieving metadata properties of specific sets of documents. For instance it can be used to get just emails related properties with: `--filter_by "contentType=message/rfc822"`
+
+```
+$ tarentula list-metadata --help
+Usage: tarentula list-metadata [OPTIONS]
+
+Options:
+  --datashare-project TEXT       Datashare project
+  --elasticsearch-url TEXT       You can additionally pass the Elasticsearch
+                                 URL in order to use scrollingcapabilities of
+                                 Elasticsearch (useful when dealing with a lot
+                                 of results)
+  --type [Document|NamedEntity]  Type of indexed documents to get metadata
+  --filter_by TEXT               Filter documents by pairs concatenated by
+                                 coma of field names and values separated by
+                                 =.Example "contentType=message/rfc822,content
+                                 Type=message/rfc822"
+  --count / --no-count           Count or not the number of docs for each
+                                 property found
+
+  --help                         Show this message and exit.
+
+```
+
+### Aggregate
+
+You can run aggregations on the data, the ElasticSearch aggregations API is partially enabled with this command.
+The possibilities are:
+
+- count: grouping by a given field different values, and count the num of docs.
+- nunique: returns the number of unique values of a given field.
+- date_histogram: returns counting of monthly or yearly grouped values for a given date field.
+- sum: returns the sum of values of number type fields.
+- min: returns the min of values of number type fields.
+- max: returns the max of values of number type fields.
+- avg: returns the average of values of number type fields.
+- stats: returns a bunch of statistics for a given number type fields.
+- string_stats: returns a bunch of string statistics for a given string type fields.
+
+
+
+```
+$ tarentula aggregate --help
+Usage: tarentula aggregate [OPTIONS]
+
+Options:
+  --apikey TEXT                   Datashare authentication apikey
+  --datashare-url TEXT            Datashare URL
+  --datashare-project TEXT        Datashare project
+  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch
+                                  URL in order to use scrollingcapabilities of
+                                  Elasticsearch (useful when dealing with a
+                                  lot of results)
+  --query TEXT                    The query string to filter documents
+  --cookies TEXT                  Key/value pair to add a cookie to each
+                                  request to the API. You can
+                                  separatesemicolons: key1=val1;key2=val2;...
+  --traceback / --no-traceback    Display a traceback in case of error
+  --type [Document|NamedEntity]   Type of indexed documents to download
+  --group_by TEXT                 Field to use to aggregate results
+  --operation_field TEXT          Field to run the operation on
+  --run [count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]
+                                  Operation to run
+  --calendar_interval [year|month]
+                                  Calendar interval for date histogram
+                                  aggregation
+  --help                          Show this message and exit.
+```
+
 ### Following your changes
 
 When running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.
 
 It uses [mathplotlib](https://matplotlib.org/) and python3-tk.
 
 If you see the following message :
@@ -369,14 +467,18 @@
 
 _To be able to do this, you will need to be part of the ICIJ organization on docker_
 
 ```
 make docker-publish
 ```
 
+**Note**: Datashare Tarentula is a multi-platform build. You might need to setup your environment for 
+multi-platform using the `make docker-setup-multiarch` command. Read more 
+[on Docker documentation](https://docs.docker.com/build/building/multi-platform/). 
+
 ### 4. Push your changes on Github
 
 Git push release and tag :
 
 ```
 git push origin master --tags
 ```
```

#### html2text {}

```diff
@@ -2,96 +2,102 @@
 tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula) Cli
 toolbelt for [Datashare](https://datashare.icij.org). ``` / \ \ \ ,, / / '-.`\
 ()/`.-' .--_'( )'_--. / /` /`""`\ `\ \ | | >< | | \ \ / / '.__.' Usage:
 tarentula [OPTIONS] COMMAND [ARGS]... Options: --syslog-address TEXT localhost
 Syslog address --syslog-port INTEGER 514 Syslog port --syslog-facility TEXT
 local7 Syslog facility --stdout-loglevel TEXT ERROR Change the default log
 level for stdout error handler --help Show this message and exit --version Show
-the installed version of Tarentula Commands: count clean-tags-by-query download
-export-by-query tagging tagging-by-query ``` ---  - [Usage](#usage) - [Cookbook
-ð©âð³](#cookbook-) - [Count](#count) - [Clean Tags by Query](#clean-tags-
-by-query) - [Download](#download) - [Export by Query](#export-by-query) -
-[Tagging](#tagging) - [CSV formats](#csv-formats) - [Tagging by Query]
-(#tagging-by-query) - [Following your changes](#following-your-changes) -
-[Configuration File](#configuration-file) - [Testing](#testing) - [Releasing]
-(#releasing) - [1. Create a new release](#1-create-a-new-release) - [2. Upload
-distributions on pypi](#2-upload-distributions-on-pypi) - [3. Build and publish
-the Docker image](#3-build-and-publish-the-docker-image) - [4. Push your
-changes on Github](#4-push-your-changes-on-github)  --- ## Usage Datashare
-Tarentula comes with basic commands to interact with a Datashare instance
-(running locally or on a remote server). Primarily focus on bulk actions, it
-provides you with both a cli interface and a python API. ### Cookbook
-ð©âð³ To learn more about how to use Datashare Tarentula with a list of
-examples, please refer to the_Cookbook. ### Count A command to just count the
-number of files matching a query. ``` Usage: tarentula count [OPTIONS] Options:
---datashare-url TEXT Datashare URL --datashare-project TEXT Datashare project -
--elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in
-order to use scrollingcapabilities of Elasticsearch (useful when dealing with a
-lot of results) --query TEXT The query string to filter documents --cookies
-TEXT Key/value pair to add a cookie to each request to the API. You can
-separatesemicolons: key1=val1;key2=val2;... --apikey TEXT Datashare
-authentication apikey in the downloaded document from the index --traceback / -
--no-traceback Display a traceback in case of error --type
-[Document|NamedEntity] Type of indexed documents to download --help Show this
-message and exit ``` ### Clean Tags by Query A command that uses Elasticsearch
-`update-by-query` feature to batch untag documents directly in the index. ```
-Usage: tarentula clean-tags-by-query [OPTIONS] Options: --datashare-project
-TEXT Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used
-to perform update by query --cookies TEXT Key/value pair to add a cookie to
-each request to the API. You can separatesemicolons: key1=val1;key2=val2;... --
-apikey TEXT Datashare authentication apikey --traceback / --no-traceback
-Display a traceback in case of error --wait-for-completion / --no-wait-for-
-completion Create a Elasticsearch task to perform the updateasynchronously --
-query TEXT Give a JSON query to filter documents that will have their tags
-cleaned. It can be afile with @path/to/file. Default to all. --help Show this
-message and exit ``` ### Download A command to download all files matching a
-query. ``` Usage: tarentula download [OPTIONS] Options: --apikey TEXT Datashare
-authentication apikey --datashare-url TEXT Datashare URL --datashare-project
-TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
-Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
-(useful when dealing with a lot of results) --query TEXT The query string to
-filter documents --destination-directory TEXT Directory documents will be
-downloaded --throttle INTEGER Request throttling (in ms) --cookies TEXT Key/
-value pair to add a cookie to each request to the API. You can
-separatesemicolons: key1=val1;key2=val2;... --path-format TEXT Downloaded
-document path template --scroll TEXT Scroll duration --source TEXT A comma-
-separated list of field to include in the downloaded document from the index --
-sort-by TEXT Field to use to sort results --order-by [asc|desc] Order to use to
-sort results --once / --not-once Download file only once --traceback / --no-
-traceback Display a traceback in case of error --progressbar / --no-progressbar
-Display a progressbar --raw-file / --no-raw-file Download raw file from
-Datashare --type [Document|NamedEntity] Type of indexed documents to download -
--help Show this message and exit. ``` ### Export by Query A command to export
-all files matching a query. ``` Usage: tarentula export-by-query [OPTIONS]
+the installed version of Tarentula Commands: aggregate count clean-tags-by-
+query download export-by-query list-metadata tagging tagging-by-query ``` --
+-  - [Installation](#installation) - [Usage](#usage) - [Cookbook ð©âð³]
+(#cookbook-) - [Count](#count) - [Clean Tags by Query](#clean-tags-by-query) -
+[Download](#download) - [Export by Query](#export-by-query) - [Tagging]
+(#tagging) - [CSV formats](#csv-formats) - [Tagging by Query](#tagging-by-
+query) - [Aggregate](#aggregate) - [Following your changes](#following-your-
+changes) - [Configuration File](#configuration-file) - [Testing](#testing) -
+[Releasing](#releasing) - [1. Create a new release](#1-create-a-new-release) -
+[2. Upload distributions on pypi](#2-upload-distributions-on-pypi) - [3. Build
+and publish the Docker image](#3-build-and-publish-the-docker-image) - [4. Push
+your changes on Github](#4-push-your-changes-on-github)  --- ## Installation
+You can insatll Datashare Tarentula with your favorite package manager: ```
+pip3 install --user tarentula ``` Or alternativly with Docker: ``` docker run
+icij/datashare-tarentula ``` ## Usage Datashare Tarentula comes with basic
+commands to interact with a Datashare instance (running locally or on a remote
+server). Primarily focus on bulk actions, it provides you with both a cli
+interface and a python API. ### Cookbook ð©âð³ To learn more about how to
+use Datashare Tarentula with a list of examples, please refer to the_Cookbook.
+### Count A command to just count the number of files matching a query. ```
+Usage: tarentula count [OPTIONS] Options: --datashare-url TEXT Datashare URL --
+datashare-project TEXT Datashare project --elasticsearch-url TEXT You can
+additionally pass the Elasticsearch URL in order to use scrollingcapabilities
+of Elasticsearch (useful when dealing with a lot of results) --query TEXT The
+query string to filter documents --cookies TEXT Key/value pair to add a cookie
+to each request to the API. You can separatesemicolons: key1=val1;key2=val2;...
+--apikey TEXT Datashare authentication apikey in the downloaded document from
+the index --traceback / --no-traceback Display a traceback in case of error --
+type [Document|NamedEntity] Type of indexed documents to download --help Show
+this message and exit ``` ### Clean Tags by Query A command that uses
+Elasticsearch `update-by-query` feature to batch untag documents directly in
+the index. ``` Usage: tarentula clean-tags-by-query [OPTIONS] Options: --
+datashare-project TEXT Datashare project --elasticsearch-url TEXT Elasticsearch
+URL which is used to perform update by query --cookies TEXT Key/value pair to
+add a cookie to each request to the API. You can separatesemicolons:
+key1=val1;key2=val2;... --apikey TEXT Datashare authentication apikey --
+traceback / --no-traceback Display a traceback in case of error --wait-for-
+completion / --no-wait-for-completion Create a Elasticsearch task to perform
+the updateasynchronously --query TEXT Give a JSON query to filter documents
+that will have their tags cleaned. It can be afile with @path/to/file. Default
+to all. --help Show this message and exit ``` ### Download A command to
+download all files matching a query. ``` Usage: tarentula download [OPTIONS]
 Options: --apikey TEXT Datashare authentication apikey --datashare-url TEXT
 Datashare URL --datashare-project TEXT Datashare project --elasticsearch-url
 TEXT You can additionally pass the Elasticsearch URL in order to use
 scrollingcapabilities of Elasticsearch (useful when dealing with a lot of
-results) --query TEXT The query string to filter documents --output-file TEXT
-Path to the CSV file --throttle INTEGER Request throttling (in ms) --cookies
-TEXT Key/value pair to add a cookie to each request to the API. You can
+results) --query TEXT The query string to filter documents --destination-
+directory TEXT Directory documents will be downloaded --throttle INTEGER
+Request throttling (in ms) --cookies TEXT Key/value pair to add a cookie to
+each request to the API. You can separatesemicolons: key1=val1;key2=val2;... --
+path-format TEXT Downloaded document path template --scroll TEXT Scroll
+duration --source TEXT A comma-separated list of field to include in the
+downloaded document from the index -f, --from INTEGER Passed to the search it
+will bypass the first n documents -l, --limit INTEGER Limit the total results
+to return --sort-by TEXT Field to use to sort results --order-by [asc|desc]
+Order to use to sort results --once / --not-once Download file only once --
+traceback / --no-traceback Display a traceback in case of error --progressbar /
+--no-progressbar Display a progressbar --raw-file / --no-raw-file Download raw
+file from Datashare --type [Document|NamedEntity] Type of indexed documents to
+download --help Show this message and exit. ``` ### Export by Query A command
+to export all files matching a query. ``` Usage: tarentula export-by-query
+[OPTIONS] Options: --apikey TEXT Datashare authentication apikey --datashare-
+url TEXT Datashare URL --datashare-project TEXT Datashare project --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in order
+to use scrollingcapabilities of Elasticsearch (useful when dealing with a lot
+of results) --query TEXT The query string to filter documents --output-file
+TEXT Path to the CSV file --throttle INTEGER Request throttling (in ms) --
+cookies TEXT Key/value pair to add a cookie to each request to the API. You can
 separatesemicolons: key1=val1;key2=val2;... --scroll TEXT Scroll duration --
 source TEXT A comma-separated list of field to include in the export --sort-by
 TEXT Field to use to sort results --order-by [asc|desc] Order to use to sort
 results --traceback / --no-traceback Display a traceback in case of error --
 progressbar / --no-progressbar Display a progressbar --type
-[Document|NamedEntity] Type of indexed documents to download --size INTEGER
-Size of the scroll request that powers the operation. --query-field / --no-
-query-field Add the query to the export CSV --help Show this message and exit.
-``` ### Tagging A command to batch tag documents with a CSV file. ``` Usage:
-tarentula tagging [OPTIONS] CSV_PATH Options: --datashare-url TEXT http://
-localhost:8080 Datashare URL --datashare-project TEXT local-datashare Datashare
-project --throttle INTEGER 0 Request throttling (in ms) --cookies TEXT _Empty
-string_ Key/value pair to add a cookie to each request to the API. You can
-separate semicolons: key1=val1;key2=val2;... --apikey TEXT None Datashare
-authentication apikey --traceback / --no-traceback Display a traceback in case
-of error --progressbar / --no-progressbar Display a progressbar --help Show
-this message and exit ``` #### CSV formats Tagging with a `documentId` and
-`routing`: ```csv tag,documentId,routing
-Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
+[Document|NamedEntity] Type of indexed documents to download -f, --from INTEGER
+Passed to the search it will bypass the first n documents -l, --limit INTEGER
+Limit the total results to return --size INTEGER Size of the scroll request
+that powers the operation. --query-field / --no-query-field Add the query to
+the export CSV --help Show this message and exit. ``` ### Tagging A command to
+batch tag documents with a CSV file. ``` Usage: tarentula tagging [OPTIONS]
+CSV_PATH Options: --datashare-url TEXT http://localhost:8080 Datashare URL --
+datashare-project TEXT local-datashare Datashare project --throttle INTEGER 0
+Request throttling (in ms) --cookies TEXT _Empty string_ Key/value pair to add
+a cookie to each request to the API. You can separate semicolons:
+key1=val1;key2=val2;... --apikey TEXT None Datashare authentication apikey --
+traceback / --no-traceback Display a traceback in case of error --progressbar /
+--no-progressbar Display a progressbar --help Show this message and exit ```
+#### CSV formats Tagging with a `documentId` and `routing`: ```csv
+tag,documentId,routing Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
 Antrodiaetidae,DWLOskax28jPQ2CjFrCo
 Atracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN
 Atypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi
 Barychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi ``` Tagging with a
 `documentUrl`: ```csv tag,documentUrl Mecicobothriidae,http://localhost:8080/#/
 d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi
 Microstigmatidae,http://localhost:8080/#/d/local-datashare/
@@ -109,19 +115,57 @@
 Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used to
 perform update by query --throttle INTEGER Request throttling (in ms) --cookies
 TEXT Key/value pair to add a cookie to each request to the API. You can
 separatesemicolons: key1=val1;key2=val2;... --apikey TEXT Datashare
 authentication apikey --traceback / --no-traceback Display a traceback in case
 of error --progressbar / --no-progressbar Display a progressbar --wait-for-
 completion / --no-wait-for-completion Create a Elasticsearch task to perform
-the updateasynchronously --help Show this message and exit ``` ### Following
-your changes When running Elasticsearch changes on big datasets, it could take
-a very long time. As we were curling ES to see if the task was still running
-well, we added a small utility to follow the changes. It makes a live graph of
-a provided ES indicator with a specified filter. It uses [mathplotlib](https://
+the updateasynchronously --help Show this message and exit ``` ### List
+Metadata You can list the metadata from the mapping, optionally counting the
+number of occurrences of each field in the index, with the `--count` parameter.
+Counting the fields is disabled by default. It includes a `--filter_by`
+parameter to narrow retrieving metadata properties of specific sets of
+documents. For instance it can be used to get just emails related properties
+with: `--filter_by "contentType=message/rfc822"` ``` $ tarentula list-metadata
+--help Usage: tarentula list-metadata [OPTIONS] Options: --datashare-project
+TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
+Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
+(useful when dealing with a lot of results) --type [Document|NamedEntity] Type
+of indexed documents to get metadata --filter_by TEXT Filter documents by pairs
+concatenated by coma of field names and values separated by =.Example
+"contentType=message/rfc822,content Type=message/rfc822" --count / --no-count
+Count or not the number of docs for each property found --help Show this
+message and exit. ``` ### Aggregate You can run aggregations on the data, the
+ElasticSearch aggregations API is partially enabled with this command. The
+possibilities are: - count: grouping by a given field different values, and
+count the num of docs. - nunique: returns the number of unique values of a
+given field. - date_histogram: returns counting of monthly or yearly grouped
+values for a given date field. - sum: returns the sum of values of number type
+fields. - min: returns the min of values of number type fields. - max: returns
+the max of values of number type fields. - avg: returns the average of values
+of number type fields. - stats: returns a bunch of statistics for a given
+number type fields. - string_stats: returns a bunch of string statistics for a
+given string type fields. ``` $ tarentula aggregate --help Usage: tarentula
+aggregate [OPTIONS] Options: --apikey TEXT Datashare authentication apikey --
+datashare-url TEXT Datashare URL --datashare-project TEXT Datashare project --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in order
+to use scrollingcapabilities of Elasticsearch (useful when dealing with a lot
+of results) --query TEXT The query string to filter documents --cookies TEXT
+Key/value pair to add a cookie to each request to the API. You can
+separatesemicolons: key1=val1;key2=val2;... --traceback / --no-traceback
+Display a traceback in case of error --type [Document|NamedEntity] Type of
+indexed documents to download --group_by TEXT Field to use to aggregate results
+--operation_field TEXT Field to run the operation on --run
+[count|nunique|date_histogram|sum|stats|string_stats|min|max|avg] Operation to
+run --calendar_interval [year|month] Calendar interval for date histogram
+aggregation --help Show this message and exit. ``` ### Following your changes
+When running Elasticsearch changes on big datasets, it could take a very long
+time. As we were curling ES to see if the task was still running well, we added
+a small utility to follow the changes. It makes a live graph of a provided ES
+indicator with a specified filter. It uses [mathplotlib](https://
 matplotlib.org/) and python3-tk. If you see the following message : ``` $
 graph_es graph_realtime.py:32: UserWarning: Matplotlib is currently using agg,
 which is a non-GUI backend, so cannot show the figure ``` Then you have to
 install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e.
 python3-tk for Debian/Ubuntu. The command has the options below: ``` $ graph_es
 --help Usage: graph_es [OPTIONS] Options: --query TEXT Give a JSON query to
 filter documents. It can be a file with @path/to/file. Default to all. --index
@@ -149,10 +193,13 @@
 package and [Docker Hub](https://hub.docker.com/) for the Docker image. ### 1.
 Create a new release ``` make [patch|minor|major] ``` ### 2. Upload
 distributions on pypi _To be able to do this, you will need to be a maintainer
 of the [pypi](https://pypi.org/project/tarentula/) project._ ``` make
 distribute ``` ### 3. Build and publish the Docker image To build and upload a
 new image on the [docker repository](https://hub.docker.com/repository/docker/
 icij/datashare-tarentula) : _To be able to do this, you will need to be part of
-the ICIJ organization on docker_ ``` make docker-publish ``` ### 4. Push your
-changes on Github Git push release and tag : ``` git push origin master --tags
-```
+the ICIJ organization on docker_ ``` make docker-publish ``` **Note**:
+Datashare Tarentula is a multi-platform build. You might need to setup your
+environment for multi-platform using the `make docker-setup-multiarch` command.
+Read more [on Docker documentation](https://docs.docker.com/build/building/
+multi-platform/). ### 4. Push your changes on Github Git push release and tag :
+``` git push origin master --tags ```
```

### Comparing `tarentula-4.3.3/pyproject.toml` & `tarentula-4.3.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tarentula"
-version = "4.3.3"
+version = "4.3.4"
 description = ""
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "tarentula"}]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
@@ -14,14 +14,16 @@
 rich = "^12"
 
 [tool.poetry.group.dev.dependencies]
 responses = "^0.22"
 pyyaml = "==5.4.0"
 argh = "==0.26.2"
 pytest = "^7.2.0"
+matplotlib = "^3.6"
+pylint = "^2.17.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 tarentula = "tarentula.cli:cli"
```

### Comparing `tarentula-4.3.3/tarentula/cli.py` & `tarentula-4.3.4/tarentula/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import click
 import logging
+import click
 
 from tarentula.config_file_reader import ConfigFileReader
 from tarentula.logger import add_syslog_handler, add_stdout_handler
+from tarentula.metadata_fields import MetadataFields
 from tarentula.tag_cleaning_by_query import TagsCleanerByQuery
 from tarentula.tagging import Tagger
 from tarentula.tagging_by_query import TaggerByQuery
 from tarentula.download import Download
 from tarentula.export_by_query import ExportByQuery
 from tarentula.count import Count
+from tarentula.aggregate import AggCount, GeneralStats, DateHistogram, NumUnique
 from tarentula import __version__
 
 
 def validate_loglevel(ctx, param, value):
+    # pylint: disable=unused-argument
     try:
         if isinstance(value, str):
             return getattr(logging, value)
         return int(value)
-    except (AttributeError, ValueError):
-        raise click.BadParameter('must be a valid log level (CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET)')
+    except (AttributeError, ValueError) as exc:
+        raise click.BadParameter('must be a valid log level (CRITICAL, ERROR, WARNING, INFO, DEBUG or NOTSET)') from exc
 
 
 def validate_progressbar(ctx, param, value):
+    # pylint: disable=unused-argument
     # If no value given, we activate the progress bar only when the
     # stdout_loglevel value is higher than INFO (20)
     return value if value is not None else ctx.obj['stdout_loglevel'] > 20
 
 
 @click.group()
 @click.pass_context
@@ -46,16 +50,18 @@
     # Pass all option to context
     ctx.ensure_object(dict)
     ctx.obj.update(options)
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-url', help='Datashare URL', default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--throttle', help='Request throttling (in ms)', default=0)
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
               callback=validate_progressbar)
 @click.argument('csv-path', type=click.Path(exists=True))
@@ -64,15 +70,16 @@
     tagger = Tagger(**options)
     # Proceed to tagging
     tagger.start()
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--elasticsearch-url', help='Elasticsearch URL which is used to perform update by query',
               default='http://localhost:9200')
 @click.option('--throttle', help='Request throttling (in ms)', default=0)
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
@@ -85,15 +92,16 @@
     # Instantiate a TaggerByQuery class with all the options
     tagger = TaggerByQuery(**options)
     tagger.start()
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--elasticsearch-url', help='Elasticsearch URL which is used to perform update by query',
               default='http://localhost:9200')
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--wait-for-completion/--no-wait-for-completion', help='Create a Elasticsearch task to perform the update'
                                                                      'asynchronously', default=True)
 @click.option('--query', help='Give a JSON query to filter documents that will have their tags cleaned. It can be a'
@@ -101,96 +109,171 @@
 def clean_tags_by_query(**options):
     tagger = TagsCleanerByQuery(**options)
     tagger.start()
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-url', help='Datashare URL', default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--elasticsearch-url', help='You can additionally pass the Elasticsearch URL in order to use scrolling'
                                           'capabilities of Elasticsearch (useful when dealing with a lot of results)',
               default=None)
 @click.option('--query', help='The query string to filter documents', default='*')
 @click.option('--destination-directory', help='Directory documents will be downloaded', default='./tmp')
 @click.option('--throttle', help='Request throttling (in ms)', default=0)
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--path-format', help='Downloaded document path template', default='{id_2b}/{id_4b}/{id}')
 @click.option('--scroll', help='Scroll duration', default=None)
 @click.option('--source', help='A comma-separated list of field to include in the downloaded document from the index',
               default=None)
+@click.option('--limit', '-l', type=int, help='Limit the total results to return', default=0)
+@click.option('--from', '-f', 'from_', type=int, help='Passed to the search it will bypass the first n documents',
+              default=0)
+@click.option('--size', help='Size of the scroll request that powers the operation.', default=1000)
 @click.option('--sort-by', help='Field to use to sort results', default='_id')
-@click.option('--order-by', help='Order to use to sort results', default='asc', 
-                            type=click.Choice(['asc', 'desc']))
+@click.option('--order-by', help='Order to use to sort results', default='asc',
+              type=click.Choice(['asc', 'desc']))
 @click.option('--once/--not-once', help='Download file only once', default=False)
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
               callback=validate_progressbar)
 @click.option('--raw-file/--no-raw-file', help='Download raw file from Datashare', default=True)
 @click.option('--type', help='Type of indexed documents to download', default='Document',
               type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
 def download(**options):
     # Instantiate a Download class with all the options
-    download = Download(**options)
-    download.start()
+    downl = Download(**options)
+    downl.start()
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-url', help='Datashare URL', default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--elasticsearch-url', help='You can additionally pass the Elasticsearch URL in order to use scrolling'
                                           'capabilities of Elasticsearch (useful when dealing with a lot of results)',
               default=None)
 @click.option('--query', help='The query string to filter documents', default='*')
 @click.option('--output-file', help='Path to the CSV file', default='tarentula_documents.csv')
 @click.option('--throttle', help='Request throttling (in ms)', default=0)
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--scroll', help='Scroll duration', default=None)
 @click.option('--source', help='A comma-separated list of field to include in the export',
               default='contentType,contentLength:0,extractionDate,path')
 @click.option('--sort-by', help='Field to use to sort results', default='_id')
-@click.option('--order-by', help='Order to use to sort results', default='asc', 
-                            type=click.Choice(['asc', 'desc']))
+@click.option('--order-by', help='Order to use to sort results', default='asc',
+              type=click.Choice(['asc', 'desc']))
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
               callback=validate_progressbar)
 @click.option('--type', help='Type of indexed documents to download', default='Document',
               type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
 @click.option('--size', help='Size of the scroll request that powers the operation.', default=1000)
+@click.option('--from', '-f', 'from_', type=int, help='Passed to the search it will bypass the first n documents',
+              default=0)
+@click.option('--limit', '-l', type=int, help='Limit the total results to return', default=0)
 @click.option('--query-field/--no-query-field', help='Add the query to the export CSV', default=True)
 def export_by_query(**options):
     # Instantiate an ExportByQuery class with all the options
     export = ExportByQuery(**options)
     export.start()
 
 
 @click.command()
 @click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
-@click.option('--datashare-url', help='Datashare URL', default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
-@click.option('--datashare-project', help='Datashare project', default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
 @click.option('--elasticsearch-url', help='You can additionally pass the Elasticsearch URL in order to use scrolling'
                                           'capabilities of Elasticsearch (useful when dealing with a lot of results)',
               default=None)
 @click.option('--query', help='The query string to filter documents', default='*')
 @click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
                                 'semicolons: key1=val1;key2=val2;...', default='')
 @click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
 @click.option('--type', help='Type of indexed documents to download', default='Document',
               type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
 def count(**options):
     # Instantiate a Count class with all the options
-    count = Count(**options)
-    count.start()
+    cnt = Count(**options)
+    cnt.start()
+
+
+@click.command()
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--elasticsearch-url', help='You can additionally pass the Elasticsearch URL in order to use scrolling'
+                                          'capabilities of Elasticsearch (useful when dealing with a lot of results)',
+              default=None)
+@click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
+@click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
+                                'semicolons: key1=val1;key2=val2;...', default='')
+@click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
+@click.option('--type', help='Type of indexed documents to get metadata', default='Document',
+              type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
+@click.option('--filter_by',
+              help='Filter documents by pairs concatenated by coma of field names and values separated by =.'
+                   'Example "contentType=message/rfc822,contentType=message/rfc822"', default='')
+@click.option('--count/--no-count', help='Count or not the number of docs for each property found', default=False)
+def list_metadata(**options):
+    metadata = MetadataFields(**options)
+    metadata.start()
+
+
+@click.command()
+@click.option('--apikey', help='Datashare authentication apikey', default=ConfigFileReader('apikey'))
+@click.option('--datashare-url', help='Datashare URL',
+              default=ConfigFileReader('datashare_url', 'http://localhost:8080'))
+@click.option('--datashare-project', help='Datashare project',
+              default=ConfigFileReader('datashare_project', 'local-datashare'))
+@click.option('--elasticsearch-url', help='You can additionally pass the Elasticsearch URL in order to use scrolling'
+                                          'capabilities of Elasticsearch (useful when dealing with a lot of results)',
+              default=None)
+@click.option('--query', help='The query string to filter documents', default='*')
+@click.option('--cookies', help='Key/value pair to add a cookie to each request to the API. You can separate'
+                                'semicolons: key1=val1;key2=val2;...', default='')
+@click.option('--traceback/--no-traceback', help='Display a traceback in case of error', default=False)
+@click.option('--type', help='Type of indexed documents to download', default='Document',
+              type=click.Choice(['Document', 'NamedEntity'], case_sensitive=True))
+@click.option('--group_by', help='Field to use to aggregate results', default=None)
+@click.option('--operation_field', help='Field to run the operation on', default=None)
+@click.option('--run', help='Operation to run ', default='count',
+              type=click.Choice(
+                  ['count', 'nunique', 'date_histogram', 'sum', 'stats', 'string_stats', 'min', 'max', 'avg']))
+@click.option('--calendar_interval', help='Calendar interval for date histogram aggregation', default='year',
+              type=click.Choice(['year', 'month']))
+def aggregate(**options):
+    agg_operation = options['run']
+
+    if agg_operation == 'count':
+        agg = AggCount(**options)
+    elif agg_operation == 'nunique':
+        agg = NumUnique(**options)
+    elif agg_operation == 'date_histogram':
+        agg = DateHistogram(**options)
+    elif agg_operation in ['sum', 'stats', 'string_stats', 'min', 'max', 'avg']:
+        agg = GeneralStats(**options)
+
+    agg.start()
 
 
 cli.add_command(tagging)
 cli.add_command(download)
 cli.add_command(tagging_by_query)
 cli.add_command(clean_tags_by_query)
 cli.add_command(export_by_query)
 cli.add_command(count)
+cli.add_command(list_metadata)
+cli.add_command(aggregate)
 
 if __name__ == '__main__':
-    cli()
+    cli(None) # ctx from @cli.pass_context
```

### Comparing `tarentula-4.3.3/tarentula/config_file_reader.py` & `tarentula-4.3.4/tarentula/config_file_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Optional
 from pathlib import Path
 from os.path import join, isfile
 
 import configparser
 import os
 
+
 class ConfigFileReader:
-    def __init__(self, name, defaultValue = None, section = 'DEFAULT'):
+    def __init__(self, name, default_value=None, section='DEFAULT'):
         self.name = name
-        self.defaultValue = defaultValue
+        self.default_value = default_value
         self.section = section
 
     def __call__(self) -> Optional[str]:
         if self.config_has_section:
-            return self.config[self.section].get(self.name, self.defaultValue)
-        return self.defaultValue
+            return self.config[self.section].get(self.name, self.default_value)
+        return self.default_value
 
     @property
     def config(self):
         config = configparser.ConfigParser()
         if self.config_path is not None:
             config.read(self.config_path)
         return config
@@ -28,14 +29,15 @@
         return self.section == 'DEFAULT' or self.config.has_section(self.section)
 
     @property
     def config_path(self) -> Optional[str]:
         for path in self.config_paths:
             if path is not None and isfile(path):
                 return path
+        return None
 
     @property
     def config_paths(self) -> list:
         return [
             self.env_path,
             self.current_directory_path,
             self.home_directory_path,
@@ -43,14 +45,15 @@
         ]
 
     @property
     def env_path(self) -> Optional[str]:
         env_value = os.getenv('TARENTULA_CONFIG', None)
         if env_value is not None:
             return os.path.abspath(env_value)
+        return None
 
     @property
     def home_directory_path(self) -> str:
         return join(Path.home(), '.tarentula.ini')
 
     @property
     def current_directory_path(self) -> str:
```

### Comparing `tarentula-4.3.3/tarentula/count.py` & `tarentula-4.3.4/tarentula/aggregate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,122 @@
 import json
+import sys
 
+from tarentula.command import Command
 from tarentula.datashare_client import DatashareClient
 from tarentula.logger import logger
 
 
-class Count:
+class Aggregate(Command):
     def __init__(self,
                  datashare_url: str = 'http://localhost:8080',
                  datashare_project: str = 'local-datashare',
                  query: str = '*',
                  cookies: str = '',
                  apikey: str = None,
                  elasticsearch_url: str = None,
                  traceback: bool = False,
-                 type: str = 'Document'):
+                 type: str = 'Document',
+                 group_by: str = 'contentType',
+                 operation_field: str = None,
+                 run: str = 'count',
+                 calendar_interval: str = 'year'
+                 ):
+        super().__init__(query, type)
         self.datashare_url = datashare_url
         self.datashare_project = datashare_project
-        self.query = query
         self.cookies_string = cookies
         self.apikey = apikey
         self.traceback = traceback
-        self.type = type
+        self.group_by = group_by
+        self.run = run
+        self.operation_field = operation_field
+        self.calendar_interval = calendar_interval
+        self.agg_level_1 = None
         try:
             self.datashare_client = DatashareClient(datashare_url,
                                                     elasticsearch_url,
                                                     datashare_project,
                                                     cookies,
                                                     apikey)
         except (ConnectionRefusedError, ConnectionError):
             logger.critical('Unable to connect to Datashare', exc_info=self.traceback)
-            exit()
+            sys.exit()
 
     @property
-    def query_body(self):
-        if self.query.startswith('@'):
-            return self.query_body_from_file
-        else:
-            return self.query_body_from_string
+    def query_body_from_string(self):
+        return {
+            "aggs": {
+                "aggregation-1": self.agg_level_1,
+            },
+            "query": (super().query_body_from_string['query'])
+        }
+
+    def aggregate_matches(self):
+        index = self.datashare_project
+        return self.datashare_client.query(index=index, query=self.query_body).get('aggregations')
+
+    def start(self):
+        agg = self.aggregate_matches()
+        print(json.dumps(agg, indent=4))
+
+
+class AggCount(Aggregate):
 
     @property
     def query_body_from_string(self):
-        return {
-            "query": {
-                "bool": {
-                    "must": [
-                        {
-                            "match": {
-                                "type": self.type
-                            }
-                        },
-                        {
-                            "query_string": {
-                                "query": self.query
-                            }
-                        }
-                    ]
+        self.agg_level_1 = {
+            "aggs": {
+                "bucket_truncate": {
+                    "bucket_sort": {
+                        "from": 0,
+                        "size": 25
+                    }
                 }
+            },
+            "terms": {
+                "field": self.group_by,
+                "order": {
+                    "_count": "desc"
+                },
+                "size": 25
             }
         }
+        return super().query_body_from_string
+
+
+class NumUnique(Aggregate):
 
     @property
-    def query_body_from_file(self):
-        with open(self.query[1:]) as json_file:
-            query_body = json.load(json_file)
-        return query_body
+    def query_body_from_string(self):
+        self.agg_level_1 = {
+            "cardinality": {
+                "field": self.operation_field
+            }
+        }
+        return super().query_body_from_string
 
-    def count_matches(self):
-        index = self.datashare_project
-        return self.datashare_client.count(index=index, query=self.query_body).get('count')
 
-    def log_matches(self):
-        index = self.datashare_project
-        count = self.count_matches()
-        logger.info('%s matching document(s) in %s' % (count, index))
-        return count
+class DateHistogram(Aggregate):
 
-    def start(self):
-        count = self.log_matches()
-        logger.info('Number of matched elements: %s' % count)
-        print('Number of matched elements: %s' % count)
+    @property
+    def query_body_from_string(self):
+        self.agg_level_1 = {
+            "date_histogram": {
+                "field": self.operation_field,
+                "calendar_interval": self.calendar_interval
+            }
+        }
+        return super().query_body_from_string
+
+
+class GeneralStats(Aggregate):
+    """Run one of the following agreggations: 'sum', 'stats', 'string_stats', 'min', 'max', 'avg' """
+
+    @property
+    def query_body_from_string(self):
+        self.agg_level_1 = {
+            self.run: {
+                "field": self.operation_field
+            }
+        }
+        return super().query_body_from_string
```

### Comparing `tarentula-4.3.3/tarentula/download.py` & `tarentula-4.3.4/tarentula/download.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,73 @@
 import json
 import shutil
+import sys
 from os import makedirs
 from os.path import join, dirname, basename, exists
 from time import sleep
 from requests.exceptions import HTTPError, ConnectionError
 from rich.progress import Progress
 from urllib3.exceptions import ProtocolError
 
+from tarentula.command import Command
 from tarentula.datashare_client import DatashareClient
 from tarentula.logger import logger
 
 
-class Download:
+class Download(Command):
     def __init__(self,
                  datashare_url: str = 'http://localhost:8080',
                  datashare_project: str = 'local-datashare',
                  destination_directory: str = './tmp',
                  query: str = '*',
                  throttle: int = 0,
                  cookies: str = '',
                  apikey: str = None,
                  elasticsearch_url: str = None,
                  path_format: str = '{id_2b}/{id_4b}/{id}',
                  scroll: str = None,
                  source: str = None,
+                 limit: int = 0,
+                 from_: int = 0,
+                 size: int = 0,
                  sort_by: str = '_id',
                  order_by: str = 'asc',
                  once: bool = False,
                  traceback: bool = False,
                  progressbar: bool = True,
                  raw_file: bool = True,
                  type: str = 'Document'):
+        super().__init__(query, type)
         self.datashare_url = datashare_url
         self.datashare_project = datashare_project
-        self.query = query
         self.destination_directory = destination_directory
         self.throttle = throttle
         self.cookies_string = cookies
         self.apikey = apikey
         self.path_format = path_format
         self.once = once
         self.traceback = traceback
         self.progressbar = progressbar
         self.raw_file = raw_file
         self.source = source
         self.scroll = scroll
+        self.limit = limit
+        self.from_ = from_
+        self.size = size
         self.sort_by = sort_by
         self.order_by = order_by
-        self.type = type
         try:
             self.datashare_client = DatashareClient(datashare_url,
                                                     elasticsearch_url,
                                                     datashare_project,
                                                     cookies,
                                                     apikey)
         except (ConnectionRefusedError, ConnectionError):
             logger.critical('Unable to connect to Datashare', exc_info=self.traceback)
-            exit()
-
-    @property
-    def query_body(self):
-        if self.query.startswith('@'):
-            return self.query_body_from_file
-        else:
-            return self.query_body_from_string
-
-    @property
-    def query_body_from_string(self):
-        return {
-            "query": {
-                "bool": {
-                    "must": [
-                        {
-                            "match": {
-                                "type": self.type
-                            }
-                        },
-                        {
-                            "query_string": {
-                                "query": self.query
-                            }
-                        }
-                    ]
-                }
-            }
-        }
-
-    @property
-    def query_body_from_file(self):
-        with open(self.query[1:]) as json_file:
-            query_body = json.load(json_file)
-        return query_body
+            sys.exit()
 
     @property
     def no_progressbar(self):
         return not self.progressbar
 
     def sleep(self):
         sleep(self.throttle / 1000)
@@ -124,50 +97,50 @@
         if parents:
             parents_path = dirname(file_path)
             makedirs(parents_path, exist_ok=True)
         return file_path
 
     def count_matches(self):
         index = self.datashare_project
-        return self.datashare_client.count(index=index, query=self.query_body).get('count')
+        total_matched = self.datashare_client \
+            .count(index=index, query=self.query_body) \
+            .get('count')
+        total_matched = total_matched - self.from_ if total_matched >= self.from_ \
+            else total_matched
+        total_matched = total_matched if (self.limit == 0) or \
+                                         (self.limit > total_matched) \
+            else self.limit
+        return total_matched
 
     def log_matches(self):
         index = self.datashare_project
         count = self.count_matches()
-        logger.info('%s matching document(s) in %s' % (count, index))
+        logger.info('%s matching document(s) in %s', count, index)
         return count
 
-    def scan_or_query_all(self):
-        index = self.datashare_project
-        source = ["path", "parentDocument", "type"] + str(self.source).split(',')
-        sort = { self.sort_by: self.order_by }
-        if self.scroll is None:
-            logger.info('Searching document(s) metadata in %s' % index)
-            return self.datashare_client.query_all(index=index, query=self.query_body, source=source, sort=sort)
-        else:
-            logger.info('Scrolling over document(s) metadata in %s' % index)
-            return self.datashare_client.scan_all(index=index, query=self.query_body, source=source, scroll=self.scroll, sort=sort)
-
     def download_raw_file(self, document):
         id = document.get('_id')
         routing = document.get('_routing', id)
         # Skip raw file
         if not self.raw_file:
-            return
+            return None
         # Skip existing
         if self.once and self.raw_file_exists(document):
-            return logger.info('Skipping existing document %s' % document.get('_id'))
+            logger.info('Skipping existing document %s', document.get('_id'))
+            return None
         # Skip non-downloadable file
         if document.get('_source', {}).get('type', None) != 'Document':
-            return logger.warning('Not a raw document. Skipping %s' % id)
-        logger.info('Downloading raw file %s' % id)
+            logger.warning('Not a raw document. Skipping %s', id)
+            return None
+        logger.info('Downloading raw file %s', id)
         document_file_stream = self.datashare_client.download(self.datashare_project, id, routing)
         document_file_stream.raw.decode_content = True
         document_file_stream.raise_for_status()
         self.save_raw_file(document, document_file_stream)
+        return None
 
     def raw_file_exists(self, document):
         raw_file_path = self.raw_file_path(document)
         return exists(raw_file_path)
 
     def save_raw_file(self, document, document_file_stream):
         file_path = self.raw_file_path(document)
@@ -177,22 +150,25 @@
     def save_indexed_document(self, indexed_document):
         file_path = self.indexed_document_path(indexed_document)
         with open(file_path, 'w') as file:
             json.dump(indexed_document, file)
 
     def start(self):
         count = self.log_matches()
-        desc = "Downloading %s document(s)" % count
+        desc = f'Downloading {count} document(s)'
+        source = ["path", "parentDocument", "type"] + str(self.source).split(',')
         try:
-            with Progress(disable=self.no_progressbar) as progress:  
+            with Progress(disable=self.no_progressbar) as progress:
                 task = progress.add_task(desc, total=count)
-                for document in self.scan_or_query_all():
+                for document in self.datashare_client.scan_or_query_all(self.datashare_project, source, self.sort_by,
+                                                                        self.order_by, self.scroll, self.query_body,
+                                                                        self.from_, self.limit, self.size):
                     try:
                         self.download_raw_file(document)
                         self.save_indexed_document(document)
-                        logger.info('Processed document %s' % document.get('_id'))
+                        logger.info('Processed document %s', document.get('_id'))
                     except HTTPError:
-                        logger.error('Unable to download document %s' % document.get('_id'), exc_info=self.traceback)
+                        logger.error('Unable to download document %s', document.get('_id'), exc_info=self.traceback)
                     progress.advance(task)
                     self.sleep()
         except ProtocolError:
             logger.error('Exception while downloading documents', exc_info=self.traceback)
```

### Comparing `tarentula-4.3.3/tarentula/export_by_query.py` & `tarentula-4.3.4/tarentula/export_by_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,81 @@
 import csv
-import json
+import sys
 
 from collections import OrderedDict
 from contextlib import contextmanager
+from time import sleep
 from requests.exceptions import HTTPError
 from rich.progress import Progress
 from urllib3.exceptions import ProtocolError
-from time import sleep
 
+from tarentula.command import Command
 from tarentula.datashare_client import DatashareClient
 from tarentula.logger import logger
 
 
-class ExportByQuery:
+class ExportByQuery(Command):
     def __init__(self,
                  datashare_url: str = 'http://localhost:8080',
                  datashare_project: str = 'local-datashare',
                  output_file: str = 'tarentula_documents.csv',
                  query: str = '*',
                  throttle: int = 0,
                  cookies: str = '',
                  apikey: str = None,
                  elasticsearch_url: str = None,
                  scroll: str = None,
                  source: str = 'contentType,contentLength:0,extractionDate,path',
                  size: int = 1000,
+                 from_: int = 0,
+                 limit: int = 0,
                  sort_by: str = '_id',
                  order_by: str = 'asc',
                  traceback: bool = False,
                  progressbar: bool = True,
                  type: str = 'Document',
                  query_field: bool = True):
+        super().__init__(query, type)
         self.datashare_url = datashare_url
         self.datashare_project = datashare_project
-        self.query = query
         self.output_file = output_file
         self.throttle = throttle
         self.cookies_string = cookies
         self.apikey = apikey
         self.traceback = traceback
         self.progressbar = progressbar
         self.scroll = scroll
         self.source = source
         self.size = size
+        self.from_ = from_
+        self.limit = limit
         self.sort_by = sort_by
         self.order_by = order_by
-        self.type = type
         self.query_field = query_field
         try:
             self.datashare_client = DatashareClient(datashare_url,
                                                     elasticsearch_url,
                                                     datashare_project,
                                                     cookies,
                                                     apikey)
         except (ConnectionRefusedError, ConnectionError):
             logger.critical('Unable to connect to Datashare', exc_info=self.traceback)
-            exit()
-
-    @property
-    def query_body(self):
-        if self.query.startswith('@'):
-            return self.query_body_from_file
-        else:
-            return self.query_body_from_string
-
-    @property
-    def query_body_from_string(self):
-        return {
-            "query": {
-                "bool": {
-                    "must": [
-                        {
-                            "match": {
-                                "type": self.type
-                            }
-                        },
-                        {
-                            "query_string": {
-                                "query": self.query
-                            }
-                        }
-                    ]
-                }
-            }
-        }
-
-    @property
-    def query_body_from_file(self):
-        with open(self.query[1:]) as json_file:
-            query_body = json.load(json_file)
-        return query_body
+            sys.exit()
 
     @property
     def no_progressbar(self):
         return not self.progressbar
 
     @property
     def source_fields(self):
-        return [ self.source_field_params(f) for f in self.source.split(',') ]
+        return [self.source_field_params(f) for f in self.source.split(',')]
 
     @property
     def source_fields_names(self):
-        return [ field.pop(0) for field in self.source_fields ]
+        return [field.pop(0) for field in self.source_fields]
 
     @property
     def csv_fields_names(self):
         names = self.default_csv_fields_names
         names += self.source_fields_names
         # Remove duplicated values while preserving order
         return list(OrderedDict.fromkeys(names))
@@ -113,52 +83,50 @@
     @property
     def default_csv_fields_names(self):
         names = ['documentUrl', 'documentId', 'rootId', 'documentNumber']
         if self.query_field:
             names.insert(0, 'query')
         return names
 
-
     def source_field_params(self, field):
         field_params = field.strip().split(':')
         field_name = field_params[0]
         field_default = field_params[1] if len(field_params) > 1 else ''
         return [field_name, field_default]
 
     def sleep(self):
         sleep(self.throttle / 1000)
 
     def count_matches(self):
         index = self.datashare_project
-        return self.datashare_client.count(index=index, query=self.query_body).get('count')
+        total_matched = self.datashare_client \
+            .count(index=index, query=self.query_body) \
+            .get('count')
+        total_matched = total_matched - self.from_ if total_matched >= self.from_ \
+            else total_matched
+        total_matched = total_matched if (self.limit == 0) or \
+                                         (self.limit > total_matched) \
+            else self.limit
+        return total_matched
 
     def log_matches(self):
         index = self.datashare_project
         count = self.count_matches()
-        logger.info('%s matching document(s) in %s' % (count, index))
+        logger.info('%s matching document(s) in %s', count, index)
         return count
 
-    def scan_or_query_all(self):
-        index = self.datashare_project
-        source = self.source_fields_names
-        sort = { self.sort_by: self.order_by }
-        if self.scroll is None:
-            logger.info('Searching document(s) metadata in %s' % index)
-            return self.datashare_client.query_all(index=index, query=self.query_body, source=source, size=self.size, sort=sort)
-        else:
-            logger.info('Scrolling over document(s) metadata in %s' % index)
-            return self.datashare_client.scan_all(index=index, query=self.query_body, source=source, scroll=self.scroll, size=self.size, sort=sort)
-
     def document_default_values(self, document, number):
         index = self.datashare_project
         id = document.get('_id')
         routing = document.get('_routing', id)
         url = self.datashare_client.document_url(index, id, routing)
-        return { 'query': self.query, 'documentUrl': url, 'documentId': id,
-                 'rootId': routing, 'documentNumber': number }
+        values = {'documentUrl': url, 'documentId': id, 'rootId': routing, 'documentNumber': number}
+        if self.query_field:
+            return {'query': self.query, **values}
+        return values
 
     def document_source_values(self, document):
         source_values = {}
         source = document.get('_source', {})
         for [name, default] in self.source_fields:
             # Get the nested value for `name` (it can be a path, ie: metadata.tika_metadata_author)
             source_values[name] = source
@@ -168,36 +136,41 @@
                 except (KeyError, TypeError):
                     source_values[name] = default
         return source_values
 
     def save_indexed_document(self, csvwriter, document, document_number):
         default_values = self.document_default_values(document, document_number)
         source_values = self.document_source_values(document)
-        csvwriter.writerow({ **default_values, **source_values })
+        csvwriter.writerow({**default_values, **source_values})
 
     @contextmanager
     def create_csv_file(self):
         with open(self.output_file, 'w', newline='') as csv_file:
-            writer = csv.DictWriter(csv_file, fieldnames=self.csv_fields_names)
+            writer = csv.DictWriter(csv_file,
+                                    fieldnames=self.csv_fields_names,
+                                    escapechar='\\')
             writer.writeheader()
             yield writer
 
     def start(self):
         count = self.log_matches()
-        desc = 'Exporting %s document(s)' % count
+        desc = f'Exporting {count} document(s)'
         try:
-            with Progress(disable=self.no_progressbar) as progress:  
-                task = progress.add_task(desc, total=count) 
-                documents = self.scan_or_query_all()
+            with Progress(disable=self.no_progressbar) as progress:
+                task = progress.add_task(desc, total=count)
+                documents = self.datashare_client.scan_or_query_all(self.datashare_project, self.source_fields_names,
+                                                                    self.sort_by,
+                                                                    self.order_by, self.scroll, self.query_body,
+                                                                    self.from_, self.limit, self.size)
                 with self.create_csv_file() as csvwriter:
                     for index, document in enumerate(documents):
                         try:
                             self.save_indexed_document(csvwriter, document, index)
-                            logger.info('Saved document %s' % document.get('_id', None))
+                            logger.info('Saved document %s', document.get('_id', None))
                         except HTTPError:
-                            logger.error('Unable to export document %s' % document.get('_id', None),
-                                exc_info=self.traceback)
+                            logger.error('Unable to export document %s', document.get('_id', None),
+                                         exc_info=self.traceback)
                         progress.advance(task)
                         self.sleep()
-                logger.info('Written documents metadata in %s' % self.output_file)
+                logger.info('Written documents metadata in %s', self.output_file)
         except ProtocolError:
             logger.error('Exception while exporting documents', exc_info=self.traceback)
```

### Comparing `tarentula-4.3.3/tarentula/graph_realtime.py` & `tarentula-4.3.4/tarentula/graph_realtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,49 +13,54 @@
                  xs_param: list = None, ys_param: list = None):
         if query.startswith("@"):
             with open(query[1:]) as f:
                 self.query = json.loads(f.read())
         else:
             self.query = json.loads(query)
         self.field = field
-        self.elasticsearch_endpoint = '%s/%s/_search?size=0' % (elasticsearch_url, index)
+        self.elasticsearch_endpoint = f'{elasticsearch_url}/{index}/_search?size=0'
         self.refresh_interval = refresh_interval
         self.xs = [] if xs_param is None else xs_param
         self.ys = [] if xs_param is None else ys_param
 
         fig = plt.figure()
         self.ani = animation.FuncAnimation(fig, self.add_point, interval=self.refresh_interval * 1000)
         self.ax = fig.add_subplot(1, 1, 1)
         plt.gcf().autofmt_xdate()
 
     def show_graph(self):
         plt.show()
 
     def add_point(self, _i):
-        result = requests.post(self.elasticsearch_endpoint, json=self.query).json()
+        # pylint: disable=invalid-name
+        result = requests.post(self.elasticsearch_endpoint, json=self.query, timeout=10).json()
         x = datetime.now()
         # call get on result while there are dots in self.field
         y = functools.reduce(dict.get, [result] + self.field.split('.'))
 
         self.xs.append(x)
         self.ys.append(y)
         self.ax.clear()
         self.ax.plot(self.xs, self.ys)
 
         plt.xticks(rotation=45, ha='right')
-        plt.title("Dynamic Plot of %s" % self.field)
-        plt.xlabel("Time")
+        plt.title(f'Dynamic Plot of {self.field}')
+        plt.xlabel('Time')
         plt.ylabel(self.field)
 
 
 @click.command()
-@click.option('--query', help='Give a JSON query to filter documents. It can be a file with @path/to/file. Default to all.', default='{"query":{"match_all":{}}}')
+@click.option('--query',
+              help='Give a JSON query to filter documents. It can be a file with @path/to/file. Default to all.',
+              default='{"query":{"match_all":{}}}')
 @click.option('--index', help='Elasticsearch index (default local-datashare)', default='local-datashare')
 @click.option('--refresh-interval', help='Graph refresh interval in seconds (default 5)', default=5)
-@click.option('--field', help='Field indicator to display over time (default hits.total.value)', default='hits.total.value')
-@click.option('--elasticsearch-url', help='Elasticsearch URL which is used to perform update by query', default='http://elasticsearch:9200')
+@click.option('--field', help='Field indicator to display over time (default hits.total.value)',
+              default='hits.total.value')
+@click.option('--elasticsearch-url', help='Elasticsearch URL which is used to perform update by query',
+              default='http://elasticsearch:9200')
 def graph(**options) -> None:
     GraphRealTime(**options).show_graph()
 
 
 if __name__ == '__main__':
     graph()
```

### Comparing `tarentula-4.3.3/tarentula/logger.py` & `tarentula-4.3.4/tarentula/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import sys
-from syslog import LOG_LOCAL7
 
-import coloredlogs
+from syslog import LOG_LOCAL7
 from logging.handlers import SysLogHandler
+import coloredlogs
 
 logger = logging.getLogger('tarentula')
 logger.setLevel(logging.INFO)
 
 
 def default_log_formatter() -> logging.Formatter:
     return logging.Formatter('%(asctime)s :: %(name)s :: %(levelname)s :: %(message)s')
 
 
 def add_syslog_handler(address: str = 'localhost', port: int = 514, facility: int = LOG_LOCAL7) -> None:
-    sysLogFormatter = default_log_formatter()
-    sysLogHandler = SysLogHandler(address = (address, port), facility = facility)
-    sysLogHandler.setLevel(logging.INFO)
-    sysLogHandler.setFormatter(sysLogFormatter)
-    logger.addHandler(sysLogHandler)
+    syslog_formatter = default_log_formatter()
+    syslog_handler = SysLogHandler(address = (address, port), facility = facility)
+    syslog_handler.setLevel(logging.INFO)
+    syslog_handler.setFormatter(syslog_formatter)
+    logger.addHandler(syslog_handler)
 
 
 def add_stdout_handler(level: int = logging.ERROR) -> None:
     fmt = '%(levelname)s %(message)s'
     logger.addHandler(logging.StreamHandler(sys.stdout))
     coloredlogs.install(level=level, logger=logger, fmt=fmt, field_styles={ 'levelname': { 'faint': True } })
```

### Comparing `tarentula-4.3.3/tarentula/tag_cleaning_by_query.py` & `tarentula-4.3.4/tarentula/tag_cleaning_by_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from http.cookies import SimpleCookie
 
 import requests
 
+from tarentula.datashare_client import HTTP_REQUEST_TIMEOUT_SEC
 from tarentula.logger import logger
 
 
 class TagsCleanerByQuery:
     def __init__(self,
                  datashare_project: str = 'local-datashare',
                  elasticsearch_url: str = 'http://localhost:9200',
@@ -36,30 +37,32 @@
         except (TypeError, AttributeError):
             return {}
 
     @property
     def headers(self):
         if self.apikey is not None:
             return {
-                'Authorization': 'bearer %s' % self.apikey
+                'Authorization': f'bearer {self.apikey}'
             }
+        return None
 
     @property
     def tagging_by_query_endpoint(self):
         url_template = '{elasticsearch_url}/{datashare_project}/_update_by_query?conflicts=proceed'
         return url_template.format(elasticsearch_url=self.elasticsearch_url, datashare_project=self.datashare_project)
 
     def start(self):
         logger.info("This action will remove all tags for documents matching query")
         script = {"script": {"source": "ctx._source['tags'] = []"}}
         params = {"wait_for_completion": str(self.wait_for_completion).lower()}
-        result = requests.post(self.tagging_by_query_endpoint, 
-                                params=params, 
-                                json={**script, **self.query},
-                                cookies=self.cookies,
-                                headers=self.headers)
+        result = requests.post(self.tagging_by_query_endpoint,
+                               params=params,
+                               json={**script, **self.query},
+                               cookies=self.cookies,
+                               headers=self.headers,
+                               timeout=HTTP_REQUEST_TIMEOUT_SEC)
         result.raise_for_status()
         if self.wait_for_completion:
-            logger.info('updated %s documents' % result.json()['updated'])
+            logger.info('updated %s documents', result.json()['updated'])
         else:
-            logger.info('task created: [%s]' % result.json()['task'])
+            logger.info('task created: [%s]', result.json()['task'])
         return result
```

### Comparing `tarentula-4.3.3/tarentula/tagging.py` & `tarentula-4.3.4/tarentula/tagging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import csv
 import re
-import requests
 from time import sleep
-from rich.progress import Progress
 from http.cookies import SimpleCookie
+from rich.progress import Progress
+import requests
 from requests.exceptions import HTTPError, ConnectionError
 
+from tarentula.datashare_client import HTTP_REQUEST_TIMEOUT_SEC
 from tarentula.logger import logger
 
 DATASHARE_DOCUMENT_ROUTE = re.compile(r'/#/d/[a-zA-Z0-9_-]+/(\w+)(?:/(\w+))?$')
 
 
 class Tagger:
     def __init__(self,
@@ -40,15 +41,15 @@
             return list(self.sanitize_row(row) for row in csv.DictReader(csv_file))
 
     @property
     def tags(self):
         return list(dict.fromkeys([row['tag'] for row in self.csv_rows]))
 
     @property
-    def documentIds(self):
+    def document_ids(self):
         return list(dict.fromkeys([row['documentId'] for row in self.csv_rows]))
 
     @property
     def tree(self):
         tree = dict()
         for row in self.csv_rows:
             # Extract row values
@@ -70,16 +71,17 @@
         except (TypeError, AttributeError):
             return {}
 
     @property
     def headers(self):
         if self.apikey is not None:
             return {
-                'Authorization': 'bearer %s' % self.apikey
+                'Authorization': f'bearer {self.apikey}'
             }
+        return None
 
     @property
     def total_steps(self):
         return sum(len(leaf['tags']) for _, leaf in self.tree.items())
 
     def sleep(self):
         sleep(self.throttle / 1000)
@@ -88,44 +90,45 @@
         if 'documentUrl' in row:
             groups = DATASHARE_DOCUMENT_ROUTE.findall(row['documentUrl'])
             if len(groups) > 0:
                 row['documentId'], row['routing'] = groups[0]
         return row
 
     def leaf_tagging_endpoint(self, leaf):
-        document_id, tags, routing = (leaf['document_id'], leaf['tags'], leaf['routing'])
+        document_id, routing = (leaf['document_id'], leaf['routing'])
         # @see https://github.com/ICIJ/datashare/wiki/Datashare-API
         url_template = '{datashare_url}/api/{datashare_project}/documents/tags/{document_id}?routing={routing}'
         return url_template.format(
             datashare_url=self.datashare_url,
             datashare_project=self.datashare_project,
             document_id=document_id,
             routing=routing
         )
 
     def summarize(self):
-        summary = 'Adding %s tags to %s documents' % (len(self.tags), len(self.documentIds))
+        summary = f'Adding {len(self.tags)} tags to {len(self.document_ids)} documents'
         logger.info(summary)
         return summary
 
-    
     def start(self):
-        with Progress(disable=self.no_progressbar) as progress:     
+        with Progress(disable=self.no_progressbar) as progress:
             desc = self.summarize()
-            task = progress.add_task(desc, total=self.total_steps) 
+            task = progress.add_task(desc, total=self.total_steps)
             for document_id, leaf in self.tree.items():
                 endpoint_url = self.leaf_tagging_endpoint(leaf)
                 for tag in leaf['tags']:
                     try:
-                        result = requests.put(endpoint_url, 
-                                                json=[tag], 
-                                                cookies=self.cookies,
-                                                headers=self.headers)
+                        result = requests.put(endpoint_url,
+                                              json=[tag],
+                                              cookies=self.cookies,
+                                              headers=self.headers,
+                                              timeout=HTTP_REQUEST_TIMEOUT_SEC)
                         result.raise_for_status()
                         if result.status_code == requests.codes.ok:
-                            logger.info('Tag "%s" already exists on document "%s"' % (tag, document_id,))
+                            logger.info('Tag "%s" already exists on document "%s"', tag, document_id)
                         elif result.status_code == requests.codes.created:
-                            logger.info('Added "%s" to document "%s"' % (tag, document_id,))
+                            logger.info('Added "%s" to document "%s"', tag, document_id)
                         self.sleep()
                     except (HTTPError, ConnectionError):
-                        logger.warning('Unable to add "%s" to document "%s"' % (tag, document_id), exc_info=self.traceback)
+                        logger.warning('Unable to add "%s" to document "%s"', tag, document_id,
+                                       exc_info=self.traceback)
                     progress.advance(task)
```

### Comparing `tarentula-4.3.3/tarentula/tagging_by_query.py` & `tarentula-4.3.4/tarentula/tagging_by_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
-import requests
 
 from http.cookies import SimpleCookie
-from requests.exceptions import HTTPError, ConnectionError
 from time import sleep
+from requests.exceptions import HTTPError, ConnectionError
 from rich.progress import Progress
+import requests
 
+from tarentula.datashare_client import HTTP_REQUEST_TIMEOUT_SEC
 from tarentula.logger import logger
 
 
 class TaggerByQuery:
     def __init__(self,
                  datashare_project: str = '',
                  elasticsearch_url: str = '',
@@ -45,23 +46,23 @@
         except (TypeError, AttributeError):
             return {}
 
     @property
     def headers(self):
         if self.apikey is not None:
             return {
-                'Authorization': 'bearer %s' % self.apikey
+                'Authorization': f'bearer {self.apikey}'
             }
+        return None
 
     @property
     def tags(self):
-        json_file = open(self.json_path, 'r')
-        tags = json.loads(json_file.read())
-        json_file.close()
-        return tags
+        with open(self.json_path, 'r') as json_file:
+            tags = json.loads(json_file.read())
+            return tags
 
     @property
     def tagging_by_query_endpoint(self):
         url_template = '{elasticsearch_url}/{datashare_project}/_update_by_query?conflicts=proceed'
         return url_template.format(elasticsearch_url=self.elasticsearch_url, datashare_project=self.datashare_project)
 
     def sleep(self):
@@ -69,15 +70,15 @@
 
     def task_url(self, task):
         url_template = '{elasticsearch_url}/_tasks/{task}'
         return url_template.format(elasticsearch_url=self.elasticsearch_url, task=task)
 
     def tag_query_as_dict(self, query):
         if isinstance(query, str):
-            return { 
+            return {
                 "query": {
                     "query_string": {
                         "query": query
                     }
                 }
             }
         return query
@@ -100,38 +101,39 @@
             },
             **self.tag_query_as_dict(query)
         }
         params = {
             "wait_for_completion": str(self.wait_for_completion).lower(),
             "scroll_size": self.scroll_size,
         }
-        result = requests.post(self.tagging_by_query_endpoint, 
-                                params=params, 
-                                json=query, 
-                                cookies=self.cookies,
-                                headers=self.headers)
+        result = requests.post(self.tagging_by_query_endpoint,
+                               params=params,
+                               json=query,
+                               cookies=self.cookies,
+                               headers=self.headers,
+                               timeout=HTTP_REQUEST_TIMEOUT_SEC)
         result.raise_for_status()
         return result
 
     @property
     def tags_count(self):
         return len(self.tags.keys())
 
     def start(self):
         count = self.tags_count
-        desc = "This action will add %s tag(s)" % count
-        with Progress(disable=self.no_progressbar) as progress:  
+        desc = f'This action will add {count} tag(s)'
+        with Progress(disable=self.no_progressbar) as progress:
             task = progress.add_task(desc, total=count)
             for (tag, query) in self.tags.items():
                 try:
-                    progress.console.print('Adding "%s" tag' % tag)
+                    progress.console.print(f'Adding "{tag}" tag')
                     result = self.tag_documents(tag, query).json()
                     if self.wait_for_completion:
-                        progress.console.print('└── documents updated in %sms' % result['took'])
-                        logger.info('Documents tagged with [%s] in %sms' % (tag, result['took']))
+                        progress.console.print(f'└── documents updated in {result["took"]}ms')
+                        logger.info('Documents tagged with [%s] in %sms', tag, result['took'])
                     else:
-                        progress.console.print('└── task created: %s' % self.task_url(result['task']))
-                        logger.info('Task [%s] created for tag [%s]' % (result['task'], tag))
+                        progress.console.print(f'└── task created: {self.task_url(result["task"])}')
+                        logger.info('Task [%s] created for tag [%s]', result['task'], tag)
                     progress.advance(task)
                     self.sleep()
                 except (HTTPError, ConnectionError):
-                    logger.error('Unable to add tag [%s] (connection error)' % tag, exc_info=self.traceback)
+                    logger.error('Unable to add tag [%s] (connection error)', tag, exc_info=self.traceback)
```

### Comparing `tarentula-4.3.3/setup.py` & `tarentula-4.3.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['click>=8.1,<9.0', 'coloredlogs==14.0', 'requests>=2.28,<3.0', 'rich>=12,<13']
 
 entry_points = \
 {'console_scripts': ['tarentula = tarentula.cli:cli']}
 
 setup_kwargs = {
     'name': 'tarentula',
-    'version': '4.3.3',
+    'version': '4.3.4',
     'description': '',
-    'long_description': '# Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula)\n\nCli toolbelt for [Datashare](https://datashare.icij.org).\n\n```\n     /      \\\n  \\  \\  ,,  /  /\n   \'-.`\\()/`.-\'\n  .--_\'(  )\'_--.\n / /` /`""`\\ `\\ \\\n  |  |  ><  |  |\n  \\  \\      /  /\n      \'.__.\'\n\nUsage: tarentula [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --syslog-address      TEXT    localhost   Syslog address\n  --syslog-port         INTEGER 514         Syslog port\n  --syslog-facility     TEXT    local7      Syslog facility\n  --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler\n  --help                                    Show this message and exit\n  --version                                 Show the installed version of Tarentula\n\nCommands:\n  count\n  clean-tags-by-query\n  download\n  export-by-query\n  tagging\n  tagging-by-query\n```\n\n---\n<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->\n\n- [Usage](#usage)\n  - [Cookbook 👩\u200d🍳](#cookbook-)\n  - [Count](#count)\n  - [Clean Tags by Query](#clean-tags-by-query)\n  - [Download](#download)\n  - [Export by Query](#export-by-query)\n  - [Tagging](#tagging)\n    - [CSV formats](#csv-formats)\n  - [Tagging by Query](#tagging-by-query)\n  - [Following your changes](#following-your-changes)\n- [Configuration File](#configuration-file)\n- [Testing](#testing)\n- [Releasing](#releasing)\n  - [1. Create a new release](#1-create-a-new-release)\n  - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)\n  - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)\n  - [4. Push your changes on Github](#4-push-your-changes-on-github)\n\n<!-- /TOC -->\n---\n\n## Usage\n\nDatashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.\n\n### Cookbook 👩\u200d🍳\n\nTo learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.\n\n### Count\n\nA command to just count the number of files matching a query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n  --datashare-url           TEXT        Datashare URL\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        You can additionally pass the Elasticsearch\n                                          URL in order to use scrollingcapabilities of\n                                          Elasticsearch (useful when dealing with a\n                                          lot of results)\n  --query                   TEXT        The query string to filter documents\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n                                          in the downloaded document from the index\n  --traceback / --no-traceback          Display a traceback in case of error\n  --type [Document|NamedEntity]         Type of indexed documents to download\n  --help                                Show this message and exit\n```\n\n### Clean Tags by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch untag documents directly in the index.\n\n```\nUsage: tarentula clean-tags-by-query [OPTIONS]\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --query                   TEXT        Give a JSON query to filter documents that\n                                          will have their tags cleaned. It can be\n                                          afile with @path/to/file. Default to all.\n  --help                                Show this message and exit\n```\n\n### Download\n\nA command to download all files matching a query.\n\n```\nUsage: tarentula download [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --destination-directory TEXT    Directory documents will be downloaded\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --path-format TEXT              Downloaded document path template\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the downloaded document from the index\n\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --once / --not-once             Download file only once\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --raw-file / --no-raw-file      Download raw file from Datashare\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --help                          Show this message and exit.\n```\n\n\n### Export by Query\n\nA command to export all files matching a query.\n\n```\nUsage: tarentula export-by-query [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --output-file TEXT              Path to the CSV file\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the export\n\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --size INTEGER                  Size of the scroll request that powers the\n                                  operation.\n\n  --query-field / --no-query-field\n                                  Add the query to the export CSV\n  --help                          Show this message and exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents with a CSV file.\n\n```\nUsage: tarentula tagging [OPTIONS] CSV_PATH\n\nOptions:\n  --datashare-url       TEXT        http://localhost:8080   Datashare URL\n  --datashare-project   TEXT        local-datashare         Datashare project\n  --throttle            INTEGER     0                       Request throttling (in ms)\n  --cookies             TEXT        _Empty string_          Key/value pair to add a cookie to each request to the API. You can separate semicolons: key1=val1;key2=val2;...\n  --apikey              TEXT        None                    Datashare authentication apikey\n  --traceback / --no-traceback                              Display a traceback in case of error\n  --progressbar / --no-progressbar                          Display a progressbar\n  --help                                                    Show this message and exit\n```\n\n#### CSV formats\n\nTagging with a `documentId` and `routing`:\n\n```csv\ntag,documentId,routing\nActinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG\nAntrodiaetidae,DWLOskax28jPQ2CjFrCo\nAtracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN\nAtypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\nBarychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\n```\n\nTagging with a `documentUrl`:\n\n```csv\ntag,documentUrl\nMecicobothriidae,http://localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi\nMicrostigmatidae,http://localhost:8080/#/d/local-datashare/iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0\nMigidae,http://localhost:8080/#/d/local-datashare/BmovvXBisWtyyx6o9cuG/BmovvXBisWtyyx6o9cuG\nNemesiidae,http://localhost:8080/#/d/local-datashare/vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN\nParatropididae,http://localhost:8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/vYl1C4bsWphUKvXEBDhM\nPorrhothelidae,http://localhost:8080/#/d/local-datashare/fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp\nTheraphosidae,http://localhost:8080/#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu\n```\n\n### Tagging by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch tag documents directly in the index.\n\nTo see an example of input file, refer to [this JSON](tests/fixtures/tags-by-content-type.json).\n\n```\nUsage: tarentula tagging-by-query [OPTIONS] JSON_PATH\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --throttle                INTEGER     Request throttling (in ms)\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --progressbar / --no-progressbar      Display a progressbar\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --help                                Show this message and exit\n```\n\n### Following your changes\n\nWhen running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.\n\nIt uses [mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf you see the following message :\n\n```\n$ graph_es\ngraph_realtime.py:32: UserWarning: Matplotlib is currently using agg, which is a non-GUI backend, so cannot show the figure\n```\n\nThen you have to install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.\n\nThe command has the options below:\n\n```\n$ graph_es --help\nUsage: graph_es [OPTIONS]\n\nOptions:\n  --query               TEXT        Give a JSON query to filter documents. It can be\n                                      a file with @path/to/file. Default to all.\n  --index               TEXT        Elasticsearch index (default local-datashare)\n  --refresh-interval    INTEGER     Graph refresh interval in seconds (default 5s)\n  --field               TEXT        Field value to display over time (default "hits.total")\n  --elasticsearch-url   TEXT        Elasticsearch URL which is used to perform\n                                      update by query (default http://elasticsearch:9200)\n```\n\n## Configuration File\n\nTarentula supports several sources for configuring its behavior, including an ini files and command-line options.\n\nConfiguration file will be searched for in the following order (use the first file found, all others are ignored):\n\n  * `TARENTULA_CONFIG` (environment variable if set)\n  * `tarentula.ini` (in the current directory)\n  * `~/.tarentula.ini` (in the home directory)\n  * `/etc/tarentula/tarentula.ini`\n\nIt should follow the following format (all values bellow are optional):\n\n```\n[DEFAULT]\napikey = SECRETHALONOPROCTIDAE\ndatashare_url = http://here:8080\ndatashare_project = local-datashare\n\n[logger]\nsyslog_address = 127.0.0.0\nsyslog_port = 514\nsyslog_facility = local7\nstdout_loglevel = INFO\n```\n\n## Testing\n\nTo test this tool, you must have Datashare and Elasticsearch running on your development machine.\n\nAfter you [installed Datashare](https://datashare.icij.org/), just run it with a test project/user:\n\n```\ndatashare -p test-datashare -u test\n```\n\nIn a separate terminal, install the development dependencies:\n\n```\nmake install\n```\n\nFinally, run the test\n\n```\nmake test\n```\n\n\n## Releasing\n\nThe releasing process uses [bumpversion](https://pypi.org/project/bumpversion/) to manage versions of this package, [pypi](https://pypi.org/project/tarentula/) to publish the Python package and [Docker Hub](https://hub.docker.com/) for the Docker image.\n\n### 1. Create a new release\n\n```\nmake [patch|minor|major]\n```\n\n### 2. Upload distributions on pypi\n\n_To be able to do this, you will need to be a maintainer of the [pypi](https://pypi.org/project/tarentula/) project._\n\n```\nmake distribute\n```\n\n### 3. Build and publish the Docker image\n\nTo build and upload a new image on the [docker repository](https://hub.docker.com/repository/docker/icij/datashare-tarentula) :\n\n_To be able to do this, you will need to be part of the ICIJ organization on docker_\n\n```\nmake docker-publish\n```\n\n### 4. Push your changes on Github\n\nGit push release and tag :\n\n```\ngit push origin master --tags\n```\n',
+    'long_description': '# Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula)\n\nCli toolbelt for [Datashare](https://datashare.icij.org).\n\n```\n     /      \\\n  \\  \\  ,,  /  /\n   \'-.`\\()/`.-\'\n  .--_\'(  )\'_--.\n / /` /`""`\\ `\\ \\\n  |  |  ><  |  |\n  \\  \\      /  /\n      \'.__.\'\n\nUsage: tarentula [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --syslog-address      TEXT    localhost   Syslog address\n  --syslog-port         INTEGER 514         Syslog port\n  --syslog-facility     TEXT    local7      Syslog facility\n  --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler\n  --help                                    Show this message and exit\n  --version                                 Show the installed version of Tarentula\n\nCommands:\n  aggregate\n  count\n  clean-tags-by-query\n  download\n  export-by-query\n  list-metadata\n  tagging\n  tagging-by-query\n```\n\n---\n<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->\n\n- [Installation](#installation)\n- [Usage](#usage)\n  - [Cookbook 👩\u200d🍳](#cookbook-)\n  - [Count](#count)\n  - [Clean Tags by Query](#clean-tags-by-query)\n  - [Download](#download)\n  - [Export by Query](#export-by-query)\n  - [Tagging](#tagging)\n    - [CSV formats](#csv-formats)\n  - [Tagging by Query](#tagging-by-query)\n  - [Aggregate](#aggregate)\n  - [Following your changes](#following-your-changes)\n- [Configuration File](#configuration-file)\n- [Testing](#testing)\n- [Releasing](#releasing)\n  - [1. Create a new release](#1-create-a-new-release)\n  - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)\n  - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)\n  - [4. Push your changes on Github](#4-push-your-changes-on-github)\n\n<!-- /TOC -->\n---\n\n## Installation\n\nYou can insatll Datashare Tarentula with your favorite package manager:\n\n```\npip3 install --user tarentula\n```\n\nOr alternativly with Docker:\n\n```\ndocker run icij/datashare-tarentula\n```\n\n## Usage\n\nDatashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.\n\n### Cookbook 👩\u200d🍳\n\nTo learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.\n\n### Count\n\nA command to just count the number of files matching a query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n  --datashare-url           TEXT        Datashare URL\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        You can additionally pass the Elasticsearch\n                                          URL in order to use scrollingcapabilities of\n                                          Elasticsearch (useful when dealing with a\n                                          lot of results)\n  --query                   TEXT        The query string to filter documents\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n                                          in the downloaded document from the index\n  --traceback / --no-traceback          Display a traceback in case of error\n  --type [Document|NamedEntity]         Type of indexed documents to download\n  --help                                Show this message and exit\n```\n\n### Clean Tags by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch untag documents directly in the index.\n\n```\nUsage: tarentula clean-tags-by-query [OPTIONS]\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --query                   TEXT        Give a JSON query to filter documents that\n                                          will have their tags cleaned. It can be\n                                          afile with @path/to/file. Default to all.\n  --help                                Show this message and exit\n```\n\n### Download\n\nA command to download all files matching a query.\n\n```\nUsage: tarentula download [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --destination-directory TEXT    Directory documents will be downloaded\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --path-format TEXT              Downloaded document path template\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the downloaded document from the index\n\n  -f, --from INTEGER              Passed to the search it will bypass the\n                                  first n documents\n  -l, --limit INTEGER             Limit the total results to return\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --once / --not-once             Download file only once\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --raw-file / --no-raw-file      Download raw file from Datashare\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --help                          Show this message and exit.\n```\n\n\n### Export by Query\n\nA command to export all files matching a query.\n\n```\nUsage: tarentula export-by-query [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n\n  --query TEXT                    The query string to filter documents\n  --output-file TEXT              Path to the CSV file\n  --throttle INTEGER              Request throttling (in ms)\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n\n  --scroll TEXT                   Scroll duration\n  --source TEXT                   A comma-separated list of field to include\n                                  in the export\n\n  --sort-by TEXT                  Field to use to sort results\n  --order-by [asc|desc]           Order to use to sort results\n  --traceback / --no-traceback    Display a traceback in case of error\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  -f, --from INTEGER              Passed to the search it will bypass the\n                                  first n documents\n  -l, --limit INTEGER             Limit the total results to return\n  --size INTEGER                  Size of the scroll request that powers the\n                                  operation.\n\n  --query-field / --no-query-field\n                                  Add the query to the export CSV\n  --help                          Show this message and exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents with a CSV file.\n\n```\nUsage: tarentula tagging [OPTIONS] CSV_PATH\n\nOptions:\n  --datashare-url       TEXT        http://localhost:8080   Datashare URL\n  --datashare-project   TEXT        local-datashare         Datashare project\n  --throttle            INTEGER     0                       Request throttling (in ms)\n  --cookies             TEXT        _Empty string_          Key/value pair to add a cookie to each request to the API. You can separate semicolons: key1=val1;key2=val2;...\n  --apikey              TEXT        None                    Datashare authentication apikey\n  --traceback / --no-traceback                              Display a traceback in case of error\n  --progressbar / --no-progressbar                          Display a progressbar\n  --help                                                    Show this message and exit\n```\n\n#### CSV formats\n\nTagging with a `documentId` and `routing`:\n\n```csv\ntag,documentId,routing\nActinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG\nAntrodiaetidae,DWLOskax28jPQ2CjFrCo\nAtracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN\nAtypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\nBarychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\n```\n\nTagging with a `documentUrl`:\n\n```csv\ntag,documentUrl\nMecicobothriidae,http://localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi\nMicrostigmatidae,http://localhost:8080/#/d/local-datashare/iuL6GUBpO7nKyfSSFaS0/iuL6GUBpO7nKyfSSFaS0\nMigidae,http://localhost:8080/#/d/local-datashare/BmovvXBisWtyyx6o9cuG/BmovvXBisWtyyx6o9cuG\nNemesiidae,http://localhost:8080/#/d/local-datashare/vZJQpKQYhcI577gJR0aN/vZJQpKQYhcI577gJR0aN\nParatropididae,http://localhost:8080/#/d/local-datashare/vYl1C4bsWphUKvXEBDhM/vYl1C4bsWphUKvXEBDhM\nPorrhothelidae,http://localhost:8080/#/d/local-datashare/fgCt6JLfHSl160fnsjRp/fgCt6JLfHSl160fnsjRp\nTheraphosidae,http://localhost:8080/#/d/local-datashare/WvwVvNjEDQJXkwHISQIu/WvwVvNjEDQJXkwHISQIu\n```\n\n### Tagging by Query\n\nA command that uses Elasticsearch `update-by-query` feature to batch tag documents directly in the index.\n\nTo see an example of input file, refer to [this JSON](tests/fixtures/tags-by-content-type.json).\n\n```\nUsage: tarentula tagging-by-query [OPTIONS] JSON_PATH\n\nOptions:\n  --datashare-project       TEXT        Datashare project\n  --elasticsearch-url       TEXT        Elasticsearch URL which is used to perform\n                                          update by query\n  --throttle                INTEGER     Request throttling (in ms)\n  --cookies                 TEXT        Key/value pair to add a cookie to each\n                                          request to the API. You can\n                                          separatesemicolons: key1=val1;key2=val2;...\n  --apikey                  TEXT        Datashare authentication apikey\n  --traceback / --no-traceback          Display a traceback in case of error\n  --progressbar / --no-progressbar      Display a progressbar\n  --wait-for-completion / --no-wait-for-completion\n                                        Create a Elasticsearch task to perform the\n                                          updateasynchronously\n  --help                                Show this message and exit\n```\n\n\n### List Metadata\n\nYou can list the metadata from the mapping, optionally counting the number of occurrences of each field in the index, with the `--count` parameter. Counting the fields is disabled by default.\n\nIt includes a `--filter_by` parameter to narrow retrieving metadata properties of specific sets of documents. For instance it can be used to get just emails related properties with: `--filter_by "contentType=message/rfc822"`\n\n```\n$ tarentula list-metadata --help\nUsage: tarentula list-metadata [OPTIONS]\n\nOptions:\n  --datashare-project TEXT       Datashare project\n  --elasticsearch-url TEXT       You can additionally pass the Elasticsearch\n                                 URL in order to use scrollingcapabilities of\n                                 Elasticsearch (useful when dealing with a lot\n                                 of results)\n  --type [Document|NamedEntity]  Type of indexed documents to get metadata\n  --filter_by TEXT               Filter documents by pairs concatenated by\n                                 coma of field names and values separated by\n                                 =.Example "contentType=message/rfc822,content\n                                 Type=message/rfc822"\n  --count / --no-count           Count or not the number of docs for each\n                                 property found\n\n  --help                         Show this message and exit.\n\n```\n\n### Aggregate\n\nYou can run aggregations on the data, the ElasticSearch aggregations API is partially enabled with this command.\nThe possibilities are:\n\n- count: grouping by a given field different values, and count the num of docs.\n- nunique: returns the number of unique values of a given field.\n- date_histogram: returns counting of monthly or yearly grouped values for a given date field.\n- sum: returns the sum of values of number type fields.\n- min: returns the min of values of number type fields.\n- max: returns the max of values of number type fields.\n- avg: returns the average of values of number type fields.\n- stats: returns a bunch of statistics for a given number type fields.\n- string_stats: returns a bunch of string statistics for a given string type fields.\n\n\n\n```\n$ tarentula aggregate --help\nUsage: tarentula aggregate [OPTIONS]\n\nOptions:\n  --apikey TEXT                   Datashare authentication apikey\n  --datashare-url TEXT            Datashare URL\n  --datashare-project TEXT        Datashare project\n  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch\n                                  URL in order to use scrollingcapabilities of\n                                  Elasticsearch (useful when dealing with a\n                                  lot of results)\n  --query TEXT                    The query string to filter documents\n  --cookies TEXT                  Key/value pair to add a cookie to each\n                                  request to the API. You can\n                                  separatesemicolons: key1=val1;key2=val2;...\n  --traceback / --no-traceback    Display a traceback in case of error\n  --type [Document|NamedEntity]   Type of indexed documents to download\n  --group_by TEXT                 Field to use to aggregate results\n  --operation_field TEXT          Field to run the operation on\n  --run [count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]\n                                  Operation to run\n  --calendar_interval [year|month]\n                                  Calendar interval for date histogram\n                                  aggregation\n  --help                          Show this message and exit.\n```\n\n### Following your changes\n\nWhen running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.\n\nIt uses [mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf you see the following message :\n\n```\n$ graph_es\ngraph_realtime.py:32: UserWarning: Matplotlib is currently using agg, which is a non-GUI backend, so cannot show the figure\n```\n\nThen you have to install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.\n\nThe command has the options below:\n\n```\n$ graph_es --help\nUsage: graph_es [OPTIONS]\n\nOptions:\n  --query               TEXT        Give a JSON query to filter documents. It can be\n                                      a file with @path/to/file. Default to all.\n  --index               TEXT        Elasticsearch index (default local-datashare)\n  --refresh-interval    INTEGER     Graph refresh interval in seconds (default 5s)\n  --field               TEXT        Field value to display over time (default "hits.total")\n  --elasticsearch-url   TEXT        Elasticsearch URL which is used to perform\n                                      update by query (default http://elasticsearch:9200)\n```\n\n## Configuration File\n\nTarentula supports several sources for configuring its behavior, including an ini files and command-line options.\n\nConfiguration file will be searched for in the following order (use the first file found, all others are ignored):\n\n  * `TARENTULA_CONFIG` (environment variable if set)\n  * `tarentula.ini` (in the current directory)\n  * `~/.tarentula.ini` (in the home directory)\n  * `/etc/tarentula/tarentula.ini`\n\nIt should follow the following format (all values bellow are optional):\n\n```\n[DEFAULT]\napikey = SECRETHALONOPROCTIDAE\ndatashare_url = http://here:8080\ndatashare_project = local-datashare\n\n[logger]\nsyslog_address = 127.0.0.0\nsyslog_port = 514\nsyslog_facility = local7\nstdout_loglevel = INFO\n```\n\n## Testing\n\nTo test this tool, you must have Datashare and Elasticsearch running on your development machine.\n\nAfter you [installed Datashare](https://datashare.icij.org/), just run it with a test project/user:\n\n```\ndatashare -p test-datashare -u test\n```\n\nIn a separate terminal, install the development dependencies:\n\n```\nmake install\n```\n\nFinally, run the test\n\n```\nmake test\n```\n\n\n## Releasing\n\nThe releasing process uses [bumpversion](https://pypi.org/project/bumpversion/) to manage versions of this package, [pypi](https://pypi.org/project/tarentula/) to publish the Python package and [Docker Hub](https://hub.docker.com/) for the Docker image.\n\n### 1. Create a new release\n\n```\nmake [patch|minor|major]\n```\n\n### 2. Upload distributions on pypi\n\n_To be able to do this, you will need to be a maintainer of the [pypi](https://pypi.org/project/tarentula/) project._\n\n```\nmake distribute\n```\n\n### 3. Build and publish the Docker image\n\nTo build and upload a new image on the [docker repository](https://hub.docker.com/repository/docker/icij/datashare-tarentula) :\n\n_To be able to do this, you will need to be part of the ICIJ organization on docker_\n\n```\nmake docker-publish\n```\n\n**Note**: Datashare Tarentula is a multi-platform build. You might need to setup your environment for \nmulti-platform using the `make docker-setup-multiarch` command. Read more \n[on Docker documentation](https://docs.docker.com/build/building/multi-platform/). \n\n### 4. Push your changes on Github\n\nGit push release and tag :\n\n```\ngit push origin master --tags\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,40 +1,44 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['tarentula']
 package_data = \ {'': ['*']} install_requires = \ ['click>=8.1,<9.0',
 'coloredlogs==14.0', 'requests>=2.28,<3.0', 'rich>=12,<13'] entry_points = \
 {'console_scripts': ['tarentula = tarentula.cli:cli']} setup_kwargs = { 'name':
-'tarentula', 'version': '4.3.3', 'description': '', 'long_description': '#
+'tarentula', 'version': '4.3.4', 'description': '', 'long_description': '#
 Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-
 tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-
 tarentula)\n\nCli toolbelt for [Datashare](https://
 datashare.icij.org).\n\n```\n / \\\n \\ \\ ,, / /\n \'-.`\\()/`.-\'\n .--_\'
 ( )\'_--.\n / /` /`""`\\ `\\ \\\n | | >< | |\n \\ \\ / /\n \'.__.\'\n\nUsage:
 tarentula [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n --syslog-address TEXT
 localhost Syslog address\n --syslog-port INTEGER 514 Syslog port\n --syslog-
 facility TEXT local7 Syslog facility\n --stdout-loglevel TEXT ERROR Change the
 default log level for stdout error handler\n --help Show this message and
-exit\n --version Show the installed version of Tarentula\n\nCommands:\n count\n
-clean-tags-by-query\n download\n export-by-query\n tagging\n tagging-by-
-query\n```\n\n---\n\n\n- [Usage](#usage)\n - [Cookbook ð©\u200dð³]
-(#cookbook-)\n - [Count](#count)\n - [Clean Tags by Query](#clean-tags-by-
-query)\n - [Download](#download)\n - [Export by Query](#export-by-query)\n -
-[Tagging](#tagging)\n - [CSV formats](#csv-formats)\n - [Tagging by Query]
-(#tagging-by-query)\n - [Following your changes](#following-your-changes)\n-
-[Configuration File](#configuration-file)\n- [Testing](#testing)\n- [Releasing]
-(#releasing)\n - [1. Create a new release](#1-create-a-new-release)\n - [2.
-Upload distributions on pypi](#2-upload-distributions-on-pypi)\n - [3. Build
-and publish the Docker image](#3-build-and-publish-the-docker-image)\n - [4.
-Push your changes on Github](#4-push-your-changes-on-github)\n\n\n---\n\n##
-Usage\n\nDatashare Tarentula comes with basic commands to interact with a
-Datashare instance (running locally or on a remote server). Primarily focus on
-bulk actions, it provides you with both a cli interface and a python
-API.\n\n### Cookbook ð©\u200dð³\n\nTo learn more about how to use Datashare
-Tarentula with a list of examples, please refer to the_Cookbook.\n\n###
-Count\n\nA command to just count the number of files matching a
-query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n --datashare-url
+exit\n --version Show the installed version of Tarentula\n\nCommands:\n
+aggregate\n count\n clean-tags-by-query\n download\n export-by-query\n list-
+metadata\n tagging\n tagging-by-query\n```\n\n---\n\n\n- [Installation]
+(#installation)\n- [Usage](#usage)\n - [Cookbook ð©\u200dð³](#cookbook-)\n
+- [Count](#count)\n - [Clean Tags by Query](#clean-tags-by-query)\n -
+[Download](#download)\n - [Export by Query](#export-by-query)\n - [Tagging]
+(#tagging)\n - [CSV formats](#csv-formats)\n - [Tagging by Query](#tagging-by-
+query)\n - [Aggregate](#aggregate)\n - [Following your changes](#following-
+your-changes)\n- [Configuration File](#configuration-file)\n- [Testing]
+(#testing)\n- [Releasing](#releasing)\n - [1. Create a new release](#1-create-
+a-new-release)\n - [2. Upload distributions on pypi](#2-upload-distributions-
+on-pypi)\n - [3. Build and publish the Docker image](#3-build-and-publish-the-
+docker-image)\n - [4. Push your changes on Github](#4-push-your-changes-on-
+github)\n\n\n---\n\n## Installation\n\nYou can insatll Datashare Tarentula with
+your favorite package manager:\n\n```\npip3 install --user tarentula\n```\n\nOr
+alternativly with Docker:\n\n```\ndocker run icij/datashare-
+tarentula\n```\n\n## Usage\n\nDatashare Tarentula comes with basic commands to
+interact with a Datashare instance (running locally or on a remote server).
+Primarily focus on bulk actions, it provides you with both a cli interface and
+a python API.\n\n### Cookbook ð©\u200dð³\n\nTo learn more about how to use
+Datashare Tarentula with a list of examples, please refer to the
+Cookbook.\n\n### Count\n\nA command to just count the number of files matching
+a query.\n\n```\nUsage: tarentula count [OPTIONS]\n\nOptions:\n --datashare-url
 TEXT Datashare URL\n --datashare-project TEXT Datashare project\n --
 elasticsearch-url TEXT You can additionally pass the Elasticsearch\n URL in
 order to use scrollingcapabilities of\n Elasticsearch (useful when dealing with
 a\n lot of results)\n --query TEXT The query string to filter documents\n --
 cookies TEXT Key/value pair to add a cookie to each\n request to the API. You
 can\n separatesemicolons: key1=val1;key2=val2;...\n --apikey TEXT Datashare
 authentication apikey\n in the downloaded document from the index\n --traceback
@@ -60,43 +64,47 @@
 of\n Elasticsearch (useful when dealing with a\n lot of results)\n\n --query
 TEXT The query string to filter documents\n --destination-directory TEXT
 Directory documents will be downloaded\n --throttle INTEGER Request throttling
 (in ms)\n --cookies TEXT Key/value pair to add a cookie to each\n request to
 the API. You can\n separatesemicolons: key1=val1;key2=val2;...\n\n --path-
 format TEXT Downloaded document path template\n --scroll TEXT Scroll duration\n
 --source TEXT A comma-separated list of field to include\n in the downloaded
-document from the index\n\n --sort-by TEXT Field to use to sort results\n --
-order-by [asc|desc] Order to use to sort results\n --once / --not-once Download
-file only once\n --traceback / --no-traceback Display a traceback in case of
-error\n --progressbar / --no-progressbar\n Display a progressbar\n --raw-file /
---no-raw-file Download raw file from Datashare\n --type [Document|NamedEntity]
-Type of indexed documents to download\n --help Show this message and
+document from the index\n\n -f, --from INTEGER Passed to the search it will
+bypass the\n first n documents\n -l, --limit INTEGER Limit the total results to
+return\n --sort-by TEXT Field to use to sort results\n --order-by [asc|desc]
+Order to use to sort results\n --once / --not-once Download file only once\n --
+traceback / --no-traceback Display a traceback in case of error\n --progressbar
+/ --no-progressbar\n Display a progressbar\n --raw-file / --no-raw-file
+Download raw file from Datashare\n --type [Document|NamedEntity] Type of
+indexed documents to download\n --help Show this message and
 exit.\n```\n\n\n### Export by Query\n\nA command to export all files matching a
 query.\n\n```\nUsage: tarentula export-by-query [OPTIONS]\n\nOptions:\n --
 apikey TEXT Datashare authentication apikey\n --datashare-url TEXT Datashare
 URL\n --datashare-project TEXT Datashare project\n --elasticsearch-url TEXT You
 can additionally pass the Elasticsearch\n URL in order to use
 scrollingcapabilities of\n Elasticsearch (useful when dealing with a\n lot of
 results)\n\n --query TEXT The query string to filter documents\n --output-file
 TEXT Path to the CSV file\n --throttle INTEGER Request throttling (in ms)\n --
 cookies TEXT Key/value pair to add a cookie to each\n request to the API. You
 can\n separatesemicolons: key1=val1;key2=val2;...\n\n --scroll TEXT Scroll
 duration\n --source TEXT A comma-separated list of field to include\n in the
 export\n\n --sort-by TEXT Field to use to sort results\n --order-by [asc|desc]
 Order to use to sort results\n --traceback / --no-traceback Display a traceback
 in case of error\n --progressbar / --no-progressbar\n Display a progressbar\n -
--type [Document|NamedEntity] Type of indexed documents to download\n --size
-INTEGER Size of the scroll request that powers the\n operation.\n\n --query-
-field / --no-query-field\n Add the query to the export CSV\n --help Show this
-message and exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents
-with a CSV file.\n\n```\nUsage: tarentula tagging [OPTIONS]
-CSV_PATH\n\nOptions:\n --datashare-url TEXT http://localhost:8080 Datashare
-URL\n --datashare-project TEXT local-datashare Datashare project\n --throttle
-INTEGER 0 Request throttling (in ms)\n --cookies TEXT _Empty string_ Key/value
-pair to add a cookie to each request to the API. You can separate semicolons:
+-type [Document|NamedEntity] Type of indexed documents to download\n -f, --from
+INTEGER Passed to the search it will bypass the\n first n documents\n -l, --
+limit INTEGER Limit the total results to return\n --size INTEGER Size of the
+scroll request that powers the\n operation.\n\n --query-field / --no-query-
+field\n Add the query to the export CSV\n --help Show this message and
+exit.\n```\n\n\n### Tagging\n\nA command to batch tag documents with a CSV
+file.\n\n```\nUsage: tarentula tagging [OPTIONS] CSV_PATH\n\nOptions:\n --
+datashare-url TEXT http://localhost:8080 Datashare URL\n --datashare-project
+TEXT local-datashare Datashare project\n --throttle INTEGER 0 Request
+throttling (in ms)\n --cookies TEXT _Empty string_ Key/value pair to add a
+cookie to each request to the API. You can separate semicolons:
 key1=val1;key2=val2;...\n --apikey TEXT None Datashare authentication apikey\n
 --traceback / --no-traceback Display a traceback in case of error\n --
 progressbar / --no-progressbar Display a progressbar\n --help Show this message
 and exit\n```\n\n#### CSV formats\n\nTagging with a `documentId` and `routing`:
 \n\n```csv\ntag,documentId,routing\nActinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG\nAntrodiaetidae,DWLOskax28jPQ2CjFrCo\nAtracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN\nAtypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\nBarychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi\n```\n\nTagging
 with a `documentUrl`:\n\n```csv\ntag,documentUrl\nMecicobothriidae,http://
 localhost:8080/#/d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/
@@ -118,27 +126,67 @@
 query\n --throttle INTEGER Request throttling (in ms)\n --cookies TEXT Key/
 value pair to add a cookie to each\n request to the API. You can\n
 separatesemicolons: key1=val1;key2=val2;...\n --apikey TEXT Datashare
 authentication apikey\n --traceback / --no-traceback Display a traceback in
 case of error\n --progressbar / --no-progressbar Display a progressbar\n --
 wait-for-completion / --no-wait-for-completion\n Create a Elasticsearch task to
 perform the\n updateasynchronously\n --help Show this message and
-exit\n```\n\n### Following your changes\n\nWhen running Elasticsearch changes
-on big datasets, it could take a very long time. As we were curling ES to see
-if the task was still running well, we added a small utility to follow the
-changes. It makes a live graph of a provided ES indicator with a specified
-filter.\n\nIt uses [mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf
-you see the following message :\n\n```\n$ graph_es\ngraph_realtime.py:32:
-UserWarning: Matplotlib is currently using agg, which is a non-GUI backend, so
-cannot show the figure\n```\n\nThen you have to install [tkinter](https://
-docs.python.org/3/library/tkinter.html), i.e. python3-tk for Debian/
-Ubuntu.\n\nThe command has the options below:\n\n```\n$ graph_es --help\nUsage:
-graph_es [OPTIONS]\n\nOptions:\n --query TEXT Give a JSON query to filter
-documents. It can be\n a file with @path/to/file. Default to all.\n --index
-TEXT Elasticsearch index (default local-datashare)\n --refresh-interval INTEGER
+exit\n```\n\n\n### List Metadata\n\nYou can list the metadata from the mapping,
+optionally counting the number of occurrences of each field in the index, with
+the `--count` parameter. Counting the fields is disabled by default.\n\nIt
+includes a `--filter_by` parameter to narrow retrieving metadata properties of
+specific sets of documents. For instance it can be used to get just emails
+related properties with: `--filter_by "contentType=message/rfc822"`\n\n```\n$
+tarentula list-metadata --help\nUsage: tarentula list-metadata
+[OPTIONS]\n\nOptions:\n --datashare-project TEXT Datashare project\n --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch\n URL in
+order to use scrollingcapabilities of\n Elasticsearch (useful when dealing with
+a lot\n of results)\n --type [Document|NamedEntity] Type of indexed documents
+to get metadata\n --filter_by TEXT Filter documents by pairs concatenated by\n
+coma of field names and values separated by\n =.Example "contentType=message/
+rfc822,content\n Type=message/rfc822"\n --count / --no-count Count or not the
+number of docs for each\n property found\n\n --help Show this message and
+exit.\n\n```\n\n### Aggregate\n\nYou can run aggregations on the data, the
+ElasticSearch aggregations API is partially enabled with this command.\nThe
+possibilities are:\n\n- count: grouping by a given field different values, and
+count the num of docs.\n- nunique: returns the number of unique values of a
+given field.\n- date_histogram: returns counting of monthly or yearly grouped
+values for a given date field.\n- sum: returns the sum of values of number type
+fields.\n- min: returns the min of values of number type fields.\n- max:
+returns the max of values of number type fields.\n- avg: returns the average of
+values of number type fields.\n- stats: returns a bunch of statistics for a
+given number type fields.\n- string_stats: returns a bunch of string statistics
+for a given string type fields.\n\n\n\n```\n$ tarentula aggregate --
+help\nUsage: tarentula aggregate [OPTIONS]\n\nOptions:\n --apikey TEXT
+Datashare authentication apikey\n --datashare-url TEXT Datashare URL\n --
+datashare-project TEXT Datashare project\n --elasticsearch-url TEXT You can
+additionally pass the Elasticsearch\n URL in order to use scrollingcapabilities
+of\n Elasticsearch (useful when dealing with a\n lot of results)\n --query TEXT
+The query string to filter documents\n --cookies TEXT Key/value pair to add a
+cookie to each\n request to the API. You can\n separatesemicolons:
+key1=val1;key2=val2;...\n --traceback / --no-traceback Display a traceback in
+case of error\n --type [Document|NamedEntity] Type of indexed documents to
+download\n --group_by TEXT Field to use to aggregate results\n --
+operation_field TEXT Field to run the operation on\n --run
+[count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]\n Operation
+to run\n --calendar_interval [year|month]\n Calendar interval for date
+histogram\n aggregation\n --help Show this message and exit.\n```\n\n###
+Following your changes\n\nWhen running Elasticsearch changes on big datasets,
+it could take a very long time. As we were curling ES to see if the task was
+still running well, we added a small utility to follow the changes. It makes a
+live graph of a provided ES indicator with a specified filter.\n\nIt uses
+[mathplotlib](https://matplotlib.org/) and python3-tk.\n\nIf you see the
+following message :\n\n```\n$ graph_es\ngraph_realtime.py:32: UserWarning:
+Matplotlib is currently using agg, which is a non-GUI backend, so cannot show
+the figure\n```\n\nThen you have to install [tkinter](https://docs.python.org/
+3/library/tkinter.html), i.e. python3-tk for Debian/Ubuntu.\n\nThe command has
+the options below:\n\n```\n$ graph_es --help\nUsage: graph_es
+[OPTIONS]\n\nOptions:\n --query TEXT Give a JSON query to filter documents. It
+can be\n a file with @path/to/file. Default to all.\n --index TEXT
+Elasticsearch index (default local-datashare)\n --refresh-interval INTEGER
 Graph refresh interval in seconds (default 5s)\n --field TEXT Field value to
 display over time (default "hits.total")\n --elasticsearch-url TEXT
 Elasticsearch URL which is used to perform\n update by query (default http://
 elasticsearch:9200)\n```\n\n## Configuration File\n\nTarentula supports several
 sources for configuring its behavior, including an ini files and command-line
 options.\n\nConfiguration file will be searched for in the following order (use
 the first file found, all others are ignored):\n\n * `TARENTULA_CONFIG`
@@ -161,14 +209,17 @@
 release\n\n```\nmake [patch|minor|major]\n```\n\n### 2. Upload distributions on
 pypi\n\n_To be able to do this, you will need to be a maintainer of the [pypi]
 (https://pypi.org/project/tarentula/) project._\n\n```\nmake
 distribute\n```\n\n### 3. Build and publish the Docker image\n\nTo build and
 upload a new image on the [docker repository](https://hub.docker.com/
 repository/docker/icij/datashare-tarentula) :\n\n_To be able to do this, you
 will need to be part of the ICIJ organization on docker_\n\n```\nmake docker-
-publish\n```\n\n### 4. Push your changes on Github\n\nGit push release and tag
-:\n\n```\ngit push origin master --tags\n```\n', 'author': 'ICIJ',
-'author_email': 'engineering@icij.org', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
+publish\n```\n\n**Note**: Datashare Tarentula is a multi-platform build. You
+might need to setup your environment for \nmulti-platform using the `make
+docker-setup-multiarch` command. Read more \n[on Docker documentation](https://
+docs.docker.com/build/building/multi-platform/). \n\n### 4. Push your changes
+on Github\n\nGit push release and tag :\n\n```\ngit push origin master --
+tags\n```\n', 'author': 'ICIJ', 'author_email': 'engineering@icij.org',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
 'entry_points': entry_points, 'python_requires': '>=3.8,<3.11', } setup
 (**setup_kwargs)
```

### Comparing `tarentula-4.3.3/PKG-INFO` & `tarentula-4.3.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarentula
-Version: 4.3.3
+Version: 4.3.4
 Summary: 
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,46 +36,64 @@
   --syslog-port         INTEGER 514         Syslog port
   --syslog-facility     TEXT    local7      Syslog facility
   --stdout-loglevel     TEXT    ERROR       Change the default log level for stdout error handler
   --help                                    Show this message and exit
   --version                                 Show the installed version of Tarentula
 
 Commands:
+  aggregate
   count
   clean-tags-by-query
   download
   export-by-query
+  list-metadata
   tagging
   tagging-by-query
 ```
 
 ---
 <!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->
 
+- [Installation](#installation)
 - [Usage](#usage)
   - [Cookbook 👩‍🍳](#cookbook-)
   - [Count](#count)
   - [Clean Tags by Query](#clean-tags-by-query)
   - [Download](#download)
   - [Export by Query](#export-by-query)
   - [Tagging](#tagging)
     - [CSV formats](#csv-formats)
   - [Tagging by Query](#tagging-by-query)
+  - [Aggregate](#aggregate)
   - [Following your changes](#following-your-changes)
 - [Configuration File](#configuration-file)
 - [Testing](#testing)
 - [Releasing](#releasing)
   - [1. Create a new release](#1-create-a-new-release)
   - [2. Upload distributions on pypi](#2-upload-distributions-on-pypi)
   - [3. Build and publish the Docker image](#3-build-and-publish-the-docker-image)
   - [4. Push your changes on Github](#4-push-your-changes-on-github)
 
 <!-- /TOC -->
 ---
 
+## Installation
+
+You can insatll Datashare Tarentula with your favorite package manager:
+
+```
+pip3 install --user tarentula
+```
+
+Or alternativly with Docker:
+
+```
+docker run icij/datashare-tarentula
+```
+
 ## Usage
 
 Datashare Tarentula comes with basic commands to interact with a Datashare instance (running locally or on a remote server). Primarily focus on bulk actions, it provides you with both a cli interface and a python API.
 
 ### Cookbook 👩‍🍳
 
 To learn more about how to use Datashare Tarentula with a list of examples, please refer to <a href="./COOKBOOK.md">the Cookbook</a>.
@@ -154,14 +172,17 @@
                                   separatesemicolons: key1=val1;key2=val2;...
 
   --path-format TEXT              Downloaded document path template
   --scroll TEXT                   Scroll duration
   --source TEXT                   A comma-separated list of field to include
                                   in the downloaded document from the index
 
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
   --sort-by TEXT                  Field to use to sort results
   --order-by [asc|desc]           Order to use to sort results
   --once / --not-once             Download file only once
   --traceback / --no-traceback    Display a traceback in case of error
   --progressbar / --no-progressbar
                                   Display a progressbar
   --raw-file / --no-raw-file      Download raw file from Datashare
@@ -199,14 +220,17 @@
 
   --sort-by TEXT                  Field to use to sort results
   --order-by [asc|desc]           Order to use to sort results
   --traceback / --no-traceback    Display a traceback in case of error
   --progressbar / --no-progressbar
                                   Display a progressbar
   --type [Document|NamedEntity]   Type of indexed documents to download
+  -f, --from INTEGER              Passed to the search it will bypass the
+                                  first n documents
+  -l, --limit INTEGER             Limit the total results to return
   --size INTEGER                  Size of the scroll request that powers the
                                   operation.
 
   --query-field / --no-query-field
                                   Add the query to the export CSV
   --help                          Show this message and exit.
 ```
@@ -278,14 +302,88 @@
   --progressbar / --no-progressbar      Display a progressbar
   --wait-for-completion / --no-wait-for-completion
                                         Create a Elasticsearch task to perform the
                                           updateasynchronously
   --help                                Show this message and exit
 ```
 
+
+### List Metadata
+
+You can list the metadata from the mapping, optionally counting the number of occurrences of each field in the index, with the `--count` parameter. Counting the fields is disabled by default.
+
+It includes a `--filter_by` parameter to narrow retrieving metadata properties of specific sets of documents. For instance it can be used to get just emails related properties with: `--filter_by "contentType=message/rfc822"`
+
+```
+$ tarentula list-metadata --help
+Usage: tarentula list-metadata [OPTIONS]
+
+Options:
+  --datashare-project TEXT       Datashare project
+  --elasticsearch-url TEXT       You can additionally pass the Elasticsearch
+                                 URL in order to use scrollingcapabilities of
+                                 Elasticsearch (useful when dealing with a lot
+                                 of results)
+  --type [Document|NamedEntity]  Type of indexed documents to get metadata
+  --filter_by TEXT               Filter documents by pairs concatenated by
+                                 coma of field names and values separated by
+                                 =.Example "contentType=message/rfc822,content
+                                 Type=message/rfc822"
+  --count / --no-count           Count or not the number of docs for each
+                                 property found
+
+  --help                         Show this message and exit.
+
+```
+
+### Aggregate
+
+You can run aggregations on the data, the ElasticSearch aggregations API is partially enabled with this command.
+The possibilities are:
+
+- count: grouping by a given field different values, and count the num of docs.
+- nunique: returns the number of unique values of a given field.
+- date_histogram: returns counting of monthly or yearly grouped values for a given date field.
+- sum: returns the sum of values of number type fields.
+- min: returns the min of values of number type fields.
+- max: returns the max of values of number type fields.
+- avg: returns the average of values of number type fields.
+- stats: returns a bunch of statistics for a given number type fields.
+- string_stats: returns a bunch of string statistics for a given string type fields.
+
+
+
+```
+$ tarentula aggregate --help
+Usage: tarentula aggregate [OPTIONS]
+
+Options:
+  --apikey TEXT                   Datashare authentication apikey
+  --datashare-url TEXT            Datashare URL
+  --datashare-project TEXT        Datashare project
+  --elasticsearch-url TEXT        You can additionally pass the Elasticsearch
+                                  URL in order to use scrollingcapabilities of
+                                  Elasticsearch (useful when dealing with a
+                                  lot of results)
+  --query TEXT                    The query string to filter documents
+  --cookies TEXT                  Key/value pair to add a cookie to each
+                                  request to the API. You can
+                                  separatesemicolons: key1=val1;key2=val2;...
+  --traceback / --no-traceback    Display a traceback in case of error
+  --type [Document|NamedEntity]   Type of indexed documents to download
+  --group_by TEXT                 Field to use to aggregate results
+  --operation_field TEXT          Field to run the operation on
+  --run [count|nunique|date_histogram|sum|stats|string_stats|min|max|avg]
+                                  Operation to run
+  --calendar_interval [year|month]
+                                  Calendar interval for date histogram
+                                  aggregation
+  --help                          Show this message and exit.
+```
+
 ### Following your changes
 
 When running Elasticsearch changes on big datasets, it could take a very long time. As we were curling ES to see if the task was still running well, we added a small utility to follow the changes. It makes a live graph of a provided ES indicator with a specified filter.
 
 It uses [mathplotlib](https://matplotlib.org/) and python3-tk.
 
 If you see the following message :
@@ -386,14 +484,18 @@
 
 _To be able to do this, you will need to be part of the ICIJ organization on docker_
 
 ```
 make docker-publish
 ```
 
+**Note**: Datashare Tarentula is a multi-platform build. You might need to setup your environment for 
+multi-platform using the `make docker-setup-multiarch` command. Read more 
+[on Docker documentation](https://docs.docker.com/build/building/multi-platform/). 
+
 ### 4. Push your changes on Github
 
 Git push release and tag :
 
 ```
 git push origin master --tags
 ```
```

#### html2text {}

```diff
@@ -1,104 +1,110 @@
-Metadata-Version: 2.1 Name: tarentula Version: 4.3.3 Summary: Author: ICIJ
+Metadata-Version: 2.1 Name: tarentula Version: 4.3.4 Summary: Author: ICIJ
 Author-email: engineering@icij.org Requires-Python: >=3.8,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: coloredlogs (==14.0) Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: rich (>=12,<13) Description-Content-Type: text/markdown #
 Datashare Tarentula [![CircleCI](https://circleci.com/gh/ICIJ/datashare-
 tarentula.svg?style=svg)](https://circleci.com/gh/ICIJ/datashare-tarentula) Cli
 toolbelt for [Datashare](https://datashare.icij.org). ``` / \ \ \ ,, / / '-.`\
 ()/`.-' .--_'( )'_--. / /` /`""`\ `\ \ | | >< | | \ \ / / '.__.' Usage:
 tarentula [OPTIONS] COMMAND [ARGS]... Options: --syslog-address TEXT localhost
 Syslog address --syslog-port INTEGER 514 Syslog port --syslog-facility TEXT
 local7 Syslog facility --stdout-loglevel TEXT ERROR Change the default log
 level for stdout error handler --help Show this message and exit --version Show
-the installed version of Tarentula Commands: count clean-tags-by-query download
-export-by-query tagging tagging-by-query ``` ---  - [Usage](#usage) - [Cookbook
-ð©âð³](#cookbook-) - [Count](#count) - [Clean Tags by Query](#clean-tags-
-by-query) - [Download](#download) - [Export by Query](#export-by-query) -
-[Tagging](#tagging) - [CSV formats](#csv-formats) - [Tagging by Query]
-(#tagging-by-query) - [Following your changes](#following-your-changes) -
-[Configuration File](#configuration-file) - [Testing](#testing) - [Releasing]
-(#releasing) - [1. Create a new release](#1-create-a-new-release) - [2. Upload
-distributions on pypi](#2-upload-distributions-on-pypi) - [3. Build and publish
-the Docker image](#3-build-and-publish-the-docker-image) - [4. Push your
-changes on Github](#4-push-your-changes-on-github)  --- ## Usage Datashare
-Tarentula comes with basic commands to interact with a Datashare instance
-(running locally or on a remote server). Primarily focus on bulk actions, it
-provides you with both a cli interface and a python API. ### Cookbook
-ð©âð³ To learn more about how to use Datashare Tarentula with a list of
-examples, please refer to the_Cookbook. ### Count A command to just count the
-number of files matching a query. ``` Usage: tarentula count [OPTIONS] Options:
---datashare-url TEXT Datashare URL --datashare-project TEXT Datashare project -
--elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in
-order to use scrollingcapabilities of Elasticsearch (useful when dealing with a
-lot of results) --query TEXT The query string to filter documents --cookies
-TEXT Key/value pair to add a cookie to each request to the API. You can
-separatesemicolons: key1=val1;key2=val2;... --apikey TEXT Datashare
-authentication apikey in the downloaded document from the index --traceback / -
--no-traceback Display a traceback in case of error --type
-[Document|NamedEntity] Type of indexed documents to download --help Show this
-message and exit ``` ### Clean Tags by Query A command that uses Elasticsearch
-`update-by-query` feature to batch untag documents directly in the index. ```
-Usage: tarentula clean-tags-by-query [OPTIONS] Options: --datashare-project
-TEXT Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used
-to perform update by query --cookies TEXT Key/value pair to add a cookie to
-each request to the API. You can separatesemicolons: key1=val1;key2=val2;... --
-apikey TEXT Datashare authentication apikey --traceback / --no-traceback
-Display a traceback in case of error --wait-for-completion / --no-wait-for-
-completion Create a Elasticsearch task to perform the updateasynchronously --
-query TEXT Give a JSON query to filter documents that will have their tags
-cleaned. It can be afile with @path/to/file. Default to all. --help Show this
-message and exit ``` ### Download A command to download all files matching a
-query. ``` Usage: tarentula download [OPTIONS] Options: --apikey TEXT Datashare
-authentication apikey --datashare-url TEXT Datashare URL --datashare-project
-TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
-Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
-(useful when dealing with a lot of results) --query TEXT The query string to
-filter documents --destination-directory TEXT Directory documents will be
-downloaded --throttle INTEGER Request throttling (in ms) --cookies TEXT Key/
-value pair to add a cookie to each request to the API. You can
-separatesemicolons: key1=val1;key2=val2;... --path-format TEXT Downloaded
-document path template --scroll TEXT Scroll duration --source TEXT A comma-
-separated list of field to include in the downloaded document from the index --
-sort-by TEXT Field to use to sort results --order-by [asc|desc] Order to use to
-sort results --once / --not-once Download file only once --traceback / --no-
-traceback Display a traceback in case of error --progressbar / --no-progressbar
-Display a progressbar --raw-file / --no-raw-file Download raw file from
-Datashare --type [Document|NamedEntity] Type of indexed documents to download -
--help Show this message and exit. ``` ### Export by Query A command to export
-all files matching a query. ``` Usage: tarentula export-by-query [OPTIONS]
+the installed version of Tarentula Commands: aggregate count clean-tags-by-
+query download export-by-query list-metadata tagging tagging-by-query ``` --
+-  - [Installation](#installation) - [Usage](#usage) - [Cookbook ð©âð³]
+(#cookbook-) - [Count](#count) - [Clean Tags by Query](#clean-tags-by-query) -
+[Download](#download) - [Export by Query](#export-by-query) - [Tagging]
+(#tagging) - [CSV formats](#csv-formats) - [Tagging by Query](#tagging-by-
+query) - [Aggregate](#aggregate) - [Following your changes](#following-your-
+changes) - [Configuration File](#configuration-file) - [Testing](#testing) -
+[Releasing](#releasing) - [1. Create a new release](#1-create-a-new-release) -
+[2. Upload distributions on pypi](#2-upload-distributions-on-pypi) - [3. Build
+and publish the Docker image](#3-build-and-publish-the-docker-image) - [4. Push
+your changes on Github](#4-push-your-changes-on-github)  --- ## Installation
+You can insatll Datashare Tarentula with your favorite package manager: ```
+pip3 install --user tarentula ``` Or alternativly with Docker: ``` docker run
+icij/datashare-tarentula ``` ## Usage Datashare Tarentula comes with basic
+commands to interact with a Datashare instance (running locally or on a remote
+server). Primarily focus on bulk actions, it provides you with both a cli
+interface and a python API. ### Cookbook ð©âð³ To learn more about how to
+use Datashare Tarentula with a list of examples, please refer to the_Cookbook.
+### Count A command to just count the number of files matching a query. ```
+Usage: tarentula count [OPTIONS] Options: --datashare-url TEXT Datashare URL --
+datashare-project TEXT Datashare project --elasticsearch-url TEXT You can
+additionally pass the Elasticsearch URL in order to use scrollingcapabilities
+of Elasticsearch (useful when dealing with a lot of results) --query TEXT The
+query string to filter documents --cookies TEXT Key/value pair to add a cookie
+to each request to the API. You can separatesemicolons: key1=val1;key2=val2;...
+--apikey TEXT Datashare authentication apikey in the downloaded document from
+the index --traceback / --no-traceback Display a traceback in case of error --
+type [Document|NamedEntity] Type of indexed documents to download --help Show
+this message and exit ``` ### Clean Tags by Query A command that uses
+Elasticsearch `update-by-query` feature to batch untag documents directly in
+the index. ``` Usage: tarentula clean-tags-by-query [OPTIONS] Options: --
+datashare-project TEXT Datashare project --elasticsearch-url TEXT Elasticsearch
+URL which is used to perform update by query --cookies TEXT Key/value pair to
+add a cookie to each request to the API. You can separatesemicolons:
+key1=val1;key2=val2;... --apikey TEXT Datashare authentication apikey --
+traceback / --no-traceback Display a traceback in case of error --wait-for-
+completion / --no-wait-for-completion Create a Elasticsearch task to perform
+the updateasynchronously --query TEXT Give a JSON query to filter documents
+that will have their tags cleaned. It can be afile with @path/to/file. Default
+to all. --help Show this message and exit ``` ### Download A command to
+download all files matching a query. ``` Usage: tarentula download [OPTIONS]
 Options: --apikey TEXT Datashare authentication apikey --datashare-url TEXT
 Datashare URL --datashare-project TEXT Datashare project --elasticsearch-url
 TEXT You can additionally pass the Elasticsearch URL in order to use
 scrollingcapabilities of Elasticsearch (useful when dealing with a lot of
-results) --query TEXT The query string to filter documents --output-file TEXT
-Path to the CSV file --throttle INTEGER Request throttling (in ms) --cookies
-TEXT Key/value pair to add a cookie to each request to the API. You can
+results) --query TEXT The query string to filter documents --destination-
+directory TEXT Directory documents will be downloaded --throttle INTEGER
+Request throttling (in ms) --cookies TEXT Key/value pair to add a cookie to
+each request to the API. You can separatesemicolons: key1=val1;key2=val2;... --
+path-format TEXT Downloaded document path template --scroll TEXT Scroll
+duration --source TEXT A comma-separated list of field to include in the
+downloaded document from the index -f, --from INTEGER Passed to the search it
+will bypass the first n documents -l, --limit INTEGER Limit the total results
+to return --sort-by TEXT Field to use to sort results --order-by [asc|desc]
+Order to use to sort results --once / --not-once Download file only once --
+traceback / --no-traceback Display a traceback in case of error --progressbar /
+--no-progressbar Display a progressbar --raw-file / --no-raw-file Download raw
+file from Datashare --type [Document|NamedEntity] Type of indexed documents to
+download --help Show this message and exit. ``` ### Export by Query A command
+to export all files matching a query. ``` Usage: tarentula export-by-query
+[OPTIONS] Options: --apikey TEXT Datashare authentication apikey --datashare-
+url TEXT Datashare URL --datashare-project TEXT Datashare project --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in order
+to use scrollingcapabilities of Elasticsearch (useful when dealing with a lot
+of results) --query TEXT The query string to filter documents --output-file
+TEXT Path to the CSV file --throttle INTEGER Request throttling (in ms) --
+cookies TEXT Key/value pair to add a cookie to each request to the API. You can
 separatesemicolons: key1=val1;key2=val2;... --scroll TEXT Scroll duration --
 source TEXT A comma-separated list of field to include in the export --sort-by
 TEXT Field to use to sort results --order-by [asc|desc] Order to use to sort
 results --traceback / --no-traceback Display a traceback in case of error --
 progressbar / --no-progressbar Display a progressbar --type
-[Document|NamedEntity] Type of indexed documents to download --size INTEGER
-Size of the scroll request that powers the operation. --query-field / --no-
-query-field Add the query to the export CSV --help Show this message and exit.
-``` ### Tagging A command to batch tag documents with a CSV file. ``` Usage:
-tarentula tagging [OPTIONS] CSV_PATH Options: --datashare-url TEXT http://
-localhost:8080 Datashare URL --datashare-project TEXT local-datashare Datashare
-project --throttle INTEGER 0 Request throttling (in ms) --cookies TEXT _Empty
-string_ Key/value pair to add a cookie to each request to the API. You can
-separate semicolons: key1=val1;key2=val2;... --apikey TEXT None Datashare
-authentication apikey --traceback / --no-traceback Display a traceback in case
-of error --progressbar / --no-progressbar Display a progressbar --help Show
-this message and exit ``` #### CSV formats Tagging with a `documentId` and
-`routing`: ```csv tag,documentId,routing
-Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
+[Document|NamedEntity] Type of indexed documents to download -f, --from INTEGER
+Passed to the search it will bypass the first n documents -l, --limit INTEGER
+Limit the total results to return --size INTEGER Size of the scroll request
+that powers the operation. --query-field / --no-query-field Add the query to
+the export CSV --help Show this message and exit. ``` ### Tagging A command to
+batch tag documents with a CSV file. ``` Usage: tarentula tagging [OPTIONS]
+CSV_PATH Options: --datashare-url TEXT http://localhost:8080 Datashare URL --
+datashare-project TEXT local-datashare Datashare project --throttle INTEGER 0
+Request throttling (in ms) --cookies TEXT _Empty string_ Key/value pair to add
+a cookie to each request to the API. You can separate semicolons:
+key1=val1;key2=val2;... --apikey TEXT None Datashare authentication apikey --
+traceback / --no-traceback Display a traceback in case of error --progressbar /
+--no-progressbar Display a progressbar --help Show this message and exit ```
+#### CSV formats Tagging with a `documentId` and `routing`: ```csv
+tag,documentId,routing Actinopodidae,l7VnZZEzg2fr960NWWEG,l7VnZZEzg2fr960NWWEG
 Antrodiaetidae,DWLOskax28jPQ2CjFrCo
 Atracidae,6VE7cVlWszkUd94XeuSd,vZJQpKQYhcI577gJR0aN
 Atypidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi
 Barychelidae,DbhveTJEwQfJL5Gn3Zgi,DbhveTJEwQfJL5Gn3Zgi ``` Tagging with a
 `documentUrl`: ```csv tag,documentUrl Mecicobothriidae,http://localhost:8080/#/
 d/local-datashare/DbhveTJEwQfJL5Gn3Zgi/DbhveTJEwQfJL5Gn3Zgi
 Microstigmatidae,http://localhost:8080/#/d/local-datashare/
@@ -116,19 +122,57 @@
 Datashare project --elasticsearch-url TEXT Elasticsearch URL which is used to
 perform update by query --throttle INTEGER Request throttling (in ms) --cookies
 TEXT Key/value pair to add a cookie to each request to the API. You can
 separatesemicolons: key1=val1;key2=val2;... --apikey TEXT Datashare
 authentication apikey --traceback / --no-traceback Display a traceback in case
 of error --progressbar / --no-progressbar Display a progressbar --wait-for-
 completion / --no-wait-for-completion Create a Elasticsearch task to perform
-the updateasynchronously --help Show this message and exit ``` ### Following
-your changes When running Elasticsearch changes on big datasets, it could take
-a very long time. As we were curling ES to see if the task was still running
-well, we added a small utility to follow the changes. It makes a live graph of
-a provided ES indicator with a specified filter. It uses [mathplotlib](https://
+the updateasynchronously --help Show this message and exit ``` ### List
+Metadata You can list the metadata from the mapping, optionally counting the
+number of occurrences of each field in the index, with the `--count` parameter.
+Counting the fields is disabled by default. It includes a `--filter_by`
+parameter to narrow retrieving metadata properties of specific sets of
+documents. For instance it can be used to get just emails related properties
+with: `--filter_by "contentType=message/rfc822"` ``` $ tarentula list-metadata
+--help Usage: tarentula list-metadata [OPTIONS] Options: --datashare-project
+TEXT Datashare project --elasticsearch-url TEXT You can additionally pass the
+Elasticsearch URL in order to use scrollingcapabilities of Elasticsearch
+(useful when dealing with a lot of results) --type [Document|NamedEntity] Type
+of indexed documents to get metadata --filter_by TEXT Filter documents by pairs
+concatenated by coma of field names and values separated by =.Example
+"contentType=message/rfc822,content Type=message/rfc822" --count / --no-count
+Count or not the number of docs for each property found --help Show this
+message and exit. ``` ### Aggregate You can run aggregations on the data, the
+ElasticSearch aggregations API is partially enabled with this command. The
+possibilities are: - count: grouping by a given field different values, and
+count the num of docs. - nunique: returns the number of unique values of a
+given field. - date_histogram: returns counting of monthly or yearly grouped
+values for a given date field. - sum: returns the sum of values of number type
+fields. - min: returns the min of values of number type fields. - max: returns
+the max of values of number type fields. - avg: returns the average of values
+of number type fields. - stats: returns a bunch of statistics for a given
+number type fields. - string_stats: returns a bunch of string statistics for a
+given string type fields. ``` $ tarentula aggregate --help Usage: tarentula
+aggregate [OPTIONS] Options: --apikey TEXT Datashare authentication apikey --
+datashare-url TEXT Datashare URL --datashare-project TEXT Datashare project --
+elasticsearch-url TEXT You can additionally pass the Elasticsearch URL in order
+to use scrollingcapabilities of Elasticsearch (useful when dealing with a lot
+of results) --query TEXT The query string to filter documents --cookies TEXT
+Key/value pair to add a cookie to each request to the API. You can
+separatesemicolons: key1=val1;key2=val2;... --traceback / --no-traceback
+Display a traceback in case of error --type [Document|NamedEntity] Type of
+indexed documents to download --group_by TEXT Field to use to aggregate results
+--operation_field TEXT Field to run the operation on --run
+[count|nunique|date_histogram|sum|stats|string_stats|min|max|avg] Operation to
+run --calendar_interval [year|month] Calendar interval for date histogram
+aggregation --help Show this message and exit. ``` ### Following your changes
+When running Elasticsearch changes on big datasets, it could take a very long
+time. As we were curling ES to see if the task was still running well, we added
+a small utility to follow the changes. It makes a live graph of a provided ES
+indicator with a specified filter. It uses [mathplotlib](https://
 matplotlib.org/) and python3-tk. If you see the following message : ``` $
 graph_es graph_realtime.py:32: UserWarning: Matplotlib is currently using agg,
 which is a non-GUI backend, so cannot show the figure ``` Then you have to
 install [tkinter](https://docs.python.org/3/library/tkinter.html), i.e.
 python3-tk for Debian/Ubuntu. The command has the options below: ``` $ graph_es
 --help Usage: graph_es [OPTIONS] Options: --query TEXT Give a JSON query to
 filter documents. It can be a file with @path/to/file. Default to all. --index
@@ -156,10 +200,13 @@
 package and [Docker Hub](https://hub.docker.com/) for the Docker image. ### 1.
 Create a new release ``` make [patch|minor|major] ``` ### 2. Upload
 distributions on pypi _To be able to do this, you will need to be a maintainer
 of the [pypi](https://pypi.org/project/tarentula/) project._ ``` make
 distribute ``` ### 3. Build and publish the Docker image To build and upload a
 new image on the [docker repository](https://hub.docker.com/repository/docker/
 icij/datashare-tarentula) : _To be able to do this, you will need to be part of
-the ICIJ organization on docker_ ``` make docker-publish ``` ### 4. Push your
-changes on Github Git push release and tag : ``` git push origin master --tags
-```
+the ICIJ organization on docker_ ``` make docker-publish ``` **Note**:
+Datashare Tarentula is a multi-platform build. You might need to setup your
+environment for multi-platform using the `make docker-setup-multiarch` command.
+Read more [on Docker documentation](https://docs.docker.com/build/building/
+multi-platform/). ### 4. Push your changes on Github Git push release and tag :
+``` git push origin master --tags ```
```

