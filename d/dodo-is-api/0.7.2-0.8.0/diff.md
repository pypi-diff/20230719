# Comparing `tmp/dodo_is_api-0.7.2.tar.gz` & `tmp/dodo_is_api-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.7.2.tar", max compression
+gzip compressed data, was "dodo_is_api-0.8.0.tar", max compression
```

## Comparing `dodo_is_api-0.7.2.tar` & `dodo_is_api-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.7.2/LICENSE
--rw-r--r--   0        0        0     2689 2023-06-11 19:00:32.393182 dodo_is_api-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.7.2/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.7.2/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0    16088 2023-06-11 18:35:09.363455 dodo_is_api-0.7.2/dodo_is_api/connection/asynchronous.py
--rw-r--r--   0        0        0     3160 2023-06-12 05:17:25.385543 dodo_is_api-0.7.2/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0    15937 2023-06-11 18:35:09.368594 dodo_is_api-0.7.2/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.7.2/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0      583 2023-06-11 08:10:22.290413 dodo_is_api-0.7.2/dodo_is_api/logger.py
--rw-r--r--   0        0        0      419 2023-06-11 13:11:06.903175 dodo_is_api-0.7.2/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0      149 2023-06-11 08:39:51.057307 dodo_is_api-0.7.2/dodo_is_api/models/channel_stop_types.py
--rw-r--r--   0        0        0      349 2023-06-11 08:21:43.504521 dodo_is_api-0.7.2/dodo_is_api/models/country_codes.py
--rw-r--r--   0        0        0     1551 2023-06-11 20:17:46.220836 dodo_is_api-0.7.2/dodo_is_api/models/courier_orders.py
--rw-r--r--   0        0        0     1068 2023-06-11 20:17:46.212257 dodo_is_api-0.7.2/dodo_is_api/models/delivery_statistics.py
--rw-r--r--   0        0        0      174 2023-06-11 08:41:14.500495 dodo_is_api-0.7.2/dodo_is_api/models/delivery_transport_names.py
--rw-r--r--   0        0        0      860 2023-06-11 20:17:46.224929 dodo_is_api-0.7.2/dodo_is_api/models/late_delivery_vouchers.py
--rw-r--r--   0        0        0      308 2023-06-11 13:11:06.905522 dodo_is_api-0.7.2/dodo_is_api/models/order_sources.py
--rw-r--r--   0        0        0      647 2023-06-11 20:19:11.590789 dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_statistics.py
--rw-r--r--   0        0        0      869 2023-06-11 20:19:11.594036 dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_time.py
--rw-r--r--   0        0        0      781 2023-06-11 20:19:11.596459 dodo_is_api-0.7.2/dodo_is_api/models/production_productivity_statistics.py
--rw-r--r--   0        0        0      161 2023-06-11 08:37:28.682394 dodo_is_api-0.7.2/dodo_is_api/models/sales_channels.py
--rw-r--r--   0        0        0     1115 2023-06-11 20:19:11.598966 dodo_is_api-0.7.2/dodo_is_api/models/stop_sales.py
--rw-r--r--   0        0        0      582 2023-06-12 05:23:52.281457 dodo_is_api-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 dodo_is_api-0.7.2/setup.py
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 dodo_is_api-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2695 2023-07-19 13:29:07.937687 dodo_is_api-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.8.0/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.8.0/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0    17318 2023-07-19 13:15:20.606145 dodo_is_api-0.8.0/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     3160 2023-06-12 05:17:25.385543 dodo_is_api-0.8.0/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0    17155 2023-07-19 13:16:02.350971 dodo_is_api-0.8.0/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.8.0/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0      583 2023-06-11 08:10:22.290413 dodo_is_api-0.8.0/dodo_is_api/logger.py
+-rw-r--r--   0        0        0      419 2023-06-11 13:11:06.903175 dodo_is_api-0.8.0/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-11 08:39:51.057307 dodo_is_api-0.8.0/dodo_is_api/models/channel_stop_types.py
+-rw-r--r--   0        0        0      349 2023-06-11 08:21:43.504521 dodo_is_api-0.8.0/dodo_is_api/models/country_codes.py
+-rw-r--r--   0        0        0     1551 2023-06-11 20:17:46.220836 dodo_is_api-0.8.0/dodo_is_api/models/courier_orders.py
+-rw-r--r--   0        0        0     1068 2023-06-11 20:17:46.212257 dodo_is_api-0.8.0/dodo_is_api/models/delivery_statistics.py
+-rw-r--r--   0        0        0      174 2023-06-11 08:41:14.500495 dodo_is_api-0.8.0/dodo_is_api/models/delivery_transport_names.py
+-rw-r--r--   0        0        0      860 2023-06-11 20:17:46.224929 dodo_is_api-0.8.0/dodo_is_api/models/late_delivery_vouchers.py
+-rw-r--r--   0        0        0      308 2023-06-11 13:11:06.905522 dodo_is_api-0.8.0/dodo_is_api/models/order_sources.py
+-rw-r--r--   0        0        0      647 2023-06-11 20:19:11.590789 dodo_is_api-0.8.0/dodo_is_api/models/orders_handover_statistics.py
+-rw-r--r--   0        0        0      869 2023-06-11 20:19:11.594036 dodo_is_api-0.8.0/dodo_is_api/models/orders_handover_time.py
+-rw-r--r--   0        0        0      781 2023-06-11 20:19:11.596459 dodo_is_api-0.8.0/dodo_is_api/models/production_productivity_statistics.py
+-rw-r--r--   0        0        0      161 2023-06-11 08:37:28.682394 dodo_is_api-0.8.0/dodo_is_api/models/sales_channels.py
+-rw-r--r--   0        0        0     1440 2023-07-19 13:12:37.975763 dodo_is_api-0.8.0/dodo_is_api/models/stop_sales.py
+-rw-r--r--   0        0        0      582 2023-07-19 13:28:43.217231 dodo_is_api-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 dodo_is_api-0.8.0/setup.py
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 dodo_is_api-0.8.0/PKG-INFO
```

### Comparing `dodo_is_api-0.7.2/LICENSE` & `dodo_is_api-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/README.md` & `dodo_is_api-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     access_token = 'your access token'
     country_code = models.CountryCode.RU
 
     from_date = datetime(2004, 10, 7)
     to_date = datetime(2004, 10, 7, 23)
     units = [UUID('ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb')]
 
