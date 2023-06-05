# Comparing `tmp/smarthouse-0.1.2.tar.gz` & `tmp/smarthouse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarthouse-0.1.2.tar", last modified: Wed May 17 16:28:22 2023, max compression
+gzip compressed data, was "smarthouse-0.1.3.tar", last modified: Mon Jun  5 12:49:18 2023, max compression
```

## Comparing `smarthouse-0.1.2.tar` & `smarthouse-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.365688 smarthouse-0.1.2/
--rw-r--r--   0 ivan       (501) staff       (20)     4845 2023-05-17 16:28:22.362554 smarthouse-0.1.2/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     4306 2023-05-17 16:27:56.000000 smarthouse-0.1.2/README.md
--rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.2/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-17 16:28:22.366019 smarthouse-0.1.2/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-05-17 16:27:56.000000 smarthouse-0.1.2/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.353646 smarthouse-0.1.2/smarthouse/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/action_decorators.py
--rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.2/smarthouse/app.py
--rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/device.py
--rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/device_generator.py
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/logger.py
--rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/storage.py
--rw-r--r--   0 ivan       (501) staff       (20)     8436 2023-05-17 16:27:56.000000 smarthouse-0.1.2/smarthouse/telegram_client.py
--rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.360947 smarthouse-0.1.2/smarthouse.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     4845 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      290 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       11 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.144427 smarthouse-0.1.3/
+-rw-r--r--   0 ivan       (501) staff       (20)     4918 2023-06-05 12:49:18.143894 smarthouse-0.1.3/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     4379 2023-05-17 16:35:41.000000 smarthouse-0.1.3/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.3/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-06-05 12:49:18.144702 smarthouse-0.1.3/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-06-05 12:48:54.000000 smarthouse-0.1.3/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.138275 smarthouse-0.1.3/smarthouse/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/action_decorators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.3/smarthouse/app.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/device.py
+-rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/device_generator.py
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/logger.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/storage.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8195 2023-06-05 12:47:44.000000 smarthouse-0.1.3/smarthouse/telegram_client.py
+-rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.142514 smarthouse-0.1.3/smarthouse.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     4918 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-06-05 12:49:18.000000 smarthouse-0.1.3/smarthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      290 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       11 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/top_level.txt
```

### Comparing `smarthouse-0.1.2/PKG-INFO` & `smarthouse-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Smart House Scenarios
 Home-page: UNKNOWN
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,15 @@
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
 * Доведение устройств до конечного состояния (проверяет с сервера)
 * Введение устройств в карантин, если они не отвечают или как-то еще сломаны, таким образом, чтобы сценарии продолжали работать корректно
 * При быстром выводе из карантина (происходит опрос устройства) после последней команды доведет устройство до состояния с последней команды
+* Хранение последних данных с устройств
 * Система lock'ов устройств
 * Обнаружение человеческого вмешательства и установка lock'ов, от сценариев на настроенное время
 * Легкое хранилище данных в файле
 * Интеграция с web для управления
 * Интеграция с tg ботом для сообщений об ошибках и управлением
 
 Quick start
```

### Comparing `smarthouse-0.1.2/README.md` & `smarthouse-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
 * Доведение устройств до конечного состояния (проверяет с сервера)
 * Введение устройств в карантин, если они не отвечают или как-то еще сломаны, таким образом, чтобы сценарии продолжали работать корректно
 * При быстром выводе из карантина (происходит опрос устройства) после последней команды доведет устройство до состояния с последней команды
+* Хранение последних данных с устройств
 * Система lock'ов устройств
 * Обнаружение человеческого вмешательства и установка lock'ов, от сценариев на настроенное время
 * Легкое хранилище данных в файле
 * Интеграция с web для управления
 * Интеграция с tg ботом для сообщений об ошибках и управлением
 
 Quick start
