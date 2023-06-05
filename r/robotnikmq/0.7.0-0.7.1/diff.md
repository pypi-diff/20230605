# Comparing `tmp/robotnikmq-0.7.0.tar.gz` & `tmp/robotnikmq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotnikmq-0.7.0.tar", last modified: Sun Apr 23 03:35:23 2023, max compression
+gzip compressed data, was "robotnikmq-0.7.1.tar", last modified: Mon Jun  5 00:04:12 2023, max compression
```

## Comparing `robotnikmq-0.7.0.tar` & `robotnikmq-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.7.0/LICENSE
--rw-r--r--   0        0        0     6284 2023-04-23 03:34:39.968822 robotnikmq-0.7.0/README.md
--rw-r--r--   0        0        0     1299 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0      364 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/__init__.py
--rwxr-xr-x   0        0        0     6280 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/config.py
--rw-r--r--   0        0        0     6434 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/core.py
--rwxr-xr-x   0        0        0      652 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/error.py
--rw-r--r--   0        0        0      325 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/log.py
--rw-r--r--   0        0        0     2543 2023-04-23 03:34:39.984822 robotnikmq-0.7.0/robotnikmq/rpc_client.py
--rw-r--r--   0        0        0    11527 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/rpc_server.py
--rw-r--r--   0        0        0     4397 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/subscriber.py
--rwxr-xr-x   0        0        0     2055 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/topic.py
--rw-r--r--   0        0        0      471 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/robotnikmq/utils.py
--rw-r--r--   0        0        0      364 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      454 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/conftest.py
--rwxr-xr-x   0        0        0    14200 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0    13569 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/test_rpc.py
--rw-r--r--   0        0        0      622 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/integration/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.7.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4105 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_config.py
--rw-r--r--   0        0        0      261 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_error.py
--rw-r--r--   0        0        0     1818 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_message.py
--rw-r--r--   0        0        0     1292 2023-04-23 03:34:39.988822 robotnikmq-0.7.0/tests/unit/test_validation.py
--rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 robotnikmq-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6284 2023-04-25 15:42:45.413531 robotnikmq-0.7.1/README.md
+-rw-r--r--   0        0        0     1299 2023-06-04 22:11:58.368533 robotnikmq-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2023-04-25 15:42:45.413531 robotnikmq-0.7.1/robotnikmq/__init__.py
+-rwxr-xr-x   0        0        0     6332 2023-06-04 23:19:49.578221 robotnikmq-0.7.1/robotnikmq/config.py
+-rw-r--r--   0        0        0     6920 2023-06-04 23:51:05.567909 robotnikmq-0.7.1/robotnikmq/core.py
+-rwxr-xr-x   0        0        0      652 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/robotnikmq/error.py
+-rw-r--r--   0        0        0      325 2023-04-25 15:42:45.417532 robotnikmq-0.7.1/robotnikmq/log.py
+-rw-r--r--   0        0        0     2485 2023-06-04 23:21:22.614467 robotnikmq-0.7.1/robotnikmq/rpc_client.py
+-rw-r--r--   0        0        0    11950 2023-06-04 23:37:29.062585 robotnikmq-0.7.1/robotnikmq/rpc_server.py
+-rw-r--r--   0        0        0     4402 2023-06-04 22:59:50.487503 robotnikmq-0.7.1/robotnikmq/subscriber.py
+-rwxr-xr-x   0        0        0     2065 2023-06-04 22:51:58.781977 robotnikmq-0.7.1/robotnikmq/topic.py
+-rw-r--r--   0        0        0      471 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/robotnikmq/utils.py
+-rw-r--r--   0        0        0      364 2023-04-25 15:42:45.417532 robotnikmq-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-18 03:25:43.096855 robotnikmq-0.7.1/tests/integration/conftest.py
+-rwxr-xr-x   0        0        0    14263 2023-06-04 23:50:38.922690 robotnikmq-0.7.1/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0    13569 2023-04-18 03:25:43.096855 robotnikmq-0.7.1/tests/integration/test_rpc.py
+-rw-r--r--   0        0        0      622 2023-04-18 03:25:43.096855 robotnikmq-0.7.1/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4105 2023-04-18 03:25:43.096855 robotnikmq-0.7.1/tests/unit/test_config.py
+-rw-r--r--   0        0        0      261 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/tests/unit/test_error.py
+-rw-r--r--   0        0        0     1853 2023-06-04 23:16:59.402456 robotnikmq-0.7.1/tests/unit/test_message.py
+-rw-r--r--   0        0        0     1292 2022-12-29 00:46:05.562203 robotnikmq-0.7.1/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 robotnikmq-0.7.1/PKG-INFO
```

### Comparing `robotnikmq-0.7.0/LICENSE` & `robotnikmq-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/README.md` & `robotnikmq-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/pyproject.toml` & `robotnikmq-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "robotnikmq"
-version = "0.7.0"
+version = "0.7.1"
 description = "Utilities for safe, efficient, and scalable infrastructure using RabbitMQ"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
