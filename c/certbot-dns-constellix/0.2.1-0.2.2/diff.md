# Comparing `tmp/certbot-dns-constellix-0.2.1.tar.gz` & `tmp/certbot-dns-constellix-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-constellix-0.2.1.tar", last modified: Fri Oct 30 15:44:00 2020, max compression
+gzip compressed data, was "certbot-dns-constellix-0.2.2.tar", last modified: Mon Jun  5 12:23:16 2023, max compression
```

## Comparing `certbot-dns-constellix-0.2.1.tar` & `certbot-dns-constellix-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 15:44:00.992952 certbot-dns-constellix-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6102 2020-10-30 15:44:00.992952 certbot-dns-constellix-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4120 2020-10-30 15:43:53.000000 certbot-dns-constellix-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 15:44:00.988952 certbot-dns-constellix-0.2.1/certbot_dns_constellix/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-30 15:43:53.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10263 2020-10-30 15:43:53.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix/dns_constellix.py
--rw-r--r--   0 runner    (1001) docker     (116)     5928 2020-10-30 15:43:53.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix/dns_constellix_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 15:44:00.988952 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6102 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      428 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       88 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-10-30 15:44:00.000000 certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-10-30 15:44:00.992952 certbot-dns-constellix-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2052 2020-10-30 15:43:53.000000 certbot-dns-constellix-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:23:16.929472 certbot-dns-constellix-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-05 12:23:06.000000 certbot-dns-constellix-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-05 12:23:16.929472 certbot-dns-constellix-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-05 12:23:06.000000 certbot-dns-constellix-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:23:16.929472 certbot-dns-constellix-0.2.2/certbot_dns_constellix/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:23:06.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-05 12:23:06.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix/dns_constellix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:23:16.929472 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 12:23:16.000000 certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 12:23:16.929472 certbot-dns-constellix-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-05 12:23:06.000000 certbot-dns-constellix-0.2.2/setup.py
```

### Comparing `certbot-dns-constellix-0.2.1/PKG-INFO` & `certbot-dns-constellix-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,15 @@
 Metadata-Version: 2.1
 Name: certbot-dns-constellix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Constellix DNS Authenticator plugin for Certbot
 Home-page: https://github.com/Constellix/certbot-constellix
 Author: Jessica Smith
-Author-email: jsmith@constellix.com
+Author-email: jsmith@tiggee.com
 License: Apache License 2.0
