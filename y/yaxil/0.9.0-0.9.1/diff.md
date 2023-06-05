# Comparing `tmp/yaxil-0.9.0-py2.py3-none-any.whl.zip` & `tmp/yaxil-0.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30116 bytes, number of entries: 19
--rw-r--r--  2.0 unx    45043 b- defN 23-Mar-09 14:39 yaxil/__init__.py
--rw-r--r--  2.0 unx      232 b- defN 23-Mar-09 14:41 yaxil/__version__.py
--rw-r--r--  2.0 unx       84 b- defN 23-Mar-09 14:24 yaxil/assessments/__init__.py
--rw-r--r--  2.0 unx    22420 b- defN 23-Mar-09 14:24 yaxil/assessments/neuroinfo/__init__.py
--rw-r--r--  2.0 unx     7117 b- defN 23-Mar-09 14:24 yaxil/assessments/neuroinfo/legacy/__init__.py
--rw-r--r--  2.0 unx      524 b- defN 23-Mar-09 14:24 yaxil/assessments/neuroinfo/session/__init__.py
--rw-r--r--  2.0 unx    16280 b- defN 23-Mar-09 15:37 yaxil/bids/__init__.py
--rw-r--r--  2.0 unx     2805 b- defN 23-Mar-09 14:24 yaxil/commons/__init__.py
--rw-r--r--  2.0 unx     1656 b- defN 23-Mar-09 14:24 yaxil/dicom/__init__.py
--rw-r--r--  2.0 unx      625 b- defN 23-Mar-09 14:24 yaxil/exceptions/__init__.py
--rw-r--r--  2.0 unx      783 b- defN 23-Mar-09 14:24 yaxil/functools/__init__.py
--rw-r--r--  2.0 unx     1283 b- defN 23-Mar-09 14:24 yaxil/session/__init__.py
--rwxr-xr-x  2.0 unx     9426 b- defN 23-Mar-09 16:30 yaxil-0.9.0.data/scripts/ArcGet.py
--rwxr-xr-x  2.0 unx     4101 b- defN 23-Mar-09 16:30 yaxil-0.9.0.data/scripts/xnat_auth
--rw-r--r--  2.0 unx     1541 b- defN 23-Mar-09 16:30 yaxil-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Mar-09 16:30 yaxil-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-09 16:30 yaxil-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-09 16:30 yaxil-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1586 b- defN 23-Mar-09 16:30 yaxil-0.9.0.dist-info/RECORD
-19 files, 116009 bytes uncompressed, 27520 bytes compressed:  76.3%
+Zip file size: 30333 bytes, number of entries: 19
+-rw-r--r--  2.0 unx    46824 b- defN 23-Jun-05 18:53 yaxil/__init__.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-05 19:04 yaxil/__version__.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Feb-24 17:08 yaxil/assessments/__init__.py
+-rw-r--r--  2.0 unx    22420 b- defN 23-Feb-24 17:08 yaxil/assessments/neuroinfo/__init__.py
+-rw-r--r--  2.0 unx     7117 b- defN 23-Feb-24 17:08 yaxil/assessments/neuroinfo/legacy/__init__.py
+-rw-r--r--  2.0 unx      580 b- defN 23-Jun-05 18:46 yaxil/assessments/neuroinfo/session/__init__.py
+-rw-r--r--  2.0 unx    16280 b- defN 23-Jun-05 15:40 yaxil/bids/__init__.py
+-rw-r--r--  2.0 unx     2805 b- defN 23-Feb-24 17:08 yaxil/commons/__init__.py
+-rw-r--r--  2.0 unx     1656 b- defN 23-Feb-24 17:08 yaxil/dicom/__init__.py
+-rw-r--r--  2.0 unx      625 b- defN 23-Feb-24 17:08 yaxil/exceptions/__init__.py
+-rw-r--r--  2.0 unx      783 b- defN 23-Feb-24 17:08 yaxil/functools/__init__.py
+-rw-r--r--  2.0 unx     1358 b- defN 23-Jun-05 18:45 yaxil/session/__init__.py
+-rwxr-xr-x  2.0 unx     9426 b- defN 23-Jun-05 19:06 yaxil-0.9.1.data/scripts/ArcGet.py
+-rwxr-xr-x  2.0 unx     4101 b- defN 23-Jun-05 19:06 yaxil-0.9.1.data/scripts/xnat_auth
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-05 19:06 yaxil-0.9.1.dist-info/RECORD
+19 files, 117921 bytes uncompressed, 27737 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -30,29 +30,29 @@
 
 Filename: yaxil/functools/__init__.py
 Comment: 
 
 Filename: yaxil/session/__init__.py
 Comment: 
 
