# Comparing `tmp/pythttp-0.1.1.tar.gz` & `tmp/pythttp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.1.tar", last modified: Sat Jun  3 23:41:43 2023, max compression
+gzip compressed data, was "pythttp-0.1.2.tar", last modified: Mon Jun  5 16:11:13 2023, max compression
```

## Comparing `pythttp-0.1.1.tar` & `pythttp-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.928562 pythttp-0.1.1/
--rw-rw-rw-   0        0        0     1093 2023-06-03 23:41:43.927586 pythttp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.1/README.md
--rw-rw-rw-   0        0        0      419 2023-06-03 23:41:39.000000 pythttp-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.911836 pythttp-0.1.1/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.1.1/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3391 2023-06-03 23:41:07.000000 pythttp-0.1.1/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    10102 2023-06-03 23:41:07.000000 pythttp-0.1.1/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     2936 2023-06-03 23:41:05.000000 pythttp-0.1.1/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:41:04.000000 pythttp-0.1.1/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-05-31 09:28:19.000000 pythttp-0.1.1/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.926610 pythttp-0.1.1/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 23:41:43.928562 pythttp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-03 23:41:36.000000 pythttp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.496167 pythttp-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-05 16:11:13.496167 pythttp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.2/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-05 16:10:10.000000 pythttp-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.483155 pythttp-0.1.2/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3501 2023-06-05 14:12:28.000000 pythttp-0.1.2/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    12967 2023-06-05 16:11:02.000000 pythttp-0.1.2/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     3182 2023-06-05 05:07:07.000000 pythttp-0.1.2/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.495166 pythttp-0.1.2/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:11:13.496167 pythttp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-05 16:10:31.000000 pythttp-0.1.2/setup.py
```

### Comparing `pythttp-0.1.1/PKG-INFO` & `pythttp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.1/README.md` & `pythttp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.1/pythttp/Log_Manager.py` & `pythttp-0.1.2/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.1/pythttp/Protocol.py` & `pythttp-0.1.2/pythttp/Protocol.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,22 +25,22 @@
             print(f'Request to server failed... Reason: {e}')
         finally:
             self.s.close()
 
     def BindAddress(self, address='0.0.0.0', port=80):
         external_ip = request.urlopen('https://ident.me').read().decode('utf8')  
         self.s.bind((address, port))
-        self.log(f"[Server started on] ==> \033[96m{external_ip}:{port}\033[0m")
+        self.log(f"[ Server started on ] ==> \033[96m{external_ip}:{port}\033[0m")
 
     def listen(self, limit=0):
         self.s.listen(limit)
 
     def AcceptConnection(self):
         self.c, self.addr = self.s.accept()
-        self.log(msg=f"[Connected with] ==> \033[32m{self.addr}\033[0m")
+        self.log(msg=f"[ Connected with ] ==> \033[32m{self.addr}\033[0m")
         return self.c, self.addr
     
     def Receive(self, socket=None, address=None, max_recv_size=1):
         received_data = b''
         header_list = []
         sokt=self.c
         if socket is not None:
@@ -53,18 +53,18 @@
             max_buf_size = self.ExtractPostBodySize(header_list)
             buf_size = 2048
             while True:
                 post_body += socket[0].recv(buf_size)
                 if max_buf_size == len(post_body):
                     break
                 buf_size = buf_size * 2
