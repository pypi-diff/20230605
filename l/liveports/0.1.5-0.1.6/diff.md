# Comparing `tmp/liveports-0.1.5.tar.gz` & `tmp/liveports-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.5.tar", last modified: Sun Jun  4 23:35:49 2023, max compression
+gzip compressed data, was "liveports-0.1.6.tar", last modified: Mon Jun  5 10:44:42 2023, max compression
```

## Comparing `liveports-0.1.5.tar` & `liveports-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-04 23:35:49.188103 liveports-0.1.5/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-04 23:35:49.188103 liveports-0.1.5/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.5/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-04 23:35:49.188103 liveports-0.1.5/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.5/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-03 11:03:34.000000 liveports-0.1.5/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    11638 2023-06-04 23:31:30.000000 liveports-0.1.5/liveports/client.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-04 23:35:49.188103 liveports-0.1.5/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      287 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-04 23:35:49.000000 liveports-0.1.5/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-04 23:35:49.188103 liveports-0.1.5/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      602 2023-06-04 16:39:35.000000 liveports-0.1.5/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 10:44:42.240049 liveports-0.1.6/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.6/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 10:44:42.240049 liveports-0.1.6/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.6/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 10:44:42.240049 liveports-0.1.6/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.6/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-03 11:03:34.000000 liveports-0.1.6/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12094 2023-06-05 10:44:34.000000 liveports-0.1.6/liveports/client.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.6/liveports/logviewer.html
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-05 10:44:42.240049 liveports-0.1.6/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-05 10:44:42.000000 liveports-0.1.6/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-05 10:44:42.240049 liveports-0.1.6/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-05 08:39:59.000000 liveports-0.1.6/setup.py
```

### Comparing `liveports-0.1.5/liveports/blaster_utils.py` & `liveports-0.1.6/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1.5/liveports/client.py` & `liveports-0.1.6/liveports/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,36 +25,44 @@
 ssl_context = ssl.create_default_context()
 ssl_context.check_hostname = False
 ssl_context.verify_mode = ssl.CERT_NONE
 
 socketserver.TCPServer.allow_reuse_address = True
 
 # Process command line arguments
+try:
+	SOURCE = CommandLineArgs.get("source", "")  # given domain
 
-SOURCE = CommandLineArgs.get("source", "")  # given domain
-
-# If request logging enabled, we will use a proxy server to log request/response
-LOCAL_PROXY_PORT = int(CommandLineArgs.get("proxyPort", 4060))
-LOG_VIEWER_PORT = int(CommandLineArgs.get("logViewerPort") or (LOCAL_PROXY_PORT + 1))
-DEBUG_LOG_LEVEL = int(CommandLineArgs.get("logLevel", 0))
-# target
-TARGET_HOST = "localhost"
-if(target_host := CommandLineArgs.get("target")):
-	TARGET_PROTOCOL = urlparse(target_host).scheme or "http"
-	TARGET_PORT = urlparse(target_host).port or (80 if TARGET_PROTOCOL == "http" else 443)
-	TARGET_HOST = urlparse(target_host).hostname or "localhost"
-else:
-	TARGET_PORT = int(CommandLineArgs.get("targetPort") or CommandLineArgs["args"][-1])
-	TARGET_PROTOCOL = (
-		CommandLineArgs.get("targetProtocol")
-		or (CommandLineArgs["args"][1] if len(CommandLineArgs["args"]) > 1 else "http")
-	).lower()
-
-NO_PROXY = bool(CommandLineArgs.get("noproxy", False)) and TARGET_HOST == "localhost"  # only when target host is localhost
-
+	# If request logging enabled, we will use a proxy server to log request/response
+	LOCAL_PROXY_PORT = int(CommandLineArgs.get("proxyPort", 4060))
+	LOG_VIEWER_PORT = int(CommandLineArgs.get("logViewerPort") or (LOCAL_PROXY_PORT + 1))
+	DEBUG_LOG_LEVEL = int(CommandLineArgs.get("logLevel") or 0)
+	# target
+	TARGET_HOST = "localhost"
+	if(target_host := CommandLineArgs.get("target")):
+		TARGET_PROTOCOL = urlparse(target_host).scheme or "http"
+		TARGET_PORT = urlparse(target_host).port or (80 if TARGET_PROTOCOL == "http" else 443)
+		TARGET_HOST = urlparse(target_host).hostname or "localhost"
+	else:
+		TARGET_PORT = int(CommandLineArgs.get("targetPort") or CommandLineArgs["args"][-1])
+		TARGET_PROTOCOL = (
+			CommandLineArgs.get("targetProtocol")
+			or (CommandLineArgs["args"][1] if len(CommandLineArgs["args"]) > 1 else "http")
+		).lower()
+
+	NO_PROXY = bool(CommandLineArgs.get("noproxy", False)) and TARGET_HOST == "localhost"  # only when target host is localhost
+except Exception:
+	print('''
+Invalid Arguments. Usage Examples:
+liveports http 3000
+liveports https 3000
+liveports https 3000 --source="https://yourdomain.com" 
+liveports https 3000 --source="https://yourdomain.com" --noproxy # for no mediating logging
+''')
+	sys.exit(1)
 
 if(TARGET_PROTOCOL not in ["http", "https"]):
 	print("Invalid protocol: must be one of http/https", TARGET_PROTOCOL)
 	sys.exit(1)
 
 
 class Client:
@@ -264,31 +272,32 @@
 				data = source.recv(4096)
 				if not data:
 					self.is_running = False
 					break
 				buf.extend(data)
 				target.sendall(data)
 			target.shutdown(socket.SHUT_RDWR)
-		except Exception:
+		except Exception as ex:
+			DEBUG_LOG_LEVEL > 2 and print("error proxessing connection forwarding: ", str(ex))
 			pass
 
 
 SERVER_CACHED_RESP_FILE = os.path.join(os.path.dirname(__file__), "liveports.json")
 LOCK_FILE = os.path.join(tempfile.gettempdir(), f"liveports_{SOURCE}.lock")
 
 
 def get_config():
 	if(
 		os.path.isfile(SERVER_CACHED_RESP_FILE)
 		and (contents := open(SERVER_CACHED_RESP_FILE).read().strip())
 	):
 		try:
 			return json.loads(contents)
-		except Exception:
-			pass
+		except Exception as ex:
+			DEBUG_LOG_LEVEL > 2 and print("could not load config file", str(ex))
 	return {}
 
 
 def save_config(config):
 	cache = get_config()
 	prev_source_config = cache.get(SOURCE) or {}
 	prev_source_config.update(config)
```