-Description: # certbot-dns-constellix Documentation
-        
-        The `certbot-dns-constellix` plugin is used to automate the process of a `dns-01` challenge in Certbot to allow the requesting and renewal of SSL certificates through the Constellix DNS API.
-        
-        This is done through the process of adding and removing TXT records to the appropriate domain in your Constellix DNS account. 
-        
-        There are two different methods of installing, configuring and using the plugin depending on if you're using certbot installed through snapd or through your operating system's package manager.
-        
-        ## Certbot Installed using Snapd
-        
-        If you installed certbot using snapd, do the following to install and configure the plugin:
-        
-        ### Installation
-        
-        Run the following commands to install the plugin with snapd.
-        
-        ```
-        sudo snap install certbot-dns-constellix
-        sudo snap set certbot trust-plugin-with-root=ok
-        sudo snap connect certbot:plugin certbot-dns-constellix
-        ```
-        
-        Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
-        
-        ### Configuration
-        
-        The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
-        
-        These will need to be added to a file, eg. `constellix.ini` in the following format:
-        
-        ```
-        dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
-        dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
-        dns_constellix_endpoint=https://api.dns.constellix.com/v1
-        ```
-        
-        #### Caution
-        
-        You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
-        
-        ### Usage
-        
-        Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
-        
-        ```
-        certbot certonly \
-            --authenticator=dns-constellix \
-            --dns-constellix-credentials=~./constellix.ini \
-            -d example.com
-        ```
-        
-        For more options please check the certbot documentation.
-        
-        ## Certbot Installed using OS Package Manager/Python
-        
-        If you installed certbot using your operating system's package manager (apt, yum, etc.) or directly with Python, you can install it using these instructions.
-        
-        ### Installation
-        
-        Run the following commands to install the plugin using pip.
-        
-        ```
-        sudo python3 -m pip install certbot-dns-constellix
-        ```
-        
-        Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
-        
-        ### Configuration
-        
-        The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
-        
-        These will need to be added to a file, eg. `constellix.ini` in the following format:
-        
-        ```
-        certbot-dns-constellix:dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
-        certbot-dns-constellix:dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
-        certbot-dns-constellix:dns_constellix_endpoint=https://api.dns.constellix.com/v1
-        ```
-        
-        The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
-        
-        #### Caution
-        
-        You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
-        
-        ### Usage
-        
-        Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
-        
-        ```
-        certbot certonly \
-            --authenticator=certbot-dns-constellix:dns-constellix \
-            --certbot-dns-constellix:dns-constellix-credentials=~./constellix.ini \
-            -d example.com
-        ```
-        
-        The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
-        
-        For more options please check the certbot documentation.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -125,7 +23,122 @@
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# certbot-dns-constellix Documentation
+
+The `certbot-dns-constellix` plugin is used to automate the process of a `dns-01` challenge in Certbot to allow the requesting and renewal of SSL certificates through the Constellix DNS API.
+
+This is done through the process of adding and removing TXT records to the appropriate domain in your Constellix DNS account. 
+
+There are two different methods of installing, configuring and using the plugin depending on if you're using certbot installed through snapd or through your operating system's package manager.
+
+## Certbot Installed using Snapd
+
+If you installed certbot using snapd, do the following to install and configure the plugin:
+
+### Installation
+
+Run the following commands to install the plugin with snapd.
+
+```
+sudo snap install certbot-dns-constellix
+sudo snap set certbot trust-plugin-with-root=ok
+sudo snap connect certbot:plugin certbot-dns-constellix
+```
+
+Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
+
+### Configuration
+
+The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
+
+These will need to be added to a file, eg. `constellix.ini` in the following format:
+
+```
+dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
+dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
+dns_constellix_endpoint=https://api.dns.constellix.com/v1
+```
+
+#### Caution
+
+You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
+
+### Usage
+
+Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
+
+```
+certbot certonly \
+    --authenticator=dns-constellix \
+    --dns-constellix-credentials=~./constellix.ini \
+    -d example.com
+```
+
+For more options please check the certbot documentation.
+
+## Certbot Installed using OS Package Manager/Python
+
+If you installed certbot using your operating system's package manager (apt, yum, etc.) or directly with Python, you can install it using these instructions.
+
+### Installation
+
+Run the following commands to install the plugin using pip.
+
+```
+sudo python3 -m pip install certbot-dns-constellix
+```
+
+Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
+
+### Configuration
+
+The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
+
+These will need to be added to a file, eg. `constellix.ini` in the following format:
+
+```
+certbot-dns-constellix:dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
+certbot-dns-constellix:dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
+certbot-dns-constellix:dns_constellix_endpoint=https://api.dns.constellix.com/v1
+```
+
+The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
+
+#### Caution
+
+You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
+
+### Usage
+
+Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
+
+```
+certbot certonly \
+    --authenticator=certbot-dns-constellix:dns-constellix \
+    --certbot-dns-constellix:dns-constellix-credentials=~./constellix.ini \
+    -d example.com
+```
+
+The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
+
+For more options please check the certbot documentation.
+
+## License
+
+Copyright 2020 Constellix, a division of Tiggee LLC.
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.
+
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+
+See the License for the specific language governing permissions and limitations under the License.
```

### Comparing `certbot-dns-constellix-0.2.1/README.md` & `certbot-dns-constellix-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -94,7 +94,20 @@
     -d example.com
 ```
 
 The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
 
 For more options please check the certbot documentation.
 
+## License
+
+Copyright 2020 Constellix, a division of Tiggee LLC.
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.
+
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+
+See the License for the specific language governing permissions and limitations under the License.
```

### Comparing `certbot-dns-constellix-0.2.1/certbot_dns_constellix/dns_constellix.py` & `certbot-dns-constellix-0.2.2/certbot_dns_constellix/dns_constellix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """DNS Authenticator for Constellix."""
-import json
 import logging
 import time
 import hmac
 import hashlib
 from base64 import b64encode
 
 import requests
-import zope.interface
 
 from certbot import errors
