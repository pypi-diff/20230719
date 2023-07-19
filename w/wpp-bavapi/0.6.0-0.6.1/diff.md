# Comparing `tmp/wpp-bavapi-0.6.0.tar.gz` & `tmp/wpp-bavapi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp-bavapi-0.6.0.tar", last modified: Thu Jul 13 12:47:18 2023, max compression
+gzip compressed data, was "wpp-bavapi-0.6.1.tar", last modified: Wed Jul 19 14:46:38 2023, max compression
```

## Comparing `wpp-bavapi-0.6.0.tar` & `wpp-bavapi-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/_int_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.609901 wpp-bavapi-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-19 14:46:38.609901 wpp-bavapi-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.605901 wpp-bavapi-0.6.1/bavapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.605901 wpp-bavapi-0.6.1/bavapi/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/parsing/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/parsing/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.605901 wpp-bavapi-0.6.1/bavapi/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/reference/_int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/reference/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/bavapi/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:46:38.609901 wpp-bavapi-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.609901 wpp-bavapi-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-19 14:46:11.000000 wpp-bavapi-0.6.1/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:38.609901 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 14:46:38.000000 wpp-bavapi-0.6.1/wpp_bavapi.egg-info/top_level.txt
```

### Comparing `wpp-bavapi-0.6.0/LICENSE` & `wpp-bavapi-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/PKG-INFO` & `wpp-bavapi-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wpp-bavapi-0.6.0/README.md` & `wpp-bavapi-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/__init__.py` & `wpp-bavapi-0.6.1/bavapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/client.py` & `wpp-bavapi-0.6.1/bavapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,22 +379,22 @@
         include: OptionalListOr[str] = None,
         metric_keys: OptionalListOr[str] = None,
         stack_data: bool = False,
         **kwargs: BaseListOrValues,
     ) -> "DataFrame":
         """Query the Fount `brandscape-data` endpoint.
 
-        This endpoint requires at least one of the following combinations of parameters:
+        This endpoint requires at least one of the following combinations of filters:
 
         - `studies`
         - `brand_name`
         - `brands`
-        - `year_number` and `brands`/`brand_name`
-        - `country_code` and `brands`/`brand_name`
-        - `year_number` and `country_code`
+        - `year_number`/`years` and `brands`/`brand_name`
+        - `country_code`/`countries` and `brands`/`brand_name`
+        - `year_number`/`years` and `country_code`/`countries`
 
         An audience filter is also highly recommended, as otherwise the API will return
         data for all audiences (there are more than 30 standard audiences).
 
         The `Audiences` class is provided to make it easier to filter audiences.
 
         Note that this endpoint has a default set of `include` resources:
@@ -428,14 +428,16 @@
         fields : str or list[str], optional
             Fields to retrieve in API response, by default None
 
             Only specified fields are returned.
             If `fields` is None, all fields are returned.
         include : str or list[str], optional
             Additional resources to include in API response, by default None
+        metric_keys: str or list[str], optional
+            Key or list of keys for the metrics included in the response, by default None
         stack_data : bool, optional
             Whether to expand nested lists into new dictionaries, by default False
         **kwargs
             Additional parameters to pass to the Query. See `Other Parameters`.
             For any filters, use the `filters` parameter.
 
         Other Parameters
@@ -469,21 +471,21 @@
         filters = _filters.BrandscapeFilters.ensure(
             filters,
             country_code=country_code,
             year_number=year_number,
             audiences=audiences,
             brand_name=brand_name,
             studies=studies,
-            metric_keys=metric_keys,
         )
 
         query: Query[_filters.BrandscapeFilters] = Query(
             filters=filters,
             fields=fields,
             include=_default_brandscape_include(include),
+            metric_keys=metric_keys,
             **kwargs,  # type: ignore[arg-type]
         )
 
         items = await self._client.query("brandscape-data", query)
 
         # Prefix 'global' to avoid clashing with 'brand_name' on 'brand' includes
         return parse_response(items, "global", expand=stack_data)
```

### Comparing `wpp-bavapi-0.6.0/bavapi/filters.py` & `wpp-bavapi-0.6.1/bavapi/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,29 @@
     def ensure(
         cls: Type[F],
         filters: Optional[FiltersOrMapping["FountFilters"]],
         **addl_filters: InputSequenceOrValues,
     ) -> Optional[F]:
         """Ensure FountFilters class from dictionary or other FountFilters class.
 