-    "typeguard>=3.0.2",
+    "typeguard>=4.0.0",
     "pyyaml>=6.0",
     "pydantic>=1.0",
     "pika>=1.3.0",
     "funcy>=1.17",
     "arrow>=1.2.3",
     "types-pika>=1.2.0b1",
     "types-pyyaml>=6.0.11",
```

### Comparing `robotnikmq-0.7.0/robotnikmq/config.py` & `robotnikmq-0.7.1/robotnikmq/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions and objects related to the Configuration of RobotnikMQ
 """
 from pathlib import Path
 from random import choice
 from ssl import create_default_context
-from typing import Union, List, Optional, Dict, Any
+from typing import Union, List, Optional, Dict, Any, TypedDict
 
 from pika import ConnectionParameters, SSLOptions  # type: ignore
 from pika.credentials import PlainCredentials  # type: ignore
 from pydantic import BaseModel  # type: ignore
 from pydantic import validator
 from typeguard import typechecked
 from yaml import safe_load  # type: ignore
@@ -160,39 +160,39 @@
 def conn_config(attempts: int, min_wait: int, max_wait: int) -> ConnectionConfig:
     return ConnectionConfig(
         attempts=attempts,
         wait_random_min_seconds=min_wait,
         wait_random_max_seconds=max_wait,
     )
 
+@typechecked
+class RobotnikConfigTypedDict(TypedDict):
+    tiers: List[List[Dict]]
+    connection: Dict
 
+@typechecked
 class RobotnikConfig(BaseModel):
     tiers: List[List[ServerConfig]]
     connection: ConnectionConfig = ConnectionConfig()
 
-    @typechecked
     def tier(self, index: int) -> List[ServerConfig]:
         return self.tiers[index]
 
-    @typechecked
     def a_server(self, tier: int) -> ServerConfig:
         return choice(self.tier(tier))
 
-    @typechecked
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> RobotnikConfigTypedDict:
         return self.dict()
 
-    @typechecked
     @staticmethod
     def from_tiered(
         tiers: List[List[ServerConfig]],
     ) -> "RobotnikConfig":
         return RobotnikConfig(tiers=tiers)
 
-    @typechecked
     @staticmethod
     def from_connection_params(conn_params: ConnectionParameters) -> "RobotnikConfig":
         return RobotnikConfig(
             tiers=[[ServerConfig.from_connection_params(conn_params)]]
         )
```

### Comparing `robotnikmq-0.7.0/robotnikmq/core.py` & `robotnikmq-0.7.1/robotnikmq/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from contextlib import contextmanager
+from dataclasses import dataclass
 from datetime import datetime
 from json import loads as _from_json
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from random import sample
 from threading import current_thread
-from typing import Optional, Callable, Any, Dict, Union, Generator, List
+from typing import Optional, Callable, Any, Dict, Union, Generator, List, TypedDict
 from uuid import uuid4 as uuid, UUID
 
 from arrow import Arrow, get as to_arrow, now
 from funcy import first
 from pika import BlockingConnection
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.exceptions import AMQPError, AMQPConnectionError
@@ -53,66 +54,77 @@
 def valid_json(string: str) -> bool:
     try:
         _from_json(string)
         return True
     except JSONDecodeError:
         return False
 
+@typechecked
+class MessageTypedDict(TypedDict):
+    contents: Dict[str, Any]
+    routing_key: Optional[str]
+    timestamp: Union[int, float]
+    msg_id: str
 
+@typechecked
+@dataclass(frozen=True)
 class Message:
-    @typechecked
-    def __init__(
-        self,
+    contents: Union[BaseModel, Dict[str, Any]]
+    routing_key: str
+    timestamp: Arrow
+    msg_id: Union[str, UUID]
+
+    @staticmethod
+    def of(
         contents: Union[BaseModel, Dict[str, Any]],
         routing_key: Optional[str] = None,
-        timestamp: Union[int, float, datetime, None] = None,
+        timestamp: Union[int, float, datetime, Arrow, None] = None,
         msg_id: Union[str, UUID, None] = None,
-    ):
-        self.msg_id = msg_id or uuid()
+    ) -> 'Message':
+        msg_id = msg_id or uuid()
         if not jsonable(contents):
             raise ValueError("Contents of message have to be JSON-serializeable")
-        self.contents = contents.dict() if isinstance(contents, BaseModel) else contents
-        self.routing_key: str = routing_key or ""
-        self.timestamp: Arrow = to_arrow(timestamp) if timestamp is not None else now()
+        contents = contents.dict() if isinstance(contents, BaseModel) else contents
+        routing_key: str = routing_key or ""
+        timestamp: Arrow = to_arrow(timestamp) if timestamp is not None else now()
+        return Message(contents, routing_key, timestamp, msg_id)
+
+    def with_routing_key(self, routing_key: Optional[str]) -> 'Message':
+        return Message.of(self.contents, routing_key, self.timestamp, self.msg_id)
 
-    @typechecked
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> MessageTypedDict:
         return {
             "routing_key": self.routing_key,
             "contents": self.contents,
             "msg_id": str(self.msg_id),
             "timestamp": self.timestamp.int_timestamp,
         }
 
-    @typechecked
     def to_json(self) -> str:
         return _to_json(self.to_dict())
 
     @staticmethod
-    @typechecked
-    def of(body: str) -> "Message":  # pylint: disable=C0103
+    def of_json(body: str) -> "Message":  # pylint: disable=C0103
         try:
             msg = _from_json(body)
-            return Message(
+            return Message.of(
                 msg["contents"], msg["routing_key"], msg["timestamp"], msg["msg_id"]
             )
         except (JSONDecodeError, KeyError) as exc:
             raise MalformedMessage(body) from exc
 
-    @typechecked
     def __getitem__(self, key: str) -> Any:
         return self.contents[key]
 
     def keys(self):
         return self.contents.keys()
 
     def values(self):
         return self.contents.values()
 
-    @typechecked
     def __contains__(self, item: str) -> bool:
         return item in self.contents
 
     def __iter__(self):
         return iter(self.contents)
 
     @property
```

### Comparing `robotnikmq-0.7.0/robotnikmq/error.py` & `robotnikmq-0.7.1/robotnikmq/error.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/robotnikmq/rpc_client.py` & `robotnikmq-0.7.1/robotnikmq/rpc_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,33 +6,31 @@
 from typeguard import typechecked
 
 from robotnikmq.core import Robotnik, RobotnikConfig
 from robotnikmq.rpc_server import RpcError, RpcResponse
 from robotnikmq.utils import to_json
 
 
+@typechecked
 class RpcClient(Robotnik):
-    @typechecked
     def __init__(self, config: Optional[RobotnikConfig] = None):
         super().__init__(config=config)
         self.response: Optional[Any] = None
         self.callback_queue = None
         self.corr_id = str(uuid())
 
-    @typechecked
     def _on_response(self, _, __, props: BasicProperties, body: bytes) -> None:
         self.response = body.decode() if self.corr_id == props.correlation_id else None
 
-    @typechecked
     def call(self, queue: str,
              args: Optional[Dict[str, Any]] = None,
              str_args: Optional[str] = None,
              timeout: Optional[float] = None,
              raise_on_error: bool = False) -> Union[RpcError, str, int, float,
-                                                    Dict[str, Any], List[Dict[str, Any]]]:
+                                                    Dict, List[Dict]]:
         with self.open_channel() as channel:
             result = channel.queue_declare(queue='', exclusive=True)
             self.callback_queue = result.method.queue
             channel.basic_consume(
                 queue=self.callback_queue,
                 on_message_callback=self._on_response,
                 auto_ack=True)
```

### Comparing `robotnikmq-0.7.0/robotnikmq/rpc_server.py` & `robotnikmq-0.7.1/robotnikmq/rpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from dataclasses import dataclass
 from inspect import signature, Parameter
 from json import loads as _from_json
 from traceback import format_exc
 from socket import gethostname
-from typing import Optional, Callable, Union, Any, Dict, Tuple, List
+from typing import Optional, Callable, Union, Any, Dict, Tuple, List, TypedDict, Type
 from typing import get_type_hints, get_origin, get_args
 from uuid import uuid4 as uuid, UUID
 
 from pika import BasicProperties
 from pika.exceptions import AMQPError, ChannelError, AMQPConnectionError
 from tenacity import retry, wait_exponential, retry_if_exception_type
 from typeguard import typechecked
@@ -19,79 +20,91 @@
 
 @typechecked
 def _type_hint_str(typ: Any) -> str:
     if get_origin(typ) is Union:
         return f"Union[{','.join([_type_hint_str(t) for t in get_args(typ)])}]"
     return str(typ.__name__)
 
+@typechecked
+class RpcErrorTypedDict(TypedDict):
+    request_id: str
+    type: str
+    details: Union[None, str, Dict[str, Any]]
 
+@typechecked
+@dataclass(frozen=True)
 class RpcError:
-    @typechecked
-    def __init__(
-        self,
+    request_id: Union[str, UUID]
+    details: Union[None, str, Dict[str, Any]]
+
+    @staticmethod
+    def of(
         request_id: Union[str, UUID, None] = None,
         details: Union[None, str, Dict[str, Any]] = None,
-    ):
-        self.request_id = request_id or uuid()
-        self.details = details
+    ) -> 'RpcError':
+        return RpcError(request_id or uuid(), details)
 
-    @typechecked
     def to_json(self) -> str:
         return _to_json(self.to_dict())
 
-    @typechecked
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> RpcErrorTypedDict:
         return {
             "request_id": str(self.request_id),
             "type": "error",
             "details": self.details,
         }
 
     @staticmethod
-    @typechecked
-    def from_json(json_str: Union[str, bytes]) -> Optional["RpcError"]:
+    def from_json(json_str: Union[str, bytes]) -> Optional['RpcError']:
         json_str = json_str if isinstance(json_str, str) else json_str.decode()
         log.debug(json_str)
         if valid_json(json_str):
             data = _from_json(json_str)
             if all(k in data for k in {"request_id", "type", "details"}):
-                return RpcError(request_id=data["request_id"], details=data["details"])
+                return RpcError.of(request_id=data["request_id"], details=data["details"])
         return None
 
 
+@typechecked
+class RpcResponseTypedDict(TypedDict):
+    request_id: str
+    type: str
+    data: Union[None, str, int, float, Dict[str, Any], List[Dict[str, Any]]]
+
+
+@typechecked
+@dataclass(frozen=True)
 class RpcResponse:
-    @typechecked
-    def __init__(
-        self,
+    request_id: Union[str, UUID]
+    data: Union[None, str, int, float, Dict[str, Any], List[Dict[str, Any]]]
+
+    @staticmethod
+    def of(
         request_id: Union[str, UUID, None] = None,
         data: Union[None, str, int, float, Dict[str, Any], List[Dict[str, Any]]] = None,
-    ):
-        self.request_id = request_id or uuid()
-        self.data = data
+    ) -> 'RpcResponse':
+        return RpcResponse(request_id or uuid(), data)
 
-    @typechecked
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> RpcResponseTypedDict:
         return {
             "request_id": str(self.request_id),
             "type": "response",
             "data": self.data,
         }
 
-    @typechecked
     def to_json(self) -> str:
         return _to_json(self.to_dict())
 
     @staticmethod
-    @typechecked
     def from_json(json_str: Union[str, bytes]) -> Optional["RpcResponse"]:
         json_str = json_str if isinstance(json_str, str) else json_str.decode()
         if valid_json(json_str):
             data = _from_json(json_str)
             if all(k in data for k in ("request_id", "type", "data")):
-                return RpcResponse(request_id=data["request_id"], data=data["data"])
+                return RpcResponse.of(request_id=data["request_id"], data=data["data"])
         return None
 
 
 class RpcServer(Robotnik):
     @typechecked
     def __init__(
         self,
@@ -112,15 +125,15 @@
         self.channel.queue_declare(
             queue=queue + self.docs_queue_suffix, exclusive=False
         )
 
         @typechecked
         def docs_callback(_, method, props: BasicProperties, __) -> None:
             req_id = props.correlation_id or uuid()
-            response = RpcResponse(
+            response = RpcResponse.of(
                 req_id,
                 data={
                     "rpc_queue": queue,
                     "inputs": self._get_input_type_strings(queue),
                     "returns": self._get_return_type_str(queue),
                     "description": callback.__doc__,
                 },
@@ -136,49 +149,49 @@
         self.channel.basic_consume(
             queue=queue + self.docs_queue_suffix,
             on_message_callback=docs_callback,
             auto_ack=False,
         )
 
     @typechecked
-    def _get_defaults(self, queue: str) -> Dict[str, Any]:
+    def _get_defaults(self, queue: str) -> Dict:
         params = signature(self._callbacks[queue]).parameters
         return {
             p: params[p].default
             for p in params
             if params[p].default is not Parameter.empty
         }
 
     @typechecked
-    def _get_input_types(self, queue: str) -> Dict[str, Any]:
+    def _get_input_types(self, queue: str) -> Dict:
         return {
             k: v
             for k, v in get_type_hints(self._callbacks[queue]).items()
             if k != "return"
         }
 
     @typechecked
-    def _get_input_type_strings(self, queue: str) -> Dict[str, Any]:
+    def _get_input_type_strings(self, queue: str) -> Dict:
         return {
             k: _type_hint_str(v)
             for k, v in get_type_hints(self._callbacks[queue]).items()
             if k != "return"
         }
 
     @typechecked
     def _get_return_type_str(self, queue: str) -> Any:
         return _type_hint_str(get_type_hints(self._callbacks[queue])["return"])
 
-    @staticmethod
     @typechecked
+    @staticmethod
     def _is_optional(arg_type: Any) -> bool:
         return get_origin(arg_type) is Union and type(None) in get_args(arg_type)
 
-    @staticmethod
     @typechecked
+    @staticmethod
     def _valid_arg(arg_value: Any, arg_type: Any) -> bool:
         if arg_type is Any:
             return True
         if get_origin(arg_type) is Union:
             if (type(None) in get_args(arg_type)) and (
                 arg_value is None or arg_value == {}
             ):  # Optional
@@ -189,18 +202,15 @@
         if get_origin(arg_type) is dict:
             key_type, val_type = get_args(arg_type)
             return all(
                 RpcServer._valid_arg(key, key_type) for key in arg_value.keys()
             ) and all(RpcServer._valid_arg(val, val_type) for val in arg_value.values())
         return isinstance(arg_value, arg_type)
 
-    @typechecked
-    def _valid_inputs(
-        self, queue: str, inputs: Dict[str, Any]
-    ) -> Tuple[bool, Optional[str]]:
+    def _valid_inputs(self, queue: str, inputs: Dict[str, Any]) -> Tuple[bool, Optional[str]]:
         inputs_with_defaults = {**self._get_defaults(queue), **inputs}
         for arg_name, arg_type in self._get_input_types(queue).items():
             if arg_name not in inputs_with_defaults and not self._is_optional(arg_type):
                 return False, f"Missing required argument {arg_name}"
             if arg_name in inputs_with_defaults and not self._valid_arg(
                 inputs_with_defaults[arg_name], arg_type
             ):
@@ -221,43 +231,43 @@
         def meta_callback(_, method, props: BasicProperties, body: bytes):
             req_id = props.correlation_id or uuid()
             with thread_name(req_id):
                 self.log.debug("Request received")
                 try:
                     try:
                         if valid_json(body.decode()):
-                            input_args: Dict[str, Any] = _from_json(body.decode())
+                            input_args: Dict = _from_json(body.decode())
                             self.log.debug(f"Input JSON is valid: {input_args}")
                             valid_inputs, msg = self._valid_inputs(queue, input_args)
                             if not valid_inputs:
                                 self.log.debug("Invalid input")
-                                response = RpcError(req_id, msg).to_json()
+                                response = RpcError.of(req_id, msg).to_json()
                             elif not input_args:
                                 self.log.debug(f"Executing: {callback}")
-                                response = RpcResponse(req_id, callback()).to_json()
+                                response = RpcResponse.of(req_id, callback()).to_json()
                             else:
                                 self.log.debug(
                                     f"Executing: {callback} with inputs: {input_args}"
                                 )
-                                response = RpcResponse(
+                                response = RpcResponse.of(
                                     req_id, callback(**input_args)
                                 ).to_json()
                         else:
-                            response = RpcError(
+                            response = RpcError.of(
                                 req_id, "Input could not be decoded as JSON"
                             ).to_json()
                     except (AMQPError, ChannelError):
                         raise  # we want this kind of exception to be caught further down
                     except Exception:  # pylint: disable=W0703
                         self.log.error(
                             "An error has occurred during the execution of the RPC method"
                         )
                         for line in format_exc().split("\n"):
                             self.log.error(line)
-                        response = RpcError(
+                        response = RpcError.of(
                             request_id=req_id,
                             details=f"There was an error "
                             f"while processing the "
                             f"request, please refer "
                             f"to server log with "
                             f"request ID: "
                             f"{req_id}",
```

### Comparing `robotnikmq-0.7.0/robotnikmq/subscriber.py` & `robotnikmq-0.7.1/robotnikmq/subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     queue=queue_name,  # pragma: no cover
                     auto_ack=False,
                     inactivity_timeout=inactivity_timeout,
                 ):
                     if method and body:
                         channel.basic_ack(delivery_tag=method.delivery_tag or 0)
                         try:
-                            yield Message.of(body.decode())
+                            yield Message.of_json(body.decode())
                         except MalformedMessage:
                             self.log.debug(format_exc())
                     else:
                         yield None
             finally:
                 try:
                     channel.cancel()
```

### Comparing `robotnikmq-0.7.0/robotnikmq/topic.py` & `robotnikmq-0.7.1/robotnikmq/topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         Args:
             msg (Message): The message to be broadcast.
             routing_key (Optional[str], optional): Routing key used to broadcast the message.
                                                    Defaults to an empty string.
             on_msg_error (AMQPErrorCallback, optional): _description_. Defaults to None.
         """
