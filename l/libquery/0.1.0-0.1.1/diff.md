# Comparing `tmp/libquery-0.1.0.tar.gz` & `tmp/libquery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquery-0.1.0.tar", max compression
+gzip compressed data, was "libquery-0.1.1.tar", max compression
```

## Comparing `libquery-0.1.0.tar` & `libquery-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34523 2023-07-16 16:39:37.808078 libquery-0.1.0/LICENSE
--rw-r--r--   0        0        0       64 2023-07-16 16:39:37.808078 libquery-0.1.0/README.md
--rw-r--r--   0        0        0      418 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/base.py
--rw-r--r--   0        0        0      101 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/david_rumsey_map_collection/__init__.py
--rw-r--r--   0        0        0     4401 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/david_rumsey_map_collection/_fetch_metadata.py
--rw-r--r--   0        0        0     1517 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/david_rumsey_map_collection/_querier.py
--rw-r--r--   0        0        0     1721 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/david_rumsey_map_collection/_typing.py
--rw-r--r--   0        0        0       67 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/gallica/__init__.py
--rw-r--r--   0        0        0     8781 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/gallica/_fetch_metadata.py
--rw-r--r--   0        0        0     1849 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/gallica/_querier.py
--rw-r--r--   0        0        0     2158 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/gallica/_typing.py
--rw-r--r--   0        0        0      717 2023-07-16 16:39:37.808078 libquery-0.1.0/libquery/gallica/_utils.py
--rw-r--r--   0        0        0       83 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/__init__.py
--rw-r--r--   0        0        0     2758 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_extract_images.py
--rw-r--r--   0        0        0     3230 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_fetch_file.py
--rw-r--r--   0        0        0     4443 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_fetch_metadata.py
--rw-r--r--   0        0        0     1485 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_querier.py
--rw-r--r--   0        0        0     2633 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_typing.py
--rw-r--r--   0        0        0      243 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/internet_archive/_utils.py
--rw-r--r--   0        0        0       87 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/library_of_congress/__init__.py
--rw-r--r--   0        0        0     4109 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/library_of_congress/_fetch_metadata.py
--rw-r--r--   0        0        0     1296 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/library_of_congress/_querier.py
--rw-r--r--   0        0        0     6698 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/library_of_congress/_typing.py
--rw-r--r--   0        0        0     1755 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/typing.py
--rw-r--r--   0        0        0     5200 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/utils/image.py
--rw-r--r--   0        0        0      427 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/utils/jsonl.py
--rw-r--r--   0        0        0     1950 2023-07-16 16:39:37.812078 libquery-0.1.0/libquery/utils/metadata.py
--rw-r--r--   0        0        0      576 2023-07-16 16:39:37.812078 libquery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 libquery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-19 03:43:43.310995 libquery-0.1.1/LICENSE
+-rw-r--r--   0        0        0      661 2023-07-19 03:43:43.310995 libquery-0.1.1/README.md
+-rw-r--r--   0        0        0      418 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/base.py
+-rw-r--r--   0        0        0       90 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/david_rumsey_map_collection/__init__.py
+-rw-r--r--   0        0        0     4296 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/david_rumsey_map_collection/_fetch_metadata.py
+-rw-r--r--   0        0        0     1555 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/david_rumsey_map_collection/_querier.py
+-rw-r--r--   0        0        0     1804 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/david_rumsey_map_collection/_typing.py
+-rw-r--r--   0        0        0       56 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/gallica/__init__.py
+-rw-r--r--   0        0        0     8744 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/gallica/_fetch_metadata.py
+-rw-r--r--   0        0        0     1896 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/gallica/_querier.py
+-rw-r--r--   0        0        0     2306 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/gallica/_typing.py
+-rw-r--r--   0        0        0      717 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/gallica/_utils.py
+-rw-r--r--   0        0        0       72 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/__init__.py
+-rw-r--r--   0        0        0     2746 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_extract_images.py
+-rw-r--r--   0        0        0     3213 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_fetch_file.py
+-rw-r--r--   0        0        0     4374 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_fetch_metadata.py
+-rw-r--r--   0        0        0     1395 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_querier.py
+-rw-r--r--   0        0        0     2750 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_typing.py
+-rw-r--r--   0        0        0      243 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/internet_archive/_utils.py
+-rw-r--r--   0        0        0       76 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/library_of_congress/__init__.py
+-rw-r--r--   0        0        0     4079 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/library_of_congress/_fetch_metadata.py
+-rw-r--r--   0        0        0     1283 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/library_of_congress/_querier.py
+-rw-r--r--   0        0        0     6656 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/library_of_congress/_typing.py
+-rw-r--r--   0        0        0     1755 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/typing.py
+-rw-r--r--   0        0        0     5237 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/utils/image.py
+-rw-r--r--   0        0        0      425 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/utils/jsonl.py
+-rw-r--r--   0        0        0     1940 2023-07-19 03:43:43.314995 libquery-0.1.1/libquery/utils/metadata.py
+-rw-r--r--   0        0        0      576 2023-07-19 03:43:43.314995 libquery-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 libquery-0.1.1/PKG-INFO
```

### Comparing `libquery-0.1.0/LICENSE` & `libquery-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libquery-0.1.0/libquery/base.py` & `libquery-0.1.1/libquery/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 class BaseQuerierWithQueryReturn(BaseQuerier):
     """
     The base of queriers whose
     query returns are to be stored as individual JSON lines files.
     """
 
-    def __init__(self, metadata_dir: str,
-                 img_dir: str):
+    def __init__(self, metadata_dir: str, img_dir: str):
         """
         Args
         ----
         metadata_dir : str
             The directory storing the metadata from each query.
         img_dir : str
             The directory storing the images from each query.
@@ -36,15 +35,15 @@
 
         self.metadata_dir = metadata_dir
         self.img_dir = img_dir
 
     @property
     def query_return_dir(self) -> str:
         """The directory storing the metadata from each query."""
-        dirname = 'query-return'
-        return f'{self.metadata_dir}/{dirname}'
+        dirname = "query-return"
+        return f"{self.metadata_dir}/{dirname}"
 
     @property
     def metadata_path(self) -> str:
         """The file storing the metadata from each query."""
-        filename = 'metadata.jsonl'
-        return f'{self.metadata_dir}/{filename}'
+        filename = "metadata.jsonl"
+        return f"{self.metadata_dir}/{filename}"
```

### Comparing `libquery-0.1.0/libquery/david_rumsey_map_collection/_fetch_metadata.py` & `libquery-0.1.1/libquery/david_rumsey_map_collection/_fetch_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,26 @@
     """
     Get the number of entries matching the url.
     Use the 'totalResults' attribute returned by David Rumsey Map Collection.
     """
 
     response = requests.get(base_url)
     data = response.json()
-    return int(data['totalResults'])
+    return int(data["totalResults"])
 
 
 def _get_query_param(base_url: str) -> str:
     """
     Split the query parameter from the url.
     """
 
-    return base_url.split('?')[1]
+    return base_url.split("?")[1]
 
 
-def _build_queries(base_url: str,
-                  query_return_path: str) -> List[str]:
+def _build_queries(base_url: str, query_return_path: str) -> List[str]:
     """
     Build a list of urls to query.
     The urls already queried according to
     the stored metadata will be excluded.
 
     Note
     ----
@@ -51,50 +50,48 @@
     different return values when David Rumsey Map Collection updates,
     the deduplication may cause new images to be ignored.
     Thus, the deduplication only apply to the queried in the recent 7 days.
     """
 
     n_records = _fetch_num_records(base_url)
     n_samples = 1
-    queries = [f'{base_url}&os={offset}&bs={n_samples}'
-               for offset in range(n_records)]
+    queries = [f"{base_url}&os={offset}&bs={n_samples}" for offset in range(n_records)]
     return filter_queries(queries, query_return_path)
 
 
 def _parse(response: Response) -> MetadataEntry:
     """
     Parse metadata of entries in David Rumsey Map Collection.
     """
 
     data = response.json()
 
-    assert len(data['results']) == 1, f"length = {len(data['results'])}"
+    assert len(data["results"]) == 1, f"length = {len(data['results'])}"
 
-    result = data['results'][0]
+    result = data["results"][0]
 
     # relayButtonUrl and relayButtonTitle are useless but take much storage
-    del result['relayButtonUrl']
-    del result['relayButtonTitle']
+    del result["relayButtonUrl"]
+    del result["relayButtonTitle"]
 
-    source = 'David Rumsey Map Collection'
-    id_in_source = result['id']
+    source = "David Rumsey Map Collection"
+    id_in_source = result["id"]
 
     return {
-        'uuid': str(uuid5(UUID(int=0), f'{source}/{id_in_source}')),
-        'url': response.url,
-        'source': source,
-        'idInSource': id_in_source,
-        'accessDate': datetime.now(timezone.utc).isoformat(),
-        'sourceData': result,
+        "uuid": str(uuid5(UUID(int=0), f"{source}/{id_in_source}")),
+        "url": response.url,
+        "source": source,
+        "idInSource": id_in_source,
+        "accessDate": datetime.now(timezone.utc).isoformat(),
+        "sourceData": result,
     }
 
 
 @backoff.on_exception(backoff.constant, ProxyError)
-def fetch_metadata(base_urls: List[str],
-                   query_return_dir: str) -> None:
+def fetch_metadata(base_urls: List[str], query_return_dir: str) -> None:
     """
     Given base urls, generate metadata queries, and store the query results.
 
     Avoid duplication with the entries
     already stored in existing metadata files.
     The duplication is checked by idInSource.
 
