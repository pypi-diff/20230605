# Comparing `tmp/helyos_agent_sdk-0.4.0.tar.gz` & `tmp/helyos_agent_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helyos_agent_sdk-0.4.0.tar", max compression
+gzip compressed data, was "helyos_agent_sdk-0.5.0.tar", max compression
```

## Comparing `helyos_agent_sdk-0.4.0.tar` & `helyos_agent_sdk-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       88 2023-01-26 14:16:59.066461 helyos_agent_sdk-0.4.0/helyos_agent_sdk/__init__.py
--rw-r--r--   0        0        0    14824 2023-04-20 14:39:37.636614 helyos_agent_sdk-0.4.0/helyos_agent_sdk/client.py
--rw-r--r--   0        0        0    14965 2023-01-26 14:16:49.073494 helyos_agent_sdk-0.4.0/helyos_agent_sdk/connector.py
--rw-r--r--   0        0        0      463 2023-04-10 14:06:03.061672 helyos_agent_sdk-0.4.0/helyos_agent_sdk/exceptions.py
--rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.4.0/helyos_agent_sdk/models.py
--rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.4.0/LICENSE
--rw-r--r--   0        0        0     1107 2023-04-20 13:23:00.871923 helyos_agent_sdk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.4.0/README.md
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.4.0/setup.py
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-06-05 09:45:43.988640 helyos_agent_sdk-0.5.0/helyos_agent_sdk/__init__.py
+-rw-r--r--   0        0        0    15199 2023-06-04 15:09:10.821100 helyos_agent_sdk-0.5.0/helyos_agent_sdk/client.py
+-rw-r--r--   0        0        0    16156 2023-06-04 14:32:41.591598 helyos_agent_sdk-0.5.0/helyos_agent_sdk/connector.py
+-rw-r--r--   0        0        0      463 2023-04-10 14:06:03.061672 helyos_agent_sdk-0.5.0/helyos_agent_sdk/exceptions.py
+-rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.5.0/helyos_agent_sdk/models.py
+-rw-r--r--   0        0        0    13711 2023-06-04 15:06:26.315652 helyos_agent_sdk-0.5.0/helyos_agent_sdk/mqtt_client.py
+-rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1129 2023-06-05 12:55:41.365651 helyos_agent_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.5.0/README.md
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.5.0/setup.py
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.5.0/PKG-INFO
```

### Comparing `helyos_agent_sdk-0.4.0/helyos_agent_sdk/client.py` & `helyos_agent_sdk-0.5.0/helyos_agent_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
             context.check_hostname = False
             context.verify_mode =  ssl.CERT_NONE
 
         ssl_options = pika.SSLOptions(context, rabbitmq_host)
     else:
         ssl_options = None
 
-
-
     if temporary:
         params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=60, blocked_connection_timeout=60,
                                             ssl_options=ssl_options)
     else:
         params = pika.ConnectionParameters(rabbitmq_host,  rabbitmq_port, '/', credentials,heartbeat=3600,blocked_connection_timeout=300,
                                             ssl_options=ssl_options )
     _connection = pika.BlockingConnection(params)
@@ -76,14 +74,16 @@
         self.ca_certificate = ca_certificate
         self.uuid = uuid
         self.enable_ssl = enable_ssl
 
         self.connection = None
         self.channel = None
         self.checkin_data = None
+        self._protocol = 'AMQP'
+
         self.tries = 0
         self.rbmq_username = None
         self.rbmq_password = None
         
         if pubkey is None:
             self.private_key, self.public_key = generate_private_public_keys()
         else:
@@ -166,27 +166,30 @@
             raise HelyOSAnonymousConnectionError(
                     "Not able to connect as anonymous to rabbitMQ to perform check in.")
     
         
         # step 2 - creates a temporary queue to receive checkin response
         temp_queue = self.guest_channel.queue_declare(queue='', exclusive=True)            
         self.checkin_response_queue = temp_queue.method.queue 
