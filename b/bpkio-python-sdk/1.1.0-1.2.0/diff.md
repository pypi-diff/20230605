# Comparing `tmp/bpkio_python_sdk-1.1.0.tar.gz` & `tmp/bpkio_python_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.1.0.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.2.0.tar", max compression
```

## Comparing `bpkio_python_sdk-1.1.0.tar` & `bpkio_python_sdk-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,61 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.1.0/README.md
--rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.1.0/bpkio_api/__init__.py
--rw-r--r--   0        0        0     5127 2023-05-17 20:59:10.717567 bpkio_python_sdk-1.1.0/bpkio_api/api.py
--rw-r--r--   0        0        0     1044 2023-04-20 16:56:18.119327 bpkio_python_sdk-1.1.0/bpkio_api/caching.py
--rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.1.0/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.1.0/bpkio_api/defaults.py
--rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4379 2023-05-12 07:24:24.240126 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      658 2023-04-14 21:22:20.218915 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0    21801 2023-05-17 17:12:06.162415 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21435 2023-05-16 19:15:10.787303 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0     2667 2023-05-12 07:24:24.242152 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     5713 2023-05-12 07:24:24.242673 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2619 2023-05-12 07:24:24.243027 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.1.0/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.1.0/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3333 2023-05-04 10:23:23.525504 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4390 2023-05-17 17:41:42.490027 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.1.0/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.1.0/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     3082 2023-05-02 21:12:09.864720 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1516 2023-05-02 21:16:30.728876 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.1.0/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.1.0/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2000 2023-05-12 19:28:37.449401 bpkio_python_sdk-1.1.0/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.1.0/bpkio_api/mappings.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.1.0/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.1.0/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     4815 2023-05-16 12:12:43.320150 bpkio_python_sdk-1.1.0/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1776 2023-04-27 17:11:34.397967 bpkio_python_sdk-1.1.0/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.1.0/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.1.0/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.1.0/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.1.0/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.1.0/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      911 2023-05-01 20:11:46.199279 bpkio_python_sdk-1.1.0/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.1.0/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     1604 2023-04-14 21:22:20.224021 bpkio_python_sdk-1.1.0/bpkio_api/response_handler.py
--rw-r--r--   0        0        0     1195 2023-05-17 22:55:41.179720 bpkio_python_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.2.0/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.2.0/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     5308 2023-05-21 17:03:47.808287 bpkio_python_sdk-1.2.0/bpkio_api/api.py
+-rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.2.0/bpkio_api/caching.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.2.0/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.2.0/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4521 2023-05-20 12:34:42.082005 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      666 2023-05-20 12:34:42.082634 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/enums.py
+-rw-r--r--   0        0        0    21988 2023-05-20 12:34:42.083318 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21622 2023-05-20 12:34:42.084047 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0     2675 2023-05-20 12:34:42.084780 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     5879 2023-05-20 12:34:42.085269 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2627 2023-05-20 12:34:42.085823 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.2.0/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.2.0/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3644 2023-06-02 14:52:57.666804 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4431 2023-06-02 14:35:26.107648 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.2.0/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.2.0/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/curl.py
+-rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/exporter.py
+-rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/markdown.py
+-rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/postman.py
+-rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_items.py
+-rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_recorder.py
+-rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/text.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.2.0/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.2.0/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.2.0/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.2.0/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.2.0/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.2.0/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.2.0/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.2.0/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.2.0/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.2.0/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.2.0/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.2.0/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.2.0/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.2.0/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.2.0/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     1941 2023-05-21 20:52:58.371698 bpkio_python_sdk-1.2.0/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-06-05 14:46:01.091632 bpkio_python_sdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.2.0/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/api.py` & `bpkio_python_sdk-1.2.0/bpkio_api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,35 +15,37 @@
     ServicesApi,
     SourcesApi,
     TenantsApi,
     TranscodingProfilesApi,
     UsersApi,
 )
 from bpkio_api.exceptions import InvalidApiKeyFormat
