# Comparing `tmp/stigg_api_client_v2-0.491.9.tar.gz` & `tmp/stigg_api_client_v2-0.492.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.491.9.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.492.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.491.9.tar` & `stigg_api_client_v2-0.492.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-18 13:54:32.528784 stigg_api_client_v2-0.491.9/README.md
--rw-r--r--   0        0        0      432 2023-07-18 13:55:19.025778 stigg_api_client_v2-0.491.9/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-18 13:54:32.528784 stigg_api_client_v2-0.491.9/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-18 13:54:32.528784 stigg_api_client_v2-0.491.9/stigg/client.py
--rw-r--r--   0        0        0    40220 2023-07-18 13:55:17.325745 stigg_api_client_v2-0.491.9/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-18 13:55:15.909717 stigg_api_client_v2-0.491.9/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-18 13:55:16.817735 stigg_api_client_v2-0.491.9/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68230 2023-07-18 13:55:17.037739 stigg_api_client_v2-0.491.9/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-18 13:55:11.493627 stigg_api_client_v2-0.491.9/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-18 13:55:16.817735 stigg_api_client_v2-0.491.9/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-18 13:55:15.853716 stigg_api_client_v2-0.491.9/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-18 13:55:15.869716 stigg_api_client_v2-0.491.9/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67803 2023-07-18 13:55:11.721632 stigg_api_client_v2-0.491.9/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-18 13:55:15.893717 stigg_api_client_v2-0.491.9/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24352 2023-07-18 13:55:13.461668 stigg_api_client_v2-0.491.9/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-18 13:55:15.857716 stigg_api_client_v2-0.491.9/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-18 13:55:15.865716 stigg_api_client_v2-0.491.9/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-18 13:55:16.817735 stigg_api_client_v2-0.491.9/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56292 2023-07-18 13:55:16.817735 stigg_api_client_v2-0.491.9/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-18 13:55:15.921717 stigg_api_client_v2-0.491.9/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-18 13:55:15.929718 stigg_api_client_v2-0.491.9/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-18 13:55:15.913717 stigg_api_client_v2-0.491.9/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-18 13:55:15.969718 stigg_api_client_v2-0.491.9/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-18 13:55:15.945718 stigg_api_client_v2-0.491.9/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-18 13:55:15.941718 stigg_api_client_v2-0.491.9/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-18 13:55:15.977718 stigg_api_client_v2-0.491.9/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-18 13:55:15.933718 stigg_api_client_v2-0.491.9/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-18 13:55:15.953718 stigg_api_client_v2-0.491.9/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-18 13:55:15.961718 stigg_api_client_v2-0.491.9/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-18 13:55:15.817715 stigg_api_client_v2-0.491.9/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-18 13:55:15.813715 stigg_api_client_v2-0.491.9/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-18 13:55:15.841716 stigg_api_client_v2-0.491.9/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126904 2023-07-18 13:55:15.797715 stigg_api_client_v2-0.491.9/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-18 13:55:15.901717 stigg_api_client_v2-0.491.9/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-18 13:55:15.809715 stigg_api_client_v2-0.491.9/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-18 13:55:15.833716 stigg_api_client_v2-0.491.9/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-18 13:55:15.889717 stigg_api_client_v2-0.491.9/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-18 13:55:15.885717 stigg_api_client_v2-0.491.9/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-18 13:55:15.877716 stigg_api_client_v2-0.491.9/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-18 13:55:16.825735 stigg_api_client_v2-0.491.9/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-18 13:55:15.825715 stigg_api_client_v2-0.491.9/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-18 13:55:15.845716 stigg_api_client_v2-0.491.9/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-18 13:55:15.981719 stigg_api_client_v2-0.491.9/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.491.9/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-19 06:15:26.580399 stigg_api_client_v2-0.492.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-19 06:16:41.112405 stigg_api_client_v2-0.492.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-19 06:15:26.580399 stigg_api_client_v2-0.492.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-19 06:15:26.580399 stigg_api_client_v2-0.492.0/stigg/client.py
+-rw-r--r--   0        0        0    40056 2023-07-19 06:16:38.796407 stigg_api_client_v2-0.492.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-19 06:16:36.808408 stigg_api_client_v2-0.492.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-19 06:16:38.112407 stigg_api_client_v2-0.492.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68230 2023-07-19 06:16:38.436407 stigg_api_client_v2-0.492.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-19 06:16:30.656409 stigg_api_client_v2-0.492.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-19 06:16:38.112407 stigg_api_client_v2-0.492.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-19 06:16:36.728408 stigg_api_client_v2-0.492.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-19 06:16:36.752408 stigg_api_client_v2-0.492.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67803 2023-07-19 06:16:30.960409 stigg_api_client_v2-0.492.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-19 06:16:36.788408 stigg_api_client_v2-0.492.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24102 2023-07-19 06:16:33.292410 stigg_api_client_v2-0.492.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-19 06:16:36.736408 stigg_api_client_v2-0.492.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-19 06:16:36.744408 stigg_api_client_v2-0.492.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-19 06:16:38.112407 stigg_api_client_v2-0.492.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56292 2023-07-19 06:16:38.108407 stigg_api_client_v2-0.492.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-19 06:16:36.840408 stigg_api_client_v2-0.492.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-19 06:16:36.852408 stigg_api_client_v2-0.492.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-19 06:16:36.820408 stigg_api_client_v2-0.492.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-19 06:16:36.904408 stigg_api_client_v2-0.492.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-19 06:16:36.872408 stigg_api_client_v2-0.492.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-19 06:16:36.864408 stigg_api_client_v2-0.492.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-19 06:16:36.920408 stigg_api_client_v2-0.492.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-19 06:16:36.856408 stigg_api_client_v2-0.492.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-19 06:16:36.888408 stigg_api_client_v2-0.492.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-19 06:16:36.896408 stigg_api_client_v2-0.492.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-19 06:16:36.680408 stigg_api_client_v2-0.492.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-19 06:16:36.668408 stigg_api_client_v2-0.492.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-19 06:16:36.708408 stigg_api_client_v2-0.492.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126054 2023-07-19 06:16:36.648408 stigg_api_client_v2-0.492.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-19 06:16:36.800408 stigg_api_client_v2-0.492.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-19 06:16:36.664408 stigg_api_client_v2-0.492.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-19 06:16:36.700408 stigg_api_client_v2-0.492.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-19 06:16:36.780408 stigg_api_client_v2-0.492.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-19 06:16:36.772408 stigg_api_client_v2-0.492.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-19 06:16:36.764408 stigg_api_client_v2-0.492.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-19 06:16:38.120407 stigg_api_client_v2-0.492.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-19 06:16:36.688408 stigg_api_client_v2-0.492.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-19 06:16:36.716408 stigg_api_client_v2-0.492.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-19 06:16:36.928408 stigg_api_client_v2-0.492.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.492.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.491.9/README.md` & `stigg_api_client_v2-0.492.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.491.9/stigg/client.py` & `stigg_api_client_v2-0.492.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/__init__.py` & `stigg_api_client_v2-0.492.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
@@ -50,15 +50,14 @@
     FontWeight,
     HookSortFields,
     HookStatus,
     ImportIntegrationTaskSortFields,
     IntegrationSortFields,
     MemberSortFields,
     MemberStatus,