-Filename: yaxil-0.9.0.data/scripts/ArcGet.py
+Filename: yaxil-0.9.1.data/scripts/ArcGet.py
 Comment: 
 
-Filename: yaxil-0.9.0.data/scripts/xnat_auth
+Filename: yaxil-0.9.1.data/scripts/xnat_auth
 Comment: 
 
-Filename: yaxil-0.9.0.dist-info/LICENSE
+Filename: yaxil-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: yaxil-0.9.0.dist-info/METADATA
+Filename: yaxil-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: yaxil-0.9.0.dist-info/WHEEL
+Filename: yaxil-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: yaxil-0.9.0.dist-info/top_level.txt
+Filename: yaxil-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: yaxil-0.9.0.dist-info/RECORD
+Filename: yaxil-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yaxil/__init__.py

```diff
@@ -51,47 +51,93 @@
     def __init__(self, url, content):
         self.url = url
         self.content = content
 
 XnatAuth = col.namedtuple("XnatAuth", [
     "url",
     "username",
-    "password"
+    "password",
+    "cookie"
 ])
 '''
 Container to hold XNAT authentication information. Fields include the ``url``,
 ``username``, and ``password``.
 '''
 
 def test_auth(auth):
     '''
-    Validate auth object against XNAT
+    Validate credentials against XNAT
 
     Example:
         >>> import yaxil
         >>> auth = yaxil.auth('doctest')
         >>> yaxil.test_auth(auth)
         True
     '''
     baseurl = auth.url.rstrip('/')
     url = f'{baseurl}/data/projects'
-    r = requests.get(url, auth=basicauth(auth), params={ 'columns': 'ID' })
+    r = requests.get(
+        url,
+        auth=basicauth(auth),
+        params={
+            'columns': 'ID'
+        }
+    )
     if r.status_code == requests.codes.UNAUTHORIZED:
         return False
     return True
 
+def start_session(auth):
+    '''
+    Return auth object with populated authentication cookie (JSESSIONID)
+    '''
+    baseurl = auth.url.rstrip('/')
+    url = f'{baseurl}/data/JSESSION'
+    r = requests.get(
+        url,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
+    if r.status_code != requests.codes.ok:
+        raise SessionError(f'response not ok ({r.status_code}) from {r.url}')
+    return XnatAuth(
+        username=auth.username,
+        password=auth.password,
+        url=auth.url,
+        cookie={
+            'JSESSIONID': r.text
+        }
+    )
+
+def end_session(auth):
+    if not auth.cookie:
+        return
+    baseurl = auth.url.rstrip('/')
+    url = f'{baseurl}/data/JSESSION'
+    r = requests.delete(
+        url,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
+    if r.status_code != requests.codes.ok:
+        raise SessionError('response not ok ({0}) from {1}'.format(r.status_code, r.url))
+
+class SessionError(Exception):
+    pass
+
 def basicauth(auth):
     '''
     Create basic auth tuple for requests.
     '''
     if auth.username and auth.password:
         return (auth.username, auth.password)
     return None
 
-@contextmanager
 def session(auth):
     '''
     Create a session context to avoid passing `auth` to
     every function.
 
     Example:
         >>> import yaxil
@@ -102,16 +148,15 @@
         XNAT_E...
 
     :param auth: XNAT authentication
     :type auth: :mod:`yaxil.XnatAuth`
     :returns: YAXIL session object
     :rtype: :mod:`yaxil.session.Session`
     '''
-    sess = Session(auth)
-    yield sess
+    return Session(auth)
 
 def auth2(alias=None, host=None, username=None, password=None, cfg='~/.xnat_auth'):
     '''
     Create authentication object from an ``xnat_auth`` file, function arguments, 
     or environment variables (``XNAT_HOST``, ``XNAT_USER``, and ``XNAT_PASS``), 
     in that order
 
@@ -123,37 +168,49 @@
         >>> os.environ['XNAT_PASS'] = '*****'
         >>> yaxil.auth2()
         XnatAuth(url='https://xnat.example.com', username='username', password='*****')
     '''
     result = tuple()
     # First, look for authentication data in ~/.xnat_auth
     if alias:
-        logger.debug('returning authentication data from %s', cfg)
+        logger.debug(f'returning authentication data from {cfg}')
         return auth(alias)
     # Second, look for authentication data from --host, --user, --password function arguments
     authargs = (host, username)
     if any(authargs):
         if not all(authargs):
             raise AuthError('you must supply --host, --username and --password (or password prompt)')
         logger.debug('returning authentication data from command line')
         if not password:
             password = gp.getpass('Enter XNAT passphrase:')
-        return XnatAuth(url=host, username=username, password=password)
+        obj = XnatAuth(
+            url=host,
+            username=username,
+            password=password,
+            cookie=None
+        )
+        return start_session(obj)
     # Third, look for authentication data in environment variables
     host = os.environ.get('XNAT_HOST', None)
     username = os.environ.get('XNAT_USER', None)
     password = os.environ.get('XNAT_PASS', None)
     authargs = (host, username)
     if any(authargs):
         if not all(authargs):
             raise AuthError('you must set $XNAT_HOST, $XNAT_USER, and $XNAT_PASS (or password prompt)')
         logger.debug('returning authentication data from environment variables')
         if not password:
             password = gp.getpass('Enter XNAT passphrase:')
-        return XnatAuth(url=host, username=username, password=password)
+        obj = XnatAuth(
+            url=host,
+            username=username,
+            password=password,
+            cookie=None
+        )
+        return start_session(obj)
     raise AuthError('you must provide authentication data using xnat_auth, command line, or environment variables')
 
 def auth(alias=None, url=None, cfg="~/.xnat_auth"):
     '''
     Read connection details from an xnat_auth XML file
 
     Example:
@@ -206,19 +263,21 @@
     password = res.findall("password")
     if not password:
         password = gp.getpass('Enter XNAT passphrase:')
     elif len(password) > 1:
         raise AuthError("too many passwords for %s in %s" % (alias, cfg))
     else:
         password = password.pop().text
-    return XnatAuth(
+    obj = XnatAuth(
         url=url.pop().text,
         username=username.pop().text,
-        password=password
+        password=password,
+        cookie=None
     )
+    return start_session(obj)
 
 Subject = col.namedtuple('Subject', [
     'uri',
     'label',
     'id',
     'project'
 ])
@@ -260,16 +319,21 @@
         'columns': ','.join(columns)
     }
     if label:
         payload['label'] = label
     if project:
         payload['project'] = project
     # submit the request
-    r = requests.get(url, params=payload, auth=basicauth(auth),
-                     verify=CHECK_CERTIFICATE)
+    r = requests.get(
+        url,
+        params=payload,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
     # validate response
     if r.status_code != requests.codes.ok:
         raise AccessionError(f'response not ok ({r.status_code} {r.reason}) from {r.url}')
     try:
         results = r.json()
         __quick_validate(results)
     except ResultSetError as e:
@@ -350,15 +414,21 @@
         payload['project'] = subject.project
         payload['xnat:subjectassessordata/subject_id'] = subject.id
     if daterange:
         start = arrow.get(daterange[0]).format('MM/DD/YYYY')
         stop = arrow.get(daterange[1]).format('MM/DD/YYYY')
         payload['date'] = '{0}-{1}'.format(start, stop)
     # submit request
-    r = requests.get(url, params=payload, auth=basicauth(auth), verify=CHECK_CERTIFICATE)
+    r = requests.get(
+        url,
+        params=payload,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
     # validate response
     if r.status_code != requests.codes.ok:
         raise AccessionError(f'response not ok ({r.status_code} {r.reason}) from {r.url}')
     try:
         results = r.json()
         __quick_validate(results)
     except ResultSetError as e:
@@ -439,15 +509,21 @@
     # build the url
     url = "%s/data/experiments/%s/scans/%s/files?format=zip" % (auth.url.rstrip('/'),
             aid, ','.join([str(x) for x in scan_ids]))
     # issue the http request, with exponential backoff retry behavior
     backoff = 10
     for _ in range(attempts):
         logger.debug("issuing http request %s", url)
-        r = requests.get(url, stream=True, auth=basicauth(auth), verify=CHECK_CERTIFICATE)
+        r = requests.get(
+            url,
+            stream=True,
+            auth=basicauth(auth),
+            cookies=auth.cookie,
+            verify=CHECK_CERTIFICATE
+        )
         logger.debug("response headers %s", r.headers)
         if r.status_code == requests.codes.ok:
             break
         fuzz = random.randint(0, 10)
         logger.warning("download unsuccessful (%s), retrying in %s seconds", r.status_code,
             backoff + fuzz)
         time.sleep(backoff + fuzz)
@@ -616,15 +692,20 @@
     :rtype: dict
     '''
     if not aid:
         aid = accession(auth, label, project)
     # get scans for accession as a csv
     url = "%s/data/experiments/%s/scans?format=csv" % (auth.url.rstrip('/'), aid)
     logger.debug("issuing http request %s", url)
-    r = requests.get(url, auth=basicauth(auth), verify=CHECK_CERTIFICATE)
+    r = requests.get(
+        url,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
     if r.status_code != requests.codes.ok:
         raise ScanSearchError(f'response not ok ({r.status_code} {r.reason}) from {r.url}')
     if not r.content:
         raise ScanSearchError("response is empty from %s" % r.url)
     # read the result into a csv reader
     reader = csv.reader(io.StringIO(r.content.decode()))
     columns = next(reader)
@@ -917,15 +998,21 @@
     '''
     if not params:
         params = {}
     url = "%s/%s" % (auth.url.rstrip('/'), path.lstrip('/'))
     params["format"] = fmt
     logger.debug("issuing http request %s", url)
     logger.debug("query parameters %s", params)
-    r = requests.get(url, params=params, auth=basicauth(auth), verify=CHECK_CERTIFICATE)
+    r = requests.get(
+        url,
+        params=params,
+        auth=basicauth(auth),
+        cookies=auth.cookie,
+        verify=CHECK_CERTIFICATE
+    )
     if r.status_code != requests.codes.ok:
         raise RestApiError(f'response not ok ({r.status_code} {r.reason}) from {r.url}')
     if not r.content:
         raise RestApiError("response is empty from %s" % r.url)
     if autobox:
         return r.url,_autobox(r.text, fmt)
     else:
@@ -954,14 +1041,15 @@
         params['format'] = fmt
     logger.debug(f'GET {url}')
     logger.debug(f'query parameters {params}')
     r = requests.get(
         url,
         params=params,
         auth=basicauth(auth),
+        cookies=auth.cookie,
         verify=CHECK_CERTIFICATE
     )
     if r.status_code != requests.codes.ok:
         raise RestApiError(f'response not ok ({r.status_code} {r.reason}) from {r.url}')
     if not r.content:
         raise RestApiError(f'response is empty from {r.url}')
     if autobox:
@@ -1018,14 +1106,15 @@
     :rtype: bool
     '''
     url = '{0}/data/{1}/{2}'.format(auth.url.rstrip('/'), datatype, xnatid)
     logger.debug('issuing http request %s', url)
     r = requests.get(
         url,
         auth=basicauth(auth),
+        cookies=auth.cookie,
         verify=CHECK_CERTIFICATE
     )
     if r.status_code == requests.codes.ok:
         return True
     return False
 
 def has(auth, xsitype, project=None):
@@ -1122,15 +1211,16 @@
     baseurl = auth.url.rstrip('/')
     
     # create (post) new image assessor
     url = f'{baseurl}/data/experiments/{sid}/assessors'
     logger.debug(f'posting {assessment} to {url}')
     r = requests.post(
         url,
-        auth=(auth.username, auth.password),
+        auth=basicauth(auth),
+        cookies=auth.cookie,
         files={
             'file': open(assessment, 'rb')
         },
         allow_redirects=True,
         verify=CHECK_CERTIFICATE
     )
     if r.status_code == requests.codes.ok:
@@ -1142,15 +1232,16 @@
        raise StoreRESTError(f'assessment {assessment} failed to upload ({r.status_code})')
 
     # create (put) new image assessor resource folder
     url = f'{baseurl}/data/experiments/{sid}/assessors/{aid}/resources/{resource_name}'
     logger.debug('PUT %s', url)
     r = requests.put(
         url,
-        auth=(auth.username, auth.password),
+        auth=basicauth(auth),
+        cookies=auth.cookie,
         allow_redirects=True,
         verify=CHECK_CERTIFICATE
     )
     if r.status_code == requests.codes.ok:
         logger.debug(f'resource folder created {resource_name}')
     elif r.status_code == requests.codes.conflict:
         logger.debug(f'resource folder {resource_name} likely already exists')
@@ -1162,15 +1253,16 @@
       resource_dir = os.path.join(resources, resource)
       for f in os.listdir(resource_dir):
         fullfile = os.path.join(resource_dir, f)
         url = f'{baseurl}/data/experiments/{sid}/assessors/{aid}/resources/{resource_name}/files/{resource}/{f}'
         logger.debug('PUT %s', url)
         r = requests.put(
           url,
-          auth=(auth.username, auth.password),
+          auth=basicauth(auth),
+          cookies=auth.cookie,
           files={
             'file': open(fullfile, 'rb')
           },
           allow_redirects=True,
           verify=CHECK_CERTIFICATE
         )
         if r.status_code == requests.codes.ok:
```

