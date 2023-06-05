# Comparing `tmp/splathash-0.1.2.tar.gz` & `tmp/splathash-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splathash-0.1.2.tar", last modified: Mon Jun  5 11:33:40 2023, max compression
+gzip compressed data, was "splathash-0.1.3.tar", last modified: Mon Jun  5 13:13:19 2023, max compression
```

## Comparing `splathash-0.1.2.tar` & `splathash-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.336229 splathash-0.1.2/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      177 2023-06-05 10:11:09.000000 splathash-0.1.2/AUTHORS.rst
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        2 2023-06-05 10:11:09.000000 splathash-0.1.2/LICENSE
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      103 2023-06-05 11:19:57.000000 splathash-0.1.2/MANIFEST.in
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     3725 2023-06-05 11:33:40.336229 splathash-0.1.2/PKG-INFO
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     2875 2023-06-05 11:19:37.000000 splathash-0.1.2/README.md
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      844 2023-06-05 11:33:40.336229 splathash-0.1.2/setup.cfg
--rwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)       38 2023-06-05 11:16:42.000000 splathash-0.1.2/setup.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.332229 splathash-0.1.2/splathash/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       22 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/__init__.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       25 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/admin.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      113 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/apps.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       25 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/models.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.332229 splathash-0.1.2/splathash/test_utils/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/__init__.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.336229 splathash-0.1.2/splathash/test_utils/test_app/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/test_app/__init__.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       70 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/test_app/admin.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       90 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/test_app/apps.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.336229 splathash-0.1.2/splathash/test_utils/test_app/migrations/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/test_app/migrations/__init__.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       58 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/test_utils/test_app/models.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      234 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/urls.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/splathash/views.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.332229 splathash-0.1.2/splathash.egg-info/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     3725 2023-06-05 11:33:40.000000 splathash-0.1.2/splathash.egg-info/PKG-INFO
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      718 2023-06-05 11:33:40.000000 splathash-0.1.2/splathash.egg-info/SOURCES.txt
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        1 2023-06-05 11:33:40.000000 splathash-0.1.2/splathash.egg-info/dependency_links.txt
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       12 2023-06-05 11:33:40.000000 splathash-0.1.2/splathash.egg-info/requires.txt
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       16 2023-06-05 11:33:40.000000 splathash-0.1.2/splathash.egg-info/top_level.txt
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.336229 splathash-0.1.2/tests/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/__init__.py
-drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 11:33:40.336229 splathash-0.1.2/tests/example/
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/example/__init__.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      837 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/example/urls.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     3029 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/settings.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      335 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/test_models.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      185 2023-06-05 10:18:53.000000 splathash-0.1.2/tests/urls.py
--rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      389 2023-06-05 10:11:09.000000 splathash-0.1.2/tests/wsgi.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.348358 splathash-0.1.3/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     2763 2023-06-05 12:49:24.000000 splathash-0.1.3/LICENSE
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      104 2023-06-05 12:49:57.000000 splathash-0.1.3/MANIFEST.in
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     3181 2023-06-05 13:13:19.348358 splathash-0.1.3/PKG-INFO
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     2312 2023-06-05 13:11:09.000000 splathash-0.1.3/README.rst
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      879 2023-06-05 13:13:19.348358 splathash-0.1.3/setup.cfg
+-rwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)       38 2023-06-05 12:50:15.000000 splathash-0.1.3/setup.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/splathash/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       22 2023-06-05 13:13:15.000000 splathash-0.1.3/splathash/__init__.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/admin.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       93 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/apps.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/models.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/splathash/test_utils/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/test_utils/__init__.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/splathash/test_utils/test_app/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/test_utils/test_app/__init__.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       36 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/test_utils/test_app/admin.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       90 2023-06-05 12:57:37.000000 splathash-0.1.3/splathash/test_utils/test_app/apps.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/splathash/test_utils/test_app/migrations/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/test_utils/test_app/migrations/__init__.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       28 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/test_utils/test_app/models.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      181 2023-06-05 12:55:52.000000 splathash-0.1.3/splathash/urls.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:20.000000 splathash-0.1.3/splathash/views.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/splathash.egg-info/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     3181 2023-06-05 13:13:19.000000 splathash-0.1.3/splathash.egg-info/PKG-INFO
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      707 2023-06-05 13:13:19.000000 splathash-0.1.3/splathash.egg-info/SOURCES.txt
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        1 2023-06-05 13:13:19.000000 splathash-0.1.3/splathash.egg-info/dependency_links.txt
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       12 2023-06-05 13:13:19.000000 splathash-0.1.3/splathash.egg-info/requires.txt
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)       16 2023-06-05 13:13:19.000000 splathash-0.1.3/splathash.egg-info/top_level.txt
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.344358 splathash-0.1.3/tests/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:25.000000 splathash-0.1.3/tests/__init__.py
+drwxrwxr-x   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 13:13:19.348358 splathash-0.1.3/tests/example/
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)        0 2023-06-05 12:48:25.000000 splathash-0.1.3/tests/example/__init__.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      831 2023-06-05 12:57:37.000000 splathash-0.1.3/tests/example/urls.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)     2872 2023-06-05 12:48:25.000000 splathash-0.1.3/tests/settings.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      257 2023-06-05 12:48:25.000000 splathash-0.1.3/tests/test_models.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      168 2023-06-05 12:57:37.000000 splathash-0.1.3/tests/urls.py
+-rw-rw-r--   0 snnbotchway  (1000) snnbotchway  (1000)      389 2023-06-05 12:48:25.000000 splathash-0.1.3/tests/wsgi.py
```

### Comparing `splathash-0.1.2/README.md` & `splathash-0.1.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,91 @@
-# Splathash
+Splathash
+=========
 
