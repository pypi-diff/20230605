# Comparing `tmp/macrometa-target-collection-0.0.63.tar.gz` & `tmp/macrometa-target-collection-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.63.tar", last modified: Tue May 30 04:21:16 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.64.tar", last modified: Mon Jun  5 17:20:18 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.63.tar` & `macrometa-target-collection-0.0.64.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.484135 macrometa-target-collection-0.0.64/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14466 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.63/LICENSE` & `macrometa-target-collection-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.63/PKG-INFO` & `macrometa-target-collection-0.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.63
+Version: 0.0.64
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.63/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.64/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.63/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.64/macrometa_target_collection/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     if state is not None:
         line = json.dumps(state)
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
-def try_upsert(collection: StandardCollection, record_batch: RecordBatch, force=False):
+def try_upsert(collection: StandardCollection, record_batch: RecordBatch, client, force=False):
     if record_batch.length() >= record_batch.max_batch_size or force:
         to_insert = record_batch.flush()
         to_update = []
         records_array = remove_time_extracted(to_insert)
 
         for i, r in enumerate(collection.insert_many(records_array)):
             if type(r) is DocumentInsertError:
@@ -111,37 +111,40 @@
 
         if len(to_update) > 0:
             records_array = remove_time_extracted(to_update)
             for i, r in enumerate(collection.update_many(records_array)):
                 if type(r) is DocumentInsertError:
                     # Increment ingest_errors metric
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-                    print(f'Failed to insert/update record: {to_update[i]}. {r}')
+                    logger.warn(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
                     diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
                         diff.total_seconds())
+        try_delete(client, collection)
         record_batch.last_executed_time = datetime.now(timezone.utc)
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
-def try_delete(collection: StandardCollection, _key: str):
+def try_delete(client, collection: StandardCollection):
     try:
-        collection.delete(_key)
+    
+        client.execute_query(f"FOR d IN @@collection FILTER d._sdc_deleted_at != null REMOVE d._key IN @@collection",
+                                  bind_vars={"@collection": collection.name})
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-        logger.warn(f'Failed to delete record with _key: {_key}. {e}')
+        logger.warn(f'Failed to delete records. {e}')
 
 
-def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch):
+def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch, client):
     state = None
     schemas = {}
     key_properties = {}
     validators = {}
 
     for message in messages:
         try:
@@ -205,32 +208,25 @@
                         logger.info(f"Primary key of the source doesn't satisfy the constraints of macrometa "
                                     f"document key, Hashing the key and using it in hex form to make it compliant.")
                     if _key:
                         rec['_key'] = _key
                 except:
                     _key = None
 
-                if '_sdc_deleted_at' in rec:
-                    if rec['_sdc_deleted_at']:
-                        if _key:
-                            try_delete(collection, _key)
-                    else:
-                        rec.pop('_sdc_deleted_at', None)
-                        logger.info(f'record is {rec}')
-                        record_batch.append(rec)
-                else:
-                    record_batch.append(rec)
+                if '_sdc_deleted_at' in rec and not rec['_sdc_deleted_at']:
+                    rec.pop('_sdc_deleted_at', None)
+                record_batch.append(rec)
             except TypeError as e:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 # TODO: This is temporary until json serializing issue for Decimals are fixed in pyC8
                 logger.debug("pyC8 error occurred")
 
             state = None
-            try_upsert(collection, record_batch)
+            try_upsert(collection, record_batch, client)
         elif message_type == 'STATE':
             logger.debug('Setting state to {}'.format(o['value']))
             state = o['value']
             emit_state(state)
         elif message_type == 'SCHEMA':
             stream = o['stream']
             schemas[stream] = o['schema']
@@ -253,28 +249,28 @@
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     elif time_extracted.tzinfo is None:
         # If the datetime object is timezone-naive, set it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     return time_extracted
 
 
-def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch) -> AbstractEventLoop:
+def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch, client) -> AbstractEventLoop:
     event_loop = asyncio.new_event_loop()
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
-    asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
+    asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch, client), event_loop)
     return event_loop
 
 
-async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
+async def process_batch(collection: StandardCollection, record_batch: RecordBatch, client) -> None:
     while True:
         await asyncio.sleep(record_batch.interval)
         timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
-            try_upsert(collection, record_batch, force=True)
+            try_upsert(collection, record_batch, client, force=True)
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
 
@@ -300,21 +296,21 @@
     )
 
     if not client.has_collection(target_collection):
         client.create_collection(name=target_collection)
 
     collection = client.get_collection(target_collection)
     record_batch = RecordBatch(config)
-    event_loop = setup_batch_task(collection, record_batch)
+    event_loop = setup_batch_task(collection, record_batch, client)
     input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    state = persist_messages(collection, input_messages, record_batch)
+    state = persist_messages(collection, input_messages, record_batch, client)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
-    try_upsert(collection, record_batch, force=True)
+    try_upsert(collection, record_batch, client, force=True)
 
     if is_metrics_enabled.lower() == 'true':
         # Wait for Prometheus to scrape the metrics
         while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total",
                                      f"workflow=\"{workflow_label}\""):
             logger.info("Waiting for metrics scrape...")
             time.sleep(15)
```

### Comparing `macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.63
+Version: 0.0.64
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.63/pyproject.toml` & `macrometa-target-collection-0.0.64/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.63"
+version = "0.0.64"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