## yaxil/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'yaxil'
 __description__ = 'Yet another XNAT interface libary'
 __url__ = 'https://github.com/harvard-nrg/yaxil'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## yaxil/assessments/neuroinfo/session/__init__.py

```diff
@@ -1,15 +1,22 @@
+import yaxil
 import yaxil.assessments.neuroinfo as neuroinfo
 
 class Session:
     def __init__(self, auth):
         self._auth = auth
+
     def boldqc(self, *args, **kwargs):
         return neuroinfo.boldqc(self._auth, *args, **kwargs)
+
     def anatqc(self, *args, **kwargs):
         return neuroinfo.anatqc(self._auth, *args, **kwargs)
+
     def t2qc(self, *args, **kwargs):
         return neuroinfo.t2qc(self._auth, *args, **kwargs)
+
     def __enter__(self):
         return self
+
     def __exit__(self, type, value, traceback):
+        yaxil.end_session(self._auth)
         return
```

## yaxil/session/__init__.py

```diff
@@ -1,14 +1,12 @@
 import yaxil
 
 class Session(object):
     def __init__(self, auth):
         self._auth = auth
-        self.url = auth.url
-        self.username = auth.username
 
     def accession(self, *args, **kwargs):
         return yaxil.accession(self._auth, *args, **kwargs)
 
     def subjects(self, *args, **kwargs):
         return yaxil.subjects(self._auth, *args, **kwargs)
 
@@ -32,12 +30,16 @@
 
     def has(self, *args, **kwargs):
         return yaxil.has(self._auth, *args, **kwargs)
 
     def storexar(self, *args, **kwargs):
         return yaxil.storexar(self._auth, *args, **kwargs)
 
+    def storerest(self, *args, **kwargs):
+        return yaxil.storerest(self._auth, *args, **kwargs)
+
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
+        yaxil.end_session(self._auth)
         return
```

