# Comparing `tmp/mumee-0.0.3.tar.gz` & `tmp/mumee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mumee-0.0.3.tar", max compression
+gzip compressed data, was "mumee-0.0.4.tar", max compression
```

## Comparing `mumee-0.0.3.tar` & `mumee-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1063 2023-07-17 16:42:04.835913 mumee-0.0.3/LICENSE
--rw-r--r--   0        0        0     2317 2023-07-17 16:42:04.835913 mumee-0.0.3/README.md
--rw-r--r--   0        0        0      520 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/__init__.py
--rw-r--r--   0        0        0      328 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/__init__.py
--rw-r--r--   0        0        0      180 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/clients/__init__.py
--rw-r--r--   0        0        0     5390 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/clients/spotify_metadata_client.py
--rw-r--r--   0        0        0     4960 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/clients/ytmusic_metadata_client.py
--rw-r--r--   0        0        0       74 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/config/__init__.py
--rw-r--r--   0        0        0      419 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/config/spotify_options.py
--rw-r--r--   0        0        0      532 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/__init__.py
--rw-r--r--   0        0        0      705 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/spotify_playlist_handler.py
--rw-r--r--   0        0        0      652 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/spotify_search_handler.py
--rw-r--r--   0        0        0      693 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/spotify_track_handler.py
--rw-r--r--   0        0        0      711 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/ytmusic_playlist_handler.py
--rw-r--r--   0        0        0      652 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/ytmusic_search_handler.py
--rw-r--r--   0        0        0      696 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/handlers/ytmusic_track_handler.py
--rw-r--r--   0        0        0      249 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/playlist_metadata.py
--rw-r--r--   0        0        0      456 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/classes/song_metadata.py
--rw-r--r--   0        0        0       68 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/di/__init__.py
--rw-r--r--   0        0        0      800 2023-07-17 16:42:04.835913 mumee-0.0.3/mumee/di/dependency_injector.py
--rw-r--r--   0        0        0       90 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/errors/__init__.py
--rw-r--r--   0        0        0       83 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/errors/metadata_client_error.py
--rw-r--r--   0        0        0       87 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/interfaces/__init__.py
--rw-r--r--   0        0        0      231 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/interfaces/base_metadata_client.py
--rw-r--r--   0        0        0      878 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/main.py
--rw-r--r--   0        0        0        0 2023-07-17 16:42:04.839913 mumee-0.0.3/mumee/py.typed
--rw-r--r--   0        0        0     1324 2023-07-17 16:42:04.839913 mumee-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 mumee-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-19 09:03:39.990929 mumee-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2311 2023-07-19 09:03:39.990929 mumee-0.0.4/README.md
+-rw-r--r--   0        0        0      520 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/classes/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/classes/clients/__init__.py
+-rw-r--r--   0        0        0     5715 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/clients/spotify_metadata_client.py
+-rw-r--r--   0        0        0     5439 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/clients/ytmusic_metadata_client.py
+-rw-r--r--   0        0        0       74 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/config/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/config/spotify_options.py
+-rw-r--r--   0        0        0      532 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_playlist_handler.py
+-rw-r--r--   0        0        0      652 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_search_handler.py
+-rw-r--r--   0        0        0      693 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_track_handler.py
+-rw-r--r--   0        0        0      711 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_playlist_handler.py
+-rw-r--r--   0        0        0      652 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_search_handler.py
+-rw-r--r--   0        0        0      696 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_track_handler.py
+-rw-r--r--   0        0        0      249 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/playlist_metadata.py
+-rw-r--r--   0        0        0      557 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/song_metadata.py
+-rw-r--r--   0        0        0       68 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/di/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/di/dependency_injector.py
+-rw-r--r--   0        0        0       90 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/errors/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/errors/metadata_client_error.py
+-rw-r--r--   0        0        0       87 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/interfaces/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/interfaces/base_metadata_client.py
+-rw-r--r--   0        0        0      904 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/py.typed
+-rw-r--r--   0        0        0     1324 2023-07-19 09:03:39.994929 mumee-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 mumee-0.0.4/PKG-INFO
```

### Comparing `mumee-0.0.3/LICENSE` & `mumee-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/README.md` & `mumee-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Song Metadata Client
+# Mumee
 
-**Get metadata about your favorite songs and playlists !**
+**Get metadata about your favorite songs and playlists !**  
+Mumee stands for *MUsic MEtadata Explorer*
 
 ## Features
 
 - Automatic metadata fetching from different services
   - Currently supported : Spotify, Youtube Music
 - Metadata fetching from an URL or a query
 - Supports playlist URLs
@@ -77,10 +78,10 @@
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
-- Interface for SongMetadataClient and only exposed interface for DI ?
 - Support for Amazon Music
 - More metadata in the SongMetadata class
+- Allow return of multiple results
```

### Comparing `mumee-0.0.3/mumee/__init__.py` & `mumee-0.0.4/mumee/__init__.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/clients/spotify_metadata_client.py` & `mumee-0.0.4/mumee/classes/clients/spotify_metadata_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,29 +63,39 @@
 
         return self._to_song_metadata(track_info)
 
     def _to_song_metadata(self, track_info: Dict[str, Any]) -> SongMetadata:
         artist_names = [artist["name"] for artist in track_info["artists"]]
         album_info = self._client.album(track_info["album"]["id"]) or {}
 
