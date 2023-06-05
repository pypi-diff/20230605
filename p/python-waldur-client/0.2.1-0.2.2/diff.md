# Comparing `tmp/python-waldur-client-0.2.1.tar.gz` & `tmp/python-waldur-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-waldur-client-0.2.1.tar", last modified: Sat Feb 18 07:14:15 2023, max compression
+gzip compressed data, was "python-waldur-client-0.2.2.tar", last modified: Mon Jun  5 09:02:54 2023, max compression
```

## Comparing `python-waldur-client-0.2.1.tar` & `python-waldur-client-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 07:14:15.217656 python-waldur-client-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-02-03 13:42:49.000000 python-waldur-client-0.2.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      672 2023-02-18 07:14:15.213657 python-waldur-client-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-02-03 13:42:49.000000 python-waldur-client-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-18 07:14:15.217656 python-waldur-client-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 07:14:15.213657 python-waldur-client-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 07:14:15.213657 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      672 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-18 07:14:15.000000 python-waldur-client-0.2.1/src/python_waldur_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    75479 2023-02-18 07:12:59.000000 python-waldur-client-0.2.1/src/waldur_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-11 11:52:58.000000 python-waldur-client-0.2.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-11 11:52:58.000000 python-waldur-client-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:02:54.666197 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 09:02:54.000000 python-waldur-client-0.2.2/src/python_waldur_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    77001 2023-06-05 08:44:36.000000 python-waldur-client-0.2.2/src/waldur_client.py
```

### Comparing `python-waldur-client-0.2.1/LICENSE.md` & `python-waldur-client-0.2.2/LICENSE.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 OpenNode LLC
+Copyright (c) 2021-2023 OpenNode LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `python-waldur-client-0.2.1/PKG-INFO` & `python-waldur-client-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.1/setup.py` & `python-waldur-client-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 tests_requires = [
     "responses>=0.5.0",
     "pytest>=6.2.5",
 ]
 
 setup(
     name="python-waldur-client",
-    version="0.2.1",
+    version="0.2.2",
     author="OpenNode Team",
     author_email="info@opennodecloud.com",
     url="https://waldur.com",
     license="MIT",
     description="REST client for the Waldur API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `python-waldur-client-0.2.1/src/python_waldur_client.egg-info/PKG-INFO` & `python-waldur-client-0.2.2/src/python_waldur_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.1/src/waldur_client.py` & `python-waldur-client-0.2.2/src/waldur_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
         Invoice = "invoices"
         InvoiceItems = "invoice-items"
         MarketplaceCategories = "marketplace-categories"
         MarketplaceProviderOffering = "marketplace-provider-offerings"
         MarketplaceOrder = "marketplace-orders"
         MarketplaceOrderItem = "marketplace-order-items"
         MarketplaceProviderPlan = "marketplace-plans"
-        MarketplacePublicPlan = "marketplace-public-plans"
         MarketplacePublicOffering = "marketplace-public-offerings"
         MarketplaceResources = "marketplace-resources"
         MarketplaceStats = "marketplace-stats"
         MarketplaceSlurm = "marketplace-slurm"
         MarketplaceSlurmRemote = "marketplace-slurm-remote"
         MarketplaceRobotAccount = "marketplace-robot-accounts"
         OfferingPermissions = "marketplace-offering-permissions"
@@ -213,16 +212,22 @@
 
     def _build_url(self, endpoint, action=None):
         parts = [endpoint]
         if action:
             parts.append(action)
         return urljoin(self.api_url, self._ensure_trailing_slash("/".join(parts)))
 
-    def _build_resource_url(self, endpoint, uid, action=None):
-        parts = [endpoint, str(uid)]
+    def _build_resource_url(
+        self, endpoint, uid1, action=None, sub_endpoint=None, uid2=None
+    ):
+        parts = [endpoint, str(uid1)]
+
+        if sub_endpoint is not None and uid2 is not None:
+            parts.extend([sub_endpoint, str(uid2)])
+
         if action:
             parts.append(action)
         return self._build_url("/".join(parts))
 
     def _parse_error(self, response):
         reason = getattr(response, "reason")
 
@@ -234,18 +239,27 @@
         details = "URL %s. Status: %s. Reason: %s." % (
             response.url,
             response.status_code,
             reason,
         )
         return "Server refuses to communicate. %s" % details
 
-    def _make_request(self, method, url, valid_states, retry_count=3, **kwargs):
+    def _make_request(
+        self,
+        method,
+        url,
+        valid_states,
+        retry_count=3,
+        prev_response_data=None,
+        **kwargs,
+    ):
         if retry_count == 0:
             raise WaldurClientException(
-                "Reached a limit of retries for the operation: %s %s" % (method, url)
+                "Reached a limit of retries for the operation: %s %s, body: %s"
+                % (method, url, prev_response_data)
             )
 
         params = dict(headers=self.headers, verify=verify_ssl)
         params.update(kwargs)
 
         try:
             response = getattr(requests, method)(url, **params)
