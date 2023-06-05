# Comparing `tmp/stigg_api_client_v2-0.455.1.tar.gz` & `tmp/stigg_api_client_v2-0.457.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.455.1.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.457.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.455.1.tar` & `stigg_api_client_v2-0.457.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1644 2023-06-04 18:07:43.779315 stigg_api_client_v2-0.455.1/README.md
--rw-r--r--   0        0        0      653 2023-06-04 18:24:42.183484 stigg_api_client_v2-0.455.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-04 18:07:43.784846 stigg_api_client_v2-0.455.1/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-04 18:07:43.785257 stigg_api_client_v2-0.455.1/stigg/client.py
--rw-r--r--   0        0        0    39396 2023-06-04 18:24:19.683744 stigg_api_client_v2-0.455.1/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-04 18:24:18.689998 stigg_api_client_v2-0.455.1/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-04 18:24:18.690591 stigg_api_client_v2-0.455.1/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-04 18:24:16.930449 stigg_api_client_v2-0.455.1/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-04 18:24:16.972178 stigg_api_client_v2-0.455.1/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    69448 2023-06-04 18:24:19.294767 stigg_api_client_v2-0.455.1/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-04 18:24:17.006165 stigg_api_client_v2-0.455.1/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-04 18:24:17.158839 stigg_api_client_v2-0.455.1/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23614 2023-06-04 18:24:12.475276 stigg_api_client_v2-0.455.1/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-04 18:24:16.954335 stigg_api_client_v2-0.455.1/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-04 18:24:16.965719 stigg_api_client_v2-0.455.1/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-04 18:24:18.691154 stigg_api_client_v2-0.455.1/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-04 18:24:18.688734 stigg_api_client_v2-0.455.1/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-04 18:24:17.040776 stigg_api_client_v2-0.455.1/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-04 18:24:17.056710 stigg_api_client_v2-0.455.1/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-04 18:24:17.029202 stigg_api_client_v2-0.455.1/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-04 18:24:17.127131 stigg_api_client_v2-0.455.1/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-04 18:24:17.083970 stigg_api_client_v2-0.455.1/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-04 18:24:17.075087 stigg_api_client_v2-0.455.1/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-04 18:24:17.145489 stigg_api_client_v2-0.455.1/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-04 18:24:17.065205 stigg_api_client_v2-0.455.1/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-04 18:24:17.098387 stigg_api_client_v2-0.455.1/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-04 18:24:17.115650 stigg_api_client_v2-0.455.1/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-04 18:24:16.864204 stigg_api_client_v2-0.455.1/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-04 18:24:16.853174 stigg_api_client_v2-0.455.1/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-04 18:24:16.907506 stigg_api_client_v2-0.455.1/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0      550 2023-06-04 18:24:16.944200 stigg_api_client_v2-0.455.1/stigg/generated/initiate_checkout.py
--rw-r--r--   0        0        0   125103 2023-06-04 18:24:16.820439 stigg_api_client_v2-0.455.1/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-04 18:24:17.018208 stigg_api_client_v2-0.455.1/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-04 18:24:16.844291 stigg_api_client_v2-0.455.1/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-04 18:24:16.896951 stigg_api_client_v2-0.455.1/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-04 18:24:16.995717 stigg_api_client_v2-0.455.1/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      637 2023-06-04 18:24:16.987321 stigg_api_client_v2-0.455.1/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-04 18:24:18.698552 stigg_api_client_v2-0.455.1/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-04 18:24:16.875655 stigg_api_client_v2-0.455.1/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-04 18:24:16.919309 stigg_api_client_v2-0.455.1/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-04 18:24:17.171712 stigg_api_client_v2-0.455.1/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.455.1/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-05 15:28:34.592325 stigg_api_client_v2-0.457.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/stigg/client.py
+-rw-r--r--   0        0        0    39450 2023-06-05 15:28:33.020334 stigg_api_client_v2-0.457.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-05 15:28:31.772341 stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-05 15:28:31.796341 stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    69448 2023-06-05 15:28:32.808335 stigg_api_client_v2-0.457.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-05 15:28:31.816341 stigg_api_client_v2-0.457.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-05 15:28:31.896340 stigg_api_client_v2-0.457.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23614 2023-06-05 15:28:29.668351 stigg_api_client_v2-0.457.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-05 15:28:31.788341 stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-05 15:28:31.792341 stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53088 2023-06-05 15:28:32.520337 stigg_api_client_v2-0.457.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-05 15:28:31.836340 stigg_api_client_v2-0.457.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-05 15:28:31.844340 stigg_api_client_v2-0.457.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-05 15:28:31.828340 stigg_api_client_v2-0.457.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-05 15:28:31.884340 stigg_api_client_v2-0.457.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-05 15:28:31.860340 stigg_api_client_v2-0.457.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-05 15:28:31.856340 stigg_api_client_v2-0.457.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-05 15:28:31.892340 stigg_api_client_v2-0.457.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-05 15:28:31.848340 stigg_api_client_v2-0.457.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-05 15:28:31.868340 stigg_api_client_v2-0.457.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-05 15:28:31.876340 stigg_api_client_v2-0.457.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-05 15:28:31.740341 stigg_api_client_v2-0.457.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-05 15:28:31.736341 stigg_api_client_v2-0.457.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-05 15:28:31.760341 stigg_api_client_v2-0.457.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0      550 2023-06-05 15:28:31.780341 stigg_api_client_v2-0.457.0/stigg/generated/initiate_checkout.py
+-rw-r--r--   0        0        0   125804 2023-06-05 15:28:31.720341 stigg_api_client_v2-0.457.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-05 15:28:31.824340 stigg_api_client_v2-0.457.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-05 15:28:31.732341 stigg_api_client_v2-0.457.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-05 15:28:31.756341 stigg_api_client_v2-0.457.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-05 15:28:31.812340 stigg_api_client_v2-0.457.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      637 2023-06-05 15:28:31.808340 stigg_api_client_v2-0.457.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-05 15:28:32.608336 stigg_api_client_v2-0.457.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-05 15:28:31.748341 stigg_api_client_v2-0.457.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-05 15:28:31.768341 stigg_api_client_v2-0.457.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      451 2023-06-05 15:28:31.904340 stigg_api_client_v2-0.457.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.457.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.455.1/README.md` & `stigg_api_client_v2-0.457.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.455.1/pyproject.toml` & `stigg_api_client_v2-0.457.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.455.1"
+version = "0.457.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ariadne-codegen = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0"
 black = "^22.8"