@@ -107,42 +104,40 @@
         The path to the folder for storing the metadata files.
     """
 
     if not os.path.exists(query_return_dir):
         os.makedirs(query_return_dir)
 
     for base_url in base_urls:
-        print(f'Fetch Metadata from {base_url}')
+        print(f"Fetch Metadata from {base_url}")
 
         query_return_path = os.path.join(
             query_return_dir,
-            f'{_get_query_param(base_url)}.jsonl',
+            f"{_get_query_param(base_url)}.jsonl",
         )
         queries = _build_queries(base_url, query_return_path)
-        
-        with open(query_return_path, 'a', encoding='utf-8') as f:
-            for query in tqdm(queries, desc='Progress'):
+
+        with open(query_return_path, "a", encoding="utf-8") as f:
+            for query in tqdm(queries, desc="Progress"):
                 response = requests.get(query)
                 metadata_entry = _parse(response)
-                f.write(
-                    f'{json.dumps(metadata_entry, ensure_ascii=False)}\n')
+                f.write(f"{json.dumps(metadata_entry, ensure_ascii=False)}\n")
 
         # For duplicate entries, only keep the latest one.
         deduplicate(query_return_path)
 
 
-def merge_metadata(base_urls: List[str],
-                   query_return_dir: str) -> List[MetadataEntry]:
+def merge_metadata(base_urls: List[str], query_return_dir: str) -> List[MetadataEntry]:
     """
     Merge metadata of different queries.
     Return the merge result.
     """
 
     entries: List[MetadataEntry] = []
     for base_url in base_urls:
         path = os.path.join(
             query_return_dir,
-            f'{_get_query_param(base_url)}.jsonl',
+            f"{_get_query_param(base_url)}.jsonl",
         )
         if os.path.exists(path):
             entries += load_jl(path)
     return entries
```

### Comparing `libquery-0.1.0/libquery/david_rumsey_map_collection/_querier.py` & `libquery-0.1.1/libquery/library_of_congress/_querier.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 """
 The entrance to querier class.
 """
 
 from typing import List
 
-from ..base import BaseQuerierWithQueryReturn
+from ..base import BaseQuerier
 from ..typing import ImageQuery
 from ..utils.image import fetch as fetch_image
-from ..utils.jsonl import save_jl
-from ..utils.metadata import deduplicate
-from ._fetch_metadata import fetch_metadata, merge_metadata
-from ._typing import MetadataEntry, SourceData
-
-
-def _get_download_url(source_data: SourceData) -> str:
-    return source_data['urlSize4'] if 'urlSize4' in source_data\
-        else source_data['urlSize2']
+from ._fetch_metadata import fetch_metadata
+from ._typing import MetadataEntry
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
-    """Build a list of image urls to query."""
+    """
+    Build a list of image urls to query.
+    """
 
-    return [{
-        'url': _get_download_url(d['sourceData']),
-        'uuid': d['uuid'],
-    } for d in metadata]
+    return [
+        {
+            "url": d["sourceData"]["image_url"][-1],
+            "uuid": d["uuid"],
+        }
+        for d in metadata
+    ]
 
 
-class Querier(BaseQuerierWithQueryReturn):
+class LibraryOfCongress(BaseQuerier):
     """
-    The querier for the `David Rumsey Map Collection` data source.
+    The querier for the `Library of Congress` data source.
     """
 
-    def fetch_metadata(self, queries: List[str]) -> None:
+    def __init__(self, metadata_path: str, img_dir: str):
         """
         Args
         ----
-        queries : List[str]
-            The base urls for which query results are to be stored.
+        metadata_path : str
+            The file storing the metadata from each query.
+        img_dir : str
+            The directory storing the images from each query.
         """
 
-        fetch_metadata(queries, self.query_return_dir)
-        entries = merge_metadata(queries, self.query_return_dir)
-        save_jl(entries, self.metadata_path)
-        deduplicate(self.metadata_path)
+        self.metadata_path = metadata_path
+        self.img_dir = img_dir
+
+    def fetch_metadata(self, queries: List[str]) -> None:
+        fetch_metadata(queries, self.metadata_path)
 
     def fetch_image(self) -> None:
-        fetch_image(self.metadata_path,
-                    self.img_dir,
-                    _build_image_queries)
+        fetch_image(self.metadata_path, self.img_dir, _build_image_queries)
```

### Comparing `libquery-0.1.0/libquery/gallica/_fetch_metadata.py` & `libquery-0.1.1/libquery/gallica/_fetch_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,121 +25,127 @@
 def _try_fetch_xml(url: str) -> Union[Dict, None]:
     response = requests.get(url)
 
     # If the server raises error,
     # the returned XML will not be parsable.
     # Raise error to retry to query.
     if response.status_code != 200:
-        raise ExpatError('Request failed with status code:',
-                         response.status_code)
+        raise ExpatError("Request failed with status code:", response.status_code)
 
     # An example query with status code 200 and empty response.text:
     # https://gallica.bnf.fr/services/Pagination?ark=cb326850921
     try:
         return xmltodict.parse(response.text)
     except ExpatError:
         return None
 
 
 @backoff.on_exception(backoff.constant, KeyError)
 def _fetch_num_records(base_url: str) -> int:
     """Get the number of entries found by the search url."""
 
     payload = _try_fetch_xml(base_url)
-    n_records = payload['srw:searchRetrieveResponse']['srw:numberOfRecords']
+    n_records = payload["srw:searchRetrieveResponse"]["srw:numberOfRecords"]
     return int(n_records)
 
 
 def _get_query_param(base_url: str) -> str:
     """
     Split the query parameter from the url.
     """
 
-    query_param = base_url.split('query=')[1]
-    return f'query={query_param}'
+    query_param = base_url.split("query=")[1]
+    return f"query={query_param}"
 
 
 def _get_ark_identifier(identifier: str) -> Union[str, None]:
     """
     Extract the ark identifier from the url identifier.
     If the ark identifier cannot be parsed, return None.
 
     Examples:
     1. given 'https://gallica.bnf.fr/ark:/12148/bpt6k5619759j',
     return 'ark:/12148/bpt6k5619759j'.
     2. given 'https://gallica.bnf.fr/ark:/12148/cb32798952c/date',
     return 'ark:/12148/cb32798952c,
     """
 
-    m = re.findall(r'ark:/12148/[a-zA-Z0-9]+', identifier)
+    m = re.findall(r"ark:/12148/[a-zA-Z0-9]+", identifier)
     if len(m) != 1:
         return None
-    return f'ark:/{m[0]}'
+    return f"ark:/{m[0]}"
 
 
-def _build_queries(template_url: str,
-                   query_return_path: str) -> List[str]:
+def _build_queries(template_url: str, query_return_path: str) -> List[str]:
     """
     Build a list of urls to query.
     """
 
     # Number of entries per page (i.e., per query).
     records_per_page = 10
 
-    n_records = _fetch_num_records(template_url.format(
-        startRecord=1,
-        maximumRecords=records_per_page,
-    ))
+    n_records = _fetch_num_records(
+        template_url.format(
+            startRecord=1,
+            maximumRecords=records_per_page,
+        )
+    )
     n_pages = math.ceil(n_records / records_per_page)
 
     # The first entry is indexed 1 in the database.
-    queries = [template_url.format(
-        startRecord=i * records_per_page + 1,
-        maximumRecords=records_per_page,
-    ) for i in range(n_pages)]
+    queries = [
+        template_url.format(
+            startRecord=i * records_per_page + 1,
+            maximumRecords=records_per_page,
+        )
+        for i in range(n_pages)
+    ]
     queries = [d for d in queries if d not in searched_url]
     return filter_queries(queries, query_return_path)
 
 
 def _fetch_oai_record(ark: str) -> Record:
     """
     Get OAI record information given the ARK identifier.
     Example ARK identifier: 'ark:/12148/cb32798952c'.
     """
 
     # The service of the detailed content for a collection.
-    query_term = ark.split('/')[-1]
-    oai_record_url = f'https://gallica.bnf.fr/services/OAIRecord?ark={query_term}'
+    query_term = ark.split("/")[-1]
+    oai_record_url = f"https://gallica.bnf.fr/services/OAIRecord?ark={query_term}"
 
     # Note: the server sometimes raises internal error with response.status_code = 500.
     # We ignore such errors and let the error handler outside
     # to identify such cases and retry the query.
     payload = _try_fetch_xml(oai_record_url)
-    return payload['results']['notice']['record']['metadata']['oai_dc:dc']
+    return payload["results"]["notice"]["record"]["metadata"]["oai_dc:dc"]
 
 
 def _fetch_pagination(ark: str) -> List[Page]:
     """
     Get pagination information given the ARK identifier.
     For the identifier of an image collection,
     the pagination information can be used to fetch the images.
     Example ARK identifier: 'ark:/12148/cb32798952c'.
     """
 
     # Get image page information (i.e., image list) for a collection
-    query_term = ark.split('/')[-1]
-    pagination_url = f'https://gallica.bnf.fr/services/Pagination?ark={query_term}'
+    query_term = ark.split("/")[-1]
+    pagination_url = f"https://gallica.bnf.fr/services/Pagination?ark={query_term}"
 
     pagination = _try_fetch_xml(pagination_url)
     if pagination is None:
         return []
 
     # Note: 'livre' is the French translation of 'book'
-    pages = [] if 'pages' not in pagination['livre']\
-        else pagination['livre']['pages']['page']
+    pages = (
+        []
+        if "pages" not in pagination["livre"]
+        else pagination["livre"]["pages"]["page"]
+    )
     if not isinstance(pages, list):
         pages = [pages]
     return pages
 
 
 @backoff.on_exception(backoff.constant, KeyError)
 def _fetch_identifiers(query: str) -> List[str]:
@@ -147,73 +153,69 @@
     Get the identifiers of search results, given a search query.
 
     Example identifiers:
     https://gallica.bnf.fr/ark:/12148/btv1b530093905
     """
 
     payload: Dict = _try_fetch_xml(query)