-        If `filters` is None, returns None.
-
         Parameters
         ----------
         filters : FountFilters or dict of filter values, optional
             Dictionary of filters or FountFilters class.
         **addl_filters : SequenceOrValues, optional
             Additional filters to add to the new FountFilters instance.
 
         Returns
         -------
         FountFilters, optional
-            FountFilters class or None.
+            FountFilters class or None if `filters` is None and no additional filters are passed.
+
+        Notes
+        -----
+        Defaults to values passed to `filters` when any additional filters overlap.
         """
         addl_filters = {k: v for k, v in addl_filters.items() if v}
 
         if filters is None:
             if not addl_filters:
                 return None
             return cls(**addl_filters)  # type: ignore[arg-type]
@@ -197,16 +199,14 @@
         Study years in numerical format (not IDs), by default None
     audiences : int or list[int], optional
         Fount ID of the desired audience, by default None
 
         The `Audiences` class can help with using audience IDs.
     brand_name : str, optional
         Perform a search on the brand name, by default None
-    metric_keys : str or list[str], optional
-        Metric keys to return as columns, by default None
     brands : int or list[int], optional
         Fount brand ID or list of brand IDs, by default None
     categories : int or list[int], optional
         Fount category ID or list of category IDs, by default None
     countries : int or list[int], optional
         Fount country ID or list of country IDs, by default None
 
@@ -223,15 +223,14 @@
         Request items that have been updated since the specified date, by default None
     """
 
     country_code: OptionalListOr[str] = None
     year_number: OptionalListOr[int] = None
     audiences: OptionalListOr[int] = None
     brand_name: Optional[str] = None
-    metric_keys: OptionalListOr[str] = None
     studies: OptionalListOr[int] = None
     countries: OptionalListOr[int] = None
     years: OptionalListOr[int] = None
     brands: OptionalListOr[int] = None
     categories: OptionalListOr[int] = None
 
     @model_validator(mode="before")
```

### Comparing `wpp-bavapi-0.6.0/bavapi/http.py` & `wpp-bavapi-0.6.1/bavapi/http.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/jupyter.py` & `wpp-bavapi-0.6.1/bavapi/jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/parsing/params.py` & `wpp-bavapi-0.6.1/bavapi/parsing/params.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/parsing/responses.py` & `wpp-bavapi-0.6.1/bavapi/parsing/responses.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/query.py` & `wpp-bavapi-0.6.1/bavapi/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,22 @@
         Get specific resource by ID, by default None
     filters : FountFilters instance or dict of filter values, optional
         Filters to apply to the query, by default None
     fields: str or list[str], optional
         Specific fields to retrieve from the query, by default None
     include: str or list[str], optional
         Additional resources to retrieve from the query, by default None
+    metric_keys: str or list[str], optional
+        Key or list of keys for the metrics included in the response, by default None
+
+        Currently, this parameter is only available for the `brandscape-data` endpoint.
     sort: str, optional
         Sort response by field, by default None
 
         To sort in descending (highest first) order, use a `-` before the field name:
-
         `sort="-differentiation_rank"`
 
         Sorts by item ID by default.
     page: int, optional
         Get specific page from paginated response, by default None
 
         When None, the default value in the Fount is 1
@@ -58,14 +61,15 @@
         When None, all pages will be retrieved with a `per_page` value of 100 by default.
     """
 
     item_id: Optional[int] = Field(default=None, alias="id")
     filters: Optional[_filters.FiltersOrMapping[F]] = None
     fields: OptionalListOr[str] = None
     include: OptionalListOr[str] = None
+    metric_keys: OptionalListOr[str] = None
     sort: Optional[str] = None
     page: Optional[int] = None
     per_page: Optional[int] = None
     max_pages: Optional[int] = None
 
     def to_params(self, endpoint: str) -> BaseParamsDictValues:
         """Return Fount-compatible dictionary of the query.
