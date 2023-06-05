# Comparing `tmp/reflect-client-1.0.1.tar.gz` & `tmp/reflect-client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflect-client-1.0.1.tar", last modified: Fri Jun  2 10:44:21 2023, max compression
+gzip compressed data, was "reflect-client-1.1.1.tar", last modified: Mon Jun  5 12:22:01 2023, max compression
```

## Comparing `reflect-client-1.0.1.tar` & `reflect-client-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.520117 reflect-client-1.0.1/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-02 10:44:21.519117 reflect-client-1.0.1/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-05-01 16:03:33.000000 reflect-client-1.0.1/README.md
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.517118 reflect-client-1.0.1/reflect_client/
--rw-r--r--   0 victor    (1000) victor    (1000)     3944 2023-05-01 13:15:11.000000 reflect-client-1.0.1/reflect_client/Client.py
--rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-05-01 15:17:35.000000 reflect-client-1.0.1/reflect_client/__init__.py
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.519117 reflect-client-1.0.1/reflect_client.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)      259 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       11 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       15 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-02 10:44:21.520117 reflect-client-1.0.1/setup.cfg
--rw-r--r--   0 victor    (1000) victor    (1000)      517 2023-06-02 10:43:50.000000 reflect-client-1.0.1/setup.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.344523 reflect-client-1.1.1/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-05 12:22:01.343523 reflect-client-1.1.1/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-06-03 12:07:24.000000 reflect-client-1.1.1/README.md
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.328523 reflect-client-1.1.1/reflect_client/
+-rw-r--r--   0 victor    (1000) victor    (1000)     4084 2023-06-05 12:19:31.000000 reflect-client-1.1.1/reflect_client/Client.py
+-rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-06-03 12:07:24.000000 reflect-client-1.1.1/reflect_client/__init__.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.343523 reflect-client-1.1.1/reflect_client.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)      259 2023-06-05 12:22:01.000000 reflect-client-1.1.1/reflect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       20 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       15 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-05 12:22:01.344523 reflect-client-1.1.1/setup.cfg
+-rw-r--r--   0 victor    (1000) victor    (1000)      529 2023-06-05 12:19:58.000000 reflect-client-1.1.1/setup.py
```

### Comparing `reflect-client-1.0.1/README.md` & `reflect-client-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
    ```
    pip3 install reflect-client
    ```
    
 2. **Initialize the module**
 
    ```python
-   from reflect-client import Client 
+   from reflect_client import Client 
    
    client = Client("<API URL or path to UNIX socket>", "<Optional API key>");
    ```
    
 3. **Make API request**
 
    Use the `call()` method to perform a request
```

### Comparing `reflect-client-1.0.1/reflect_client/Client.py` & `reflect-client-1.1.1/reflect_client/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,17 @@
             # Append tailing "/" for HTTP if absent
             self._endpoint = self._endpoint if self._endpoint[-1] == "/" else self._endpoint + "/"
             # Flag which enables or disables SSL peer validation (for self-signed certificates)
             self._https_peer_verify = https_peer_verify
 
     # Close socket connection when class instance removed
     def __del__(self):
-        self._socket.close()
+        # Close socket if connected
+        if (self._con == Connection.AF_UNIX):
+            self._socket.close()
 
     # Resolve connection type from endpoint string.
     # If the string is a valid URL we will treat it as HTTP otherwise we will assume it's a path on disk to a UNIX socket file.
     def resolve_connection(self, endpoint: str) -> Connection:
         return Connection.HTTP if validators.url(endpoint) else Connection.AF_UNIX
 
     # Check if provided "method" is an instance of the Method enum. Else return default
@@ -71,17 +73,17 @@
         return headers
 
     # Make request and return response over HTTP
     def http_call(self, endpoint: str, method: Method, payload: list = None) -> tuple:
         # Remove leading "/" if present, as it's already present in self._endpoint
         endpoint = endpoint if endpoint[-1] != "/" else endpoint[:-1]
         
-        resp = requests.request(method.name, self._endpoint + endpoint, headers=self.http_headers(), data=json.dumps(payload))
-        # Return response as tuple of response code and response body as plain text
-        return (resp.status_code, resp.text)
+        resp = requests.request(method.name, self._endpoint + endpoint, verify=self._https_peer_verify, headers=self.http_headers(), data=json.dumps(payload))
+        # Return response as tuple of response code and response body as decoded JSON (mixed)
+        return (resp.status_code, json.loads(resp.text))
 
     def socket_txn(self, endpoint: str, method: Union[Method, str] = None, payload: list = None) -> tuple:
         data = f'["{endpoint}","{method.name}","{json.dumps(payload)}"]'
         tx = self._socket.sendall(b'["order","GET",""]')
         rx = self._socket.recv(__class__.SOCKET_READ_BYTES)
 
         return tuple(json.loads(rx))
```