-    records = payload['srw:searchRetrieveResponse']['srw:records']['srw:record']
+    records = payload["srw:searchRetrieveResponse"]["srw:records"]["srw:record"]
 
     if not isinstance(records, list):
         records = [records]
 
-    identifiers = [
-        d['srw:recordData']['oai_dc:dc']['dc:identifier']
-        for d in records
-    ]
+    identifiers = [d["srw:recordData"]["oai_dc:dc"]["dc:identifier"] for d in records]
     return [d for d in identifiers if d is not None]
 
 
 def _fetch_source_data(identifier: str) -> SourceData:
-    source_data = {'identifier': identifier}
+    source_data = {"identifier": identifier}
 
     # If the identifier does not contain 'ark:/',
     # the ark identifier cannot be parsed, and the OAI record cannot be found.
-    if 'ark:/' not in identifier:
+    if "ark:/" not in identifier:
         return source_data
 
     # ARK identifier of the form 'ark:/12148/cb32798952c'.
     ark = _get_ark_identifier(identifier)
     if ark is None:
         return source_data
 
-    source_data['record'] = _fetch_oai_record(ark)
+    source_data["record"] = _fetch_oai_record(ark)
 
     # If the entry is not in Gallica, its images cannot be obtained.
-    if 'gallica.bnf.fr/ark:/' in identifier:
-        source_data['pages'] = _fetch_pagination(ark)
+    if "gallica.bnf.fr/ark:/" in identifier:
+        source_data["pages"] = _fetch_pagination(ark)
 
     return source_data
 
 
 def _parse(query: str, identifier: str) -> MetadataEntry:
     """
     Parse each record, which may have more than one images.
 
     Example identifier:
     https://gallica.bnf.fr/ark:/12148/btv1b530093905
     """
 
-    source_name = 'Gallica'
+    source_name = "Gallica"
     id_in_source = identifier
     source_data = _fetch_source_data(identifier)
 
     return {
-        'uuid': str(uuid5(UUID(int=0), f'{source_name}/{id_in_source}')),
-        'url': query,
-        'source': source_name,
-        'idInSource': id_in_source,
-        'accessDate': datetime.now(timezone.utc).isoformat(),
-        'sourceData': source_data
+        "uuid": str(uuid5(UUID(int=0), f"{source_name}/{id_in_source}")),
+        "url": query,
+        "source": source_name,
+        "idInSource": id_in_source,
+        "accessDate": datetime.now(timezone.utc).isoformat(),
+        "sourceData": source_data,
     }
 
 
 @backoff.on_exception(backoff.constant, (ProxyError, SSLError))
-def fetch_metadata(base_urls: List[str],
-                   query_return_dir: str) -> None:
+def fetch_metadata(base_urls: List[str], query_return_dir: str) -> None:
     """
     Given base url and title keywords, generate metadata queries, and store the query results.
 
     Args
     ----
     base_urls:
         The base URLs for generating queries.
@@ -223,53 +225,52 @@
 
     if not os.path.exists(query_return_dir):
         os.makedirs(query_return_dir)
 
     visited_id_in_source = []
 
     for template_url in base_urls:
-        print(f'Fetch Metadata from {template_url}')
+        print(f"Fetch Metadata from {template_url}")
 
         query_return_path = os.path.join(
             query_return_dir,
-            f'{_get_query_param(template_url)}.jsonl',
+            f"{_get_query_param(template_url)}.jsonl",
         )
         queries = _build_queries(template_url, query_return_path)
 
-        entries = [] if not os.path.exists(query_return_path)\
-            else load_jl(query_return_path)
-        visited_id_in_source += [d['idInSource'] for d in entries]
+        entries = (
+            [] if not os.path.exists(query_return_path) else load_jl(query_return_path)
+        )
+        visited_id_in_source += [d["idInSource"] for d in entries]
 
-        with open(query_return_path, 'a', encoding='utf8') as f:
-            for query in tqdm(queries, desc='Progress'):
+        with open(query_return_path, "a", encoding="utf8") as f:
+            for query in tqdm(queries, desc="Progress"):
                 identifiers = _fetch_identifiers(query)
                 for identifier in identifiers:
                     if isinstance(identifier, list):
                         identifier = identifier[0]
 
                     id_in_source = identifier
                     if id_in_source in visited_id_in_source:
                         continue
                     visited_id_in_source.append(id_in_source)
 
                     metadata_entry = _parse(query, identifier)
                     if metadata_entry is not None:
-                        f.write(
-                            f'{json.dumps(metadata_entry, ensure_ascii=False)}\n')
+                        f.write(f"{json.dumps(metadata_entry, ensure_ascii=False)}\n")
                 searched_url.append(query)
 
 
-def merge_metadata(base_urls: List[str],
-                   query_return_dir: str) -> List[MetadataEntry]:
+def merge_metadata(base_urls: List[str], query_return_dir: str) -> List[MetadataEntry]:
     """
     Combine metadata files into one.
     """
 
     entries = []
     for base_url in base_urls:
         path = os.path.join(
             query_return_dir,
-            f'{_get_query_param(base_url)}.jsonl',
+            f"{_get_query_param(base_url)}.jsonl",
         )
         if os.path.exists(path):
             entries += load_jl(path)
     return entries
```

### Comparing `libquery-0.1.0/libquery/gallica/_querier.py` & `libquery-0.1.1/libquery/gallica/_querier.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
     """Build a list of image urls to query."""
 
     img_queries = []
     for d in metadata:
-        if 'pages' not in d['sourceData']:
+        if "pages" not in d["sourceData"]:
             continue
-        pages = d['sourceData']['pages']
-        img_queries += [{
-            'url': get_image_url(page, d),
-            'uuid': get_image_uuid(page, d),
-            # The file extension in Gallica are jpeg, and cannot be inferred
-            # with mimetypes.guess_extension.
-            'extension': '.jpeg',
-        } for page in pages]
+        pages = d["sourceData"]["pages"]
+        img_queries += [
+            {
+                "url": get_image_url(page, d),
+                "uuid": get_image_uuid(page, d),
+                # The file extension in Gallica are jpeg, and cannot be inferred
+                # with mimetypes.guess_extension.
+                "extension": ".jpeg",
+            }
+            for page in pages
+        ]
     return img_queries
 
 
-class Querier(BaseQuerierWithQueryReturn):
+class Gallica(BaseQuerierWithQueryReturn):
     """
     The querier for the `Gallica` data source.
     """
 
     def fetch_metadata(self, queries: List[str]) -> None:
         """
         Args