## Comparing `yaxil-0.9.0.data/scripts/ArcGet.py` & `yaxil-0.9.1.data/scripts/ArcGet.py`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.0.data/scripts/xnat_auth` & `yaxil-0.9.1.data/scripts/xnat_auth`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.0.dist-info/LICENSE` & `yaxil-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yaxil-0.9.0.dist-info/RECORD` & `yaxil-0.9.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-yaxil/__init__.py,sha256=DXXIowptspA9LTHHhNUr3irUrSCYgjCW6kQ3YR1Ic5Q,45043
-yaxil/__version__.py,sha256=nQbzOrpqCn64lV90F3iGHGtN2BFK2Ysxf1WrqC1ob2g,232
+yaxil/__init__.py,sha256=vsE9OWmDAN--A_L1kI2ItSQtKsIUyALpmSv_RvVzJxE,46824
+yaxil/__version__.py,sha256=mjJkjqxMuvXchZ05gvTzXmCp26s1C3gjD5rQdUv6xCM,232
 yaxil/assessments/__init__.py,sha256=TpcTgZ9L8FnHvBOwkeK07BDBnoqqHLV1hVaVG9-yXg8,84
 yaxil/assessments/neuroinfo/__init__.py,sha256=HLA6BTTUeUWDau6k-_yJnM1rDlXHOyTI5cEbACpsGK8,22420
 yaxil/assessments/neuroinfo/legacy/__init__.py,sha256=k7kzdPUCcFDE7CWYzLQj6KkgokcZPiAwa0Pp62-V2fY,7117
