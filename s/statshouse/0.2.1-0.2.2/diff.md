# Comparing `tmp/statshouse-0.2.1.tar.gz` & `tmp/statshouse-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statshouse-0.2.1.tar", last modified: Fri Jun  2 11:34:29 2023, max compression
+gzip compressed data, was "statshouse-0.2.2.tar", last modified: Mon Jun  5 13:27:34 2023, max compression
```

## Comparing `statshouse-0.2.1.tar` & `statshouse-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.1/LICENSE
--rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.1/README.md
--rw-r--r--   0        0        0     1083 2023-06-02 11:34:29.307764 statshouse-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-02 11:18:06.879315 statshouse-0.2.1/src/statshouse/__init__.py
--rw-r--r--   0        0        0     3852 2023-06-02 11:17:34.943336 statshouse-0.2.1/src/statshouse/_statshouse.py
--rw-r--r--   0        0        0      195 2023-06-02 11:18:06.879315 statshouse-0.2.1/tests/test_statshouse.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.2/LICENSE
+-rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.2/README.md
+-rw-r--r--   0        0        0     1083 2023-06-05 13:27:34.788701 statshouse-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      138 2023-06-05 13:22:06.791909 statshouse-0.2.2/src/statshouse/__init__.py
+-rw-r--r--   0        0        0     3840 2023-06-05 13:22:06.787909 statshouse-0.2.2/src/statshouse/_statshouse.py
+-rw-r--r--   0        0        0      191 2023-06-05 13:22:06.783909 statshouse-0.2.2/tests/test_statshouse.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.2/PKG-INFO
```

### Comparing `statshouse-0.2.1/LICENSE` & `statshouse-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.1/README.md` & `statshouse-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.1/pyproject.toml` & `statshouse-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "statshouse"
-version = "0.2.1"
+version = "0.2.2"
 description = "StatsHouse client library for Python"
 authors = [
     { name = "Gregory Petrosyan", email = "pgregory@pgregory.net" },
 ]
 dependencies = [
     "msgpack>=1.0.5",
 ]
```

### Comparing `statshouse-0.2.1/src/statshouse/_statshouse.py` & `statshouse-0.2.2/src/statshouse/_statshouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 TAG_HOST = "_h"
 
 T = TypeVar("T")
 OneOrMany = Union[T, Sequence[T]]
 Tags = Union[Tuple[Optional[str], ...], List[Optional[str]], Dict[str, str]]
 
 
-class StatsHouse:
+class Client:
     def __init__(self, addr: str, env: str):
         self._env = env
         if addr:
             p = urllib.parse.urlsplit("//" + addr, "", False)
             self._addr = (p.hostname, p.port)
             self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         else:
@@ -99,29 +99,29 @@
             ),
         }
         if n != 0:
             packet["metrics"][0]["counter"] = float(n)
         self._send(packet, ts)
 
 
-def _init_global() -> StatsHouse:
+def _init_global() -> Client:
     p = argparse.ArgumentParser()
     p.add_argument(
         "--statshouse-addr",
         type=str,
         default=os.getenv("STATSHOUSE_ADDR", DEFAULT_STATSHOUSE_ADDR),
     )
     p.add_argument(
         "--statshouse-env", type=str, default=os.getenv("STATSHOUSE_ENV", "")
     )
 
     args, left = p.parse_known_args(sys.argv)
     sys.argv = sys.argv[:1] + left
 
-    return StatsHouse(addr=args.statshouse_addr, env=args.statshouse_env)
+    return Client(addr=args.statshouse_addr, env=args.statshouse_env)
 
 
 __sh = _init_global()
 
 
 def count(metric: str, tags: Tags, n: Real, *, ts: Real = 0):
     return __sh.count(metric, tags, n, ts=ts)
```

### Comparing `statshouse-0.2.1/PKG-INFO` & `statshouse-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statshouse
-Version: 0.2.1
+Version: 0.2.2
 Summary: StatsHouse client library for Python
 Author-Email: Gregory Petrosyan <pgregory@pgregory.net>
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