@@ -50,11 +53,13 @@
 
         fetch_metadata(queries, self.query_return_dir)
         entries = merge_metadata(queries, self.query_return_dir)
         save_jl(entries, self.metadata_path)
         deduplicate(self.metadata_path)
 
     def fetch_image(self) -> None:
-        base_fetch_image(self.metadata_path,
-                         self.img_dir,
-                         _build_image_queries,
-                         IncompleteFileHandler.SAVE)
+        base_fetch_image(
+            self.metadata_path,
+            self.img_dir,
+            _build_image_queries,
+            IncompleteFileHandler.SAVE,
+        )
```

### Comparing `libquery-0.1.0/libquery/gallica/_typing.py` & `libquery-0.1.1/libquery/gallica/_typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 """
 The type declarations specific to the `David Rumsey Map Collection` data source.
 """
 
-# pylint: disable=too-few-public-methods
-
 from typing import List, TypedDict, Union
 
 from typing_extensions import NotRequired
 
 from ..typing import MetadataEntry as BaseMetadataEntry
 
-TextWithLang = TypedDict('TextWithLang', {
-    '@xml:lang': str,
-    '#text': str,
-})
-
-Record = TypedDict('Record', {
-    '@xmlns:dc': str,
-    '@xmlns:oai_dc': str,
-    '@xmlns:xsi': str,
-    '@xsi:schemaLocation': str,
-    'dc:identifier': Union[str, List[str]],
-    'dc:relation': Union[str, List[str]],
-    'dc:source': str,
-    'dc:title': Union[str, List[Union[str, TextWithLang]]],
-
-    # The author(s).
-    'dc:creator': NotRequired[Union[str, List[str]]],
-    'dc:date': NotRequired[Union[str, List[str]]],
-    'dc:subject': NotRequired[Union[str, TextWithLang, List[Union[str, TextWithLang]], None]],
-    'dc:coverage': NotRequired[Union[str, List[str], None]],
-    'dc:format': NotRequired[Union[str, TextWithLang, List[Union[str, TextWithLang]]]],
-    # For collections within the BnF, the language code has 3 characters.
-    # For collections from outside, the language code can be arbitrary.
-    'dc:language': NotRequired[Union[str, List[str]]],
-    # Type of the document, e.g., monograph, map, image,
-    # fascicle, manuscript, score, sound, object and video.
-    'dc:type': NotRequired[List[Union[str, TextWithLang]]],
-    'dc:rights': NotRequired[List[TextWithLang]],
-    'dc:publisher': NotRequired[Union[str, List[str]]],
-    'dc:description': NotRequired[Union[str, List[str]]],
-    'dc:contributor': NotRequired[Union[str, List[str]]],
-    '#text': NotRequired[str],
-})
+TextWithLang = TypedDict(
+    "TextWithLang",
+    {
+        "@xml:lang": str,
+        "#text": str,
+    },
+)
+
+Record = TypedDict(
+    "Record",
+    {
+        "@xmlns:dc": str,
+        "@xmlns:oai_dc": str,
+        "@xmlns:xsi": str,
+        "@xsi:schemaLocation": str,
+        "dc:identifier": Union[str, List[str]],
+        "dc:relation": Union[str, List[str]],
+        "dc:source": str,
+        "dc:title": Union[str, List[Union[str, TextWithLang]]],
+        # The author(s).
+        "dc:creator": NotRequired[Union[str, List[str]]],
+        "dc:date": NotRequired[Union[str, List[str]]],
+        "dc:subject": NotRequired[
+            Union[str, TextWithLang, List[Union[str, TextWithLang]], None]
+        ],
+        "dc:coverage": NotRequired[Union[str, List[str], None]],
+        "dc:format": NotRequired[
+            Union[str, TextWithLang, List[Union[str, TextWithLang]]]
+        ],
+        # For collections within the BnF, the language code has 3 characters.
+        # For collections from outside, the language code can be arbitrary.
+        "dc:language": NotRequired[Union[str, List[str]]],
+        # Type of the document, e.g., monograph, map, image,
+        # fascicle, manuscript, score, sound, object and video.
+        "dc:type": NotRequired[List[Union[str, TextWithLang]]],
+        "dc:rights": NotRequired[List[TextWithLang]],
+        "dc:publisher": NotRequired[Union[str, List[str]]],
+        "dc:description": NotRequired[Union[str, List[str]]],
+        "dc:contributor": NotRequired[Union[str, List[str]]],
+        "#text": NotRequired[str],
+    },
+)
 
 
 class Page(TypedDict):
     numero: Union[str, None]
     ordre: str
     pagination_type: Union[str, None]
     image_width: str
@@ -58,8 +65,9 @@
     identifier: str
     record: NotRequired[Record]
     pages: NotRequired[List[Page]]
 
 
 class MetadataEntry(BaseMetadataEntry):
     """The data structure of an entry in the metadata."""
+
     sourceData: SourceData
```

### Comparing `libquery-0.1.0/libquery/gallica/_utils.py` & `libquery-0.1.1/libquery/gallica/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from ._typing import MetadataEntry, Page
 
 
 def get_image_url(page: Page, entry: MetadataEntry) -> str:
     """Get the download url of the image corresponding to a page."""
 
-    identifier = entry['sourceData']['identifier']
+    identifier = entry["sourceData"]["identifier"]
     image_id_in_source = f'{identifier}/f{page["ordre"]}'
-    return f'{image_id_in_source}.highres'
+    return f"{image_id_in_source}.highres"
 
 
 def get_image_uuid(page: Page, entry: MetadataEntry) -> str:
     """Get the uuid of the image corresponding to a page."""
 
-    source_name = entry['source']
-    identifier = entry['sourceData']['identifier']
+    source_name = entry["source"]
+    identifier = entry["sourceData"]["identifier"]
     image_id_in_source = f'{identifier}/f{page["ordre"]}'
-    return str(uuid5(UUID(int=0), f'{source_name}/{image_id_in_source}'))
+    return str(uuid5(UUID(int=0), f"{source_name}/{image_id_in_source}"))
```

### Comparing `libquery-0.1.0/libquery/internet_archive/_extract_images.py` & `libquery-0.1.1/libquery/internet_archive/_extract_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,72 +10,72 @@
 
 
 def _revise_filename(filename: str) -> str:
     """
     Revised the filename from using Internet Archive identifier to using UUID.
     """
 
-    source_name = 'Internet Archive'
+    source_name = "Internet Archive"
 
-    extension = filename.split('.')[-1]
+    extension = filename.split(".")[-1]
     uuid = get_image_uuid(filename, source_name)
-    return f'{uuid}.{extension}'
+    return f"{uuid}.{extension}"
 
 
 def _extract_images_from_zip(file: str, img_dir: str) -> None:
     """
     Extract images from a zip file.
     The zip file is expected to contain only .jp2 or .jpg files.
     """
 
     try:
-        with ZipFile(file, 'r') as zip_ref:
+        with ZipFile(file, "r") as zip_ref:
             zip_paths = zip_ref.namelist()
             for zip_path in zip_paths:
                 extension = os.path.splitext(zip_path)[-1]
-                if extension not in {'.jp2', '.jpg'}:
+                if extension not in {".jp2", ".jpg"}:
                     continue
                 _, filename = os.path.split(zip_path)
-                filename_revised = '.'.join(filename.split('.')[:-1]) + '.jpg'
+                filename_revised = ".".join(filename.split(".")[:-1]) + ".jpg"
                 filename_revised = _revise_filename(filename_revised)
 
                 # Skip, if the file is already unzipped
-                store_path = f'{img_dir}/{filename_revised}'
+                store_path = f"{img_dir}/{filename_revised}"
                 if os.path.exists(store_path):
                     continue
 
                 image_bytes = zip_ref.read(zip_path)
                 img = Image.open(io.BytesIO(image_bytes))
                 img.save(store_path)
     except BadZipFile:
-        print('Zip file corrupted:', file)
+        print("Zip file corrupted:", file)
+
 
 def extract_images(download_dir: str, img_dir: str) -> None:
     """
     Extract the images from download directory into image directory.
     """
 
     if not os.path.exists(img_dir):
         os.makedirs(img_dir)
 
     dir_names = os.listdir(download_dir)
 
     # Note: the directory name is the same as `idInSource`
-    for dir_name in tqdm(dir_names, desc='Extract Image Progress'):
-        filenames = os.listdir(f'{download_dir}/{dir_name}')
+    for dir_name in tqdm(dir_names, desc="Extract Image Progress"):
+        filenames = os.listdir(f"{download_dir}/{dir_name}")
 
         # No file is downloaded, which may happen when the file resource is not accessible.
         if len(filenames) == 0:
             continue
 
         # Note: all the non-empty directory are expected to contain one file
         # that is either a zip file or an image file.
-        assert len(filenames) == 1,\
-            f'Directory contains multiple files: {dir_name}'
+        assert len(filenames) == 1, f"Directory contains multiple files: {dir_name}"
 
         filename = filenames[0]
-        file_path = f'{download_dir}/{dir_name}/{filename}'
-        if filename.endswith('.zip'):
+        file_path = f"{download_dir}/{dir_name}/{filename}"
+        if filename.endswith(".zip"):
             _extract_images_from_zip(file_path, img_dir)
         else:
             filename_revised = _revise_filename(filename)
-            shutil.copy(file_path, f'{img_dir}/{filename_revised}')
+            shutil.copy(file_path, f"{img_dir}/{filename_revised}")
```

### Comparing `libquery-0.1.0/libquery/internet_archive/_fetch_file.py` & `libquery-0.1.1/libquery/internet_archive/_fetch_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,70 +12,74 @@
 
 class FileQuery(TypedDict):
     filename: str
     identifier: str
 
 
 def _get_filename(source_data: SourceData) -> Union[str, None]:
-    files = source_data['files']
+    files = source_data["files"]
 
     # 'JPEG' and 'PNG' correspond to collections of single images.
     # 'Single Page Processed JP2 ZIP' and 'Single Page Processed JPEG ZIP'
     # correspond to collections of multiple images.
     # Example of 'Single Page Processed JP2 ZIP':
     # <https://ia800500.us.archive.org/view_archive.php?archive=/25/items/essaisurlastatis00gueruoft/essaisurlastatis00gueruoft_jp2.zip>
     # Example of 'Single Page Processed JPEG ZIP':
     # <https://ia801402.us.archive.org/view_archive.php?archive=/10/items/1926981926m1931eng/1926981926m1931eng_jpg.zip>
     image_formats = [
-        'JPEG', 'PNG',
-        'Single Page Processed JP2 ZIP',
-        'Single Page Processed JPEG ZIP',
+        "JPEG",
+        "PNG",
+        "Single Page Processed JP2 ZIP",
+        "Single Page Processed JPEG ZIP",
     ]
-    image_files = [d for d in files if d['format'] in image_formats]
+    image_files = [d for d in files if d["format"] in image_formats]
     if len(image_files) == 0:
         return None
 
     # Download the first image.
-    return image_files[0]['name']
+    return image_files[0]["name"]
 
 
 def _build_queries(metadata: List[MetadataEntry]) -> List[FileQuery]:
     """
     Build a list of image urls to query.
     Note that internetarchive's download API already
     avoids downloading files already stored.
     """
 
     img_queries = []
     for d in metadata:
-        source_data = d['sourceData']
-        identifier = source_data['metadata']['identifier']
+        source_data = d["sourceData"]
+        identifier = source_data["metadata"]["identifier"]
         filename = _get_filename(source_data)
         if filename is None:
             continue
-        img_queries.append({'filename': filename,
-                            'identifier': identifier})
+        img_queries.append(
+            {
+                "filename": filename,
+                "identifier": identifier,
+            }
+        )
 
     return img_queries
 
 
-def _filter_queries(img_queries: List[FileQuery],
-                   download_dir: str) -> List[FileQuery]:
+def _filter_queries(img_queries: List[FileQuery], download_dir: str) -> List[FileQuery]:
     """
     Filter urls queried before according to the stored files.
     """
 
     return [
-        d for d in img_queries
+        d
+        for d in img_queries
         if not isfile(f'{download_dir}/{d["identifier"]}/{d["filename"]}')
     ]
 
 
-def fetch_file(metadata_path: str,
-               download_dir: str) -> None:
+def fetch_file(metadata_path: str, download_dir: str) -> None:
     """
     Given base urls, generate file queries, and store the query results.
 
     Args
     ----
     metadata_path : str
         The path to the metadata file where file urls are stored.
@@ -85,15 +89,13 @@
 
     if not os.path.exists(download_dir):
         os.makedirs(download_dir)
 
     metadata = load_jl(metadata_path)
     img_queries = _filter_queries(_build_queries(metadata), download_dir)
 
-    for query in tqdm(img_queries, desc='Fetch File Progress'):
+    for query in tqdm(img_queries, desc="Fetch File Progress"):
         try:
-            download(query['identifier'],
-                     files=query['filename'],
-                     destdir=download_dir)
+            download(query["identifier"], files=query["filename"], destdir=download_dir)
         except (ConnectTimeout, HTTPError) as e:
             # Internet Archive raises 403 Forbidden when item is not available.
             print(e)
```

### Comparing `libquery-0.1.0/libquery/internet_archive/_fetch_metadata.py` & `libquery-0.1.1/libquery/internet_archive/_fetch_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Utility functions for getting metadata from David Rumsey Map Collection.
 """
 
-# pylint: disable=invalid-name,disallowed-name
-
 import os
 import json
 from datetime import datetime, timezone
 from uuid import uuid5, UUID
 from typing import Dict, List, Tuple
 
 import backoff
@@ -16,82 +14,82 @@
 from slugify import slugify
 from tqdm import tqdm
 
 from ..utils.jsonl import load_jl
 from ._typing import MetadataEntry
 
 fields = [
-    'avg_rating',
-    'backup_location',
-    'btih',
-    'call_number',
-    'collection',
-    'contributor',
-    'coverage',
-    'creator',
-    'date',
-    'description',
-    'downloads',
-    'external-identifier',
-    'foldoutcount',
-    'format',
-    'genre',
-    'identifier',
-    'imagecount',
-    'indexflag',
-    'item_size',
-    'language',
-    'licenseurl',
-    'mediatype',
-    'members',
-    'month',
-    'name',
-    'noindex',
-    'num_reviews',
-    'oai_updatedate',
-    'publicdate',
-    'publisher',
-    'related-external-id',
-    'reviewdate',
-    'rights',
-    'scanningcentre',
-    'source',
-    'stripped_tags',
-    'subject',
-    'title',
-    'type',
-    'volume',
-    'week',
-    'year'
+    "avg_rating",
+    "backup_location",
+    "btih",
+    "call_number",
+    "collection",
+    "contributor",
+    "coverage",
+    "creator",
+    "date",
+    "description",
+    "downloads",
+    "external-identifier",
+    "foldoutcount",
+    "format",
+    "genre",
+    "identifier",
+    "imagecount",
+    "indexflag",
+    "item_size",
+    "language",
+    "licenseurl",
+    "mediatype",
+    "members",
+    "month",
+    "name",
+    "noindex",
+    "num_reviews",
+    "oai_updatedate",
+    "publicdate",
+    "publisher",
+    "related-external-id",
+    "reviewdate",
+    "rights",
+    "scanningcentre",
+    "source",
+    "stripped_tags",
+    "subject",
+    "title",
+    "type",
+    "volume",
+    "week",
+    "year",
 ]
 
 
 def _parse(search_result: Dict, query: str) -> MetadataEntry:
     """
     Parse metadata of entries in Internet Archive.
     """
 
     source_data = search_result.item_metadata
-    source = 'Internet Archive'
-    id_in_source = source_data['metadata']['identifier']
+    source = "Internet Archive"
+    id_in_source = source_data["metadata"]["identifier"]
 
     return {
-        'uuid': str(uuid5(UUID(int=0), f'{source}/{id_in_source}')),
-        'url': f'https://archive.org/search?query={query}',
-        'source': source,
-        'idInSource': id_in_source,
-        'accessDate': datetime.now(timezone.utc).isoformat(),
-        'sourceData': source_data,
+        "uuid": str(uuid5(UUID(int=0), f"{source}/{id_in_source}")),
+        "url": f"https://archive.org/search?query={query}",
+        "source": source,
+        "idInSource": id_in_source,
+        "accessDate": datetime.now(timezone.utc).isoformat(),
+        "sourceData": source_data,
     }
 
 
 @backoff.on_exception(backoff.constant, ProxyError)