-        self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback)
+        self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback_wrapper)
 
 
     def __prepare_checkin_for_already_connected(self):
          # step 1 - use existent connection
         self.guest_channel = self.channel
         # step 2 - creates a temporary queue to receive checkin response
         temp_queue = self.guest_channel.queue_declare(queue='', exclusive=True)            
         self.checkin_response_queue = temp_queue.method.queue 
-        self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback)
+        self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback_wrapper)
 
 
     def connect_rabbitmq(self, username, password):
+        return self.connect(username, password)
+
+    def connect(self, username, password):
         """
         Creates the connection between agent and the RabbitMQ server.
         
         .. code-block:: python
 
             helyos_client = HelyOSClient(host='myrabbitmq.com', port=5672, uuid='3452345-52453-43525')
             helyos_client.connect_rabbitmq('my_username', 'secret_password') #  <===
@@ -253,15 +256,27 @@
 
         self.guest_channel.basic_publish(exchange = AGENT_ANONYMOUS_EXCHANGE,
                                   routing_key =  self.checking_routing_key,
                                   properties=pika.BasicProperties(reply_to = self.checkin_response_queue, user_id = username),
                                   body=json.dumps(checkin_msg))
         
 
-    def __checkin_callback(self, ch, method, properties, received_str):
+    def __checkin_callback_wrapper(self, channel, method, properties, received_str):
+        try:
+            self.__checkin_callback(received_str)
+            channel.stop_consuming()
+        except  Exception as inst: 
+            self.tries += 1
+            print(f"try {self.tries}")
+            if self.tries > 3:
+                channel.stop_consuming()
+
+        
+
+    def __checkin_callback(self, received_str):
         received_message_str = json.loads(received_str)['message']    
         received_message = json.loads(received_message_str)
         
         msg_type = received_message['type']
         if msg_type != 'checkin':
             print("waiting response...")
             return
@@ -272,35 +287,28 @@
             print(body)
             message  = body.get('message', "Check in refused")
             raise HelyOSCheckinError(f"{message}: code {response_code}")
             
         password = body.pop('rbmq_password', None)
         self.ca_certificate =  body.get('ca_certificate', self.ca_certificate)
         
-        try:
-            if password:
-                self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password, self.enable_ssl, self.ca_certificate)
-                self.channel = self.connection.channel()
-                self.rbmq_username = body['rbmq_username']
-                self.rbmq_password = password
-
-                print('uuid', self.uuid)
-                print('username', body['rbmq_username'])
-                print('password', len(password)*'*')
-
-            self.uuid = received_message['uuid']
-            self.checkin_data = body
-            ch.stop_consuming()
+        if password:
+            self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password, self.enable_ssl, self.ca_certificate)
+            self.channel = self.connection.channel()
+            self.rbmq_username = body['rbmq_username']
+            self.rbmq_password = password
+
+            print('uuid', self.uuid)
+            print('username', body['rbmq_username'])
+            print('password', len(password)*'*')
+
+        self.uuid = received_message['uuid']
+        self.checkin_data = body
             
 
-        except  Exception as inst: 
-            self.tries += 1
-            print(f"try {self.tries}")
-            if self.tries > 3:
-                ch.stop_consuming()
 
 
     @auth_required            
     def publish(self, routing_key, message, encrypted=False, exchange=AGENTS_UL_EXCHANGE):
         """ Publish message in RabbitMQ
 
             :param routing_key: RabbitMQ routing_key 