```

### Comparing `smarthouse-0.1.2/pyproject.toml` & `smarthouse-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/setup.py` & `smarthouse-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-dotenv",
     ]
 }
 
 
 setup(
     name="smarthouse",
-    version="0.1.2",
+    version="0.1.3",
     description="Smart House Scenarios",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://smarthouse.readthedocs.io/",
     author="Ivan Kriuchkov",
     author_email="vivenchik@gmail.com",
     license="MIT",
```

### Comparing `smarthouse-0.1.2/smarthouse/action_decorators.py` & `smarthouse-0.1.3/smarthouse/action_decorators.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/smarthouse/app.py` & `smarthouse-0.1.3/smarthouse/app.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/smarthouse/device.py` & `smarthouse-0.1.3/smarthouse/device.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/smarthouse/storage.py` & `smarthouse-0.1.3/smarthouse/storage.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/smarthouse/telegram_client.py` & `smarthouse-0.1.3/smarthouse/telegram_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,69 +70,68 @@
             return
         message = message.rstrip("\n").strip()
         _exc: Optional[Exception] = None
         done = False
         for _ in range(20):
             response_message_id = None
             async with self._w_lock:
-                async with self._bot:
-                    try:
+                try:
+                    async with self._bot:
                         response = await self._bot.send_message(
                             text=message,
                             chat_id=self._chat_id,
                             disable_notification=True,
                             reply_to_message_id=replay_message_id,
                             read_timeout=10,
                         )
                         done = True
                         response_message_id = response.message_id
                         await asyncio.sleep(0.5)
                         break
-                    except httpx.ReadError as exc:
-                        _exc = exc
-                    except telegram.error.BadRequest as exc:
-                        if exc.message == "Message is too long":
-                            sep = len(message) // 2
-                            new_lines = [m.end() for m in re.finditer("\n", message)]
-                            if new_lines:
-                                old_line = 0
-                                cur_line = 0
-                                for new_line in new_lines:
-                                    old_line = cur_line
-                                    cur_line = new_line
-                                    if cur_line >= len(message) / 2:
-                                        break
-
-                                if cur_line - len(message) / 2 > len(message) / 2 - old_line:
-                                    sep = old_line
-                                else:
-                                    sep = cur_line
-
-                            await self.write_tg(
-                                message[:sep],
-                                replay_message_id=replay_message_id,
-                                to_delete=to_delete,
-                                to_delete_timestamp=to_delete_timestamp,
-                            )
-                            await self.write_tg(
-                                message[sep:],
-                                replay_message_id=replay_message_id,
-                                to_delete=to_delete,
-                                to_delete_timestamp=to_delete_timestamp,
-                            )
-                            return
-                        elif exc.message == "Message text is empty":
-                            pass
-                        else:
-                            await asyncio.sleep(1)
-
-                    except (telegram.error.NetworkError, telegram.error.TimedOut):
+                except (telegram.error.NetworkError, telegram.error.TimedOut):
+                    pass
+                except httpx.ReadError as exc:
+                    _exc = exc
+                except telegram.error.BadRequest as exc:
+                    if exc.message == "Message is too long":
+                        sep = len(message) // 2
+                        new_lines = [m.end() for m in re.finditer("\n", message)]
+                        if new_lines:
+                            old_line = 0
+                            cur_line = 0
+                            for new_line in new_lines:
+                                old_line = cur_line
+                                cur_line = new_line
+                                if cur_line >= len(message) / 2:
+                                    break
+
+                            if cur_line - len(message) / 2 > len(message) / 2 - old_line:
+                                sep = old_line
+                            else:
+                                sep = cur_line
+
+                        await self.write_tg(
+                            message[:sep],
+                            replay_message_id=replay_message_id,
+                            to_delete=to_delete,
+                            to_delete_timestamp=to_delete_timestamp,
+                        )
+                        await self.write_tg(
+                            message[sep:],
+                            replay_message_id=replay_message_id,
+                            to_delete=to_delete,
+                            to_delete_timestamp=to_delete_timestamp,
+                        )
+                        return
+                    elif exc.message == "Message text is empty":
                         pass
-                    except Exception as exc:
-                        _exc = exc
+                    else:
+                        await asyncio.sleep(1)
+                except Exception as exc:
+                    _exc = exc
 
         if _exc is not None:
             raise _exc
         if not done:
             raise TGException("try again")
 
         if to_delete:
@@ -149,75 +148,75 @@
     async def write_tg_document(self, document):
         if not self._prod or self.telegram_token is None:
             return
 
         _exc = None
         for _ in range(20):
             async with self._w_lock:
-                async with self._bot:
-                    try:
+                try:
+                    async with self._bot:
                         await self._bot.send_document(
                             chat_id=self._chat_id,
                             document=document,
                             disable_notification=True,
                             read_timeout=10,
                         )
                         return
-                    except (httpx.ReadError, telegram.error.BadRequest) as exc:
-                        _exc = exc
-                    except (telegram.error.NetworkError, telegram.error.TimedOut):
-                        pass
-                    except Exception as exc:
-                        _exc = exc
+                except (telegram.error.NetworkError, telegram.error.TimedOut):
+                    pass
+                except (httpx.ReadError, telegram.error.BadRequest) as exc:
+                    _exc = exc
+                except Exception as exc:
+                    _exc = exc
 
         if _exc is not None:
             raise _exc
         raise TGException("try again")
 
     async def delete_message(self, message_id=None):
         if not self._prod or self.telegram_token is None:
             return
 
         _exc = None
         for _ in range(20):
             async with self._w_lock:
-                async with self._bot:
-                    try:
+                try:
+                    async with self._bot:
                         await self._bot.delete_message(chat_id=self._chat_id, message_id=message_id, read_timeout=10)
                         return
-                    except httpx.ReadError as exc:
-                        _exc = exc
-                    except telegram.error.BadRequest as exc:
-                        if exc.message == "Message to delete not found":
-                            pass
-                    except (telegram.error.NetworkError, telegram.error.TimedOut):
+                except (telegram.error.NetworkError, telegram.error.TimedOut):
+                    pass
+                except telegram.error.BadRequest as exc:
+                    if exc.message == "Message to delete not found":
                         pass
-                    except Exception as exc:
-                        _exc = exc
+                except httpx.ReadError as exc:
+                    _exc = exc
+                except Exception as exc:
+                    _exc = exc
 
         if _exc is not None:
             raise _exc
         raise TGException("try again")
 
     async def update_tg(self):
         if not self._prod or self.telegram_token is None:
             return
         storage = Storage()
         updates = []
         async with self._r_lock:
-            async with self._bot:
-                try:
+            try:
+                async with self._bot:
                     updates = await self._bot.get_updates(
                         offset=storage.get(SKeys.offset_tg), timeout=10, read_timeout=10
                     )
-                except (httpx.ReadError, telegram.error.BadRequest) as exc:
-                    raise exc
-                except (telegram.error.NetworkError, telegram.error.TimedOut):
-                    pass
-                except Exception as exc:
-                    raise exc
+            except (telegram.error.NetworkError, telegram.error.TimedOut):
+                pass
+            except (httpx.ReadError, telegram.error.BadRequest) as exc:
+                raise exc
+            except Exception as exc:
+                raise exc
 
         for update in updates:
             storage.put(SKeys.offset_tg, update.update_id + 1)
             if str(update.message.chat_id) == self._chat_id:
                 message = update.message.text
                 await self.get_handler(message)(self, update)
```

### Comparing `smarthouse-0.1.2/smarthouse/utils.py` & `smarthouse-0.1.3/smarthouse/utils.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.2/smarthouse.egg-info/PKG-INFO` & `smarthouse-0.1.3/smarthouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Smart House Scenarios
 Home-page: UNKNOWN
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,15 @@
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
 * Доведение устройств до конечного состояния (проверяет с сервера)
 * Введение устройств в карантин, если они не отвечают или как-то еще сломаны, таким образом, чтобы сценарии продолжали работать корректно
 * При быстром выводе из карантина (происходит опрос устройства) после последней команды доведет устройство до состояния с последней команды
+* Хранение последних данных с устройств
 * Система lock'ов устройств
 * Обнаружение человеческого вмешательства и установка lock'ов, от сценариев на настроенное время
 * Легкое хранилище данных в файле
 * Интеграция с web для управления
 * Интеграция с tg ботом для сообщений об ошибках и управлением
 
 Quick start
```