-def fetch_metadata(queries: List[str],
-                   query_return_dir: str,
-                   deduplicate: bool = True) -> None:
+def fetch_metadata(
+    queries: List[str], query_return_dir: str, deduplicate: bool = True
+) -> None:
     """
     Given the search queries, and store the query results.
 
     Args
     ----
     queries : List[str]
         The search queries.
@@ -103,53 +101,56 @@
         The duplication is checked by idInSource.
     """
 
     if not os.path.exists(query_return_dir):
         os.makedirs(query_return_dir)
 
     for query in queries:
-        print(f'Fetch Metadata from {query}')
+        print(f"Fetch Metadata from {query}")
 
-        query_return_path = f'{query_return_dir}/{slugify(query)}.jsonl'
-        search_results = internetarchive.search_items(
-            query, fields=fields)
+        query_return_path = f"{query_return_dir}/{slugify(query)}.jsonl"
+        search_results = internetarchive.search_items(query, fields=fields)
 
         if deduplicate:
-            entries = [] if not os.path.exists(query_return_path)\
+            entries = (
+                []
+                if not os.path.exists(query_return_path)
                 else load_jl(query_return_path)
-            visited_id_in_source = {d['idInSource'] for d in entries}
+            )
+            visited_id_in_source = {d["idInSource"] for d in entries}
 
-        with open(query_return_path, 'a', encoding='utf-8') as f:
-            for d in tqdm(search_results.iter_as_items(), desc='Progress'):
+        with open(query_return_path, "a", encoding="utf-8") as f:
+            for d in tqdm(search_results.iter_as_items(), desc="Progress"):
                 entry = _parse(d, query)
-                if not deduplicate or entry['idInSource'] not in visited_id_in_source:
-                    f.write(f'{json.dumps(entry)}\n')
+                if not deduplicate or entry["idInSource"] not in visited_id_in_source:
+                    f.write(f"{json.dumps(entry)}\n")
 
 
-def merge_deduplicate_metadata(queries: List[str],
-                               query_return_dir: str) -> Tuple[List, int]:
+def merge_deduplicate_metadata(
+    queries: List[str], query_return_dir: str
+) -> Tuple[List, int]:
     """
     Merge metadata of different queries
     and deduplicate the metadata entries by idInSource.
     For duplicate entries, one is kept and the others are removed.
     Return the merge result and number of duplicates.
 
     TODO: check whether this function should be kept,
     or it should be replaced with _utils.metadata.deduplicate.
     """
 
     entries: List[MetadataEntry] = []
 
     for query in queries:
-        query_return_path = f'{query_return_dir}/{slugify(query)}.jsonl'
+        query_return_path = f"{query_return_dir}/{slugify(query)}.jsonl"
         if os.path.exists(query_return_path):
             entries += load_jl(query_return_path)
 
     # Build the mapping from idInSource to index.
     id2index = {}
     for i, entry in enumerate(entries):
-        if entry['idInSource'] not in id2index:
-            id2index[entry['idInSource']] = i
+        if entry["idInSource"] not in id2index:
+            id2index[entry["idInSource"]] = i
 
     selected_indices = list(id2index.values())
     entries_filtered = [entries[i] for i in selected_indices]
     return entries_filtered
```

### Comparing `libquery-0.1.0/libquery/internet_archive/_querier.py` & `libquery-0.1.1/libquery/internet_archive/_querier.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 from ._fetch_metadata import (
     fetch_metadata,
     merge_deduplicate_metadata,
 )
 from ._fetch_file import fetch_file
 
 
-class Querier(BaseQuerierWithQueryReturn):
+class InternetArchive(BaseQuerierWithQueryReturn):
     """
     The querier for the `Internet Archive` data source.
     """
 
-    def __init__(self, metadata_dir: str,
-                 download_dir: str,
-                 img_dir: str):
+    def __init__(self, metadata_dir: str, download_dir: str, img_dir: str):
         """
         Args
         ----
         metadata_path : str
             The file storing the metadata from each query.
         download_dir : str
             The directory storing the downloads from each query.
@@ -34,17 +32,14 @@
         """
 
         self.metadata_dir = metadata_dir
         self.download_dir = download_dir
         self.img_dir = img_dir
 
     def fetch_metadata(self, queries: List[str]) -> None:
-        fetch_metadata(queries,
-                       self.query_return_dir,
-                       deduplicate=True)
-        entries = merge_deduplicate_metadata(
-            queries, self.query_return_dir)
+        fetch_metadata(queries, self.query_return_dir, deduplicate=True)
+        entries = merge_deduplicate_metadata(queries, self.query_return_dir)
         save_jl(entries, self.metadata_path)
 
     def fetch_image(self) -> None:
         fetch_file(self.metadata_path, self.download_dir)
         extract_images(self.download_dir, self.img_dir)