+from bpkio_api.helpers.recorder import SessionRecorder
 from bpkio_api.mappings import model_to_endpoint
 from bpkio_api.models import Tenant
 
 
 class BroadpeakIoApi(Consumer):
     def __init__(
         self,
         *,
         tenant: Optional[str] = None,
         api_key: Optional[str] = None,
         fqdn: str = DEFAULT_FQDN,
         use_cache: bool = True,
+        session_file: Optional[str] = None,
         **kwargs,
     ):
         if tenant and api_key:
             raise ValueError("You can't specify both tenant and api_key")
 
         tp = TenantProfileProvider()
 
         if tenant:
-            if isinstance(tenant, str):                
+            if isinstance(tenant, str):
                 t = tp.get_tenant_profile(tenant)
             if isinstance(tenant, TenantProfile):
                 t = tenant
             self._api_key = t.api_key
             self._fqdn = t.fqdn
 
         elif api_key:
@@ -74,14 +76,16 @@
 
         super().__init__(base_url, auth=BearerToken(self._api_key), **kwargs)
 
         tenant_id = self.parse_api_key().get("tenantId")
         if use_cache:
             init_cache(self.fqdn, tenant_id)
 
+        self.session_recorder = SessionRecorder(session_file)
+
         self.sources = SourcesApi(base_url, auth=BearerToken(self._api_key), **kwargs)
         self.services = ServicesApi(base_url, auth=BearerToken(self._api_key), **kwargs)
         self.tenants = TenantsApi(base_url, auth=BearerToken(self._api_key), **kwargs)
         self.users = UsersApi(base_url, auth=BearerToken(self._api_key), **kwargs)
         self.transcoding_profiles = TranscodingProfilesApi(
             base_url, auth=BearerToken(self._api_key), **kwargs
         )
@@ -124,14 +128,15 @@
             return True
         except:
             return False
 
     def get_tenant_id(self) -> int:
         return self.parse_api_key().get("tenantId")
 
+    @SessionRecorder.do_not_record
     def get_self_tenant(self) -> Tenant:
         """Get tenant linked to the current API Key"""
 
         tenant_id = self.get_tenant_id()
         tenant = self.tenants.retrieve(tenant_id)
         tenant._fqdn = self.fqdn
         return tenant
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/caching.py` & `bpkio_python_sdk-1.2.0/bpkio_api/caching.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os
 import tempfile
 
 import diskcache
 
+from .helpers.recorder import SessionComment, SessionRecorder
+
 logger = logging.getLogger(__name__)
 
 CACHE: diskcache.Cache | None = None
 
 
 def init_cache(fqdn, tenant_id):
     temp_dir = tempfile.gettempdir()
@@ -22,17 +24,48 @@
     """Decorator to retrieve and/or store the results of an API helper method into Cache"""
 
     def decorator(func):
         def wrapper(*args, **kwargs):
             global CACHE
             if CACHE is not None and key in CACHE:
                 logger.debug(f"Cache entry found for '{key}'")
+                SessionRecorder.record(SessionComment("Cache hit"))
                 return CACHE[key]
             result = func(*args, **kwargs)
             if CACHE is not None:
                 CACHE.set(key=key, value=result, expire=ttl)
                 logger.debug(f"Adding cache entry for '{key}'")
             return result
 
         return wrapper
 
     return decorator
+
+
+def invalidate_cache(key: str):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            result = func(*args, **kwargs)
+
+            global CACHE
+            if CACHE is not None and key in CACHE:
+                del CACHE[key]
+                logger.debug("Cache for '{key}' cleared")
+            return result
+
+        return wrapper
+
+    return decorator
+
+
+def clear_cache_entry(key: str):
+    global CACHE
+    if CACHE is not None and key in CACHE:
+        del CACHE[key]
+        logger.debug(f"Cache for '{key}' cleared")
+
+
+def clear_cache():
+    global CACHE
+    if CACHE is not None:
+        CACHE.clear()
+        logger.debug("Cache cleared")
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.2.0/bpkio_api/credential_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/categories.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 )
 
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import ResourceExistsError
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Categories import Category, CategoryIn
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
+from .enums import UpsertOperationType
 
