# Comparing `tmp/silicron-0.0.3.tar.gz` & `tmp/silicron-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicron-0.0.3.tar", last modified: Mon Jun  5 04:14:12 2023, max compression
+gzip compressed data, was "silicron-0.0.4.tar", last modified: Mon Jun  5 05:15:06 2023, max compression
```

## Comparing `silicron-0.0.3.tar` & `silicron-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.350742 silicron-0.0.3/
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 04:14:12.350581 silicron-0.0.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2094 2023-06-05 03:52:57.000000 silicron-0.0.3/README.md
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-05 04:14:12.350804 silicron-0.0.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      530 2023-06-05 04:13:48.000000 silicron-0.0.3/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.349271 silicron-0.0.3/silicron/
--rw-r--r--   0 michael    (501) staff       (20)       26 2023-05-26 09:29:50.000000 silicron-0.0.3/silicron/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     7029 2023-06-05 04:11:37.000000 silicron-0.0.3/silicron/api.py
--rw-r--r--   0 michael    (501) staff       (20)      362 2023-06-05 03:45:00.000000 silicron-0.0.3/silicron/models.py
--rw-r--r--   0 michael    (501) staff       (20)      837 2023-06-05 03:45:00.000000 silicron-0.0.3/silicron/utils.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 04:14:12.350241 silicron-0.0.3/silicron.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 04:14:11.000000 silicron-0.0.3/silicron.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      220 2023-06-05 04:14:12.000000 silicron-0.0.3/silicron.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-05 04:14:11.000000 silicron-0.0.3/silicron.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-05 04:14:12.000000 silicron-0.0.3/silicron.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 05:15:06.628249 silicron-0.0.4/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 05:15:06.628103 silicron-0.0.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2094 2023-06-05 03:52:57.000000 silicron-0.0.4/README.md
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-05 05:15:06.628300 silicron-0.0.4/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      679 2023-06-05 05:15:03.000000 silicron-0.0.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 05:15:06.627200 silicron-0.0.4/silicron/
+-rw-r--r--   0 michael    (501) staff       (20)       26 2023-05-26 09:29:50.000000 silicron-0.0.4/silicron/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     6606 2023-06-05 05:14:34.000000 silicron-0.0.4/silicron/api.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-05 05:15:06.627896 silicron-0.0.4/silicron.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-05 05:15:06.000000 silicron-0.0.4/silicron.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      214 2023-06-05 05:15:06.000000 silicron-0.0.4/silicron.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-05 05:15:06.000000 silicron-0.0.4/silicron.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       26 2023-06-05 05:15:06.000000 silicron-0.0.4/silicron.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-05 05:15:06.000000 silicron-0.0.4/silicron.egg-info/top_level.txt
```

### Comparing `silicron-0.0.3/README.md` & `silicron-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `silicron-0.0.3/silicron/api.py` & `silicron-0.0.4/silicron/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,108 +3,114 @@
 import logging
 import os
 
 # Third party imports
 import requests
 import tqdm
 
-# Our imports
-import silicron.utils as utils
-import silicron.models as models
-
 # Constants
 STAGING_API_ENDPOINT = "https://wsesuzvgd0.execute-api.us-east-1.amazonaws.com/staging"
 
-# TODO this can be made way neater by putting configs in the init function.
 
 class Silicron:
-    def __init__(self, api_key: str = ""):
+    """Silicron Class
+
+    Attributes:
+        api_key (str): The API key to use for authentication.
+        chatbot (str): The chatbot to use for chat.
+        database (str): The database to use for chat.
+        api_endpoint (str): The API endpoint to use for requests.
+        fn_endpoints (Dict[str, str]): A dictionary containing the API endpoints
+            for each function.
+        session (requests.Session): A requests session object to use for requests.
+    """
+
+    def __init__(
+        self, api_key: str = "", chatbot: str = "chatgpt3.5-turbo", database: str = ""
+    ):
         """Initialize the Silicron class.
 
         Args:
             api_key (str): The API key to use for authentication.
-            api_endpoint (str): The API endpoint to use for requests.
-            fn_endpoints (Dict[str, str]): A dictionary containing the API endpoints
-                for each function.
-            session (requests.Session): A requests session object to use for requests.
+            chatbot (str): The chatbot to use for chat.
+            database (str): The database to use for chat.
         """
+        # Chatbot config.
         self.api_key = api_key
+        self.chatbot = chatbot
+        self.database = database
+
+        # Network config.
         self.api_endpoint = os.getenv(
             "SILICRON_LOCAL_API_ENDPOINT", STAGING_API_ENDPOINT
         )
         self.fn_endpoints = {
             "chat": f"{self.api_endpoint}/chat",
             "upload": f"{self.api_endpoint}/upload",
         }
         self.session = requests.Session()
 
         # Set logging level
         logging.basicConfig(level=logging.INFO)
 
-    def chat(self, prompt: str, config: Dict[str, Any] = None) -> Dict[str, Any]:
+    def chat(self, prompt: str) -> Dict[str, Any]:
         """Send a chat prompt to the Silicron API and get a response.
 
         Args:
             prompt (str): The chat prompt to send to the Silicron API.
-            config (Dict[str, Any], optional): A dictionary containing additional
-                configuration for the API. Defaults to None.
 
         Returns:
             Dict[str, Any]: The response from the Silicron API as a dictionary.
 
         Raises:
             requests.exceptions.HTTPError: If an HTTP error occurs.
             requests.exceptions.RequestException: If a request error occurs.
         """
-        # Set default config if none provided
-        config = utils.set_config(config)
-
         # HTTP body for the request
-        body = {"api_key": self.api_key, "prompt": prompt, "config": config}
+        body = {
+            "api_key": self.api_key,
+            "prompt": prompt,
+            "config": {
+                "chatbot": self.chatbot,
+                "database": self.database,
+            },
+        }
 
         try:
             # Send POST request to Silicron API
             response = self.session.post(self.fn_endpoints["chat"], json=body)
 
             # Raise an HTTPError if the response contains an HTTP error status code
             response.raise_for_status()
 
             # Parse the JSON response body into a Python dictionary
             response_dict = response.json()
-            print(response_dict)
 
             # Update the response_code
             response_dict["response_code"] = 200
 
-            # Create an instance of ChatResponse
-            chat_response = models.ChatResponse(**response_dict)
-
-            return chat_response.dict()
+            return response_dict
 
         except requests.exceptions.HTTPError as http_err:
             return {"response": str(http_err), "response_code": 500}
         except requests.exceptions.RequestException as req_err:
             return {"response": str(req_err), "response_code": 500}
 
-    def upload(
-        self, files: Union[str, List[str]], database: str = ""
-    ) -> List[Dict[str, Any]]:
+    def upload(self, files: Union[str, List[str]]) -> List[Dict[str, Any]]:
         """Upload data to users' database.
 
         We can't use the json parameter in the requests.post() method because
         we need to send a file in the request body. JSON parameter is still the
         preferred way to send data to the API.
 
         TODO: Uploading a file into a non-existent index returns a 200 status code.
 
         Args:
             files (Union[str, List[str]]): The path to the data file or a list of
                 paths to process.
-            database (str): The name of their data split to get context from.
-                Defaults to ''.
 
         Returns:
             List[Dict[str, Any]]: The responses from the Silicron API as a list of dictionaries.
 
         Raises:
             requests.exceptions.HTTPError: If an HTTP error occurs.
             requests.exceptions.RequestException: If a request error occurs.
@@ -117,15 +123,15 @@
 
         for file in tqdm.tqdm(files, desc="Uploading files", unit="file"):
             try:
                 # Open the file in binary mode
                 with open(file, "rb") as f:
                     # HTTP body for the request
                     file_body = {"file": f}
-                    data_body = {"api_key": self.api_key, "database": database}
+                    data_body = {"api_key": self.api_key, "database": self.database}
 
                     # Send POST request to Silicron API
                     response = self.session.post(
                         self.fn_endpoints["upload"],
                         data=data_body,
                         files=file_body,
                     )
@@ -135,52 +141,41 @@
 
                     # Convert the response to a JSON object
                     response_json = response.json()
 
                     # Add a response_code field to the response
                     response_json["response_code"] = response.status_code
 
-                    # Enforce response schema
-                    responses.append(models.UploadResponse(**response_json))
+                    responses.append(response_json)  # Append the dictionary directly
 
             except FileNotFoundError as fnf_err:
                 logging.error(f"File not found: {file}. Error: {fnf_err}")
                 responses.append(
-                    models.UploadResponse(
-                        response=f"File not found: {file}", response_code=404
-                    )
+                    {"response": f"File not found: {file}", "response_code": 404}
                 )
             except requests.exceptions.HTTPError as http_err:
                 logging.error(f"HTTP error occurred while uploading {file}: {http_err}")
                 if response.status_code == 403:
                     responses.append(
-                        models.UploadResponse(
-                            response="Invalid API Key", response_code=403
-                        )
+                        {"response": "Invalid API Key", "response_code": 403}
                     )
                     break
                 else:
                     responses.append(
-                        models.UploadResponse(
-                            response="HTTP error occurred", response_code=500
-                        )
+                        {"response": "HTTP error occurred", "response_code": 500}
                     )
             except requests.exceptions.RequestException as req_err:
                 logging.error(
                     f"Request error occurred while uploading {file}: {req_err}"
                 )
                 responses.append(
-                    models.UploadResponse(
-                        response="Request error occurred", response_code=500
-                    )
+                    {"response": "Request error occurred", "response_code": 500}
                 )
             except Exception as e:
                 logging.error(
                     f"An unexpected error occurred while uploading {file}: {e}"
                 )
                 responses.append(
-                    UploadResponse(
-                        response="Unexpected error occurred", response_code=500
-                    )
+                    {"response": "Unexpected error occurred", "response_code": 500}
                 )
 
         return responses
```