```

### Comparing `libquery-0.1.0/libquery/internet_archive/_typing.py` & `libquery-0.1.1/libquery/internet_archive/_typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 The type declarations specific to the `Internet Archive` data source.
 """
 
-# pylint: disable=too-few-public-methods
-
 from typing import List, TypedDict, Union
 
 from typing_extensions import NotRequired
 
 from ..typing import MetadataEntry as BaseMetadataEntry
 
 
@@ -22,51 +20,54 @@
     crc32: NotRequired[str]
     sha1: NotRequired[str]
     rotation: NotRequired[str]
     original: NotRequired[str]
 
 
 """The data directly returned from the url."""
-InternetArchiveMetadata = TypedDict('InternetArchiveMetadata', {
-    # The identifier that can be used to retrieve the item through
-    # internetarchive.get_item(identifier)
-    'identifier': str,
-    'mediatype': str,
-    'title': str,
-    'publicdate': str,
-    'uploader': str,
-    'addeddate': str,
-    'collection': Union[List[str], str],
-    'description': NotRequired[Union[List[str], str]],
-    'call_number': NotRequired[str],
-    # The entries' corresponding location
-    'coverage': NotRequired[Union[List[str], str]],
-    'creator': NotRequired[Union[List[str], str]],
-    # The publication date.
-    'date': NotRequired[Union[List[str], str]],
-    # The number of times the item has been viewed on archive.org
-    'external-identifier': NotRequired[Union[List[str], str]],
-    'format': NotRequired[str],
-    'language': NotRequired[Union[List[str], str]],
-    'map-type': NotRequired[Union[List[str], str]],
-    'publisher': NotRequired[Union[List[str], str]],
-    # Copyright information
-    'rights': NotRequired[str],
-    'scanner': NotRequired[str],
-    'size': NotRequired[str],
-    # The url of the entry in the original data source.
-    'source': NotRequired[str],
-    'subject': NotRequired[Union[List[str], str]],
-    # The warning about the metadata.
-    'warning': NotRequired[str],
-    'year': NotRequired[str],
-    'isbn': NotRequired[Union[List[str], str]],
-    'issn': NotRequired[str],
-    'date_range': NotRequired[str]
-})
+InternetArchiveMetadata = TypedDict(
+    "InternetArchiveMetadata",
+    {
+        # The identifier that can be used to retrieve the item through
+        # internetarchive.get_item(identifier)
+        "identifier": str,
+        "mediatype": str,
+        "title": str,
+        "publicdate": str,
+        "uploader": str,
+        "addeddate": str,
+        "collection": Union[List[str], str],
+        "description": NotRequired[Union[List[str], str]],
+        "call_number": NotRequired[str],
+        # The entries' corresponding location
+        "coverage": NotRequired[Union[List[str], str]],
+        "creator": NotRequired[Union[List[str], str]],
+        # The publication date.
+        "date": NotRequired[Union[List[str], str]],
+        # The number of times the item has been viewed on archive.org
+        "external-identifier": NotRequired[Union[List[str], str]],
+        "format": NotRequired[str],
+        "language": NotRequired[Union[List[str], str]],
+        "map-type": NotRequired[Union[List[str], str]],
+        "publisher": NotRequired[Union[List[str], str]],
+        # Copyright information
+        "rights": NotRequired[str],
+        "scanner": NotRequired[str],
+        "size": NotRequired[str],
+        # The url of the entry in the original data source.
+        "source": NotRequired[str],
+        "subject": NotRequired[Union[List[str], str]],
+        # The warning about the metadata.
+        "warning": NotRequired[str],
+        "year": NotRequired[str],
+        "isbn": NotRequired[Union[List[str], str]],
+        "issn": NotRequired[str],
+        "date_range": NotRequired[str],
+    },
+)
 
 
 class SourceData(TypedDict):
     created: int
     d1: str
     d2: str
     dir: str
@@ -80,8 +81,9 @@
     workable_servers: List[str]
     reviews: NotRequired[List[str]]
     servers_unavailable: NotRequired[bool]
 
 
 class MetadataEntry(BaseMetadataEntry):
     """The data structure of an entry in the metadata."""
+
     sourceData: SourceData
```

### Comparing `libquery-0.1.0/libquery/library_of_congress/_fetch_metadata.py` & `libquery-0.1.1/libquery/library_of_congress/_fetch_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,82 +11,82 @@
 from tqdm import tqdm
 
 from ..utils.jsonl import load_jl
 from ..utils.metadata import deduplicate, filter_queries
 from ._typing import MetadataEntry
 
 
-def _fetch_num_pages(base_url: str,
-                    records_per_page: Literal[25, 50, 100, 150]) -> Union[int, None]:
+def _fetch_num_pages(
+    base_url: str, records_per_page: Literal[25, 50, 100, 150]
+) -> Union[int, None]:
     """
     Get the number of found pages, given the search base url.
 
     Note
     ----
     Library of congress only allow records_per_page in [25, 50, 100, 150].
     """
 
-    pagination_url = f'{base_url}&at=pagination&c={records_per_page}'
+    pagination_url = f"{base_url}&at=pagination&c={records_per_page}"
     response = requests.get(pagination_url)
     if response.status_code == 403:
-        print('403 Forbidden at', pagination_url)
+        print("403 Forbidden at", pagination_url)
         return None
-    return response.json()['pagination']['total']
+    return response.json()["pagination"]["total"]
 
 
-def _build_queries(base_urls: List[str],
-                  metadata_path: str) -> List[str]:
+def _build_queries(base_urls: List[str], metadata_path: str) -> List[str]:
     """
     Build a list of urls to query.
     """
 
     # Number of entries per page (i.e., per query).
     records_per_page = 25
 
     queries = []
     for base_url in base_urls:
         n_pages = _fetch_num_pages(base_url, records_per_page)
         if n_pages is None:
             continue
         # The first page is indexed 1 in the database.
-        queries += [f'{base_url}&sp={i+1}&c={records_per_page}'
-                    for i in range(n_pages)]
+        queries += [f"{base_url}&sp={i+1}&c={records_per_page}" for i in range(n_pages)]
     return filter_queries(queries, metadata_path)
 
 
 def _parse(response: Response) -> List[MetadataEntry]:
     """
     Parse metadata of entries in Library of Congress.
     """
 
     data = response.json()
-    if 'results' not in data:
+    if "results" not in data:
         return []
 
     entries: List[MetadataEntry] = []
-    for result in data['results']:
-        is_image = 'image_url' in result and len(result['image_url']) >= 1
-        if (not is_image) or ('item' not in result):
+    for result in data["results"]:
+        is_image = "image_url" in result and len(result["image_url"]) >= 1
+        if (not is_image) or ("item" not in result):
             continue
-        source = 'Library of Congress'
-        id_in_source = result['id'].split('/')[-2]
-        entries.append({
-            'uuid': str(uuid5(UUID(int=0), f'{source}/{id_in_source}')),
-            'url': response.url,
-            'source': source,
-            'idInSource': id_in_source,
-            'accessDate': datetime.now(timezone.utc).isoformat(),
-            'sourceData': result,
-        })
+        source = "Library of Congress"
+        id_in_source = result["id"].split("/")[-2]
+        entries.append(
+            {
+                "uuid": str(uuid5(UUID(int=0), f"{source}/{id_in_source}")),
+                "url": response.url,
+                "source": source,
+                "idInSource": id_in_source,
+                "accessDate": datetime.now(timezone.utc).isoformat(),
+                "sourceData": result,
+            }
+        )
     return entries
 
 
 @backoff.on_exception(backoff.constant, (ProxyError, SSLError))
-def fetch_metadata(base_urls: List[str],
-                   metadata_path: str) -> None:
+def fetch_metadata(base_urls: List[str], metadata_path: str) -> None:
     """
     Given base urls, generate metadata queries, and store the query results.
 
     Args
     ----
     base_urls : List[str]
         The base urls for generating queries.
@@ -95,32 +95,31 @@
         The path to the folder for storing the metadata.
     """
 
     output_dir = os.path.dirname(metadata_path)
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
-    metadata = [] if not os.path.exists(metadata_path)\
-        else load_jl(metadata_path)
+    metadata = [] if not os.path.exists(metadata_path) else load_jl(metadata_path)
 
-    queried_view_urls = [d['sourceData']['url'] for d in metadata]
+    queried_view_urls = [d["sourceData"]["url"] for d in metadata]
 
     # TODO: store the query result of each query in an individual jsonl to:
     # 1. reduce file size
     # 2. allow deduplication in the merged jsonl without removing
     # the original queried record, which cause query progress to be lost
 
     # TODO: make the progress logging scheme consistent with other data sources
 
     # Each query queries a page with multiple entries.
     queries = _build_queries(base_urls, metadata_path)
-    with open(metadata_path, 'a', encoding='utf-8') as f:
-        for query in tqdm(queries, desc='Fetch Metadata Progress'):
+    with open(metadata_path, "a", encoding="utf-8") as f:
+        for query in tqdm(queries, desc="Fetch Metadata Progress"):
             response = requests.get(query)
             entries = _parse(response)
             for d in entries:
-                if d['sourceData']['url'] not in queried_view_urls:
-                    f.write(f'{json.dumps(d, ensure_ascii=False)}\n')
+                if d["sourceData"]["url"] not in queried_view_urls:
+                    f.write(f"{json.dumps(d, ensure_ascii=False)}\n")
 
     # For duplicate entries (returned by different search queries),
     # only keep the latest one.
     # deduplicate(metadata_path)
```

### Comparing `libquery-0.1.0/libquery/library_of_congress/_querier.py` & `libquery-0.1.1/libquery/david_rumsey_map_collection/_querier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 """
 The entrance to querier class.
 """
 
 from typing import List
 
-from ..base import BaseQuerier
+from ..base import BaseQuerierWithQueryReturn
 from ..typing import ImageQuery
 from ..utils.image import fetch as fetch_image
-from ._fetch_metadata import fetch_metadata
-from ._typing import MetadataEntry
+from ..utils.jsonl import save_jl
+from ..utils.metadata import deduplicate
+from ._fetch_metadata import fetch_metadata, merge_metadata
+from ._typing import MetadataEntry, SourceData
+
+
+def _get_download_url(source_data: SourceData) -> str:
+    return (
+        source_data["urlSize4"]
+        if "urlSize4" in source_data
+        else source_data["urlSize2"]
+    )
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
-    """
-    Build a list of image urls to query.
-    """
+    """Build a list of image urls to query."""
 
-    return [{
-        'url': d['sourceData']['image_url'][-1],
-        'uuid': d['uuid'],
-    } for d in metadata]
+    return [
+        {
+            "url": _get_download_url(d["sourceData"]),
+            "uuid": d["uuid"],
+        }
+        for d in metadata
+    ]
 
 
-class Querier(BaseQuerier):
+class DavidRumseyMapCollection(BaseQuerierWithQueryReturn):
     """
-    The querier for the `Library of Congress` data source.
+    The querier for the `David Rumsey Map Collection` data source.
     """
 
-    def __init__(self, metadata_path: str,
-                 img_dir: str):
+    def fetch_metadata(self, queries: List[str]) -> None:
         """
         Args
         ----
-        metadata_path : str
-            The file storing the metadata from each query.
-        img_dir : str
-            The directory storing the images from each query.
+        queries : List[str]
+            The base urls for which query results are to be stored.
         """
 
-        self.metadata_path = metadata_path
-        self.img_dir = img_dir
-
-    def fetch_metadata(self, queries: List[str]) -> None:
-        fetch_metadata(queries, self.metadata_path)
+        fetch_metadata(queries, self.query_return_dir)
+        entries = merge_metadata(queries, self.query_return_dir)
+        save_jl(entries, self.metadata_path)
+        deduplicate(self.metadata_path)
 
     def fetch_image(self) -> None:
-        fetch_image(self.metadata_path,
-                    self.img_dir,
-                    _build_image_queries)
+        fetch_image(self.metadata_path, self.img_dir, _build_image_queries)
```

### Comparing `libquery-0.1.0/libquery/library_of_congress/_typing.py` & `libquery-0.1.1/libquery/library_of_congress/_typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 The type declarations specific to the `Internet Archive` data source.
 
 See reference on the response data structure at
 <https://www.loc.gov/apis/json-and-yaml/responses/item-and-resource/>
 """
 