-@response_handler(raise_for_status)
+
+@response_handler(postprocess_response)
 class CategoriesApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json(List[Category])
     @get("categories")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[Category]:  # type: ignore
@@ -37,15 +39,15 @@
         """Get a single category, by ID"""
 
     @json
     @returns.json(Category)
     @post("categories")
     def create(self, category: Body(type=CategoryIn)) -> Category:  # type: ignore
         """Create a new category"""
-        
+
     @json
     @returns.json(Category)
     @put("categories/{category_id}")
     def update(self, category_id: int, category: Body(type=CategoryIn)) -> Category:  # type: ignore
         """Update a category"""
 
     @delete("categories/{category_id}")
@@ -89,31 +91,33 @@
         """
         if not filters:
             filters = [(value, field, method)]
 
         sources = self.list()
         return search_array_with_filters(sources, filters=filters)
 
-    def upsert(self, category: CategoryIn, if_exists: str | None = None) -> Category:
+    def upsert(
+        self, category: CategoryIn, if_exists: str | None = None
+    ) -> Tuple[Category, UpsertOperationType]:
         """Create, retrieve or update a category
 
         Args:
             category (CategoryIn): The category payload
             if_exists (str): What to do if the category already exists (error, retrieve, update)
 
         Returns:
             Category: the category retrieved or created
         """
 
         try:
-            return (self.create(category), 1)
+            return (self.create(category), UpsertOperationType.CREATED)
         except ResourceExistsError as e:
             if if_exists == "error":
-                return (category, -1)
-                        
+                return (category, UpsertOperationType.ERROR)
+
             existing_category = self.search(value=category.name, field="name")[0]
-    
+
             if if_exists == "retrieve":
-                return (existing_category, 0)
-            elif if_exists == "update":                
+                return (existing_category, UpsertOperationType.RETRIEVED)
+            elif if_exists == "update":
                 updated_category = self.update(existing_category.id, category)
-                return (updated_category, 2)
+                return (updated_category, UpsertOperationType.UPDATED)
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/consumption.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 
 from uplink import Consumer, Query, get, response_handler, returns
 
 from bpkio_api.models.Consumption import ConsumptionData
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class ConsumptionApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("consumption")
     def retrieve(
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 from bpkio_api.exceptions import BroadpeakIoHelperError, ResourceExistsError
 from bpkio_api.helpers.list import collect_from_ids, get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models import ContentReplacementSlot
 from bpkio_api.models import Services as Svc
 from bpkio_api.models import VirtualChannelSlot, VirtualChannelSlotIn
-from bpkio_api.response_handler import raise_for_status, return_count
+from bpkio_api.response_handler import postprocess_response, return_count
 
+from .enums import UpsertOperationType
 
-@response_handler(raise_for_status)
+
+@response_handler(postprocess_response)
 class ServicesApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
         self.virtual_channel = VirtualChannelServiceApi(
             parent_api=self, base_url=base_url, **kwargs
         )
@@ -203,15 +205,15 @@
         if_exists: str = "retrieve",
         unique_fields: List[str | Tuple] = [],
     ) -> Tuple[
         Svc.VirtualChannelService
         | Svc.ContentReplacementService
         | Svc.AdInsertionService
         | Svc.ServiceIn,
-        int,
+        UpsertOperationType,
     ]:
         """Creates a service with adaptable behaviour if it already exist.
 
         Args:
             service (ServiceIn): The payload for the service to create
             if_exists (str): What action to take if it exists:
               `error` (default) returns an error;