-[![PyPi-version]][PyPi]
+A Django USSD framework package.
 
-**A Django USSD framework package.**
-
-## Requirements
+Requirements
+------------
 
 - Python 3.8+
 - Django 4.2, 4.1, 4.0, 3.2
 
 We **highly recommend** and only officially support the latest patch release of
 each Python and Django series.
 
-## Installation
+Installation
+------------
 
 1. Install using `pip`...
 
-    ```bash
-    pip install splathash
-    ```
+    .. code-block:: bash
+
+        pip install splathash
+
+2. Add "splathash" to your INSTALLED_APPS setting like this:
 
-2. Add "splathash" to your INSTALLED_APPS setting like this::
+    .. code-block:: python
 
-    INSTALLED_APPS = [
-        ...,
-        "splathash",
-    ]
+        INSTALLED_APPS = [
+            ...,
+            "splathash",
+        ]
 
-3. Include the splathash URLconf in your project urls.py like this::
+3. Include the splathash URLconf in your project urls.py like this:
 
-    path("splathash/", include("splathash.urls")),
+    .. code-block::
+
+        path("splathash/", include("splathash.urls")),
 
 4. Run ``python manage.py migrate`` to apply migrations.
 
 5. Start the development server and visit http://127.0.0.1:8000/splathash/playground/
    to test your USSD endpoint (you'll need to login with a user in the admin panel first).
 
-## Contributing and development
+Contributing and development
+----------------------------
 
 1. To start contributing to **Splathash**, clone the repository's develop branch:
 
-    ```bash
-    git clone -b develop https://github.com/nalo-solutions/splathash
-    ```
+    .. code-block:: bash
+
+        git clone -b develop https://github.com/nalo-solutions/splathash
 
 2. Create a virtual env with all development dependencies.
 
-    ```bash
-    cd splathash
-    python3 -m venv venv
-    source venv/bin/activate
-    pip install -r requirements.txt
-    ```
+    .. code-block:: bash
+
+        cd splathash
+        python3 -m venv venv
+        source venv/bin/activate
+        pip install -r requirements.txt
 
 3. In the main project directory, you'll find the `splathash` folder, which serves as both the main package itself and a Django app within the `testproject` Django project. Additionally, the `testapp` is another Django app within the `testproject` setup.
 This project is designed to facilitate testing of the `splathash` package within a Django project. To run the development server, use the following command:
 
-    ```bash
-    python manage.py runserver
-    ```
+    .. code-block:: bash
+
+        python manage.py runserver
 
 4. Run the tests with:
 
-    ```bash
-    pytest
-    ```
+    .. code-block:: bash
+
+        pytest
 
-## Committing your code
+Committing your code
+--------------------
 
 Before committing please make sure you have installed the `pre-commit` hooks in your local git repository:
 
-```bash
-pre-commit install
-```
+.. code-block:: bash
 
-This will ensure that your code is cleaned before you commit it.
+    pre-commit install
 
-## Creating releases
-
-1. Make sure you have poetry installed:
+This will ensure that your code is cleaned before you commit it.
 
-    ```bash
-    pip install poetry
-    ```
-
-2. Update the version with a valid bump rule:
-
-    ```bash
-    poetry version <rule>
-    ```
-
-    The table below illustrates the effect of these rules with concrete examples.
-
-    | RULE       | BEFORE  | AFTER   |
-    | ---------- | ------- | ------- |
-    | major      | 1.3.0   | 2.0.0   |
-    | minor      | 2.1.4   | 2.2.0   |
-    | patch      | 4.1.1   | 4.1.2   |
-    | premajor   | 1.0.2   | 2.0.0a0 |
-    | preminor   | 1.0.2   | 1.1.0a0 |
-    | prepatch   | 1.0.2   | 1.0.3a0 |
-    | prerelease | 1.0.2   | 1.0.3a0 |
-    | prerelease | 1.0.3a0 | 1.0.3a1 |
-    | prerelease | 1.0.3b0 | 1.0.3b1 |
+Creating releases
+-----------------
 
-3. Create a release on the GitHub repository to trigger the release workflow.
+1. Update the version in setup.cfg and splathash/__init__.py.
 
-[pypi-version]: https://img.shields.io/pypi/v/splathash.svg
-[pypi]: https://img.shields.io/pypi/v/splathash.svg
+2. Merge new release into main to trigger the workflow.
```

### Comparing `splathash-0.1.2/splathash.egg-info/SOURCES.txt` & `splathash-0.1.3/splathash.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-AUTHORS.rst
 LICENSE
 MANIFEST.in
-README.md
+README.rst
 setup.cfg
 setup.py
 splathash/__init__.py
 splathash/admin.py
 splathash/apps.py
 splathash/models.py
 splathash/urls.py
```

### Comparing `splathash-0.1.2/tests/example/urls.py` & `splathash-0.1.3/tests/example/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.conf.urls import url, include
     2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
 """
-from django.conf.urls import url, include
 from django.contrib import admin
-
+from django.urls import include, path
 
 urlpatterns = [
-    url(r'^admin/', admin.site.urls),
-    url(r'', include('splathash.urls', namespace='splathash')),
+    path("admin/", admin.site.urls),
+    path("", include("splathash.urls", namespace="splathash")),
 ]
```

### Comparing `splathash-0.1.2/tests/settings.py` & `splathash-0.1.3/tests/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,106 +9,101 @@
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/1.9/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = "8(_=&2o)0&ba2fsl1o%ka5smaduheo$%rx*0p6=&i+x9bkqo&u"
+SECRET_KEY = "key"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
 # Application definition
 
 INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-
-    'splathash',
-    
-
-    # if your app has other dependencies that need to be added to the site
-    # they should be added here
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "splathash",
 ]
 
 MIDDLEWARE = [
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
 
-ROOT_URLCONF = 'tests.urls'
+ROOT_URLCONF = "tests.urls"
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [os.path.join(BASE_DIR, 'templates'), ],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [
+            os.path.join(BASE_DIR, "templates"),
+        ],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
             ],
         },
     },
 ]
 
-WSGI_APPLICATION = 'tests.wsgi.application'
+WSGI_APPLICATION = "tests.wsgi.application"
 
 # Database
 # https://docs.djangoproject.com/en/1.9/ref/settings/#databases
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": os.path.join(BASE_DIR, "db.sqlite3"),
     }
 }
 
 # Password validation
 # https://docs.djangoproject.com/en/1.9/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
-        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
+        "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator",
     },
     {
-        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
+        "NAME": "django.contrib.auth.password_validation.MinimumLengthValidator",
     },
     {
-        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
+        "NAME": "django.contrib.auth.password_validation.CommonPasswordValidator",
     },
     {
-        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
+        "NAME": "django.contrib.auth.password_validation.NumericPasswordValidator",
     },
 ]
 
 # Internationalization
 # https://docs.djangoproject.com/en/1.9/topics/i18n/
 
-LANGUAGE_CODE = 'en-us'
+LANGUAGE_CODE = "en-us"
 
-TIME_ZONE = 'UTC'
+TIME_ZONE = "UTC"
 
 USE_I18N = True
 
-USE_L10N = True
-
 USE_TZ = True
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/1.9/howto/static-files/
 
-STATIC_URL = '/static/'
+STATIC_URL = "/static/"
```