-            return 'Body', post_body
-        self.log(msg=f"[{parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
-        return 'Header', header_list
-    
+            self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
+            return header_list , post_body
+        self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
+        return header_list
 
     def ExtractPostBodySize(self, header):
         content_length_header = next((header for header in header if 'Content-Length' in header), None)
         if content_length_header:
             content_length_str = ''.join(filter(str.isdigit, content_length_header))
             return int(content_length_str)
         return 0
@@ -73,13 +73,13 @@
         thread_name,thread = self.Thread.ThreadConstructor(target=self.Receive,args=socket_and_addres)
         self.Thread.USERS.append(socket_and_addres[1])
         self.Thread.USERS_COUNT+=1
         self.Thread.ThreadSessions[thread_name]=socket_and_addres[1]
         self.Thread.user_socket_dict[socket_and_addres[1]]=socket_and_addres[0]
         return thread_name,thread
 
-    def SendResponse(self,query,socket_and_addres):
+    def SendResponse(self,Response,socket_and_addres):
         addr = f'\033[31m{socket_and_addres[1]}\033[0m'
-        socket_and_addres[0][0].send(query)
+        socket_and_addres[0][0].send(Response)
         socket_and_addres[0][0].close()
-        self.log(msg=f'[Disconnected from] ==> {addr}')
+        self.log(msg=f'[ Disconnected from ] ==> {addr}')
         self.Thread.finished_users.append(socket_and_addres[1])
```

### Comparing `pythttp-0.1.1/pythttp/RequestHandler.py` & `pythttp-0.1.2/pythttp/RequestHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,127 @@
 from .Protocol import *
-from .Structure import StructDB
+from .Structure import *
+from .Log_Manager import Log
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 import secrets
 import base64
+import json
 import uuid
 import re
 
 
 class Handler:
     def __init__(self) -> None:
         self.http=HyperTextTransferProtocol()
         self.Thread=self.http.Thread
         self.ServerUsersDB=[]
+        self.Sessions = []
         self.ServerDB={}
+        self.log=Log().logging
+        self.HandleloadDB()
 
     def RunServer(self):
         self.http.BindAddress()
         self.http.listen()
         while True:
             user_info=self.http.AcceptConnection()
             self.Thread.ThreadConstructor(target=self.HandleRequestThread,args=user_info)[1].start()
     
     def HandleRequestThread(self, client_socket, client_address):
         socket_and_address = [(client_socket,), client_address]
         thread_name, thread = self.http.AssignUserThread(socket_and_address)
         thread.start()
         thread.join()
+        Request=thread.result
         first_line = thread.result[0]
-        if 'Header' == first_line:
-            query=self.HandleGETRequest(thread)
-        # elif 'Body' == first_line:
-        #     query=self.HandleTextFileRequest()
-            # file_name=thread.result[1][1].split('"')[3]
-            # self.ImgFileUpload(thread.result[1][4].encode(),f'{file_name}')
-            # query=self.HandleFileRequest(self.ServerDB['Img'][file_name])
-        elif 'Body' == first_line:
-            post_data=parse.unquote(thread.result[1])
-            if '&' in post_data:
-                UserInfo=post_data.split('&')
-                if len(UserInfo) == 3:
-                    query=self.Sign_Up_handler(UserInfo[0],UserInfo[1],UserInfo[2])
-                elif len(UserInfo) == 2:
-                    query=self.login_handler(UserInfo[0],UserInfo[1])
-
+        if 'GET' in first_line:
+            Response=self.HandleGETRequest(Request)
+        elif 'POST' in first_line[0]:
+            Response=self.HandlePOSTRequest(Request)
         else:
-            return 'This communication is not HTTP protocol'
-        self.http.SendResponse(query, socket_and_address)
+            raise Exception('This communication is not HTTP protocol')
+        self.http.SendResponse(Response, socket_and_address)
         self.Thread.find_stopped_thread()
         self.Thread.ThreadDestructor(thread_name, client_address)
 
-    def HandleGETRequest(self, thread):
-        result = parse.unquote(thread.result[1][0]).split(' ')[1].replace('\\','/')
+    def HandleGETRequest(self, Request):
+        result = parse.unquote(Request[0]).split(' ')[1].replace('\\','/')
         try:
             Response = self.HandleTextFileRequest()
             if '?print=' in result:
-                Response = self.HandleTextFileRequest(query=result.split('=')[1])
-            elif '.ico' in result:
-                Response=self.HandleFileRequest(result)
-            elif '.html' in result:
-                Response=self.HandleTextFileRequest(result)
+                Response = self.HandleTextFileRequest(msg=result.split('=')[1])
             elif '.png' in result:
                 Response= self.HandleFileRequest(f'{result}')
+            elif '.ico' in result:
+                Response=self.HandleFileRequest(result)
             elif '/upload_form' == result:
                 Response= self.HandleTextFileRequest('/upload_form.html')
-            elif '/signup_form' == result:
-                Response= self.HandleTextFileRequest('/signup_form.html')
-            elif '/login_form' == result:
-                Response= self.HandleTextFileRequest('/login_form.html')
+            elif not self.verifySessionCookie(Request)[0]:
+                if '/SignUp_form' == result:
+                    Response= self.HandleTextFileRequest('/SignUp_form.html')
+                elif '/Login_form' == result:
+                    Response= self.HandleTextFileRequest('/Login_form.html')
+            elif (self.verifySessionCookie(Request)[0] and '/Logout_form' == result):
+                Response= self.HandleTextFileRequest('/Logout_form.html')
+            elif '.html' in result:
+                Response=self.HandleTextFileRequest(result)
             return Response
         except FileNotFoundError:
             with open('resource/Hello world.html','r',encoding='UTF-8') as arg:
                 print(f'해당 resource{result}파일을 찾을수 없습니다.')
                 Error_Response=arg.read().format(msg=f'해당 resource{result}파일을 찾을수 없습니다.').encode('utf-8')
                 return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
-        
+
+    def HandlePOSTRequest(self,Request):
+        JsonData=parse.unquote(Request[1])
+        DictPostData=json.loads(JsonData)
+        Form=DictPostData['Form']
+        Response=self.HandleTextFileRequest()
+        try:
+            if Form == 'SignUp':
+                Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'])
+            elif Form == 'Login':
+                Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'])
+            elif Form == 'Logout':
+                SessionID=self.verifySessionCookie(Request[0])[1]
+                Response=self.Logout_Handler(SessionID)
+        except Exception as e:
+            Response=self.ErrorHandler(e)
+        return Response
+
+    def verifySessionCookie(self,RequestData:list):
+        for data in RequestData:
+            if ('Cookie' in data):
+                Values = data.split('SessionID=')[1]
+                for Session in self.Sessions:
+                    if Values==Session.SessionToken:
+                        return True, Values
+        return False, None
+
     def HandleFileRequest(self,img_file='/a.png'):
         with open(f'resource{img_file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
             return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
         
-    def HandleTextFileRequest(self,flie='/Hello world.html', query='아무튼 웹 서버임'):
+    def HandleTextFileRequest(self,flie='/Hello world.html'):
         with open(f'resource{flie}','r',encoding='UTF-8') as TextFile:
+            Response_file=TextFile.read().encode('UTF-8')
+        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+    
+    def HandleMultiFileRequest(self,title,headline,pagemsg,Cookie=None):
+        with open(f'resource/multipurpos_page.html','r',encoding='UTF-8') as TextFile:
             Text=TextFile.read()
-            try:
-                Response_file=self.addFormatToHTML(Text,self.ServerDB['Img'],'<img src="{val}" alt="{key}">\n\t').encode('UTF-8')
-            except KeyError:
-                Response_file=Text.format(msg=query,Format='').encode('UTF-8')
+            Response_file=Text.format(title=title,headline=headline,pagemsg=pagemsg).encode('UTF-8')
+        return PrepareHeader()._response_headers('200 OK',Response_file,Cookie=Cookie) + Response_file
+    
+    def ErrorHandler(self,Error_msg):
+        with open(f'resource/Error_Form.html','r',encoding='UTF-8') as TextFile:
+            Response_file=TextFile.read()
+            Response_file=Response_file.format(msg=Error_msg).encode('utf-8')
         return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
     
     def addFormatToHTML(self,HtmlText : str, FormatData : dict, style : str):
         Format=''
         for key,val in FormatData.items():
             Format+=f'{style.format(val=val,key=key)}'
         HtmlText=HtmlText.format(Format=Format)
@@ -98,39 +129,69 @@
     
     def ImgFileUpload(self,img_file,file_name):
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
             self.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             return file_name
 
-
-    def Sign_Up_handler(self,UserID,UserName,UserPw):
+    def SignUp_Handler(self,UserID,UserName,UserPw):
         UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         for DB in self.ServerUsersDB:
             if (UserUID == DB.UserUID):
-                return self.HandleTextFileRequest(query=f'User information error! Duplicate ID! : {UserID}')
+                return self.HandleMultiFileRequest('Error Page','Error!',f'User information error! Duplicate ID! : {UserID}')
         try:
-            AuthenticatedName,AuthenticatedPassword=Verify().VerifyCredentials(UserName.split('=')[1], UserPw.split('=')[1])
+            AuthenticatedName,AuthenticatedPassword=Verify().VerifyCredentials(UserName, UserPw)
         except Exception as e:
-            return self.HandleTextFileRequest(query=f'User information error! Invalid nickname or password : {UserName,UserPw}')
+            return self.ErrorHandler(Error_msg=f'{e} : {UserName,UserPw}')
         self.ServerUsersDB.append(StructDB(UserUID,AuthenticatedName,AuthenticatedPassword))
-        return self.HandleTextFileRequest(query=f'Thanks for signing up!\n\nWelcome!')
+        self.log(f"[ SignUp User ] ==> UUID : \033[96m{UserUID}\033[0m")
+        self.HandleSaveDB()
+        return self.HandleMultiFileRequest('SignUp Successful','SignUp Successful! \n User : {UserName}','Your registration has been successfully completed. You can start using our services.')
+
+    def Login_Handler(self, user_id, user_pw):
+        user_uid = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), user_id)
+        # Check if user is already logged in
+        if self.Sessions:
+            for session in self.Sessions:
+                if session.UserInfo['UserUID'] == user_uid:
+                    return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
+        # Check user credentials and create new session
+        for db in self.ServerUsersDB:
+            if user_uid == db.UserUID and user_pw == db.UserPw:
+                session_id = self.RegisterUserSession(7, {'UserUID': user_uid})
+                self.log(f"[New Session Constructed] ==> SessionID: \033[96m{session_id}\033[0m")
+                return self.HandleMultiFileRequest('Welcome', f'Welcome! User: {user_id}', f"Dear {user_id}, thank you for logging in. We're excited to have you on board!", Cookie=f'SessionID = {session_id}')        
+        return self.ErrorHandler(Error_msg=f'User ID or password does not exist: {user_id, user_pw}')
 
