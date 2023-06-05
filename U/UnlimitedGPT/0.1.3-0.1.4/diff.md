# Comparing `tmp/UnlimitedGPT-0.1.3.tar.gz` & `tmp/UnlimitedGPT-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.3.tar", last modified: Sat Jun  3 21:40:43 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.4.tar", last modified: Mon Jun  5 20:46:10 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.3.tar` & `UnlimitedGPT-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.087476 UnlimitedGPT-0.1.3/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    27442 2023-06-03 21:33:51.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.091475 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2379 2023-06-03 21:04:32.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.091475 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-03 21:39:00.000000 UnlimitedGPT-0.1.3/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.286138 UnlimitedGPT-0.1.4/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.278137 UnlimitedGPT-0.1.4/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    28040 2023-06-05 20:42:13.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2343 2023-06-05 20:09:14.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-05 20:46:10.286138 UnlimitedGPT-0.1.4/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-05 20:45:07.000000 UnlimitedGPT-0.1.4/setup.py
```

### Comparing `UnlimitedGPT-0.1.3/PKG-INFO` & `UnlimitedGPT-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.3
+Version: 0.1.4
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.3/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.4/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
                     raise ValueError('Please install Xvfb to start a virtual display by running `sudo apt install xvfb`')
                 raise e
 
         self.logger.debug('Initializing browser...')
         
         options = ChromeOptions()
         options.add_argument('--window-size=1024,768')
+        options.add_argument('--disable-popup-blocking')
         if self._proxy:
             options.add_argument(f'--proxy-server={self._proxy}')
         for arg in self._chrome_args:
             options.add_argument(arg)
         try:
             self.driver = ChatGPTDriver(options=options, headless=self._headless)
         except TypeError as e:
@@ -351,14 +352,74 @@
             'Copy code`', '`'
         ).rstrip("\n")
 
         self.logger.debug(f'Message sent')
 
         return ChatGPTResponse(content, self._conversation_id)
 
+    def regenerate_response(self, message_timeout: int = 240, click_timeout: int = 20) -> ChatGPTResponse:
+        """
+        Regenerate the response.
+
+        Returns:
+        ----------
+            response (ChatGPTResponse): The newly regenerated response data.
+            message_timeout (int, optional): Time to wait for the message to regenerate before timing out. Defaults to 240.
+            click_timeout (int, optional): Time to wait for the click to succeed before timing out. Defaults to 20.
+
+        Raises:
+        ----------
+            TimeoutException: If the message fails to send.
+            TimeoutException: If the click fails to succeed.
+            ValueError: If the response is invalid.
+            ValueError: If the response is not found.
+        """
+        self.logger.debug('Regenerating response...')
+
+        # Click "Regenerate response" button
+        regenerate_response_clicked = self.driver.safe_click(
+            CGPTV.regenerate_response, timeout = click_timeout
+        )
+        if not regenerate_response_clicked:
+            self.logger.debug('Could not click regenerate response button')
+            raise TimeoutException('Could not click regenerate response button')
+
+        # Get the response, same way as send_message without the part of sending the message
+        self.logger.debug('Waiting for completion...')
+        WebDriverWait(self.driver, message_timeout).until_not(
+            EC.presence_of_element_located(CGPTV.streaming)
+        )
+
+        self.logger.debug('Getting response...')
+        responses = self.driver.find_elements(*CGPTV.big_response)
+        if responses:
+            response = responses[-1]
+            if 'text-red' in response.get_attribute('class'):
+                self.logger.debug('Response is an error')
+                raise ValueError(response.text)
+        response = self.driver.find_elements(*CGPTV.small_response)
+        try:
+            response = response[-1]
+        except IndexError:
+            self.logger.debug('Response not found, resetting conversation...')
+            self.reset_conversation()
+            raise ValueError('Response not found')
+
+        content = markdownify(
+            response.get_attribute('innerHTML'),
+            escape_asterisks=False,
+            escape_underscores=False,
+
+        ).replace(
+            'Copy code`', '`'
+        ).rstrip("\n")
+        
+        self.logger.debug('Regenerated response')
+        return ChatGPTResponse(content, self._conversation_id)
+
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
         """
         if not self.driver.current_url.startswith('https://chat.openai.com/'):
             return self.logger.debug('Current URL is not chat page, skipping reset')
 
@@ -467,28 +528,33 @@
             
             self.logger.debug('Theme switched')
             self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find theme buttons')
             return self._get_out_of_menu()
 
-    def switch_account(self, session_token: str):
+    def switch_account(self, session_token: str) -> SessionData:
         """
         Switch the account.
 
         Args:
         ----------
             session_token (str): The session token for authentication.
 