@@ -348,7 +356,14 @@
 
         """
         
         self.set_instant_actions_queue()
         self.channel.basic_consume(queue=self.instant_actions_queue.method.queue, auto_ack=True,
                                    on_message_callback=instant_actions_callback)
 
+
+    def start_listening(self):
+        self.channel.start_consuming()
+
+    def stop_listening(self):
+        self.channel.stop_consuming()
+
```

### Comparing `helyos_agent_sdk-0.4.0/helyos_agent_sdk/connector.py` & `helyos_agent_sdk-0.5.0/helyos_agent_sdk/connector.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,66 +4,75 @@
 from .client import HelyOSClient
 from .models import (ASSIGNMENT_STATUS, AGENT_STATE, Pose, ASSIGNMENT_MESSAGE_TYPE, INSTANT_ACTIONS_TYPE, WorkProcessResourcesRequest,
                     AssignmentCommandMessage, AssignmentMetadata, AssignmentCancelMessage, AgentCurrentResources, AgentStateBody, 
                     AgentStateMessage, AssignmentCurrentStatus)
 
             
 
-def parse_assignment_message(self, ch, method, properties, received_str):    
+def parse_assignment_message(self, ch, properties, received_str):    
     received_message_str = json.loads(received_str)['message']    
     received_message = json.loads(received_message_str)
     action_type = received_message.get('type', None)
+    sender = None
+    if hasattr(properties, 'user_id'):
+        sender =  properties.user_id
+
     
     if action_type == ASSIGNMENT_MESSAGE_TYPE.EXECUTION:
         command_message = { 'type' : received_message['type'],
                             'work_process_id': received_message['work_process_id'],
                             'assignment_metadata': AssignmentMetadata(**received_message['assignment_metadata']),
                             'body': received_message['body'],
                             '_version': received_message['_version'] }
                                                                           
         inst_assignm_exec = AssignmentCommandMessage(**command_message)
-        return self.assignment_callback(ch, method, properties, inst_assignm_exec)
+        return self.assignment_callback(ch, sender, inst_assignm_exec)
         
-    return self.other_assignment_callback(ch, method, properties, received_str)
+    return self.other_assignment_callback(ch,  sender, received_str)
     
+
+
     
-def parse_instant_actions(self, ch, method, properties, received_str):
+def parse_instant_actions(self, ch, properties, received_str):
     received_message_str = json.loads(received_str)['message']    
     received_message = json.loads(received_message_str)
     action_type = received_message.get('type', None)
+    sender = None
+    if hasattr(properties, 'user_id'):
+        sender =  properties.user_id
 
     if action_type == INSTANT_ACTIONS_TYPE.CANCEL:
         command_message = { 'type' : received_message['type'],
                             'work_process_id': received_message['work_process_id'],
                             'assignment_metadata': AssignmentMetadata(**received_message['assignment_metadata']),
                             'body': received_message['body'],
                             '_version': received_message['_version'] }
         inst_assignm_cancel = AssignmentCancelMessage(**command_message)      
         print("call cancel callback")
-        return self.cancel_callback(ch, method, properties, inst_assignm_cancel)
+        return self.cancel_callback(ch, sender, inst_assignm_cancel)
 
     if action_type == INSTANT_ACTIONS_TYPE.RESERVE:
         inst_wp_clearance = WorkProcessResourcesRequest(**received_message['body'])
-        return self.reserve_callback(ch, method, properties, inst_wp_clearance)
+        return self.reserve_callback(ch, sender, inst_wp_clearance)
 
     if action_type == INSTANT_ACTIONS_TYPE.RELEASE:
         inst_wp_clearance = WorkProcessResourcesRequest(**received_message['body'])
-        return self.release_callback(ch, method, properties, inst_wp_clearance)   
+        return self.release_callback(ch, sender, inst_wp_clearance)   
         
     if action_type == INSTANT_ACTIONS_TYPE.WPCLEREANCE:  # Backward compatibility
         work_process_id = received_message['body']['wp_id']        
         operation_types_required = received_message['body']['operation_types_required']
         reserved = received_message['body']['reserved']
         inst_wp_clearance = WorkProcessResourcesRequest(work_process_id, operation_types_required, reserved)
         if reserved:
-            return self.reserve_callback(ch, method, properties, inst_wp_clearance)
+            return self.reserve_callback(ch, sender, inst_wp_clearance)
         else:
-            return self.release_callback(ch, method, properties, inst_wp_clearance)
+            return self.release_callback(ch, sender, inst_wp_clearance)
 
-    return self.other_instant_actions_callback(ch, method, properties, received_str)
+    return self.other_instant_actions_callback(ch, sender, received_str)
     
 
 
 class AgentConnector():
     agent_status = AGENT_STATE.FREE
     agent_pose: Pose = Pose(x=0, y=0, z=0, orientations=[0])
     agent_resources = None
@@ -102,42 +111,54 @@
         self.encrypted = encrypted
         if pose:
             self.agent_pose = pose
 
 
     __instant_actions_callback = parse_instant_actions
     __assignment_callback = parse_assignment_message
-    assignment_callback = lambda  self, ch, method, properties, received_msg : print("assignment", received_msg)
-    cancel_callback = lambda self, ch, method, properties, received_msg : print("cancel callback", received_msg)
-    reserve_callback = lambda self, ch, method, properties, received_msg : print("reserve callback", received_msg)
-    release_callback = lambda self, ch, method, properties, received_msg : print("release callback", received_msg)
-    other_instant_actions_callback = lambda self, ch, method, properties, received_msg : print("instant_action_callback", received_msg)
-    other_assignment_callback = lambda self, ch, method, properties, received_msg : print("other_assignment_callback", received_msg)
+    assignment_callback = lambda  self, ch, sender, received_msg : print("assignment", sender, received_msg)
+    cancel_callback = lambda self, ch, sender, received_msg : print("cancel callback", sender, received_msg)
+    reserve_callback = lambda self, ch, sender, received_msg : print("reserve callback", sender, received_msg)
+    release_callback = lambda self, ch, sender, received_msg : print("release callback", sender, received_msg)
+    other_instant_actions_callback = lambda self, ch, sender, received_msg : print("instant_action_callback", sender, received_msg)
+    other_assignment_callback = lambda self, ch, sender, received_msg : print("other_assignment_callback", sender,  received_msg)
         
 
     def consume_instant_action_messages(self, reserve_callback=None, release_callback=None, cancel_callback=None,  other_callback=None):
         """Register the callback functions for instant actions
         