-# pylint: disable=too-few-public-methods
-
 from typing import Any, List, TypedDict, Union
 
 from typing_extensions import NotRequired
 
 from ..typing import MetadataEntry as BaseMetadataEntry
 
 
@@ -186,8 +184,9 @@
     reproductions: NotRequired[str]
     unrestricted: NotRequired[bool]
     publication_frequency: NotRequired[List[str]]
 
 
 class MetadataEntry(BaseMetadataEntry):
     """The data structure of an entry in the metadata."""
+
     sourceData: SourceData
```

### Comparing `libquery-0.1.0/libquery/typing.py` & `libquery-0.1.1/libquery/typing.py`

 * *Files identical despite different names*

### Comparing `libquery-0.1.0/libquery/utils/image.py` & `libquery-0.1.1/libquery/utils/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from tqdm import tqdm
 
 from ..typing import ImageQuery, MetadataEntry
 from .jsonl import load_jl
 
 
 def _filename2uuid(filename: str) -> str:
-    return filename.split('.')[0]
+    return filename.split(".")[0]
 
 
 def _try_remove_image(img_dir: str, uuid: str) -> bool:
     """Try removing an image given uuid."""
 
     filenames = os.listdir(img_dir)
     filename = next((d for d in filenames if _filename2uuid(d) == uuid), None)
@@ -36,24 +36,22 @@
     if not os.path.isfile(file_path):
         return False
 
     remove(uuid)
     return True
 
 
-def filter_queries(img_queries: List[ImageQuery],
-                   img_dir: str) -> List[ImageQuery]:
+def filter_queries(img_queries: List[ImageQuery], img_dir: str) -> List[ImageQuery]:
     """
     Filter urls queried before according to the stored images.
     """
 
-    filenames = [d for d in listdir(img_dir)
-                 if isfile(join(img_dir, d))]
+    filenames = [d for d in listdir(img_dir) if isfile(join(img_dir, d))]
     img_uuids = {_filename2uuid(d) for d in filenames}
-    return [d for d in img_queries if d['uuid'] not in img_uuids]
+    return [d for d in img_queries if d["uuid"] not in img_uuids]
 
 
 class IncompleteFileHandler(Enum):
     """The type of handlers when incomplete file is received."""
 
     # Raise error when incomplete file is received.
     RAISE_ERROR = 1
@@ -63,26 +61,31 @@
     SAVE = 3
 
 
 last_uuid = None
 
 
 def _backoff_handler(details: Details) -> None:
-    print('Error occurred. Retry fetching the images:', details)
+    print("Error occurred. Retry fetching the images:", details)
 
-    img_dir = details['args'][1] if 'img_dir' not in details['kwargs']\
-        else details['kwargs']['img_dir']
+    img_dir = (
+        details["args"][1]
+        if "img_dir" not in details["kwargs"]
+        else details["kwargs"]["img_dir"]
+    )
     is_removed = _try_remove_image(img_dir, last_uuid)
     if is_removed:
-        print('remove', last_uuid)
+        print("remove", last_uuid)
 
 
-@backoff.on_exception(backoff.constant,
-                      (ChunkedEncodingError, ProxyError, SSLError),
-                      on_backoff=_backoff_handler)
+@backoff.on_exception(
+    backoff.constant,
+    (ChunkedEncodingError, ProxyError, SSLError),
+    on_backoff=_backoff_handler,
+)
 def fetch(
     metadata_path: str,
     img_dir: str,
     _build_queries: Callable[[List[MetadataEntry]], List[ImageQuery]],
     incomplete_file_handler: IncompleteFileHandler = IncompleteFileHandler.RAISE_ERROR,
 ) -> None:
     """
@@ -100,25 +103,25 @@
         os.makedirs(img_dir)
 
     s = requests.Session()
 
     metadata = load_jl(metadata_path)
     img_queries = filter_queries(_build_queries(metadata), img_dir)
 
-    for query in tqdm(img_queries, desc='Fetch Image Progress'):
-        uuid = query['uuid']
+    for query in tqdm(img_queries, desc="Fetch Image Progress"):
+        uuid = query["uuid"]
         global last_uuid
         last_uuid = uuid
 
         # Note: some database may continuously raise error for a certain resource.
         # It is necessary to ignore such resources instead of keep fetching repeatedly.
         try:
-            response = s.get(query['url'])
+            response = s.get(query["url"])
         except SSLError as e:
-            print(f'Error {e}')
+            print(f"Error {e}")
 
         # 403 Forbidden
         if response.status_code == 403:
             continue
 
         # 429 Too Many Requests
         if response.status_code == 429:
@@ -129,30 +132,36 @@
         if response.status_code == 500:
             continue
 
         # 503 Service Unavailable
         if response.status_code == 503:
             continue
 
-        extension = query['extension'] if 'extension' in query\
-            else mimetypes.guess_extension(response.headers['content-type'])
+        extension = (
+            query["extension"]
+            if "extension" in query
+            else mimetypes.guess_extension(response.headers["content-type"])
+        )
 
         # In some cases, the extension may not be set.
         # For example, when the response is a plain text string.
         if extension is None:
             continue
 
         # If the file is not fully returned, which may frequently happen for large images.
         # Note: there is no guarantee that the server will set the correct content-length.
         # For example, Gallica often returns incorrect 'content-length' even if the image is correctly returned.
-        if 'content-length' in response.headers and len(response.content) != int(response.headers['content-length']):
+        if "content-length" in response.headers and len(response.content) != int(
+            response.headers["content-length"]
+        ):
             print(
-                f'Status code {response.status_code} - File not fully returned for url = {query["url"]}: {len(response.content)} != {response.headers["content-length"]}')
+                f'Status code {response.status_code} - File not fully returned for url = {query["url"]}: {len(response.content)} != {response.headers["content-length"]}'
+            )
             if incomplete_file_handler == IncompleteFileHandler.RAISE_ERROR:
                 raise ProxyError()
             elif incomplete_file_handler == IncompleteFileHandler.IGNORE:
                 continue
             elif incomplete_file_handler == IncompleteFileHandler.SAVE:
                 pass
 
-        with open(f'{img_dir}/{uuid}{extension}', 'wb') as f:
+        with open(f"{img_dir}/{uuid}{extension}", "wb") as f:
             f.write(response.content)
```

### Comparing `libquery-0.1.0/libquery/utils/metadata.py` & `libquery-0.1.1/libquery/utils/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     metadata_path : str
         The path to the metadata to be read and edited.
     """
 
     entries = load_jl(metadata_path)
     id_in_source_to_entry = {}
     for d in entries:
-        id_in_source = d['idInSource']
+        id_in_source = d["idInSource"]
         if id_in_source not in id_in_source_to_entry:
             id_in_source_to_entry[id_in_source] = d
             continue
         prev_access_date = parser.parse(
-            id_in_source_to_entry[id_in_source]['accessDate'])
-        new_access_date = parser.parse(d['accessDate'])
+            id_in_source_to_entry[id_in_source]["accessDate"]
+        )
+        new_access_date = parser.parse(d["accessDate"])
         if new_access_date > prev_access_date:
             id_in_source_to_entry[id_in_source] = d
     save_jl(id_in_source_to_entry.values(), metadata_path)
 
 
-def filter_queries(queries: List[str],
-                   metadata_path: str) -> List[str]:
+def filter_queries(queries: List[str], metadata_path: str) -> List[str]:
     """
     Filter stale queries.
     Discard the metadata queries that have been executed
     in the recent 30 days.
     """
 
     metadata: List[MetadataEntry] = []
@@ -53,12 +53,12 @@
 
     # Regard the data queried 30 days ago as stale.
     # Stale queries will be executed again.
     stale_threshold = 30
     now = datetime.now(timezone.utc)
     queried_urls = set()
     for d in metadata:
-        access_date = parser.parse(d['accessDate'])
+        access_date = parser.parse(d["accessDate"])
         delta = now - access_date
         if delta.days < stale_threshold:
-            queried_urls.add(d['url'])
+            queried_urls.add(d["url"])
     return [d for d in queries if d not in queried_urls]
```

### Comparing `libquery-0.1.0/pyproject.toml` & `libquery-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libquery"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Yu Zhang <yuzhang94@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

