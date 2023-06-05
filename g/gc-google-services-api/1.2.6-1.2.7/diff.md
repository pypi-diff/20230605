# Comparing `tmp/gc_google_services_api-1.2.6.tar.gz` & `tmp/gc_google_services_api-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc_google_services_api-1.2.6.tar", max compression
+gzip compressed data, was "gc_google_services_api-1.2.7.tar", max compression
```

## Comparing `gc_google_services_api-1.2.6.tar` & `gc_google_services_api-1.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35148 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/LICENSE
--rw-r--r--   0        0        0     4790 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/README.md
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/__init__.py
--rw-r--r--   0        0        0      799 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/__init__.py
--rw-r--r--   0        0        0     2114 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/test_auth.py
--rw-r--r--   0        0        0     1700 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/__init__.py
--rw-r--r--   0        0        0      921 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/test_bigquery.py
--rw-r--r--   0        0        0     3842 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/__init__.py
--rw-r--r--   0        0        0     7150 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/test_calendar.py
--rw-r--r--   0        0        0     1681 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/__init__.py
--rw-r--r--   0        0        0     2731 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/test_gmail.py
--rw-r--r--   0        0        0     1818 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__tests__/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__tests__/test_gsheet.py
--rw-r--r--   0        0        0        0 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/drive.py
--rw-r--r--   0        0        0     3243 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/workspace.py
--rw-r--r--   0        0        0      458 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/LICENSE
+-rw-r--r--   0        0        0     4789 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/auth/__tests__/__init__.py
+-rw-r--r--   0        0        0     2168 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/auth/__tests__/test_auth.py
+-rw-r--r--   0        0        0     1790 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/bigquery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/bigquery/__tests__/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/bigquery/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0     4192 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/calendar_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/calendar_api/__tests__/__init__.py
+-rw-r--r--   0        0        0     7927 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/calendar_api/__tests__/test_calendar.py
+-rw-r--r--   0        0        0     1711 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gmail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gmail/__tests__/__init__.py
+-rw-r--r--   0        0        0     2827 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gmail/__tests__/test_gmail.py
+-rw-r--r--   0        0        0     2085 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gsheet/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gsheet/__tests__/__init__.py
+-rw-r--r--   0        0        0     3635 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/gsheet/__tests__/test_gsheet.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/permissions/__init__.py
+-rw-r--r--   0        0        0     3281 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/permissions/drive.py
+-rw-r--r--   0        0        0     3506 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/gc_google_services_api/permissions/workspace.py
+-rw-r--r--   0        0        0      656 2023-06-05 12:07:43.709766 gc_google_services_api-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.7/PKG-INFO
```

### Comparing `gc_google_services_api-1.2.6/LICENSE` & `gc_google_services_api-1.2.7/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `gc_google_services_api-1.2.6/README.md` & `gc_google_services_api-1.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 make test
 ```
 
 # Publish new version
 When your Pull Request is approved and merged with master, then to can generate new version running the next command:
 
 ```bash
-make v=X.Y.Z release 
+make v=X.Y.Z release
 ```
 or you can execute
 ```bash
 poetry version X.Y.Z <-- (New version)
 git commit -am "Release vX.Y.Z"
 git tag vX.Y.Z
 git push --follow-tags
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/auth/__init__.py` & `gc_google_services_api-1.2.7/gc_google_services_api/auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import base64
 import json
 import os
 
 from google.oauth2 import service_account
 
-CREDENTIALS_BASE64 = os.environ.get('GOOGLE_SERVICE_ACCOUNT_CREDENTIALS', '')
+CREDENTIALS_BASE64 = os.environ.get("GOOGLE_SERVICE_ACCOUNT_CREDENTIALS", "")
 
 try:
     CREDENTIALS_CONTENT = json.loads(base64.b64decode(CREDENTIALS_BASE64))
 except json.JSONDecodeError as e:
-    print('[ERROR CREDENTIALS_CONTENT]: ', e)
-    CREDENTIALS_CONTENT = ''
+    print("[ERROR CREDENTIALS_CONTENT]: ", e)
+    CREDENTIALS_CONTENT = ""
 
 
 class Auth:
     def __init__(self, scopes, subject_email=None) -> None:
         self.scopes = scopes
         self.subject_email = subject_email
 
     def get_credentials(self):
         credentials = service_account.Credentials.from_service_account_info(
-            CREDENTIALS_CONTENT,
-            scopes=self.scopes)
+            CREDENTIALS_CONTENT, scopes=self.scopes
+        )
 
         if self.subject_email:
             credentials = credentials.with_subject(self.subject_email)
 
         return credentials
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/test_auth.py` & `gc_google_services_api-1.2.7/gc_google_services_api/auth/__tests__/test_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,53 @@
 
 from gc_google_services_api.auth import Auth
 
 
 class AuthTestSuite(unittest.TestCase):
     def _create_service_account_mock(self, service_account):
         from_service_account_info_mock = Mock()
-        from_service_account_info_mock.from_service_account_info.return_value = 'CREDENTIALS'  # noqa: E501
+        from_service_account_info_mock.from_service_account_info.return_value = (  # noqa: E501
+            "CREDENTIALS"
+        )
 
         service_account.Credentials = from_service_account_info_mock
 
         return service_account
 
     def _create_service_account_with_subject_mock(self, service_account):
         with_subject_mock = Mock()
-        with_subject_mock.with_subject.return_value = 'CREDENTIALS_WITH_SUBJECT'  # noqa: E501
+        with_subject_mock.with_subject.return_value = "CREDENTIALS_WITH_SUBJECT"  # noqa: E501
         from_service_account_info_mock = Mock()
-        from_service_account_info_mock.from_service_account_info.return_value = with_subject_mock  # noqa: E501
+        from_service_account_info_mock.from_service_account_info.return_value = (  # noqa: E501
+            with_subject_mock
+        )
 
         service_account.Credentials = from_service_account_info_mock
 
         return service_account
 
-    @patch('gc_google_services_api.auth.service_account')
+    @patch("gc_google_services_api.auth.service_account")
     # @patch.dict(os.environ, {'GOOGLE_SERVICE_ACCOUNT_CREDENTIALS': '213'})
     def test_auth_set_google_credentials_with_scopes(self, service_account):
         service_account = self._create_service_account_mock(service_account)
-        expected_result = 'CREDENTIALS'
-        scopes = ['scope1', 'scope2']
+        expected_result = "CREDENTIALS"
+        scopes = ["scope1", "scope2"]
         response = Auth(scopes).get_credentials()
 
         self.assertEqual(response, expected_result)
         service_account.Credentials.from_service_account_info.assert_called_once_with(  # noqa: E501
-            '',
-            scopes=scopes)
+            "", scopes=scopes
+        )
 
-    @patch('gc_google_services_api.auth.service_account')
+    @patch("gc_google_services_api.auth.service_account")
     # @patch.dict(os.environ, {'GOOGLE_SERVICE_ACCOUNT_CREDENTIALS': '213'})
     def test_auth_set_google_credentials_with_subject(self, service_account):
         service_account = self._create_service_account_with_subject_mock(
-            service_account)
+            service_account
+        )
 
-        expected_result = 'CREDENTIALS_WITH_SUBJECT'
-        scopes = ['scope1', 'scope2']
-        subject_email = 'subject@email.com'
+        expected_result = "CREDENTIALS_WITH_SUBJECT"
+        scopes = ["scope1", "scope2"]
+        subject_email = "subject@email.com"
         response = Auth(scopes, subject_email).get_credentials()
 
         self.assertEqual(response, expected_result)
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__init__.py` & `gc_google_services_api-1.2.7/gc_google_services_api/bigquery/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
-from google.cloud import bigquery
+
 from google.api_core.exceptions import NotFound
+from google.cloud import bigquery
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 def execute_query(query="", error_value=[]):
@@ -13,15 +14,15 @@
     """
     client = bigquery.Client()
     query_job = client.query(query)
 
     try:
         return query_job.result()
     except Exception as e:
-        print('[ERROR]: ', e)
+        print("[ERROR]: ", e)
         return error_value
 
 
 class BigQueryManager:
     def __init__(self, project_id, dataset_id):
         self.project_id = project_id
         self.dataset_id = dataset_id
@@ -29,21 +30,25 @@
         self.client = bigquery.Client(project=project_id)
 
     def create_table_if_not_exists(self, table_id, schema={}):
         def _parse_schemas():
             schema_fields = []
             for field_name, field_type in schema.items():
                 schema_fields.append(
-                    bigquery.SchemaField(field_name, field_type))
+                    bigquery.SchemaField(
+                        field_name,
+                        field_type,
+                    )
+                )
 
             return schema_fields
 
         try:
             self.client.get_table(
-                f"{self.project_id}.{self.dataset_id}.{table_id}"
+                f"{self.project_id}.{self.dataset_id}.{table_id}",
             )
         except NotFound:
             table_ref = self.client.dataset(self.dataset_id).table(table_id)
             table = bigquery.Table(table_ref, schema=_parse_schemas())
             self.client.create_table(table)
 
     def execute_query(self, query="", error_value=[]):
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/test_bigquery.py` & `gc_google_services_api-1.2.7/gc_google_services_api/bigquery/__tests__/test_bigquery.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,28 @@
 
 
 class TestSuite(unittest.TestCase):
     def _create_bigquery_mock():
         mock = Mock()
 
         bigquery_client_result_mock = Mock()
-        bigquery_client_result_mock.result.return_value = 'bigquery_query_result'  # noqa: E501
+        bigquery_client_result_mock.result.return_value = (
+            "bigquery_query_result"  # noqa: E501
+        )
 
         bigquery_client_mock = Mock()
         bigquery_client_mock.query.return_value = bigquery_client_result_mock
 
         mock.Client.return_value = bigquery_client_mock
 
         return mock
 
-    @patch('gc_google_services_api.bigquery.bigquery', new=_create_bigquery_mock())  # noqa: E501
-    def test_execute_query_method_should_returns_bigquery_results_method_when_query_return_successfully(self):  # noqa: E501
-        expected_result = 'bigquery_query_result'
+    @patch(
+        "gc_google_services_api.bigquery.bigquery", new=_create_bigquery_mock()
+    )  # noqa: E501
+    def test_execute_query_method_should_returns_bigquery_results_method_when_query_return_successfully(  # noqa: E501
+        self,
+    ):  # noqa: E501
+        expected_result = "bigquery_query_result"
         response = execute_query("BIGQUERY_QUERY")
 
         self.assertEqual(response, expected_result)
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__init__.py` & `gc_google_services_api-1.2.7/gc_google_services_api/calendar_api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,106 +5,121 @@
 
 from gc_google_services_api.auth import Auth
 
 DEFAULT_DATE_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S+01:00"
 DEFAULT_MIN_DATE_TIME_FORMAT = "%Y-%m-%dT00:00:00+01:00"
 DEFAULT_MAX_DATE_TIME_FORMAT = "%Y-%m-%dT23:59:59+01:00"
 SCOPES = [
-    'https://www.googleapis.com/auth/calendar.readonly',
-    'https://www.googleapis.com/auth/calendar.events'
+    "https://www.googleapis.com/auth/calendar.readonly",
+    "https://www.googleapis.com/auth/calendar.events",
 ]
 SCOPES_DIRECTORY = [
-    'https://www.googleapis.com/auth/admin.directory.resource.calendar'
-]
-AUTHENTICATION_EMAIL = os.getenv('AUTHENTICATION_EMAIL', '')
+    "https://www.googleapis.com/auth/admin.directory.resource.calendar"
+]  # noqa: E501
+AUTHENTICATION_EMAIL = os.getenv("AUTHENTICATION_EMAIL", "")
 
 
 class Calendar:
     def __init__(self, minDate=None, maxDate=None, filterByCreator=None):
         self.minDate = minDate
         self.maxDate = maxDate
         self.filterByCreator = filterByCreator
         self.resources = []
         self.calendars = []
         self.calendar_events = {}
 
         self._initialize_authentication()
 
     def _initialize_authentication(self):
-        self.credentials = Auth(
-            SCOPES,
-            AUTHENTICATION_EMAIL
-        ).get_credentials()
+        self.credentials = Auth(SCOPES, AUTHENTICATION_EMAIL).get_credentials()
         self.credentials_directory = Auth(
-            SCOPES_DIRECTORY,
-            AUTHENTICATION_EMAIL
+            SCOPES_DIRECTORY, AUTHENTICATION_EMAIL
         ).get_credentials()
 
         self.service_calendar = build(
-            'calendar',
-            'v3',
-            credentials=self.credentials)
+            "calendar",
+            "v3",
+            credentials=self.credentials,
+        )
         self.service_directory = build(
-            'admin',
-            'directory_v1',
-            credentials=self.credentials_directory)
+            "admin", "directory_v1", credentials=self.credentials_directory
+        )
 
     def get_all_resources(self):
-        result = self.service_directory.resources().calendars().list(
-            customer='my_customer'
-        ).execute()
+        result = (
+            self.service_directory.resources()
+            .calendars()
+            .list(customer="my_customer")
+            .execute()
+        )
 
-        return result['items']
+        return result["items"]
 
     def request_calendars(self, pageToken=None):
-        result = self.service_calendar.calendarList().list(
-            pageToken=pageToken,
-            showDeleted=False,
-            showHidden=True,
-        ).execute()
+        result = (
+            self.service_calendar.calendarList()
+            .list(
+                pageToken=pageToken,
+                showDeleted=False,
+                showHidden=True,
+            )
+            .execute()
+        )
 
-        self.calendars.extend(result['items'])
-        nextPageToken = result.get('nextPageToken', None)
+        self.calendars.extend(result["items"])
+        nextPageToken = result.get("nextPageToken", None)
         if nextPageToken:
             self.request_calendars(pageToken=nextPageToken)
 
     def request_calendar_events(self, calendar_id, pageToken=None):
-        result = self.service_calendar.events().list(
-            calendarId=calendar_id,
-            pageToken=pageToken,
-            showDeleted=False,
-            timeMin=self.minDate.strftime(
-                DEFAULT_MIN_DATE_TIME_FORMAT) if self.minDate else None
-        ).execute()
+        result = (
+            self.service_calendar.events()
+            .list(
+                calendarId=calendar_id,
+                pageToken=pageToken,
+                showDeleted=False,
+                timeMin=self.minDate.strftime(DEFAULT_MIN_DATE_TIME_FORMAT)
+                if self.minDate
+                else None,
+            )
+            .execute()
+        )
 
-        for event in result['items']:
-            if event['status'] != 'cancelled':
+        for event in result["items"]:
+            if event["status"] != "cancelled":
                 try:
-                    if self.filterByCreator and event['creator']['email'] == self.filterByCreator:  # noqa: E501
+                    if (
+                        self.filterByCreator
+                        and event["creator"]["email"] == self.filterByCreator
+                    ):  # noqa: E501
                         if self.maxDate:
                             event_enddate = datetime.strptime(
-                                event['end']['dateTime'],
-                                DEFAULT_DATE_TIME_FORMAT)
+                                event["end"]["dateTime"],
+                                DEFAULT_DATE_TIME_FORMAT,
+                            )
                             max_date = datetime.strptime(
                                 self.maxDate.strftime(
-                                    DEFAULT_MAX_DATE_TIME_FORMAT),
-                                DEFAULT_DATE_TIME_FORMAT)
+                                    DEFAULT_MAX_DATE_TIME_FORMAT
+                                ),  # noqa: E501
+                                DEFAULT_DATE_TIME_FORMAT,
+                            )
 
-                            if (event_enddate > max_date):
+                            if event_enddate > max_date:
                                 continue
 
                         if calendar_id not in self.calendar_events:
                             self.calendar_events[calendar_id] = []
 
                         self.calendar_events[calendar_id].append(event)
                 except KeyError:
                     print(event)
 
-        nextPageToken = result.get('nextPageToken', None)
+        nextPageToken = result.get("nextPageToken", None)
         if nextPageToken:
             self.request_calendar_events(calendar_id, pageToken=nextPageToken)
 
     def remove_event(self, calendar_id, event_id):
-        return self.service_calendar.events().delete(
-            calendarId=calendar_id,
-            eventId=event_id
-        ).execute()
+        return (
+            self.service_calendar.events()
+            .delete(calendarId=calendar_id, eventId=event_id)
+            .execute()
+        )
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/test_calendar.py` & `gc_google_services_api-1.2.7/gc_google_services_api/calendar_api/__tests__/test_calendar.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,187 +6,226 @@
 
 
 class TestSuite(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.start_date = datetime.today()
         self.end_date = datetime.today() + timedelta(days=1)
-        self.filterByCreator = 'test@test.com'
+        self.filterByCreator = "test@test.com"
 
     def _create_Auth_mock(self, Auth):
         auth_mock = Mock()
-        auth_mock.get_credentials.return_value = 'CREDENTIALS'
+        auth_mock.get_credentials.return_value = "CREDENTIALS"
 
         Auth.return_value = auth_mock
 
         return Auth
 
     def _create_build_mock(self, build, items_value=[], event_items=[]):
         # Directory mock
         service = Mock()
         resources = Mock()
         calendars = Mock()
         list = Mock()
 
-        list.execute.return_value = {'items': items_value}
+        list.execute.return_value = {"items": items_value}
         calendars.list.return_value = list
         resources.calendars.return_value = calendars
         service.resources.return_value = resources
         # End Directory mock
         # Calendar mock
         calendarList = Mock()
         calendarListMethod = Mock()
         events = Mock()
         events_list = Mock()
         delete = Mock()
-        delete.execute.return_value = 'DELETED'
-        events_list.execute.return_value = {'items': event_items}
+        delete.execute.return_value = "DELETED"
+        events_list.execute.return_value = {"items": event_items}
         events.list.return_value = events_list
         events.delete.return_value = delete
-        calendarListMethod.execute.return_value = {'items': items_value}
+        calendarListMethod.execute.return_value = {"items": items_value}
         calendarList.list.return_value = calendarListMethod
         service.calendarList.return_value = calendarList
         service.events.return_value = events
         # EndCalendar mock
 
         build.return_value = service
 
         return build
 
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_calendar_constructor_should_initialize_authentication(self, build, Auth):  # noqa: E501
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_calendar_constructor_should_initialize_authentication(
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         build = self._create_build_mock(build)
 
         Calendar(self.start_date, self.end_date, self.filterByCreator)
 
         Auth.assert_has_calls(
             [
-                call([
-                    'https://www.googleapis.com/auth/calendar.readonly',
-                    'https://www.googleapis.com/auth/calendar.events'
-                ], '')
+                call(
+                    [
+                        "https://www.googleapis.com/auth/calendar.readonly",
+                        "https://www.googleapis.com/auth/calendar.events",
+                    ],
+                    "",
+                )
             ],
             [
-                call([
-                    'https://www.googleapis.com/auth/admin.directory.resource.calendar',  # noqa: E501
-                ], '')
+                call(
+                    [
+                        "https://www.googleapis.com/auth/admin.directory.resource.calendar",  # noqa: E501
+                    ],
+                    "",
+                )
             ],
         )
 
         build.assert_has_calls(
-            [
-                call('calendar', 'v3', credentials='CREDENTIALS')
-            ],
-            [
-                call('admin', 'directory_v1', credentials='CREDENTIALS')
-            ]
+            [call("calendar", "v3", credentials="CREDENTIALS")],
+            [call("admin", "directory_v1", credentials="CREDENTIALS")],
         )
 
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_get_all_resources_should_return_items_response(self, build, Auth):  # noqa: E501
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_get_all_resources_should_return_items_response(
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         build = self._create_build_mock(build)
 
         calendar_instance = Calendar(
-            self.start_date, self.end_date, self.filterByCreator)
+            self.start_date, self.end_date, self.filterByCreator
+        )
         resources = calendar_instance.get_all_resources()
 
         self.assertEqual(resources, [])
 
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_request_calendars_should_save_all_calendars(self, build, Auth):  # noqa: E501
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_request_calendars_should_save_all_calendars(
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         build = self._create_build_mock(build, [1, 2])
 
         calendar_instance = Calendar(
-            self.start_date, self.end_date, self.filterByCreator)
+            self.start_date, self.end_date, self.filterByCreator
+        )
         calendar_instance.request_calendars()
 
         self.assertEqual(calendar_instance.calendars, [1, 2])
 
         build().calendarList().list.assert_called_once_with(
-            pageToken=None,
-            showDeleted=False,
-            showHidden=True)
+            pageToken=None, showDeleted=False, showHidden=True
+        )
 
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_request_calendar_events_should_request_events_with_correct_params(self, build, Auth):  # noqa: E501
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_request_calendar_events_should_request_events_with_correct_params(
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         build = self._create_build_mock(build, [1, 2])
 
         calendar_instance = Calendar(
-            self.start_date,
-            self.end_date,
-            self.filterByCreator)
-        calendar_instance.request_calendar_events('1')
+            self.start_date, self.end_date, self.filterByCreator
+        )
+        calendar_instance.request_calendar_events("1")
 
         self.assertEqual(calendar_instance.calendar_events, {})
 
         build().events().list.assert_called_once_with(
-            calendarId='1',
+            calendarId="1",
             pageToken=None,
             showDeleted=False,
-            timeMin=self.start_date.strftime("%Y-%m-%dT00:00:00+01:00"))
+            timeMin=self.start_date.strftime("%Y-%m-%dT00:00:00+01:00"),
+        )
 
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_request_calendar_events_should_filter_events_by_creator_and_dates(self, build, Auth):  # noqa: E501
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_request_calendar_events_should_filter_events_by_creator_and_dates(  # noqa: E501
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         events_fixtures = [
             {
-                'status': 'confirmed',
-                'creator': {'email': 'test@test.com'},
-                'end': {'dateTime': self.start_date.strftime("%Y-%m-%dT10:00:00+01:00")},  # noqa: E501
+                "status": "confirmed",
+                "creator": {"email": "test@test.com"},
+                "end": {
+                    "dateTime": self.start_date.strftime(
+                        "%Y-%m-%dT10:00:00+01:00"
+                    )  # noqa: E501
+                },  # noqa: E501
             },
             {
-                'status': 'confirmed',
-                'creator': {'email': 'test@test.com'},
-                'end': {'dateTime': self.end_date.strftime("2054-%m-%dT10:00:00+01:00")},  # noqa: E501
+                "status": "confirmed",
+                "creator": {"email": "test@test.com"},
+                "end": {
+                    "dateTime": self.end_date.strftime(
+                        "2054-%m-%dT10:00:00+01:00"
+                    )  # noqa: E501
+                },  # noqa: E501
             },
             {
-                'status': 'cancelled',
-                'creator': {'email': 'test@test.com'},
-                'end': {'dateTime': self.start_date.strftime("%Y-%m-%dT10:00:00+01:00")},  # noqa: E501
+                "status": "cancelled",
+                "creator": {"email": "test@test.com"},
+                "end": {
+                    "dateTime": self.start_date.strftime(
+                        "%Y-%m-%dT10:00:00+01:00"
+                    )  # noqa: E501
+                },  # noqa: E501
             },
             {
-                'status': 'confirmed',
-                'creator': {'email': 'other@test.com'},
-                'end': {'dateTime': self.start_date.strftime("%Y-%m-%dT10:00:00+01:00")},  # noqa: E501
+                "status": "confirmed",
+                "creator": {"email": "other@test.com"},
+                "end": {
+                    "dateTime": self.start_date.strftime(
+                        "%Y-%m-%dT10:00:00+01:00"
+                    )  # noqa: E501
+                },  # noqa: E501
             },
         ]
         build = self._create_build_mock(build, [1, 2], events_fixtures)
 
         calendar_instance = Calendar(
-            self.start_date,
-            self.end_date,
-            self.filterByCreator)
-        calendar_instance.request_calendar_events('1')
-
-        self.assertDictEqual(calendar_instance.calendar_events, {
-            '1': [{
-                'status': 'confirmed',
-                'creator': {'email': 'test@test.com'},
-                'end': {'dateTime': self.start_date.strftime("%Y-%m-%dT10:00:00+01:00")},  # noqa: E501
-            }]
-        })
-
-    @patch('gc_google_services_api.calendar_api.Auth')
-    @patch('gc_google_services_api.calendar_api.build')
-    def test_remove_event_should_call_api_with_correct_params(self, build, Auth):  # noqa: E501
+            self.start_date, self.end_date, self.filterByCreator
+        )
+        calendar_instance.request_calendar_events("1")
+
+        self.assertDictEqual(
+            calendar_instance.calendar_events,
+            {
+                "1": [
+                    {
+                        "status": "confirmed",
+                        "creator": {"email": "test@test.com"},
+                        "end": {
+                            "dateTime": self.start_date.strftime(
+                                "%Y-%m-%dT10:00:00+01:00"
+                            )
+                        },  # noqa: E501
+                    }
+                ]
+            },
+        )
+
+    @patch("gc_google_services_api.calendar_api.Auth")
+    @patch("gc_google_services_api.calendar_api.build")
+    def test_remove_event_should_call_api_with_correct_params(
+        self, build, Auth
+    ):  # noqa: E501
         Auth = self._create_Auth_mock(Auth)
         build = self._create_build_mock(build)
 
         calendar_instance = Calendar(
-            self.start_date,
-            self.end_date,
-            self.filterByCreator)
-        response = calendar_instance.remove_event('1', '2')
+            self.start_date, self.end_date, self.filterByCreator
+        )
+        response = calendar_instance.remove_event("1", "2")
 
-        self.assertEqual(response, 'DELETED')
+        self.assertEqual(response, "DELETED")
         build().events().delete.assert_called_once_with(
-            calendarId='1',
-            eventId='2')
+            calendarId="1",
+            eventId="2",
+        )
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/gmail/__init__.py` & `gc_google_services_api-1.2.7/gc_google_services_api/gmail/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,53 +6,55 @@
 from email.mime.text import MIMEText
 
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from gc_google_services_api.auth import Auth
 
-AUTHENTICATION_EMAIL = os.getenv('AUTHENTICATION_EMAIL', '')
+AUTHENTICATION_EMAIL = os.getenv("AUTHENTICATION_EMAIL", "")
 
 SCOPES = [
-    'https://www.googleapis.com/auth/gmail.send',
+    "https://www.googleapis.com/auth/gmail.send",
 ]
 
 
 class Gmail:
-    def __init__(self, subject_email, type='raw') -> None:
+    def __init__(self, subject_email, type="raw") -> None:
         self.message_type = type
         self.credentials = Auth(SCOPES, subject_email).get_credentials()
-        self.service = build('gmail', 'v1', credentials=self.credentials)
+        self.service = build("gmail", "v1", credentials=self.credentials)
 
     def send_email(self, email_message, email_subject, to=[]):
         def _create_message():
-            if self.message_type == 'raw':
+            if self.message_type == "raw":
                 message = EmailMessage()
 
                 message.set_content(email_message)
             else:
-                message = MIMEText(email_message, 'html')
+                message = MIMEText(email_message, "html")
 
-            message['to'] = to
-            message['from'] = AUTHENTICATION_EMAIL
-            message['subject'] = email_subject
+            message["to"] = to
+            message["from"] = AUTHENTICATION_EMAIL
+            message["subject"] = email_subject
 
             return message
 
         try:
             message = _create_message()
 
             # encoded message
-            encoded_message = base64.urlsafe_b64encode(message.as_bytes()) \
-                .decode()
-
-            create_message = {
-                'raw': encoded_message
-            }
-            send_message = (self.service.users().messages().send(
-                userId='me',
-                body=create_message).execute())
+            encoded_message = base64.urlsafe_b64encode(
+                message.as_bytes(),
+            ).decode()
+
+            create_message = {"raw": encoded_message}
+            send_message = (
+                self.service.users()
+                .messages()
+                .send(userId="me", body=create_message)
+                .execute()
+            )
         except HttpError as error:
-            print(f'An error occurred: {error}')
+            print(f"An error occurred: {error}")
             send_message = None
 
         return send_message
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/test_gmail.py` & `gc_google_services_api-1.2.7/gc_google_services_api/gmail/__tests__/test_gmail.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,64 +7,74 @@
 class TestSuite(unittest.TestCase):
     def _create_build_mock(self, build):
         build_service = Mock()
         users = Mock()
         messages = Mock()
         execute = Mock()
 
-        execute.execute.return_value = 'execute'
+        execute.execute.return_value = "execute"
 
         messages.send.return_value = execute
 
         users.messages.return_value = messages
 
         build_service.users.return_value = users
 
         build.return_value = build_service
 
         return build
 
     def _create_service_account_mock(self, service_account):
         with_subject_mock = Mock()
-        with_subject_mock.with_subject.return_value = 'CREDENTIALS_TEST'
-        service_account.Credentials.from_service_account_info.return_value = with_subject_mock  # noqa: E501
+        with_subject_mock.with_subject.return_value = "CREDENTIALS_TEST"
+        service_account.Credentials.from_service_account_info.return_value = (
+            with_subject_mock  # noqa: E501
+        )
 
         return service_account
 
-    @patch('gc_google_services_api.gmail.build')
-    @patch('gc_google_services_api.auth.service_account')
-    def test_gmail_call_auth_when_instance_is_created(self, service_account, build):  # noqa: E501
+    @patch("gc_google_services_api.gmail.build")
+    @patch("gc_google_services_api.auth.service_account")
+    def test_gmail_call_auth_when_instance_is_created(
+        self, service_account, build
+    ):  # noqa: E501
         self._create_build_mock(build)
         service_account = self._create_service_account_mock(service_account)
-        subject_email = 'TEST_SUBJECT_EMAIL'
+        subject_email = "TEST_SUBJECT_EMAIL"
 
         Gmail(subject_email)
 
         service_account.Credentials.from_service_account_info.assert_called_once_with(  # noqa: E501
-            '',
-            scopes=['https://www.googleapis.com/auth/gmail.send'])
+            "", scopes=["https://www.googleapis.com/auth/gmail.send"]
+        )
         build.assert_called_once_with(
-            'gmail', 'v1', credentials='CREDENTIALS_TEST')
+            "gmail",
+            "v1",
+            credentials="CREDENTIALS_TEST",
+        )
 
-    @patch('gc_google_services_api.gmail.build')
-    @patch('gc_google_services_api.auth.service_account')
-    def test_gmail_call_send_email_service_whith_all_content(self, service_account, build):  # noqa: E501
+    @patch("gc_google_services_api.gmail.build")
+    @patch("gc_google_services_api.auth.service_account")
+    def test_gmail_call_send_email_service_whith_all_content(
+        self, service_account, build
+    ):  # noqa: E501
         build = self._create_build_mock(build)
         service_account = self._create_service_account_mock(service_account)
-        subject_email = 'TEST_SUBJECT_EMAIL@test.com'
+        subject_email = "TEST_SUBJECT_EMAIL@test.com"
 
         response = Gmail(subject_email).send_email(
-            'test message',
-            'test@test.com',
-            'totest@test.com')
+            "test message", "test@test.com", "totest@test.com"
+        )
 
         service_account.Credentials.from_service_account_info.assert_called_once_with(  # noqa: E501
-            '',
-            scopes=['https://www.googleapis.com/auth/gmail.send'])
+            "", scopes=["https://www.googleapis.com/auth/gmail.send"]
+        )
 
         build().users().messages().send.assert_called_once_with(
-            userId='me',
-            body={'raw': 'Q29udGVudC1UeXBlOiB0ZXh0L3BsYWluOyBjaGFyc2V0PSJ1dGYtOCIKQ29udGVudC1UcmFuc2Zlci1FbmNvZGluZzogN2JpdApNSU1FLVZlcnNpb246IDEuMAp0bzogdG90ZXN0QHRlc3QuY29tCmZyb206CnN1YmplY3Q6IHRlc3RAdGVzdC5jb20KCnRlc3QgbWVzc2FnZQo='}  # noqa: E501
+            userId="me",
+            body={
+                "raw": "Q29udGVudC1UeXBlOiB0ZXh0L3BsYWluOyBjaGFyc2V0PSJ1dGYtOCIKQ29udGVudC1UcmFuc2Zlci1FbmNvZGluZzogN2JpdApNSU1FLVZlcnNpb246IDEuMAp0bzogdG90ZXN0QHRlc3QuY29tCmZyb206CnN1YmplY3Q6IHRlc3RAdGVzdC5jb20KCnRlc3QgbWVzc2FnZQo="  # noqa: E501
+            },
         )
         build().users().messages().send().execute.assert_called_once_with()
 
-        self.assertEqual(response, 'execute')
+        self.assertEqual(response, "execute")
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__init__.py` & `gc_google_services_api-1.2.7/gc_google_services_api/gsheet/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 import os
 from urllib.error import HTTPError
 
 from apiclient import discovery
 
 from gc_google_services_api.auth import Auth
 
-API_NAME = 'sheets'
-API_VERSION = 'v4'
-AUTHENTICATION_EMAIL = os.environ.get('AUTHENTICATION_EMAIL', '')
-SCOPES = [
-    'https://www.googleapis.com/auth/spreadsheets'
-]
+API_NAME = "sheets"
+API_VERSION = "v4"
+AUTHENTICATION_EMAIL = os.environ.get("AUTHENTICATION_EMAIL", "")
+SCOPES = ["https://www.googleapis.com/auth/spreadsheets"]
 
 
 class GSheet(object):
     def __init__(self, subject_email=None) -> None:
         self.credentials = Auth(SCOPES, subject_email).get_credentials()
         self.service = discovery.build(
-            API_NAME, API_VERSION, credentials=self.credentials)
+            API_NAME, API_VERSION, credentials=self.credentials
+        )
 
     def read_gsheet(self, sheet_name, spreadsheet_id, spreadsheet_range):
-        return self.service.spreadsheets().values().get(
-            spreadsheetId=spreadsheet_id,
-            range='{}!{}'.format(sheet_name, spreadsheet_range),
-        ).execute()
+        return (
+            self.service.spreadsheets()
+            .values()
+            .get(
+                spreadsheetId=spreadsheet_id,
+                range="{}!{}".format(sheet_name, spreadsheet_range),
+            )
+            .execute()
+        )
 
     def get_sheetnames(self, spreadsheet_id):
-        return self.service.spreadsheets().get(
-            spreadsheetId=spreadsheet_id,
-        ).execute()
+        return (
+            self.service.spreadsheets()
+            .get(
+                spreadsheetId=spreadsheet_id,
+            )
+            .execute()
+        )
 
     def create_spreadsheet(self, spreadsheet_body):
         try:
-            spreadsheet = self.service.spreadsheets().create(
-                body=spreadsheet_body,
-                fields='spreadsheetId') \
+            spreadsheet = (
+                self.service.spreadsheets()
+                .create(body=spreadsheet_body, fields="spreadsheetId")
                 .execute()
+            )
 
-            return spreadsheet.get('spreadsheetId')
+            return spreadsheet.get("spreadsheetId")
         except HTTPError as error:
             print(f"An error occurred: {error}")
 
             return error
 
     def write_in_spreadsheet(self, spreadsheet_id, range_name, body):
         try:
-            results = self.service.spreadsheets().values().append(
-                spreadsheetId=spreadsheet_id,
-                range=range_name,
-                valueInputOption="USER_ENTERED",
-                body=body).execute()
+            results = (
+                self.service.spreadsheets()
+                .values()
+                .append(
+                    spreadsheetId=spreadsheet_id,
+                    range=range_name,
+                    valueInputOption="USER_ENTERED",
+                    body=body,
+                )
+                .execute()
+            )
 
             return results
         except HTTPError as error:
             print(f"An error occurred: {error}")
 
             return error
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/permissions/drive.py` & `gc_google_services_api-1.2.7/gc_google_services_api/permissions/drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,104 @@
 import time
 
 from googleapiclient.discovery import build
 
 from gc_google_services_api.auth import Auth
 
 SCOPES = [
-    'https://www.googleapis.com/auth/spreadsheets',
-    'https://www.googleapis.com/auth/drive',
+    "https://www.googleapis.com/auth/spreadsheets",
+    "https://www.googleapis.com/auth/drive",
 ]
 EMPTY_ARRAY = []
 
 
 class Drive:
     """
-        Google API documentation:
-            - https://developers.google.com/drive/api/guides/manage-shareddrives  # noqa: E501
+    Google API documentation:
+        - https://developers.google.com/drive/api/guides/manage-shareddrives  # noqa: E501
     """
+
     def __init__(self, subject_email) -> None:
         self.credentials = Auth(SCOPES, subject_email).get_credentials()
-        self.service = build('drive', 'v3', credentials=self.credentials)
+        self.service = build("drive", "v3", credentials=self.credentials)
         self.shared_drives = []
 
     def _add_shared_drive(self, shared_drive):
         self.shared_drives.append(shared_drive)
 
     def store_drives(self, drives):
         for drive in drives:
-            if drive['name'].startswith('AC -'):
+            if drive["name"].startswith("AC -"):
                 self._add_shared_drive(drive)
 
     def get_permissions_from_file(self, file_id):
-        results = self.service.permissions().list(
-            fileId=file_id,
-            useDomainAdminAccess=True,
-            supportsAllDrives=True,
-            fields='permissions/id,permissions/displayName,permissions/role,permissions/emailAddress'  # noqa: E501
-        ).execute()
+        results = (
+            self.service.permissions()
+            .list(
+                fileId=file_id,
+                useDomainAdminAccess=True,
+                supportsAllDrives=True,
+                fields="permissions/id,permissions/displayName,permissions/role,permissions/emailAddress",  # noqa: E501
+            )
+            .execute()
+        )
 
-        return results.get('permissions', EMPTY_ARRAY)
+        return results.get("permissions", EMPTY_ARRAY)
 
     def get_shared_drives(self, next_page_token=None) -> None:
-        results = self.service.drives().list(
-            fields='nextPageToken, drives(id, name)',
-            q=None,
-            useDomainAdminAccess=True,
-            pageToken=next_page_token,
-            pageSize=100,
-        ).execute()
+        results = (
+            self.service.drives()
+            .list(
+                fields="nextPageToken, drives(id, name)",
+                q=None,
+                useDomainAdminAccess=True,
+                pageToken=next_page_token,
+                pageSize=100,
+            )
+            .execute()
+        )
 
-        drives = results.get('drives', EMPTY_ARRAY)
+        drives = results.get("drives", EMPTY_ARRAY)
         self.store_drives(drives)
 
-        next_page_token = results.get('nextPageToken', None)
+        next_page_token = results.get("nextPageToken", None)
         if next_page_token:
             print("Requesting shared drives ({})...".format(next_page_token))
             self.get_shared_drives(next_page_token)
 
     def find_email_in_permissions(self, email_to_delete):
         shared_drives = []
         for num, drive in enumerate(self.shared_drives):
-            print("Requesting permissions for file {}/{}".format(num +
-                  1, len(self.shared_drives)))
+            print(
+                "Requesting permissions for file {}/{}".format(
+                    num + 1, len(self.shared_drives)
+                )
+            )
             if num > 0 and (num % 25 == 0):
                 time.sleep(2)
 
-            permissions = self.get_permissions_from_file(drive['id'])
+            permissions = self.get_permissions_from_file(drive["id"])
             for permission in permissions:
-                if permission['emailAddress'] == email_to_delete:
+                if permission["emailAddress"] == email_to_delete:
                     shared_drives.append(
                         {
-                            "drive_name": drive['name'],
-                            "drive_id": drive['id'],
-                            "permission_id": permission['id'],
+                            "drive_name": drive["name"],
+                            "drive_id": drive["id"],
+                            "permission_id": permission["id"],
                         }
                     )
 
         return shared_drives
 
     def delete_file_permission(self, file_id, permission_id):
-        results = self.service.permissions().delete(
-            fileId=file_id,
-            permissionId=permission_id,
-            useDomainAdminAccess=True,
-            supportsAllDrives=True,
-        ).execute()
+        results = (
+            self.service.permissions()
+            .delete(
+                fileId=file_id,
+                permissionId=permission_id,
+                useDomainAdminAccess=True,
+                supportsAllDrives=True,
+            )
+            .execute()
+        )
 
         return results
```