+        thumbnails = [
+            (tn["width"] * tn["height"], tn["url"]) for tn in album_info["images"]
+        ]
+
         result = SongMetadata(
             name=track_info["name"],
             artists=artist_names,
             artist=artist_names[0],
             album_name=album_info["name"],
             album_artist=album_info["artists"][0]["name"],
             disc_number=track_info["disc_number"],
             disc_count=int(album_info["tracks"]["items"][-1]["disc_number"]),
             track_number=track_info["track_number"],
             track_count=album_info["total_tracks"],
             genres=album_info["genres"],
-            duration=track_info["duration_ms"] / 1000,
+            duration=int(track_info["duration_ms"] / 1000),
             date=album_info["release_date"],
             year=int(album_info["release_date"][:4]),
+            is_song=True,
+            id=track_info["id"],
+            explicit=track_info["explicit"],
+            cover_url=max(thumbnails)[1],
+            url=track_info["external_urls"]["spotify"],
         )
+
         return result
 
     def get_playlist(self, url: str) -> PlaylistMetadata:
         if "open.spotify.com" not in url or "playlist" not in url:
             raise MetadataClientError(f"Invalid Spotify playlist URL: {url}")
 
         track_info = self._client.playlist(url)
```

### Comparing `mumee-0.0.3/mumee/classes/clients/ytmusic_metadata_client.py` & `mumee-0.0.4/mumee/classes/clients/ytmusic_metadata_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,19 @@
 
         track_info = best_result[0]
         if track_info.get("album", {}).get("id") is not None:
             album_info = self._client.get_album(track_info["album"]["id"])
         else:
             album_info = None
 
+        thumbnails = [
+            (tn["width"] * tn["height"], tn["url"])
+            for tn in (album_info if album_info else track_info)["thumbnails"]
+        ]
+
         result = SongMetadata(
             name=track_info["title"],
             artists=[artist["name"] for artist in track_info["artists"]],
             artist=track_info["artists"][0]["name"],
             album_name=album_info["title"] if album_info is not None else None,
             album_artist=album_info["artists"][0]["name"]
             if album_info is not None
@@ -94,14 +99,19 @@
             if album_info is not None
             else None,
             track_count=album_info["trackCount"] if album_info is not None else None,
             genres=[],
             duration=track_info["duration_seconds"],
             date=None,
             year=int(album_info["year"]) if album_info is not None else None,
+            explicit=track_info["isExplicit"],
+            cover_url=max(thumbnails)[1],
+            is_song=track_info["resultType"] == "song",
+            id=track_info["videoId"],
+            url=f"https://{'music' if track_info['resultType'] == 'song' else 'www'}.youtube.com/watch?v={track_info['videoId']}",
         )
 
         return result
 
     def _get_best_result(
         self, query: str, tracks_info: List[Dict[str, Any]]
     ) -> Tuple[Dict[str, Any], str, float]:
```

### Comparing `mumee-0.0.3/mumee/classes/handlers/__init__.py` & `mumee-0.0.4/mumee/classes/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/spotify_playlist_handler.py` & `mumee-0.0.4/mumee/classes/handlers/spotify_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/spotify_search_handler.py` & `mumee-0.0.4/mumee/classes/handlers/spotify_search_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/spotify_track_handler.py` & `mumee-0.0.4/mumee/classes/handlers/spotify_track_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/ytmusic_playlist_handler.py` & `mumee-0.0.4/mumee/classes/handlers/ytmusic_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/ytmusic_search_handler.py` & `mumee-0.0.4/mumee/classes/handlers/ytmusic_search_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/classes/handlers/ytmusic_track_handler.py` & `mumee-0.0.4/mumee/classes/handlers/ytmusic_track_handler.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/di/dependency_injector.py` & `mumee-0.0.4/mumee/di/dependency_injector.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.3/mumee/main.py` & `mumee-0.0.4/mumee/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 
         self._client = services.build().resolve(BaseMetadataClient)
 
     def search(self, url_or_query: str) -> Union[SongMetadata, PlaylistMetadata]:
         result = self._client.exec(url_or_query)
 
         if result is None:
-            raise MetadataClientError("No result")
+            raise MetadataClientError(f"No result for query {url_or_query}")
 
         return result
```

### Comparing `mumee-0.0.3/pyproject.toml` & `mumee-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Mumee"
-version = "0.0.3"
+version = "0.0.4"
 description = "MUsic MEtadata Explorer"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mumee"}]
 
 keywords = ["mumee", "metadata", "python", "song metadata", "spotify", "youtube", "youtube music", "music", "song"]
```

### Comparing `mumee-0.0.3/PKG-INFO` & `mumee-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumee
-Version: 0.0.3
+Version: 0.0.4
 Summary: MUsic MEtadata Explorer
 Home-page: https://github.com/Billuc/Mumee
 License: MIT
 Keywords: mumee,metadata,python,song metadata,spotify,youtube,youtube music,music,song
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -23,17 +23,18 @@
 Requires-Dist: spotipy (>=2.23.0,<3.0.0)
 Requires-Dist: taipan-di (>=0.0.7,<0.0.8)
 Requires-Dist: ytmusicapi (>=1.0.2,<2.0.0)
 Project-URL: Documentation, https://github.com/Billuc/Mumee
 Project-URL: Repository, https://github.com/Billuc/Mumee
 Description-Content-Type: text/markdown
 
-# Song Metadata Client
+# Mumee
 
-**Get metadata about your favorite songs and playlists !**
+**Get metadata about your favorite songs and playlists !**  
+Mumee stands for *MUsic MEtadata Explorer*
 
 ## Features
 
 - Automatic metadata fetching from different services
   - Currently supported : Spotify, Youtube Music
 - Metadata fetching from an URL or a query
 - Supports playlist URLs
@@ -106,11 +107,11 @@
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
-- Interface for SongMetadataClient and only exposed interface for DI ?
 - Support for Amazon Music
 - More metadata in the SongMetadata class
+- Allow return of multiple results
```