@@ -82,15 +86,16 @@
 
         if isinstance(self.filters, _filters.FountFilters):
             filters = self.filters.model_dump(by_alias=True, exclude_defaults=True)
         elif self.filters is not None:
             filters = cast(BaseParamsDict, self.filters)
         filters = to_fount_params(filters, "filter")
         fields = to_fount_params(
-            {endpoint: self.fields} if self.fields else fields, "fields"
+            {endpoint.replace("-", "_"): self.fields} if self.fields else fields,
+            "fields",
         )
 
         params = {
             **self.model_dump(exclude=exclude, by_alias=True, exclude_defaults=True),
             **filters,
             **fields,
         }
@@ -114,15 +119,17 @@
         Query
             New `Query` instance with page parameters.
         """
         if self.page and self.per_page:
             return self
 
         return self.__class__.model_construct(
-            self.model_fields_set.union({"page", "per_page"}),
+            self.model_fields_set.union(   # pylint: disable=no-member
+                {"page", "per_page"}
+            ),
             page=self.page or page,
             per_page=self.per_page or per_page,
             filters=self.filters,  # avoid turning filters into dictionary
             **self.model_dump(
                 by_alias=True,
                 exclude={"page", "per_page", "filters"},
                 exclude_defaults=True,
```

### Comparing `wpp-bavapi-0.6.0/bavapi/reference/generate_reference.py` & `wpp-bavapi-0.6.1/bavapi/reference/generate_reference.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/bavapi/sync.py` & `wpp-bavapi-0.6.1/bavapi/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""Convenience functions to perform queries to the Fount synchronously.
+"""
+Convenience functions to perform queries to the Fount synchronously.
 
