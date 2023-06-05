# Comparing `tmp/django-auth-adfs-1.9.6.tar.gz` & `tmp/django-auth-adfs-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auth-adfs-1.9.6.tar", last modified: Fri May  6 13:12:45 2022, max compression
+gzip compressed data, was "django-auth-adfs-1.9.7.tar", last modified: Fri May 27 17:43:34 2022, max compression
```

## Comparing `django-auth-adfs-1.9.6.tar` & `django-auth-adfs-1.9.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1296 2022-05-06 13:12:38.083410 django-auth-adfs-1.9.6/LICENSE
--rw-r--r--   0        0        0     4026 2022-05-06 13:12:38.083410 django-auth-adfs-1.9.6/README.rst
--rw-r--r--   0        0        0      136 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/__init__.py
--rw-r--r--   0        0        0    13286 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/backend.py
--rw-r--r--   0        0        0    15424 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/config.py
--rw-r--r--   0        0        0      221 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/drf-urls.py
--rw-r--r--   0        0        0      355 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/drf_urls.py
--rw-r--r--   0        0        0      110 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/exceptions.py
--rw-r--r--   0        0        0     2249 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/middleware.py
--rw-r--r--   0        0        0     1656 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/rest_framework.py
--rw-r--r--   0        0        0      137 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/signals.py
--rw-r--r--   0        0        0      652 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/templates/django_auth_adfs/login_failed.html
--rw-r--r--   0        0        0      533 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/urls.py
--rw-r--r--   0        0        0     4100 2022-05-06 13:12:38.087410 django-auth-adfs-1.9.6/django_auth_adfs/views.py
--rw-r--r--   0        0        0     2063 2022-05-06 13:12:38.111410 django-auth-adfs-1.9.6/pyproject.toml
--rw-r--r--   0        0        0     5179 2022-05-06 13:12:45.066115 django-auth-adfs-1.9.6/setup.py
--rw-r--r--   0        0        0     5973 2022-05-06 13:12:45.066590 django-auth-adfs-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1296 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/LICENSE
+-rw-r--r--   0        0        0     4026 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/README.rst
+-rw-r--r--   0        0        0      136 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/__init__.py
+-rw-r--r--   0        0        0    13286 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/backend.py
+-rw-r--r--   0        0        0    15424 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/config.py
+-rw-r--r--   0        0        0      221 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/drf-urls.py
+-rw-r--r--   0        0        0      355 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/drf_urls.py
+-rw-r--r--   0        0        0      110 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/exceptions.py
+-rw-r--r--   0        0        0     2249 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/middleware.py
+-rw-r--r--   0        0        0     1656 2022-05-27 17:43:26.472853 django-auth-adfs-1.9.7/django_auth_adfs/rest_framework.py
+-rw-r--r--   0        0        0      137 2022-05-27 17:43:26.476853 django-auth-adfs-1.9.7/django_auth_adfs/signals.py
+-rw-r--r--   0        0        0      652 2022-05-27 17:43:26.476853 django-auth-adfs-1.9.7/django_auth_adfs/templates/django_auth_adfs/login_failed.html
+-rw-r--r--   0        0        0      533 2022-05-27 17:43:26.476853 django-auth-adfs-1.9.7/django_auth_adfs/urls.py
+-rw-r--r--   0        0        0     4100 2022-05-27 17:43:26.476853 django-auth-adfs-1.9.7/django_auth_adfs/views.py
+-rw-r--r--   0        0        0     2055 2022-05-27 17:43:26.500853 django-auth-adfs-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0     5181 2022-05-27 17:43:34.948127 django-auth-adfs-1.9.7/setup.py
+-rw-r--r--   0        0        0     5975 2022-05-27 17:43:34.948630 django-auth-adfs-1.9.7/PKG-INFO
```

### Comparing `django-auth-adfs-1.9.6/LICENSE` & `django-auth-adfs-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/README.rst` & `django-auth-adfs-1.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/backend.py` & `django-auth-adfs-1.9.7/django_auth_adfs/backend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -276,22 +276,22 @@
 class AdfsAuthCodeBackend(AdfsBaseBackend):
     """
     Authentication backend to allow authenticating users against a
     Microsoft ADFS server with an authorization code.
     """
 
     def authenticate(self, request=None, authorization_code=None, **kwargs):
-        # If loaded data is too old, reload it again
-        provider_config.load_config()
-
         # If there's no token or code, we pass control to the next authentication backend
         if authorization_code is None or authorization_code == '':
             logger.debug("django_auth_adfs authentication backend was called but no authorization code was received")
             return
 
