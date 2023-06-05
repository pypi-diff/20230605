# Comparing `tmp/python-keycloak-api-client-0.6.0.tar.gz` & `tmp/python-keycloak-api-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-keycloak-api-client-0.6.0.tar", last modified: Tue Mar  7 14:28:24 2023, max compression
+gzip compressed data, was "python-keycloak-api-client-0.7.0.tar", last modified: Mon Jun  5 10:37:27 2023, max compression
```

## Comparing `python-keycloak-api-client-0.6.0.tar` & `python-keycloak-api-client-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2000 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      959 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/keycloak_api_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/keycloak_api_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15138 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/keycloak_api_client/api_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/keycloak_api_client/data_classes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/keycloak_api_client/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/keycloak_api_client/factories.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2000 2023-03-07 14:28:24.000000 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1234 2023-03-07 14:28:24.000000 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-07 14:28:24.000000 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-03-07 14:28:24.000000 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-03-07 14:28:24.000000 python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      135 2023-03-07 14:28:24.382136 python-keycloak-api-client-0.6.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14554 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/api_client_test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-07 14:28:24.378136 python-keycloak-api-client-0.6.0/tests/cassettes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12289 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_count_users.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28025 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_create_client_and_create_mapper.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6942 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6950 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6512 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6513 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user_by_id.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12066 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_get_user_tokens.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37491 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_password_reset.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23632 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_register_then_update_then_get_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7379 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_search_for_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6945 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15948 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/cassettes/test_send_verification_email.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tests/factories_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-03-07 14:28:23.000000 python-keycloak-api-client-0.6.0/tox.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1072 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/keycloak_api_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16448 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/api_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1008 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/data_classes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/factories.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      135 2023-06-05 10:37:27.225013 python-keycloak-api-client-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17086 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/api_client_test.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/tests/cassettes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12289 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_count_users.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28025 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_create_client_and_create_mapper.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9991 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_delete_client.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6942 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6950 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6512 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6513 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_by_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12066 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_user_tokens.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37491 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_password_reset.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23632 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_register_then_update_then_get_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9710 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_clients_by_client_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7379 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6945 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15948 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_send_verification_email.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3344 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/factories_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tox.ini
```

### Comparing `python-keycloak-api-client-0.6.0/LICENSE.txt` & `python-keycloak-api-client-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/PKG-INFO` & `python-keycloak-api-client-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-api-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Client for Keycloak Api (mostly users and impersonation)
 Home-page: https://github.com/masterplandev/python-keycloak-api-client
 Author: Szymon Marcinkowski
 Author-email: szymon@masterhub.com
 License: MIT
 Description: # Python Keycloak Client
         
@@ -27,14 +27,18 @@
         
         ```bash
         $ pip install -e .
         ```
         
         ## Changelog
         
+        ### v0.7.0
+        - Added methods `search_clients_by_client_id` and `delete_client`
+        - Added `KeycloakClient` dataclass
+        
         ### v0.6.0
         - Added methods `create_client` and `create_mapper_for_client`
         
         ### v0.5.0
         - Added method `send_verification_email`
         
         ### v0.4.0
```

### Comparing `python-keycloak-api-client-0.6.0/README.md` & `python-keycloak-api-client-0.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
 ```bash
 $ pip install -e .
 ```
 
 ## Changelog
 
+### v0.7.0
+- Added methods `search_clients_by_client_id` and `delete_client`
+- Added `KeycloakClient` dataclass
+
 ### v0.6.0
 - Added methods `create_client` and `create_mapper_for_client`
 
 ### v0.5.0
 - Added method `send_verification_email`
 
 ### v0.4.0
```

### Comparing `python-keycloak-api-client-0.6.0/keycloak_api_client/api_client.py` & `python-keycloak-api-client-0.7.0/keycloak_api_client/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 from typing import List, Optional
 from urllib import parse
 from uuid import UUID
 
 import requests
 
 from keycloak_api_client.data_classes import (
+    KeycloakClient,
     KeycloakFederatedIdentity,
     KeycloakTokens,
     WriteKeycloakUser,
     ReadKeycloakUser
 )
 from keycloak_api_client.exceptions import KeycloakApiClientException