-            :param reserve_callback: reserve_callback(ch, method, properties, received_str) 
+            :param reserve_callback: reserve_callback(ch:Channel , sender: string, message: WorkProcessResourcesRequest) 
             :type reserve_callback: func
-            :param release_callback: release_callback(ch, method, properties, received_str) 
+            :param release_callback: release_callback(ch, sender, message: WorkProcessResourcesRequest) 
             :type release_callback: func 
             :param cancel_callback: cancel_callback 
-            :type cancel_callback: func(ch, method, properties, received_str)
+            :type cancel_callback: func(ch, sender, message: AssignmentCancelMessage)
             :param other_callback: Non-helyOS related instant action
-            :type other_callback: func(ch, method, properties, received_str) 
+            :type other_callback: func(ch: Channel, sender:string, message: string) 
 
         """
 
 
         if cancel_callback is not None: self.cancel_callback = cancel_callback
         if reserve_callback is not None: self.reserve_callback = reserve_callback
         if release_callback is not None: self.release_callback = release_callback
         if other_callback is not None: self.other_instant_actions_callback = other_callback
 
+        def amqp_callback(ch, method, properties, message): 
+            return parse_instant_actions(self, ch, properties, received_str=message)
+        
+        def mqtt_callback(ch, userdata, message): 
+            return parse_instant_actions(self, ch, {'user_id': None}, received_str= message.payload.decode())
+        
+        if self.helyos_client._protocol == 'AMQP':
+            self.__instant_actions_callback = amqp_callback
+
+        if self.helyos_client._protocol == 'MQTT':
+            self.__instant_actions_callback = mqtt_callback
+
         self.helyos_client.consume_instant_actions_messages(self.__instant_actions_callback)
         
 
     def consume_assignment_messages(self, assignment_callback=None, other_callback=None):
         """Register the callback functions for assignments or order (VDA5050)
         
             :param reserve_callback: assignment_callback(ch, method, properties, received_str) 
