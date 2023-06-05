# Comparing `tmp/liveports-0.1.7.tar.gz` & `tmp/liveports-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.7.tar", last modified: Mon Jun  5 14:24:27 2023, max compression
+gzip compressed data, was "liveports-0.1.8.tar", last modified: Mon Jun  5 16:51:45 2023, max compression
```

## Comparing `liveports-0.1.7.tar` & `liveports-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 14:24:27.450228 liveports-0.1.7/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.7/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 14:24:27.450228 liveports-0.1.7/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.7/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 14:24:27.450228 liveports-0.1.7/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.7/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-03 11:03:34.000000 liveports-0.1.7/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12660 2023-06-05 14:24:02.000000 liveports-0.1.7/liveports/client.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.7/liveports/logviewer.html
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 14:24:27.450228 liveports-0.1.7/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-05 14:24:27.000000 liveports-0.1.7/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-05 14:24:27.450228 liveports-0.1.7/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-05 14:21:49.000000 liveports-0.1.7/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.8/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 16:51:45.272141 liveports-0.1.8/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.8/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.8/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-03 11:03:34.000000 liveports-0.1.8/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12765 2023-06-05 16:03:38.000000 liveports-0.1.8/liveports/client.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.8/liveports/logviewer.html
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 16:51:45.272141 liveports-0.1.8/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-05 16:51:45.000000 liveports-0.1.8/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-05 16:51:45.272141 liveports-0.1.8/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-05 16:04:20.000000 liveports-0.1.8/setup.py
```

### Comparing `liveports-0.1.7/liveports/blaster_utils.py` & `liveports-0.1.8/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1.7/liveports/client.py` & `liveports-0.1.8/liveports/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,24 +255,27 @@
 
 # PROXY SERVER
 class ProxyHandler(socketserver.BaseRequestHandler):
 	is_running = True
 
 	def handle(self):
 		# Connect to the destination server
+		self.request.settimeout(5)
 		req_data = bytearray()
 		resp_data = bytearray()
 		target_sock = None
 		try:
 			target_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 			# Wrap the destination socket with SSL
 			if(TARGET_PROTOCOL == "https"):
 				target_sock = ssl_context.wrap_socket(target_sock)
 
+			target_sock.settimeout(5)
 			target_sock.connect((TARGET_HOST, TARGET_PORT))
+
 			thread = threading.Thread(target=self.forward_data, args=(self.request, target_sock, req_data))
 			thread.start()
 
 			self.forward_data(target_sock, self.request, resp_data)
 			# Wait for the threads to complete
 			thread.join()
 		except Exception as ex:
@@ -282,15 +285,18 @@
 			self.request.close()
 			target_sock and target_sock.close()
 
 		LogViewer.process_wire_log(req_data, resp_data)
 
 	def forward_data(self, source, target, buf):
 		while self.is_running and Client.is_running:
-			data = source.recv(4096)
+			try:
+				data = source.recv(4096)
+			except TimeoutError:
+				continue
 			if not data:
 				self.is_running = False
 				break
 			buf.extend(data)
 			target.sendall(data)
 		target.shutdown(socket.SHUT_WR)
```

### Comparing `liveports-0.1.7/liveports/logviewer.html` & `liveports-0.1.8/liveports/logviewer.html`

 * *Files identical despite different names*

### Comparing `liveports-0.1.7/setup.py` & `liveports-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='liveports',
-    version='0.1.7',
+    version='0.1.8',
     description='Give address to your localmachine',
     author='Abhinav',
     author_email='abhinavabcd@gmail.com',
     packages=['liveports'],
     include_package_data=True,
     install_requires=[
         "requests>=2.23.0",
```