@@ -225,18 +227,18 @@
             AdInsertionService | ServiceIn, int]:
             The resource created or retrieved, with an indicator:
             1 = created, 0 = retrieved, 2 = updated, -1 = failed
 
         """
 
         try:
-            return (self.create(service), 1)
+            return (self.create(service), UpsertOperationType.CREATED)
         except ResourceExistsError as e:
             if if_exists == "error":
-                return (service, -1)
+                return (service, UpsertOperationType.ERROR)
 
             unique_fields = list(set(unique_fields + ["name"]))
             for fld in unique_fields:
                 # single field
                 if isinstance(fld, str):
                     fld = (fld,)
 
@@ -244,24 +246,24 @@
                 dupes = find_duplicates_of(
                     obj=service, in_list=self.list(), by_fields=fld
                 )
                 if dupes:
                     existing_resource = self.retrieve(dupes[0][1].id)
 
                     if if_exists == "retrieve":
-                        return (existing_resource, 0)
+                        return (existing_resource, UpsertOperationType.RETRIEVED)
                     elif if_exists == "update":
                         updated_resource = self._update(existing_resource.id, service)
-                        return (updated_resource, 2)
+                        return (updated_resource, UpsertOperationType.UPDATED)
 
 
 # === CONTENT-REPLACEMENT SERVICES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class ContentReplacementServiceApi(Consumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
         self.slots = ContentReplacementServiceSlotsApi(base_url, **kwargs)
 
@@ -317,15 +319,15 @@
         if not filters:
             filters = [(value, field, method)]
 
         services = self.list()
         return search_array_with_filters(services, filters=filters)
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class ContentReplacementServiceSlotsApi(Consumer):
     @returns.json()
     @get("services/content-replacement/{service_id}/slots")
     def get_page(
         self,
         service_id,
         offset: Query = 0,
@@ -392,15 +394,15 @@
             categories=categories,
         )
 
 
 # === VIRTUAL-CHANNEL SERVICES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class VirtualChannelServiceApi(Consumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
         self.slots = VirtualChannelServiceSlotsApi(base_url, **kwargs)
 
@@ -454,15 +456,15 @@
         if not filters:
             filters = [(value, field, method)]
 
         services = self.list()
         return search_array_with_filters(services, filters=filters)
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class VirtualChannelServiceSlotsApi(Consumer):
     @returns.json()
     @get("services/virtual-channel/{service_id}/slots")
     def get_page(
         self,
         service_id,
         offset: Query = 0,
@@ -537,15 +539,15 @@
             categories=categories,
         )
 
 
 # === AD-INSERTION SERVICES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class AdInsertionServiceApi(Consumer):
     def __init__(self, parent_api: ServicesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(Svc.AdInsertionService)
     @get("services/ad-insertion/{service_id}")
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 from bpkio_api.caching import cache_api_results
 from bpkio_api.exceptions import BroadpeakIoHelperError, ResourceExistsError
 from bpkio_api.helpers.list import collect_from_ids, get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models import Sources as S
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
+from .enums import UpsertOperationType
 
-@response_handler(raise_for_status)
+
+@response_handler(postprocess_response)
 class SourcesApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
         self.asset = AssetSourcesApi(parent_api=self, base_url=base_url, **kwargs)
         self.live = LiveSourcesApi(parent_api=self, base_url=base_url, **kwargs)
         self.asset_catalog = AssetCatalogSourcesApi(
@@ -206,15 +208,15 @@
     ) -> Tuple[
         S.AssetSource
         | S.AdServerSource
         | S.AssetCatalogSource
         | S.SlateSource
         | S.LiveSource
         | S.SourceIn,
-        int,
+        UpsertOperationType,
     ]:
         """Creates a source with adaptable behaviour if it already exist.
 
         Args:
             source (SourceIn): The payload for the source to create
             if_exists (str): What action to take if it exists:
               `error` (default) returns an error;