### Comparing `gc_google_services_api-1.2.6/gc_google_services_api/permissions/workspace.py` & `gc_google_services_api-1.2.7/gc_google_services_api/permissions/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,109 @@
 from googleapiclient.discovery import build
 
 from gc_google_services_api.auth import Auth
 
 SCOPES = [
-    'https://www.googleapis.com/auth/admin.directory.group',
-    'https://www.googleapis.com/auth/admin.directory.user',
-    'https://www.googleapis.com/auth/admin.directory.rolemanagement'
+    "https://www.googleapis.com/auth/admin.directory.group",
+    "https://www.googleapis.com/auth/admin.directory.user",
+    "https://www.googleapis.com/auth/admin.directory.rolemanagement",
 ]
 EMPTY_ARRAY = []
 
 
 class WorkSpace:
     """
-        Google API documentation:
-            - https://developers.google.com/resources/api-libraries/documentation/admin/directory_v1/python/latest/admin_directory_v1.groups.html # noqa: E501
-            - https://googleapis.github.io/google-api-python-client/docs/dyn/admin_directory_v1.users.html
+    Google API documentation:
+        - https://developers.google.com/resources/api-libraries/documentation/admin/directory_v1/python/latest/admin_directory_v1.groups.html # noqa: E501
+        - https://googleapis.github.io/google-api-python-client/docs/dyn/admin_directory_v1.users.html
     """
 
     def __init__(self, subject_email, domain) -> None:
         self.domain = domain
         self.credentials = Auth(SCOPES, subject_email).get_credentials()