-    with httpx.AsyncClient() as http_client:
+    async with httpx.AsyncClient() as http_client:
         connection = AsyncDodoISAPIConnection(
             http_client=http_client,
             access_token=access_token,
             country_code=country_code,
         )
 
         stop_sales = await connection.get_stop_sales_by_products(
```

### Comparing `dodo_is_api-0.7.2/dodo_is_api/connection/asynchronous.py` & `dodo_is_api-0.8.0/dodo_is_api/connection/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,54 @@
         return parse_obj_as(
             list[models.StopSaleByProduct],
             response_data['stopSalesByProducts'],
         )
 
     # Delivery API
 
+    async def get_stop_sales_by_sectors(
+            self,
+            *,
+            from_date: datetime,
+            to_date: datetime,
+            units: Iterable[UUID],
+    ) -> list:
+        """Retrieve stop sales by sectors.
+
+        References:
+            Documentation: https://dodo-brands.stoplight.io/docs/dodo-is/3e817cbe2a17a-dostavka-stop-prodazhi-po-sektoram
+
+        Keyword Args:
+            from_date: start of period in ISO 8601 format.
+            to_date: end of period in ISO 8601 format.
+            units: collection of unit's UUIDs.
+
+        Returns:
+            List of stop sales by sectors.
+        """
+        url = f'{self.base_url}/delivery/stop-sales-sectors'
+        request_query_params = build_request_query_params(
+            from_date=from_date,
+            to_date=to_date,
+            unit_uuids=units,
+        )
+
+        response = await self._http_client.get(
+            url=url,
+            params=request_query_params,
+            headers=self.request_headers,
+        )
+        raise_for_status(response)
+
+        response_data: dict = response.json()
+        return parse_obj_as(
+            list[models.StopSaleBySector],
+            response_data['stopSalesBySectors'],
+        )
+
     async def iter_late_delivery_vouchers(
             self,
             *,
             from_date: datetime,
             to_date: datetime,
             units: Iterable[UUID],
             take: int = 1000,
```

### Comparing `dodo_is_api-0.7.2/dodo_is_api/connection/base.py` & `dodo_is_api-0.8.0/dodo_is_api/connection/base.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/connection/synchronous.py` & `dodo_is_api-0.8.0/dodo_is_api/connection/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,7 +517,47 @@
             to_date=to_date,
             units=units,
         )
         for batch_orders in iterator:
             couriers_orders += batch_orders
 
         return couriers_orders
+
+    def get_stop_sales_by_sectors(
+            self,
+            *,
+            from_date: datetime,
+            to_date: datetime,
+            units: Iterable[UUID],
+    ) -> list:
+        """Retrieve stop sales by sectors.
+
+        References:
+            Documentation: https://dodo-brands.stoplight.io/docs/dodo-is/3e817cbe2a17a-dostavka-stop-prodazhi-po-sektoram
+
+        Keyword Args:
+            from_date: start of period in ISO 8601 format.
+            to_date: end of period in ISO 8601 format.
+            units: collection of unit's UUIDs.
+
+        Returns:
+            List of stop sales by sectors.
+        """
+        url = f'{self.base_url}/delivery/stop-sales-sectors'
+        request_query_params = build_request_query_params(
+            from_date=from_date,
+            to_date=to_date,
+            unit_uuids=units,
+        )
+
+        response = self._http_client.get(
+            url=url,
+            params=request_query_params,
+            headers=self.request_headers,
+        )
+        raise_for_status(response)
+
+        response_data: dict = response.json()
+        return parse_obj_as(
+            list[models.StopSaleBySector],
+            response_data['stopSalesBySectors'],
+        )
```

### Comparing `dodo_is_api-0.7.2/dodo_is_api/logger.py` & `dodo_is_api-0.8.0/dodo_is_api/logger.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/courier_orders.py` & `dodo_is_api-0.8.0/dodo_is_api/models/courier_orders.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/delivery_statistics.py` & `dodo_is_api-0.8.0/dodo_is_api/models/delivery_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/late_delivery_vouchers.py` & `dodo_is_api-0.8.0/dodo_is_api/models/late_delivery_vouchers.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_statistics.py` & `dodo_is_api-0.8.0/dodo_is_api/models/orders_handover_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_time.py` & `dodo_is_api-0.8.0/dodo_is_api/models/orders_handover_time.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/production_productivity_statistics.py` & `dodo_is_api-0.8.0/dodo_is_api/models/production_productivity_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.2/dodo_is_api/models/stop_sales.py` & `dodo_is_api-0.8.0/dodo_is_api/models/stop_sales.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,35 +7,45 @@
 from .sales_channels import SalesChannel
 
 __all__ = (
     'StopSale',
     'StopSaleByProduct',
     'StopSaleByIngredient',
     'StopSaleBySalesChannel',
+    'StopSaleBySector',
 )
 
 
 class StopSale(BaseModel):
     id: UUID
     unit_uuid: UUID = Field(alias='unitId')
     unit_name: str = Field(alias='unitName')
-    reason: str
     started_at: datetime = Field(alias='startedAt')
     ended_at: datetime | None = Field(alias='endedAt')
     stopped_by_user_id: UUID = Field(alias='stoppedByUserId')
     resumed_by_user_id: UUID | None = Field(alias='resumedByUserId')
 
     class Config:
         allow_population_by_field_name = True
 
 
 class StopSaleBySalesChannel(StopSale):
+    reason: str
     sales_channel_name: SalesChannel = Field(alias='salesChannelName')
     channel_stop_type: ChannelStopType = Field(alias='channelStopType')
 
 
 class StopSaleByIngredient(StopSale):
+    reason: str
     ingredient_name: str = Field(alias='ingredientName')
 
 
 class StopSaleByProduct(StopSale):
+    reason: str
     product_name: str = Field(alias='productName')
+
+
+class StopSaleBySector(StopSale):
+    sector_name: str = Field(alias='sectorName')
+    is_sub_sector: bool = Field(alias='isSubSector')
+    stopped_by_user_id: UUID = Field(alias='suspendedByUserId')
+    resumed_by_user_id: UUID | None = Field(alias='resumedUserId')
```

### Comparing `dodo_is_api-0.7.2/pyproject.toml` & `dodo_is_api-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.7.2"
+version = "0.8.0"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dodo_is_api-0.7.2/setup.py` & `dodo_is_api-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['httpx>=0.23.3,<0.24.0',
  'pydantic>=1.10.9,<2.0.0',
  'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.7.2',
+    'version': '0.8.0',
     'description': '',
-    'long_description': '<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n🌩️ Synchronous version:\n\n```python\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.synchronous import DodoISAPIConnection\n\n\ndef main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.Client() as http_client:\n        connection = DodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    main()\n```\n\n⚡️ Asynchronous version:\n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync def main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.AsyncClient() as http_client:\n        connection = AsyncDodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = await connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```',
+    'long_description': '<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n🌩️ Synchronous version:\n\n```python\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.synchronous import DodoISAPIConnection\n\n\ndef main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.Client() as http_client:\n        connection = DodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    main()\n```\n\n⚡️ Asynchronous version:\n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync def main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    async with httpx.AsyncClient() as http_client:\n        connection = AsyncDodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = await connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0',
 'pydantic>=1.10.9,<2.0.0', 'structlog>=23.1.0,<24.0.0'] setup_kwargs =
-{ 'name': 'dodo-is-api', 'version': '0.7.2', 'description': '',
+{ 'name': 'dodo-is-api', 'version': '0.8.0', 'description': '',
 'long_description': '
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
 \n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-
 api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n####
@@ -26,16 +26,16 @@
 \'__main__\':\n main()\n```\n\nâ¡ï¸ Asynchronous version:
 \n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import
 UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom
 dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync
 def main():\n access_token = \'your access token\'\n country_code =
 models.CountryCode.RU\n\n from_date = datetime(2004, 10, 7)\n to_date =
 datetime(2004, 10, 7, 23)\n units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-
-7ae7d0c4e0bb\')]\n\n with httpx.AsyncClient() as http_client:\n connection =
-AsyncDodoISAPIConnection(\n http_client=http_client,\n
+7ae7d0c4e0bb\')]\n\n async with httpx.AsyncClient() as http_client:\n
+connection = AsyncDodoISAPIConnection(\n http_client=http_client,\n
 access_token=access_token,\n country_code=country_code,\n )\n\n stop_sales =
 await connection.get_stop_sales_by_products(\n from_date=from_date,\n
 to_date=to_date,\n units=units,\n )\n\n print(stop_sales)\n\n\nif __name__ ==
 \'__main__\':\n asyncio.run(main())\n```', 'author': 'Eldos', 'author_email':
 'eldos.baktybekov@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'None', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.11,<4.0', } setup
```

### Comparing `dodo_is_api-0.7.2/PKG-INFO` & `dodo_is_api-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodo-is-api
-Version: 0.7.2
+Version: 0.8.0
 Summary: 
 Author: Eldos
 Author-email: eldos.baktybekov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
@@ -107,15 +107,15 @@
     access_token = 'your access token'
     country_code = models.CountryCode.RU
 
     from_date = datetime(2004, 10, 7)
     to_date = datetime(2004, 10, 7, 23)
     units = [UUID('ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb')]
 
-    with httpx.AsyncClient() as http_client:
+    async with httpx.AsyncClient() as http_client:
         connection = AsyncDodoISAPIConnection(
             http_client=http_client,
             access_token=access_token,
             country_code=country_code,
         )
 
         stop_sales = await connection.get_stop_sales_by_products(
```