@@ -226,18 +228,18 @@
         Returns:
             Tuple[AssetSource | AdServerSource | AssetCatalogSource | SlateSource | LiveSource | None, int]:
             The resource created or retrieved, with an indicator: 1 = created, 0 = retrieved, 2 = updated, -1 = failed
 
         """
 
         try:
-            return (self.create(source), 1)
+            return (self.create(source), UpsertOperationType.CREATED)
         except ResourceExistsError as e:
             if if_exists == "error":
-                return (source, -1)
+                return (source, UpsertOperationType.ERROR)
 
             unique_fields = list(set(unique_fields + ["name"]))
             for fld in unique_fields:
                 # single field
                 if isinstance(fld, str):
                     fld = (fld,)
 
@@ -245,18 +247,18 @@
                 dupes = find_duplicates_of(
                     obj=source, in_list=self.list(), by_fields=fld
                 )
                 if dupes:
                     existing_resource = self.retrieve(dupes[0][1].id)
 
                     if if_exists == "retrieve":
-                        return (existing_resource, 0)
+                        return (existing_resource, UpsertOperationType.RETRIEVED)
                     elif if_exists == "update":
                         updated_resource = self._update(existing_resource.id, source)
-                        return (updated_resource, 2)
+                        return (updated_resource, UpsertOperationType.UPDATED)
 
     def check_by_id(self, source_id: int) -> List[S.SourceCheckResult]:
         source = self.retrieve(source_id=source_id)
 
         if source:
             url = source.url
             if source.type == S.SourceType.ASSET_CATALOG:
@@ -264,15 +266,15 @@
 
             return self.check(type=source.type, url=url)
 
 
 # === ASSET SOURCES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class AssetSourcesApi(Consumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AssetSource)
     @get("sources/asset/{source_id}")
@@ -327,15 +329,15 @@
         sources = self.list()
         return search_array_with_filters(sources, filters=filters)
 
 
 # === LIVE SOURCES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class LiveSourcesApi(Consumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.LiveSource)
     @get("sources/live/{source_id}")
@@ -390,15 +392,15 @@
         sources = self.list()
         return search_array_with_filters(sources, filters=filters)
 
 
 # === ASSET CATALOG SOURCES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class AssetCatalogSourcesApi(Consumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AssetCatalogSource)
     @get("sources/asset-catalog/{source_id}")
@@ -453,15 +455,15 @@
         sources = self.list()
         return search_array_with_filters(sources, filters=filters)
 
 
 # === AD SERVER SOURCES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class AdServerSourcesApi(Consumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.AdServerSource)
     @get("sources/ad-server/{source_id}")
@@ -544,15 +546,15 @@
         sources = self.list()
         return search_array_with_filters(sources, filters=filters)
 
 
 # === SLATE SOURCES ===
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class SlateSourcesApi(Consumer):
     def __init__(self, parent_api: SourcesApi, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
         self.parent_api = parent_api
 
     @returns.json(S.SlateSource)
     @get("sources/slate/{source_id}")
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/tenants.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from uplink import Consumer, Query, get, response_handler, returns
 
 from bpkio_api.caching import cache_api_results
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Tenants import Tenant
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class TenantsApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json(List[Tenant])
     @get("tenants")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[Tenant]:  # type: ignore
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.objects import find_duplicates_of
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.TranscodingProfiles import (
     TranscodingProfile,
     TranscodingProfileIn,
 )
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
+from .enums import UpsertOperationType
 
-@response_handler(raise_for_status)
+
+@response_handler(postprocess_response)
 class TranscodingProfilesApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("transcoding-profiles")
     def get_page(
@@ -101,15 +103,15 @@
         profiles = self.list(tenantId=tenantId)
         return search_array_with_filters(profiles, filters=filters)
 
     def upsert(
         self,
         profile: TranscodingProfileIn,
         if_exists: str = "retrieve",
-    ) -> Tuple[TranscodingProfile | TranscodingProfileIn, int,]:  # type: ignore
+    ) -> Tuple[TranscodingProfile | TranscodingProfileIn, UpsertOperationType]:  # type: ignore
         """Creates a transcoding profile with adaptable behaviour if it already exist.
 
         Args:
             profile (TranscodingProfileIn): The payload for the source to create
             if_exists (str): What action to take if it exists:
               `error` (default) returns an error;
               `retrieve` returns the existing object;