-        self.service = build('admin', 'directory_v1',
-                             credentials=self.credentials)
+        self.service = build(
+            "admin",
+            "directory_v1",
+            credentials=self.credentials,
+        )
         self.groups_to_delete = []
 
     def _add_groups(self, group):
         self.groups_to_delete.append(group)
 
     def store_groups(self, groups):
         for group in groups:
             self._add_groups(group)
 
     def get_groups_by_email(self, email, next_page_token=None):
-        results = self.service.groups().list(
-            domain=self.domain,
-            maxResults=200,
-            pageToken=next_page_token,
-            userKey=email,
-        ).execute()
+        results = (
+            self.service.groups()
+            .list(
+                domain=self.domain,
+                maxResults=200,
+                pageToken=next_page_token,
+                userKey=email,
+            )
+            .execute()
+        )
 
-        groups = results.get('groups', EMPTY_ARRAY)
+        groups = results.get("groups", EMPTY_ARRAY)
         self.store_groups(groups)
 
-        next_page_token = results.get('nextPageToken', None)
+        next_page_token = results.get("nextPageToken", None)
         if next_page_token:
             print("Requesting groups ({})...".format(next_page_token))
             self.get_groups_by_email(email, next_page_token)
 
     def get_all_groups(self, next_page_token=None):
         # TODO: Almacenar en una variable todos los grupos