@@ -253,15 +267,20 @@
             raise WaldurClientException(str(error))
 
         if response.status_code not in valid_states:
             # a special treatment for 409 response, which can be due to async operations
             if response.status_code == 409:
                 time.sleep(2)  # wait for things to calm down
                 return self._make_request(
-                    method, url, valid_states, retry_count - 1, **kwargs
+                    method,
+                    url,
+                    valid_states,
+                    retry_count - 1,
+                    prev_response_data=response.text,
+                    **kwargs,
                 )
             error = self._parse_error(response)
             raise WaldurClientException(error)
 
         if method == "head":
             return response
         if response.text:
@@ -841,14 +860,31 @@
 
     def marketplace_resource_get_plan_periods(self, resource_uuid: str):
         url = self._build_resource_url(
             self.Endpoints.MarketplaceResources, resource_uuid, action="plan_periods"
         )
         return self._get(url, valid_states=[200])
 
+    def marketplace_public_offering_get_plans(self, offering_uuid: str):
+        url = self._build_resource_url(
+            self.Endpoints.MarketplacePublicOffering, offering_uuid, action="plans"
+        )
+        return self._get(url, valid_states=[200])
+
+    def marketplace_public_offering_get_plan_details(
+        self, offering_uuid: str, plan_uuid: str
+    ):
+        url = self._build_resource_url(
+            self.Endpoints.MarketplacePublicOffering,
+            "plans",
+            offering_uuid,
+            plan_uuid,
+        )
+        return self._get(url, valid_states=[200])
+
     def update_marketplace_resource(self, resource_uuid: str, **kwargs):
         return self._patch_resource(
             self.Endpoints.MarketplaceResources, resource_uuid, kwargs
         )
 
     def get_instance_via_marketplace(self, name, project=None):
         """Get an openstack instance via marketplace.
@@ -1073,16 +1109,18 @@
                 self.Endpoints.MarketplacePublicOffering,
                 offering,
                 {"project_uuid": project_uuid, "state": ["Active", "Paused"]},
             )
         else:
             return
 
-    def _get_plan(self, identifier):
-        return self._get_resource(self.Endpoints.MarketplacePublicPlan, identifier)
+    def _get_plan(self, offering_identifier, plan_identifier):
+        return self.marketplace_public_offering_get_plan_details(
+            offering_identifier, plan_identifier
+        )
 
     def create_marketplace_order(
         self, project, offering, plan=None, attributes=None, limits=None
     ):
         """
         Create order with one item in Waldur Marketplace.
 
@@ -1090,15 +1128,15 @@
         :param offering: the name or UUID of the offering
         :param plan: the name or UUID of the plan.
         :param attributes: order item attributes.
         :param limits: order item limits.
         """
         project_uuid = self._get_project(project)["uuid"]
         offering_uuid = self._get_offering(offering, project)["uuid"]
-        plan_uuid = plan and self._get_plan(plan)["uuid"]
+        plan_uuid = plan and self._get_plan(offering_uuid, plan)["uuid"]
         return self.marketplace_resource_create_order(
             project_uuid, offering_uuid, plan_uuid, attributes, limits
         )
 
     def get_order(self, order_uuid):
         return self._get_resource(WaldurClient.Endpoints.MarketplaceOrder, order_uuid)
 
@@ -1628,15 +1666,18 @@
             ),
             "attributes": attributes,
             "limits": limits,
         }
 
         if plan_uuid:
             order_item["plan"] = self._build_resource_url(
-                self.Endpoints.MarketplacePublicPlan, plan_uuid
+                self.Endpoints.MarketplacePublicOffering,
+                "plans",
+                offering_uuid,
+                plan_uuid,
             )
 
         if callback_url:
             order_item["callback_url"] = callback_url
 
         # TODO: replace with checkbox data from frontend
         order_item["accepting_terms_of_service"] = True
@@ -2069,27 +2110,38 @@
 
     def list_robot_account(self, filters=None):
         return self._query_resource_list(
             self.Endpoints.MarketplaceRobotAccount, filters
         )
 
     def create_robot_account(self, resource, type, users=[], username="", keys=[]):
+        params = {
+            "resource": resource,
+            "type": type,
+            "users": users,
+            "username": username,
+            "keys": keys,
+        }
+        if is_uuid(resource):
+            params["resource"] = self._build_url(
+                self.Endpoints.MarketplaceResources + "/" + resource
+            )
+        if users:
+            for idx, user in enumerate(users):
+                if is_uuid(user):
+                    params["users"][idx] = self._build_url(
+                        self.Endpoints.Users + "/" + user
+                    )
         return self._create_resource(
             self.Endpoints.MarketplaceRobotAccount,
-            payload={
-                "resource": resource,
-                "type": type,
-                "username": username,
-                "users": users,
-                "keys": keys,
-            },
+            payload=params,
         )
 
     def update_robot_account(self, account_uuid, payload):
-        return self._update_resource(
+        return self._patch_resource(
             self.Endpoints.MarketplaceRobotAccount,
             account_uuid,
             payload,
         )
 
     def delete_robot_account(self, account_uuid):
         return self._delete_resource(
```

