# Comparing `tmp/abusentry-0.2.1.tar.gz` & `tmp/abusentry-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\abusentry-0.2.1.tar", last modified: Sun Jun  4 22:55:47 2023, max compression
+gzip compressed data, was "dist\abusentry-0.2.3.tar", last modified: Sun Jun  4 22:57:53 2023, max compression
```

## Comparing `abusentry-0.2.1.tar` & `abusentry-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 22:55:47.000000 abusentry-0.2.1/
--rw-rw-rw-   0        0        0     3406 2023-06-04 22:55:47.000000 abusentry-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4144 2023-06-04 15:16:27.000000 abusentry-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry/
--rw-rw-rw-   0        0        0      675 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/__init__.py
--rw-rw-rw-   0        0        0      732 2023-06-04 15:16:44.000000 abusentry-0.2.1/abusentry/__version__.py
--rw-rw-rw-   0        0        0     5701 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/abusentry.py
--rw-rw-rw-   0        0        0     7280 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/decode.py
--rw-rw-rw-   0        0        0     4717 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/digs.py
--rw-rw-rw-   0        0        0     5806 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/dnscheck.py
--rw-rw-rw-   0        0        0     7217 2023-06-04 22:55:40.000000 abusentry-0.2.1/abusentry/ipcheck.py
--rw-rw-rw-   0        0        0     4992 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/mailer.py
--rw-rw-rw-   0        0        0     5099 2023-06-04 15:26:43.000000 abusentry-0.2.1/abusentry/malvera.py
--rw-rw-rw-   0        0        0     9645 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/sniper.py
--rw-rw-rw-   0        0        0      966 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/strip.py
--rw-rw-rw-   0        0        0     5538 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/unshorten.py
--rw-rw-rw-   0        0        0     3448 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/urlscan.py
-drwxrwxrwx   0        0        0        0 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry/utils/
--rw-rw-rw-   0        0        0     4876 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/__init__.py
--rw-rw-rw-   0        0        0     3160 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/config.py
--rw-rw-rw-   0        0        0     6752 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/utils/dns.py
--rw-rw-rw-   0        0        0     1170 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/env.py
--rw-rw-rw-   0        0        0      394 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/exceptions.py
--rw-rw-rw-   0        0        0     3999 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/fangs.py
--rw-rw-rw-   0        0        0     9550 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/utils/http.py
--rw-rw-rw-   0        0        0     2089 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/utils/ipaddr.py
--rw-rw-rw-   0        0        0     7855 2023-06-04 15:16:27.000000 abusentry-0.2.1/abusentry/virustotal.py
--rw-rw-rw-   0        0        0     9116 2023-06-04 22:46:14.000000 abusentry-0.2.1/abusentry/whobe.py
-drwxrwxrwx   0        0        0        0 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/
--rw-rw-rw-   0        0        0     3406 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      444 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      207 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 22:55:47.000000 abusentry-0.2.1/abusentry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 22:55:47.000000 abusentry-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2949 2023-06-04 22:53:42.000000 abusentry-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:57:53.000000 abusentry-0.2.3/
+-rw-rw-rw-   0        0        0     3406 2023-06-04 22:57:53.000000 abusentry-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4144 2023-06-04 15:16:27.000000 abusentry-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry/
+-rw-rw-rw-   0        0        0      675 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-06-04 15:16:44.000000 abusentry-0.2.3/abusentry/__version__.py
+-rw-rw-rw-   0        0        0     5701 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/abusentry.py
+-rw-rw-rw-   0        0        0     7280 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/decode.py
+-rw-rw-rw-   0        0        0     4717 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/digs.py
+-rw-rw-rw-   0        0        0     5806 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/dnscheck.py
+-rw-rw-rw-   0        0        0     7217 2023-06-04 22:55:40.000000 abusentry-0.2.3/abusentry/ipcheck.py
+-rw-rw-rw-   0        0        0     4992 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/mailer.py
+-rw-rw-rw-   0        0        0     5099 2023-06-04 15:26:43.000000 abusentry-0.2.3/abusentry/malvera.py
+-rw-rw-rw-   0        0        0     9645 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/sniper.py
+-rw-rw-rw-   0        0        0      966 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/strip.py
+-rw-rw-rw-   0        0        0     5538 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/unshorten.py
+-rw-rw-rw-   0        0        0     3448 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/urlscan.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry/utils/
+-rw-rw-rw-   0        0        0     4876 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/__init__.py
+-rw-rw-rw-   0        0        0     3160 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/config.py
+-rw-rw-rw-   0        0        0     6752 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/utils/dns.py
+-rw-rw-rw-   0        0        0     1170 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/env.py
+-rw-rw-rw-   0        0        0      394 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/exceptions.py
+-rw-rw-rw-   0        0        0     3999 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/fangs.py
+-rw-rw-rw-   0        0        0     9550 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/utils/http.py
+-rw-rw-rw-   0        0        0     2089 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/utils/ipaddr.py
+-rw-rw-rw-   0        0        0     7855 2023-06-04 15:16:27.000000 abusentry-0.2.3/abusentry/virustotal.py
+-rw-rw-rw-   0        0        0     9116 2023-06-04 22:46:14.000000 abusentry-0.2.3/abusentry/whobe.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/
+-rw-rw-rw-   0        0        0     3406 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      444 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      207 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 22:57:53.000000 abusentry-0.2.3/abusentry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 22:57:53.000000 abusentry-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2949 2023-06-04 22:56:56.000000 abusentry-0.2.3/setup.py
```

### Comparing `abusentry-0.2.1/PKG-INFO` & `abusentry-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abusentry
-Version: 0.2.1
+Version: 0.2.3
 Summary: A set of tools for security auditing websites and domains.
 Home-page: https://github.com/xransum/abusentry/
 Author: Kevin Haas
 Author-email: kevin.haas96@gmail.com
 License: GPLv3+
 Description: ## What is AbuSentry?
