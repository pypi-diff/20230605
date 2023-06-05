# Comparing `tmp/osais-1.0.46.tar.gz` & `tmp/osais-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-hsdvnndl\osais-1.0.46.tar", last modified: Fri May 19 11:37:26 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-d_3bmnv_\osais-1.0.47.tar", last modified: Mon Jun  5 21:05:21 2023, max compression
```

## Comparing `osais-1.0.46.tar` & `osais-1.0.47.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.466733 osais-1.0.46/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.46/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-19 11:37:26.466733 osais-1.0.46/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.46/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.461733 osais-1.0.46/osais/
--rw-rw-rw-   0        0        0     1041 2023-05-19 11:36:31.000000 osais-1.0.46/osais/__init__.py
--rw-rw-rw-   0        0        0    54875 2023-05-19 11:36:03.000000 osais-1.0.46/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.465737 osais-1.0.46/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 11:37:26.466733 osais-1.0.46/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-05-19 11:36:43.000000 osais-1.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.818984 osais-1.0.47/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.47/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-06-05 21:05:21.818984 osais-1.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.47/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.813985 osais-1.0.47/osais/
+-rw-rw-rw-   0        0        0     1041 2023-06-05 20:59:14.000000 osais-1.0.47/osais/__init__.py
+-rw-rw-rw-   0        0        0    55617 2023-06-05 20:59:01.000000 osais-1.0.47/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.817985 osais-1.0.47/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.47/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 21:05:21.819983 osais-1.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-06-05 20:59:29.000000 osais-1.0.47/setup.py
```

### Comparing `osais-1.0.46/LICENSE` & `osais-1.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.46/PKG-INFO` & `osais-1.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.46
+Version: 1.0.47
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.46/osais/__init__.py` & `osais-1.0.47/osais/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.46"
+__version__="1.0.47"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
```

### Comparing `osais-1.0.46/osais/osais.py` & `osais-1.0.47/osais/osais.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.46"
+__version__="1.0.47"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -456,15 +456,16 @@
 gVAIAuthToken=None              ## authToken into OSAIS for when working as virtual AI
 
 ## authenticate into OSAIS as a CLIENT (most likely DEMO CLIENT)
 gClientID=None                  ## ID of authenticated client into OSAIS 
 gClientAuthToken=None           ## the resulting Auth token as Client, after login
 
 ## Gateway
-gOriginGateway=None             ## location of the local gateway for this (local) AI
+gOriginGateway=None             ## location of the local gateway for this (local) AI, as http://{ip}:{port}
+gGatewayTunnel=None             ## tunnel for the gateway (to be used when inside a docker)
 
 ## AWS related
 gS3=None
 gS3Bucket=None
 gAWSSession=None
 
 ## IP and Ports
@@ -478,14 +479,15 @@
 gAProcessed=[]                  ## all token being sent to processing (never call twice for same)
 gIsScheduled=False              ## do we have a scheduled event running?
 
 ## run times
 gIsBusy=False                   ## True if AI busy processing
 gDefaultCost=1000               ## default cost value in ms (will get overriden fast, this value is no big deal)
 gaProcessTime=[]                ## Array of last x (10/20?) time spent for processed requests 
+gAverageCostInUSD=0             ## average cost value in USD
 
 ## processing specifics
 gArgsOSAIS=None                 ## the args passed to the AI which are specific to OSAIS for sending notifications
 
 ## when running as vAI
 gInputDir="./_input/"
 gOutputDir="./_output/"
@@ -598,14 +600,15 @@
     global gName
     global gVAIToken
     global gVAISecret
     global gAWSSession
     global gS3
     global gS3Bucket
     global gOriginOSAIS
+    global gGatewayTunnel
 
     AWSID=None
     AWSSecret=None
 
     ## read env from config file
     if _filename!=None:
         try:
@@ -632,14 +635,16 @@
                         gVAIToken = value
                     elif key == "VAI_SECRET":
                         gVAISecret = value
                     elif key == "AWS_ACCESS_KEY_ID":
                         AWSID = value
                     elif key == "AWS_ACCESS_KEY_SECRET":
                         AWSSecret = value
+                    elif key == "TUNNEL_GATEWAY":
+                        gGatewayTunnel = value
         except Exception as err: 
             consoleLog({"msg": f'No env file {_filename}'})
 
     # overload with env settings if any
     print(f'=> Setting env vars from ENV...')
     if os.environ.get('IS_DEBUG'):
         _isDebug=(os.environ.get('IS_DEBUG')=="True")
@@ -687,14 +692,17 @@
         print(f'=> Logged into AWS S3')
         
     if gIsDebug: 
         gOriginOSAIS="http://"+gIPLocal+":3022/"
     else:
         gOriginOSAIS="https://opensourceais.com/"
 