@@ -145,22 +166,34 @@
             :param other_callback: Non-helyOS related instant action
             :type other_callback: func(ch, method, properties, received_str) 
         """
         
         if assignment_callback is not None: self.assignment_callback = assignment_callback 
         if other_callback is not None: self.other_assignment_callback = other_callback
 
+        def amqp_callback(ch, method, properties, message): 
+            return parse_assignment_message(self, ch, properties, received_str=message)
+        
+        def mqtt_callback(ch, userdata, message): 
+            return parse_assignment_message(self, ch, {'user_id': None}, received_str= message.payload.decode())
+        
+        if self.helyos_client._protocol == 'AMQP':
+            self.__assignment_callback = amqp_callback
+
+        if self.helyos_client._protocol == 'MQTT':
+            self.__assignment_callback = mqtt_callback
+
         self.helyos_client.consume_assignment_messages(self.__assignment_callback)
 
-    def start_consuming(self):
-        self.helyos_client.channel.start_consuming()
+    def start_listening(self):
+        self.helyos_client.start_listening()
         
         
-    def stop_consuming(self):
-        self.helyos_client.channel.stop_consuming()
+    def stop_listening(self):
+        self.helyos_client.stop_listening()
 
 
     def publish_general_updates(self, body={}):
         """ 
             Updates agent properties of agent: name, code, factsheet, etc.
             This is published in a low-priority queue to helyOS; in very high load conditions, some messages
             may be expired before helyOS consumption.
```

### Comparing `helyos_agent_sdk-0.4.0/helyos_agent_sdk/models.py` & `helyos_agent_sdk-0.5.0/helyos_agent_sdk/models.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.4.0/LICENSE` & `helyos_agent_sdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.4.0/pyproject.toml` & `helyos_agent_sdk-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helyos_agent_sdk"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Carlos Viol Barbosa <you@example.com>"]
 readme = "README.md"
 packages = [{include = "helyos_agent_sdk"}]
 keywords = ["autonomous driving", "helyos", "sdk"]
 
 homepage = "https://helyos.ivi.fraunhofer.de"
@@ -20,14 +20,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pika = "^1.3.1"
 pycryptodome = "^3.15.0"
 dataclasses-json = "^0.5.7"
+paho-mqtt = "^1.6.1"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^19.10b0"
 pre-commit = {version = "^2.4.0", python = "^3.6.1"}
 pylint = "^2.5.0"