+        # If loaded data is too old, reload it again
+        provider_config.load_config()
+
         adfs_response = self.exchange_auth_code(authorization_code, request)
         access_token = adfs_response["access_token"]
         user = self.process_access_token(access_token, adfs_response)
         return user
 
 
 class AdfsAccessTokenBackend(AdfsBaseBackend):
```

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/config.py` & `django-auth-adfs-1.9.7/django_auth_adfs/config.py`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/middleware.py` & `django-auth-adfs-1.9.7/django_auth_adfs/middleware.py`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/rest_framework.py` & `django-auth-adfs-1.9.7/django_auth_adfs/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/templates/django_auth_adfs/login_failed.html` & `django-auth-adfs-1.9.7/django_auth_adfs/templates/django_auth_adfs/login_failed.html`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/urls.py` & `django-auth-adfs-1.9.7/django_auth_adfs/urls.py`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/django_auth_adfs/views.py` & `django-auth-adfs-1.9.7/django_auth_adfs/views.py`

 * *Files identical despite different names*

### Comparing `django-auth-adfs-1.9.6/pyproject.toml` & `django-auth-adfs-1.9.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'django-auth-adfs'
-version = "1.9.6"  # Remember to also change __init__.py version
+version = "1.9.7"  # Remember to also change __init__.py version
 description = 'A Django authentication backend for Microsoft ADFS and AzureAD'
 authors = ['Joris Beckers <joris.beckers@gmail.com>']
 maintainers = ['Jonas Krüger Svensson <jonas-ks@hotmail.com>', 'Sondre Lillebø Gundersen <sondrelg@live.no>']
 license = 'BSD'
 homepage = 'https://github.com/snok/django-auth-adfs'
 repository = 'https://github.com/snok/django-auth-adfs'
 documentation = 'https://django-auth-adfs.readthedocs.io/en/latest'
@@ -39,15 +39,15 @@
 django = [
     { version = '^2.2 || ^3', python = '<=3.7' },
     { version = '^2.2 || ^3 || ^4', python = '>=3.8' },
 ]
 requests = '^1 || ^2'
 urllib3 = '^1.26.0'
 cryptography = '>=1.7,<39.0'
-PyJWT = "^1.3.0 || ^2.0"
+PyJWT = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 responses = '*'
 mock = '*'
 coverage = '*'
 djangorestframework = '*'
 django-filter = "^2.4.0"
```

### Comparing `django-auth-adfs-1.9.6/setup.py` & `django-auth-adfs-1.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['django_auth_adfs']
 
 package_data = \
 {'': ['*'], 'django_auth_adfs': ['templates/django_auth_adfs/*']}
 
 install_requires = \