@@ -120,18 +122,18 @@
         Returns:
             Tuple[TranscodingProfile | None, int]:
                 The resource created or retrieved, with an indicator: 1 = created, 0 = retrieved, 2 = updated, -1 = failed
 
         """
 
         try:
-            return (self.create(profile), 1)
+            return (self.create(profile), UpsertOperationType.CREATED)
         except ResourceExistsError as e:
             if if_exists == "error":
-                return (profile, -1)
+                return (profile, UpsertOperationType.ERROR)
 
             unique_fields = list(set("name"))
             for fld in unique_fields:
                 # single field
                 if isinstance(fld, str):
                     fld = (fld,)
 
@@ -139,11 +141,11 @@
                 dupes = find_duplicates_of(
                     obj=profile, in_list=self.list(), by_fields=fld
                 )
                 if dupes:
                     existing_resource = self.retrieve(dupes[0][1].id)
 
                     if if_exists == "retrieve":
-                        return (existing_resource, 0)
+                        return (existing_resource, UpsertOperationType.RETRIEVED)
                     elif if_exists == "update":
                         updated_resource = self.update(existing_resource.id, profile)
-                        return (updated_resource, 2)
+                        return (updated_resource, UpsertOperationType.UPDATED)
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from uplink import Consumer, Query, get, response_handler, returns
 
 from bpkio_api.caching import cache_api_results
 from bpkio_api.helpers.list import get_all_with_pagination
 from bpkio_api.helpers.search import SearchMethod, search_array_with_filters
 from bpkio_api.models.Users import User
-from bpkio_api.response_handler import raise_for_status
+from bpkio_api.response_handler import postprocess_response
 
 
-@response_handler(raise_for_status)
+@response_handler(postprocess_response)
 class UsersApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("users")
     def get_page(self, offset: Query = 0, limit: Query = 5) -> List[User]:  # type: ignore
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.2.0/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         _registry[content_type] = handler_cls
     for extension in handler_cls.file_extensions:
         _registry[extension] = handler_cls
 
 
 def fetch_content_with_size_limit(url, size_limit, enforce_limit=True):
     response = requests.get(url, stream=True, headers=headers)
+    if response.status_code != 200:
+        raise BroadpeakIoHelperError(
+            status_code=response.status_code,
+            message=f"Unable to fetch content - server response {response.status_code} for url {url}",
+            original_message="",
+        )
+
     content = b""
     for chunk in response.iter_content(chunk_size=1024):
         content += chunk
         if len(content) > size_limit:
             raise Exception("Content too long to be parseable efficiently")
     return content
 
@@ -83,15 +90,15 @@
                     if handler.is_supported_content(content):
                         handler_cls = handler
                         break
 
         if handler_cls is None:
             raise ValueError(
                 "Could not determine content type from content-type, file extension, or content of URL: "
-                f"{content_type} / {file_extension}"
+                f"- TYPE: {content_type} \n- EXTENSION: {file_extension} \n- CONTENT: {content}"
             )
 
         return handler_cls(url, content)
 
     except Exception as e:
         raise BroadpeakIoHelperError(
             status_code=400,
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/generic.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/hls.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 
     def has_children(self) -> bool:
         if self.document.is_variant:
             return True
         return False
 
     def get_child(self, index: int):
+        playlists = self.document.playlists + self.document.media
+
         try:
-            return HLSHandler(url=self.document.playlists[index - 1].absolute_uri)
+            return HLSHandler(url=playlists[index - 1].absolute_uri)
         except IndexError as e:
             raise BroadpeakIoHelperError(
                 status_code=404,
                 message=f"The HLS manifest only has {len(self.document.playlists)} renditions.",
                 original_message=e.args[0],
             )
 
@@ -77,18 +79,18 @@
         """Calculates the number of segments in the stream
 
         Returns:
             int
         """
         sub = self._fetch_sub(self.document.playlists[0].absolute_uri)
         return len(sub.segments)
-    
+
     def has_muxed_audio(self) -> bool:
         """Checks is the audio stream is muxed in with video