-    def login_handler(self,UserID,UserPw):
-        UserPw=UserPw.split('=')[1]
-        UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
-        for DB in self.ServerUsersDB:
-            if (UserUID == DB.UserUID and UserPw == DB.UserPw):
-                SessionID=SessionsManager().RegisterUserSession(7,UserInfo={'UserUID':UserUID})
-                with open(f'resource/Hello world.html','r',encoding='UTF-8') as TextFile:
-                    Text=TextFile.read()
-                    Response_file=Text.format(msg=f"Login complete!\n\nWelcome! User : {UserUID}").encode('UTF-8')
-                    return PrepareHeader()._response_headers('200 OK',Response_file,Cookie=f'SessionID = {SessionID}') + Response_file
-        return self.HandleTextFileRequest(query=f'User ID or password does not exist : {UserID,UserPw}')
+    
+    def Logout_Handler(self,SessionID):
+        for Session in self.Sessions:
+            if Session.SessionToken == SessionID:
+                self.Sessions.remove(Session)
+                self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{SessionID}\033[0m")
+                return self.HandleMultiFileRequest('Logout',f'Goodbye!',f'Thank you for using our services. We hope to see you again soon!')
+        return self.ErrorHandler(Error_msg=f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
+
+    def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
+        SessionInfo = Session(SessionValidityDays, UserInfo)
+        self.Sessions.append(SessionInfo)
+        return SessionInfo.SessionToken
 
+    def HandleSaveDB(self):
+        with open(f'resource/ServerUserDB.DB','wb') as DBfile:
+            pickle.dump(self.ServerUsersDB,DBfile)
+            self.log(f"[ Database Save Successful ] ==> \033[96mresource/ServerUserDB.DB\033[0m")
+
+    def HandleloadDB(self):
+        try:
+            with open(f'resource/ServerUserDB.DB','rb') as DBfile:
+                self.ServerUsersDB=pickle.load(DBfile)
+                self.log(f"[ Database Load Successful ] ==> \033[96mresource/ServerUserDB.DB\033[0m")
+        except FileNotFoundError:
+            pass
 
 @dataclass
 class Session:
     """
     Session class represents a data model for storing session information.
 
     Attributes:
@@ -178,23 +239,14 @@
         """
         Method executed after initialization.
         Generates the session token.
         
         """
         self.Token = secrets.token_hex(self.length)
 
-class SessionsManager:
-    def __init__(self) -> None:
-        self.Sessions = []
-
-    def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
-        SessionInfo = Session(SessionValidityDays, UserInfo)
-        self.Sessions.append(SessionInfo)
-        return SessionInfo.SessionToken
-
 class Verify:
 
     def __init__(self) -> None:
         pass
 
     def VerifyCredentials(self, UserID, UserPw):
         if not self._VerifyUserID(UserID):
```

### Comparing `pythttp-0.1.1/pythttp/Structure.py` & `pythttp-0.1.2/pythttp/Structure.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,24 @@
     def __post_init__(self):
         self.StructDBdict['UserUID'] = self.UserUID
         self.StructDBdict['UserName'] = self.UserName
         self.StructDBdict['UserPw'] = self.UserPw
         self.StructDBdict['UserEmail'] = self.UserEmail
         self.StructDBdict['UserUploadFiles'] = self.UserUploadFiles
 
-class DBManger:
-    
-    def PASS(self):
-        pass
-
-
+def ParseStringToDict(string):
+    result = {}
+    parts = string.split('&')
+    for part in parts:
+        key_value = part.split('=')
+        if len(key_value) == 2:
+            key = key_value[0].strip()
+            value = key_value[1].strip()
+            result[key] = value
+    return result
 
 class PrepareHeader:
     def __init__(self, user_agent='127.0.0.1', body=None):
         self.body = body
         self.status_code="HTTP/1.1 200 OK"
         self.string_header = self.status_code + '\r\n'
         self.default_header = {}
```

### Comparing `pythttp-0.1.1/pythttp/Thread_Manager.py` & `pythttp-0.1.2/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.1/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.2/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.1/setup.py` & `pythttp-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.1",
+    version="0.1.2",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