-        msg.routing_key = routing_key or msg.routing_key or ""
+        msg = msg.with_routing_key(routing_key or msg.routing_key or "")
         self.log.info("Broadcasting message (routing-key: [{}]):\n{}",
                       msg.routing_key, json.dumps(msg.to_dict(), indent=4))
         self.channel.basic_publish(
             exchange=self.exchange,
             routing_key=msg.routing_key,
             body=json.dumps(msg.to_dict()),
         )
```

### Comparing `robotnikmq-0.7.0/tests/integration/test_broadcast.py` & `robotnikmq-0.7.1/tests/integration/test_broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     pass
 else:
     cleanup_on_sigterm()
 
 
 def test_basic_broadcast(robotnikmq_config):
     topic = Topic(META_QUEUE, robotnikmq_config)
-    topic.broadcast(Message({"stuff": "Hello world!"}))
+    topic.broadcast(Message.of({"stuff": "Hello world!"}))
 
 
 # TODO: Figure out how to turn testcontainer on and off to test failure modes and reconnecting
 
 
 def test_unable_to_connect():
     config = RobotnikConfig(
@@ -40,15 +40,15 @@
                 server_config("127.0.0.1", 1, "", "", ""),
                 server_config("127.0.0.2", 1, "1", "1", "1"),
             ]
         ],
     )
     with raises(UnableToConnect) as exc:
         medium = Topic(META_QUEUE, config)