-    MeterSortFields,
     MeterType,
     MonthlyAccordingTo,
     PackageDTOSortFields,
     PackageEntitlementSortFields,
     PackageStatus,
     PaymentMethodType,
     PlanSortFields,
@@ -365,15 +364,14 @@
     CreateManyPackageEntitlementsInput,
     CreateManyPromotionalEntitlementsInput,
     CreateMeter,
     CreateOneEnvironmentInput,
     CreateOneFeatureInput,
     CreateOneHookInput,
     CreateOneIntegrationInput,
-    CreateOneMeterInput,
     CreateOneProductInput,
     CursorPaging,
     CustomerBillingInfo,
     CustomerFilter,
     CustomerFilterCustomerSubscriptionFilter,
     CustomerFilterPromotionalEntitlementFilter,
     CustomerInput,
@@ -449,17 +447,15 @@
     IntegrationSort,
     IntFieldComparison,
     IntFieldComparisonBetween,
     MemberFilter,
     MemberSort,
     MeterAggregation,
     MeterConditionInput,
-    MeterFilter,
     MeterFilterDefinitionInput,
-    MeterSort,
     MeterTypeFilterComparison,
     MoneyInputDTO,
     MonthlyResetPeriodConfigInput,
     NumberFieldComparison,
     NumberFieldComparisonBetween,
     PackageDTOFilter,
     PackageDTOSort,
@@ -673,15 +669,14 @@
     "CreateManyPackageEntitlementsInput",
     "CreateManyPromotionalEntitlementsInput",
     "CreateMeter",
     "CreateOneEnvironmentInput",
     "CreateOneFeatureInput",
     "CreateOneHookInput",
     "CreateOneIntegrationInput",
-    "CreateOneMeterInput",
     "CreateOneProductInput",
     "CreateSubscription",
     "CreateSubscriptionCreateSubscription",
     "Currency",
     "CursorPaging",
     "CustomerBillingInfo",
     "CustomerFilter",
