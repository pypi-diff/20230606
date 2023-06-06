# Comparing `tmp/stigg_api_client_v2-0.457.0.tar.gz` & `tmp/stigg_api_client_v2-0.458.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.457.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.458.4.tar", max compression
```

## Comparing `stigg_api_client_v2-0.457.0.tar` & `stigg_api_client_v2-0.458.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1644 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/README.md
--rw-r--r--   0        0        0      653 2023-06-05 15:28:34.592325 stigg_api_client_v2-0.457.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-05 15:27:57.152520 stigg_api_client_v2-0.457.0/stigg/client.py
--rw-r--r--   0        0        0    39450 2023-06-05 15:28:33.020334 stigg_api_client_v2-0.457.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-05 15:28:31.772341 stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-05 15:28:31.796341 stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    69448 2023-06-05 15:28:32.808335 stigg_api_client_v2-0.457.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-05 15:28:31.816341 stigg_api_client_v2-0.457.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-05 15:28:31.896340 stigg_api_client_v2-0.457.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23614 2023-06-05 15:28:29.668351 stigg_api_client_v2-0.457.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-05 15:28:31.788341 stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-05 15:28:31.792341 stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-05 15:28:32.524337 stigg_api_client_v2-0.457.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-05 15:28:32.520337 stigg_api_client_v2-0.457.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-05 15:28:31.836340 stigg_api_client_v2-0.457.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-05 15:28:31.844340 stigg_api_client_v2-0.457.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-05 15:28:31.828340 stigg_api_client_v2-0.457.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-05 15:28:31.884340 stigg_api_client_v2-0.457.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-05 15:28:31.860340 stigg_api_client_v2-0.457.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-05 15:28:31.856340 stigg_api_client_v2-0.457.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-05 15:28:31.892340 stigg_api_client_v2-0.457.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-05 15:28:31.848340 stigg_api_client_v2-0.457.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-05 15:28:31.868340 stigg_api_client_v2-0.457.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-05 15:28:31.876340 stigg_api_client_v2-0.457.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-05 15:28:31.740341 stigg_api_client_v2-0.457.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-05 15:28:31.736341 stigg_api_client_v2-0.457.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-05 15:28:31.760341 stigg_api_client_v2-0.457.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0      550 2023-06-05 15:28:31.780341 stigg_api_client_v2-0.457.0/stigg/generated/initiate_checkout.py
--rw-r--r--   0        0        0   125804 2023-06-05 15:28:31.720341 stigg_api_client_v2-0.457.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-05 15:28:31.824340 stigg_api_client_v2-0.457.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-05 15:28:31.732341 stigg_api_client_v2-0.457.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-05 15:28:31.756341 stigg_api_client_v2-0.457.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-05 15:28:31.812340 stigg_api_client_v2-0.457.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      637 2023-06-05 15:28:31.808340 stigg_api_client_v2-0.457.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-05 15:28:32.608336 stigg_api_client_v2-0.457.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-05 15:28:31.748341 stigg_api_client_v2-0.457.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-05 15:28:31.768341 stigg_api_client_v2-0.457.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-05 15:28:31.904340 stigg_api_client_v2-0.457.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.457.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-06 10:25:41.448505 stigg_api_client_v2-0.458.4/README.md
+-rw-r--r--   0        0        0      653 2023-06-06 10:26:30.525655 stigg_api_client_v2-0.458.4/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-06 10:25:41.448505 stigg_api_client_v2-0.458.4/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-06 10:25:41.448505 stigg_api_client_v2-0.458.4/stigg/client.py
+-rw-r--r--   0        0        0    39450 2023-06-06 10:26:28.465605 stigg_api_client_v2-0.458.4/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-06 10:26:27.989592 stigg_api_client_v2-0.458.4/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-06 10:26:27.989592 stigg_api_client_v2-0.458.4/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-06 10:26:26.873563 stigg_api_client_v2-0.458.4/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-06 10:26:26.901564 stigg_api_client_v2-0.458.4/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    69448 2023-06-06 10:26:28.269600 stigg_api_client_v2-0.458.4/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-06 10:26:26.929565 stigg_api_client_v2-0.458.4/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-06 10:26:27.029567 stigg_api_client_v2-0.458.4/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23614 2023-06-06 10:26:23.941487 stigg_api_client_v2-0.458.4/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-06 10:26:26.889564 stigg_api_client_v2-0.458.4/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-06 10:26:26.897564 stigg_api_client_v2-0.458.4/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-06 10:26:27.989592 stigg_api_client_v2-0.458.4/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53088 2023-06-06 10:26:27.985592 stigg_api_client_v2-0.458.4/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-06 10:26:26.953565 stigg_api_client_v2-0.458.4/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-06 10:26:26.965566 stigg_api_client_v2-0.458.4/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-06 10:26:26.945565 stigg_api_client_v2-0.458.4/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-06 10:26:27.013567 stigg_api_client_v2-0.458.4/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-06 10:26:26.981566 stigg_api_client_v2-0.458.4/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-06 10:26:26.977566 stigg_api_client_v2-0.458.4/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-06 10:26:27.021567 stigg_api_client_v2-0.458.4/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-06 10:26:26.969566 stigg_api_client_v2-0.458.4/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-06 10:26:26.993566 stigg_api_client_v2-0.458.4/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-06 10:26:27.005567 stigg_api_client_v2-0.458.4/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-06 10:26:26.833562 stigg_api_client_v2-0.458.4/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-06 10:26:26.825562 stigg_api_client_v2-0.458.4/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-06 10:26:26.857563 stigg_api_client_v2-0.458.4/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0      550 2023-06-06 10:26:26.881563 stigg_api_client_v2-0.458.4/stigg/generated/initiate_checkout.py
+-rw-r--r--   0        0        0   125804 2023-06-06 10:26:26.805561 stigg_api_client_v2-0.458.4/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-06 10:26:26.937565 stigg_api_client_v2-0.458.4/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-06 10:26:26.817562 stigg_api_client_v2-0.458.4/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-06 10:26:26.853563 stigg_api_client_v2-0.458.4/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-06 10:26:26.921564 stigg_api_client_v2-0.458.4/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      637 2023-06-06 10:26:26.917564 stigg_api_client_v2-0.458.4/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-06 10:26:27.993592 stigg_api_client_v2-0.458.4/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-06 10:26:26.841562 stigg_api_client_v2-0.458.4/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-06 10:26:26.865563 stigg_api_client_v2-0.458.4/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      451 2023-06-06 10:26:27.037567 stigg_api_client_v2-0.458.4/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.458.4/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.457.0/README.md` & `stigg_api_client_v2-0.458.4/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.457.0/pyproject.toml` & `stigg_api_client_v2-0.458.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.457.0"
+version = "0.458.4"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.458.4/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.458.4/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.458.4/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.458.4/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/client.py` & `stigg_api_client_v2-0.458.4/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.458.4/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.458.4/stigg/generated/entitlements_updated.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.458.4/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.458.4/stigg/generated/estimate_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.458.4/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.458.4/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.458.4/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -55,36 +77,14 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -124,14 +124,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
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
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -146,25 +157,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
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
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,25 +328,32 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -392,21 +399,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -813,34 +813,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -855,14 +835,34 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1268,28 +1268,28 @@
 
 
 class SubscriptionPreviewFragmentProrationNetAmount(BaseModel):
     amount: float
     currency: Currency
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1303,22 +1303,22 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
@@ -1371,19 +1371,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_active_subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_mock_paywall.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.458.4/stigg/generated/get_sdk_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/initiate_checkout.py` & `stigg_api_client_v2-0.458.4/stigg/generated/initiate_checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.458.4/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.458.4/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.458.4/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.458.4/stigg/generated/provision_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.458.4/stigg/generated/report_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.457.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.458.4/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-05 15:28
+# Generated by ariadne-codegen on 2023-06-06 10:26
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.457.0/PKG-INFO` & `stigg_api_client_v2-0.458.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.457.0
+Version: 0.458.4
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

