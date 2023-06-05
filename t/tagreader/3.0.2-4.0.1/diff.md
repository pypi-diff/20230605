# Comparing `tmp/tagreader-3.0.2.tar.gz` & `tmp/tagreader-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-3.0.2.tar", last modified: Wed Jun 22 13:32:06 2022, max compression
+gzip compressed data, was "tagreader-4.0.1.tar", max compression
```

## Comparing `tagreader-3.0.2.tar` & `tagreader-4.0.1.tar`

### file list

```diff
@@ -1,26 +1,10 @@
-drwxrwxrwx   0        0        0        0 2022-06-22 13:32:06.611927 tagreader-3.0.2/
--rw-rw-rw-   0        0        0     4471 2022-06-22 13:30:54.000000 tagreader-3.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1085 2022-06-22 13:30:54.000000 tagreader-3.0.2/LICENSE
--rw-rw-rw-   0        0        0      187 2022-06-22 13:30:54.000000 tagreader-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3039 2022-06-22 13:32:06.611927 tagreader-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2022-06-22 13:30:54.000000 tagreader-3.0.2/README.md
--rw-rw-rw-   0        0        0       94 2022-06-22 13:30:54.000000 tagreader-3.0.2/dev-requirements.in
--rw-rw-rw-   0        0        0     5113 2022-06-22 13:30:54.000000 tagreader-3.0.2/dev-requirements.txt
--rw-rw-rw-   0        0        0      145 2022-06-22 13:30:54.000000 tagreader-3.0.2/pytest.ini
--rw-rw-rw-   0        0        0      140 2022-06-22 13:30:54.000000 tagreader-3.0.2/requirements.in
--rw-rw-rw-   0        0        0      732 2022-06-22 13:32:06.611927 tagreader-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3597 2022-06-22 13:30:54.000000 tagreader-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-22 13:32:06.608926 tagreader-3.0.2/tagreader/
--rw-rw-rw-   0        0        0      604 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/__init__.py
--rw-rw-rw-   0        0        0    16311 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/cache.py
--rw-rw-rw-   0        0        0    18354 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/clients.py
--rw-rw-rw-   0        0        0    24369 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/odbc_handlers.py
--rw-rw-rw-   0        0        0     7652 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/utils.py
--rw-rw-rw-   0        0        0      181 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader/version.py
--rw-rw-rw-   0        0        0    32206 2022-06-22 13:30:54.000000 tagreader-3.0.2/tagreader/web_handlers.py
-drwxrwxrwx   0        0        0        0 2022-06-22 13:32:06.610929 tagreader-3.0.2/tagreader.egg-info/
--rw-rw-rw-   0        0        0     3039 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-22 13:32:06.000000 tagreader-3.0.2/tagreader.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1064 2023-05-10 10:09:58.051900 tagreader-4.0.1/LICENSE
+-rw-r--r--   0        0        0     2767 2023-06-04 08:39:01.932022 tagreader-4.0.1/README.md
+-rw-r--r--   0        0        0     1408 2023-06-05 11:45:51.193262 tagreader-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      587 2023-06-04 08:39:01.936509 tagreader-4.0.1/tagreader/__init__.py
+-rw-r--r--   0        0        0    16016 2023-06-04 08:39:01.937333 tagreader-4.0.1/tagreader/cache.py
+-rw-r--r--   0        0        0    18678 2023-06-04 08:39:01.937705 tagreader-4.0.1/tagreader/clients.py
+-rw-r--r--   0        0        0    23714 2023-06-04 08:39:01.938228 tagreader-4.0.1/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     7574 2023-06-04 08:39:01.938561 tagreader-4.0.1/tagreader/utils.py
+-rw-r--r--   0        0        0    31605 2023-06-04 08:39:01.938889 tagreader-4.0.1/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4391 1970-01-01 00:00:00.000000 tagreader-4.0.1/PKG-INFO
```

### Comparing `tagreader-3.0.2/PKG-INFO` & `tagreader-4.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,75 @@
-Metadata-Version: 2.1
-Name: tagreader
-Version: 3.0.2
-Summary: Library for reading from Aspen InfoPlus.21 and OSIsoft PI IMS servers
-Home-page: https://github.com/equinor/tagreader-python
-Author: Einar S. Idsø
-Author-email: eiids@equinor.com
-License: MIT
-Keywords: Aspen InfoPlus.21,OSIsoft PI
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Tagreader #
-
-Tagreader is a Python package for reading trend data from the OSIsoft
-PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use,
-and present as similar interfaces as possible to the backend historians.
-
-While originally developed for Windows, Tagreader can since release 3.0.0
-also be used on Linux and Windows platforms.
-
-Queries can be performed using either REST API (preferred) or ODBC queries.
-The use of ODBC queries require installation of proprietary drivers from
-AspenTech and OSIsoft that are only available for Windows.
-
-Trend data is output as Pandas Dataframes. The HDF5 file format is used
-to cache results.
-
-## Requirements
-
-Python >=3.7 with the following packages:
-
-  + pandas >= 1.0.0
-  + tables (*)
-  + requests
-  + requests-kerberos
-  + certifi >= 2020.04.05
-  + pyodbc (**)
-
-*) If tables is not installed, caching of fetched data will be disabled.
-Tables will be installed alongside Tagreader unless the installation is
-known to fail, which is the case for Macs with M1 chip.
-
-**) If using ODBC connections, you must also install proprietary drivers for
-PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
-Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
-systems.
-
-## Installation
-
-To install and/or upgrade:
-
-```
-pip install --upgrade tagreader
-```
-
-## Usage example ##
-
-```
-import tagreader
-c = tagreader.IMSClient("mysource", "aspenone")
-print(c.search("tag*"))
-df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
-```
-
-Also see the
-[quickstart](https://github.com/equinor/tagreader-python/blob/master/docs/quickstart.ipynb)
-document and the
-[manual](docs/https://github.com/equinor/tagreader-python/blob/master/docs/manual.md)
-for more information.
-
-
+# tagreader-python <!-- omit in toc -->
+
+![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
+[![Devops Build Status](https://dev.azure.com/EIIDS/tagreader/_apis/build/status/equinor.tagreader-python?branchName=master)](https://dev.azure.com/EIIDS/tagreader/_build/latest?definitionId=5&branchName=master)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader) 
+![PyPI](https://img.shields.io/pypi/v/tagreader) 
+[![Downloads](https://pepy.tech/badge/tagreader)](https://pepy.tech/project/tagreader)
+
+Tagreader is a Python package for reading trend data from the OSIsoft
+PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use, 
+and present as similar interfaces as possible to the backend historians.
+
+While originally developed for Windows, Tagreader can since release 3.0.0
+also be used on Linux and Windows platforms.
+
+Queries can be performed using either REST API (preferred) or ODBC queries.
+The use of ODBC queries require installation of proprietary drivers from
+AspenTech and OSIsoft that are only available for Windows.
+
+Trend data is output as Pandas Dataframes. The HDF5 file format is used
+to cache results.
+
+## Requirements
+
+Python >=3.8 with the following packages:
+
+  + pandas >= 1.0.0
+  + tables (*)
+  + requests
+  + requests-kerberos
+  + certifi >= 2023.5.7
+  + pyodbc (**)
+
+*) If tables is not installed, caching of fetched data will be disabled.
+Tables will be installed alongside Tagreader unless the installation is
+known to fail, which is the case for Macs with ARM CPU.
+
+**) If using ODBC connections, you must also install proprietary drivers for
+PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
+Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
+systems.
+
+## Installation
+
+To install and/or upgrade:
+
+``` 
+pip install --upgrade tagreader
+```
+
+If you wish to use ODBC connections to the IMS servers, you will also need 
+to install some proprietary drivers. There is more information in the 
+[manual](docs/manual.md#odbc-drivers). Please note that the web APIs should
+normally be preferred.
+
+## Usage example
+
+```
+import tagreader
+c = tagreader.IMSClient("mysource", "aspenone")
+print(c.search("tag*"))
+df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
+```
+
+## Documentation
+
+There is a [quickstart](docs/quickstart.ipynb) example file that should get
+you going. Also check out the [manual](docs/manual.md) for more information.
+
+## Contributing
+
+All contributions are welcome, including code, bug reports, issues, feature
+requests, and documentation. The preferred way of submitting a contribution
+is to either create an issue on GitHub or to fork the project and make a pull
+request.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tagreader-3.0.2/tagreader/cache.py` & `tagreader-4.0.1/tagreader/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,433 +1,431 @@
-import os
-import warnings
-from importlib.util import find_spec
-from typing import Dict, List, Tuple, Union
-
-import pandas as pd
-
-from .utils import ReaderType
-
-
-def safe_tagname(tagname: str) -> str:
-    tagname = tagname.replace(".", "_")
-    tagname = "".join(c for c in tagname if c.isalnum() or c == "_").strip()
-    if tagname[0].isnumeric():
-        tagname = "_" + tagname  # Conform to NaturalName
-    return tagname
-
-
-def timestamp_to_epoch(timestamp: pd.Timestamp) -> int:
-    origin = pd.Timestamp("1970-01-01")
-    if timestamp.tzinfo is not None:
-        timestamp = timestamp.tz_convert("UTC").tz_localize(None)
-    return (timestamp - origin) // pd.Timedelta("1s")  # type: ignore
-
-
-class BucketCache:
-    def __init__(self, filename: str, path: str = ".") -> None:
-        if not find_spec("tables"):
-            warnings.warn("Package 'tables' not installed. Disabling cache.")
-            return None
-        self.filename = os.path.splitext(filename)[0] + ".h5"
-        self.filename = os.path.join(path, self.filename)
-
-    def _key_path(
-        self,
-        tagname: str,
-        readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
-        stepped: bool,
-        status: bool,
-        starttime: pd.Timestamp = None,
-        endtime: pd.Timestamp = None,
-    ) -> str:
-        """Return a string on the form
-        /tagname/readtype[/sample_time][/stepped][/status]/_starttime_endtime
-        tagname: safe tagname
-        sample_time: integer value. Empty for RAW.
-        stepped: "stepped" if value was read as stepped. Empty if not.
-        status: "status" if value contains status. Empty if not.
-        starttime: The starttime of the query that created the bucket.
-        endtime: The endtime of the query that created the bucket.
-        """
-        tagname = safe_tagname(tagname)
-
-        ts = (
-            int(ts.total_seconds())
-            if readtype != ReaderType.RAW and isinstance(ts, pd.Timedelta)
-            else ts
-        )
-        timespan = ""
-        if starttime is not None:
-            starttime_epoch = timestamp_to_epoch(starttime)
-            endtime_epoch = timestamp_to_epoch(endtime)
-            timespan = f"/_{starttime_epoch}_{endtime_epoch}"
-
-        keyval = (
-            f"/{tagname}"
-            f"/{readtype.name}"
-            f"{(ts is not None and readtype != ReaderType.RAW) * f'/s{ts}'}"
-            f"{stepped * '/stepped'}"
-            f"{status * '/status'}"
-            f"{timespan}"
-        )
-        return keyval
-
-    def store_tag_metadata(
-        self, tagname: str, metadata: Dict[str, Union[str, int]]
-    ) -> None:
-        tagname = safe_tagname(tagname)
-        key = f"/{tagname}"
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key not in f:
-                f.put(key, pd.DataFrame())
-            origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:
-                origmetadata = f.get_storer(key).attrs.metadata
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
-
-    def fetch_tag_metadata(
-        self, tagname: str, properties: Union[str, List[str]]
-    ) -> Dict[str, Union[str, int]]:
-        res = {}  # type: Dict[str, Union[str, int]]
-        if not os.path.isfile(self.filename):
-            return res
-        tagname = safe_tagname(tagname)
-        key = f"/{tagname}"
-        if isinstance(properties, str):
-            properties = [properties]
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:
-                return {}
-            metadata = f.get_storer(key).attrs.metadata
-        for p in properties:
-            if p in metadata.keys():
-                res[p] = metadata.get(p)
-        return res
-
-    def remove(self, filename: str = None) -> None:
-        if not filename:
-            filename = self.filename
-        if os.path.isfile(filename):
-            os.unlink(filename)
-
-    def store(
-        self,
-        df: pd.DataFrame,
-        tagname: str,
-        readtype: ReaderType,
-        ts: pd.Timestamp,
-        stepped: bool,
-        status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
-    ) -> None:
-        if df.empty:
-            return
-
-        intersecting = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
-        )
-        if len(intersecting) > 0:
-            with pd.HDFStore(self.filename, mode="a") as f:
-                for dataset in intersecting:
-                    this_start, this_end = self._get_intervals_from_dataset_name(
-                        dataset
-                    )
-                    starttime = min(starttime, this_start)
-                    endtime = max(endtime, this_end)
-                    df = pd.concat([df, f.get(dataset)])
-                    del f[dataset]
-            df = df[~df.index.duplicated(keep="first")].sort_index()
-        key = self._key_path(tagname, readtype, ts, stepped, status, starttime, endtime)
-        with pd.HDFStore(self.filename, mode="a") as f:
-            f.put(key, df, format="table")
-
-    @staticmethod
-    def _get_intervals_from_dataset_name(
-        name: str,
-    ) -> Tuple[pd.Timestamp, pd.Timestamp]:
-        name_with_times = name.split("/")[-1]
-        if not name_with_times.count("_") == 2:
-            return (None, None)
-        _, starttime_epoch, endtime_epoch = name_with_times.split("_")
-        starttime = pd.to_datetime(int(starttime_epoch), unit="s").tz_localize("UTC")
-        endtime = pd.to_datetime(int(endtime_epoch), unit="s").tz_localize("UTC")
-        return starttime, endtime
-
-    def get_intersecting_datasets(
-        self,
-        tagname: str,
-        readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
-        stepped: bool,
-        status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
-    ) -> List[str]:
-
-        if not os.path.isfile(self.filename):
-            return []
-        intersecting_datasets = []
-        with pd.HDFStore(self.filename, mode="r") as f:
-            for bucket in f.walk(
-                where=self._key_path(tagname, readtype, ts, stepped, status)
-            ):
-                for leaf in bucket[2]:
-                    dataset = bucket[0] + "/" + leaf
-                    starttime_ds, endtime_ds = self._get_intervals_from_dataset_name(
-                        dataset
-                    )
-                    if endtime_ds >= starttime and endtime >= starttime_ds:
-                        intersecting_datasets.append(dataset)
-        return intersecting_datasets
-
-    def get_missing_intervals(
-        self,
-        tagname: str,
-        readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
-        stepped: bool,
-        status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
-    ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
-
-        datasets = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
-        )
-        missing_intervals = [(starttime, endtime)]
-        for dataset in datasets:
-            b = self._get_intervals_from_dataset_name(dataset)
-            for _ in range(0, len(missing_intervals)):
-                r = missing_intervals.pop(0)
-                if b[1] < r[0] or b[0] > r[1]:
-                    # No overlap
-                    missing_intervals.append(r)
-                elif b[0] <= r[0] and b[1] >= r[1]:
-                    # The bucket covers the entire interval
-                    continue
-                elif b[0] > r[0] and b[1] < r[1]:
-                    # The bucket splits the interval in two
-                    missing_intervals.append((r[0], b[0]))
-                    missing_intervals.append((b[1], r[1]))
-                elif b[0] <= r[0] and r[0] <= b[1] < r[1]:
-                    # The bucket chomps the start of the interval
-                    missing_intervals.append((b[1], r[1]))
-                elif r[0] < b[0] <= r[1] and b[1] >= r[1]:
-                    # The bucket chomps the end of the interval
-                    missing_intervals.append((r[0], b[0]))
-        return missing_intervals
-
-    def fetch(
-        self,
-        tagname: str,
-        readtype: ReaderType,
-        ts: int,
-        stepped: bool,
-        status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
-    ) -> pd.DataFrame:
-        df = pd.DataFrame()
-        if not os.path.isfile(self.filename):
-            return df
-
-        datasets = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
-        )
-
-        with pd.HDFStore(self.filename, mode="r") as f:
-            for dataset in datasets:
-                # df = df.append(
-                #     f.select(dataset, where="index >= starttime and index <= endtime")
-                # )
-                df = pd.concat(
-                    [
-                        df,
-                        f.select(
-                            dataset, where="index >= starttime and index <= endtime"
-                        ),
-                    ]
-                )
-
-        return df.sort_index()
-
-
-class SmartCache:
-    def __init__(self, filename: str, path: str = ".") -> None:
-        if not find_spec("tables"):
-            warnings.warn("Package 'tables' not installed. Disabling cache.")
-            return None
-        self.filename = os.path.splitext(filename)[0] + ".h5"
-        self.filename = os.path.join(path, self.filename)
-        # self.open(self.filename)
-
-    # def open(self, filename=None):
-    #     if filename is None:
-    #         filename = self.filename
-    #     self.hdfstore = pd.HDFStore(filename)
-    #
-    # def close(self):
-    #     self.hdfstore.close()
-
-    @staticmethod
-    def key_path(
-        df: Union[str, pd.DataFrame],
-        readtype: ReaderType,
-        ts: Union[int, pd.Timedelta] = None,
-    ) -> str:
-        """Return a string on the form
-        XXX/sYY/ZZZ where XXX is the ReadType, YY is the interval between samples
-        (in seconds) and ZZZ is a safe tagname.
-        """
-        name = list(df)[0] if isinstance(df, pd.DataFrame) else df
-        name = safe_tagname(name)
-        ts = int(ts.total_seconds()) if isinstance(ts, pd.Timedelta) else ts
-        if readtype != ReaderType.RAW:
-            if ts is None:
-                # Determine sample time by reading interval between first two
-                # samples of dataframe.
-                if isinstance(df, pd.DataFrame):
-                    interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)
-                else:
-                    raise TypeError
-            else:
-                interval = int(ts)
-            return f"{readtype.name}/s{interval}/{name}"
-        else:
-            return f"{readtype.name}/{name}"
-
-    def store(
-        self,
-        df: pd.DataFrame,
-        readtype: ReaderType,
-        ts: Union[int, pd.Timedelta] = None,
-    ) -> None:
-        key = self.key_path(df, readtype, ts)
-        if df.empty:
-            return  # Weirdness ensues when using empty df in select statement below
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key in f:
-                idx = f.select(  # noqa: F841
-                    key, where="index in df.index", columns=["index"]
-                ).index
-                f.append(key, df.query("index not in @idx"))
-            else:
-                f.append(key, df)
-
-    def fetch(
-        self,
-        tagname: str,
-        readtype: ReaderType,
-        ts: Union[int, pd.Timestamp] = None,
-        start_time: pd.Timestamp = None,
-        stop_time: pd.Timestamp = None,
-    ) -> pd.DataFrame:
-        df = pd.DataFrame()
-        if not os.path.isfile(self.filename):
-            return df
-        key = self.key_path(tagname, readtype, ts)
-        where = []
-        if start_time is not None:
-            where.append("index >= start_time")
-        if stop_time is not None:
-            where.append("index <= stop_time")
-        wheretxt = " and ".join(where)
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key in f:
-                if wheretxt:
-                    df = f.select(key, where=wheretxt)
-                else:
-                    df = f.select(key)
-        return df.sort_index()
-
-    def store_tag_metadata(
-        self, tagname: str, metadata: Dict[str, Union[str, int]]
-    ) -> None:
-        tagname = safe_tagname(tagname)
-        key = f"/metadata/{tagname}"
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key not in f:
-                f.put(key, pd.DataFrame())
-            origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:
-                origmetadata = f.get_storer(key).attrs.metadata
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
-
-    def fetch_tag_metadata(
-        self, tagname: str, properties: Union[str, List[str]]
-    ) -> Dict[str, Union[str, int]]:
-        res = {}  # type: Dict[str, Union[str, int]]
-        if not os.path.isfile(self.filename):
-            return res
-        tagname = safe_tagname(tagname)
-        key = f"/metadata/{tagname}"
-        if isinstance(properties, str):
-            properties = [properties]
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:
-                return {}
-            metadata = f.get_storer(key).attrs.metadata
-        for p in properties:
-            if p in metadata.keys():
-                res[p] = metadata.get(p)
-        return res
-
-    def remove(self, filename: str = None) -> None:
-        if not filename:
-            filename = self.filename
-            # self.close()
-        if os.path.isfile(filename):
-            os.unlink(filename)
-
-    def _match_tag(self, key, readtype=None, ts=None, tagname=None):  # type: ignore
-        def readtype_to_str(rt):  # type: ignore
-            return getattr(
-                rt, "name", rt
-            )  # if isinstance(rt, ReaderType) always returns False...?
-
-        def timedelta_to_str(t):  # type: ignore
-            if isinstance(t, pd.Timedelta):
-                return str(int(t.total_seconds()))
-            return t
-
-        key = "/" + key.lstrip("/")  # Ensure absolute path
-        readtype = readtype if isinstance(readtype, list) else [readtype]
-        ts = ts if isinstance(ts, list) else [ts]
-        tagname = tagname if isinstance(tagname, list) else [tagname]
-        readtype = list(map(readtype_to_str, readtype))
-        ts = list(map(timedelta_to_str, ts))
-        if tagname[0] is not None:
-            tagname = list(map(safe_tagname, tagname))
-        # print(f"Readtype: {readtype}, ts: {ts}, tagname: {tagname}")
-        elements = key.split("/")[1:]
-        if len(elements) == 2:
-            elements.insert(1, None)
-        else:
-            elements[1] = int(elements[1][1:])  # Discard the initial s
-        if elements[0] not in readtype and readtype[0] is not None:
-            # print(f"{elements[0]} not in {readtype}")
-            return False
-        if elements[1] not in ts and ts[0] is not None:
-            # print(f"{elements[1]} not in {ts}")
-            return False
-        if elements[2] not in tagname and tagname[0] is not None:
-            # print(f"{elements[2]} not in {tagname}")
-            return False
-        return True
-
-    def delete_key(
-        self,
-        tagname: str = None,
-        readtype: ReaderType = None,
-        ts: Union[int, List[int]] = None,
-    ) -> None:
-        with pd.HDFStore(self.filename) as f:
-            for key in f:
-                if self._match_tag(key, tagname=tagname, readtype=readtype, ts=ts):
-                    f.remove(key)
-
-    def _get_hdfstore(self, mode: str = "r") -> pd.HDFStore:
-        f = pd.HDFStore(self.filename, mode)
-        return f
+import os
+import warnings
+from importlib.util import find_spec
+from typing import Dict, List, Tuple, Union
+
+import pandas as pd
+
+from .utils import ReaderType
+
+
+def safe_tagname(tagname: str) -> str:
+    tagname = tagname.replace(".", "_")
+    tagname = "".join(c for c in tagname if c.isalnum() or c == "_").strip()
+    if tagname[0].isnumeric():
+        tagname = "_" + tagname  # Conform to NaturalName
+    return tagname
+
+
+def timestamp_to_epoch(timestamp: pd.Timestamp) -> int:
+    origin = pd.Timestamp("1970-01-01")
+    if timestamp.tzinfo is not None:
+        timestamp = timestamp.tz_convert("UTC").tz_localize(None)
+    return (timestamp - origin) // pd.Timedelta("1s")  # type: ignore
+
+
+class BucketCache:
+    def __init__(self, filename: str, path: str = ".") -> None:
+        if not find_spec("tables"):
+            warnings.warn("Package 'tables' not installed. Disabling cache.")
+            return None
+        self.filename = os.path.splitext(filename)[0] + ".h5"
+        self.filename = os.path.join(path, self.filename)
+
+    def _key_path(
+        self,
+        tagname: str,
+        readtype: ReaderType,
+        ts: Union[int, pd.Timedelta],
+        stepped: bool,
+        status: bool,
+        starttime: pd.Timestamp = None,
+        endtime: pd.Timestamp = None,
+    ) -> str:
+        """Return a string on the form
+        /tagname/readtype[/sample_time][/stepped][/status]/_starttime_endtime
+        tagname: safe tagname
+        sample_time: integer value. Empty for RAW.
+        stepped: "stepped" if value was read as stepped. Empty if not.
+        status: "status" if value contains status. Empty if not.
+        starttime: The starttime of the query that created the bucket.
+        endtime: The endtime of the query that created the bucket.
+        """
+        tagname = safe_tagname(tagname)
+
+        ts = (
+            int(ts.total_seconds())
+            if readtype != ReaderType.RAW and isinstance(ts, pd.Timedelta)
+            else ts
+        )
+        timespan = ""
+        if starttime is not None:
+            starttime_epoch = timestamp_to_epoch(starttime)
+            endtime_epoch = timestamp_to_epoch(endtime)
+            timespan = f"/_{starttime_epoch}_{endtime_epoch}"
+
+        keyval = (
+            f"/{tagname}"
+            f"/{readtype.name}"
+            f"{(ts is not None and readtype != ReaderType.RAW) * f'/s{ts}'}"
+            f"{stepped * '/stepped'}"
+            f"{status * '/status'}"
+            f"{timespan}"
+        )
+        return keyval
+
+    def store_tag_metadata(
+        self, tagname: str, metadata: Dict[str, Union[str, int]]
+    ) -> None:
+        tagname = safe_tagname(tagname)
+        key = f"/{tagname}"
+        with pd.HDFStore(self.filename, mode="a") as f:
+            if key not in f:
+                f.put(key, pd.DataFrame())
+            origmetadata = {}
+            if "metadata" in f.get_storer(key).attrs:
+                origmetadata = f.get_storer(key).attrs.metadata
+            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
+
+    def fetch_tag_metadata(
+        self, tagname: str, properties: Union[str, List[str]]
+    ) -> Dict[str, Union[str, int]]:
+        res = {}  # type: Dict[str, Union[str, int]]
+        if not os.path.isfile(self.filename):
+            return res
+        tagname = safe_tagname(tagname)
+        key = f"/{tagname}"
+        if isinstance(properties, str):
+            properties = [properties]
+        with pd.HDFStore(self.filename, mode="r") as f:
+            if key not in f or "metadata" not in f.get_storer(key).attrs:
+                return {}
+            metadata = f.get_storer(key).attrs.metadata
+        for p in properties:
+            if p in metadata.keys():
+                res[p] = metadata.get(p)
+        return res
+
+    def remove(self, filename: str = None) -> None:  # type: ignore[assignment]
+        if not filename:
+            filename = self.filename
+        if os.path.isfile(filename):
+            os.unlink(filename)
+
+    def store(
+        self,
+        df: pd.DataFrame,
+        tagname: str,
+        readtype: ReaderType,
+        ts: pd.Timestamp,
+        stepped: bool,
+        status: bool,
+        starttime: pd.Timestamp,
+        endtime: pd.Timestamp,
+    ) -> None:
+        if df.empty:
+            return
+
+        intersecting = self.get_intersecting_datasets(
+            tagname, readtype, ts, stepped, status, starttime, endtime
+        )
+        if len(intersecting) > 0:
+            with pd.HDFStore(self.filename, mode="a") as f:
+                for dataset in intersecting:
+                    this_start, this_end = self._get_intervals_from_dataset_name(
+                        dataset
+                    )
+                    starttime = min(starttime, this_start)
+                    endtime = max(endtime, this_end)
+                    df = pd.concat([df, f.get(dataset)])
+                    del f[dataset]
+            df = df[~df.index.duplicated(keep="first")].sort_index()
+        key = self._key_path(tagname, readtype, ts, stepped, status, starttime, endtime)
+        with pd.HDFStore(self.filename, mode="a") as f:
+            f.put(key, df, format="table")
+
+    @staticmethod
+    def _get_intervals_from_dataset_name(
+        name: str,
+    ) -> Tuple[pd.Timestamp, pd.Timestamp]:
+        name_with_times = name.split("/")[-1]
+        if not name_with_times.count("_") == 2:
+            return (None, None)
+        _, starttime_epoch, endtime_epoch = name_with_times.split("_")
+        starttime = pd.to_datetime(int(starttime_epoch), unit="s").tz_localize("UTC")
+        endtime = pd.to_datetime(int(endtime_epoch), unit="s").tz_localize("UTC")
+        return starttime, endtime
+
+    def get_intersecting_datasets(
+        self,
+        tagname: str,
+        readtype: ReaderType,
+        ts: Union[int, pd.Timedelta],
+        stepped: bool,
+        status: bool,
+        starttime: pd.Timestamp,
+        endtime: pd.Timestamp,
+    ) -> List[str]:
+        if not os.path.isfile(self.filename):
+            return []
+        intersecting_datasets = []
+        with pd.HDFStore(self.filename, mode="r") as f:
+            for bucket in f.walk(
+                where=self._key_path(tagname, readtype, ts, stepped, status)
+            ):
+                for leaf in bucket[2]:
+                    dataset = bucket[0] + "/" + leaf
+                    starttime_ds, endtime_ds = self._get_intervals_from_dataset_name(
+                        dataset
+                    )
+                    if endtime_ds >= starttime and endtime >= starttime_ds:
+                        intersecting_datasets.append(dataset)
+        return intersecting_datasets
+
+    def get_missing_intervals(
+        self,
+        tagname: str,
+        readtype: ReaderType,
+        ts: Union[int, pd.Timedelta],
+        stepped: bool,
+        status: bool,
+        starttime: pd.Timestamp,
+        endtime: pd.Timestamp,
+    ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
+        datasets = self.get_intersecting_datasets(
+            tagname, readtype, ts, stepped, status, starttime, endtime
+        )
+        missing_intervals = [(starttime, endtime)]
+        for dataset in datasets:
+            b = self._get_intervals_from_dataset_name(dataset)
+            for _ in range(0, len(missing_intervals)):
+                r = missing_intervals.pop(0)
+                if b[1] < r[0] or b[0] > r[1]:
+                    # No overlap
+                    missing_intervals.append(r)
+                elif b[0] <= r[0] and b[1] >= r[1]:
+                    # The bucket covers the entire interval
+                    continue
+                elif b[0] > r[0] and b[1] < r[1]:
+                    # The bucket splits the interval in two
+                    missing_intervals.append((r[0], b[0]))
+                    missing_intervals.append((b[1], r[1]))
+                elif b[0] <= r[0] and r[0] <= b[1] < r[1]:
+                    # The bucket chomps the start of the interval
+                    missing_intervals.append((b[1], r[1]))
+                elif r[0] < b[0] <= r[1] and b[1] >= r[1]:
+                    # The bucket chomps the end of the interval
+                    missing_intervals.append((r[0], b[0]))
+        return missing_intervals
+
+    def fetch(
+        self,
+        tagname: str,
+        readtype: ReaderType,
+        ts: int,
+        stepped: bool,
+        status: bool,
+        starttime: pd.Timestamp,
+        endtime: pd.Timestamp,
+    ) -> pd.DataFrame:
+        df = pd.DataFrame()
+        if not os.path.isfile(self.filename):
+            return df
+
+        datasets = self.get_intersecting_datasets(
+            tagname, readtype, ts, stepped, status, starttime, endtime
+        )
+
+        with pd.HDFStore(self.filename, mode="r") as f:
+            for dataset in datasets:
+                # df = df.append(
+                #     f.select(dataset, where="index >= starttime and index <= endtime")
+                # )
+                df = pd.concat(
+                    [
+                        df,
+                        f.select(
+                            dataset, where="index >= starttime and index <= endtime"
+                        ),
+                    ]
+                )
+
+        return df.sort_index()
+
+
+class SmartCache:
+    def __init__(self, filename: str, path: str = ".") -> None:
+        if not find_spec("tables"):
+            warnings.warn("Package 'tables' not installed. Disabling cache.")
+            return None
+        self.filename = os.path.splitext(filename)[0] + ".h5"
+        self.filename = os.path.join(path, self.filename)
+        # self.open(self.filename)
+
+    # def open(self, filename=None):
+    #     if filename is None:
+    #         filename = self.filename
+    #     self.hdfstore = pd.HDFStore(filename)
+    #
+    # def close(self):
+    #     self.hdfstore.close()
+
+    @staticmethod
+    def key_path(
+        df: Union[str, pd.DataFrame],
+        readtype: ReaderType,
+        ts: Union[int, pd.Timedelta] = None,
+    ) -> str:
+        """Return a string on the form
+        XXX/sYY/ZZZ where XXX is the ReadType, YY is the interval between samples
+        (in seconds) and ZZZ is a safe tagname.
+        """
+        name = list(df)[0] if isinstance(df, pd.DataFrame) else df
+        name = safe_tagname(name)
+        ts = int(ts.total_seconds()) if isinstance(ts, pd.Timedelta) else ts
+        if readtype != ReaderType.RAW:
+            if ts is None:
+                # Determine sample time by reading interval between first two
+                # samples of dataframe.
+                if isinstance(df, pd.DataFrame):
+                    interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)
+                else:
+                    raise TypeError
+            else:
+                interval = int(ts)
+            return f"{readtype.name}/s{interval}/{name}"
+        else:
+            return f"{readtype.name}/{name}"
+
+    def store(
+        self,
+        df: pd.DataFrame,
+        readtype: ReaderType,
+        ts: Union[int, pd.Timedelta] = None,
+    ) -> None:
+        key = self.key_path(df, readtype, ts)
+        if df.empty:
+            return  # Weirdness ensues when using empty df in select statement below
+        with pd.HDFStore(self.filename, mode="a") as f:
+            if key in f:
+                idx = f.select(  # noqa: F841
+                    key, where="index in df.index", columns=["index"]
+                ).index
+                f.append(key, df.query("index not in @idx"))
+            else:
+                f.append(key, df)
+
+    def fetch(
+        self,
+        tagname: str,
+        readtype: ReaderType,
+        ts: Union[int, pd.Timestamp] = None,
+        start_time: pd.Timestamp = None,
+        stop_time: pd.Timestamp = None,
+    ) -> pd.DataFrame:
+        df = pd.DataFrame()
+        if not os.path.isfile(self.filename):
+            return df
+        key = self.key_path(tagname, readtype, ts)
+        where = []
+        if start_time is not None:
+            where.append("index >= start_time")
+        if stop_time is not None:
+            where.append("index <= stop_time")
+        wheretxt = " and ".join(where)
+        with pd.HDFStore(self.filename, mode="r") as f:
+            if key in f:
+                if wheretxt:
+                    df = f.select(key, where=wheretxt)
+                else:
+                    df = f.select(key)
+        return df.sort_index()
+
+    def store_tag_metadata(
+        self, tagname: str, metadata: Dict[str, Union[str, int]]
+    ) -> None:
+        tagname = safe_tagname(tagname)
+        key = f"/metadata/{tagname}"
+        with pd.HDFStore(self.filename, mode="a") as f:
+            if key not in f:
+                f.put(key, pd.DataFrame())
+            origmetadata = {}
+            if "metadata" in f.get_storer(key).attrs:
+                origmetadata = f.get_storer(key).attrs.metadata
+            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
+
+    def fetch_tag_metadata(
+        self, tagname: str, properties: Union[str, List[str]]
+    ) -> Dict[str, Union[str, int]]:
+        res = {}  # type: Dict[str, Union[str, int]]
+        if not os.path.isfile(self.filename):
+            return res
+        tagname = safe_tagname(tagname)
+        key = f"/metadata/{tagname}"
+        if isinstance(properties, str):
+            properties = [properties]
+        with pd.HDFStore(self.filename, mode="r") as f:
+            if key not in f or "metadata" not in f.get_storer(key).attrs:
+                return {}
+            metadata = f.get_storer(key).attrs.metadata
+        for p in properties:
+            if p in metadata.keys():
+                res[p] = metadata.get(p)
+        return res
+
+    def remove(self, filename: str = None) -> None:  # type: ignore[assignment]
+        if not filename:
+            filename = self.filename
+            # self.close()
+        if os.path.isfile(filename):
+            os.unlink(filename)
+
+    def _match_tag(self, key, readtype=None, ts=None, tagname=None):  # type: ignore
+        def readtype_to_str(rt):  # type: ignore
+            return getattr(
+                rt, "name", rt
+            )  # if isinstance(rt, ReaderType) always returns False...?
+
+        def timedelta_to_str(t):  # type: ignore
+            if isinstance(t, pd.Timedelta):
+                return str(int(t.total_seconds()))
+            return t
+
+        key = "/" + key.lstrip("/")  # Ensure absolute path
+        readtype = readtype if isinstance(readtype, list) else [readtype]
+        ts = ts if isinstance(ts, list) else [ts]
+        tagname = tagname if isinstance(tagname, list) else [tagname]
+        readtype = list(map(readtype_to_str, readtype))
+        ts = list(map(timedelta_to_str, ts))
+        if tagname[0] is not None:
+            tagname = list(map(safe_tagname, tagname))
+        # print(f"Readtype: {readtype}, ts: {ts}, tagname: {tagname}")
+        elements = key.split("/")[1:]
+        if len(elements) == 2:
+            elements.insert(1, None)
+        else:
+            elements[1] = int(elements[1][1:])  # Discard the initial s
+        if elements[0] not in readtype and readtype[0] is not None:
+            # print(f"{elements[0]} not in {readtype}")
+            return False
+        if elements[1] not in ts and ts[0] is not None:
+            # print(f"{elements[1]} not in {ts}")
+            return False
+        if elements[2] not in tagname and tagname[0] is not None:
+            # print(f"{elements[2]} not in {tagname}")
+            return False
+        return True
+
+    def delete_key(
+        self,
+        tagname: str = None,  # type: ignore[assignment]
+        readtype: ReaderType = None,  # type: ignore[assignment]
+        ts: Union[int, List[int]] = None,  # type: ignore[assignment]
+    ) -> None:
+        with pd.HDFStore(self.filename) as f:
+            for key in f:
+                if self._match_tag(key, tagname=tagname, readtype=readtype, ts=ts):
+                    f.remove(key)
+
+    def _get_hdfstore(self, mode: str = "r") -> pd.HDFStore:
+        f = pd.HDFStore(self.filename, mode)
+        return f
```

### Comparing `tagreader-3.0.2/tagreader/clients.py` & `tagreader-4.0.1/tagreader/clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,489 +1,539 @@
-import os
-import warnings
-from itertools import groupby
-from operator import itemgetter
-
-import pandas as pd
-
-from .cache import BucketCache, SmartCache
-from .utils import (ReaderType, ensure_datetime_with_tz, find_registry_key,
-                    find_registry_key_from_name, is_windows, logging)
-from .web_handlers import (AspenHandlerWeb, PIHandlerWeb, get_auth_aspen,
-                           get_auth_pi, list_aspenone_sources,
-                           list_piwebapi_sources)
-
-if is_windows():
-    import pyodbc
-
-    from .odbc_handlers import (AspenHandlerODBC, PIHandlerODBC,
-                                list_aspen_sources, list_pi_sources)
-    from .utils import winreg
-
-logging.basicConfig(
-    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
-)
-
-
-def list_sources(imstype, url=None, auth=None, verifySSL=None):
-    accepted_values = ["pi", "aspen", "ip21", "piwebapi", "aspenone"]
-    if not imstype or imstype.lower() not in accepted_values:
-        raise ValueError(f"`imstype` must be one of {accepted_values}")
-
-    if imstype.lower() == "pi":
-        return list_pi_sources()
-    elif imstype.lower() in ["aspen", "ip21"]:
-        return list_aspen_sources()
-    elif imstype.lower() == "piwebapi":
-        if url is None:
-            url = r"https://piwebapi.equinor.com/piwebapi"
-        if auth is None:
-            auth = get_auth_pi()
-        if verifySSL is None:
-            verifySSL = True
-        return list_piwebapi_sources(url=url, auth=auth, verifySSL=verifySSL)
-    elif imstype.lower() == "aspenone":
-        if url is None:
-            url = r"https://aspenone.api.equinor.com"
-        if auth is None:
-            auth = get_auth_aspen()
-        if verifySSL is None:
-            verifySSL = True
-        return list_aspenone_sources(url=url, auth=auth, verifySSL=verifySSL)
-
-
-def get_missing_intervals(df, start_time, stop_time, ts, read_type):
-    if (
-        read_type == ReaderType.RAW
-    ):  # Fixme: How to check for completeness for RAW data?
-        return [[start_time, stop_time]]
-    seconds = int(ts.total_seconds())
-    tvec = pd.date_range(start=start_time, end=stop_time, freq=f"{seconds}s")
-    if len(df) == len(tvec):  # Short-circuit if dataset is complete
-        return []
-    values_in_df = tvec.isin(df.index)
-    missing_intervals = []
-    for k, g in groupby(enumerate(values_in_df), lambda ix: ix[1]):
-        if not k:
-            seq = list(map(itemgetter(0), g))
-            missing_intervals.append(
-                (pd.Timestamp(tvec[seq[0]]), pd.Timestamp(tvec[seq[-1]]))
-            )
-            # Should be unnecessary to fetch overlapping points since get_next_timeslice
-            # ensures start <= t <= stop
-            # missingintervals.append((pd.Timestamp(tvec[seq[0]]),
-            #                          pd.Timestamp(tvec[min(seq[-1]+1, len(tvec)-1)])))
-    return missing_intervals
-
-
-def get_next_timeslice(start_time, stop_time, ts, max_steps=None):
-    if max_steps is None:
-        calc_stop_time = stop_time
-    else:
-        calc_stop_time = start_time + ts * max_steps
-    calc_stop_time = min(stop_time, calc_stop_time)
-    # Ensure we include the last data point.
-    # Discrepancies between Aspen and Pi for +ts
-    # Discrepancies between IMS and cache for e.g. ts.
-    # if calc_stop_time == stop_time:
-    #     calc_stop_time += ts / 2
-    return start_time, calc_stop_time
-
-
-def get_server_address_aspen(datasource):
-    """Data sources are listed under
-    HKEY_CURRENT_USER\\Software\\AspenTech\\ADSA\\Caches\\AspenADSA\\username.
-    For each data source there are multiple keys with Host entries. We start by
-    identifying the correct key to use by locating the UUID for Aspen SQLplus
-    services located under Aspen SQLplus service component. Then we find the
-    host and port based on the path above and the UUID.
-    """
-
-    regkey_clsid = winreg.OpenKey(
-        winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Classes\Wow6432Node\CLSID"
-    )
-    regkey, _ = find_registry_key_from_name(
-        regkey_clsid, "Aspen SQLplus service component"
-    )
-    regkey_implemented_categories = winreg.OpenKeyEx(regkey, "Implemented Categories")
-
-    _, aspen_UUID = find_registry_key_from_name(
-        regkey_implemented_categories, "Aspen SQLplus services"
-    )
-
-    reg_adsa = winreg.OpenKey(
-        winreg.HKEY_CURRENT_USER,
-        r"Software\AspenTech\ADSA\Caches\AspenADSA\\" + os.getlogin(),
-    )
-
-    try:
-        reg_site_key = winreg.OpenKey(reg_adsa, datasource + "\\" + aspen_UUID)
-        host = winreg.QueryValueEx(reg_site_key, "Host")[0]
-        port = int(winreg.QueryValueEx(reg_site_key, "Port")[0])
-        return host, port
-    except FileNotFoundError:
-        return None
-
-
-def get_server_address_pi(datasource):
-    """
-    PI data sources are listed under
-    HKEY_LOCAL_MACHINE\\Software\\Wow6432Node\\PISystem\\PI-SDK\\x.x\\ServerHandles or
-    \\Software\\PISystem\\PI-SDK\\x.x\\ServerHandles.
-
-    :param datasource: Name of data source
-    :return: host, port
-    :type: tuple(string, int)
-    """
-    try:
-        reg_key = winreg.OpenKey(
-            winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Wow6432Node\PISystem\PI-SDK"
-        )
-        reg_key_handles = find_registry_key(reg_key, "ServerHandles")
-        reg_site_key = find_registry_key(reg_key_handles, datasource)
-        if reg_site_key is None:
-            reg_key = winreg.OpenKey(
-                winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\PISystem\PI-SDK"
-            )
-            reg_key_handles = find_registry_key(reg_key, "ServerHandles")
-            reg_site_key = find_registry_key(reg_key_handles, datasource)
-        if reg_site_key is not None:
-            host = winreg.QueryValueEx(reg_site_key, "path")[0]
-            port = int(winreg.QueryValueEx(reg_site_key, "port")[0])
-            return host, port
-    except FileNotFoundError:
-        return None
-
-
-def get_handler(
-    imstype,
-    datasource,
-    url=None,
-    host=None,
-    port=None,
-    options={},
-    verifySSL=None,
-    auth=None,
-):
-    accepted_imstypes = ["pi", "aspen", "ip21", "piwebapi", "aspenone"]
-
-    if not imstype or imstype.lower() not in accepted_imstypes:
-        raise ValueError(f"`imstype` must be one of {accepted_imstypes}")
-
-    if imstype.lower() == "pi":
-        if not is_windows():
-            raise RuntimeError(
-                "ODBC drivers not available for non-Windows environments. "
-                "Try Web API ('piwebapi') instead."
-            )
-        if "PI ODBC Driver" not in pyodbc.drivers():
-            raise RuntimeError(
-                "No PI ODBC driver detected. "
-                "Either switch to Web API ('piwebapi') or install appropriate driver."
-            )
-        if host is None:
-            hostport = get_server_address_pi(datasource)
-            if not hostport:
-                raise ValueError(
-                    f"Unable to locate data source '{datasource}'."
-                    "Do you have correct permissions?"
-                )
-            host, port = hostport
-        if port is None:
-            port = 5450
-        return PIHandlerODBC(host=host, port=port, options=options)
-
-    if imstype.lower() in ["aspen", "ip21"]:
-        if not is_windows():
-            raise RuntimeError(
-                "ODBC drivers not available for non-Windows environments. "
-                "Try Web API ('aspenone') instead."
-            )
-        if "AspenTech SQLplus" not in pyodbc.drivers():
-            raise RuntimeError(
-                "No Aspen SQLplus ODBC driver detected. "
-                "Either switch to Web API ('aspenone') or install appropriate driver."
-            )
-        if host is None:
-            hostport = get_server_address_aspen(datasource)
-            if not hostport:
-                raise ValueError(
-                    f"Unable to locate data source '{datasource}'."
-                    "Do you have correct permissions?"
-                )
-            host, port = hostport
-        if port is None:
-            port = 10014
-        return AspenHandlerODBC(host=host, port=port, options=options)
-
-    if imstype.lower() == "piwebapi":
-        return PIHandlerWeb(
-            url=url,
-            datasource=datasource,
-            options=options,
-            verifySSL=verifySSL,
-            auth=auth,
-        )
-
-    if imstype.lower() in ["aspenone"]:
-        return AspenHandlerWeb(
-            datasource=datasource,
-            url=url,
-            options=options,
-            verifySSL=verifySSL,
-            auth=auth,
-        )
-
-
-class IMSClient:
-    def __init__(
-        self,
-        datasource,
-        imstype=None,
-        tz="Europe/Oslo",
-        url=None,
-        host=None,
-        port=None,
-        handler_options={},
-        verifySSL=None,
-        auth=None,
-    ):
-        self.handler = None
-        self.datasource = datasource.lower()  # FIXME
-        self.tz = tz
-        self.handler = get_handler(
-            imstype,
-            datasource,
-            url=url,
-            host=host,
-            port=port,
-            options=handler_options,
-            verifySSL=verifySSL,
-            auth=auth,
-        )
-        self.cache = SmartCache(datasource)
-
-    def connect(self):
-        self.handler.connect()
-
-    def search_tag(self, tag=None, desc=None):
-        warnings.warn("This function is deprecated. Please call 'search()' instead")
-        return self.search(tag=tag, desc=desc)
-
-    def search(self, tag=None, desc=None):
-        return self.handler.search(tag, desc)
-
-    def _get_metadata(self, tag):
-        return self.handler._get_tag_metadata(tag)
-
-    def _read_single_tag(
-        self, tag, start_time, stop_time, ts, read_type, get_status, cache=None
-    ):
-        if read_type == ReaderType.SNAPSHOT:
-            metadata = self._get_metadata(tag)
-            df = self.handler.read_tag(
-                tag, start_time, stop_time, ts, read_type, metadata, get_status
-            )
-        else:
-            stepped = False
-            missing_intervals = [(start_time, stop_time)]
-            df = pd.DataFrame()
-
-            if (
-                isinstance(cache, SmartCache)
-                and read_type != ReaderType.RAW
-                and not get_status
-            ):
-                time_slice = get_next_timeslice(start_time, stop_time, ts)
-                df = cache.fetch(
-                    tag,
-                    readtype=read_type,
-                    ts=ts,
-                    start_time=time_slice[0],
-                    stop_time=time_slice[1],
-                )
-                missing_intervals = get_missing_intervals(
-                    df, start_time, stop_time, ts, read_type
-                )
-                if not missing_intervals:
-                    return df.tz_convert(self.tz).sort_index()
-            elif isinstance(cache, BucketCache):
-                df = cache.fetch(
-                    tag,
-                    readtype=read_type,
-                    ts=ts,
-                    stepped=stepped,
-                    status=get_status,
-                    starttime=start_time,
-                    endtime=stop_time,
-                )
-                missing_intervals = cache.get_missing_intervals(
-                    tag,
-                    readtype=read_type,
-                    ts=ts,
-                    stepped=stepped,
-                    status=get_status,
-                    starttime=start_time,
-                    endtime=stop_time,
-                )
-                if not missing_intervals:
-                    return df.tz_convert(self.tz).sort_index()
-
-            metadata = self._get_metadata(tag)
-            frames = [df]
-            for (start, stop) in missing_intervals:
-                while True:
-                    df = self.handler.read_tag(
-                        tag, start, stop, ts, read_type, metadata, get_status
-                    )
-                    if len(df.index) > 0:
-                        if (
-                            cache is not None
-                            and read_type
-                            not in [
-                                ReaderType.SNAPSHOT,
-                                ReaderType.RAW,
-                            ]
-                            and not get_status
-                        ):
-                            cache.store(df, read_type, ts)
-                    frames.append(df)
-                    if len(df) < self.handler._max_rows:
-                        break
-                    start = df.index[-1]
-                # if read_type != ReaderType.RAW:
-                #     time_slice = [start, start]
-                #     while time_slice[1] < stop:
-                #         time_slice = get_next_timeslice(
-                #             time_slice[1], stop, ts, self.handler._max_rows
-                #         )
-                #         df = self.handler.read_tag(
-                #             tag, time_slice[0], time_slice[1], ts, read_type, metadata
-                #         )
-                #         if len(df.index) > 0:
-                #             if cache is not None and read_type != ReaderType.RAW:
-                #                 cache.store(df, read_type, ts)
-                #             frames.append(df)
-
-            # df = pd.concat(frames, verify_integrity=True)
-            df = pd.concat(frames)
-            # read_type INT leads to overlapping values after concatenating
-            # due to both start time and end time included.
-            # Aggregate read_types (should) align perfectly and don't
-            # (shouldn't) need deduplication.
-            df = df[~df.index.duplicated(keep="first")]  # Deduplicate on index
-        df = df.tz_convert(self.tz).sort_index()
-        df = df.rename(columns={"value": tag})
-        return df
-
-    def get_units(self, tags):
-        if isinstance(tags, str):
-            tags = [tags]
-        units = {}
-        for tag in tags:
-            if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tag, "unit")
-                if "unit" in r:
-                    units[tag] = r["unit"]
-            if tag not in units:
-                unit = self.handler._get_tag_unit(tag)
-                if self.cache is not None and unit is not None:
-                    self.cache.store_tag_metadata(tag, {"unit": unit})
-                units[tag] = unit
-        return units
-
-    def get_descriptions(self, tags):
-        if isinstance(tags, str):
-            tags = [tags]
-        descriptions = {}
-        for tag in tags:
-            if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tag, "description")
-                if "description" in r:
-                    descriptions[tag] = r["description"]
-            if tag not in descriptions:
-                desc = self.handler._get_tag_description(tag)
-                if self.cache is not None and desc is not None:
-                    self.cache.store_tag_metadata(tag, {"description": desc})
-                descriptions[tag] = desc
-        return descriptions
-
-    def read_tags(self, tags, start_time, stop_time, ts, read_type=ReaderType.INT):
-        warnings.warn(
-            (
-                "This function has been renamed to read() and is deprecated. "
-                "Please call 'read()' instead"
-            )
-        )
-        return self.read(
-            tags=tags,
-            start_time=start_time,
-            end_time=stop_time,
-            ts=ts,
-            read_type=read_type,
-            get_status=False,
-        )
-
-    def read(
-        self,
-        tags,
-        start_time=None,
-        end_time=None,
-        ts=60,
-        read_type=ReaderType.INT,
-        get_status=False,
-    ):
-        """Reads values for the specified [tags] from the IMS server for the
-        time interval from [start_time] to [stop_time] in intervals [ts].
-
-        The interval [ts] can be specified as pd.Timedelta or as an integer,
-        in which case it will be interpreted as seconds.
-
-        Default value for [read_type] is ReaderType.INT, which interpolates
-        the raw data.
-        All possible values for read_type are defined in the ReaderType class,
-        which can be imported as follows:
-            from utils import ReaderType
-
-        Values for ReaderType.* that should work for all handlers are:
-            INT, RAW, MIN, MAX, RNG, AVG, VAR, STD and SNAPSHOT
-        """
-        if isinstance(tags, str):
-            tags = [tags]
-        if read_type in [ReaderType.RAW, ReaderType.SNAPSHOT] and len(tags) > 1:
-            raise RuntimeError(
-                "Unable to read raw/sampled data for multiple tags since they don't "
-                "share time vector. Read one at a time."
-            )
-        if read_type != ReaderType.SNAPSHOT:
-            start_time = ensure_datetime_with_tz(start_time, tz=self.tz)
-        if end_time:
-            end_time = ensure_datetime_with_tz(end_time, tz=self.tz)
-        if not isinstance(ts, pd.Timedelta):
-            ts = pd.Timedelta(ts, unit="s")
-
-        cols = []
-        for tag in tags:
-            cols.append(
-                self._read_single_tag(
-                    tag,
-                    start_time,
-                    end_time,
-                    ts,
-                    read_type,
-                    get_status,
-                    cache=self.cache,
-                )
-            )
-        return pd.concat(cols, axis=1)
-
-    def query_sql(self, query: str, parse: bool = True):
-        """[summary]
-        Args:
-            query (str): [description]
-            parse (bool, optional): Whether to attempt to parse query return
-                                    value as table. Defaults to True.
-        Returns:
-            Union[pd.DataFrame, pyodbc.Cursor, str]: Return value
-        """
-        df_or_cursor = self.handler.query_sql(query=query, parse=parse)
-        return df_or_cursor
+import os
+import warnings
+from itertools import groupby
+from operator import itemgetter
+
+import pandas as pd
+
+from .cache import BucketCache, SmartCache
+from .utils import (
+    ReaderType,
+    ensure_datetime_with_tz,
+    find_registry_key,
+    find_registry_key_from_name,
+    is_windows,
+    logging,
+)
+from .web_handlers import (
+    AspenHandlerWeb,
+    PIHandlerWeb,
+    get_auth_aspen,
+    get_auth_pi,
+    get_url_aspen,
+    get_url_pi,
+    list_aspenone_sources,
+    list_piwebapi_sources,
+)
+
+if is_windows():
+    import pyodbc
+
+    from .odbc_handlers import (
+        AspenHandlerODBC,
+        PIHandlerODBC,
+        list_aspen_sources,
+        list_pi_sources,
+    )
+    from .utils import winreg
+
+logging.basicConfig(
+    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
+)
+
+
+class DuplicateTagsWarning(UserWarning):
+    pass
+
+
+warnings.simplefilter("always", DuplicateTagsWarning)
+
+
+def list_sources(imstype, url=None, auth=None, verifySSL=None):
+    accepted_values = ["piwebapi", "aspenone"]
+    win_accepted_values = ["pi", "aspen", "ip21"]
+    if is_windows():
+        accepted_values.extend(win_accepted_values)
+
+    if imstype is None or imstype.lower() not in accepted_values:
+        import platform
+
+        raise ValueError(
+            f"Input `imstype` must be one of {accepted_values} when called from {platform.system()} environment."
+        )
+
+    if imstype.lower() == "pi":
+        return list_pi_sources()
+    elif imstype.lower() in ["aspen", "ip21"]:
+        return list_aspen_sources()
+    elif imstype.lower() == "piwebapi":
+        if auth is None:
+            auth = get_auth_pi()
+        if verifySSL is None:
+            verifySSL = True
+        return list_piwebapi_sources(url=url, auth=auth, verifySSL=verifySSL)
+    elif imstype.lower() == "aspenone":
+        if auth is None:
+            auth = get_auth_aspen()
+        if verifySSL is None:
+            verifySSL = True
+        return list_aspenone_sources(url=url, auth=auth, verifySSL=verifySSL)
+
+
+def get_missing_intervals(df, start_time, stop_time, ts, read_type):
+    if (
+        read_type == ReaderType.RAW
+    ):  # Fixme: How to check for completeness for RAW data?
+        return [[start_time, stop_time]]
+    seconds = int(ts.total_seconds())
+    tvec = pd.date_range(start=start_time, end=stop_time, freq=f"{seconds}s")
+    if len(df) == len(tvec):  # Short-circuit if dataset is complete
+        return []
+    values_in_df = tvec.isin(df.index)
+    missing_intervals = []
+    for k, g in groupby(enumerate(values_in_df), lambda ix: ix[1]):
+        if not k:
+            seq = list(map(itemgetter(0), g))
+            missing_intervals.append(
+                (pd.Timestamp(tvec[seq[0]]), pd.Timestamp(tvec[seq[-1]]))
+            )
+            # Should be unnecessary to fetch overlapping points since get_next_timeslice
+            # ensures start <= t <= stop
+            # missingintervals.append((pd.Timestamp(tvec[seq[0]]),
+            #                          pd.Timestamp(tvec[min(seq[-1]+1, len(tvec)-1)])))
+    return missing_intervals
+
+
+def get_next_timeslice(start_time, stop_time, ts, max_steps=None):
+    if max_steps is None:
+        calc_stop_time = stop_time
+    else:
+        calc_stop_time = start_time + ts * max_steps
+    calc_stop_time = min(stop_time, calc_stop_time)
+    # Ensure we include the last data point.
+    # Discrepancies between Aspen and Pi for +ts
+    # Discrepancies between IMS and cache for e.g. ts.
+    # if calc_stop_time == stop_time:
+    #     calc_stop_time += ts / 2
+    return start_time, calc_stop_time
+
+
+def get_server_address_aspen(datasource):
+    """Data sources are listed under
+    HKEY_CURRENT_USER\\Software\\AspenTech\\ADSA\\Caches\\AspenADSA\\username.
+    For each data source there are multiple keys with Host entries. We start by
+    identifying the correct key to use by locating the UUID for Aspen SQLplus
+    services located under Aspen SQLplus service component. Then we find the
+    host and port based on the path above and the UUID.
+    """
+
+    if not is_windows():
+        return None
+
+    regkey_clsid = winreg.OpenKey(
+        winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Classes\Wow6432Node\CLSID"
+    )
+    regkey, _ = find_registry_key_from_name(
+        regkey_clsid, "Aspen SQLplus service component"
+    )
+    regkey_implemented_categories = winreg.OpenKeyEx(regkey, "Implemented Categories")
+
+    _, aspen_UUID = find_registry_key_from_name(
+        regkey_implemented_categories, "Aspen SQLplus services"
+    )
+
+    reg_adsa = winreg.OpenKey(
+        winreg.HKEY_CURRENT_USER,
+        r"Software\AspenTech\ADSA\Caches\AspenADSA\\" + os.getlogin(),
+    )
+
+    try:
+        reg_site_key = winreg.OpenKey(reg_adsa, datasource + "\\" + aspen_UUID)
+        host = winreg.QueryValueEx(reg_site_key, "Host")[0]
+        port = int(winreg.QueryValueEx(reg_site_key, "Port")[0])
+        return host, port
+    except FileNotFoundError:
+        return None
+
+
+def get_server_address_pi(datasource):
+    """
+    PI data sources are listed under
+    HKEY_LOCAL_MACHINE\\Software\\Wow6432Node\\PISystem\\PI-SDK\\x.x\\ServerHandles or
+    \\Software\\PISystem\\PI-SDK\\x.x\\ServerHandles.
+
+    :param datasource: Name of data source
+    :return: host, port
+    :type: tuple(string, int)
+    """
+
+    if not is_windows():
+        return None
+
+    try:
+        reg_key = winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Wow6432Node\PISystem\PI-SDK"
+        )
+        reg_key_handles = find_registry_key(reg_key, "ServerHandles")
+        reg_site_key = find_registry_key(reg_key_handles, datasource)
+        if reg_site_key is None:
+            reg_key = winreg.OpenKey(
+                winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\PISystem\PI-SDK"
+            )
+            reg_key_handles = find_registry_key(reg_key, "ServerHandles")
+            reg_site_key = find_registry_key(reg_key_handles, datasource)
+        if reg_site_key is not None:
+            host = winreg.QueryValueEx(reg_site_key, "path")[0]
+            port = int(winreg.QueryValueEx(reg_site_key, "port")[0])
+            return host, port
+    except FileNotFoundError:
+        return None
+
+
+def get_handler(
+    imstype,
+    datasource,
+    url=None,
+    host=None,
+    port=None,
+    options={},
+    verifySSL=None,
+    auth=None,
+):
+    if imstype is None:
+        if datasource in list_aspenone_sources():
+            imstype = "aspenone"
+        elif datasource in list_piwebapi_sources():
+            imstype = "piwebapi"
+
+    accepted_imstypes = ["pi", "aspen", "ip21", "piwebapi", "aspenone"]
+
+    if not imstype or imstype.lower() not in accepted_imstypes:
+        raise ValueError(f"`imstype` must be one of {accepted_imstypes}")
+
+    if imstype.lower() == "pi":
+        if not is_windows():
+            raise RuntimeError(
+                "ODBC drivers not available for non-Windows environments. "
+                "Try Web API ('piwebapi') instead."
+            )
+        if "PI ODBC Driver" not in pyodbc.drivers():
+            raise RuntimeError(
+                "No PI ODBC driver detected. "
+                "Either switch to Web API ('piwebapi') or install appropriate driver."
+            )
+        if host is None:
+            hostport = get_server_address_pi(datasource)
+            if not hostport:
+                raise ValueError(
+                    f"Unable to locate data source '{datasource}'."
+                    "Do you have correct permissions?"
+                )
+            host, port = hostport
+        if port is None:
+            port = 5450
+        return PIHandlerODBC(host=host, port=port, options=options)
+
+    if imstype.lower() in ["aspen", "ip21"]:
+        if not is_windows():
+            raise RuntimeError(
+                "ODBC drivers not available for non-Windows environments. "
+                "Try Web API ('aspenone') instead."
+            )
+        if "AspenTech SQLplus" not in pyodbc.drivers():
+            raise RuntimeError(
+                "No Aspen SQLplus ODBC driver detected. "
+                "Either switch to Web API ('aspenone') or install appropriate driver."
+            )
+        if host is None:
+            hostport = get_server_address_aspen(datasource)
+            if not hostport:
+                raise ValueError(
+                    f"Unable to locate data source '{datasource}'."
+                    "Do you have correct permissions?"
+                )
+            host, port = hostport
+        if port is None:
+            port = 10014
+        return AspenHandlerODBC(host=host, port=port, options=options)
+
+    if imstype.lower() == "piwebapi":
+        return PIHandlerWeb(
+            url=url,
+            datasource=datasource,
+            options=options,
+            verifySSL=verifySSL,
+            auth=auth,
+        )
+
+    if imstype.lower() in ["aspenone"]:
+        return AspenHandlerWeb(
+            datasource=datasource,
+            url=url,
+            options=options,
+            verifySSL=verifySSL,
+            auth=auth,
+        )
+
+
+class IMSClient:
+    def __init__(
+        self,
+        datasource,
+        imstype=None,
+        tz="Europe/Oslo",
+        url=None,
+        host=None,
+        port=None,
+        handler_options={},
+        verifySSL=None,
+        auth=None,
+    ):
+        self.handler = None
+        self.datasource = datasource.lower()  # FIXME
+        self.tz = tz
+        self.handler = get_handler(
+            imstype,
+            datasource,
+            url=url,
+            host=host,
+            port=port,
+            options=handler_options,
+            verifySSL=verifySSL,
+            auth=auth,
+        )
+        self.cache = SmartCache(datasource)
+
+    def connect(self):
+        self.handler.connect()
+
+    def search_tag(self, tag=None, desc=None):
+        warnings.warn("This function is deprecated. Please call 'search()' instead")
+        return self.search(tag=tag, desc=desc)
+
+    def search(self, tag=None, desc=None):
+        return self.handler.search(tag, desc)
+
+    def _get_metadata(self, tag):
+        return self.handler._get_tag_metadata(tag)
+
+    def _read_single_tag(
+        self, tag, start_time, stop_time, ts, read_type, get_status, cache=None
+    ):
+        if read_type == ReaderType.SNAPSHOT:
+            metadata = self._get_metadata(tag)
+            df = self.handler.read_tag(
+                tag, start_time, stop_time, ts, read_type, metadata, get_status
+            )
+        else:
+            stepped = False
+            missing_intervals = [(start_time, stop_time)]
+            df = pd.DataFrame()
+
+            if (
+                isinstance(cache, SmartCache)
+                and read_type != ReaderType.RAW
+                and not get_status
+            ):
+                time_slice = get_next_timeslice(start_time, stop_time, ts)
+                df = cache.fetch(
+                    tag,
+                    readtype=read_type,
+                    ts=ts,
+                    start_time=time_slice[0],
+                    stop_time=time_slice[1],
+                )
+                missing_intervals = get_missing_intervals(
+                    df, start_time, stop_time, ts, read_type
+                )
+                if not missing_intervals:
+                    return df.tz_convert(self.tz).sort_index()
+            elif isinstance(cache, BucketCache):
+                df = cache.fetch(
+                    tag,
+                    readtype=read_type,
+                    ts=ts,
+                    stepped=stepped,
+                    status=get_status,
+                    starttime=start_time,
+                    endtime=stop_time,
+                )
+                missing_intervals = cache.get_missing_intervals(
+                    tag,
+                    readtype=read_type,
+                    ts=ts,
+                    stepped=stepped,
+                    status=get_status,
+                    starttime=start_time,
+                    endtime=stop_time,
+                )
+                if not missing_intervals:
+                    return df.tz_convert(self.tz).sort_index()
+
+            metadata = self._get_metadata(tag)
+            frames = [df]
+            for start, stop in missing_intervals:
+                while True:
+                    df = self.handler.read_tag(
+                        tag, start, stop, ts, read_type, metadata, get_status
+                    )
+                    if len(df.index) > 0:
+                        if (
+                            cache is not None
+                            and read_type
+                            not in [
+                                ReaderType.SNAPSHOT,
+                                ReaderType.RAW,
+                            ]
+                            and not get_status
+                        ):
+                            cache.store(df, read_type, ts)
+                    frames.append(df)
+                    if len(df) < self.handler._max_rows:
+                        break
+                    start = df.index[-1]
+                # if read_type != ReaderType.RAW:
+                #     time_slice = [start, start]
+                #     while time_slice[1] < stop:
+                #         time_slice = get_next_timeslice(
+                #             time_slice[1], stop, ts, self.handler._max_rows
+                #         )
+                #         df = self.handler.read_tag(
+                #             tag, time_slice[0], time_slice[1], ts, read_type, metadata
+                #         )
+                #         if len(df.index) > 0:
+                #             if cache is not None and read_type != ReaderType.RAW:
+                #                 cache.store(df, read_type, ts)
+                #             frames.append(df)
+
+            # df = pd.concat(frames, verify_integrity=True)
+            df = pd.concat(frames)
+            # read_type INT leads to overlapping values after concatenating
+            # due to both start time and end time included.
+            # Aggregate read_types (should) align perfectly and don't
+            # (shouldn't) need deduplication.
+            df = df[~df.index.duplicated(keep="first")]  # Deduplicate on index
+        df = df.tz_convert(self.tz).sort_index()
+        df = df.rename(columns={"value": tag})
+        return df
+
+    def get_units(self, tags):
+        if isinstance(tags, str):
+            tags = [tags]
+        units = {}
+        for tag in tags:
+            if self.cache is not None:
+                r = self.cache.fetch_tag_metadata(tag, "unit")
+                if "unit" in r:
+                    units[tag] = r["unit"]
+            if tag not in units:
+                unit = self.handler._get_tag_unit(tag)
+                if self.cache is not None and unit is not None:
+                    self.cache.store_tag_metadata(tag, {"unit": unit})
+                units[tag] = unit
+        return units
+
+    def get_descriptions(self, tags):
+        if isinstance(tags, str):
+            tags = [tags]
+        descriptions = {}
+        for tag in tags:
+            if self.cache is not None:
+                r = self.cache.fetch_tag_metadata(tag, "description")
+                if "description" in r:
+                    descriptions[tag] = r["description"]
+            if tag not in descriptions:
+                desc = self.handler._get_tag_description(tag)
+                if self.cache is not None and desc is not None:
+                    self.cache.store_tag_metadata(tag, {"description": desc})
+                descriptions[tag] = desc
+        return descriptions
+
+    def read_tags(self, tags, start_time, stop_time, ts, read_type=ReaderType.INT):
+        warnings.warn(
+            (
+                "This function has been renamed to read() and is deprecated. "
+                "Please call 'read()' instead"
+            )
+        )
+        return self.read(
+            tags=tags,
+            start_time=start_time,
+            end_time=stop_time,
+            ts=ts,
+            read_type=read_type,
+            get_status=False,
+        )
+
+    def read(
+        self,
+        tags,
+        start_time=None,
+        end_time=None,
+        ts=60,
+        read_type=ReaderType.INT,
+        get_status=False,
+    ):
+        """Reads values for the specified [tags] from the IMS server for the
+        time interval from [start_time] to [stop_time] in intervals [ts].
+
+        The interval [ts] can be specified as pd.Timedelta or as an integer,
+        in which case it will be interpreted as seconds.
+
+        Default value for [read_type] is ReaderType.INT, which interpolates
+        the raw data.
+        All possible values for read_type are defined in the ReaderType class,
+        which can be imported as follows:
+            from utils import ReaderType
+
+        Values for ReaderType.* that should work for all handlers are:
+            INT, RAW, MIN, MAX, RNG, AVG, VAR, STD and SNAPSHOT
+        """
+
+        if isinstance(tags, str):
+            tags = [tags]
+        if read_type in [ReaderType.RAW, ReaderType.SNAPSHOT] and len(tags) > 1:
+            raise RuntimeError(
+                "Unable to read raw/sampled data for multiple tags since they don't "
+                "share time vector. Read one at a time."
+            )
+        if read_type != ReaderType.SNAPSHOT:
+            start_time = ensure_datetime_with_tz(start_time, tz=self.tz)
+        if end_time:
+            end_time = ensure_datetime_with_tz(end_time, tz=self.tz)
+        if not isinstance(ts, pd.Timedelta):
+            ts = pd.Timedelta(ts, unit="s")
+
+        oldtags = tags
+        tags = list(dict.fromkeys(tags))
+        if len(oldtags) > len(tags):
+            duplicates = set([x for n, x in enumerate(oldtags) if x in oldtags[:n]])
+            warnings.warn(
+                f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}",
+                DuplicateTagsWarning,
+            )
+        cols = []
+        for tag in tags:
+            cols.append(
+                self._read_single_tag(
+                    tag,
+                    start_time,
+                    end_time,
+                    ts,
+                    read_type,
+                    get_status,
+                    cache=self.cache,
+                )
+            )
+        return pd.concat(cols, axis=1)
+
+    def query_sql(self, query: str, parse: bool = True):
+        """[summary]
+        Args:
+            query (str): [description]
+            parse (bool, optional): Whether to attempt to parse query return
+                                    value as table. Defaults to True.
+        Returns:
+            Union[pd.DataFrame, pyodbc.Cursor, str]: Return value
+        """
+        df_or_cursor = self.handler.query_sql(query=query, parse=parse)
+        return df_or_cursor
```

### Comparing `tagreader-3.0.2/tagreader/utils.py` & `tagreader-4.0.1/tagreader/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,233 +1,244 @@
-import enum
-import logging
-import platform
-import warnings
-
-import pandas as pd
-import pytz
-
-
-def is_windows() -> bool:
-    return platform.system() == "Windows"
-
-
-def is_mac() -> bool:
-    return platform.system() == "Darwin"
-
-
-def is_linux() -> bool:
-    return platform.system() == "Linux"
-
-
-if is_windows():
-    import winreg
-
-
-if is_mac():
-    import socket
-    import subprocess
-
-
-def find_registry_key(base_key, search_key_name):
-    search_key_name = search_key_name.lower()
-    if base_key is not None:
-        num_keys, _, _ = winreg.QueryInfoKey(base_key)
-        for i in range(0, num_keys):
-            key_name = winreg.EnumKey(base_key, i)
-            if key_name.lower() == search_key_name:
-                return winreg.OpenKey(base_key, key_name)
-            else:
-                key = find_registry_key(
-                    winreg.OpenKey(base_key, key_name), search_key_name
-                )
-            if key is not None:
-                return key
-    return None
-
-
-def find_registry_key_from_name(base_key, search_key_name):
-    search_key_name = search_key_name.lower()
-    num_keys, _, _ = winreg.QueryInfoKey(base_key)
-    key = key_string = None
-    for i in range(0, num_keys):
-        try:
-            key_string = winreg.EnumKey(base_key, i)
-            key = winreg.OpenKey(base_key, key_string)
-            _, num_vals, _ = winreg.QueryInfoKey(key)
-            if num_vals > 0:
-                (_, key_name, _) = winreg.EnumValue(key, 0)
-                if str(key_name).lower() == search_key_name:
-                    break
-        except Exception as err:
-            logging.error("{}: {}".format(i, err))
-    return key, key_string
-
-
-def ensure_datetime_with_tz(date_stamp, tz="Europe/Oslo"):
-    if isinstance(date_stamp, str):
-        date_stamp = pd.to_datetime(date_stamp, dayfirst=True)
-
-    if not date_stamp.tzinfo:
-        date_stamp = pytz.timezone(tz).localize(date_stamp)
-
-    return date_stamp
-
-
-def urljoin(*args):
-    """Joins components of URL. Ensures slashes are inserted or removed where
-    needed, and does not strip trailing slash of last element.
-
-    Arguments:
-        str
-    Returns:
-        str -- Generated URL
-    """
-    trailing_slash = "/" if args[-1].endswith("/") else ""
-    return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
-
-
-class ReaderType(enum.IntEnum):
-    """Enumerates available types of data to read.
-
-    For members with more than one name per value, the first member (the
-    original) needs to be untouched since it may be used as back-reference
-    (specifically for cache hierarchies).
-    """
-
-    RAW = SAMPLED = ACTUAL = enum.auto()  # Raw sampled data
-    SHAPEPRESERVING = BESTFIT = enum.auto()  # Minimum data points for preserving shape
-    INT = INTERPOLATE = INTERPOLATED = enum.auto()  # Interpolated data
-    MIN = MINIMUM = enum.auto()  # Min value
-    MAX = MAXIMUM = enum.auto()  # Max value
-    AVG = AVERAGE = AVERAGED = enum.auto()  # Averaged data
-    VAR = VARIANCE = enum.auto()  # Variance of data
-    STD = STDDEV = enum.auto()  # Standard deviation of data
-    RNG = RANGE = enum.auto()  # Range of data
-    COUNT = enum.auto()  # Number of data points
-    GOOD = enum.auto()  # Number of good data points
-    BAD = NOTGOOD = enum.auto()  # Number of not good data points
-    TOTAL = enum.auto()  # Number of total data
-    SUM = enum.auto()  # Sum of data
-    SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
-
-
-def add_statoil_root_certificate(noisy=True):
-    """This is a utility function for Equinor employees on Equinor managed machines.
-
-    The function searches for the Statoil Root certificate in the
-    cert store and imports it to the cacert bundle. Does nothing if not
-    running on Equinor host.
-
-    This needs to be repeated after updating the cacert module.
-
-    Returns:
-        bool: True if function completes successfully
-    """
-    import hashlib
-    import ssl
-
-    import certifi
-
-    STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
-
-    found = False
-
-    if is_linux():
-        return True
-    elif is_windows():
-        if noisy:
-            print("Scanning CA certs in Windows cert store", end="")
-        for cert in ssl.enum_certificates("CA"):
-            if noisy:
-                print(".", end="")
-            der = cert[0]
-            if hashlib.sha1(der).hexdigest() == STATOIL_ROOT_PEM_HASH:
-                found = True
-                if noisy:
-                    print(" found it!")
-                break
-    elif is_mac():
-        import subprocess
-        macos_ca_certs = subprocess.run(["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-Z"],
-                                        stdout=subprocess.PIPE).stdout
-
-        if STATOIL_ROOT_PEM_HASH.upper() in str(macos_ca_certs).upper():
-            c = get_macos_statoil_certificates()
-            for cert in c:
-                if hashlib.sha1(cert).hexdigest() == STATOIL_ROOT_PEM_HASH:
-                    der = cert
-                    found = True
-                    break
-
-    if found:
-        pem = ssl.DER_cert_to_PEM_cert(der)
-        if pem in certifi.contents():
-            if noisy:
-                print("Certificate already exists in certifi store. Nothing to do.")
-        else:
-            if noisy:
-                print("Writing certificate to certifi store.")
-            cafile = certifi.where()
-            with open(cafile, "ab") as f:
-                f.write(bytes(pem, "ascii"))
-            if noisy:
-                print("Completed")
-    else:
-        warnings.warn("Unable to locate root certificate on this host.")
-
-    return found
-
-
-def get_macos_statoil_certificates():
-    import ssl
-    import tempfile
-
-    ctx = ssl.create_default_context()
-    macos_ca_certs = subprocess.run(
-        ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-p"], stdout=subprocess.PIPE).stdout
-    with tempfile.NamedTemporaryFile('w+b') as tmp_file:
-        tmp_file.write(macos_ca_certs)
-        ctx.load_verify_locations(tmp_file.name)
-
-    return ctx.get_ca_certs(binary_form=True)
-
-
-def is_equinor() -> bool:
-    """Determines whether code is running on an Equinor host
-
-    If Windows host:
-    Finds host's domain in Windows Registry at
-    HKLM\\SYSTEM\\ControlSet001\\Services\\Tcpip\\Parameters\\Domain
-    If mac os host:
-    Finds statoil.net as AD hostname in certificates
-    If Linux host:
-    Checks whether statoil.no is search domain
-
-    Returns:
-        bool: True if Equinor
-    """
-    if is_windows():
-        with winreg.OpenKey(
-            winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\ControlSet001\Services\Tcpip\Parameters"
-        ) as key:
-            domain = winreg.QueryValueEx(key, "Domain")
-        if "statoil" in domain[0]:
-            return True
-    elif is_mac():
-        s = subprocess.run(
-            ["security", "find-certificate", "-a", "-c" "client.statoil.net"], stdout=subprocess.PIPE).stdout
-
-        host = socket.gethostname()
-
-        if host + ".client.statoil.net" in str(s):
-            return True
-        elif "client.statoil.net" in host and host in str(s):
-            return True
-    elif is_linux():
-        with open("/etc/resolv.conf", "r") as f:
-            if "statoil.no" in f.read():
-                return True
-    else:
-        raise OSError(
-            f"Unsupported system: {platform.system()}. Please report this as an issue.")
-    return False
+import enum
+import logging
+import platform
+import warnings
+
+import pandas as pd
+import pytz
+
+
+def is_windows() -> bool:
+    return platform.system() == "Windows"
+
+
+def is_mac() -> bool:
+    return platform.system() == "Darwin"
+
+
+def is_linux() -> bool:
+    return platform.system() == "Linux"
+
+
+if is_windows():
+    import winreg
+
+
+if is_mac():
+    import socket
+    import subprocess
+
+
+def find_registry_key(base_key, search_key_name):
+    search_key_name = search_key_name.lower()
+    if base_key is not None:
+        num_keys, _, _ = winreg.QueryInfoKey(base_key)
+        for i in range(0, num_keys):
+            key_name = winreg.EnumKey(base_key, i)
+            if key_name.lower() == search_key_name:
+                return winreg.OpenKey(base_key, key_name)
+            else:
+                key = find_registry_key(
+                    winreg.OpenKey(base_key, key_name), search_key_name
+                )
+            if key is not None:
+                return key
+    return None
+
+
+def find_registry_key_from_name(base_key, search_key_name):
+    search_key_name = search_key_name.lower()
+    num_keys, _, _ = winreg.QueryInfoKey(base_key)
+    key = key_string = None
+    for i in range(0, num_keys):
+        try:
+            key_string = winreg.EnumKey(base_key, i)
+            key = winreg.OpenKey(base_key, key_string)
+            _, num_vals, _ = winreg.QueryInfoKey(key)
+            if num_vals > 0:
+                (_, key_name, _) = winreg.EnumValue(key, 0)
+                if str(key_name).lower() == search_key_name:
+                    break
+        except Exception as err:
+            logging.error("{}: {}".format(i, err))
+    return key, key_string
+
+
+def ensure_datetime_with_tz(date_stamp, tz="Europe/Oslo"):
+    if isinstance(date_stamp, str):
+        try:
+            date_stamp = pd.to_datetime(date_stamp, format="ISO8601")
+        except ValueError:
+            date_stamp = pd.to_datetime(date_stamp, dayfirst=True)
+
+    if not date_stamp.tzinfo:
+        date_stamp = pytz.timezone(tz).localize(date_stamp)
+
+    return date_stamp
+
+
+def urljoin(*args):
+    """Joins components of URL. Ensures slashes are inserted or removed where
+    needed, and does not strip trailing slash of last element.
+
+    Arguments:
+        str
+    Returns:
+        str -- Generated URL
+    """
+    trailing_slash = "/" if args[-1].endswith("/") else ""
+    return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
+
+
+class ReaderType(enum.IntEnum):
+    """Enumerates available types of data to read.
+
+    For members with more than one name per value, the first member (the
+    original) needs to be untouched since it may be used as back-reference
+    (specifically for cache hierarchies).
+    """
+
+    RAW = SAMPLED = ACTUAL = enum.auto()  # Raw sampled data
+    SHAPEPRESERVING = BESTFIT = enum.auto()  # Minimum data points for preserving shape
+    INT = INTERPOLATE = INTERPOLATED = enum.auto()  # Interpolated data
+    MIN = MINIMUM = enum.auto()  # Min value
+    MAX = MAXIMUM = enum.auto()  # Max value
+    AVG = AVERAGE = AVERAGED = enum.auto()  # Averaged data
+    VAR = VARIANCE = enum.auto()  # Variance of data
+    STD = STDDEV = enum.auto()  # Standard deviation of data
+    RNG = RANGE = enum.auto()  # Range of data
+    COUNT = enum.auto()  # Number of data points
+    GOOD = enum.auto()  # Number of good data points
+    BAD = NOTGOOD = enum.auto()  # Number of not good data points
+    TOTAL = enum.auto()  # Number of total data
+    SUM = enum.auto()  # Sum of data
+    SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
+
+
+def add_statoil_root_certificate(noisy=True):
+    """This is a utility function for Equinor employees on Equinor managed machines.
+
+    The function searches for the Statoil Root certificate in the
+    cert store and imports it to the cacert bundle. Does nothing if not
+    running on Equinor host.
+
+    This needs to be repeated after updating the cacert module.
+
+    Returns:
+        bool: True if function completes successfully
+    """
+    import hashlib
+    import ssl
+
+    import certifi
+
+    STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
+
+    found = False
+
+    if is_linux():
+        return True
+    elif is_windows():
+        if noisy:
+            print("Scanning CA certs in Windows cert store", end="")
+        for cert in ssl.enum_certificates("CA"):
+            if noisy:
+                print(".", end="")
+            der = cert[0]
+            if hashlib.sha1(der).hexdigest() == STATOIL_ROOT_PEM_HASH:
+                found = True
+                if noisy:
+                    print(" found it!")
+                break
+    elif is_mac():
+        import subprocess
+
+        macos_ca_certs = subprocess.run(
+            ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-Z"],
+            stdout=subprocess.PIPE,
+        ).stdout
+
+        if STATOIL_ROOT_PEM_HASH.upper() in str(macos_ca_certs).upper():
+            c = get_macos_statoil_certificates()
+            for cert in c:
+                if hashlib.sha1(cert).hexdigest() == STATOIL_ROOT_PEM_HASH:
+                    der = cert
+                    found = True
+                    break
+
+    if found:
+        pem = ssl.DER_cert_to_PEM_cert(der)
+        if pem in certifi.contents():
+            if noisy:
+                print("Certificate already exists in certifi store. Nothing to do.")
+        else:
+            if noisy:
+                print("Writing certificate to certifi store.")
+            cafile = certifi.where()
+            with open(cafile, "ab") as f:
+                f.write(bytes(pem, "ascii"))
+            if noisy:
+                print("Completed")
+    else:
+        warnings.warn("Unable to locate root certificate on this host.")
+
+    return found
+
+
+def get_macos_statoil_certificates():
+    import ssl
+    import tempfile
+
+    ctx = ssl.create_default_context()
+    macos_ca_certs = subprocess.run(
+        ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-p"],
+        stdout=subprocess.PIPE,
+    ).stdout
+    with tempfile.NamedTemporaryFile("w+b") as tmp_file:
+        tmp_file.write(macos_ca_certs)
+        ctx.load_verify_locations(tmp_file.name)
+
+    return ctx.get_ca_certs(binary_form=True)
+
+
+def is_equinor() -> bool:
+    """Determines whether code is running on an Equinor host
+
+    If Windows host:
+    Finds host's domain in Windows Registry at
+    HKLM\\SYSTEM\\ControlSet001\\Services\\Tcpip\\Parameters\\Domain
+    If mac os host:
+    Finds statoil.net as AD hostname in certificates
+    If Linux host:
+    Checks whether statoil.no is search domain
+
+    Returns:
+        bool: True if Equinor
+    """
+    if is_windows():
+        with winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\ControlSet001\Services\Tcpip\Parameters"
+        ) as key:
+            domain = winreg.QueryValueEx(key, "Domain")
+        if "statoil" in domain[0]:
+            return True
+    elif is_mac():
+        s = subprocess.run(
+            ["security", "find-certificate", "-a", "-c" "client.statoil.net"],
+            stdout=subprocess.PIPE,
+        ).stdout
+
+        host = socket.gethostname()
+
+        if host + ".client.statoil.net" in str(s):
+            return True
+        elif "client.statoil.net" in host and host in str(s):
+            return True
+    elif is_linux():
+        with open("/etc/resolv.conf", "r") as f:
+            if "statoil.no" in f.read():
+                return True
+    else:
+        raise OSError(
+            f"Unsupported system: {platform.system()}. Please report this as an issue."
+        )
+    return False
```

### Comparing `tagreader-3.0.2/tagreader/web_handlers.py` & `tagreader-4.0.1/tagreader/web_handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,923 +1,936 @@
-import datetime
-import re
-import urllib
-import warnings
-from typing import Union
-
-import numpy as np
-import pandas as pd
-import pytz
-import requests
-from requests_kerberos import OPTIONAL, HTTPKerberosAuth
-
-from .utils import ReaderType, is_mac, is_windows, logging, urljoin
-
-# Requests will use simplejson if it has been installed, so handle both errors here
-try:
-    from simplejson.errors import JSONDecodeError
-except ImportError:
-    from json.decoder import JSONDecodeError
-
-logging.basicConfig(
-    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
-)
-
-
-def get_verifySSL():
-    if is_windows() or is_mac():
-        return True
-    return "/etc/ssl/certs/ca-bundle.trust.crt"
-
-
-def get_auth_pi():
-    return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
-
-
-def get_auth_aspen():
-    return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
-
-
-def list_aspenone_sources(
-    url=r"https://aspenone.api.equinor.com",
-    auth=None,
-    verifySSL=None,
-):
-    if auth is None:
-        auth = get_auth_aspen()
-
-    if verifySSL is False:
-        requests.packages.urllib3.disable_warnings(
-            requests.packages.urllib3.exceptions.InsecureRequestWarning
-        )
-    elif verifySSL is None:
-        verifySSL = get_verifySSL()
-
-    url_ = urljoin(url, "DataSources")
-    params = {"service": "ProcessData", "allQuotes": 1}
-
-    res = requests.get(url_, params=params, auth=auth, verify=verifySSL)
-    if res.status_code == 200:
-        source_list = [r["n"] for r in res.json()["data"] if r["t"] == "IP21"]
-        return source_list
-    elif res.status_code == 404:
-        print("Not found")
-    elif res.status_code == 401:
-        print("Not authorized")
-    res.raise_for_status()
-
-
-def list_piwebapi_sources(
-    url=r"https://piwebapi.equinor.com/piwebapi",
-    auth=None,
-    verifySSL=None,
-):
-    if auth is None:
-        auth = get_auth_pi()
-
-    if verifySSL is False:
-        requests.packages.urllib3.disable_warnings(
-            requests.packages.urllib3.exceptions.InsecureRequestWarning
-        )
-    elif verifySSL is None:
-        verifySSL = get_verifySSL()
-
-    url_ = urljoin(url, "dataservers")
-    res = requests.get(url_, auth=auth, verify=verifySSL)
-    if res.status_code == 200:
-        source_list = [r["Name"] for r in res.json()["Items"]]
-        return source_list
-    elif res.status_code == 404:
-        print("Not found")
-    elif res.status_code == 401:
-        print("Not authorized")
-    res.raise_for_status()
-
-
-class AspenHandlerWeb:
-    def __init__(
-        self,
-        datasource=None,
-        url=None,
-        auth=None,
-        verifySSL=None,
-        options={},
-    ):
-        self._max_rows = options.get("max_rows", 100000)
-        if url is None:
-            url = r"https://aspenone.api.equinor.com"
-        self.datasource = datasource
-        self.base_url = url
-        self.session = requests.Session()
-        self.session.auth = auth if auth is not None else get_auth_aspen()
-        if verifySSL is False:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
-        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
-        self._connection_string = ""  # Used for raw SQL queries
-
-    @staticmethod
-    def generate_connection_string(host, *_, **__):
-        raise NotImplementedError
-
-    @staticmethod
-    def generate_search_query(tag=None, desc=None, datasource=None):
-        if not datasource:
-            raise ValueError("Data source is required argument")
-        # Aspen Web API expects single space instead of consecutive spaces.
-        tag = " ".join(tag.split())
-        params = {"datasource": datasource, "tag": tag, "max": 100, "getTrendable": 0}
-        return params
-
-    def generate_read_query(
-        self,
-        tagname,
-        mapname,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-    ):
-        # Maxpoints is used for Actual (raw) and Bestfit (shapepreserving).
-        # Probably need to handle this in another way at some point
-        maxpoints = self._max_rows
-        stepped = 0
-        outsiders = 0
-
-        rt = {
-            ReaderType.RAW: 0,
-            ReaderType.SHAPEPRESERVING: 2,
-            ReaderType.INT: 1,
-            ReaderType.MIN: 14,
-            ReaderType.MAX: 13,
-            ReaderType.AVG: 12,
-            ReaderType.VAR: 18,
-            ReaderType.STD: 17,
-            ReaderType.RNG: 15,
-            ReaderType.COUNT: -1,
-            ReaderType.GOOD: 11,
-            ReaderType.BAD: 10,
-            ReaderType.TOTAL: -1,
-            ReaderType.SUM: 16,
-            ReaderType.SNAPSHOT: -1,
-        }.get(read_type, -1)
-
-        if read_type == ReaderType.SNAPSHOT:
-            if stop_time is not None:
-                use_current = 0
-                end_time = int(stop_time.timestamp()) * 1000
-            else:
-                use_current = 1
-                end_time = 0
-
-            query = f'<Q f="d" allQuotes="1" rt="{end_time}" uc="{use_current}">'
-        else:
-            query = '<Q f="d" allQuotes="1">'
-
-        query += "<Tag>" f"<N><![CDATA[{tagname}]]></N>"
-
-        if mapname:
-            query += f"<M><![CDATA[{mapname}]]></M>"
-
-        query += f"<D><![CDATA[{self.datasource}]]></D>" "<F><![CDATA[VAL]]></F>"
-
-        if read_type == ReaderType.SNAPSHOT:
-            query += "<VS>1</VS>"
-        else:
-            query += (
-                "<HF>0</HF>"  # History format: 0=Raw, 1=RecordAsString
-                f"<St>{int(start_time.timestamp())*1000}</St>"
-                f"<Et>{int(stop_time.timestamp())*1000}</Et>"
-                f"<RT>{rt}</RT>"
-            )
-        if read_type in [ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
-            query += f"<X>{maxpoints}</X>"
-        if read_type not in [ReaderType.INT, ReaderType.SNAPSHOT]:
-            query += f"<O>{outsiders}</O>"
-        if read_type not in [ReaderType.RAW]:
-            query += f"<S>{stepped}</S>"
-        if read_type not in [
-            ReaderType.RAW,
-            ReaderType.SHAPEPRESERVING,
-            ReaderType.SNAPSHOT,
-        ]:
-            query += (
-                f"<P>{int(sample_time.total_seconds())}</P>"
-                "<PU>3</PU>"  # Period Unit: 0=day, 1=hour, 2=min, 3=sec
-            )
-        if read_type not in [
-            ReaderType.RAW,
-            ReaderType.SHAPEPRESERVING,
-            ReaderType.INT,
-            ReaderType.SNAPSHOT,
-        ]:
-            query += (
-                # Method: 0=integral, 2=value, 3=integral complete, 4=value complete
-                # Value averages all actual values inside interval
-                # Integral time-weighs values
-                "<AM>0</AM>"
-                "<AS>0</AS>"  # Start: 0=Start of day, 1=Start of time
-                "<AA>0</AA>"  # Anchor: 0=Begin, 1=Middle, 2=End
-                # TODO: Unify anchor selection among all handlers
-                "<DSA>0</DSA>"  # DS Adjust: 0=False, 1=True
-            )
-        query += "</Tag></Q>"
-
-        return query
-
-    def verify_connection(self, datasource):
-        """Connects to the URL and verifies that the provided data source exists.
-
-        :param datasource: Data source to look for
-        :type datasource: String
-        :raises ConnectionError: If connection fails
-        :return: True if datasource exists, False if not.
-        :rtype: Bool
-        """
-        url = urljoin(self.base_url, "Datasources")
-        params = {"service": "ProcessData", "allQuotes": 1}
-        if not self.session.verify:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
-
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-        j = res.json()
-        for item in j["data"]:
-            if item["n"] == datasource:
-                return True
-        return False
-
-    def connect(self):
-        try:
-            self.verify_connection(self.datasource)
-        except requests.ConnectionError:
-            raise ConnectionError(
-                f"Not able to connect to {self.base_url}. Check network connection."
-            ) from None
-
-    @staticmethod
-    def split_tagmap(tagmap):
-        return tuple(tagmap.split(";") if ";" in tagmap else (tagmap, None))
-
-    def generate_get_unit_query(self, tag):
-        tagname, _ = self.split_tagmap(tag)
-        parts = [
-            '<Q allQuotes="1" attributeData="1">',
-            "<Tag>",
-            f"<N><![CDATA[{tagname}]]></N>",
-            "<T>0</T>",  # What is this?
-            f"<G><![CDATA[{tagname}]]></G>",
-            f"<D><![CDATA[{self.datasource}]]></D>",
-            "<AL>",
-            # Units only or MAP_Units only: ATCAI=>3. Both: Units=psig, MAP_Units=3
-            "<A>Units</A>",
-            "<A>MAP_Units</A>",
-            "<VS>0</VS>",  # What is this?
-            "</AL>",
-            "</Tag>",
-            "</Q>",
-        ]
-        return "".join(parts)
-
-    def generate_get_map_query(self, tagname):
-        parts = [
-            '<Q allQuotes="1" categoryInfo="1">',
-            "<Tag>",
-            f"<N><![CDATA[{tagname}]]></N>",
-            "<T>0</T>",  # What is this?
-            f"<G><![CDATA[{tagname}]]></G>",
-            f"<D><![CDATA[{self.datasource}]]></D>",
-            "</Tag>",
-            "</Q>",
-        ]
-        return "".join(parts)
-
-    def _get_maps(self, tagname):
-        params = self.generate_get_map_query(tagname)
-        url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-        j = res.json()
-
-        if "tags" not in j["data"]:
-            return {}
-
-        ret = {}
-        for item in j["data"]["tags"][0]["categories"][0]["ta"]:
-            ret[item["m"]] = True if item["d"] == "True" else False
-        return ret
-
-    def _get_default_mapname(self, tagname):
-        (tagname, _) = self.split_tagmap(tagname)
-        allmaps = self._get_maps(tagname)
-        for k, v in allmaps.items():
-            if v:
-                return k
-
-    def search(self, tag=None, desc=None):
-        if tag is None:
-            raise ValueError("Tag is a required argument")
-
-        tag = tag.replace("%", "*") if isinstance(tag, str) else None
-        # Prepare for regex
-        desc = desc.replace("%", "*") if isinstance(desc, str) else None
-        desc = desc.replace("*", ".*") if isinstance(desc, str) else None
-
-        params = self.generate_search_query(tag, desc, self.datasource)
-        # Ensure space is encoded as "%20" instead of default "+" and leave asterisks
-        # unencoded. Otherwise searches for tags containing spaces break, as do wildcard
-        # searches.
-        encoded_params = urllib.parse.urlencode(
-            params, safe="*", quote_via=urllib.parse.quote
-        )
-        url = urljoin(self.base_url, "Browse?")
-        url += encoded_params
-        res = self.session.get(url)
-
-        res.raise_for_status()
-        j = res.json()
-
-        if "tags" not in j["data"]:
-            return []
-
-        ret = []
-        for item in j["data"]["tags"]:
-            tagname = item["t"]
-            description = self._get_tag_description(tagname)
-            ret.append((tagname, description))
-
-        if not desc:
-            return ret
-
-        r = re.compile(desc)
-        ret = [x for x in ret if r.search(x[1])]
-        return ret
-
-    def _get_tag_metadata(self, tag):
-        return {}  # FIXME
-
-    def _get_tag_unit(self, tag):
-        query = self.generate_get_unit_query(tag)
-        url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=query)
-        res.raise_for_status()
-        j = res.json()
-        try:
-            attrdata = j["data"]["tags"][0]["attrData"]
-        except Exception:
-            print(f"Error. I got this: {j}")
-            raise KeyError
-        unit = ""
-        for a in attrdata:
-            if a["g"] == "Units":
-                unit = a["samples"][0]["v"]
-                break
-        return unit
-
-    def generate_get_description_query(self, tag):
-        tagname, _ = self.split_tagmap(tag)
-        parts = [
-            '<Q allQuotes="1" attributeData="1">',
-            "<Tag>",
-            f"<N><![CDATA[{tagname}]]></N>",
-            "<T>0</T>",  # What is this?
-            f"<G><![CDATA[{tagname}]]></G>",
-            f"<D><![CDATA[{self.datasource}]]></D>",
-            "<AL>",
-            "<A>DSCR</A>",
-            "<VS>0</VS>",  # What is this?
-            "</AL>",
-            "</Tag>",
-            "</Q>",
-        ]
-        return "".join(parts)
-
-    def _get_tag_description(self, tag):
-        query = self.generate_get_description_query(tag)
-        url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=query)
-        res.raise_for_status()
-        j = res.json()
-        try:
-            desc = j["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
-        except Exception:
-            desc = ""
-        return desc
-
-    def read_tag(
-        self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
-    ):
-        if read_type not in [
-            ReaderType.INT,
-            ReaderType.MIN,
-            ReaderType.MAX,
-            ReaderType.RNG,
-            ReaderType.AVG,
-            ReaderType.VAR,
-            ReaderType.STD,
-            ReaderType.SNAPSHOT,
-            ReaderType.RAW,
-        ]:
-            raise NotImplementedError
-
-        if read_type == ReaderType.SNAPSHOT:
-            url = urljoin(self.base_url, "Attribute")
-        else:
-            url = urljoin(self.base_url, "History")
-
-        # Actual and bestfit read types allow specifying maxpoints.
-        # Aggregate reads limit to 10 000 points and issue a moredata-token.
-        # TODO: May need to look into using this later - most likely more
-        # efficient than creating new query starting at previous stoptime.
-        # Interpolated reads return error message if more than 100 000 points,
-        # so we need to limit the range. Note -1 because INT normally includes
-        # both start and end time.
-        if read_type == ReaderType.INT:
-            stop_time = min(stop_time, start_time + sample_time * (self._max_rows - 1))
-
-        tagname, mapname = self.split_tagmap(tag)
-
-        params = self.generate_read_query(
-            tagname, mapname, start_time, stop_time, sample_time, read_type
-        )
-
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-
-        if len(res.text) == 0:  # res.text='' for timestamps in future
-            return pd.DataFrame(columns=[tag])
-
-        try:
-            j = res.json()
-        except JSONDecodeError:
-            # AspenOne sometimes returns completely and utterly invalid -nan.
-            # Since json/simplejson has no mechanism to handle this, we need to
-            # pre-process
-            import json
-
-            txt = res.text.replace('"v":nan', '"v":NaN').replace('"v":-nan', '"v":NaN')
-            j = json.loads(txt)
-
-        if "er" in j["data"][0]["samples"][0]:
-            warnings.warn(j["data"][0]["samples"][0]["es"])
-            return pd.DataFrame(columns=[tag])
-        if get_status:
-            # The "l" field maps 1:1 to ODBC status field values 0, 1, 2, 4, 5, 6
-            df = (
-                pd.DataFrame.from_dict(j["data"][0]["samples"])
-                .drop(labels=["s", "V"], axis="columns")
-                .rename(columns={"t": "Timestamp", "v": "Value", "l": "Status"})
-            )
-        else:
-            df = (
-                pd.DataFrame.from_dict(j["data"][0]["samples"])
-                .drop(labels=["l", "s", "V"], axis="columns")
-                .rename(columns={"t": "Timestamp", "v": "Value"})
-            )
-
-        # Ensure non-numericals like "1.#QNAN" are returned as NaN
-        df["Value"] = pd.to_numeric(df.Value, errors="coerce")
-
-        df["Timestamp"] = pd.to_datetime(df["Timestamp"], unit="ms", origin="unix")
-        df = df.set_index("Timestamp", drop=True).tz_localize("UTC")
-        df.index.name = "time"
-        return df.rename(columns={"Value": tag, "Status": tag + "::status"})
-
-    @staticmethod
-    def generate_sql_query(
-        connection_string=None, datasource=None, query=None, max_rows=100000
-    ):
-        if connection_string is not None:
-            connstr = f'<SQL c="{connection_string}" m="{max_rows}" to="30" s="1">'
-        else:
-            connstr = (
-                f'<SQL t="SQLplus" ds="{datasource}" '
-                'dso="CHARINT=N;CHARFLOAT=N;CHARTIME=N;CONVERTERRORS=N" '
-                f'm="{max_rows}" to="30" s="1">'
-            )
-
-        connstr += f"<![CDATA[{query}]]></SQL>"
-        return connstr
-
-    def initialize_connectionstring(
-        self, host=None, port=10014, connection_string=None
-    ):
-        if connection_string:
-            self._connection_string = connection_string
-        else:
-            self._connection_string = (
-                f"DRIVER=AspenTech SQLPlus;HOST={host};"
-                f"PORT={port};CHARINT=N;CHARFLOAT=N;"
-                "CHARTIME=N;CONVERTERRORS=N"
-            )
-
-    def query_sql(self, query: str, parse: bool = True) -> Union[str, pd.DataFrame]:
-        url = urljoin(self.base_url, "SQL")
-        if self._connection_string is None:
-            params = self.generate_sql_query(
-                datasource=self.datasource, query=query, max_rows=self._max_rows
-            )
-        else:
-            params = self.generate_sql_query(
-                connection_string=self._connection_string,
-                query=query,
-                max_rows=self._max_rows,
-            )
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-        # For now just return result as text regardless of value of parse
-        if parse:
-            raise NotImplementedError(
-                "Use parse=False to receive and handle text result instead"
-            )
-        return res.text
-
-
-class PIHandlerWeb:
-    def __init__(
-        self,
-        url=None,
-        datasource=None,
-        auth=None,
-        verifySSL=None,
-        options={},
-    ):
-        self._max_rows = options.get("max_rows", 10000)
-        if url is None:
-            url = r"https://piwebapi.equinor.com/piwebapi"
-        self.base_url = url
-        self.datasource = datasource
-        self.session = requests.Session()
-        self.session.auth = auth if auth is not None else get_auth_pi()
-        if verifySSL is False:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
-        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
-        self.webidcache = {}
-
-    @staticmethod
-    def _time_to_UTC_string(time):
-        timecast_format_query = "%d-%b-%y %H:%M:%S"
-        if isinstance(time, datetime.datetime):
-            return time.astimezone(pytz.UTC).strftime(timecast_format_query)
-        else:
-            return time.tz_convert("UTC").strftime(timecast_format_query)
-
-    @staticmethod
-    def generate_connection_string(host, *_, **__):
-        raise NotImplementedError
-
-    @staticmethod
-    def escape(s):
-        # https://techsupport.osisoft.com/Documentation/PI-Web-API/help/topics/search-queries.html  # noqa: E501
-        return s.translate(
-            str.maketrans(
-                {
-                    "+": r"\+",
-                    "-": r"\-",
-                    "&": r"\&",
-                    "|": r"\|",
-                    "(": r"\(",
-                    ")": r"\)",
-                    "{": r"\{",
-                    "}": r"\}",
-                    "[": r"\[",
-                    "]": r"\]",
-                    "^": r"\^",
-                    '"': r"\"",
-                    "~": r"\~",
-                    # Do not escape wildcard
-                    # "*": r"\*",
-                    ":": r"\:",
-                    "\\": r"\\",
-                    " ": r"\ ",
-                }
-            )
-        )
-
-    @staticmethod
-    def generate_search_query(tag=None, desc=None, datasource=None):
-        q = []
-        if tag is not None:
-            q.extend([f"name:{PIHandlerWeb.escape(tag)}"])
-        if desc is not None:
-            q.extend([f"description:{PIHandlerWeb.escape(desc)}"])
-        query = " AND ".join(q)
-        params = {"q": f"{query}"}
-
-        if datasource is not None:
-            params["scope"] = f"pi:{datasource}"
-
-        return params
-
-    def generate_read_query(
-        self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
-    ):
-
-        if read_type in [
-            ReaderType.COUNT,
-            ReaderType.GOOD,
-            ReaderType.BAD,
-            ReaderType.TOTAL,
-            ReaderType.SUM,
-            ReaderType.SHAPEPRESERVING,
-        ]:
-            raise NotImplementedError
-
-        webid = tag
-
-        seconds = 0
-        if read_type != ReaderType.SNAPSHOT:
-            seconds = int(sample_time.total_seconds())
-
-        get_action = {
-            ReaderType.INT: "interpolated",
-            ReaderType.RAW: "recorded",
-            ReaderType.SNAPSHOT: "value",
-            ReaderType.SHAPEPRESERVING: "plot",
-        }.get(read_type, "summary")
-
-        url = f"streams/{webid}/{get_action}"
-        params = {}
-
-        if read_type != ReaderType.SNAPSHOT:
-            params["startTime"] = self._time_to_UTC_string(start_time)
-            params["endTime"] = self._time_to_UTC_string(stop_time)
-            params["timeZone"] = "UTC"
-        elif read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            params["time"] = self._time_to_UTC_string(stop_time)
-            params["timeZone"] = "UTC"
-
-        summary_type = {
-            ReaderType.MIN: "Minimum",
-            ReaderType.MAX: "Maximum",
-            ReaderType.AVG: "Average",
-            ReaderType.VAR: "StdDev",
-            ReaderType.STD: "StdDev",
-            ReaderType.RNG: "Range",
-        }.get(read_type, None)
-
-        if ReaderType.INT == read_type:
-            params["interval"] = f"{seconds}s"
-        elif summary_type:
-            params["summaryType"] = summary_type
-            params["summaryDuration"] = f"{seconds}s"
-
-        if self._is_summary(read_type):
-            params["selectedFields"] = "Links;Items.Value.Timestamp;Items.Value.Value"
-            if get_status:
-                params["selectedFields"] += (
-                    ";Items.Value.Good"
-                    ";Items.Value.Questionable"
-                    ";Items.Value.Substituted"
-                )
-        elif read_type in [ReaderType.INT, ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
-            params["selectedFields"] = "Links;Items.Timestamp;Items.Value"
-            if get_status:
-                params[
-                    "selectedFields"
-                ] += ";Items.Good;Items.Questionable;Items.Substituted"
-        elif read_type == ReaderType.SNAPSHOT:
-            params["selectedFields"] = "Timestamp;Value"
-            if get_status:
-                params["selectedFields"] += ";Good;Questionable;Substituted"
-
-        if read_type == ReaderType.RAW:
-            params["maxCount"] = self._max_rows
-
-        return (url, params)
-
-    def verify_connection(self, datasource):
-        """Connects to the URL and verifies that the provided data source exists.
-
-        :param source: Data source to look for
-        :type source: String
-        :raises ConnectionError: If connection fails
-        :return: True if data source exists, False if not.
-        :rtype: Bool
-        """
-        url = urljoin(self.base_url, "dataservers")
-        res = self.session.get(url)
-        res.raise_for_status()
-        j = res.json()
-        for item in j["Items"]:
-            if item["Name"] == datasource:
-                return True
-        return False
-
-    def connect(self):
-        try:
-            self.verify_connection(self.datasource)
-        except requests.ConnectionError:
-            raise ConnectionError(
-                f"Not able to connect to {self.base_url}. Check network connection."
-            ) from None
-
-    def search(self, tag=None, desc=None):
-        params = self.generate_search_query(tag, desc, self.datasource)
-        url = urljoin(self.base_url, "search", "query")
-        done = False
-        ret = []
-        while not done:
-            res = self.session.get(url, params=params)
-
-            res.raise_for_status()
-            j = res.json()
-            for item in j["Items"]:
-                description = item["Description"] if "Description" in item else ""
-                ret.append((item["Name"], description))
-            next_start = int(j["Links"]["Next"].split("=")[-1])
-            if int(j["Links"]["Last"].split("=")[-1]) >= next_start:
-                params["start"] = next_start
-            else:
-                done = True
-        return ret
-
-    def _get_tag_metadata(self, tag):
-        return {}  # FIXME
-
-    def _get_tag_unit(self, tag):
-        webid = self.tag_to_webid(tag)
-        if webid is None:
-            return None
-        url = urljoin(self.base_url, "points", webid)
-        res = self.session.get(url)
-        res.raise_for_status()
-        j = res.json()
-        unit = j["EngineeringUnits"]
-        return unit
-
-    def _get_tag_description(self, tag):
-        webid = self.tag_to_webid(tag)
-        if webid is None:
-            return None
-        url = urljoin(self.base_url, "points", webid)
-        res = self.session.get(url)
-        res.raise_for_status()
-        j = res.json()
-        description = j["Descriptor"]
-        return description
-
-    def tag_to_webid(self, tag):
-        """Given a tag, returns the WebId.
-
-        :param tag: The tag
-        :type tag: str
-        :raises ConnectionError: If connection or query fails
-        :return: WebId
-        :rtype: str
-        """
-        if tag not in self.webidcache:
-            params = self.generate_search_query(tag=tag, datasource=self.datasource)
-            params["fields"] = "name;webid"
-            url = urljoin(self.base_url, "search", "query")
-            res = self.session.get(url, params=params)
-            res.raise_for_status()
-            j = res.json()
-
-            if len(j["Errors"]) > 0:
-                msg = f"Received error from server when searching for WebId for {tag}: {j['Errors']}"  # noqa: E501
-                raise ValueError(msg)
-
-            if len(j["Items"]) > 1:
-                # Compare elements and if same, return the first
-                first = j["Items"][0]
-                for item in j["Items"][1:]:
-                    if item != first:
-                        raise AssertionError(
-                            f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."  # noqa: E501
-                        )
-            elif len(j["Items"]) == 0:
-                warnings.warn(f"Tag {tag} not found")
-                return None
-
-            webid = j["Items"][0]["WebId"]
-            self.webidcache[tag] = webid
-        return self.webidcache[tag]
-
-    @staticmethod
-    def _is_summary(read_type):
-        if read_type in [
-            ReaderType.AVG,
-            ReaderType.MIN,
-            ReaderType.MAX,
-            ReaderType.RNG,
-            ReaderType.STD,
-            ReaderType.VAR,
-        ]:
-            return True
-        return False
-
-    def read_tag(
-        self,
-        tag,
-        start_time=None,
-        stop_time=None,
-        sample_time=None,
-        read_type=ReaderType.INTERPOLATED,
-        metadata=None,
-        get_status=False,
-    ):
-        webid = self.tag_to_webid(tag)
-        if not webid:
-            return pd.DataFrame()
-
-        (url, params) = self.generate_read_query(
-            webid, start_time, stop_time, sample_time, read_type, get_status=get_status
-        )
-        url = urljoin(self.base_url, url)
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-
-        j = res.json()
-        if read_type == ReaderType.SNAPSHOT:
-            df = pd.DataFrame.from_dict([j])
-        else:
-            # Summary (aggregated) data and DigitalSets return Value as dict
-            df = pd.json_normalize(data=j, record_path="Items")
-
-        # Can happen for RAW reads w/o data in interval
-        if df.empty:
-            return df
-
-        # Summary data, digitalset or invalid data
-        if "Value" not in df.columns:
-            # Either digitalset or invalid data. Set invalid to NaN
-            if "Value.Name" in df.columns:
-                df.loc[df["Value.Name"] == "No Data", "Value.Value"] = np.nan
-            # Replaced below replacement test with above when adding get_status
-            # since we should avoid getting Good when get_status == False
-            # Value.Name can also be the name of the digitalset, e.g. "Active"
-            # Alternative: df["Value.IsSystem"] == True since it seems to be False
-            # for digitalsets?
-            #    df.loc[df.Good == False, "Value.Value"] = np.nan  # noqa E712
-            df = df.rename(
-                columns={
-                    "Value.Value": "Value",
-                    "Value.Timestamp": "Timestamp",
-                    "Value.Good": "Good",
-                    "Value.Questionable": "Questionable",
-                    "Value.Substituted": "Substituted",
-                }
-            )
-
-        df = df.filter(["Timestamp", "Value", "Good", "Questionable", "Substituted"])
-
-        try:
-            if read_type == ReaderType.RAW or read_type == ReaderType.SNAPSHOT:
-                # Sub-second timestamps are common
-                df["Timestamp"] = pd.to_datetime(
-                    df["Timestamp"], format="%Y-%m-%dT%H:%M:%S.%fZ", utc=True
-                )
-            else:
-                # Sub-second timestamps are uncommon
-                df["Timestamp"] = pd.to_datetime(
-                    df["Timestamp"], format="%Y-%m-%dT%H:%M:%SZ", utc=True
-                )
-        except ValueError:
-            df["Timestamp"] = pd.to_datetime(df["Timestamp"], utc=True)
-
-        if read_type == ReaderType.VAR:
-            df["Value"] = df["Value"] ** 2
-
-        df = df.set_index("Timestamp", drop=True)
-        df.index.name = "time"
-        # df = df.tz_localize("UTC")
-
-        # Correct weird bug in PI Web API where MAX timestamps end of interval while
-        # all the other summaries stamp start of interval by shifting all timestamps
-        # one interval down.
-        if read_type == ReaderType.MAX and df.index[0] > start_time:
-            df.index = df.index - sample_time
-
-        if get_status:
-            df["Status"] = (
-                # Values are boolean, but no need to do .astype(int)
-                df["Questionable"]
-                + 2 * (1 - df["Good"])
-                + 4 * df["Substituted"]
-            )
-            df = df.drop(columns=["Good", "Questionable", "Substituted"])
-
-        return df.rename(columns={"Value": tag, "Status": tag + "::status"})
-
-    def query_sql(self, query: str, parse: bool = True) -> pd.DataFrame:
-        raise NotImplementedError
+import datetime
+import re
+import urllib
+import warnings
+from typing import Union
+
+import numpy as np
+import pandas as pd
+import pytz
+import requests
+from requests_kerberos import OPTIONAL, HTTPKerberosAuth
+
+from .utils import ReaderType, is_mac, is_windows, logging, urljoin
+
+# Requests will use simplejson if it has been installed, so handle both errors here
+try:
+    from simplejson.errors import JSONDecodeError
+except ImportError:
+    from json.decoder import JSONDecodeError
+
+logging.basicConfig(
+    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
+)
+
+
+def get_verifySSL():
+    if is_windows() or is_mac():
+        return True
+    return "/etc/ssl/certs/ca-bundle.trust.crt"
+
+
+def get_auth_pi():
+    return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
+
+
+def get_url_pi():
+    return r"https://piwebapi.equinor.com/piwebapi"
+
+
+def get_auth_aspen():
+    return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
+
+
+def get_url_aspen():
+    # internal url (redirects to dll)
+    return r"https://aspenone.api.equinor.com"
+
+
+def list_aspenone_sources(url=None, auth=None, verifySSL=None):
+    if url is None:
+        url = get_url_aspen()
+
+    if auth is None:
+        auth = get_auth_aspen()
+
+    if verifySSL is False:
+        requests.packages.urllib3.disable_warnings(
+            requests.packages.urllib3.exceptions.InsecureRequestWarning
+        )
+    elif verifySSL is None:
+        verifySSL = get_verifySSL()
+
+    url_ = urljoin(url, "DataSources")
+    params = {"service": "ProcessData", "allQuotes": 1}
+
+    res = requests.get(url_, params=params, auth=auth, verify=verifySSL)
+    if res.status_code == 200:
+        try:
+            source_list = [r["n"] for r in res.json()["data"] if r["t"] == "IP21"]
+            return source_list
+        except JSONDecodeError:
+            print("Did not return json")
+    elif res.status_code == 404:
+        print("Not found")
+    elif res.status_code == 401:
+        print("Not authorized")
+    res.raise_for_status()
+
+
+def list_piwebapi_sources(url=None, auth=None, verifySSL=None):
+    if url is None:
+        url = get_url_pi()
+
+    if auth is None:
+        auth = get_auth_pi()
+
+    if verifySSL is False:
+        requests.packages.urllib3.disable_warnings(
+            requests.packages.urllib3.exceptions.InsecureRequestWarning
+        )
+    elif verifySSL is None:
+        verifySSL = get_verifySSL()
+
+    url_ = urljoin(url, "dataservers")
+    res = requests.get(url_, auth=auth, verify=verifySSL)
+
+    if res.status_code == 200:
+        try:
+            source_list = [r["Name"] for r in res.json()["Items"]]
+            return source_list
+        except JSONDecodeError:
+            print("Did not return json")
+    elif res.status_code == 404:
+        print("Not found")
+    elif res.status_code == 401:
+        print("Not authorized")
+    res.raise_for_status()
+
+
+class AspenHandlerWeb:
+    def __init__(
+        self,
+        datasource=None,
+        url=None,
+        auth=None,
+        verifySSL=None,
+        options={},
+    ):
+        self._max_rows = options.get("max_rows", 100000)
+        if url is None:
+            url = get_url_aspen()
+        self.datasource = datasource
+        self.base_url = url
+        self.session = requests.Session()
+        self.session.auth = auth if auth is not None else get_auth_aspen()
+        if verifySSL is False:
+            requests.packages.urllib3.disable_warnings(
+                requests.packages.urllib3.exceptions.InsecureRequestWarning
+            )
+        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
+        self._connection_string = ""  # Used for raw SQL queries
+
+    @staticmethod
+    def generate_connection_string(host, *_, **__):
+        raise NotImplementedError
+
+    @staticmethod
+    def generate_search_query(tag=None, desc=None, datasource=None):
+        if not datasource:
+            raise ValueError("Data source is required argument")
+        # Aspen Web API expects single space instead of consecutive spaces.
+        tag = " ".join(tag.split())
+        params = {"datasource": datasource, "tag": tag, "max": 100, "getTrendable": 0}
+        return params
+
+    def generate_read_query(
+        self,
+        tagname,
+        mapname,
+        start_time,
+        stop_time,
+        sample_time,
+        read_type,
+        metadata=None,
+    ):
+        # Maxpoints is used for Actual (raw) and Bestfit (shapepreserving).
+        # Probably need to handle this in another way at some point
+        maxpoints = self._max_rows
+        stepped = 0
+        outsiders = 0
+
+        rt = {
+            ReaderType.RAW: 0,
+            ReaderType.SHAPEPRESERVING: 2,
+            ReaderType.INT: 1,
+            ReaderType.MIN: 14,
+            ReaderType.MAX: 13,
+            ReaderType.AVG: 12,
+            ReaderType.VAR: 18,
+            ReaderType.STD: 17,
+            ReaderType.RNG: 15,
+            ReaderType.COUNT: -1,
+            ReaderType.GOOD: 11,
+            ReaderType.BAD: 10,
+            ReaderType.TOTAL: -1,
+            ReaderType.SUM: 16,
+            ReaderType.SNAPSHOT: -1,
+        }.get(read_type, -1)
+
+        if read_type == ReaderType.SNAPSHOT:
+            if stop_time is not None:
+                use_current = 0
+                end_time = int(stop_time.timestamp()) * 1000
+            else:
+                use_current = 1
+                end_time = 0
+
+            query = f'<Q f="d" allQuotes="1" rt="{end_time}" uc="{use_current}">'
+        else:
+            query = '<Q f="d" allQuotes="1">'
+
+        query += "<Tag>" f"<N><![CDATA[{tagname}]]></N>"
+
+        if mapname:
+            query += f"<M><![CDATA[{mapname}]]></M>"
+
+        query += f"<D><![CDATA[{self.datasource}]]></D>" "<F><![CDATA[VAL]]></F>"
+
+        if read_type == ReaderType.SNAPSHOT:
+            query += "<VS>1</VS>"
+        else:
+            query += (
+                "<HF>0</HF>"  # History format: 0=Raw, 1=RecordAsString
+                f"<St>{int(start_time.timestamp())*1000}</St>"
+                f"<Et>{int(stop_time.timestamp())*1000}</Et>"
+                f"<RT>{rt}</RT>"
+            )
+        if read_type in [ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
+            query += f"<X>{maxpoints}</X>"
+        if read_type not in [ReaderType.INT, ReaderType.SNAPSHOT]:
+            query += f"<O>{outsiders}</O>"
+        if read_type not in [ReaderType.RAW]:
+            query += f"<S>{stepped}</S>"
+        if read_type not in [
+            ReaderType.RAW,
+            ReaderType.SHAPEPRESERVING,
+            ReaderType.SNAPSHOT,
+        ]:
+            query += (
+                f"<P>{int(sample_time.total_seconds())}</P>"
+                "<PU>3</PU>"  # Period Unit: 0=day, 1=hour, 2=min, 3=sec
+            )
+        if read_type not in [
+            ReaderType.RAW,
+            ReaderType.SHAPEPRESERVING,
+            ReaderType.INT,
+            ReaderType.SNAPSHOT,
+        ]:
+            query += (
+                # Method: 0=integral, 2=value, 3=integral complete, 4=value complete
+                # Value averages all actual values inside interval
+                # Integral time-weighs values
+                "<AM>0</AM>"
+                "<AS>0</AS>"  # Start: 0=Start of day, 1=Start of time
+                "<AA>0</AA>"  # Anchor: 0=Begin, 1=Middle, 2=End
+                # TODO: Unify anchor selection among all handlers
+                "<DSA>0</DSA>"  # DS Adjust: 0=False, 1=True
+            )
+        query += "</Tag></Q>"
+
+        return query
+
+    def verify_connection(self, datasource):
+        """Connects to the URL and verifies that the provided data source exists.
+
+        :param datasource: Data source to look for
+        :type datasource: String
+        :raises ConnectionError: If connection fails
+        :return: True if datasource exists, False if not.
+        :rtype: Bool
+        """
+        url = urljoin(self.base_url, "Datasources")
+        params = {"service": "ProcessData", "allQuotes": 1}
+        if not self.session.verify:
+            requests.packages.urllib3.disable_warnings(
+                requests.packages.urllib3.exceptions.InsecureRequestWarning
+            )
+
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+        j = res.json()
+        for item in j["data"]:
+            if item["n"] == datasource:
+                return True
+        return False
+
+    def connect(self):
+        try:
+            self.verify_connection(self.datasource)
+        except requests.ConnectionError:
+            raise ConnectionError(
+                f"Not able to connect to {self.base_url}. Check network connection."
+            ) from None
+
+    @staticmethod
+    def split_tagmap(tagmap):
+        return tuple(tagmap.split(";") if ";" in tagmap else (tagmap, None))
+
+    def generate_get_unit_query(self, tag):
+        tagname, _ = self.split_tagmap(tag)
+        parts = [
+            '<Q allQuotes="1" attributeData="1">',
+            "<Tag>",
+            f"<N><![CDATA[{tagname}]]></N>",
+            "<T>0</T>",  # What is this?
+            f"<G><![CDATA[{tagname}]]></G>",
+            f"<D><![CDATA[{self.datasource}]]></D>",
+            "<AL>",
+            # Units only or MAP_Units only: ATCAI=>3. Both: Units=psig, MAP_Units=3
+            "<A>Units</A>",
+            "<A>MAP_Units</A>",
+            "<VS>0</VS>",  # What is this?
+            "</AL>",
+            "</Tag>",
+            "</Q>",
+        ]
+        return "".join(parts)
+
+    def generate_get_map_query(self, tagname):
+        parts = [
+            '<Q allQuotes="1" categoryInfo="1">',
+            "<Tag>",
+            f"<N><![CDATA[{tagname}]]></N>",
+            "<T>0</T>",  # What is this?
+            f"<G><![CDATA[{tagname}]]></G>",
+            f"<D><![CDATA[{self.datasource}]]></D>",
+            "</Tag>",
+            "</Q>",
+        ]
+        return "".join(parts)
+
+    def _get_maps(self, tagname):
+        params = self.generate_get_map_query(tagname)
+        url = urljoin(self.base_url, "TagInfo")
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+        j = res.json()
+
+        if "tags" not in j["data"]:
+            return {}
+
+        ret = {}
+        for item in j["data"]["tags"][0]["categories"][0]["ta"]:
+            ret[item["m"]] = True if item["d"] == "True" else False
+        return ret
+
+    def _get_default_mapname(self, tagname):
+        (tagname, _) = self.split_tagmap(tagname)
+        allmaps = self._get_maps(tagname)
+        for k, v in allmaps.items():
+            if v:
+                return k
+
+    def search(self, tag=None, desc=None):
+        if tag is None:
+            raise ValueError("Tag is a required argument")
+
+        tag = tag.replace("%", "*") if isinstance(tag, str) else None
+        # Prepare for regex
+        desc = desc.replace("%", "*") if isinstance(desc, str) else None
+        desc = desc.replace("*", ".*") if isinstance(desc, str) else None
+
+        params = self.generate_search_query(tag, desc, self.datasource)
+        # Ensure space is encoded as "%20" instead of default "+" and leave asterisks
+        # unencoded. Otherwise searches for tags containing spaces break, as do wildcard
+        # searches.
+        encoded_params = urllib.parse.urlencode(
+            params, safe="*", quote_via=urllib.parse.quote
+        )
+        url = urljoin(self.base_url, "Browse?")
+        url += encoded_params
+        res = self.session.get(url)
+
+        res.raise_for_status()
+        j = res.json()
+
+        if "tags" not in j["data"]:
+            return []
+
+        ret = []
+        for item in j["data"]["tags"]:
+            tagname = item["t"]
+            description = self._get_tag_description(tagname)
+            ret.append((tagname, description))
+
+        if not desc:
+            return ret
+
+        r = re.compile(desc)
+        ret = [x for x in ret if r.search(x[1])]
+        return ret
+
+    def _get_tag_metadata(self, tag):
+        return {}  # FIXME
+
+    def _get_tag_unit(self, tag):
+        query = self.generate_get_unit_query(tag)
+        url = urljoin(self.base_url, "TagInfo")
+        res = self.session.get(url, params=query)
+        res.raise_for_status()
+        j = res.json()
+        try:
+            attrdata = j["data"]["tags"][0]["attrData"]
+        except Exception:
+            print(f"Error. I got this: {j}")
+            raise KeyError
+        unit = ""
+        for a in attrdata:
+            if a["g"] == "Units":
+                unit = a["samples"][0]["v"]
+                break
+        return unit
+
+    def generate_get_description_query(self, tag):
+        tagname, _ = self.split_tagmap(tag)
+        parts = [
+            '<Q allQuotes="1" attributeData="1">',
+            "<Tag>",
+            f"<N><![CDATA[{tagname}]]></N>",
+            "<T>0</T>",  # What is this?
+            f"<G><![CDATA[{tagname}]]></G>",
+            f"<D><![CDATA[{self.datasource}]]></D>",
+            "<AL>",
+            "<A>DSCR</A>",
+            "<VS>0</VS>",  # What is this?
+            "</AL>",
+            "</Tag>",
+            "</Q>",
+        ]
+        return "".join(parts)
+
+    def _get_tag_description(self, tag):
+        query = self.generate_get_description_query(tag)
+        url = urljoin(self.base_url, "TagInfo")
+        res = self.session.get(url, params=query)
+        res.raise_for_status()
+        j = res.json()
+        try:
+            desc = j["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
+        except Exception:
+            desc = ""
+        return desc
+
+    def read_tag(
+        self,
+        tag,
+        start_time,
+        stop_time,
+        sample_time,
+        read_type,
+        metadata=None,
+        get_status=False,
+    ):
+        if read_type not in [
+            ReaderType.INT,
+            ReaderType.MIN,
+            ReaderType.MAX,
+            ReaderType.RNG,
+            ReaderType.AVG,
+            ReaderType.VAR,
+            ReaderType.STD,
+            ReaderType.SNAPSHOT,
+            ReaderType.RAW,
+        ]:
+            raise NotImplementedError
+
+        if read_type == ReaderType.SNAPSHOT:
+            url = urljoin(self.base_url, "Attribute")
+        else:
+            url = urljoin(self.base_url, "History")
+
+        # Actual and bestfit read types allow specifying maxpoints.
+        # Aggregate reads limit to 10 000 points and issue a moredata-token.
+        # TODO: May need to look into using this later - most likely more
+        # efficient than creating new query starting at previous stoptime.
+        # Interpolated reads return error message if more than 100 000 points,
+        # so we need to limit the range. Note -1 because INT normally includes
+        # both start and end time.
+        if read_type == ReaderType.INT:
+            stop_time = min(stop_time, start_time + sample_time * (self._max_rows - 1))
+
+        tagname, mapname = self.split_tagmap(tag)
+
+        params = self.generate_read_query(
+            tagname, mapname, start_time, stop_time, sample_time, read_type
+        )
+
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+
+        if len(res.text) == 0:  # res.text='' for timestamps in future
+            return pd.DataFrame(columns=[tag])
+
+        try:
+            j = res.json()
+        except JSONDecodeError:
+            # AspenOne sometimes returns completely and utterly invalid -nan.
+            # Since json/simplejson has no mechanism to handle this, we need to
+            # pre-process
+            import json
+
+            txt = res.text.replace('"v":nan', '"v":NaN').replace('"v":-nan', '"v":NaN')
+            j = json.loads(txt)
+
+        if "er" in j["data"][0]["samples"][0]:
+            warnings.warn(j["data"][0]["samples"][0]["es"])
+            return pd.DataFrame(columns=[tag])
+        if get_status:
+            # The "l" field maps 1:1 to ODBC status field values 0, 1, 2, 4, 5, 6
+            df = (
+                pd.DataFrame.from_dict(j["data"][0]["samples"])
+                .drop(labels=["s", "V"], axis="columns")
+                .rename(columns={"t": "Timestamp", "v": "Value", "l": "Status"})
+            )
+        else:
+            df = (
+                pd.DataFrame.from_dict(j["data"][0]["samples"])
+                .drop(labels=["l", "s", "V"], axis="columns")
+                .rename(columns={"t": "Timestamp", "v": "Value"})
+            )
+
+        # Ensure non-numericals like "1.#QNAN" are returned as NaN
+        df["Value"] = pd.to_numeric(df.Value, errors="coerce")
+
+        df["Timestamp"] = pd.to_datetime(df["Timestamp"], unit="ms", origin="unix")
+        df = df.set_index("Timestamp", drop=True).tz_localize("UTC")
+        df.index.name = "time"
+        return df.rename(columns={"Value": tag, "Status": tag + "::status"})
+
+    @staticmethod
+    def generate_sql_query(
+        connection_string=None, datasource=None, query=None, max_rows=100000
+    ):
+        if connection_string is not None:
+            connstr = f'<SQL c="{connection_string}" m="{max_rows}" to="30" s="1">'
+        else:
+            connstr = (
+                f'<SQL t="SQLplus" ds="{datasource}" '
+                'dso="CHARINT=N;CHARFLOAT=N;CHARTIME=N;CONVERTERRORS=N" '
+                f'm="{max_rows}" to="30" s="1">'
+            )
+
+        connstr += f"<![CDATA[{query}]]></SQL>"
+        return connstr
+
+    def initialize_connectionstring(
+        self, host=None, port=10014, connection_string=None
+    ):
+        if connection_string:
+            self._connection_string = connection_string
+        else:
+            self._connection_string = (
+                f"DRIVER=AspenTech SQLPlus;HOST={host};"
+                f"PORT={port};CHARINT=N;CHARFLOAT=N;"
+                "CHARTIME=N;CONVERTERRORS=N"
+            )
+
+    def query_sql(self, query: str, parse: bool = True) -> Union[str, pd.DataFrame]:
+        url = urljoin(self.base_url, "SQL")
+        if self._connection_string is None:
+            params = self.generate_sql_query(
+                datasource=self.datasource, query=query, max_rows=self._max_rows
+            )
+        else:
+            params = self.generate_sql_query(
+                connection_string=self._connection_string,
+                query=query,
+                max_rows=self._max_rows,
+            )
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+        # For now just return result as text regardless of value of parse
+        if parse:
+            raise NotImplementedError(
+                "Use parse=False to receive and handle text result instead"
+            )
+        return res.text
+
+
+class PIHandlerWeb:
+    def __init__(
+        self,
+        url=None,
+        datasource=None,
+        auth=None,
+        verifySSL=None,
+        options={},
+    ):
+        self._max_rows = options.get("max_rows", 10000)
+        if url is None:
+            url = get_url_pi()
+        self.base_url = url
+        self.datasource = datasource
+        self.session = requests.Session()
+        self.session.auth = auth if auth is not None else get_auth_pi()
+        if verifySSL is False:
+            requests.packages.urllib3.disable_warnings(
+                requests.packages.urllib3.exceptions.InsecureRequestWarning
+            )
+        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
+        self.webidcache = {}
+
+    @staticmethod
+    def _time_to_UTC_string(time):
+        timecast_format_query = "%d-%b-%y %H:%M:%S"
+        if isinstance(time, datetime.datetime):
+            return time.astimezone(pytz.UTC).strftime(timecast_format_query)
+        else:
+            return time.tz_convert("UTC").strftime(timecast_format_query)
+
+    @staticmethod
+    def generate_connection_string(host, *_, **__):
+        raise NotImplementedError
+
+    @staticmethod
+    def escape(s):
+        # https://techsupport.osisoft.com/Documentation/PI-Web-API/help/topics/search-queries.html  # noqa: E501
+        return s.translate(
+            str.maketrans(
+                {
+                    "+": r"\+",
+                    "-": r"\-",
+                    "&": r"\&",
+                    "|": r"\|",
+                    "(": r"\(",
+                    ")": r"\)",
+                    "{": r"\{",
+                    "}": r"\}",
+                    "[": r"\[",
+                    "]": r"\]",
+                    "^": r"\^",
+                    '"': r"\"",
+                    "~": r"\~",
+                    # Do not escape wildcard
+                    # "*": r"\*",
+                    ":": r"\:",
+                    "\\": r"\\",
+                    " ": r"\ ",
+                }
+            )
+        )
+
+    @staticmethod
+    def generate_search_query(tag=None, desc=None, datasource=None):
+        q = []
+        if tag is not None:
+            q.extend([f"name:{PIHandlerWeb.escape(tag)}"])
+        if desc is not None:
+            q.extend([f"description:{PIHandlerWeb.escape(desc)}"])
+        query = " AND ".join(q)
+        params = {"q": f"{query}"}
+
+        if datasource is not None:
+            params["scope"] = f"pi:{datasource}"
+
+        return params
+
+    def generate_read_query(
+        self,
+        tag,
+        start_time,
+        stop_time,
+        sample_time,
+        read_type,
+        metadata=None,
+        get_status=False,
+    ):
+        if read_type in [
+            ReaderType.COUNT,
+            ReaderType.GOOD,
+            ReaderType.BAD,
+            ReaderType.TOTAL,
+            ReaderType.SUM,
+            ReaderType.SHAPEPRESERVING,
+        ]:
+            raise NotImplementedError
+
+        webid = tag
+
+        seconds = 0
+        if read_type != ReaderType.SNAPSHOT:
+            seconds = int(sample_time.total_seconds())
+
+        get_action = {
+            ReaderType.INT: "interpolated",
+            ReaderType.RAW: "recorded",
+            ReaderType.SNAPSHOT: "value",
+            ReaderType.SHAPEPRESERVING: "plot",
+        }.get(read_type, "summary")
+
+        url = f"streams/{webid}/{get_action}"
+        params = {}
+
+        if read_type != ReaderType.SNAPSHOT:
+            params["startTime"] = self._time_to_UTC_string(start_time)
+            params["endTime"] = self._time_to_UTC_string(stop_time)
+            params["timeZone"] = "UTC"
+        elif read_type == ReaderType.SNAPSHOT and stop_time is not None:
+            params["time"] = self._time_to_UTC_string(stop_time)
+            params["timeZone"] = "UTC"
+
+        summary_type = {
+            ReaderType.MIN: "Minimum",
+            ReaderType.MAX: "Maximum",
+            ReaderType.AVG: "Average",
+            ReaderType.VAR: "StdDev",
+            ReaderType.STD: "StdDev",
+            ReaderType.RNG: "Range",
+        }.get(read_type, None)
+
+        if ReaderType.INT == read_type:
+            params["interval"] = f"{seconds}s"
+        elif summary_type:
+            params["summaryType"] = summary_type
+            params["summaryDuration"] = f"{seconds}s"
+
+        if self._is_summary(read_type):
+            params["selectedFields"] = "Links;Items.Value.Timestamp;Items.Value.Value"
+            if get_status:
+                params["selectedFields"] += (
+                    ";Items.Value.Good"
+                    ";Items.Value.Questionable"
+                    ";Items.Value.Substituted"
+                )
+        elif read_type in [ReaderType.INT, ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
+            params["selectedFields"] = "Links;Items.Timestamp;Items.Value"
+            if get_status:
+                params[
+                    "selectedFields"
+                ] += ";Items.Good;Items.Questionable;Items.Substituted"
+        elif read_type == ReaderType.SNAPSHOT:
+            params["selectedFields"] = "Timestamp;Value"
+            if get_status:
+                params["selectedFields"] += ";Good;Questionable;Substituted"
+
+        if read_type == ReaderType.RAW:
+            params["maxCount"] = self._max_rows
+
+        return (url, params)
+
+    def verify_connection(self, datasource):
+        """Connects to the URL and verifies that the provided data source exists.
+
+        :param source: Data source to look for
+        :type source: String
+        :raises ConnectionError: If connection fails
+        :return: True if data source exists, False if not.
+        :rtype: Bool
+        """
+        url = urljoin(self.base_url, "dataservers")
+        res = self.session.get(url)
+        res.raise_for_status()
+        j = res.json()
+        for item in j["Items"]:
+            if item["Name"] == datasource:
+                return True
+        return False
+
+    def connect(self):
+        try:
+            self.verify_connection(self.datasource)
+        except requests.ConnectionError:
+            raise ConnectionError(
+                f"Not able to connect to {self.base_url}. Check network connection."
+            ) from None
+
+    def search(self, tag=None, desc=None):
+        params = self.generate_search_query(tag, desc, self.datasource)
+        url = urljoin(self.base_url, "search", "query")
+        done = False
+        ret = []
+        while not done:
+            res = self.session.get(url, params=params)
+
+            res.raise_for_status()
+            j = res.json()
+            for item in j["Items"]:
+                description = item["Description"] if "Description" in item else ""
+                ret.append((item["Name"], description))
+            next_start = int(j["Links"]["Next"].split("=")[-1])
+            if int(j["Links"]["Last"].split("=")[-1]) >= next_start:
+                params["start"] = next_start
+            else:
+                done = True
+        return ret
+
+    def _get_tag_metadata(self, tag):
+        return {}  # FIXME
+
+    def _get_tag_unit(self, tag):
+        webid = self.tag_to_webid(tag)
+        if webid is None:
+            return None
+        url = urljoin(self.base_url, "points", webid)
+        res = self.session.get(url)
+        res.raise_for_status()
+        j = res.json()
+        unit = j["EngineeringUnits"]
+        return unit
+
+    def _get_tag_description(self, tag):
+        webid = self.tag_to_webid(tag)
+        if webid is None:
+            return None
+        url = urljoin(self.base_url, "points", webid)
+        res = self.session.get(url)
+        res.raise_for_status()
+        j = res.json()
+        description = j["Descriptor"]
+        return description
+
+    def tag_to_webid(self, tag):
+        """Given a tag, returns the WebId.
+
+        :param tag: The tag
+        :type tag: str
+        :raises ConnectionError: If connection or query fails
+        :return: WebId
+        :rtype: str
+        """
+        if tag not in self.webidcache:
+            params = self.generate_search_query(tag=tag, datasource=self.datasource)
+            params["fields"] = "name;webid"
+            url = urljoin(self.base_url, "search", "query")
+            res = self.session.get(url, params=params)
+            res.raise_for_status()
+            j = res.json()
+
+            if len(j["Errors"]) > 0:
+                msg = f"Received error from server when searching for WebId for {tag}: {j['Errors']}"  # noqa: E501
+                raise ValueError(msg)
+
+            if len(j["Items"]) > 1:
+                # Compare elements and if same, return the first
+                first = j["Items"][0]
+                for item in j["Items"][1:]:
+                    if item != first:
+                        raise AssertionError(
+                            f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."  # noqa: E501
+                        )
+            elif len(j["Items"]) == 0:
+                warnings.warn(f"Tag {tag} not found")
+                return None
+
+            webid = j["Items"][0]["WebId"]
+            self.webidcache[tag] = webid
+        return self.webidcache[tag]
+
+    @staticmethod
+    def _is_summary(read_type):
+        if read_type in [
+            ReaderType.AVG,
+            ReaderType.MIN,
+            ReaderType.MAX,
+            ReaderType.RNG,
+            ReaderType.STD,
+            ReaderType.VAR,
+        ]:
+            return True
+        return False
+
+    def read_tag(
+        self,
+        tag,
+        start_time=None,
+        stop_time=None,
+        sample_time=None,
+        read_type=ReaderType.INTERPOLATED,
+        metadata=None,
+        get_status=False,
+    ):
+        webid = self.tag_to_webid(tag)
+        if not webid:
+            return pd.DataFrame()
+
+        (url, params) = self.generate_read_query(
+            webid, start_time, stop_time, sample_time, read_type, get_status=get_status
+        )
+        url = urljoin(self.base_url, url)
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+
+        j = res.json()
+        if read_type == ReaderType.SNAPSHOT:
+            df = pd.DataFrame.from_dict([j])
+        else:
+            # Summary (aggregated) data and DigitalSets return Value as dict
+            df = pd.json_normalize(data=j, record_path="Items")
+
+        # Can happen for RAW reads w/o data in interval
+        if df.empty:
+            return df
+
+        # Summary data, digitalset or invalid data
+        if "Value" not in df.columns:
+            # Either digitalset or invalid data. Set invalid to NaN
+            if "Value.Name" in df.columns:
+                df.loc[df["Value.Name"] == "No Data", "Value.Value"] = np.nan
+            # Replaced below replacement test with above when adding get_status
+            # since we should avoid getting Good when get_status == False
+            # Value.Name can also be the name of the digitalset, e.g. "Active"
+            # Alternative: df["Value.IsSystem"] == True since it seems to be False
+            # for digitalsets?
+            #    df.loc[df.Good == False, "Value.Value"] = np.nan  # noqa E712
+            df = df.rename(
+                columns={
+                    "Value.Value": "Value",
+                    "Value.Timestamp": "Timestamp",
+                    "Value.Good": "Good",
+                    "Value.Questionable": "Questionable",
+                    "Value.Substituted": "Substituted",
+                }
+            )
+
+        df = df.filter(["Timestamp", "Value", "Good", "Questionable", "Substituted"])
+
+        try:
+            if read_type == ReaderType.RAW or read_type == ReaderType.SNAPSHOT:
+                # Sub-second timestamps are common
+                df["Timestamp"] = pd.to_datetime(
+                    df["Timestamp"], format="%Y-%m-%dT%H:%M:%S.%fZ", utc=True
+                )
+            else:
+                # Sub-second timestamps are uncommon
+                df["Timestamp"] = pd.to_datetime(
+                    df["Timestamp"], format="%Y-%m-%dT%H:%M:%SZ", utc=True
+                )
+        except ValueError:
+            df["Timestamp"] = pd.to_datetime(df["Timestamp"], utc=True)
+
+        if read_type == ReaderType.VAR:
+            df["Value"] = df["Value"] ** 2
+
+        df = df.set_index("Timestamp", drop=True)
+        df.index.name = "time"
+        # df = df.tz_localize("UTC")
+
+        # Correct weird bug in PI Web API where MAX timestamps end of interval while
+        # all the other summaries stamp start of interval by shifting all timestamps
+        # one interval down.
+        if read_type == ReaderType.MAX and df.index[0] > start_time:
+            df.index = df.index - sample_time
+
+        if get_status:
+            df["Status"] = (
+                # Values are boolean, but no need to do .astype(int)
+                df["Questionable"]
+                + 2 * (1 - df["Good"])
+                + 4 * df["Substituted"]
+            )
+            df = df.drop(columns=["Good", "Questionable", "Substituted"])
+
+        return df.rename(columns={"Value": tag, "Status": tag + "::status"})
+
+    def query_sql(self, query: str, parse: bool = True) -> pd.DataFrame:
+        raise NotImplementedError
```