+ariadne-codegen = "^0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ariadne-codegen]
 schema_path = "../api-client-schema/src/generated/schema.graphql"
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/__init__.py` & `stigg_api_client_v2-0.457.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -335,14 +335,15 @@
     AddonUpdateInput,
     Address,
     ApiKeyFilter,
     ApiKeySort,
     ArchiveCouponInput,
     ArchivePlanInput,
     AttachCustomerPaymentMethodInput,
+    BillableFeatureInput,
     BillingModelFilterComparison,
     BillingPeriodFilterComparison,
     BooleanFieldComparison,
     CheckoutOptions,
     ClearCustomerPersistentCacheInput,
     CouponFilter,
     CouponFilterCustomerFilter,
@@ -623,14 +624,15 @@
     "ApiKeySortFields",
     "ApiKeyType",
     "ArchiveCouponInput",
     "ArchivePlanInput",
     "AsyncBaseClient",
     "AttachCustomerPaymentMethodInput",
     "BaseModel",
+    "BillableFeatureInput",
     "BillingAnchor",
     "BillingModel",
     "BillingModelFilterComparison",
     "BillingPeriod",
     "BillingPeriodFilterComparison",
     "BooleanFieldComparison",
     "CancelSubscription",
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.457.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/base_model.py` & `stigg_api_client_v2-0.457.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/client.py` & `stigg_api_client_v2-0.457.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.457.0/stigg/generated/create_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.457.0/stigg/generated/entitlements_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/enums.py` & `stigg_api_client_v2-0.457.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.457.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/fragments.py` & `stigg_api_client_v2-0.457.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,25 +124,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -157,14 +146,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,14 +328,27 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -462,27 +475,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -568,29 +568,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -655,14 +640,29 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1279,17 +1279,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1303,14 +1303,16 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
@@ -1320,42 +1322,40 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_active_subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_customer_by_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_products.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.457.0/stigg/generated/get_sdk_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/initiate_checkout.py` & `stigg_api_client_v2-0.457.0/stigg/generated/initiate_checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/input_types.py` & `stigg_api_client_v2-0.457.0/stigg/generated/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -165,14 +165,19 @@
     customer_id: Optional[str] = Field(alias="customerId")
     environment_id: Optional[str] = Field(alias="environmentId")
     payment_method_id: str = Field(alias="paymentMethodId")
     ref_id: Optional[str] = Field(alias="refId")
     vendor_identifier: VendorIdentifier = Field(alias="vendorIdentifier")
 
 