-        results = self.service.groups().list(
-            domain=self.domain,
-            maxResults=200,
-            pageToken=next_page_token,
-        ).execute()
+        results = (
+            self.service.groups()
+            .list(
+                domain=self.domain,
+                maxResults=200,
+                pageToken=next_page_token,
+            )
+            .execute()
+        )
 
-        groups = results.get('groups', EMPTY_ARRAY)
+        groups = results.get("groups", EMPTY_ARRAY)
         self.store_groups(groups)
 
-        next_page_token = results.get('nextPageToken', None)
+        next_page_token = results.get("nextPageToken", None)
         if next_page_token:
             print("Requesting groups ({})...".format(next_page_token))
             self.get_all_groups(next_page_token)
 
     def get_members_from_group(self, group_key):
         results = self.service.members().list(groupKey=group_key).execute()
 
-        return results.get('members', EMPTY_ARRAY)
+        return results.get("members", EMPTY_ARRAY)
 
     def delete_group_permission(self, group_id, email_to_delete):
-        results = self.service.members().delete(
-            groupKey=group_id,
-            memberKey=email_to_delete,
-        ).execute()
+        results = (
+            self.service.members()
+            .delete(
+                groupKey=group_id,
+                memberKey=email_to_delete,
+            )
+            .execute()
+        )
 
         return results
 
     def find_groups_permission_to_delete(self, groups, email_to_delete):
         group_permissions_to_delete = []
         for group in groups:
-            group_members = self.get_members_from_group(group['id'])
+            group_members = self.get_members_from_group(group["id"])
 
             for member in group_members:
-                if member['email'] == email_to_delete:
-                    group_permissions_to_delete.append({
-                        "group_name": group['name'],
-                        "group_id": group['id'],
-                    })
+                if member["email"] == email_to_delete:
+                    group_permissions_to_delete.append(
+                        {
+                            "group_name": group["name"],
+                            "group_id": group["id"],
+                        }
+                    )
                     break
 
         return group_permissions_to_delete
```

### Comparing `gc_google_services_api-1.2.6/PKG-INFO` & `gc_google_services_api-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gc-google-services-api
-Version: 1.2.6
+Version: 1.2.7
 Summary: 
 Author: Jonathan Rodríguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: google-api-python-client (>=2.80.0,<3.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.6.0,<4.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
+Requires-Dist: pre-commit (>=3.3.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![Publish to PyPI.org](https://github.com/GoodCod3/gc-google-services-api/actions/workflows/pr.yml/badge.svg)](https://github.com/GoodCod3/gc-google-services-api/actions/workflows/pr.yml)
 
 # How to contribute
 After clone repository
 ## 1.- Install dependencies
@@ -29,15 +30,15 @@
 make test
 ```
 
 # Publish new version
 When your Pull Request is approved and merged with master, then to can generate new version running the next command:
 
 ```bash
-make v=X.Y.Z release 
+make v=X.Y.Z release
 ```
 or you can execute
 ```bash
 poetry version X.Y.Z <-- (New version)
 git commit -am "Release vX.Y.Z"
 git tag vX.Y.Z
 git push --follow-tags
```