-        
+
         Returns:
             bool
         """
         for media in self.document.media:
             if media.type == "AUDIO":
                 if media.uri is None:
                     return True
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vast.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vmap.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/hls.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,32 @@
             bandwidth = variant.stream_info.bandwidth
             frame_rate = variant.stream_info.frame_rate
 
             codecstrings = variant.stream_info.codecs
             codecs = CodecStringParser.parse_multi_codec_string(codecstrings)
 
             for codec in codecs:
+                video_profile = "main"
                 if codec["type"] == "video":
+                    video_profile = codec.get("profile")
                     codec["resolution"] = resolution
                     codec["bitrate"] = bandwidth
                     codec["framerate"] = frame_rate or self.get_framerate(
                         variant.absolute_uri
                     )
                     codec["audio-group"] = variant.stream_info.audio
                     video_renditions[variant.uri] = codec
 
                 if codec["type"] == "audio":
-                    # TODO - extract audio info
-                    codec["bitrate"] = bandwidth
+                    # TODO - better mechanism to actually extract audio info
+                    if video_profile == "baseline":
+                        codec["bitrate"] = "64k"
+                    else:
+                        codec["bitrate"] = "128k"
+                        
                     audio_renditions[variant.stream_info.audio] = codec
 
                     if len(variant.media) and variant.media[0].uri is None:
                         codec["muxed"] = True
 
                 # TODO - determine when audio is muxed in
                 # TODO - when audio not muxed in (separate or adjoining streaminf),
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,36 @@
         }
 
         jobs = []
         for r in renditions:
             if r["type"] == "video":
                 jobs.append(
                     {
-                        "level": r["level"],
+                        "level": str(r["level"]),
                         "scale": f"-1:{r['resolution'][1]}",
-                        "bitratev": r["bitrate"],
+                        "bitratev": str(r["bitrate"]),
                         "profilev": r["profile"],
-                        "frameratev": r["framerate"],
+                        "frameratev": str(r["framerate"]),
                     }
                 )
 
             if r["type"] == "audio":
                 audio_spec = {
                     "codeca": "aac",
-                    "bitratea": r["bitrate"],
+                    "bitratea": str(r["bitrate"]),
                     "loudnorm": "I=-23:TP=-1",
                 }
 
-                if r.get("muxed") is True:
-                    common.update(audio_spec)
+                # if r.get("muxed") is True:
+                #     common.update(audio_spec)
 
-                else:
-                    jobs.append(audio_spec)
+                # else:
+                #     jobs.append(audio_spec)
+
+                common.update(audio_spec)
 
         profile = {
             "packaging": {
                 "--hls.client_manifest_version=": "4",
                 "--hls.minimum_fragment_length=": "4",
             },
             "servicetype": "offline_transcoding",
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.2.0/bpkio_api/helpers/times.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,7 +60,11 @@
 def to_local_tz(dt_with_timezone):
     current_tz = datetime.now().astimezone().tzinfo
     dt_local = dt_with_timezone.astimezone(current_tz)
     return (
         dt_local.strftime("%Y-%m-%d %H:%M:%S.")
         + f"{dt_local.microsecond // 1000:03d} {dt_local.tzname()}"
     )
+
+
+def relative_time(time: datetime):
+    return "{} ({})".format(to_local_tz(time), to_relative_time(time))
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/mappings.py` & `bpkio_python_sdk-1.2.0/bpkio_api/mappings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/Services.py`

 * *Files 17% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 class LiveAdPreRollModelIn(BaseModel):
     adServer: BaseResource
     maxDuration: Optional[float]
     offset: Optional[float]
 
 
-class _WithCommonAdInsertionServiceFields:
+class WithCommonAdInsertionServiceFields(BaseModel):
     enableAdTranscoding: Optional[bool] = False
     enableServerSideAdTracking: Optional[bool] = False
     enableSSATCheckChunk: Optional[bool] = False
 
     transcodingProfile: Optional[TranscodingProfileId] = None
 
     @property
@@ -128,25 +128,25 @@
     def make_full_url(self, extra=None, *args, **kwargs):
         if extra:
             return urljoin(self.url, extra)
 
         return self.url
 
 
-class AdInsertionServiceIn(ServiceIn, _WithCommonAdInsertionServiceFields):
+class AdInsertionServiceIn(ServiceIn, WithCommonAdInsertionServiceFields):
     vodAdInsertion: Optional[VodAdInsertionModelIn] = None
     liveAdPreRoll: Optional[LiveAdPreRollModelIn] = None
     liveAdReplacement: Optional[LiveAdReplacementModelIn] = None
 
     # TODO: parse the specific sub-type of source
     source: BaseResource
 
 
 class AdInsertionService(
-    ServiceIn, WithCommonServiceFields, _WithCommonAdInsertionServiceFields
+    WithCommonAdInsertionServiceFields, WithCommonServiceFields, ServiceIn
 ):
     vodAdInsertion: Optional[VodAdInsertionModel] = None
     liveAdPreRoll: Optional[LiveAdPreRollModel] = None
     liveAdReplacement: Optional[LiveAdReplacementModel] = None
 
     # TODO: parse the specific sub-type of source
     source: SourceSparse
@@ -157,37 +157,48 @@
 
 
 # === CONTENT-REPLACEMENT SERVICE Models ===
 
 
 class ContentReplacementServiceIn(ServiceIn):
     # TODO: parse the specific sub-type of source
+    source: BaseResource
+    replacement: BaseResource
+
+
+class ContentReplacementService(WithCommonServiceFields, ServiceIn):
     source: SourceSparse
     replacement: SourceSparse
 
-
-class ContentReplacementService(ContentReplacementServiceIn, WithCommonServiceFields):
     @property
     def type(self):
         return ServiceType.CONTENT_REPLACEMENT
 
 
-# === CONTENT-REPLACEMENT SERVICE Models ===
-
+# === VIRTUAL-CHANNEL SERVICE Models ===
 
-class VirtualChannelServiceIn(ServiceIn):
-    # TODO: parse the specific sub-type of source
-    baseLive: BaseResource
 
+class WithCommonVirtualChannelServiceFields(BaseModel):
     enableAdTranscoding: Optional[bool] = False
     enableServerSideAdTracking: Optional[bool] = False
     enableSSATCheckChunk: Optional[bool] = False
-    adBreakInsertion: Optional[AdBreakInsertionModel] = None
 
-    # TODO - migrate to TranscodingProfile Model
-    transcodingProfile: Optional[BaseResource] = None
+    transcodingProfile: Optional[TranscodingProfileId] = None
 
 
-class VirtualChannelService(VirtualChannelServiceIn, WithCommonServiceFields):
+class VirtualChannelServiceIn(ServiceIn, WithCommonVirtualChannelServiceFields):
+    # TODO: parse the specific sub-type of source
+    baseLive: BaseResource
+
+    adBreakInsertion: Optional[AdBreakInsertionModelIn] = None
+
+
+class VirtualChannelService(
+    WithCommonVirtualChannelServiceFields, WithCommonServiceFields, ServiceIn
+):
+    baseLive: SourceSparse
+
+    adBreakInsertion: Optional[AdBreakInsertionModel] = None
+
     @property
     def type(self):
         return ServiceType.VIRTUAL_CHANNEL
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/Slots.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel
 
-from bpkio_api.helpers.times import to_local_tz, to_relative_time
 from bpkio_api.models.common import BaseResource
 from bpkio_api.models.Sources import SourceSparse
+from bpkio_api.helpers.times import relative_time
 
 
 class VirtualChannelSlotType(Enum):
     CONTENT = "content"
     AD_BREAK = "ad-break"
 
     def __str__(self):
@@ -59,9 +59,8 @@
 
 
 class ContentReplacementSlot(BaseResource, ContentReplacementSlotBase):
     replacement: SourceSparse
     category: BaseResource | None
 
 
-def relative_time(time: datetime):
-    return "{} ({})".format(to_local_tz(time), to_relative_time(time))
+
```

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/Sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/common.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.2.0/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.1.0/pyproject.toml` & `bpkio_python_sdk-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.1.0"
+version = "1.2.0"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bpkio_python_sdk-1.1.0/PKG-INFO` & `bpkio_python_sdk-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

