# Comparing `tmp/cert_manager-2.3.0.tar.gz` & `tmp/cert_manager-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert_manager-2.3.0.tar", max compression
+gzip compressed data, was "cert_manager-2.3.1.tar", max compression
```

## Comparing `cert_manager-2.3.0.tar` & `cert_manager-2.3.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1496 2022-09-12 15:32:36.583713 cert_manager-2.3.0/LICENSE.txt
--rw-r--r--   0        0        0     6606 2022-09-12 15:32:36.583713 cert_manager-2.3.0/README.md
--rw-r--r--   0        0        0      464 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/__init__.py
--rw-r--r--   0        0        0      282 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/__version__.py
--rw-r--r--   0        0        0    10489 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/_certificates.py
--rw-r--r--   0        0        0     2323 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/_endpoint.py
--rw-r--r--   0        0        0     6242 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/_helpers.py
--rw-r--r--   0        0        0     6334 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/acme.py
--rw-r--r--   0        0        0     5234 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/admin.py
--rw-r--r--   0        0        0     8377 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/client.py
--rw-r--r--   0        0        0     7548 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/domain.py
--rw-r--r--   0        0        0     3345 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/organization.py
--rw-r--r--   0        0        0     1504 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/person.py
--rw-r--r--   0        0        0     4950 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/report.py
--rw-r--r--   0        0        0     9322 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/smime.py
--rw-r--r--   0        0        0     2093 2022-09-12 15:32:36.583713 cert_manager-2.3.0/cert_manager/ssl.py
--rw-r--r--   0        0        0      901 2022-09-12 15:32:36.583713 cert_manager-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     7520 1970-01-01 00:00:00.000000 cert_manager-2.3.0/setup.py
--rw-r--r--   0        0        0     7437 1970-01-01 00:00:00.000000 cert_manager-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-06-05 13:27:19.106395 cert_manager-2.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     6449 2023-06-05 13:27:19.106395 cert_manager-2.3.1/README.md
+-rw-r--r--   0        0        0      464 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/__version__.py
+-rw-r--r--   0        0        0    10552 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/_certificates.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/_endpoint.py
+-rw-r--r--   0        0        0     6345 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/_helpers.py
+-rw-r--r--   0        0        0     6391 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/acme.py
+-rw-r--r--   0        0        0     5234 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/admin.py
+-rw-r--r--   0        0        0     8377 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/client.py
+-rw-r--r--   0        0        0     7548 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/domain.py
+-rw-r--r--   0        0        0     3345 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/organization.py
+-rw-r--r--   0        0        0     1504 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/person.py
+-rw-r--r--   0        0        0     4950 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/report.py
+-rw-r--r--   0        0        0     9322 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/smime.py
+-rw-r--r--   0        0        0     2093 2023-06-05 13:27:19.106395 cert_manager-2.3.1/cert_manager/ssl.py
+-rw-r--r--   0        0        0      887 2023-06-05 13:27:19.110395 cert_manager-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7331 1970-01-01 00:00:00.000000 cert_manager-2.3.1/PKG-INFO
```

### Comparing `cert_manager-2.3.0/LICENSE.txt` & `cert_manager-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/README.md` & `cert_manager-2.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # python-cert_manager
 
 This library provides a [Python][1] interface to the [Sectigo][2] Certificate Manager REST API.  python-cert_manager is open sourced under the [BSD 3-Clause license](LICENSE.txt).
 
 ![checks](https://github.com/broadinstitute/python-cert_manager/workflows/checks/badge.svg?branch=main)
-[![codecov](https://codecov.io/gh/broadinstitute/python-cert_manager/branch/main/graph/badge.svg)](https://codecov.io/gh/broadinstitute/python-cert_manager)
 
 ## Basics
 
 `cert_manager` runs on [Python][1] >= 3.7
 
 ## Features
```

### Comparing `cert_manager-2.3.0/cert_manager/_certificates.py` & `cert_manager-2.3.1/cert_manager/_certificates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Define the cert_manager._certificate.Certificates base class."""
 
 import logging
 from requests.exceptions import HTTPError
 
-from ._helpers import Pending
+from ._helpers import CustomFieldsError, Pending
 from ._endpoint import Endpoint
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Certificates(Endpoint):
     """Act as a superclass for all certificate-related classes.
@@ -87,43 +87,43 @@
         :raises Exception: if any of the validation steps fail
         """
         # Make sure all custom fields are valid if present
         custom_field_names = [f['name'] for f in self.custom_fields]
         for custom_field in custom_fields:
             if not isinstance(custom_field, dict):
                 msg = "Values in the custom_fields list must be dictionaries, not {}"
-                raise Exception(msg.format(type(custom_field)))
+                raise CustomFieldsError(msg.format(type(custom_field)))
             if not ('name' in custom_field and 'value' in custom_field):
-                raise Exception(
+                raise CustomFieldsError(
                     "Dictionaries in the custom_fields list must contain both a 'name' key and 'value' key"
                 )
             if custom_field.get('name') not in custom_field_names:
                 msg = "Custom field {} not defined for your account. defined custom fields are {}"
-                raise Exception(msg.format(custom_field.get('name'), custom_field_names))
+                raise CustomFieldsError(msg.format(custom_field.get('name'), custom_field_names))
         mandatory_fields = [f['name'] for f in self.custom_fields if f['mandatory'] is True]
         for field_name in mandatory_fields:
             # for each mandatory field, there should be exactly one dict in the custom_fields list
             # whose name matches that mandatory field name
             matching_fields = [f for f in custom_fields if f['name'] == field_name]
             if len(matching_fields) < 1:
-                raise Exception(f"Missing mandatory custom field {field_name}")
+                raise CustomFieldsError(f"Missing mandatory custom field {field_name}")
             if len(matching_fields) > 1:
-                raise Exception(f"Too many custom field objects with name {field_name}")
+                raise CustomFieldsError(f"Too many custom field objects with name {field_name}")
 
     def collect(self, cert_id, cert_format):
         """Retrieve an existing certificate from the API.
 
         This method will raise a Pending exception if the certificate is still in a pending state.
 
         :param int cert_id: The certificate ID
         :param str cert_format: The format in which to retreive the certificate. Allowed values: *self.valid_formats*
         :return str: the string representing the certificate in the requested format
         """
         if cert_format not in self.valid_formats:
-            raise Exception(f"Invalid cert format {cert_format} provided")
+            raise ValueError(f"Invalid cert format {cert_format} provided")
 
         url = self._url(f"/collect/{cert_id}/{cert_format}")
 
         try:
             result = self._client.get(url)
         except HTTPError as exc:
             raise Pending(f"certificate {cert_id} still in 'pending' state") from exc
@@ -152,25 +152,25 @@
         org_id = kwargs.get("org_id")
         subject_alt_names = kwargs.get("subject_alt_names", None)
         external_requester = kwargs.get("external_requester", None)
         custom_fields = kwargs.get("custom_fields", [])
 
         # Make sure a valid certificate type name was provided
         if cert_type_name not in self.types:
-            raise Exception(f"Incorrect certificate type specified: '{cert_type_name}'")
+            raise ValueError(f"Incorrect certificate type specified: '{cert_type_name}'")
 
         type_id = self.types[cert_type_name]["id"]
         terms = self.types[cert_type_name]["terms"]
 
         # Make sure a valid term is specified
         if term not in terms:
             # You have to do the list/map/str thing because join can only operate on
             # a list of strings, and this will be a list of numbers
             trm = ", ".join(list(map(str, terms)))
-            raise Exception(f"Incorrect term specified: {term}.  Valid terms are {trm}.")
+            raise ValueError(f"Incorrect term specified: {term}.  Valid terms are {trm}.")
 
         self._validate_custom_fields(custom_fields)
 
         # SAN field needs to be a comma-separated string, not a list, opposite to replace
         final_san = subject_alt_names
         if isinstance(subject_alt_names, list):
             final_san = ",".join(subject_alt_names)
@@ -226,15 +226,15 @@
             Reason can be up to 512 characters and cannot be blank (i.e. empty string)
         :return dict: The revocation result. "Successful" on success
         """
         url = self._url(f"/revoke/{cert_id}")
 
         # Sectigo has a 512 character limit on the "reason" message, so catch that here.
         if (not reason) or (len(reason) > 511):
-            raise Exception("Sectigo limit: reason must be > 0 character and < 512 characters")
+            raise ValueError("Sectigo limit: reason must be > 0 character and < 512 characters")
 
         data = {"reason": reason}
 
         result = self._client.post(url, data=data)
         result.raise_for_status()
 
         return {}
```

### Comparing `cert_manager-2.3.0/cert_manager/_endpoint.py` & `cert_manager-2.3.1/cert_manager/_endpoint.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/_helpers.py` & `cert_manager-2.3.1/cert_manager/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,11 @@
     """Serve as a generic Exception indicating a certificate is in a pending state."""
     CODE = -183
 
 
 class Revoked(Exception):
     """Serve as a generic Exception indicating a certificate has been revoked"""
     CODE = -192
+
+
+class CustomFieldsError(Exception):
+    """Exception when custom fields do not have correct data."""
```

### Comparing `cert_manager-2.3.0/cert_manager/acme.py` & `cert_manager-2.3.1/cert_manager/acme.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 class ACMEAccount(Endpoint):
     """Query the Sectigo Cert Manager REST API for ACME Account data."""
     _find_params_to_api = {
         "org_id": "organizationId",
         "name": "name",
         "acme_server": "acmeServer",
         "cert_validation_type": "certValidationType",
-        "status": "status"
+        "status": "status",
+        "size": "size",
+        "position": "position",
     }
 
     def __init__(self, client, api_version="v1"):
         """Initialize the class.
 
         Note: The *all* method will be run on object instantiation to fetch all acme accounts
```

### Comparing `cert_manager-2.3.0/cert_manager/admin.py` & `cert_manager-2.3.1/cert_manager/admin.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/client.py` & `cert_manager-2.3.1/cert_manager/client.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/domain.py` & `cert_manager-2.3.1/cert_manager/domain.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/organization.py` & `cert_manager-2.3.1/cert_manager/organization.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/person.py` & `cert_manager-2.3.1/cert_manager/person.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/report.py` & `cert_manager-2.3.1/cert_manager/report.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/smime.py` & `cert_manager-2.3.1/cert_manager/smime.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/cert_manager/ssl.py` & `cert_manager-2.3.1/cert_manager/ssl.py`

 * *Files identical despite different names*

### Comparing `cert_manager-2.3.0/pyproject.toml` & `cert_manager-2.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cert_manager"
-version = "2.3.0"
+version = "2.3.1"
 description = "Python interface to the Sectigo Certificate Manager REST API"
 license = "BSD-3-Clause"
 authors = ["Andrew Teixeira <teixeira@broadinstitute.org>"]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/python-cert_manager.git"
 homepage = "https://github.com/broadinstitute/python-cert_manager.git"
 keywords = ["sectigo", "comodo", "certificate"]
@@ -12,15 +12,14 @@
 [tool.poetry.dependencies]
 python = "^3.7"  # Compatible python versions must be declared here
 requests = "*"
 toml = ">=0.9,<0.11"
 
 [tool.poetry.dev-dependencies]
 bump2version = "*"
-codecov = "*"
 coverage = ">=4.4.2"
 fixtures = "*"
 green = ">=2.12.0"
 mock = ">=2.0.0"
 pydocstyle = "<7"
 # 2.5.0 breaks pylama 8.3.8
 pyflakes = "< 2.5.0"
```

### Comparing `cert_manager-2.3.0/setup.py` & `cert_manager-2.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,191 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cert-manager
+Version: 2.3.1
+Summary: Python interface to the Sectigo Certificate Manager REST API
+Home-page: https://github.com/broadinstitute/python-cert_manager.git
+License: BSD-3-Clause
+Keywords: sectigo,comodo,certificate
+Author: Andrew Teixeira
+Author-email: teixeira@broadinstitute.org
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests
+Requires-Dist: toml (>=0.9,<0.11)
+Project-URL: Repository, https://github.com/broadinstitute/python-cert_manager.git
+Description-Content-Type: text/markdown
+
+# python-cert_manager
+
+This library provides a [Python][1] interface to the [Sectigo][2] Certificate Manager REST API.  python-cert_manager is open sourced under the [BSD 3-Clause license](LICENSE.txt).
+
+![checks](https://github.com/broadinstitute/python-cert_manager/workflows/checks/badge.svg?branch=main)
+
+## Basics
+
+`cert_manager` runs on [Python][1] >= 3.7
+
+## Features
+
+There are many API endpoints under Certificate Manager, and this library currently supports a subset of those endpoints.  The current list of written and tested endpoint classes includes:
+
+* Organization (/organization)
+* Person (/person)
+* SSL (/ssl)
+* Client Administrator (/admin)
+* Domain (/domain)
+* Report (/report)
+
+Other endpoints we hope to add in the near future:
+
+* Code Signing Certificates (/csod)
+* Custom Fields (/customField)
+* Domain Control Validation (/dcv)
+* Device Certificates (/device)
+* Discovery (/discovery)
+* SMIME (/smime)
+
+## Installing
+
+You can use pip to install cert_manager:
+
+```sh
+pip install cert_manager
+```
+
+## Examples
+
+This is a simple example that just shows initializing the `Client` object and using it to query the `Organization` and `SSL` endpoints:
+
+```python
+from cert_manager import Organization
+from cert_manager import Client
+from cert_manager import SSL
+
+client = Client(
+    base_url="https://cert-manager.com/api",
+    login_uri="SomeOrg",
+    username="your_username",
+    password="your_password",
+)
+
+org = Organization(client=client)
+ssl = SSL(client=client)
+
+print(ssl.types)
+print(org.all())
+```
+
+The most common process you would do, however, is enroll and then collect a certificate you want to order from the Certificate Manager:
+
+```python
+from time import sleep
+
+from cert_manager import Organization
+from cert_manager import Client
+from cert_manager import SSL
+
+client = Client(
+    base_url="https://cert-manager.com/api",
+    login_uri="SomeOrg",
+    username="your_username",
+    password="your_password",
+)
+
+# We need to enroll the certificate under an organization, so we will need to query the API for that
+org = Organization(client=client)
+# We need the SSL module to enroll the certificate
+ssl = SSL(client=client)
+
+cert_org = org.find(dept_name="MyDept")
+with open("host.csr", "r") as filep:
+    csr = filep.read()
+
+result = ssl.enroll(cert_type_name="InCommon SSL (SHA-2)", csr=csr, term=365, org_id=cert_org[0]["id"])
+
+# This is just for demonstration purposes.
+# Doing a wait loop like this to poll for the certificate is not the best way to go about this.
+while(True):
+    # Collect the certificate from Sectigo
+    try:
+        cert_pem = ssl.collect(cert_id=result["sslId"], cert_format="x509CO")
+        print(cert_pem)
+        break
+    except Pending:
+        print("Certificate is still pending...sleeping for 60s")
+        sleep(60)
+        continue
+    except Exception:
+        # For some unexpected exception, exit
+        break
+```
+
+## Contributing
+
+Pull requests to add functionality and fix bugs are always welcome.  Please check the CONTRIBUTING.md for specifics on contributions.
+
+### Testing
+
+We try to have a high level of test coverage on the code.  Therefore, when adding anything to the repo, tests should be written to test a new feature or to test a bug fix so that there won't be a regression.  This library is setup to be pretty simple to build a working development environment using [Docker][4].  Therefore, it is suggested that you have [Docker][4] installed where you clone this repository to make development easier.
+
+To start a development environment, you should be able to just run the `dev.sh` script.  This script will use the `Dockerfile` in this repository to build a [Docker][4] container with all the dependencies for development installed using [Pipenv][3].
+
+```sh
+./dev.sh
+```
+
+The first time you run the script, it should build the [Docker][4] image and then drop you into the container's shell.  The directory where you cloned this repository should be volume mounted in to `/usr/src`, which should also be the current working directory.  From there, you can make changes as you see fit.  Tests can be run from the `/usr/src` directory by simply typing `green` as [green][5] has been setup to with the correct parameters.
+
+## Changelog
+
+To generate the `CHANGELOG.md`, you will need [Docker][4] and a GitHub personal access token.  We currently use [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator) for this purpose.  The following should generate the file using information from GitHub:
+
+```sh
+docker run -it --rm \
+    -e CHANGELOG_GITHUB_TOKEN='yourtokenhere' \
+    -v "$(pwd)":/working \
+    -w /working \
+    ferrarimarco/github-changelog-generator --verbose
+```
+
+To generate the log for an upcoming release that has not yet been tagged, you can run a command to include the upcoming release version.  For example, `2.0.0`:
+
+```sh
+docker run -it --rm \
+    -e CHANGELOG_GITHUB_TOKEN='yourtokenhere' \
+    -v "$(pwd)":/working \
+    -w /working \
+    ferrarimarco/github-changelog-generator --verbose --future-release 2.0.0 --unreleased
+```
+
+As a note, this repository uses the default labels for formatting the `CHANGELOG.md`.  Label information can be found here: [Advanced-change-log-generation-examples](https://github.com/github-changelog-generator/github-changelog-generator/wiki/Advanced-change-log-generation-examples#section-options)
+
+## Releases
+
+Releases to the codebase are typically done using the [bump2version][6] tool.  This tool takes care of updating the version in all necessary files, updating its own configuration, and making a GitHub commit and tag.  We typically do version bumps as part of a PR, so you don't want to have [bump2version][6] tag the version at the same time it does the commit as commit hashes may change.  Therefore, to bump the version a patch level, one would run the command:
+
+```sh
+bump2version --verbose --no-tag patch
+```
+
+Once the PR is merged, you can then checkout the new `main` branch and tag it using the new version number that is now in `.bumpversion.cfg`:
+
+```sh
+git checkout main
+git pull --rebase
+git tag 1.0.0 -m 'Bump version: 0.1.0 → 1.0.0'
+git push --tags
+```
+
+[1]: https://www.python.org/ "Python"
+[2]: https://sectigo.com/ "Sectigo"
+[3]: https://pipenv.readthedocs.io/en/latest/ "Pipenv"
+[4]: https://www.docker.com/ "Docker"
+[5]: https://github.com/CleanCut/green "green"
+[6]: https://pypi.org/project/bump2version/ "bump2version"
 
-packages = \
-['cert_manager']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests', 'toml>=0.9,<0.11']
-
-setup_kwargs = {
-    'name': 'cert-manager',
-    'version': '2.3.0',
-    'description': 'Python interface to the Sectigo Certificate Manager REST API',
-    'long_description': '# python-cert_manager\n\nThis library provides a [Python][1] interface to the [Sectigo][2] Certificate Manager REST API.  python-cert_manager is open sourced under the [BSD 3-Clause license](LICENSE.txt).\n\n![checks](https://github.com/broadinstitute/python-cert_manager/workflows/checks/badge.svg?branch=main)\n[![codecov](https://codecov.io/gh/broadinstitute/python-cert_manager/branch/main/graph/badge.svg)](https://codecov.io/gh/broadinstitute/python-cert_manager)\n\n## Basics\n\n`cert_manager` runs on [Python][1] >= 3.7\n\n## Features\n\nThere are many API endpoints under Certificate Manager, and this library currently supports a subset of those endpoints.  The current list of written and tested endpoint classes includes:\n\n* Organization (/organization)\n* Person (/person)\n* SSL (/ssl)\n* Client Administrator (/admin)\n* Domain (/domain)\n* Report (/report)\n\nOther endpoints we hope to add in the near future:\n\n* Code Signing Certificates (/csod)\n* Custom Fields (/customField)\n* Domain Control Validation (/dcv)\n* Device Certificates (/device)\n* Discovery (/discovery)\n* SMIME (/smime)\n\n## Installing\n\nYou can use pip to install cert_manager:\n\n```sh\npip install cert_manager\n```\n\n## Examples\n\nThis is a simple example that just shows initializing the `Client` object and using it to query the `Organization` and `SSL` endpoints:\n\n```python\nfrom cert_manager import Organization\nfrom cert_manager import Client\nfrom cert_manager import SSL\n\nclient = Client(\n    base_url="https://cert-manager.com/api",\n    login_uri="SomeOrg",\n    username="your_username",\n    password="your_password",\n)\n\norg = Organization(client=client)\nssl = SSL(client=client)\n\nprint(ssl.types)\nprint(org.all())\n```\n\nThe most common process you would do, however, is enroll and then collect a certificate you want to order from the Certificate Manager:\n\n```python\nfrom time import sleep\n\nfrom cert_manager import Organization\nfrom cert_manager import Client\nfrom cert_manager import SSL\n\nclient = Client(\n    base_url="https://cert-manager.com/api",\n    login_uri="SomeOrg",\n    username="your_username",\n    password="your_password",\n)\n\n# We need to enroll the certificate under an organization, so we will need to query the API for that\norg = Organization(client=client)\n# We need the SSL module to enroll the certificate\nssl = SSL(client=client)\n\ncert_org = org.find(dept_name="MyDept")\nwith open("host.csr", "r") as filep:\n    csr = filep.read()\n\nresult = ssl.enroll(cert_type_name="InCommon SSL (SHA-2)", csr=csr, term=365, org_id=cert_org[0]["id"])\n\n# This is just for demonstration purposes.\n# Doing a wait loop like this to poll for the certificate is not the best way to go about this.\nwhile(True):\n    # Collect the certificate from Sectigo\n    try:\n        cert_pem = ssl.collect(cert_id=result["sslId"], cert_format="x509CO")\n        print(cert_pem)\n        break\n    except Pending:\n        print("Certificate is still pending...sleeping for 60s")\n        sleep(60)\n        continue\n    except Exception:\n        # For some unexpected exception, exit\n        break\n```\n\n## Contributing\n\nPull requests to add functionality and fix bugs are always welcome.  Please check the CONTRIBUTING.md for specifics on contributions.\n\n### Testing\n\nWe try to have a high level of test coverage on the code.  Therefore, when adding anything to the repo, tests should be written to test a new feature or to test a bug fix so that there won\'t be a regression.  This library is setup to be pretty simple to build a working development environment using [Docker][4].  Therefore, it is suggested that you have [Docker][4] installed where you clone this repository to make development easier.\n\nTo start a development environment, you should be able to just run the `dev.sh` script.  This script will use the `Dockerfile` in this repository to build a [Docker][4] container with all the dependencies for development installed using [Pipenv][3].\n\n```sh\n./dev.sh\n```\n\nThe first time you run the script, it should build the [Docker][4] image and then drop you into the container\'s shell.  The directory where you cloned this repository should be volume mounted in to `/usr/src`, which should also be the current working directory.  From there, you can make changes as you see fit.  Tests can be run from the `/usr/src` directory by simply typing `green` as [green][5] has been setup to with the correct parameters.\n\n## Changelog\n\nTo generate the `CHANGELOG.md`, you will need [Docker][4] and a GitHub personal access token.  We currently use [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator) for this purpose.  The following should generate the file using information from GitHub:\n\n```sh\ndocker run -it --rm \\\n    -e CHANGELOG_GITHUB_TOKEN=\'yourtokenhere\' \\\n    -v "$(pwd)":/working \\\n    -w /working \\\n    ferrarimarco/github-changelog-generator --verbose\n```\n\nTo generate the log for an upcoming release that has not yet been tagged, you can run a command to include the upcoming release version.  For example, `2.0.0`:\n\n```sh\ndocker run -it --rm \\\n    -e CHANGELOG_GITHUB_TOKEN=\'yourtokenhere\' \\\n    -v "$(pwd)":/working \\\n    -w /working \\\n    ferrarimarco/github-changelog-generator --verbose --future-release 2.0.0 --unreleased\n```\n\nAs a note, this repository uses the default labels for formatting the `CHANGELOG.md`.  Label information can be found here: [Advanced-change-log-generation-examples](https://github.com/github-changelog-generator/github-changelog-generator/wiki/Advanced-change-log-generation-examples#section-options)\n\n## Releases\n\nReleases to the codebase are typically done using the [bump2version][6] tool.  This tool takes care of updating the version in all necessary files, updating its own configuration, and making a GitHub commit and tag.  We typically do version bumps as part of a PR, so you don\'t want to have [bump2version][6] tag the version at the same time it does the commit as commit hashes may change.  Therefore, to bump the version a patch level, one would run the command:\n\n```sh\nbump2version --verbose --no-tag patch\n```\n\nOnce the PR is merged, you can then checkout the new `main` branch and tag it using the new version number that is now in `.bumpversion.cfg`:\n\n```sh\ngit checkout main\ngit pull --rebase\ngit tag 1.0.0 -m \'Bump version: 0.1.0 → 1.0.0\'\ngit push --tags\n```\n\n[1]: https://www.python.org/ "Python"\n[2]: https://sectigo.com/ "Sectigo"\n[3]: https://pipenv.readthedocs.io/en/latest/ "Pipenv"\n[4]: https://www.docker.com/ "Docker"\n[5]: https://github.com/CleanCut/green "green"\n[6]: https://pypi.org/project/bump2version/ "bump2version"\n',
-    'author': 'Andrew Teixeira',
-    'author_email': 'teixeira@broadinstitute.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/broadinstitute/python-cert_manager.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