-yaxil/assessments/neuroinfo/session/__init__.py,sha256=Gyf6NjK7mscVjbS3jv2Uo56DzvLo9kGZbzq6E3ueBe8,524
+yaxil/assessments/neuroinfo/session/__init__.py,sha256=eNjyJm-2ho-4YfcUDVEz6ZY6OCy3WeETX7hFK0cBK8E,580
 yaxil/bids/__init__.py,sha256=I4VUikLW9gLwfPmEpw4SXJDSa_riBX7IOPryykxOFF8,16280
 yaxil/commons/__init__.py,sha256=lCdwSNdIavfJi5Wux0mZ5Ay_HgKU-FnG-X6vZclDq24,2805
 yaxil/dicom/__init__.py,sha256=hsrcXBZDMBJDrDtaGuVG-T8Btb-EDBSAf5PJbs-qht0,1656
 yaxil/exceptions/__init__.py,sha256=1xNTBxyCkWGevMNBe1kbESSMD5gH06bOG_3XUMYcUHQ,625
 yaxil/functools/__init__.py,sha256=P5yiAU1yotWAFPTi0_rs9SpKTxj1EH9NeBjVMHG3lGs,783
-yaxil/session/__init__.py,sha256=MyqPGMw3c45A1WsVCrTeAt8cFUHuccyi834pE8Jf9hU,1283
-yaxil-0.9.0.data/scripts/ArcGet.py,sha256=rhYYN_-B4rEdVi8SiHkrRHkNtjZ1AksvtJjSRCI57ho,9426
-yaxil-0.9.0.data/scripts/xnat_auth,sha256=lLXqRKgio3SBv5WZAC-ZrqyWiCvbyzP2kbffQn-DFqI,4101
-yaxil-0.9.0.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
-yaxil-0.9.0.dist-info/METADATA,sha256=QlF4sZjdHQ9x3OdyOy5d3ll_bOB1DrIkP-4i-4bmu3U,387
-yaxil-0.9.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-yaxil-0.9.0.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
-yaxil-0.9.0.dist-info/RECORD,,
+yaxil/session/__init__.py,sha256=o7lK4Gv3oieGh4Mi6RiZCPEhfnfWtZh0PYGEM0aUKxE,1358
+yaxil-0.9.1.data/scripts/ArcGet.py,sha256=rhYYN_-B4rEdVi8SiHkrRHkNtjZ1AksvtJjSRCI57ho,9426
+yaxil-0.9.1.data/scripts/xnat_auth,sha256=lLXqRKgio3SBv5WZAC-ZrqyWiCvbyzP2kbffQn-DFqI,4101
+yaxil-0.9.1.dist-info/LICENSE,sha256=OeJg-nLVJUolsCpYxcm6T-P7HHtfoO7kwAC1IoZfjzA,1541
+yaxil-0.9.1.dist-info/METADATA,sha256=cUDGELh-lFHvzdno1utqdxxxiuhnuxVv7LKytUST8Ek,387
+yaxil-0.9.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+yaxil-0.9.1.dist-info/top_level.txt,sha256=fJsV0xAAilNjfeNRzE2uEHQF-aNZy0K0CH9F6qhCXbU,6
+yaxil-0.9.1.dist-info/RECORD,,
```