+        Returns:
+        ----------
+            SessionData: The new account's session data.
+
         Raises:
         ----------
             ValueError: If the session token is not provided.
             ValueError: If the response is invalid.
         """
         self.logger.debug('Switching account...')
+        self.conversation_id = '' # Old conversation ID cannot be loaded in the new account
         self.driver.execute_cdp_cmd(
             'Network.setCookie',
             {
                 'domain': 'chat.openai.com',
                 'path': '/',
                 'name': '__Secure-next-auth.session-token',
                 'value': session_token,
@@ -504,31 +570,38 @@
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
         response = loads(response)
         if (not response) or (
             'error' in response and response['error'] == 'RefreshAccessTokenError'
         ):
             raise ValueError('Invalid session token')
+        session_data = SessionData(
+            User(**response['user']),
+            response["expires"],
+            response["accessToken"],
+            response["authProvider"]
+        )
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Opening chat page...')
         self.driver.get(f'{CGPTV.chat_url}/{self._conversation_id}')
         self.logger.debug('Opened chat page')
         self._check_blocking_elements()
+        self.logger.debug('Switched account')
+        return session_data
     
     def get_session_data(self) -> SessionData:
         """
         Get the session data.
 
         Returns:
         ----------
-            SessionData: The ChatGPT session data.
+            SessionData: The current account's session data.
         """
         self.logger.debug('Getting account data...')
-        original_window = self.driver.current_window_handle
         self.logger.debug('Opening new tab...')
         self.driver.execute_script("window.open();")
         self.driver.switch_to.window(self.driver.window_handles[-1])
         self.driver.get('https://chat.openai.com/api/auth/session')
         response = self.driver.page_source
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
@@ -537,15 +610,15 @@
             User(**response['user']),
             response["expires"],
             response["accessToken"],
             response["authProvider"]
         )
         self.logger.debug('Closing tab...')
         self.driver.close()
-        self.driver.switch_to.window(original_window)
+        self.driver.switch_to.window(self.driver.window_handles[0])
         return session_data
 
     def logout(self) -> None:
         """
         Logs out of the current account signed into https://chat.openai.com
         """
         self.logger.debug('Logging out...')
@@ -611,69 +684,14 @@
             chat_history_toggle.click()
             self.logger.debug(f'Chat history is now {"enabled" if state else "disabled"}')
             self._get_out_of_menu()
         except:
             self.logger.debug(f'Could not {"enable" if state else "disable"} chat history')
             return self._get_out_of_menu()
     
-    def regenerate_response(self, message_timeout: int = 240, click_timeout: int = 20) -> ChatGPTResponse:
-        """
-        Regenerate the response.
-
-        Returns:
-        ----------
-            response (ChatGPTResponse): The newly regenerated response data.
-            message_timeout (int, optional): Time to wait for the message to regenerate before timing out. Defaults to 240.
-            click_timeout (int, optional): Time to wait for the click to succeed before timing out. Defaults to 20.
-
-        Raises:
-        ----------
-            TimeoutException: If the message fails to send.
-            TimeoutException: If the click fails to succeed.
-            ValueError: If the response is invalid.
-            ValueError: If the response is not found.
-        """
-        self.logger.debug('Regenerating response...')
-
-        # Click "Regenerate response" button
-        regenerate_response_clicked = self.driver.safe_click(
-            CGPTV.regenerate_response, timeout = click_timeout
-        )
-        if not regenerate_response_clicked:
-            self.logger.debug('Could not click regenerate response button')
-            raise TimeoutException('Could not click regenerate response button')
-
-        # Get the response, same way as send_message without the part of sending the message
-        self.logger.debug('Waiting for completion...')
-        WebDriverWait(self.driver, message_timeout).until_not(
-            EC.presence_of_element_located(CGPTV.streaming)
-        )
-
-        self.logger.debug('Getting response...')
-        responses = self.driver.find_elements(*CGPTV.big_response)
-        if responses:
-            response = responses[-1]
-            if 'text-red' in response.get_attribute('class'):
-                self.logger.debug('Response is an error')
-                raise ValueError(response.text)
-        response = self.driver.find_elements(*CGPTV.small_response)
-        try:
-            response = response[-1]
-        except IndexError:
-            self.logger.debug('Response not found, resetting conversation...')
-            self.reset_conversation()
-            raise ValueError('Response not found')
-
-        content = markdownify(response.get_attribute('innerHTML')).replace(
-            'Copy code`', '`'
-        )
-        
-        self.logger.debug('Regenerated response')
-        return ChatGPTResponse(content, self._conversation_id)
-
     def switch_conversation(self, conversation_id: str) -> None:
         """
         Switch the conversation.
 
         Args:
         ----------
             conversation_id (str): The conversation ID to switch to.
```

### Comparing `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     )
     small_response = (
         By.XPATH,
         '//div[starts-with(@class, "markdown prose w-full break-words")]',
     )
     textbox = (
         By.XPATH,
-        '/html/body/div[1]/div[2]/div[2]/div/main/div[2]/form/div/div/textarea'
+        '//textarea[@id="prompt-textarea"]'
     )
     regenerate_response = (
         By.XPATH,
-        "/html/body/div[1]/div[2]/div[2]/div/main/div[2]/form/div/div[1]/div/button"
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
     )
     new_chat = (
         By.LINK_TEXT,
         'New chat'
     )
 
     # Menu buttons
```

### Comparing `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.3
+Version: 0.1.4
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.3/setup.py` & `UnlimitedGPT-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
         'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.3",
+    version="0.1.4",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