+class BillableFeatureInput(BaseModel):
+    feature_id: str = Field(alias="featureId")
+    quantity: float
+
+
 class BillingModelFilterComparison(BaseModel):
     eq: Optional[BillingModel]
     gt: Optional[BillingModel]
     gte: Optional[BillingModel]
     i_like: Optional[BillingModel] = Field(alias="iLike")
     in_: Optional[List[BillingModel]] = Field(alias="in")
     is_: Optional[bool] = Field(alias="is")
@@ -1841,14 +1846,17 @@
 
 class ProvisionCustomerSubscriptionInput(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
     await_payment_confirmation: Optional[bool] = Field(
         alias="awaitPaymentConfirmation", default=False
     )
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_id: Optional[str] = Field(alias="billingId")
     billing_information: Optional["SubscriptionBillingInfo"] = Field(
         alias="billingInformation"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     plan_id: str = Field(alias="planId")
@@ -1868,14 +1876,17 @@
 
 class ProvisionSubscription(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
     await_payment_confirmation: Optional[bool] = Field(
         alias="awaitPaymentConfirmation", default=False
     )
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_id: Optional[str] = Field(alias="billingId")
     billing_information: Optional["SubscriptionBillingInfo"] = Field(
         alias="billingInformation"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     checkout_options: Optional["CheckoutOptions"] = Field(alias="checkoutOptions")
@@ -1893,14 +1904,17 @@
 
 class ProvisionSubscriptionInput(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
     await_payment_confirmation: Optional[bool] = Field(
         alias="awaitPaymentConfirmation", default=False
     )
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_id: Optional[str] = Field(alias="billingId")
     billing_information: Optional["SubscriptionBillingInfo"] = Field(
         alias="billingInformation"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     checkout_options: Optional["CheckoutOptions"] = Field(alias="checkoutOptions")
@@ -2233,14 +2247,17 @@
 
 class SubscriptionInput(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
     await_payment_confirmation: Optional[bool] = Field(
         alias="awaitPaymentConfirmation", default=False
     )
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_id: Optional[str] = Field(alias="billingId")
     billing_information: Optional["SubscriptionBillingInfo"] = Field(
         alias="billingInformation"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     crm_id: Optional[str] = Field(alias="crmId")
@@ -2580,14 +2597,17 @@
         alias="weeklyResetPeriodConfiguration"
     )
 
 
 class UpdateSubscriptionInput(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     environment_id: Optional[str] = Field(alias="environmentId")
     promotion_code: Optional[str] = Field(alias="promotionCode")
     ref_id: Optional[str] = Field(alias="refId")
     subscription_entitlements: Optional[
         List["UpdateSubscriptionEntitlementInput"]
     ] = Field(alias="subscriptionEntitlements")
@@ -2741,14 +2761,15 @@
 AddonUpdateInput.update_forward_refs()
 Address.update_forward_refs()
 ApiKeyFilter.update_forward_refs()
 ApiKeySort.update_forward_refs()
 ArchiveCouponInput.update_forward_refs()
 ArchivePlanInput.update_forward_refs()
 AttachCustomerPaymentMethodInput.update_forward_refs()
+BillableFeatureInput.update_forward_refs()
 BillingModelFilterComparison.update_forward_refs()
 BillingPeriodFilterComparison.update_forward_refs()
 BooleanFieldComparison.update_forward_refs()
 CheckoutOptions.update_forward_refs()
 ClearCustomerPersistentCacheInput.update_forward_refs()
 CouponFilter.update_forward_refs()
 CouponFilterCustomerFilter.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.457.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.457.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.457.0/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.457.0/stigg/generated/report_usage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.455.1/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.457.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-04 21:24
+# Generated by ariadne-codegen on 2023-06-05 15:28
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.455.1/PKG-INFO` & `stigg_api_client_v2-0.457.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.455.1
+Version: 0.457.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ariadne-codegen (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # stigg-api-client-v2 (BETA)
 
 This library provides a Python wrapper to [Stigg's GraphQL API](https://docs.stigg.io/docs/graphql-api) based on 
 the operations that are in use by the [Stigg's Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).
```

