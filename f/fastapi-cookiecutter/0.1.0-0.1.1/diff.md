# Comparing `tmp/fastapi_cookiecutter-0.1.0-py3-none-any.whl.zip` & `tmp/fastapi_cookiecutter-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 77930 bytes, number of entries: 111
+Zip file size: 77902 bytes, number of entries: 111
 -rw-r--r--  2.0 unx      896 b- defN 80-Jan-01 00:00 cookiecutter.json
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fastapi_cookiecutter/__init__.py
 -rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 fastapi_cookiecutter/main.py
 -rw-r--r--  2.0 unx     1718 b- defN 80-Jan-01 00:00 hooks/post_gen_project.py
 -rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 hooks/pre_gen_project.py
 -rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.coveragerc
 -rw-r--r--  2.0 unx     2810 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.github/workflows/build.yml
@@ -100,14 +100,14 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/__init__.py
 -rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/errors.py
 -rw-r--r--  2.0 unx     5546 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/logging.py
 -rw-r--r--  2.0 unx     3383 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/storage.py
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/version.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/.keep
--rw-r--r--  2.0 unx      318 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    11236 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12836 b- defN 16-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/RECORD
-111 files, 161603 bytes uncompressed, 56098 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11182 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12836 b- defN 16-Jan-01 00:00 fastapi_cookiecutter-0.1.1.dist-info/RECORD
+111 files, 161547 bytes uncompressed, 56070 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -312,23 +312,23 @@
 
 Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/.keep
 Comment: 
 
 Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
 Comment: 
 
-Filename: fastapi_cookiecutter-0.1.0.dist-info/LICENSE
+Filename: fastapi_cookiecutter-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_cookiecutter-0.1.0.dist-info/METADATA
+Filename: fastapi_cookiecutter-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_cookiecutter-0.1.0.dist-info/WHEEL
+Filename: fastapi_cookiecutter-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_cookiecutter-0.1.0.dist-info/entry_points.txt
+Filename: fastapi_cookiecutter-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fastapi_cookiecutter-0.1.0.dist-info/RECORD
+Filename: fastapi_cookiecutter-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py

```diff
@@ -4,8 +4,8 @@
 from app import create_application
 from app.configs import get_settings
 
 app = create_application()
 settings = get_settings()
 
 if __name__ == "__main__":
-    uvicorn.run("main:app", host="0.0.0.0", port=8080, reload=False)  # nosec
+    uvicorn.run("main:app", host="0.0.0.0", port=80, reload=False)  # nosec
```

## Comparing `fastapi_cookiecutter-0.1.0.dist-info/LICENSE` & `fastapi_cookiecutter-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_cookiecutter-0.1.0.dist-info/METADATA` & `fastapi_cookiecutter-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cookiecutter
-Version: 0.1.0
+Version: 0.1.1
 Summary: This projects consist of a cookiecutter template that generates a full structure for a creating a PyPi standard package.
 Home-page: https://github.com/zhiwei2017/fastapi-cookiecutter
 License: MIT
 Keywords: cookiecutter template,python37,python38,python39,python310,python311,github-actions,gitlab-ci,bitbucket-pipelines,fastapi,RESTful API
 Author: Zhiwei Zhang
 Author-email: zhiwei2017@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -236,19 +236,14 @@
 To use it, please check the `example <the https://github.com/tiangolo/full-stack-fastapi-postgresql/blob/master/%7B%7Bcookiecutter.project_slug%7D%7D/backend/app/app/api/api_v1/endpoints/login.py>`_.
 
 Contributing Guide
 ------------------
 
 Please check the `Contributing Guide <docs/source/07_contributing.rst>`_ for details.
 
-Acknowledgements
-----------------
-
-Special thanks to
-
 Core Team
 ---------
 
 * `Zhiwei Zhang <https://github.com/zhiwei2017>`_ - *Author* / *Maintainer* - `zhiwei2017@gmail.com <mailto:zhiwei2017@gmail.com?subject=[GitHub]FastAPI%20Cookiecutter>`_
 
 Literature
 ----------
```

## Comparing `fastapi_cookiecutter-0.1.0.dist-info/RECORD` & `fastapi_cookiecutter-0.1.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -99,13 +99,13 @@
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/errors.py,sha256=jHsHDo7_4_n7iBW7Q3BSjfSSn2FEAnjXS75S7Sdr-cs,42
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/logging.py,sha256=djHicChNqyZmsh5kXXwyob5hy4oEs7wju3qcfltAzL0,5546
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/security.py,sha256=E_A3CysQbqaoOSUj0ezI4FwvNZnAw6bUnf4Y0JTHSNQ,3383
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/storage.py,sha256=0H64vJM_4tI3kZVv60gRWeRVoUCR1CT6_2Sk_EJCXz4,1614
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/version.py,sha256=B2YH5ZW_O7hvug3_D9lOrpHwX-rEyrnZgCiU4Upe5LA,85
 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/.keep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py,sha256=_vSqAYugxOIrqiRp8erfhZSJzR9Lc0Eq6TJHo0LDtfI,318
-fastapi_cookiecutter-0.1.0.dist-info/LICENSE,sha256=XCNqPd4ciui0Mh_LoM3e93BbNdpYOKJOlP7Mft5-ufI,1069
-fastapi_cookiecutter-0.1.0.dist-info/METADATA,sha256=OC41_hq7Cpme0tAGlz9zFYcK23x5HWM6QLIeeB1_cu0,11236
-fastapi_cookiecutter-0.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-fastapi_cookiecutter-0.1.0.dist-info/entry_points.txt,sha256=aHwY9NEZa3b9usE5kZVc7yDOM_mnavtwdNPzQBy5WII,71
-fastapi_cookiecutter-0.1.0.dist-info/RECORD,,
+{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py,sha256=WvpwpTHIzMM_NVSZZ6h3ZxHsIzxoWmTqNt01o5Z35hc,316
+fastapi_cookiecutter-0.1.1.dist-info/LICENSE,sha256=XCNqPd4ciui0Mh_LoM3e93BbNdpYOKJOlP7Mft5-ufI,1069
+fastapi_cookiecutter-0.1.1.dist-info/METADATA,sha256=Blt-NXknsFq4gNdetIpgtGwXrioaMFv26BAj4lorous,11182
+fastapi_cookiecutter-0.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fastapi_cookiecutter-0.1.1.dist-info/entry_points.txt,sha256=aHwY9NEZa3b9usE5kZVc7yDOM_mnavtwdNPzQBy5WII,71
+fastapi_cookiecutter-0.1.1.dist-info/RECORD,,
```