-Can be used directly without using `asyncio`.
+Can be used directly without `asyncio`.
 
 Meant for experimentation, Jupyter notebooks, one-off scripts, etc.
 
 Use `bavapi.Client` for more advanced usage and performance benefits.
 """
 
 # pylint: disable=redefined-outer-name, too-many-arguments
@@ -328,14 +329,16 @@
     fields : str or list[str], optional
         Fields to retrieve in API response, by default None
 
         Only specified fields are returned.
         If `fields` is None, all fields are returned.
     include : str or list[str], optional
         Additional resources to include in API response, by default None
+    metric_keys: str or list[str], optional
+        Key or list of keys for the metrics included in the response, by default None
     stack_data : bool, optional
         Whether to expand nested lists into new dictionaries, by default False
     **kwargs
         Additional parameters to pass to the Query. See `Other Parameters`.
         For any filters, use the `filters` parameter.
 
     Other Parameters
```

### Comparing `wpp-bavapi-0.6.0/bavapi/typing.py` & `wpp-bavapi-0.6.1/bavapi/typing.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/pyproject.toml` & `wpp-bavapi-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wpp-bavapi"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
     { name = "Ignacio Maiz Vilches", email = "ignacio.maiz@bavgroup.com" },
 ]
 description = "Python consumer for the WPPBAV Fount API."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -47,25 +47,25 @@
     "typing-extensions >= 3.10; python_version < '3.10'",
 ]
 
 [project.urls]
 homepage = "https://github.com/wppbav/bavapi-sdk-python"
 
 [project.optional-dependencies]
-dev = ["black", "nox", "pip-tools", "pylint"]
+dev = ["black", "nox", "pip-tools"]
 doc = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
     "mkdocs-gen-files",
     "mkdocs-literate-nav",
     "mkdocs-section-index",
 ]
 test = ["coverage", "pytest", "pytest-asyncio", "python-dotenv"]
-lint = ["pylint", "mypy", "pandas-stubs"]
+lint = ["isort", "mypy", "pylint", "pandas-stubs"]
 
 [project.scripts]
 bavapi-gen-refs = "bavapi.reference.generate_reference:main"
 
 [tool.setuptools.packages.find]
 include = ["bavapi*"]
```

### Comparing `wpp-bavapi-0.6.0/tests/test_client.py` & `wpp-bavapi-0.6.1/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=protected-access, redefined-outer-name
 
 from typing import Set
 from unittest import mock
 
 import pytest
 
+from bavapi import filters
 from bavapi.client import Client, _default_brandscape_include
 from bavapi.http import HTTPClient
 from bavapi.query import Query
 from bavapi.typing import OptionalListOr
 
 from .helpers import wraps
 
@@ -82,58 +83,58 @@
     with mock.patch("bavapi.client.HTTPClient.aclose", wraps=wraps()) as mock_aclose:
         await fount.aclose()
 
     mock_aclose.assert_called_once()
 
 
 @pytest.mark.anyio
-async def test_raw_query(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"t": 1}])
-    ) as mock_base_query:
-        assert await fount.raw_query("request", Query()) == [{"t": 1}]
+@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1}]))
+async def test_raw_query(mock_query: mock.AsyncMock, fount: Client):
+    await fount.raw_query("request", Query())
 
-    mock_base_query.assert_awaited_once_with("request", Query())
+    mock_query.assert_awaited_once_with("request", Query())
 
 
 @pytest.mark.anyio
-async def test_audiences(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1}])
-    ) as mock_base_query:
-        assert (await fount.audiences(audience_id=1)).shape == (1, 1)
+@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1}]))
+async def test_audiences(mock_query: mock.AsyncMock, fount: Client):
+    await fount.audiences(active=1, include="test")
 
-    mock_base_query.assert_awaited_once_with("audiences", Query(id=1))
+    mock_query.assert_awaited_once_with(
+        "audiences", Query(filters=filters.AudiencesFilters(active=1), include="test")
+    )
 
 
 @pytest.mark.anyio
-async def test_brands(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1}])
-    ) as mock_base_query:
-        assert (await fount.brands(brand_id=1)).shape == (1, 1)
-
-    mock_base_query.assert_awaited_once_with("brands", Query(id=1))
+@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
+async def test_brands(mock_query: mock.AsyncMock, fount: Client):
+    await fount.brands(country_codes="test", fields="test")
+
+    mock_query.assert_awaited_once_with(
+        "brands",
+        Query(filters=filters.BrandsFilters(country_codes="test"), fields="test"),
+    )
 
 
 @pytest.mark.anyio
-async def test_brandscape_data(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
-    ) as mock_base_query:
-        res = await fount.brandscape_data(fields="")
-        assert res.shape == (1, 2)
+@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
+async def test_brandscape_data(mock_query: mock.AsyncMock, fount: Client):
+    await fount.brandscape_data(studies=1, metric_keys="test")
 
-    mock_base_query.assert_awaited_once_with(
+    mock_query.assert_awaited_once_with(
         "brandscape-data",
-        Query(fields="", include=["study", "brand", "category", "audience"]),
+        Query(
+            filters=filters.BrandscapeFilters(studies=1),
+            metric_keys="test",
+            include=["study", "brand", "category", "audience"],
+        ),
     )
 
 
 @pytest.mark.anyio
-async def test_studies(fount: Client):
-    with mock.patch.object(
-        fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
-    ) as mock_base_query:
-        assert (await fount.studies(study_id=1)).shape == (1, 2)
+@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
+async def test_studies(mock_query: mock.AsyncMock, fount: Client):
+    await fount.studies(include="test", full_year=1)
 
-    mock_base_query.assert_awaited_once_with("studies", Query(id=1))
+    mock_query.assert_awaited_once_with(
+        "studies", Query(filters=filters.StudiesFilters(full_year=1), include="test")
+    )
```

### Comparing `wpp-bavapi-0.6.0/tests/test_filters.py` & `wpp-bavapi-0.6.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/tests/test_http.py` & `wpp-bavapi-0.6.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/tests/test_jupyter.py` & `wpp-bavapi-0.6.1/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/tests/test_query.py` & `wpp-bavapi-0.6.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/tests/test_sync.py` & `wpp-bavapi-0.6.1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.6.0/wpp_bavapi.egg-info/PKG-INFO` & `wpp-bavapi-0.6.1/wpp_bavapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wpp-bavapi-0.6.0/wpp_bavapi.egg-info/SOURCES.txt` & `wpp-bavapi-0.6.1/wpp_bavapi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 bavapi/parsing/responses.py
 bavapi/reference/__init__.py
 bavapi/reference/_int_enum.py
 bavapi/reference/generate_reference.py
 tests/test_client.py
 tests/test_filters.py
 tests/test_http.py
+tests/test_integration.py
 tests/test_jupyter.py
 tests/test_query.py
 tests/test_sync.py
 wpp_bavapi.egg-info/PKG-INFO
 wpp_bavapi.egg-info/SOURCES.txt
 wpp_bavapi.egg-info/dependency_links.txt
 wpp_bavapi.egg-info/entry_points.txt
```