-['PyJWT>=1.3.0,<3.0',
+['PyJWT>=2.4.0,<3.0.0',
  'cryptography>=1.7,<39.0',
  'requests>=1,<3',
  'urllib3>=1.26.0,<2.0.0']
 
 extras_require = \
 {':python_version <= "3.7"': ['django>=2.2,<4'],
  ':python_version >= "3.8"': ['django>=2.2,<5']}
 
 setup_kwargs = {
     'name': 'django-auth-adfs',
-    'version': '1.9.6',
+    'version': '1.9.7',
     'description': 'A Django authentication backend for Microsoft ADFS and AzureAD',
     'long_description': 'ADFS Authentication for Django\n==============================\n\n.. image:: https://readthedocs.org/projects/django-auth-adfs/badge/?version=latest\n    :target: http://django-auth-adfs.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n.. image:: https://img.shields.io/pypi/v/django-auth-adfs.svg\n    :target: https://pypi.python.org/pypi/django-auth-adfs\n.. image:: https://img.shields.io/pypi/pyversions/django-auth-adfs.svg\n    :target: https://pypi.python.org/pypi/django-auth-adfs#downloads\n.. image:: https://img.shields.io/pypi/djversions/django-auth-adfs.svg\n    :target: https://pypi.python.org/pypi/django-auth-adfs\n.. image:: https://codecov.io/github/snok/django-auth-adfs/coverage.svg?branch=master\n    :target: https://codecov.io/github/snok/django-auth-adfs?branch=master\n\nA Django authentication backend for Microsoft ADFS and Azure AD\n\n* Free software: BSD License\n* Homepage: https://github.com/snok/django-auth-adfs\n* Documentation: http://django-auth-adfs.readthedocs.io/\n\nFeatures\n--------\n\n* Integrates Django with Active Directory on Windows 2012 R2, 2016 or Azure AD in the cloud.\n* Provides seamless single sign on (SSO) for your Django project on intranet environments.\n* Auto creates users and adds them to Django groups based on info received from ADFS.\n* Django Rest Framework (DRF) integration: Authenticate against your API with an ADFS access token.\n\nInstallation\n------------\n\nPython package::\n\n    pip install django-auth-adfs\n\nIn your project\'s ``settings.py`` add these settings.\n\n.. code-block:: python\n\n    AUTHENTICATION_BACKENDS = (\n        ...\n        \'django_auth_adfs.backend.AdfsAuthCodeBackend\',\n        ...\n    )\n\n    INSTALLED_APPS = (\n        ...\n        # Needed for the ADFS redirect URI to function\n        \'django_auth_adfs\',\n        ...\n\n    # checkout the documentation for more settings\n    AUTH_ADFS = {\n        "SERVER": "adfs.yourcompany.com",\n        "CLIENT_ID": "your-configured-client-id",\n        "RELYING_PARTY_ID": "your-adfs-RPT-name",\n        # Make sure to read the documentation about the AUDIENCE setting\n        # when you configured the identifier as a URL!\n        "AUDIENCE": "microsoft:identityserver:your-RelyingPartyTrust-identifier",\n        "CA_BUNDLE": "/path/to/ca-bundle.pem",\n        "CLAIM_MAPPING": {"first_name": "given_name",\n                          "last_name": "family_name",\n                          "email": "email"},\n    }\n\n    # Configure django to redirect users to the right URL for login\n    LOGIN_URL = "django_auth_adfs:login"\n    LOGIN_REDIRECT_URL = "/"\n\n    ########################\n    # OPTIONAL SETTINGS\n    ########################\n\n    MIDDLEWARE = (\n        ...\n        # With this you can force a user to login without using\n        # the LoginRequiredMixin on every view class\n        #\n        # You can specify URLs for which login is not enforced by\n        # specifying them in the LOGIN_EXEMPT_URLS setting.\n        \'django_auth_adfs.middleware.LoginRequiredMiddleware\',\n    )\n\nIn your project\'s ``urls.py`` add these paths:\n\n.. code-block:: python\n\n    urlpatterns = [\n        ...\n        path(\'oauth2/\', include(\'django_auth_adfs.urls\')),\n    ]\n\nThis will add these paths to Django:\n\n* ``/oauth2/login`` where users are redirected to, to initiate the login with ADFS.\n* ``/oauth2/login_no_sso`` where users are redirected to, to initiate the login with ADFS but forcing a login screen.\n* ``/oauth2/callback`` where ADFS redirects back to after login. So make sure you set the redirect URI on ADFS to this.\n* ``/oauth2/logout`` which logs out the user from both Django and ADFS.\n\nYou can use them like this in your django templates:\n\n.. code-block:: html\n\n    <a href="{% url \'django_auth_adfs:logout\' %}">Logout</a>\n    <a href="{% url \'django_auth_adfs:login\' %}">Login</a>\n    <a href="{% url \'django_auth_adfs:login-no-sso\' %}">Login (no SSO)</a>\n\nContributing\n------------\nContributions to the code are more then welcome.\nFor more details have a look at the ``CONTRIBUTING.rst`` file.\n',
     'author': 'Joris Beckers',
     'author_email': 'joris.beckers@gmail.com',
     'maintainer': 'Jonas Krüger Svensson',
     'maintainer_email': 'jonas-ks@hotmail.com',
     'url': 'https://github.com/snok/django-auth-adfs',
```

### Comparing `django-auth-adfs-1.9.6/PKG-INFO` & `django-auth-adfs-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auth-adfs
-Version: 1.9.6
+Version: 1.9.7
 Summary: A Django authentication backend for Microsoft ADFS and AzureAD
 Home-page: https://github.com/snok/django-auth-adfs
 License: BSD
 Keywords: django,authentication,adfs,azure,ad,oauth2
 Author: Joris Beckers
 Author-email: joris.beckers@gmail.com
 Maintainer: Jonas Krüger Svensson
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyJWT (>=1.3.0,<3.0)
+Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: cryptography (>=1.7,<39.0)
 Requires-Dist: django (>=2.2,<4); python_version <= "3.7"
 Requires-Dist: django (>=2.2,<5); python_version >= "3.8"
 Requires-Dist: requests (>=1,<3)
 Requires-Dist: urllib3 (>=1.26.0,<2.0.0)
 Project-URL: Documentation, https://django-auth-adfs.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/snok/django-auth-adfs
```

