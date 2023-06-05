# Comparing `tmp/django_pgpubsub-1.0.6.tar.gz` & `tmp/django_pgpubsub-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgpubsub-1.0.6.tar", max compression
+gzip compressed data, was "django_pgpubsub-1.1.0.tar", max compression
```

## Comparing `django_pgpubsub-1.0.6.tar` & `django_pgpubsub-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
--rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.6/LICENSE
--rw-r--r--   0        0        0    25976 2023-04-10 16:26:51.399667 django_pgpubsub-1.0.6/README.md
--rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.6/pgpubsub/__init__.py
--rw-r--r--   0        0        0     7492 2023-04-26 18:48:54.103379 django_pgpubsub-1.0.6/pgpubsub/channel.py
--rw-r--r--   0        0        0     5158 2023-05-01 16:03:41.570536 django_pgpubsub-1.0.6/pgpubsub/listen.py
--rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.6/pgpubsub/listeners.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.6/pgpubsub/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.6/pgpubsub/management/commands/__init__.py
--rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.6/pgpubsub/management/commands/listen.py
--rw-r--r--   0        0        0      751 2023-04-10 16:26:51.407699 django_pgpubsub-1.0.6/pgpubsub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.6/pgpubsub/migrations/__init__.py
--rw-r--r--   0        0        0      690 2023-04-10 16:26:51.408192 django_pgpubsub-1.0.6/pgpubsub/models.py
--rw-r--r--   0        0        0     2132 2023-05-01 16:03:41.571304 django_pgpubsub-1.0.6/pgpubsub/notify.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.6/pgpubsub/tests/__init__.py
--rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.6/pgpubsub/tests/apps.py
--rw-r--r--   0        0        0      640 2023-04-11 08:28:49.364826 django_pgpubsub-1.0.6/pgpubsub/tests/channels.py
--rw-r--r--   0        0        0     1926 2023-05-01 16:03:41.571905 django_pgpubsub-1.0.6/pgpubsub/tests/listeners.py
--rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0      673 2023-04-26 17:40:53.933980 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0002_auto_20230411_0829.py
--rw-r--r--   0        0        0     2880 2023-04-26 19:11:19.787192 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0003_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.6/pgpubsub/tests/migrations/__init__.py
--rw-r--r--   0        0        0     1348 2023-04-11 13:37:33.192550 django_pgpubsub-1.0.6/pgpubsub/tests/models.py
--rw-r--r--   0        0        0     6436 2023-05-01 16:03:41.572816 django_pgpubsub-1.0.6/pgpubsub/tests/test_core.py
--rw-r--r--   0        0        0     2199 2023-04-11 13:37:33.194348 django_pgpubsub-1.0.6/pgpubsub/tests/test_deserialize.py
--rw-r--r--   0        0        0     4478 2023-04-26 18:48:54.104075 django_pgpubsub-1.0.6/pgpubsub/tests/test_trigger_deserialize.py
--rw-r--r--   0        0        0     1040 2023-04-10 16:26:51.410131 django_pgpubsub-1.0.6/pgpubsub/triggers.py
--rw-r--r--   0        0        0     2082 2023-05-01 16:04:19.432801 django_pgpubsub-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.1.0/LICENSE
+-rw-r--r--   0        0        0    28647 2023-06-05 11:14:22.301311 django_pgpubsub-1.1.0/README.md
+-rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.1.0/pgpubsub/__init__.py
+-rw-r--r--   0        0        0     7361 2023-06-05 11:14:22.301580 django_pgpubsub-1.1.0/pgpubsub/channel.py
+-rw-r--r--   0        0        0     5361 2023-06-05 11:14:22.302544 django_pgpubsub-1.1.0/pgpubsub/listen.py
+-rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.1.0/pgpubsub/listeners.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.1.0/pgpubsub/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.1.0/pgpubsub/management/commands/__init__.py
+-rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.1.0/pgpubsub/management/commands/listen.py
+-rw-r--r--   0        0        0      751 2023-04-10 16:26:51.407699 django_pgpubsub-1.1.0/pgpubsub/migrations/0001_initial.py
+-rw-r--r--   0        0        0      404 2023-05-06 09:40:14.478933 django_pgpubsub-1.1.0/pgpubsub/migrations/0002_notification_created_at.py
+-rw-r--r--   0        0        0      939 2023-06-05 11:14:22.302725 django_pgpubsub-1.1.0/pgpubsub/migrations/0003_notification_db_version.py
+-rw-r--r--   0        0        0     1025 2023-06-05 11:14:22.302897 django_pgpubsub-1.1.0/pgpubsub/migrations/0004_notification_pgpubsub_notification_set_db_version.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.1.0/pgpubsub/migrations/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-05 11:14:22.303100 django_pgpubsub-1.1.0/pgpubsub/models.py
+-rw-r--r--   0        0        0     2198 2023-06-05 11:14:22.305550 django_pgpubsub-1.1.0/pgpubsub/notify.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.1.0/pgpubsub/tests/__init__.py
+-rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.1.0/pgpubsub/tests/apps.py
+-rw-r--r--   0        0        0      892 2023-06-05 11:14:22.305833 django_pgpubsub-1.1.0/pgpubsub/tests/channels.py
+-rw-r--r--   0        0        0     2343 2023-06-05 11:14:22.306340 django_pgpubsub-1.1.0/pgpubsub/tests/listeners.py
+-rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      673 2023-04-26 17:40:53.933980 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0002_auto_20230411_0829.py
+-rw-r--r--   0        0        0     2880 2023-04-26 19:11:19.787192 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0003_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py
+-rw-r--r--   0        0        0     2883 2023-06-05 11:14:22.306522 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0003_auto_20230516_1151.py
+-rw-r--r--   0        0        0      400 2023-06-05 11:14:22.306670 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0004_alter_media_id.py
+-rw-r--r--   0        0        0      350 2023-06-05 11:14:22.306952 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0005_rename_id_media_key.py
+-rw-r--r--   0        0        0      782 2023-06-05 11:14:22.307258 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0006_child_parent.py
+-rw-r--r--   0        0        0     1147 2023-06-05 11:14:22.307695 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0007_child_pgpubsub_89ef9.py
+-rw-r--r--   0        0        0      420 2023-06-05 11:14:22.307907 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0008_alter_parent_key.py
+-rw-r--r--   0        0        0     1470 2023-06-05 11:14:22.308067 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0009_auto_20230522_0720.py
+-rw-r--r--   0        0        0      380 2023-06-05 11:14:22.308186 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0010_media_store_id.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.1.0/pgpubsub/tests/migrations/__init__.py
+-rw-r--r--   0        0        0     1749 2023-06-05 11:14:22.308824 django_pgpubsub-1.1.0/pgpubsub/tests/models.py
+-rw-r--r--   0        0        0     9148 2023-06-05 11:14:22.309182 django_pgpubsub-1.1.0/pgpubsub/tests/test_core.py
+-rw-r--r--   0        0        0     2199 2023-04-11 13:37:33.194348 django_pgpubsub-1.1.0/pgpubsub/tests/test_deserialize.py
+-rw-r--r--   0        0        0     5425 2023-06-05 11:14:22.309445 django_pgpubsub-1.1.0/pgpubsub/tests/test_trigger_deserialize.py
+-rw-r--r--   0        0        0     1039 2023-06-05 11:14:22.309922 django_pgpubsub-1.1.0/pgpubsub/triggers.py
+-rw-r--r--   0        0        0     2246 2023-06-05 11:21:13.484959 django_pgpubsub-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    29769 1970-01-01 00:00:00.000000 django_pgpubsub-1.1.0/PKG-INFO
```

### Comparing `django_pgpubsub-1.0.6/LICENSE` & `django_pgpubsub-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/README.md` & `django_pgpubsub-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -310,14 +310,55 @@
 pre-creation (and would hence be ``None``) and ``new`` would refer to a copy of
 the newly created ``Author`` instance. This payload is inspired by the ``OLD``
 and ``NEW`` values available in the postgres ``CREATE TRIGGER`` statement
 (https://www.postgresql.org/docs/9.1/sql-createtrigger.html). The only custom
 logic we need to define on a trigger channel is the ``model`` class-level
 attribute.
 
+** Models migrations **
+
+Note that the payload captures the snapshot of the ``Author`` instance for some
+time. Later it will be deserialized (see more about this below in the
+Listeners section). It may happen that by that time the ``Author`` model is
+migrated in django and this requires careful handling to make sure the payload
+can still be deserialized and processed. Special handling is required when the
+migration is backward incompatible like making existing field mandatory.
+
+Let's look to the example how to do that and what tooling ``pgpubsub`` provides
+to facilitate that. Let's says we want to add a new mandatory text field
+``email`` to ``Author``.
+
+This is done in three steps (releases):
+
+1. New optional field is added. Application is modified so that new records
+   always get a value in ``email`` field.
+2. Values are populated in the existing records.
+3. Fields is made mandatory.
+
+Note that before release 2 is deployed and the migration that populates the
+field is applied modifications to some ``Author`` entities would produce
+payloads that do not have value in the ``email`` field.
+
+When release 3 is deployed the application may assume that every ``Author`` has
+``email``. The problem is that the notifications produced before release 2 is
+deployed may be still not processed (for example the listener process was not
+run or there was an issue with the processing of some specific notification and
+it was skipped). In order to safely deploy release 3 the deployer need to know
+if there are any notifications that were created before django migrations of
+the release 2 were applied.
+
+To facilitate this ``Notification`` entity stores ``db_version`` field which
+contains the latest migration identier for the django app the ``Author`` is
+defined in. The deployer may check if there are any notifications with the old
+``db_version`` before deploying version that potentially breaks backward
+compatibility in terms of the data structure. 
+
+In this case deployer should check that there are no ``Notification`` entities
+with ``db_version`` before the version that was assigned to the migrations in
+release 2.
 
 Listeners
 --------
 
 In the ``pgpubsub`` library, a *listener* is the function
 which processes notifications sent through some particular channel.
 
@@ -629,14 +670,33 @@
 to be processed. This allows to recover from scenarios like the one in the paragraph described
 above.
 
 Note that this recovery option can be enabled whenever we use the `listen` management command
 by supplying it with the `--recover` option. This will tell the listening processes to replay
 any missed stored notifications automatically when it starts up.
 
+It is important to enable server side cursors in the django settings used by
+the listener. Their usage makes memory consumption much lower during the
+recovery and that is important if there is a need to recover many notifications:
+
+```
+DATABASES = {
+    "default": {
+        "ENGINE": "django.db.backends.postgresql",
+        ...,
+        "DISABLE_SERVER_SIDE_CURSORS": False,
+    }
+}
+```
+
+or if ``dj_database_url`` is used:
+```
+DATABASES = {'default': dj_database_url.config()}
+DATABASES['default']["DISABLE_SERVER_SIDE_CURSORS"] = False
+```
 
 Live Demos
 ==========
 
 `bulk_create` over several processes
 ------------------------------------
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/channel.py` & `django_pgpubsub-1.1.0/pgpubsub/channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -179,45 +179,41 @@
         model_cls = apps.get_model(
             app_label=payload['app'],
             model_name=payload['model'],
         )
         fields = {
             field.name: field for field in model_cls._meta.fields
         }
-        db_fields = {
-            field.db_column: field for field in model_cls._meta.fields
+        db_columns = {
+            field.column: field for field in model_cls._meta.fields
         }
 
         original_state = payload[state]
         new_state = {}
         model_data = []
         if payload[state] is not None:
-            for field in list(original_state):
+            for db_field in list(original_state):
                 # Triggers serialize the notification payload with
                 # respect to how the model fields look as columns
-                # in the database. We therefore need to take
-                # care to map xxx_id named columns to the corresponding
-                # xxx model field and also to account for model fields
-                # with alternative database column names as declared
-                # by the db_column attribute.
-                value = original_state.pop(field)
-                if field.endswith('_id'):
-                    field = field.rsplit('_id')[0]
-                if field in fields:
-                    new_state[field] = value
-                elif field in db_fields:
-                    field = db_fields[field].name
-                    new_state[field] = value
+                # in the database. We therefore need to translate
+                # to model fields and skip outdated fields
+                value = original_state.pop(db_field)
+                if db_field in db_columns:
+                    model_field = db_columns[db_field].name
+                    new_state[model_field] = value
 
-            model_data.append(
-                {'fields': new_state,
-                 'id': new_state['id'],
-                 'model': f'{app}.{model_name}',
-                 },
-            )
+            pk = model_cls._meta.pk
+            serialized = {
+                'fields': new_state,
+                'pk': new_state[pk.name],
+                'model': f'{app}.{model_name}',
+            }
+            if isinstance(pk, models.fields.related.OneToOneField):
+                serialized['fields'][pk.remote_field.model._meta.pk.name] = serialized['pk']
+            model_data.append(serialized)
         return model_data
 
 
 def locate_channel(channel):
     if isinstance(channel, str):
         channel = locate(channel)
     if channel is None:
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/listen.py` & `django_pgpubsub-1.1.0/pgpubsub/listen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import multiprocessing
 import select
 from typing import List, Union
 
 from django.db import connection, transaction
 from psycopg2._psycopg import Notify
 
@@ -11,14 +12,15 @@
     Channel,
     ChannelNotFound,
     locate_channel,
     registry,
 )
 from pgpubsub.models import Notification
 
+logger = logging.getLogger(__name__)
 
 POLL = True
 
 
 def listen(
     channels: Union[List[BaseChannel], List[str]] = None,
     recover: bool = False,
@@ -26,24 +28,24 @@
     multiprocessing.set_start_method('fork', force=True)
     pg_connection = listen_to_channels(channels)
 
     if recover:
         process_stored_notifications(channels)
         process_notifications(pg_connection)
 
-    print('Listening for notifications... \n')
+    logger.info('Listening for notifications... \n')
     while POLL:
         if select.select([pg_connection], [], [], 1) == ([], [], []):
             pass
         else:
             try:
                 process_notifications(pg_connection)
             except Exception as e:
-                print(f'Encountered exception {e}')
-                print('Restarting process')
+                logger.error(f'Encountered exception {e}', exc_info=e)
+                logger.info('Restarting process')
                 connection.close()
                 process = multiprocessing.Process(target=listen, args=(channels,))
                 process.start()
                 raise
 
 
 def listen_to_channels(channels: Union[List[BaseChannel], List[str]] = None):
@@ -56,15 +58,15 @@
             for channel, callbacks in registry.items()
             if issubclass(channel, tuple(channels))
         }
     if not channels:
         raise ChannelNotFound()
     cursor = connection.cursor()
     for channel in channels:
-        print(f'Listening on {channel.name()}\n')
+        logger.info(f'Listening on {channel.name()}\n')
         cursor.execute(f'LISTEN {channel.listen_safe_name()};')
     return connection.connection
 
 
 def process_notifications(pg_connection):
     pg_connection.poll()
     while pg_connection.notifies:
@@ -92,15 +94,15 @@
         self.validate()
 
     def validate(self):
         if self.channel_cls.lock_notifications:
             raise InvalidNotificationProcessor
 
     def process(self):
-        print(f'Processing notification for {self.channel_cls.name()}\n')
+        logger.info(f'Processing notification for {self.channel_cls.name()}\n')
         return self._execute()
 
     def _execute(self):
         channel = self.channel_cls.build_from_payload(
             self.notification.payload, self.callbacks)
         channel.execute_callbacks()
         self.pg_connection.poll()
@@ -109,54 +111,56 @@
 class LockableNotificationProcessor(NotificationProcessor):
 
     def validate(self):
         if self.notification.payload == 'null':
             raise InvalidNotificationProcessor
 
     def process(self):
-        print(
+        logger.info(
             f'Processing notification for {self.channel_cls.name()}')
         notification = (
             Notification.objects.select_for_update(
                 skip_locked=True).filter(
                 channel=self.notification.channel,
                 payload=self.notification.payload,
             ).first()
         )
         if notification is None:
-            print(f'Could not obtain a lock on notification '
-                  f'{self.notification.pid}')
-            print('\n')
+            logger.info(f'Could not obtain a lock on notification '
+                        f'{self.notification.pid}\n')
         else:
-            print(f'Obtained lock on {notification}')
+            logger.info(f'Obtained lock on {notification}')
             self.notification = notification
             self._execute()
             self.notification.delete()
 
 
 class NotificationRecoveryProcessor(LockableNotificationProcessor):
 
     def validate(self):
         if self.notification.payload != 'null':
             raise InvalidNotificationProcessor
 
     def process(self):
-        print(f'Processing all notifications for channel {self.channel_cls.name()} \n')
+        logger.info(f'Processing all notifications for channel {self.channel_cls.name()} \n')
         notifications = (
             Notification.objects.select_for_update(
-                skip_locked=True).filter(channel=self.notification.channel)
+                skip_locked=True).filter(channel=self.notification.channel).iterator()
         )
-        print(f'Found notifications: {notifications}')
+        logger.info(f'Found notifications: {notifications}')
         for notification in notifications:
             self.notification = notification
             try:
                 with transaction.atomic():
                     self._execute()
             except Exception as e:
-                print(f'Encountered {e} exception when processing notification {notification}')
+                logger.error(
+                    f'Encountered {e} exception when processing notification {notification}',
+                    exc_info=e
+                )
             else:
-                print(f'Successfully processed notification {notification}')
+                logger.info(f'Successfully processed notification {notification}')
                 self.notification.delete()
 
 
 class InvalidNotificationProcessor(Exception):
     pass
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/listeners.py` & `django_pgpubsub-1.1.0/pgpubsub/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/management/commands/listen.py` & `django_pgpubsub-1.1.0/pgpubsub/management/commands/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/migrations/0001_initial.py` & `django_pgpubsub-1.1.0/pgpubsub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/notify.py` & `django_pgpubsub-1.1.0/pgpubsub/notify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import logging
 from typing import Type, Union
 
 from django.db import connection
 from django.db.transaction import atomic
 
 from pgpubsub.channel import locate_channel, Channel, registry
 
 
+logger = logging.getLogger(__name__)
+
+
 @atomic
 def notify(channel: Union[Type[Channel], str], **kwargs):
     channel_cls = locate_channel(channel)
     channel = channel_cls(**kwargs)
     serialized = channel.serialize()
     with connection.cursor() as cursor:
         name = channel_cls.name()
-        print(f'Notifying channel {name} with payload {serialized}')
+        logger.info(f'Notifying channel {name} with payload {serialized}')
         cursor.execute(
             f"select pg_notify('{channel_cls.listen_safe_name()}', '{serialized}');")
         if channel_cls.lock_notifications:
             from pgpubsub.models import Notification
             Notification.objects.create(
                 channel=name,
                 payload=serialized,
@@ -44,14 +48,14 @@
             for channel, callbacks in registry.items()
             if issubclass(channel, tuple(channels))
         }
     with connection.cursor() as cursor:
         lock_channels = [c for c in channels if c.lock_notifications]
         for channel_cls in lock_channels:
             payload = 'null'
-            print(
+            logger.info(
                 f'Notifying channel {channel_cls.name()} to recover '
                 f'previously stored notifications.\n')
             cursor.execute(
                 f"select pg_notify('{channel_cls.listen_safe_name()}', '{payload}');")
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/channels.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/channels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 import datetime
 
 from pgpubsub.channel import Channel, TriggerChannel
-from pgpubsub.tests.models import Author, Media, Post
+from pgpubsub.tests.models import Author, Child, ChildOfAbstract, Media, Post
 
 
 @dataclass
 class Reads(Channel):
     model_id: int
     model_type: str
     date: datetime.date = None
@@ -20,14 +20,26 @@
 @dataclass
 class MediaTriggerChannel(TriggerChannel):
     model = Media
     lock_notifications = True
 
 
 @dataclass
+class ChildTriggerChannel(TriggerChannel):
+    model = Child
+    lock_notifications = True
+
+
+@dataclass
+class ChildOfAbstractTriggerChannel(TriggerChannel):
+    model = ChildOfAbstract
+    lock_notifications = True
+
+
+@dataclass
 class AuthorTriggerChannel(TriggerChannel):
     model = Author
     lock_notifications = True
 
 
 @dataclass
 class PostTriggerChannel(TriggerChannel):
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/listeners.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/listeners.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import datetime
 
 from django.db.transaction import atomic
 
 import pgpubsub
 from pgpubsub.tests.channels import (
     AuthorTriggerChannel,
+    ChildOfAbstractTriggerChannel,
+    ChildTriggerChannel,
     MediaTriggerChannel,
     PostReads,
     PostTriggerChannel,
 )
-from pgpubsub.tests.models import Author, Media, Post
+from pgpubsub.tests.models import Author, Child, ChildOfAbstract, Media, Post
 
 post_reads_per_date_cache = defaultdict(dict)
 author_reads_cache = {}
 
 
 @pgpubsub.listener(PostReads)
 def update_post_reads_per_date_cache(
@@ -59,7 +61,17 @@
 
 @pgpubsub.post_save_listener(MediaTriggerChannel)
 def scan_media(old: Media, new: Media):
     if not old:
         print(f'Perform virus scan on the new media {new}.')
     else:
         print(f'Media updated; scan {new} all over again.')
+
+
+@pgpubsub.post_save_listener(ChildTriggerChannel)
+def post_child_save(old: Child, new: Child):
+    print(f'New child created {new}.')
+
+
+@pgpubsub.post_save_listener(ChildOfAbstractTriggerChannel)
+def post_child_of_abstract_save(old: ChildOfAbstract, new: ChildOfAbstract):
+    print(f'New child of abstract parent created {new}.')
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0001_initial.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0002_auto_20230411_0829.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0002_auto_20230411_0829.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/migrations/0003_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/migrations/0003_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/models.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 from django.contrib.auth.models import User
 from django.db import models
 
 from pgpubsub.notify import notify
 
 
 class Media(models.Model):
+    key = models.AutoField(primary_key=True)
     name = models.TextField()
     content_type = models.TextField(null=True)
     size = models.BigIntegerField(null=True)
+    store_id = models.TextField(null=True)
 
 
 class Author(models.Model):
     user = models.ForeignKey(
         User, on_delete=models.PROTECT, null=True)
     name = models.TextField()
     age = models.IntegerField(null=True)
@@ -43,7 +45,26 @@
         post = cls.objects.get(pk=post_id)
         notify(
             'pgpubsub.tests.channels.PostReads',
             model_id=post_id,
             date=datetime.date.today(),
         )
         return post
+
+
+class Parent(models.Model):
+    key = models.AutoField(primary_key=True, editable=False)
+
+
+class Child(Parent):
+    pass
+
+
+class AbstractParent(models.Model):
+    key = models.AutoField(primary_key=True, editable=False)
+
+    class Meta:
+        abstract = True
+
+
+class ChildOfAbstract(AbstractParent):
+    pass
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/test_core.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import datetime
 import json
 from unittest.mock import patch
 
 from django.contrib.auth.models import User
+from django.db import connection
 from django.db.transaction import atomic
+from django.db.migrations.recorder import MigrationRecorder
 import pytest
 
-from pgpubsub.listen import listen_to_channels, process_notifications, listen
+from pgpubsub.listen import (
+    listen_to_channels,
+    process_notifications,
+    listen,
+    NotificationRecoveryProcessor,
+)
 from pgpubsub.models import Notification
 from pgpubsub.notify import process_stored_notifications
 from pgpubsub.tests.channels import (
     AuthorTriggerChannel,
     MediaTriggerChannel,
 )
 from pgpubsub.tests.listeners import post_reads_per_date_cache
@@ -101,89 +108,149 @@
     assert not Post.objects.exists()
     process_notifications(pg_connection)
     assert 2 == Post.objects.count()
     post_authors = Post.objects.values_list('author_id', flat=True)
     assert [author.pk for author in authors] == list(post_authors)
 
 
+def _simulate_listener_does_not_receive_notifications(pg_connection):
+    pg_connection.notifies = []
+    pg_connection.poll()
+    assert 0 == len(pg_connection.notifies)
+
+
 @pytest.mark.django_db(transaction=True)
 def test_process_stored_notifications(pg_connection):
     Author.objects.create(name='Billy')
     Author.objects.create(name='Billy2')
     assert 2 == len(pg_connection.notifies)
     assert 2 == Notification.objects.count()
     assert 0 == Post.objects.count()
-    # Simulate when the listener fails to
-    # receive notifications
-    pg_connection.notifies = []
-    pg_connection.poll()
-    assert 0 == len(pg_connection.notifies)
+    _simulate_listener_does_not_receive_notifications(pg_connection)
     process_stored_notifications()
     pg_connection.poll()
     # One notification for each lockable channel
-    assert 3 == len(pg_connection.notifies)
+    assert 5 == len(pg_connection.notifies)
     process_notifications(pg_connection)
     assert 0 == Notification.objects.count()
     assert 2 == Post.objects.count()
 
 
 @pytest.mark.django_db(transaction=True)
 def test_recover_notifications(pg_connection):
     Author.objects.create(name='Billy')
     Author.objects.create(name='Billy2')
     pg_connection.poll()
     assert 2 == len(pg_connection.notifies)
     assert 2 == Notification.objects.count()
     assert 0 == Post.objects.count()
-    # Simulate when the listener fails to
-    # receive notifications
-    pg_connection.notifies = []
-    pg_connection.poll()
-    assert 0 == len(pg_connection.notifies)
+    _simulate_listener_does_not_receive_notifications(pg_connection)
     with patch('pgpubsub.listen.POLL', False):
         listen(recover=True)
     pg_connection.poll()
     assert 0 == Notification.objects.count()
     assert 2 == Post.objects.count()
 
-
 @pytest.mark.django_db(transaction=True)
-def test_recover_notifications_after_exception(pg_connection):
-    user = User.objects.create(username='Billy')
-    author = Author.objects.create(name='Billy', user=user)
+def test_recover_multiple_notifications(pg_connection):
+    ENTITIES_COUNT = 5
+    for i in range(ENTITIES_COUNT):
+        Author.objects.create(name=f'Billy{i}')
+    pg_connection.poll()
+    assert ENTITIES_COUNT == len(pg_connection.notifies)
+    assert ENTITIES_COUNT == Notification.objects.count()
+    assert 0 == Post.objects.count()
+    _simulate_listener_does_not_receive_notifications(pg_connection)
+    with patch('pgpubsub.listen.POLL', False):
+        listen(recover=True)
+    pg_connection.poll()
+    assert 0 == Notification.objects.count()
+    assert ENTITIES_COUNT == Post.objects.count()
 
-    # Create a Notification with a payload which will produce
-    # an exception
+
+def _create_notification_that_cannot_be_processed():
     notification = Notification.objects.last()
     payload = json.loads(notification.payload)
-    payload['new']['user_id'] = int(author.user_id) + 1
-    notification.payload = str(payload)
+    payload.pop('app', None)
+    notification.payload = json.dumps(payload)
     notification.pk = None
     notification.save()
 
+
+@pytest.mark.django_db(transaction=True)
+def test_recover_notifications_after_exception(pg_connection):
+    author = Author.objects.create(name='Billy')
+    _create_notification_that_cannot_be_processed()
     Author.objects.create(name='Billy2')
 
     pg_connection.poll()
     assert 2 == len(pg_connection.notifies)
 
     assert 3 == Notification.objects.count()
     assert 0 == Post.objects.count()
 
-    # Simulate when the listener fails to receive notifications
-    pg_connection.notifies = []
-    pg_connection.poll()
-    assert 0 == len(pg_connection.notifies)
+    _simulate_listener_does_not_receive_notifications(pg_connection)
     with patch('pgpubsub.listen.POLL', False):
         listen(recover=True)
     pg_connection.poll()
     assert 1 == Notification.objects.count()
     assert 2 == Post.objects.count()
 
+@pytest.mark.django_db(transaction=True)
+def test_recover_multiple_notifications_after_exception(pg_connection):
+    Author.objects.create(name=f'Billy_1')
+    Author.objects.create(name=f'Billy_2')
+    _create_notification_that_cannot_be_processed()
+    Author.objects.create(name=f'Billy_3')
+    _create_notification_that_cannot_be_processed()
+    _create_notification_that_cannot_be_processed()
+    _create_notification_that_cannot_be_processed()
+    Author.objects.create(name=f'Billy_4')
+    Author.objects.create(name=f'Billy_5')
+
+    GOOD_COUNT = 5
+    BROKEN_COUNT = 4
+
+    pg_connection.poll()
+    assert GOOD_COUNT == len(pg_connection.notifies)
+    assert GOOD_COUNT + BROKEN_COUNT == Notification.objects.count()
+    assert 0 == Post.objects.count()
+
+    _simulate_listener_does_not_receive_notifications(pg_connection)
+    with patch('pgpubsub.listen.POLL', False):
+        listen(recover=True)
+    pg_connection.poll()
+    assert BROKEN_COUNT == Notification.objects.count()
+    assert GOOD_COUNT == Post.objects.count()
+
 
 @pytest.mark.django_db(transaction=True)
 def test_media_insert_notify(pg_connection):
     Media.objects.create(name='avatar.jpg', content_type='image/png', size=15000)
     assert 1 == len(pg_connection.notifies)
-    stored_notification = Notification.from_channel(
-        channel=MediaTriggerChannel).get()
+    stored_notification = Notification.from_channel(channel=MediaTriggerChannel).get()
     assert 'old' in stored_notification.payload
     assert 'new' in stored_notification.payload
+
+
+@pytest.fixture
+def tx_start_time(django_db_setup):
+    with connection.cursor() as cursor:
+        cursor.execute("SELECT now();")
+        return cursor.fetchone()[0]
+
+
+@pytest.mark.django_db(transaction=True)
+def test_persistent_notification_has_a_creation_timestamp(pg_connection, tx_start_time):
+    Media.objects.create(name='avatar.jpg', content_type='image/png', size=15000)
+    assert 1 == len(pg_connection.notifies)
+    stored_notification = Notification.from_channel(channel=MediaTriggerChannel).get()
+    assert stored_notification.created_at >= tx_start_time
+
+
+@pytest.mark.django_db(transaction=True)
+def test_persistent_notification_has_a_db_version(pg_connection, tx_start_time):
+    latest_app_migration = MigrationRecorder.Migration.objects.filter(app='tests').latest('id')
+    Media.objects.create(name='avatar.jpg', content_type='image/png', size=15000)
+    assert 1 == len(pg_connection.notifies)
+    stored_notification = Notification.from_channel(channel=MediaTriggerChannel).get()
+    assert stored_notification.db_version == latest_app_migration.id
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/test_deserialize.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.6/pgpubsub/tests/test_trigger_deserialize.py` & `django_pgpubsub-1.1.0/pgpubsub/tests/test_trigger_deserialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 from django.core.serializers.json import DjangoJSONEncoder
 from django.utils import timezone
 
 from pgpubsub import TriggerChannel
 from pgpubsub.models import Notification
 from pgpubsub.tests.channels import (
     AuthorTriggerChannel,
+    ChildTriggerChannel,
+    ChildOfAbstractTriggerChannel,
     MediaTriggerChannel,
     PostTriggerChannel,
 )
-from pgpubsub.tests.models import Post, Author, Media
+from pgpubsub.tests.models import Post, Author, Child, ChildOfAbstract, Media
 
 
 def test_deserialize_post_trigger_channel():
     @dataclass
     class MyChannel(TriggerChannel):
         model: Post
 
@@ -81,39 +83,44 @@
 
 @pytest.mark.django_db(transaction=True)
 def test_deserialize_edit_payload():
     media = Media.objects.create(
         name='avatar.jpg',
         content_type='image/png',
         size=15000,
+        store_id="some-value",
     )
     assert 1 == Notification.objects.all().count()
     insert_notification = Notification.from_channel(
         channel=MediaTriggerChannel).last()
 
     deserialized = MediaTriggerChannel.deserialize(
         insert_notification.payload)
 
     assert media.name == deserialized['new'].name
-    assert media.pk == deserialized['new'].id
+    assert media.pk == deserialized['new'].pk
+    assert media.key == deserialized['new'].key
     assert media.size == deserialized['new'].size
+    assert media.store_id == deserialized['new'].store_id
 
     media.name = 'avatar_2.jpg'
     media.save()
 
     assert 2 == Notification.objects.all().count()
     edit_notification = Notification.from_channel(
         channel=MediaTriggerChannel).last()
 
     deserialized = MediaTriggerChannel.deserialize(
         edit_notification.payload)
 
     assert deserialized['new'].name == media.name
-    assert deserialized['new'].id == media.pk
+    assert deserialized['new'].pk == media.pk
+    assert deserialized['new'].key == media.key
     assert deserialized['new'].size == media.size
+    assert media.store_id == deserialized['new'].store_id
 
 
 @pytest.mark.django_db(transaction=True)
 def test_deserialize_delete_payload():
     user = User.objects.create(username='Billy')
     author = Author.objects.create(name='Billy', user=user)
 
@@ -133,7 +140,27 @@
         delete_notification.payload)
 
     assert deserialized['old'].author == post.author
     assert deserialized['old'].date.date() == post.date.date()
     assert deserialized['old'].date.time() == post.date.time()
     assert deserialized['old'].id == original_id
     assert deserialized['new'] is None
+
+
+@pytest.mark.django_db(transaction=True)
+@pytest.mark.parametrize(
+    "cls,trigger_channel_cls",
+    [
+        (Child, ChildTriggerChannel),
+        (ChildOfAbstract, ChildOfAbstractTriggerChannel)
+    ]
+)
+def test_deserialize_child_payload(cls, trigger_channel_cls):
+    child = cls.objects.create()
+
+    assert 1 == Notification.objects.all().count()
+    insert_notification = Notification.from_channel(channel=trigger_channel_cls).last()
+
+    deserialized = trigger_channel_cls.deserialize(insert_notification.payload)
+
+    assert child.pk == deserialized['new'].pk
+    assert child.key == deserialized['new'].key
```

### Comparing `django_pgpubsub-1.0.6/pgpubsub/triggers.py` & `django_pgpubsub-1.1.0/pgpubsub/triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,13 +29,12 @@
                 'old', row_to_json(OLD),
                 'new', row_to_json(NEW)
               );
         '''
 
 
 class LockableNotify(Notify):
-
     def _pre_notify(self):
         return f'''
             INSERT INTO pgpubsub_notification (channel, payload)
             VALUES ('{self.name}', to_json(payload::text));
         '''
```

### Comparing `django_pgpubsub-1.0.6/pyproject.toml` & `django_pgpubsub-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fail_under = 100
 
 [tool.poetry]
 name = "django-pgpubsub"
 packages = [
   { include = "pgpubsub" }
 ]
-version = "1.0.6"
+version = "1.1.0"
 description = "A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
@@ -46,15 +46,15 @@
 homepage = "https://github.com/Opus10/django-pgpubsub"
 repository = "https://github.com/Opus10/django-pgpubsub"
 documentation = "https://django-pgpubsub.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 django = ">=2"
-django-pgtrigger = ">=2.4.0"
+django-pgtrigger = ">=4.6.0"
 
 [tool.poetry.dev-dependencies]
 black = "21.5b1"
 dj-database-url = "0.5.0"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
@@ -79,8 +79,12 @@
 zipp = "3.4.1"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 addopts = "--reuse-db"
 testpaths = "pgpubsub/tests"
 norecursedirs = ".venv"
+log_cli = true
+log_cli_level = "INFO"
 DJANGO_SETTINGS_MODULE = "settings"
+filterwarnings = ["ignore::DeprecationWarning:django.http.request:",
+    "ignore::DeprecationWarning:django.utils.encoding:"]
```

### Comparing `django_pgpubsub-1.0.6/PKG-INFO` & `django_pgpubsub-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgpubsub
-Version: 1.0.6
+Version: 1.1.0
 Summary: A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol.
 Home-page: https://github.com/Opus10/django-pgpubsub
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
-Requires-Dist: django-pgtrigger (>=2.4.0)
+Requires-Dist: django-pgtrigger (>=4.6.0)
 Project-URL: Documentation, https://django-pgpubsub.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgpubsub
 Description-Content-Type: text/markdown
 
 django-pgpubsub
 ===============
 
@@ -340,14 +336,55 @@
 pre-creation (and would hence be ``None``) and ``new`` would refer to a copy of
 the newly created ``Author`` instance. This payload is inspired by the ``OLD``
 and ``NEW`` values available in the postgres ``CREATE TRIGGER`` statement
 (https://www.postgresql.org/docs/9.1/sql-createtrigger.html). The only custom
 logic we need to define on a trigger channel is the ``model`` class-level
 attribute.
 
+** Models migrations **
+
+Note that the payload captures the snapshot of the ``Author`` instance for some
+time. Later it will be deserialized (see more about this below in the
+Listeners section). It may happen that by that time the ``Author`` model is
+migrated in django and this requires careful handling to make sure the payload
+can still be deserialized and processed. Special handling is required when the
+migration is backward incompatible like making existing field mandatory.
+
+Let's look to the example how to do that and what tooling ``pgpubsub`` provides
+to facilitate that. Let's says we want to add a new mandatory text field
+``email`` to ``Author``.
+
+This is done in three steps (releases):
+
+1. New optional field is added. Application is modified so that new records
+   always get a value in ``email`` field.
+2. Values are populated in the existing records.
+3. Fields is made mandatory.
+
+Note that before release 2 is deployed and the migration that populates the
+field is applied modifications to some ``Author`` entities would produce
+payloads that do not have value in the ``email`` field.
+
+When release 3 is deployed the application may assume that every ``Author`` has
+``email``. The problem is that the notifications produced before release 2 is
+deployed may be still not processed (for example the listener process was not
+run or there was an issue with the processing of some specific notification and
+it was skipped). In order to safely deploy release 3 the deployer need to know
+if there are any notifications that were created before django migrations of
+the release 2 were applied.
+
+To facilitate this ``Notification`` entity stores ``db_version`` field which
+contains the latest migration identier for the django app the ``Author`` is
+defined in. The deployer may check if there are any notifications with the old
+``db_version`` before deploying version that potentially breaks backward
+compatibility in terms of the data structure. 
+
+In this case deployer should check that there are no ``Notification`` entities
+with ``db_version`` before the version that was assigned to the migrations in
+release 2.
 
 Listeners
 --------
 
 In the ``pgpubsub`` library, a *listener* is the function
 which processes notifications sent through some particular channel.
 
@@ -659,14 +696,33 @@
 to be processed. This allows to recover from scenarios like the one in the paragraph described
 above.
 
 Note that this recovery option can be enabled whenever we use the `listen` management command
 by supplying it with the `--recover` option. This will tell the listening processes to replay
 any missed stored notifications automatically when it starts up.
 
+It is important to enable server side cursors in the django settings used by
+the listener. Their usage makes memory consumption much lower during the
+recovery and that is important if there is a need to recover many notifications:
+
+```
+DATABASES = {
+    "default": {
+        "ENGINE": "django.db.backends.postgresql",
+        ...,
+        "DISABLE_SERVER_SIDE_CURSORS": False,
+    }
+}
+```
+
+or if ``dj_database_url`` is used:
+```
+DATABASES = {'default': dj_database_url.config()}
+DATABASES['default']["DISABLE_SERVER_SIDE_CURSORS"] = False
+```
 
 Live Demos
 ==========
 
 `bulk_create` over several processes
 ------------------------------------
```