-        medium.broadcast(Message({"stuff": "Hello world!"}))
+        medium.broadcast(Message.of({"stuff": "Hello world!"}))
     log.debug(str(exc))
     log.debug(str(exc.value))
 
 
 def test_basic_broadcast_receive(robotnikmq_config):
     msg_received = Event()
 
@@ -61,15 +61,15 @@
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Hello world!"}))
+        medium.broadcast(Message.of({"stuff": "Hello world!"}))
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc = Process(target=pub)
     pub_proc.start()
     assert msg_received.wait(timeout=5)
     pub_proc.terminate()
@@ -144,18 +144,18 @@
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "first message"}))
+        medium.broadcast(Message.of({"stuff": "first message"}))
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "second message"})
+            Message.of({"stuff": "second message"})
         )  # this message should not be received
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc = Process(target=pub)
     pub_proc.start()
     assert first_msg_received.wait(timeout=1)
@@ -168,15 +168,15 @@
 def test_basic_broadcast_consume(robotnikmq_config):
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Hello world!"}))
+        medium.broadcast(Message.of({"stuff": "Hello world!"}))
 
     pub_proc = Process(target=pub)
     pub_proc.start()
     stream = (
         Subscriber(config=robotnikmq_config)
         .bind(exchange=META_QUEUE)
         .consume(inactivity_timeout=0.1)
@@ -196,15 +196,15 @@
             exchange=META_QUEUE,
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.channel.basic_publish(
             exchange=META_QUEUE, routing_key="", body=json.dumps({"stuff": "MALFORMED"})
         )
-        medium.broadcast(Message({"stuff": "Hello world!"}))
+        medium.broadcast(Message.of({"stuff": "Hello world!"}))
 
     pub_proc = Process(target=pub)
     pub_proc.start()
     for msg in (
         Subscriber(config=robotnikmq_config)
         .bind(exchange=META_QUEUE)
         .consume(inactivity_timeout=0.1)
@@ -233,34 +233,34 @@
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (1)"}), routing_key="stuff.something"
+            Message.of({"stuff": "Hello world! (1)"}), routing_key="stuff.something"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (2)"}), routing_key="stuff.nothing"
+            Message.of({"stuff": "Hello world! (2)"}), routing_key="stuff.nothing"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
+        medium.broadcast(Message.of({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
     pub_proc1.start()
     pub_proc2 = Process(target=pub2)
     pub_proc2.start()
@@ -302,44 +302,44 @@
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (1)"}), routing_key="message.1"
+            Message.of({"stuff": "Hello world! (1)"}), routing_key="message.1"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (2)"}), routing_key="message.2"
+            Message.of({"stuff": "Hello world! (2)"}), routing_key="message.2"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (3)"}), routing_key="message.3"
+            Message.of({"stuff": "Hello world! (3)"}), routing_key="message.3"
         )
 
     def pub_bad():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
+        medium.broadcast(Message.of({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
     pub_proc1.start()
     pub_proc2 = Process(target=pub2)
     pub_proc2.start()
@@ -387,44 +387,44 @@
     def pub1():
         medium = Topic(
             exchange="stuff.1",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (1)"}), routing_key="message.1"
+            Message.of({"stuff": "Hello world! (1)"}), routing_key="message.1"
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.2",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (2)"}), routing_key="message.2"
+            Message.of({"stuff": "Hello world! (2)"}), routing_key="message.2"
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.3",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (3)"}), routing_key="message.3"
+            Message.of({"stuff": "Hello world! (3)"}), routing_key="message.3"
         )
 
     def pub_bad():
         medium = Topic(
             exchange="stuff.1",
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
+        medium.broadcast(Message.of({"stuff": "Bad"}), routing_key="bad.stuff.nothing")
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
     pub_proc1.start()
     pub_proc2 = Process(target=pub2)
     pub_proc2.start()
@@ -464,34 +464,34 @@
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (1)"}, routing_key="stuff.something")
+            Message.of({"stuff": "Hello world! (1)"}, routing_key="stuff.something")
         )
 
     def pub2():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
         )
         sleep(0.2)
         medium.broadcast(
-            Message({"stuff": "Hello world! (2)"}, routing_key="stuff.nothing")
+            Message.of({"stuff": "Hello world! (2)"}, routing_key="stuff.nothing")
         )
 
     def pub3():
         medium = Topic(
             exchange="stuff.something",
             config=robotnikmq_config,
         )
         sleep(0.2)
-        medium.broadcast(Message({"stuff": "Bad"}, routing_key="bad.stuff.nothing"))
+        medium.broadcast(Message.of({"stuff": "Bad"}, routing_key="bad.stuff.nothing"))
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc1 = Process(target=pub1)
     pub_proc1.start()
     pub_proc2 = Process(target=pub2)
     pub_proc2.start()
```

### Comparing `robotnikmq-0.7.0/tests/integration/test_rpc.py` & `robotnikmq-0.7.1/tests/integration/test_rpc.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/tests/integration/utils.py` & `robotnikmq-0.7.1/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/tests/unit/test_config.py` & `robotnikmq-0.7.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/tests/unit/test_message.py` & `robotnikmq-0.7.1/tests/unit/test_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 from arrow import get as to_arrow
 from pytest import raises
 
 from robotnikmq.core import Message
 
 
 def test_message_init():
-    msg = Message(contents={'stuff': 'something'})
+    msg = Message.of(contents={'stuff': 'something'})
     assert msg.contents['stuff'] == 'something'
 
 
 def test_message_read_route():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert msg.route == 'test.route'
 
 
 def test_message_getitem():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert msg['stuff'] == 'something'
 
 
 def test_message_contains():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert 'stuff' in msg
 
 
 def test_message_keys():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert set(msg.keys()) == {'stuff'}
 
 
 def test_message_values():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert set(msg.values()) == {'something'}
 
 
 def test_message_iter():
-    msg = Message(contents={'stuff': 'something'}, routing_key='test.route')
+    msg = Message.of(contents={'stuff': 'something'}, routing_key='test.route')
     assert list(i for i in msg) == [('stuff')]
 
 
 def test_message_to_dict():
-    msg = Message(contents={'stuff': 'something'})
+    msg = Message.of(contents={'stuff': 'something'})
     assert msg.to_dict()['timestamp'] == msg.timestamp.int_timestamp
 
 
 def test_message_to_json():
-    msg = Message(contents={'stuff': 'something'})
+    msg = Message.of(contents={'stuff': 'something'})
     print(msg.to_json())
     assert msg.to_json().startswith('{"routing_key": "", "contents": {"stuff": "something"}, "msg_')
 
 
 def test_message_from_json():
-    msg = Message.of('{"routing_key": "", "contents": {"stuff": "something"}, "msg_id": "11bcdb39-'
+    msg = Message.of_json('{"routing_key": "", "contents": {"stuff": "something"}, "msg_id": "11bcdb39-'
                      '56a1-4244-a567-0a5e8eaa125f", "timestamp": 1614471764}')
     assert msg.timestamp == to_arrow(1614471764)
 
 
 def test_not_jsonable():
     with raises(ValueError):
-        Message(contents={'set': {1, 2, 3, 4}})
+        Message.of(contents={'set': {1, 2, 3, 4}})
```

### Comparing `robotnikmq-0.7.0/tests/unit/test_validation.py` & `robotnikmq-0.7.1/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.7.0/PKG-INFO` & `robotnikmq-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotnikmq
-Version: 0.7.0
+Version: 0.7.1
 Summary: Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >3.8.2,<4.0
 Description-Content-Type: text/markdown
 
 # RobotnikMQ
```