@@ -881,18 +876,15 @@
     "LayoutConfigurationFragment",
     "MemberFilter",
     "MemberSort",
     "MemberSortFields",
     "MemberStatus",
     "MeterAggregation",
     "MeterConditionInput",
-    "MeterFilter",
     "MeterFilterDefinitionInput",
-    "MeterSort",
-    "MeterSortFields",
     "MeterType",
     "MeterTypeFilterComparison",
     "MigrateSubscriptionToLatest",
     "MigrateSubscriptionToLatestMigrateSubscriptionToLatest",
     "MockPaywallAddonFragment",
     "MockPaywallAddonFragmentEntitlements",
     "MockPaywallAddonFragmentPrices",
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.492.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/async_client.py` & `stigg_api_client_v2-0.492.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/base_client.py` & `stigg_api_client_v2-0.492.0/stigg/generated/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/base_model.py` & `stigg_api_client_v2-0.492.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.492.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/client.py` & `stigg_api_client_v2-0.492.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.492.0/stigg/generated/create_subscription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/enums.py` & `stigg_api_client_v2-0.492.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -378,17 +378,14 @@
     InvalidMemberDelete = "InvalidMemberDelete"
     InvalidMetadataError = "InvalidMetadataError"
     InvalidQuantity = "InvalidQuantity"
     InvalidSubscriptionStatus = "InvalidSubscriptionStatus"
     InvalidUpdatePriceUnitAmountError = "InvalidUpdatePriceUnitAmountError"
     MemberInvitationError = "MemberInvitationError"
     MemberNotFound = "MemberNotFound"