```

### Comparing `abusentry-0.2.1/README.md` & `abusentry-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/__init__.py` & `abusentry-0.2.3/abusentry/__init__.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/__version__.py` & `abusentry-0.2.3/abusentry/__version__.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/abusentry.py` & `abusentry-0.2.3/abusentry/abusentry.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/decode.py` & `abusentry-0.2.3/abusentry/decode.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/digs.py` & `abusentry-0.2.3/abusentry/digs.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/dnscheck.py` & `abusentry-0.2.3/abusentry/dnscheck.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/ipcheck.py` & `abusentry-0.2.3/abusentry/ipcheck.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/mailer.py` & `abusentry-0.2.3/abusentry/mailer.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/malvera.py` & `abusentry-0.2.3/abusentry/malvera.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/sniper.py` & `abusentry-0.2.3/abusentry/sniper.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/strip.py` & `abusentry-0.2.3/abusentry/strip.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/unshorten.py` & `abusentry-0.2.3/abusentry/unshorten.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/urlscan.py` & `abusentry-0.2.3/abusentry/urlscan.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/__init__.py` & `abusentry-0.2.3/abusentry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/config.py` & `abusentry-0.2.3/abusentry/utils/config.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/dns.py` & `abusentry-0.2.3/abusentry/utils/dns.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/env.py` & `abusentry-0.2.3/abusentry/utils/env.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/fangs.py` & `abusentry-0.2.3/abusentry/utils/fangs.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/http.py` & `abusentry-0.2.3/abusentry/utils/http.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/utils/ipaddr.py` & `abusentry-0.2.3/abusentry/utils/ipaddr.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/virustotal.py` & `abusentry-0.2.3/abusentry/virustotal.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry/whobe.py` & `abusentry-0.2.3/abusentry/whobe.py`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/abusentry.egg-info/PKG-INFO` & `abusentry-0.2.3/abusentry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abusentry
-Version: 0.2.1
+Version: 0.2.3
 Summary: A set of tools for security auditing websites and domains.
 Home-page: https://github.com/xransum/abusentry/
 Author: Kevin Haas
 Author-email: kevin.haas96@gmail.com
 License: GPLv3+
 Description: ## What is AbuSentry?
```

### Comparing `abusentry-0.2.1/abusentry.egg-info/SOURCES.txt` & `abusentry-0.2.3/abusentry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abusentry-0.2.1/setup.py` & `abusentry-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         
     return entries
 
 RELATIVE_PWD = os.path.dirname(os.path.realpath(__file__))
 
 setup(
     name='abusentry',
-    version='0.2.1',
+    version='0.2.3',
     author='Kevin Haas',
     author_email="kevin.haas96@gmail.com",
     license='GPLv3+',
     description='A set of tools for security auditing websites and domains.',
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url='https://github.com/xransum/abusentry/',
```