-from keycloak_api_client.factories import read_keycloak_user_factory
+from keycloak_api_client.factories import (
+    keycloak_client_factory,
+    read_keycloak_user_factory
+)
 
 
 class KeycloakApiClient:
 
     admin_user_access_token = None
 
     def __init__(
@@ -56,14 +60,17 @@
 
     def _get_send_verify_email_url(self, user_id: UUID) -> str:
         return f'{self._get_users_url()}/{user_id}/send-verify-email'
 
     def _get_clients_url(self) -> str:
         return f'{self.keycloak_url}/auth/admin/realms/{self.realm}/clients'
 
+    def _get_client_url(self, id_of_client: UUID) -> str:
+        return f'{self._get_clients_url()}/{id_of_client}'
+
     def _get_client_mappers_url(self, id_of_client: UUID) -> str:
         return f'{self._get_clients_url()}/{id_of_client}' \
                f'/protocol-mappers/models'
 
     def _get_authorization_header(self) -> str:
         return f'Bearer {self._get_api_admin_oidc_token()}'
 
@@ -447,7 +454,41 @@
                 'Content-Type': 'application/json'
             }
         )
         if not response.ok:
             raise KeycloakApiClientException(
                 f'Error while creating client mapper with data={data}'
             )
+
+    def search_clients_by_client_id(
+        self,
+        client_id: str
+    ) -> List[KeycloakClient]:
+
+        response = requests.get(
+            self._get_clients_url(),
+            params={
+                "clientId": client_id,
+                "search": True
+            },
+            headers={'Authorization': self._get_authorization_header()}
+        )
+        if not response.ok:
+            raise KeycloakApiClientException(
+                'Error while retrieving client data by clientId '
+                f'(clientId: {client_id})'
+            )
+        return [
+            keycloak_client_factory(client) for client in response.json()
+        ]
+
+    def delete_client(self, id_of_client: UUID) -> None:
+        response = requests.delete(
+            self._get_client_url(id_of_client=id_of_client),
+            headers={'Authorization': self._get_authorization_header()}
+        )
+        if not response.ok:
+            raise KeycloakApiClientException(
+                'Error while deleting client '
+                f'with ID={id_of_client}) '
+                f'response code={response.status_code}'
+            )
```

### Comparing `python-keycloak-api-client-0.6.0/keycloak_api_client/data_classes.py` & `python-keycloak-api-client-0.7.0/keycloak_api_client/data_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,7 +36,15 @@
     raw_data: dict
 
 
 @attr.s(auto_attribs=True)
 class KeycloakTokens:
     access_token: str
     refresh_token: str
+
+
+@attr.s(auto_attribs=True)
+class KeycloakClient:
+    keycloak_id: UUID
+    client_id: str
+    enabled: bool
+    service_account_enabled: bool
```

### Comparing `python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/PKG-INFO` & `python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-api-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Client for Keycloak Api (mostly users and impersonation)
 Home-page: https://github.com/masterplandev/python-keycloak-api-client
 Author: Szymon Marcinkowski
 Author-email: szymon@masterhub.com
 License: MIT
 Description: # Python Keycloak Client
         
@@ -27,14 +27,18 @@
         
         ```bash
         $ pip install -e .
         ```
         
         ## Changelog
         
+        ### v0.7.0
+        - Added methods `search_clients_by_client_id` and `delete_client`
+        - Added `KeycloakClient` dataclass
+        
         ### v0.6.0
         - Added methods `create_client` and `create_mapper_for_client`
         
         ### v0.5.0
         - Added method `send_verification_email`
         
         ### v0.4.0
```

### Comparing `python-keycloak-api-client-0.6.0/python_keycloak_api_client.egg-info/SOURCES.txt` & `python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 python_keycloak_api_client.egg-info/dependency_links.txt
 python_keycloak_api_client.egg-info/requires.txt
 python_keycloak_api_client.egg-info/top_level.txt
 tests/api_client_test.py
 tests/factories_test.py
 tests/cassettes/test_count_users.yaml
 tests/cassettes/test_create_client_and_create_mapper.yaml
+tests/cassettes/test_delete_client.yaml
 tests/cassettes/test_get_existing_user.yaml
 tests/cassettes/test_get_existing_user_by_keycloak_id.yaml
 tests/cassettes/test_get_not_existing_user.yaml
 tests/cassettes/test_get_not_existing_user_by_id.yaml
 tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml
 tests/cassettes/test_get_user_tokens.yaml
 tests/cassettes/test_password_reset.yaml
 tests/cassettes/test_register_then_update_then_get_user.yaml
+tests/cassettes/test_search_clients_by_client_id.yaml
 tests/cassettes/test_search_for_existing_user.yaml
 tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml
 tests/cassettes/test_send_verification_email.yaml
```

### Comparing `python-keycloak-api-client-0.6.0/setup.py` & `python-keycloak-api-client-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='python-keycloak-api-client',
-    version='0.6.0',
+    version='0.7.0',
     description='Client for Keycloak Api (mostly users and impersonation)',
     keywords='keycloak,client,api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Szymon Marcinkowski',
     author_email='szymon@masterhub.com',
     license='MIT',