```

### Comparing `helyos_agent_sdk-0.4.0/README.md` & `helyos_agent_sdk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.4.0/setup.py` & `helyos_agent_sdk-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 ['helyos_agent_sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['dataclasses-json>=0.5.7,<0.6.0',
+ 'paho-mqtt>=1.6.1,<2.0.0',
  'pika>=1.3.1,<2.0.0',
  'pycryptodome>=3.15.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'helyos-agent-sdk',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
     'long_description': '<div id="top"></div>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/">\n    <img src="helyos_logo.png" alt="Logo"  height="80">\n    <img src="truck.png" alt="Logo"  height="80">\n  </a>\n\n  <h3 align="center">helyOS Agent SDK</h3>\n\n  <p align="center">\n    Methods and data strrctures to connect autonomous vehicles to helyOS.\n    <br />\n    <a href="https://fraunhoferivi.github.io/helyOS-agent-sdk/"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/">View Demo</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Request Feature</a>\n  </p>\n</div>\n\n## About The Project\n\nThe helyos-agent-sdk python package encloses methods and data structures definitions that facilitate the connection to helyOS core through rabbitMQ.\n\n### List of features\n\n*   RabbitMQ client to communicate with helyOS. \n*   Check-in method.\n*   Agent and assignment status definitions. \n*   Easy access to helyOS assignments via callbacks. \n*   Application-level encryption.\n\n### Install\n\n```\npip install helyos_agent_sdk\n\n```\n### Usage\n\n```python\nos.environ[\'AGENTS_UL_EXCHANGE\'] = "xchange_helyos.agents.ul"\nos.environ[\'AGENTS_DL_EXCHANGE\'] = "xchange_helyos.agents.dl"\nos.environ[\'AGENT_ANONYMOUS_EXCHANGE\'] = "xchange_helyos.agents.anonymous"\nfrom helyos_agent_sdk import HelyOSClient, AgentConnector\n\n# Check in\ninitial_agent_data = {\'name\': "vehicle name", \'pose\': {\'x\':-30167, \'y\':-5415, \'orientations\':[0, 0]}, \'geometry\':{"my_custom_format": {}}}\nhelyOS_client = HelyOSClient(rabbitmq_host, rabbitmq_port, uuid=AGENT_UID)\nhelyOS_client.perform_checkin(yard_uid=\'1\', agent_data=initial_agent_data, status="free")\nhelyOS_client.get_checkin_result()\n\n\n# Communication\nagent_connector = AgentConnector(helyOS_client)\nagent_connector.publish_sensors(x=-30167, y=3000, z=0, orientations=[1500, 0], sensor= {"my_custom_format": {}})\n\n# ... #\n\nagentConnector.publish_state(status, resources, assignment_status)\n\n# ... #\n\nagentConnector.consume_instant_action_messages(my_reserve_callback, my_release_callback, my_cancel_assignm_callback, any_other_callback)\nagentConnector.consume_assignment_messages(my_assignment_callback)\nagentConnector.start_consuming()\n\n\n```\n\n\n### Contributing\n\nKeep it simple. Keep it minimal.\n\n### Authors \n\n*   Carlos E. Viol Barbosa\n*   ...\n\n### License\n\nThis project is licensed under the MIT License',
     'author': 'Carlos Viol Barbosa',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://helyos.ivi.fraunhofer.de',
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['helyos_agent_sdk'] package_data = \ {'': ['*']} install_requires = \
-['dataclasses-json>=0.5.7,<0.6.0', 'pika>=1.3.1,<2.0.0',
-'pycryptodome>=3.15.0,<4.0.0'] setup_kwargs = { 'name': 'helyos-agent-sdk',
-'version': '0.4.0', 'description': '', 'long_description': '
+['dataclasses-json>=0.5.7,<0.6.0', 'paho-mqtt>=1.6.1,<2.0.0',
+'pika>=1.3.1,<2.0.0', 'pycryptodome>=3.15.0,<4.0.0'] setup_kwargs = { 'name':
+'helyos-agent-sdk', 'version': '0.5.0', 'description': '', 'long_description':
+'
 \n\n\n
 \n
                           \n \n_[Logo]\n_[Logo]\n\n\n
                           **** helyOS Agent SDK ****
                                      \n\n
   \n Methods and data strrctures to connect autonomous vehicles to helyOS.\n
                            \n Explore_the_docs_Â»\n
```

### Comparing `helyos_agent_sdk-0.4.0/PKG-INFO` & `helyos_agent_sdk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helyos-agent-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://helyos.ivi.fraunhofer.de
 Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
+Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Project-URL: Documentation, https://fraunhoferivi.github.io/helyOS-agent-sdk/
 Project-URL: Repository, https://github.com/FraunhoferIVI/helyOS-agent-sdk
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.4.0 Summary: Home-page:
+Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.5.0 Summary: Home-page:
 https://helyos.ivi.fraunhofer.de Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa Author-email: you@example.com Requires-Python:
 >=3.7,<4.0 Classifier: Environment :: Console Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0) Requires-Dist: pika
-(>=1.3.1,<2.0.0) Requires-Dist: pycryptodome (>=3.15.0,<4.0.0) Project-URL:
-Documentation, https://fraunhoferivi.github.io/helyOS-agent-sdk/ Project-URL:
-Repository, https://github.com/FraunhoferIVI/helyOS-agent-sdk Description-
-Content-Type: text/markdown
+Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0) Requires-Dist: paho-mqtt
+(>=1.6.1,<2.0.0) Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-Dist:
+pycryptodome (>=3.15.0,<4.0.0) Project-URL: Documentation, https://
+fraunhoferivi.github.io/helyOS-agent-sdk/ Project-URL: Repository, https://
+github.com/FraunhoferIVI/helyOS-agent-sdk Description-Content-Type: text/
+markdown
 
                                  [Logo]_[Logo]
                           **** helyOS Agent SDK ****
     Methods and data strrctures to connect autonomous vehicles to helyOS.
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
```