+    if os.environ.get('TUNNEL_GATEWAY') and gGatewayTunnel==None:
+        gGatewayTunnel=os.environ.get('TUNNEL_GATEWAY')
+
     return {
         "name": gName,
         "osais": gOriginOSAIS,
         "username": gUsername,
         "isLocal": gIsLocal,
         "isVirtualAI": gIsVirtualAI,
         "isDebug": gIsDebug
@@ -714,15 +722,15 @@
 # init the dafault cost array
 def _addCost(_cost) :
     global gaProcessTime
     gaProcessTime.insert(0, _cost)
     gaProcessTime.pop()
 
 # init the dafault cost array
-def _getAverageCost() :
+def _getAverageCostInMs() :
     global gaProcessTime
     average = sum(gaProcessTime) / len(gaProcessTime)
     return average
 
 ## ------------------------------------------------------------------------
 #       args processing
 ## ------------------------------------------------------------------------
@@ -790,14 +798,15 @@
     global gVersion
     global gIsDocker
     global gMachineName
     global gUsername
     global gIsBusy
     global gLastProcessStart_at
     global gLastChecked_at
+    global gAverageCostInUSD
 
     objConf=_getFullConfig(gName)
 
     return {
         "name": gName,
         "version": gVersion,
         "location": f'http://{objConf["ip"]}:{objConf["port"]}/',
@@ -806,15 +815,16 @@
         "isRunning": True,    
         "isDocker": gIsDocker,    
         "lastActive_at": gLastChecked_at,
         "lastProcessStart_at": gLastProcessStart_at,
         "machine": gMachineName,
         "owner": gUsername, 
         "isAvailable": (gIsBusy==False),
-        "averageResponseTime": _getAverageCost(), 
+        "averageResponseTime": _getAverageCostInMs(), 
+        "averageCost": gAverageCostInUSD,           ## todo
         "config_ai": objConf["config_ai"],
         "config_base": objConf["config_base"]
     }
 
 ## ------------------------------------------------------------------------
 #       connect to Gateway
 ## ------------------------------------------------------------------------
@@ -834,15 +844,15 @@
     try:
         response = requests.post(f"{gOriginGateway}api/v1/public/ai/config", headers=headers, data=json.dumps(objParam))
         objRes=response.json()["data"]
         if objRes is None:
             raise ValueError("CRITICAL: could not notify Gateway")
 
     except Exception as err:
-        consoleLog({"msg":"CRITICAL: could not notify Gateway"})
+        consoleLog({"msg":"could not notify Gateway"})
         raise err
     return True
 
 ## PUBLIC - Reset connection to local gateway
 def osais_resetGateway(_localGateway):
     global gOriginGateway
     gOriginGateway=_localGateway
@@ -1458,15 +1468,15 @@
 ## PUBLIC - resetting who this AI is talking to (OSAIS prod and dbg)
 def osais_resetOSAIS(_location):
     global gOriginOSAIS
     gOriginOSAIS=_location
     return True
 
 ## PUBLIC - Init the Virtual AI
-def osais_initializeAI(_envFile):
+def osais_initializeAI(_envFile, _envSecret):
     global gIsDocker
     global gIsDebug
     global gIsLocal
     global gIsVirtualAI
     global gUsername
     global gName
     global gPortAI
@@ -1475,34 +1485,40 @@
     global gPortLocalOSAIS
     global gIPLocal
     global gExtIP
     global gOriginGateway
     global gVAIAuthToken
     global gOriginOSAIS
     global gClientAuthToken
+    global gGatewayTunnel
 
     ## load env 
     obj=osais_getEnv(_envFile)
+    obj2=osais_getEnv(_envSecret)
     gIsLocal=obj["isLocal"]
     gIsVirtualAI=obj["isVirtualAI"]
     gUsername=obj["username"]
     gName=obj["name"]
 
     ## from env, load AI config
     gConfig=osais_loadConfig(gName)
     gPortAI = gConfig["port"]
     gVersion = gConfig["version"]
 
 
     ## make sure we have a config file
     _loadConfig(gName)
 
-    ## where is OSAIS for us then?
+    ## where is the Gateway for us? if in Docker, we can only call the gateway on its tunnel
     gOriginGateway=f"http://{gIPLocal}:{gPortGateway}/"         ## config for local gateway (local and not virtual)
+    if gIsDocker:
+        gOriginGateway=gGatewayTunnel
+
 
+    ## where is OSAIS for us?
     ## we set OSAIS location in all cases (even if in gateway) because this AI can generate it s own page for sending reqs (needs a client logged into OSAIS)
     if gIsDebug:
         osais_resetOSAIS(f"http://{gIPLocal}:{gPortLocalOSAIS}/")
     else:
         osais_resetOSAIS("https://opensourceais.com/")
     
     if gIsVirtualAI:
```

### Comparing `osais-1.0.46/osais.egg-info/PKG-INFO` & `osais-1.0.47/osais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.46
+Version: 1.0.47
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.46/setup.py` & `osais-1.0.47/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.46',
+    version='1.0.47',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
     packages=["osais"],
     package_data={'src': ['osais.json']},
     install_requires=[
+        'asyncio ==3.4.3',
         'requests >=2.25.1',
         "schedule ==1.1.0",
         "watchdog ==2.1.9",
         "Werkzeug ==2.2.2",
         "Jinja2 ==3.1.2",
         "boto3 ==1.26.130"
     ],
```