-from certbot import interfaces
 from certbot.plugins import dns_common
 
 logger = logging.getLogger(__name__)
 
-
-@zope.interface.implementer(interfaces.IAuthenticator)
-@zope.interface.provider(interfaces.IPluginFactory)
 class Authenticator(dns_common.DNSAuthenticator):
     """DNS Authenticator for Constellix
 
     This Authenticator uses the Constellix DNS REST API to fulfill a dns-01 challenge.
     """
 
     description = "Obtain certificates using a DNS TXT record (if you are using Constellix for DNS)."
@@ -223,15 +217,15 @@
             try:
                 logger.debug("looking for zone: %s", zone_name)
                 status_code, result = self._api_request("GET", "domains/search?exact={0}".format(zone_name), {})
                 if status_code == 200 and len(result) > 0:
                     return result[0]['id'], result[0]['name']
             except errors.PluginError as e:
                 pass
-        return None
+        return None, None
 
     def get_existing_txt(self, zone_id, record_name, record_content):
         """
         Get existing TXT records for the record name.
 
         If an error occurs while requesting the record set, it is suppressed
         and None is returned.
```

### Comparing `certbot-dns-constellix-0.2.1/certbot_dns_constellix.egg-info/PKG-INFO` & `certbot-dns-constellix-0.2.2/certbot_dns_constellix.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,15 @@
 Metadata-Version: 2.1
 Name: certbot-dns-constellix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Constellix DNS Authenticator plugin for Certbot
 Home-page: https://github.com/Constellix/certbot-constellix
 Author: Jessica Smith
-Author-email: jsmith@constellix.com
+Author-email: jsmith@tiggee.com
 License: Apache License 2.0
-Description: # certbot-dns-constellix Documentation
-        
-        The `certbot-dns-constellix` plugin is used to automate the process of a `dns-01` challenge in Certbot to allow the requesting and renewal of SSL certificates through the Constellix DNS API.
-        
-        This is done through the process of adding and removing TXT records to the appropriate domain in your Constellix DNS account. 
-        
-        There are two different methods of installing, configuring and using the plugin depending on if you're using certbot installed through snapd or through your operating system's package manager.
-        
-        ## Certbot Installed using Snapd
-        
-        If you installed certbot using snapd, do the following to install and configure the plugin:
-        
-        ### Installation
-        
-        Run the following commands to install the plugin with snapd.
-        
-        ```
-        sudo snap install certbot-dns-constellix
-        sudo snap set certbot trust-plugin-with-root=ok
-        sudo snap connect certbot:plugin certbot-dns-constellix
-        ```
-        
-        Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
-        
-        ### Configuration
-        
-        The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
-        
-        These will need to be added to a file, eg. `constellix.ini` in the following format:
-        
-        ```
-        dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
-        dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
-        dns_constellix_endpoint=https://api.dns.constellix.com/v1
-        ```
-        
-        #### Caution
-        
-        You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
-        
-        ### Usage
-        
-        Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
-        
-        ```
-        certbot certonly \
-            --authenticator=dns-constellix \
-            --dns-constellix-credentials=~./constellix.ini \
-            -d example.com
-        ```
-        
-        For more options please check the certbot documentation.
-        
-        ## Certbot Installed using OS Package Manager/Python
-        
-        If you installed certbot using your operating system's package manager (apt, yum, etc.) or directly with Python, you can install it using these instructions.
-        
-        ### Installation
-        
-        Run the following commands to install the plugin using pip.
-        
-        ```
-        sudo python3 -m pip install certbot-dns-constellix
-        ```
-        
-        Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
-        
-        ### Configuration
-        
-        The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
-        
-        These will need to be added to a file, eg. `constellix.ini` in the following format:
-        
-        ```
-        certbot-dns-constellix:dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
-        certbot-dns-constellix:dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
-        certbot-dns-constellix:dns_constellix_endpoint=https://api.dns.constellix.com/v1
-        ```
-        
-        The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
-        
-        #### Caution
-        
-        You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
-        
-        ### Usage
-        
-        Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
-        
-        ```
-        certbot certonly \
-            --authenticator=certbot-dns-constellix:dns-constellix \
-            --certbot-dns-constellix:dns-constellix-credentials=~./constellix.ini \
-            -d example.com
-        ```
-        
-        The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
-        
-        For more options please check the certbot documentation.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -125,7 +23,122 @@
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# certbot-dns-constellix Documentation
+
+The `certbot-dns-constellix` plugin is used to automate the process of a `dns-01` challenge in Certbot to allow the requesting and renewal of SSL certificates through the Constellix DNS API.
+
+This is done through the process of adding and removing TXT records to the appropriate domain in your Constellix DNS account. 
+
+There are two different methods of installing, configuring and using the plugin depending on if you're using certbot installed through snapd or through your operating system's package manager.
+
+## Certbot Installed using Snapd
+
+If you installed certbot using snapd, do the following to install and configure the plugin:
+
+### Installation
+
+Run the following commands to install the plugin with snapd.
+
+```
+sudo snap install certbot-dns-constellix
+sudo snap set certbot trust-plugin-with-root=ok
+sudo snap connect certbot:plugin certbot-dns-constellix
+```
+
+Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
+
+### Configuration
+
+The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
+
+These will need to be added to a file, eg. `constellix.ini` in the following format:
+
+```
+dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
+dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
+dns_constellix_endpoint=https://api.dns.constellix.com/v1
+```
+
+#### Caution
+
+You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
+
+### Usage
+
+Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
+
+```
+certbot certonly \
+    --authenticator=dns-constellix \
+    --dns-constellix-credentials=~./constellix.ini \
+    -d example.com
+```
+
+For more options please check the certbot documentation.
+
+## Certbot Installed using OS Package Manager/Python
+
+If you installed certbot using your operating system's package manager (apt, yum, etc.) or directly with Python, you can install it using these instructions.
+
+### Installation
+
+Run the following commands to install the plugin using pip.
+
+```
+sudo python3 -m pip install certbot-dns-constellix
+```
+
+Verify that the plugin is installed by running `certbot plugins`. You should see the `dns-constellix` plugin in the list.
+
+### Configuration
+
+The plugin requires an API key and secret key for the Constellix DNS API. The key will need to have permissions to add and remove records on the domain you want to issue certificates for.
+
+These will need to be added to a file, eg. `constellix.ini` in the following format:
+
+```
+certbot-dns-constellix:dns_constellix_apikey=5fb4e76f-ac91-43e5-f982458bc595
+certbot-dns-constellix:dns_constellix_secretkey=47d99fd0-32e7-4e07-85b46d08e70b
+certbot-dns-constellix:dns_constellix_endpoint=https://api.dns.constellix.com/v1
+```
+
+The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
+
+#### Caution
+
+You should secure this file from any unauthorised access. Anyone with access to these credentials and this file will be able to add and remove records from your domain. You should configure the file to not be readable by any other users on the system
+
+### Usage
+
+Once the plugin is installed and configured it can be used by specifying the plugin in the `certbot` command and the location of the credentials file.
+
+```
+certbot certonly \
+    --authenticator=certbot-dns-constellix:dns-constellix \
+    --certbot-dns-constellix:dns-constellix-credentials=~./constellix.ini \
+    -d example.com
+```
+
+The extra `certbot-dns-constellix:` is required due to how older versions of Certbot load plugins.
+
+For more options please check the certbot documentation.
+
+## License
+
+Copyright 2020 Constellix, a division of Tiggee LLC.
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.
+
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+
+See the License for the specific language governing permissions and limitations under the License.
```

### Comparing `certbot-dns-constellix-0.2.1/setup.py` & `certbot-dns-constellix-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
-version = "0.2.1"
+version = "0.2.2"
 
 install_requires = [
     "acme>=0.29.0",
-    "certbot>=0.31.0",
+    "certbot>=2.0,<3.0",
     "setuptools",
     "requests",
     "mock",
     "requests-mock",
 ]
 
 # read the contents of your README file
@@ -23,15 +23,15 @@
     name="certbot-dns-constellix",
     version=version,
     description="Constellix DNS Authenticator plugin for Certbot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Constellix/certbot-constellix",
     author="Jessica Smith",
-    author_email="jsmith@constellix.com",
+    author_email="jsmith@tiggee.com",
     license="Apache License 2.0",
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Plugins",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: Apache Software License",
```