```

### Comparing `python-keycloak-api-client-0.6.0/tests/api_client_test.py` & `python-keycloak-api-client-0.7.0/tests/api_client_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional
 from uuid import UUID
 
 import pytest
 
 from keycloak_api_client import KeycloakApiClient
 from keycloak_api_client.data_classes import (
+    KeycloakClient,
     KeycloakFederatedIdentity,
     KeycloakTokens,
     ReadKeycloakUser,
     WriteKeycloakUser
 )
 from keycloak_api_client.exceptions import KeycloakApiClientException
 from keycloak_api_client.factories import read_keycloak_user_factory
@@ -51,14 +52,46 @@
     "notBefore": 0,
     "access": {
         "manageGroupMembership": True, "view": True,
         "mapRoles": True, "impersonate": True, "manage": True
     }
 }
 
+raw_existing_client_data = {
+    'access': {'configure': True, 'manage': True, 'view': True},
+    'alwaysDisplayInConsole': False,
+    'attributes': {'backchannel.logout.revoke.offline.tokens': 'false',
+                   'backchannel.logout.session.required': 'true'},
+    'authenticationFlowBindingOverrides': {},
+    'bearerOnly': False,
+    'clientAuthenticatorType': 'client-secret',
+    'clientId': 'existing_client_id',
+    'consentRequired': False,
+    'defaultClientScopes': ['web-origins', 'acr', 'roles', 'profile', 'email'],
+    'directAccessGrantsEnabled': True,
+    'enabled': True,
+    'frontchannelLogout': False,
+    'fullScopeAllowed': True,
+    'id': '15d9cce8-2e11-4f37-adde-cb686d037a60',
+    'implicitFlowEnabled': False,
+    'nodeReRegistrationTimeout': -1,
+    'notBefore': 0,
+    'optionalClientScopes': ['address',
+                             'phone',
+                             'offline_access',
+                             'microprofile-jwt'],
+    'protocol': 'openid-connect',
+    'publicClient': True,
+    'redirectUris': [],
+    'serviceAccountsEnabled': False,
+    'standardFlowEnabled': True,
+    'surrogateAuthRequired': False,
+    'webOrigins': []
+}
+
 
 def _keycloak_api_client_factory():
     return KeycloakApiClient(
         keycloak_url='http://localhost:8080',
         realm='my-realm',
         admin_username='admin-user',
         admin_password='admin-pass',
@@ -407,7 +440,49 @@
         "'claim.value': 'any_value', "
         "'id.token.claim': 'false', "
         "'userinfo.token.claim': 'false'}, "
         "'name': 'Test "
         "mapper', 'protocolMapper': "
         "'oidc-hardcoded-claim-mapper'}"
     )
+
+
+@pytest.mark.vcr()
+def test_search_clients_by_client_id():
+    existing_client_id = "existing_client_id"
+    non_existing_client_id = "not_existing_client_id"
+    keycloak_api_client = _keycloak_api_client_factory()
+    assert keycloak_api_client.search_clients_by_client_id(
+        client_id=existing_client_id
+    ) == [
+        KeycloakClient(
+            keycloak_id=UUID(raw_existing_client_data["id"]),
+            client_id=raw_existing_client_data["clientId"],
+            enabled=raw_existing_client_data["enabled"],
+            service_account_enabled=(
+                raw_existing_client_data["serviceAccountsEnabled"]
+            )
+        )
+    ]
+    assert keycloak_api_client.search_clients_by_client_id(
+        client_id=non_existing_client_id
+    ) == []
+
+
+@pytest.mark.vcr()
+def test_delete_client():
+    keycloak_api_client = _keycloak_api_client_factory()
+
+    with pytest.raises(KeycloakApiClientException) as ex:
+        keycloak_api_client.delete_client(
+            id_of_client=UUID("00000000-0000-0000-0000-000000000000")
+        )
+
+    assert str(ex.value) == (
+        "Error while deleting client with "
+        "ID=00000000-0000-0000-0000-000000000000) "
+        "response code=404"
+    )
+
+    keycloak_api_client.delete_client(
+        id_of_client=raw_existing_client_data['id']
+    )
```

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_count_users.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_count_users.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_create_client_and_create_mapper.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_create_client_and_create_mapper.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_existing_user.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user_by_id.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_by_id.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_get_user_tokens.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_user_tokens.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_password_reset.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_password_reset.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_register_then_update_then_get_user.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_register_then_update_then_get_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_search_for_existing_user.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.6.0/tests/cassettes/test_send_verification_email.yaml` & `python-keycloak-api-client-0.7.0/tests/cassettes/test_send_verification_email.yaml`

 * *Files identical despite different names*