-    MeterDoesNotBelongToTheEntitlementFeature = (
-        "MeterDoesNotBelongToTheEntitlementFeature"
-    )
     MeterMustBeAssociatedToMeteredFeature = "MeterMustBeAssociatedToMeteredFeature"
     MeteringNotAvailableForFeatureType = "MeteringNotAvailableForFeatureType"
     MissingEntityIdError = "MissingEntityIdError"
     NoFeatureEntitlementInSubscription = "NoFeatureEntitlementInSubscription"
     NoProductsAvailable = "NoProductsAvailable"
     OperationNotAllowedDuringInProgressExperiment = (
         "OperationNotAllowedDuringInProgressExperiment"
@@ -571,21 +568,14 @@
 
 
 class MemberStatus(str, Enum):
     INVITED = "INVITED"
     REGISTERED = "REGISTERED"
 
 
-class MeterSortFields(str, Enum):
-    createdAt = "createdAt"
-    environmentId = "environmentId"
-    id = "id"
-    updatedAt = "updatedAt"
-
-
 class MeterType(str, Enum):
     FLUCTUATING = "Fluctuating"
     INCREMENTAL = "Incremental"
     NONE = "None"
 
 
 class MonthlyAccordingTo(str, Enum):
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.492.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.492.0/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.492.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/fragments.py` & `stigg_api_client_v2-0.492.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
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
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -78,14 +56,36 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
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
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -125,25 +125,14 @@
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
@@ -158,14 +147,25 @@
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
@@ -329,21 +329,19 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
     display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -390,21 +388,14 @@
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
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -506,14 +497,23 @@
     pass
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,14 +548,80 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
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
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -620,80 +686,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
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
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1341,28 +1341,28 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
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
@@ -1376,21 +1376,20 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
@@ -1399,40 +1398,41 @@
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
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
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_active_subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_products.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_products.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.492.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/input_types.py` & `stigg_api_client_v2-0.492.0/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -36,15 +36,14 @@
     FeatureType,
     FontWeight,
     HookSortFields,
     HookStatus,
     ImportIntegrationTaskSortFields,
     IntegrationSortFields,
     MemberSortFields,
-    MeterSortFields,
     MeterType,
     MonthlyAccordingTo,
     PackageDTOSortFields,
     PackageEntitlementSortFields,
     PackageStatus,
     PlanSortFields,
     PriceSortFields,
@@ -393,16 +392,14 @@
     promotional_entitlements: List["PromotionalEntitlementInput"] = Field(
         alias="promotionalEntitlements"
     )
 
 
 class CreateMeter(BaseModel):
     aggregation: "MeterAggregation"
-    environment_id: str = Field(alias="environmentId")
-    feature_id: str = Field(alias="featureId")
     filters: List["MeterFilterDefinitionInput"]
 
 
 class CreateOneEnvironmentInput(BaseModel):
     environment: "CreateEnvironment"
     options: Optional["CreateEnvironmentOptions"]
 
@@ -415,18 +412,14 @@
     hook: "CreateHook"
 
 
 class CreateOneIntegrationInput(BaseModel):
     integration: "CreateIntegrationInput"
 
 
-class CreateOneMeterInput(BaseModel):
-    meter: "CreateMeter"
-
-
 class CreateOneProductInput(BaseModel):
     product: "ProductCreateInput"
 
 
 class CursorPaging(BaseModel):
     after: Optional[Any]
     before: Optional[Any]
@@ -1017,14 +1010,15 @@
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     environment_id: str = Field(alias="environmentId")
     feature_status: Optional[FeatureStatus] = Field(alias="featureStatus")
     feature_type: FeatureType = Field(alias="featureType")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    meter: Optional["CreateMeter"]
     meter_type: Optional[MeterType] = Field(alias="meterType")
     ref_id: str = Field(alias="refId")
 
 
 class FeatureSort(BaseModel):
     direction: SortDirection
     field: FeatureSortFields
@@ -1292,36 +1286,21 @@
     field: Optional[str]
     function: AggregationFunction
 
 
 class MeterConditionInput(BaseModel):
     field: str
     operation: ConditionOperation
-    value: str
-
-
-class MeterFilter(BaseModel):
-    and_: Optional[List["MeterFilter"]] = Field(alias="and")
-    created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
-    environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
-    id: Optional["StringFieldComparison"]
-    or_: Optional[List["MeterFilter"]] = Field(alias="or")
-    updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
+    value: Optional[str]
 
 
 class MeterFilterDefinitionInput(BaseModel):
     conditions: List["MeterConditionInput"]
 
 
-class MeterSort(BaseModel):
-    direction: SortDirection
-    field: MeterSortFields
-    nulls: Optional[SortNulls]
-
-
 class MeterTypeFilterComparison(BaseModel):
     eq: Optional[MeterType]
     gt: Optional[MeterType]
     gte: Optional[MeterType]
     i_like: Optional[MeterType] = Field(alias="iLike")
     in_: Optional[List[MeterType]] = Field(alias="in")
     is_: Optional[bool] = Field(alias="is")
@@ -1441,15 +1420,14 @@
     description: Optional[str]
     display_name_override: Optional[str] = Field(alias="displayNameOverride")
     environment_id: str = Field(alias="environmentId")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
     is_custom: Optional[bool] = Field(alias="isCustom")
-    meter_id: Optional[str] = Field(alias="meterId")
     monthly_reset_period_configuration: Optional[
         "MonthlyResetPeriodConfigInput"
     ] = Field(alias="monthlyResetPeriodConfiguration")
     order: Optional[float]
     package_id: str = Field(alias="packageId")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     usage_limit: Optional[float] = Field(alias="usageLimit")
@@ -2806,15 +2784,14 @@
 CreateManyPackageEntitlementsInput.update_forward_refs()
 CreateManyPromotionalEntitlementsInput.update_forward_refs()
 CreateMeter.update_forward_refs()
 CreateOneEnvironmentInput.update_forward_refs()
 CreateOneFeatureInput.update_forward_refs()
 CreateOneHookInput.update_forward_refs()
 CreateOneIntegrationInput.update_forward_refs()
-CreateOneMeterInput.update_forward_refs()
 CreateOneProductInput.update_forward_refs()
 CursorPaging.update_forward_refs()
 CustomerBillingInfo.update_forward_refs()
 CustomerFilter.update_forward_refs()
 CustomerFilterCustomerSubscriptionFilter.update_forward_refs()
 CustomerFilterPromotionalEntitlementFilter.update_forward_refs()
 CustomerInput.update_forward_refs()
@@ -2890,17 +2867,15 @@
 IntFieldComparisonBetween.update_forward_refs()
 IntegrationFilter.update_forward_refs()
 IntegrationSort.update_forward_refs()
 MemberFilter.update_forward_refs()
 MemberSort.update_forward_refs()
 MeterAggregation.update_forward_refs()
 MeterConditionInput.update_forward_refs()
-MeterFilter.update_forward_refs()
 MeterFilterDefinitionInput.update_forward_refs()
-MeterSort.update_forward_refs()
 MeterTypeFilterComparison.update_forward_refs()
 MoneyInputDTO.update_forward_refs()
 MonthlyResetPeriodConfigInput.update_forward_refs()
 NumberFieldComparison.update_forward_refs()
 NumberFieldComparisonBetween.update_forward_refs()
 PackageDTOFilter.update_forward_refs()
 PackageDTOSort.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.492.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.492.0/stigg/generated/provision_customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.492.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.492.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.9/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.492.0/stigg/generated/update_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-18 13:55
+# Generated by ariadne-codegen on 2023-07-19 06:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.9/PKG-INFO` & `stigg_api_client_v2-0.492.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.491.9
+Version: 0.492.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

