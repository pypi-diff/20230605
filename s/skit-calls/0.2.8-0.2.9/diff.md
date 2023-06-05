# Comparing `tmp/skit-calls-0.2.8.tar.gz` & `tmp/skit-calls-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skit-calls-0.2.8.tar", max compression
+gzip compressed data, was "skit-calls-0.2.9.tar", max compression
```

## Comparing `skit-calls-0.2.8.tar` & `skit-calls-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-04-25 13:29:12.353259 skit-calls-0.2.8/LICENSE
--rw-r--r--   0        0        0      822 2022-04-25 13:31:03.933807 skit-calls-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/__init__.py
--rw-r--r--   0        0        0     4419 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/calls.py
--rw-r--r--   0        0        0     7082 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/cli.py
--rw-r--r--   0        0        0     3725 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/constants.py
--rw-r--r--   0        0        0        0 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/data/__init__.py
--rw-r--r--   0        0        0      996 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/data/db.py
--rw-r--r--   0        0        0     5633 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/data/model.py
--rw-r--r--   0        0        0     1582 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/data/mutators.py
--rw-r--r--   0        0        0     3114 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/data/query.py
--rw-r--r--   0        0        0     1857 2022-04-25 13:29:12.357259 skit-calls-0.2.8/skit_calls/utils.py
--rw-r--r--   0        0        0     1032 2022-04-25 13:31:20.267753 skit-calls-0.2.8/setup.py
--rw-r--r--   0        0        0      901 2022-04-25 13:31:20.268108 skit-calls-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-05-04 12:13:01.259447 skit-calls-0.2.9/LICENSE
+-rw-r--r--   0        0        0      867 2022-05-04 12:15:46.997626 skit-calls-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/__init__.py
+-rw-r--r--   0        0        0     4901 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/calls.py
+-rw-r--r--   0        0        0     7506 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/cli.py
+-rw-r--r--   0        0        0     3781 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/constants.py
+-rw-r--r--   0        0        0        0 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/data/__init__.py
+-rw-r--r--   0        0        0      996 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/data/db.py
+-rw-r--r--   0        0        0     5761 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/data/model.py
+-rw-r--r--   0        0        0     1582 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/data/mutators.py
+-rw-r--r--   0        0        0     3476 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/data/query.py
+-rw-r--r--   0        0        0     1857 2022-05-04 12:13:01.263447 skit-calls-0.2.9/skit_calls/utils.py
+-rw-r--r--   0        0        0     1059 2022-05-04 12:15:59.574676 skit-calls-0.2.9/setup.py
+-rw-r--r--   0        0        0      942 2022-05-04 12:15:59.574998 skit-calls-0.2.9/PKG-INFO
```

### Comparing `skit-calls-0.2.8/LICENSE` & `skit-calls-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skit-calls-0.2.8/pyproject.toml` & `skit-calls-0.2.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skit-calls"
-version = "0.2.8"
+version = "0.2.9"
 description = "Library to fetch calls from a given environment."
 authors = ["ltbringer <amresh.venugopal@gmail.com>"]
 license = "GPL-3.0-only"
 repository = "https://github.com/skit-ai/skit-calls"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,14 +14,15 @@
 pandas = "^1.3.5"
 toml = "^0.10.2"
 loguru = "^0.5.3"
 tqdm = "^4.62.3"
 psycopg2 = "^2.9.3"
 pydash = "^5.1.0"
 attrs = "^21.4.0"
+dvc = {extras = ["s3"], version = "^2.10.2"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 httpretty = "^1.1.4"
 black = "^21.12b0"
 isort = "^5.10.1"
```

### Comparing `skit-calls-0.2.8/skit_calls/calls.py` & `skit-calls-0.2.9/skit_calls/calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,15 +108,18 @@
         return save_turns_in_memory(random_call_data)
     except SerializationFailure as e:
         logger.error(e)
         logger.error(f"This error is common if you are requesting a large dataset.")
 
 
 def select(
-    call_ids: List[int],
+    call_ids: Optional[List[int]] = None,
+    org_id: Optional[int] = None,
+    csv_file: Optional[str] = None,
+    uuid_col: Optional[str] = None,
     call_history: bool = False,
     on_disk: bool = True,
 ) -> str | pd.DataFrame:
     """
     Sample calls.
 
     :param call_ids: A list of call ids.
@@ -125,14 +128,21 @@
     :param on_disk: To save "in-memory" (works for <5k calls) vs "files", defaults to True
     :type on_disk: bool
 
     :return: A directory path if save is set to "files" otherwise path to a file.
     :rtype: str
     """
     try:
+        if csv_file and uuid_col and org_id:
+            df = pd.read_csv(csv_file)
+            call_ids = query.get_call_ids_from_uuids(org_id, tuple(df[uuid_col].unique()))
+        else:
+            raise ValueError("Both csv_file or uuid_column must be provided.")
+        if not call_ids:
+            raise ValueError("No call ids or csv file provided.")
         random_call_data = query.gen_random_calls(call_ids)
         if call_history:
             random_call_data = mutators.add_call_history(random_call_data)
         if on_disk:
             return save_turns_on_disk(random_call_data)
         return save_turns_in_memory(random_call_data)
     except SerializationFailure as e:
```

### Comparing `skit-calls-0.2.8/skit_calls/cli.py` & `skit-calls-0.2.9/skit_calls/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -131,15 +131,19 @@
     )
     parser.add_argument(
         "--asr-provider", help="Filter calls served via a specific ASR provider."
     )
 
 
 def build_select_command(parser: argparse.ArgumentParser) -> None:
-    parser.add_argument("--call-ids", type=str, nargs="+", help="The call-ids to select.")
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument("--call-ids", type=str, nargs="+", help="The call-ids to select.")
+    group.add_argument("--csv", help="CSV file that contains the call-ids to select.")
+    parser.add_argument("--org-id", help="The org for which you need the data. Required if --csv is set.")
+    parser.add_argument("--uuid-column", help="The column name of the UUID column in the CSV file. Required if --csv is set.")
     parser.add_argument("--history", action="store_true", help="Collect call history for each turn", default=False)
 
 
 def build_cli():
     version = get_version()
     parser = argparse.ArgumentParser(
         description=const.DESCRIPTION.format(version={version})
@@ -198,15 +202,15 @@
 def cmd_to_str(args: argparse.Namespace) -> str:
     utils.configure_logger(args.verbose)
 
     maybe_df = None
     if args.command == "sample":
         maybe_df = random_sample_calls(args)
     elif args.command == 'select':
-        maybe_df = calls.select(args.call_ids, args.history, on_disk=args.on_disk)
+        maybe_df = calls.select(args.call_ids, args.org_id, args.csv, args.uuid_column, args.history, on_disk=args.on_disk)
     else:
         raise argparse.ArgumentError(f"Unknown command {args.command}")
 
     if args.on_disk:
         print(maybe_df)
     else:
         _, file_path = tempfile.mkstemp(suffix=const.CSV_FILE)
```

### Comparing `skit-calls-0.2.8/skit_calls/constants.py` & `skit-calls-0.2.9/skit_calls/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 DEFAULT_TIMEZONE = "Asia/Kolkata"
 
 S3_URL_PATTERN_1 = r"https:\/\/s3\.\w{2}-(north|south|east|west)-\d{1,2}\.amazonaws\.com\/([A-Za-z0-9\-]+)\/(.+)"
 S3_URL_PATTERN_2 = r"https:\/\/([a-zA-Z\-]+)\.s3\.\w{2}-(north|south|east|west)-\d{1,2}\.amazonaws\.com\/(.+)"
 S3_OBJ_PATTERN = r"s3:\/\/([a-zA-Z0-9\-]+)\/(.+)"
 RANDOM_CALL_ID_QUERY = "RANDOM_CALL_ID_QUERY"
 RANDOM_CALL_DATA_QUERY = "RANDOM_CALL_DATA_QUERY"
+CALL_IDS_FROM_UUIDS_QUERY = "CALL_IDS_FROM_UUIDS_QUERY"
 RANDOM_CALL_DATA_CURSOR = "random_call_data_cursor"
 
 # Call types
 OUTBOUND = "OUTBOUND"
 INBOUND = "INBOUND"
 CALL_TEST = "CALL_TEST"
 DB_HOST = "DB_HOST"
```

### Comparing `skit-calls-0.2.8/skit_calls/data/db.py` & `skit-calls-0.2.9/skit_calls/data/db.py`

 * *Files identical despite different names*

### Comparing `skit-calls-0.2.8/skit_calls/data/model.py` & `skit-calls-0.2.9/skit_calls/data/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 IntentName = MaybeString
 IntentScore = MaybeFloat
 Slots = Things
 Entities = Things
 Utterances = Things
 
 
-def prediction2intent(
-    prediction: Dict[str, Any]
-) -> Tuple[IntentName, IntentScore, Slots]:
+def prediction2intent(prediction: Thing) -> Tuple[IntentName, IntentScore, Slots]:
     intents = prediction.get(const.INTENTS, [])
     if not intents:
         return None, None, []
     intent, *_ = intents
     return intent[const.NAME], intent[const.SCORE], intent[const.SLOTS]
 
 
@@ -97,14 +95,16 @@
     context: Thing | None = attr.ib(
         kw_only=True, factory=dict, converter=jsonify_maybestr, repr=False
     )
     intents_info: Things = attr.ib(
         kw_only=True, factory=list, converter=jsonify_maybestr, repr=False
     )
 
+    prediction: Thing = attr.ib(kw_only=True, factory=dict, converter=jsonify_maybestr, repr=False)
+
     intent: IntentName = attr.ib(kw_only=True, default=None)
     intent_score: IntentScore = attr.ib(kw_only=True, default=None, repr=print_floats)
     slots: Slots = attr.ib(kw_only=True, factory=list, repr=False)
     entities: Entities = attr.ib(kw_only=True, factory=list, repr=False)
 
     call_url: MaybeString = attr.ib(kw_only=True, repr=False, default=None)
     language: MaybeString = attr.ib(kw_only=True, default=None)
@@ -137,14 +137,15 @@
             call_uuid=record.call_uuid,
             conversation_id=record.conversation_id,
             conversation_uuid=record.conversation_uuid,
             audio_url=audio_url,
             call_url=call_url,
             reftime=record.reftime,
             state=record.state,
+            prediction=record.prediction,
             utterances=record.utterances,
             context=record.context,
             intents_info=record.intents_info,
             intent=intent_name,
             intent_score=intent_score,
             slots=slots,
             entities=entities,
```

### Comparing `skit-calls-0.2.8/skit_calls/data/mutators.py` & `skit-calls-0.2.9/skit_calls/data/mutators.py`

 * *Files identical despite different names*

### Comparing `skit-calls-0.2.8/skit_calls/data/query.py` & `skit-calls-0.2.9/skit_calls/data/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,22 @@
             cursor.execute(query, call_filters)
             all_ids = cursor.fetchall()
         return tuple(id_[0] for id_ in all_ids)
 
     return on_connect
 
 
+def get_call_ids_from_uuids(id_: int, uuids: Tuple[str]) -> Tuple[int]:
+    query = get_query(const.CALL_IDS_FROM_UUIDS_QUERY)
+    with connect() as conn:
+        with conn.cursor() as cursor:
+            cursor.execute(query, {const.UUID: uuids, const.ID: id_})
+            return tuple(id_[0] for id_ in cursor.fetchall())
+
+
 def gen_random_calls(
     call_ids: Tuple[int],
     asr_provider: str | None = None,
     limit: int = const.TURNS_LIMIT,
 ):
     time.sleep(1)
     query = get_query(const.RANDOM_CALL_DATA_QUERY)
@@ -84,15 +92,15 @@
     batch_size = (
         call_id_size // limit
         if call_id_size % limit == 0
         else call_id_size // limit + 1
     )
     logger.debug(f"Creating {batch_size} batches for {call_id_size} calls")
     i = 0
-    with tqdm(total=batch_size) as pbar:
+    with tqdm(total=batch_size, desc="Downloading calls dataset.") as pbar:
         for i in range(0, len(call_ids), limit):
             batch = call_ids[i : i + limit]
             with connect() as conn:
                 with conn.cursor(cursor_factory=NamedTupleCursor) as cursor:
                     cursor.execute(query, {**turn_filters, const.CALL_IDS: batch})
                     result_set = cursor.fetchall()
                     yield from as_turns(result_set)
```

### Comparing `skit-calls-0.2.8/skit_calls/utils.py` & `skit-calls-0.2.9/skit_calls/utils.py`

 * *Files identical despite different names*

### Comparing `skit-calls-0.2.8/setup.py` & `skit-calls-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.3,<6.0',
  'aiofiles>=0.8.0,<0.9.0',
  'aiohttp>=3.8.1,<4.0.0',
  'attrs>=21.4.0,<22.0.0',
+ 'dvc[s3]>=2.10.2,<3.0.0',
  'loguru>=0.5.3,<0.6.0',
  'pandas>=1.3.5,<2.0.0',
  'psycopg2>=2.9.3,<3.0.0',
  'pydash>=5.1.0,<6.0.0',
  'toml>=0.10.2,<0.11.0',
  'tqdm>=4.62.3,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['skit-calls = skit_calls.cli:main']}
 
 setup_kwargs = {
     'name': 'skit-calls',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Library to fetch calls from a given environment.',
     'long_description': None,
     'author': 'ltbringer',
     'author_email': 'amresh.venugopal@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/skit-ai/skit-calls',
```

### Comparing `skit-calls-0.2.8/PKG-INFO` & `skit-calls-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: skit-calls
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to fetch calls from a given environment.
 Home-page: https://github.com/skit-ai/skit-calls
 License: GPL-3.0-only
 Author: ltbringer
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=5.3,<6.0)
 Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: dvc[s3] (>=2.10.2,<3.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: pydash (>=5.1.0,<6.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/skit-ai/skit-calls
```

