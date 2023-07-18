# Comparing `tmp/aiosu-1.5.0.tar.gz` & `tmp/aiosu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosu-1.5.0.tar", max compression
+gzip compressed data, was "aiosu-2.0.0.tar", max compression
```

## Comparing `aiosu-1.5.0.tar` & `aiosu-2.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    35149 2023-04-17 12:54:11.518455 aiosu-1.5.0/LICENSE
--rw-r--r--   0        0        0     3855 2023-04-17 12:54:11.518455 aiosu-1.5.0/README.rst
--rw-r--r--   0        0        0      675 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/__init__.py
--rw-r--r--   0        0        0     2318 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/events.py
--rw-r--r--   0        0        0      736 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/exceptions.py
--rw-r--r--   0        0        0     1790 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/helpers.py
--rw-r--r--   0        0        0      664 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/artist.py
--rw-r--r--   0        0        0      406 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/backgrounds.py
--rw-r--r--   0        0        0      883 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/base.py
--rw-r--r--   0        0        0    13819 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/beatmap.py
--rw-r--r--   0        0        0     1954 2023-04-17 12:54:11.518455 aiosu-1.5.0/aiosu/models/changelog.py
--rw-r--r--   0        0        0     1639 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/chat.py
--rw-r--r--   0        0        0     1519 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/comment.py
--rw-r--r--   0        0        0     2280 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/common.py
--rw-r--r--   0        0        0     1624 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/event.py
--rw-r--r--   0        0        0     1633 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/forum.py
--rw-r--r--   0        0        0     1976 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/gamemode.py
--rw-r--r--   0        0        0      742 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/kudosu.py
--rw-r--r--   0        0        0     5058 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/lazer.py
--rw-r--r--   0        0        0       79 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/__init__.py
--rw-r--r--   0        0        0     3123 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/match.py
--rw-r--r--   0        0        0      272 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/legacy/replay.py
--rw-r--r--   0        0        0     6076 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/mods.py
--rw-r--r--   0        0        0     4487 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/multiplayer.py
--rw-r--r--   0        0        0     1038 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/news.py
--rw-r--r--   0        0        0     1808 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/oauthtoken.py
--rw-r--r--   0        0        0      843 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/performance.py
--rw-r--r--   0        0        0      672 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/rankings.py
--rw-r--r--   0        0        0     2845 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/replay.py
--rw-r--r--   0        0        0     1241 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/scopes.py
--rw-r--r--   0        0        0     7512 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/score.py
--rw-r--r--   0        0        0      480 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/search.py
--rw-r--r--   0        0        0      387 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/spotlight.py
--rw-r--r--   0        0        0     8983 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/user.py
--rw-r--r--   0        0        0      372 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/models/wiki.py
--rw-r--r--   0        0        0      241 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/__init__.py
--rw-r--r--   0        0        0     8815 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/accuracy.py
--rw-r--r--   0        0        0     2936 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/auth.py
--rw-r--r--   0        0        0     7905 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/binary.py
--rw-r--r--   0        0        0    22091 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/performance.py
--rw-r--r--   0        0        0     6091 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/utils/replay.py
--rw-r--r--   0        0        0      106 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v1/__init__.py
--rw-r--r--   0        0        0    17864 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v1/client.py
--rw-r--r--   0        0        0      154 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/__init__.py
--rw-r--r--   0        0        0    88480 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/client.py
--rw-r--r--   0        0        0     7691 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/clientstorage.py
--rw-r--r--   0        0        0      103 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/repository/__init__.py
--rw-r--r--   0        0        0     1905 2023-04-17 12:54:11.522456 aiosu-1.5.0/aiosu/v2/repository/oauthtoken.py
--rw-r--r--   0        0        0        0 2023-04-17 12:54:11.522456 aiosu-1.5.0/py.typed
--rw-r--r--   0        0        0     1845 2023-04-17 12:54:11.522456 aiosu-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 aiosu-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-18 23:05:06.015366 aiosu-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3860 2023-07-18 23:05:06.015366 aiosu-2.0.0/README.rst
+-rw-r--r--   0        0        0      675 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/__init__.py
+-rw-r--r--   0        0        0     2318 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/events.py
+-rw-r--r--   0        0        0      736 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/exceptions.py
+-rw-r--r--   0        0        0     1790 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/helpers.py
+-rw-r--r--   0        0        0      664 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/__init__.py
+-rw-r--r--   0        0        0     1149 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/artist.py
+-rw-r--r--   0        0        0      406 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/backgrounds.py
+-rw-r--r--   0        0        0      874 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/base.py
+-rw-r--r--   0        0        0    14988 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/beatmap.py
+-rw-r--r--   0        0        0     2175 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/changelog.py
+-rw-r--r--   0        0        0     1746 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/chat.py
+-rw-r--r--   0        0        0     1652 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/comment.py
+-rw-r--r--   0        0        0     2545 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/common.py
+-rw-r--r--   0        0        0     1715 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/event.py
+-rw-r--r--   0        0        0     1696 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/forum.py
+-rw-r--r--   0        0        0     1976 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/gamemode.py
+-rw-r--r--   0        0        0      763 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/kudosu.py
+-rw-r--r--   0        0        0     5638 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/lazer.py
+-rw-r--r--   0        0        0       79 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/legacy/__init__.py
+-rw-r--r--   0        0        0     3358 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/legacy/match.py
+-rw-r--r--   0        0        0      272 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/legacy/replay.py
+-rw-r--r--   0        0        0     6536 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/mods.py
+-rw-r--r--   0        0        0     4610 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/multiplayer.py
+-rw-r--r--   0        0        0     1074 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/news.py
+-rw-r--r--   0        0        0     1941 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/oauthtoken.py
+-rw-r--r--   0        0        0      843 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/performance.py
+-rw-r--r--   0        0        0      693 2023-07-18 23:05:06.015366 aiosu-2.0.0/aiosu/models/rankings.py
+-rw-r--r--   0        0        0     2855 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/replay.py
+-rw-r--r--   0        0        0     1241 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/scopes.py
+-rw-r--r--   0        0        0     7800 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/score.py
+-rw-r--r--   0        0        0      494 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/search.py
+-rw-r--r--   0        0        0      394 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/spotlight.py
+-rw-r--r--   0        0        0    10151 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/user.py
+-rw-r--r--   0        0        0      386 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/models/wiki.py
+-rw-r--r--   0        0        0      241 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/__init__.py
+-rw-r--r--   0        0        0     8815 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/accuracy.py
+-rw-r--r--   0        0        0     2941 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/auth.py
+-rw-r--r--   0        0        0     7905 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/binary.py
+-rw-r--r--   0        0        0    22091 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/performance.py
+-rw-r--r--   0        0        0     6182 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/utils/replay.py
+-rw-r--r--   0        0        0      106 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v1/__init__.py
+-rw-r--r--   0        0        0    17958 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v1/client.py
+-rw-r--r--   0        0        0      154 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v2/__init__.py
+-rw-r--r--   0        0        0    90367 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v2/client.py
+-rw-r--r--   0        0        0     7691 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v2/clientstorage.py
+-rw-r--r--   0        0        0      103 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v2/repository/__init__.py
+-rw-r--r--   0        0        0     1905 2023-07-18 23:05:06.019366 aiosu-2.0.0/aiosu/v2/repository/oauthtoken.py
+-rw-r--r--   0        0        0        0 2023-07-18 23:05:06.019366 aiosu-2.0.0/py.typed
+-rw-r--r--   0        0        0     1816 2023-07-18 23:05:06.019366 aiosu-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 aiosu-2.0.0/PKG-INFO
```

### Comparing `aiosu-1.5.0/LICENSE` & `aiosu-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/README.rst` & `aiosu-2.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     import aiosu
     import asyncio
     import datetime
 
 
     async def main():
-        token = aiosu.models.OAuthToken.parse_obj(json_token_from_api)
+        token = aiosu.models.OAuthToken.model_validate(json_token_from_api)
 
         # or
 
         token = aiosu.models.OAuthToken(
             access_token="access token",
             refresh_token="refresh token",
             expires_on=datetime.datetime.utcnow()
```

### Comparing `aiosu-1.5.0/aiosu/__init__.py` & `aiosu-2.0.0/aiosu/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/events.py` & `aiosu-2.0.0/aiosu/events.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/exceptions.py` & `aiosu-2.0.0/aiosu/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/helpers.py` & `aiosu-2.0.0/aiosu/helpers.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/models/__init__.py` & `aiosu-2.0.0/aiosu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/models/artist.py` & `aiosu-2.0.0/aiosu/models/artist.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,28 +36,28 @@
     is_new: bool
     cover_url: str
 
 
 class ArtistTrack(BaseModel):
     id: int
     artist_id: int
-    bpm: int
+    bpm: float
     cover_url: str
     exclusive: bool
     genre: str
     is_new: bool
     length: str
     title: str
     artist: Artist
     osz_url: str = Field(alias="osz")
     preview_url: str = Field(alias="preview")
-    album: Optional[Album]
-    album_id: Optional[int]
-    updated_at: Optional[datetime]
-    version: Optional[str]
+    album: Optional[Album] = None
+    album_id: Optional[int] = None
+    updated_at: Optional[datetime] = None
+    version: Optional[str] = None
 
 
 class ArtistResponse(CursorModel):
     """Artist response model."""
 
     artist_tracks: list[ArtistTrack]
-    search: Optional[ArtistSearch]
+    search: Optional[ArtistSearch] = None
```

### Comparing `aiosu-1.5.0/aiosu/models/beatmap.py` & `aiosu-2.0.0/aiosu/models/beatmap.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from datetime import datetime
 from enum import Enum
 from enum import unique
 from typing import Any
 from typing import Literal
 from typing import Optional
 
+from pydantic import computed_field
 from pydantic import Field
-from pydantic import root_validator
+from pydantic import model_validator
 
 from .base import BaseModel
 from .common import CursorModel
 from .gamemode import Gamemode
 from .user import User
 
 __all__ = (
@@ -133,41 +134,48 @@
             for status in list(BeatmapRankStatus):
                 if status.name_api == query.lower():
                     return status
         raise ValueError(f"BeatmapRankStatus {query} does not exist.")
 
 
 class BeatmapAvailability(BaseModel):
-    more_information: Optional[str]
-    download_disabled: Optional[bool]
+    more_information: Optional[str] = None
+    download_disabled: Optional[bool] = None
 
     @classmethod
     def _from_api_v1(cls, data: Any) -> BeatmapAvailability:
-        return cls.parse_obj({"download_disabled": data["download_unavailable"]})
+        return cls.model_validate({"download_disabled": data["download_unavailable"]})
 
 
 class BeatmapNominations(BaseModel):
-    current: Optional[int]
-    required: Optional[int]
+    current: Optional[int] = None
+    required: Optional[int] = None
+
+
+class BeatmapNomination(BaseModel):
+    beatmapset_id: int
+    reset: bool
+    user_id: int
+    rulesets: Optional[list[Gamemode]] = None
 
 
 class BeatmapCovers(BaseModel):
     cover: str
     card: str
     list: str
     slimcover: str
-    cover_2_x: Optional[str] = Field(alias="cover@2x")
-    card_2_x: Optional[str] = Field(alias="card@2x")
-    list_2_x: Optional[str] = Field(alias="list@2x")
-    slimcover_2_x: Optional[str] = Field(alias="slimcover@2x")
+    cover_2_x: Optional[str] = Field(default=None, alias="cover@2x")
+    card_2_x: Optional[str] = Field(default=None, alias="card@2x")
+    list_2_x: Optional[str] = Field(default=None, alias="list@2x")
+    slimcover_2_x: Optional[str] = Field(default=None, alias="slimcover@2x")
 
     @classmethod
     def from_beatmapset_id(cls, beatmapset_id: int) -> BeatmapCovers:
         base_url = "https://assets.ppy.sh/beatmaps/"
-        return cls.parse_obj(
+        return cls.model_validate(
             {
                 "cover": f"{base_url}{beatmapset_id}/covers/cover.jpg",
                 "card": f"{base_url}{beatmapset_id}/covers/card.jpg",
                 "list": f"{base_url}{beatmapset_id}/covers/list.jpg",
                 "slimcover": f"{base_url}{beatmapset_id}/covers/slimcover.jpg",
                 "cover_2_x": f"{base_url}{beatmapset_id}/covers/cover@2x.jpg",
                 "card_2_x": f"{base_url}{beatmapset_id}/covers/card@2x.jpg",
@@ -183,83 +191,86 @@
 
 class BeatmapHype(BaseModel):
     current: int
     required: int
 
 
 class BeatmapFailtimes(BaseModel):
-    exit: Optional[list[int]]
-    fail: Optional[list[int]]
+    exit: Optional[list[int]] = None
+    fail: Optional[list[int]] = None
 
 
 class BeatmapDifficultyAttributes(BaseModel):
     max_combo: int
     star_rating: float
     # osu standard
-    aim_difficulty: Optional[float]
-    approach_rate: Optional[float]  # osu catch + standard
-    flashlight_difficulty: Optional[float]
-    overall_difficulty: Optional[float]
-    slider_factor: Optional[float]
-    speed_difficulty: Optional[float]
-    speed_note_count: Optional[float]
+    aim_difficulty: Optional[float] = None
+    approach_rate: Optional[float] = None  # osu catch + standard
+    flashlight_difficulty: Optional[float] = None
+    overall_difficulty: Optional[float] = None
+    slider_factor: Optional[float] = None
+    speed_difficulty: Optional[float] = None
+    speed_note_count: Optional[float] = None
     # osu taiko
-    stamina_difficulty: Optional[float]
-    rhythm_difficulty: Optional[float]
-    colour_difficulty: Optional[float]
+    stamina_difficulty: Optional[float] = None
+    rhythm_difficulty: Optional[float] = None
+    colour_difficulty: Optional[float] = None
     # osu mania
-    great_hit_window: Optional[float]
-    score_multiplier: Optional[float]
+    great_hit_window: Optional[float] = None
+    score_multiplier: Optional[float] = None
 
 
 class Beatmap(BaseModel):
     id: int
     url: str
     mode: Gamemode
     beatmapset_id: int
     difficulty_rating: float
     status: BeatmapRankStatus
     total_length: int
     user_id: int
     version: str
-    accuracy: Optional[float]
-    ar: Optional[float]
-    cs: Optional[float]
-    bpm: Optional[float]
-    convert: Optional[bool]
-    count_circles: Optional[int]
-    count_sliders: Optional[int]
-    count_spinners: Optional[int]
-    deleted_at: Optional[datetime]
-    drain: Optional[float]
-    hit_length: Optional[int]
-    is_scoreable: Optional[bool]
-    last_updated: Optional[datetime]
-    passcount: Optional[int]
-    play_count: Optional[int] = Field(None, alias="playcount")
-    checksum: Optional[str]
-    max_combo: Optional[int]
-    beatmapset: Optional[Beatmapset]
-    failtimes: Optional[BeatmapFailtimes]
+    accuracy: Optional[float] = None
+    ar: Optional[float] = None
+    cs: Optional[float] = None
+    bpm: Optional[float] = None
+    convert: Optional[bool] = None
+    count_circles: Optional[int] = None
+    count_sliders: Optional[int] = None
+    count_spinners: Optional[int] = None
+    deleted_at: Optional[datetime] = None
+    drain: Optional[float] = None
+    hit_length: Optional[int] = None
+    is_scoreable: Optional[bool] = None
+    last_updated: Optional[datetime] = None
+    passcount: Optional[int] = None
+    play_count: Optional[int] = Field(default=None, alias="playcount")
+    checksum: Optional[str] = None
+    max_combo: Optional[int] = None
+    beatmapset: Optional[Beatmapset] = None
+    failtimes: Optional[BeatmapFailtimes] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def _set_url(cls, values: dict[str, Any]) -> dict[str, Any]:
         if values.get("url") is None:
             id = values["id"]
             beatmapset_id = values["beatmapset_id"]
             mode = Gamemode(values["mode"])
             values[
                 "url"
             ] = f"https://osu.ppy.sh/beatmapsets/{beatmapset_id}#{mode}/{id}"
         return values
 
+    @computed_field  # type: ignore
     @property
     def discussion_url(self) -> str:
         return f"https://osu.ppy.sh/beatmapsets/{self.beatmapset_id}/discussion/{self.id}/general"
 
+    @computed_field  # type: ignore
     @property
     def count_objects(self) -> int:
         """Total count of the objects.
 
         :raises ValueError: Raised if object counts are none
         :return: Sum of counts of all objects
         :rtype: int
@@ -270,15 +281,15 @@
             or self.count_sliders is None
         ):
             raise ValueError("Beatmap contains no object count information.")
         return self.count_spinners + self.count_circles + self.count_sliders
 
     @classmethod
     def _from_api_v1(cls, data: Any) -> Beatmap:
-        return cls.parse_obj(
+        return cls.model_validate(
             {
                 "beatmapset_id": data["beatmapset_id"],
                 "difficulty_rating": data["difficultyrating"],
                 "id": data["beatmap_id"],
                 "mode": int(data["mode"]),
                 "status": int(data["approved"]),
                 "total_length": data["total_length"],
@@ -313,44 +324,48 @@
     preview_url: str
     source: str
     status: BeatmapRankStatus
     title: str
     title_unicode: str
     user_id: int
     video: bool
-    nsfw: Optional[bool]
-    hype: Optional[BeatmapHype]
-    availability: Optional[BeatmapAvailability]
-    bpm: Optional[float]
-    can_be_hyped: Optional[bool]
-    discussion_enabled: Optional[bool]
-    discussion_locked: Optional[bool]
-    is_scoreable: Optional[bool]
-    last_updated: Optional[datetime]
-    legacy_thread_url: Optional[str]
-    nominations_summary: Optional[BeatmapNominations]
-    ranked_date: Optional[datetime]
-    storyboard: Optional[bool]
-    submitted_date: Optional[datetime]
-    tags: Optional[str]
-    ratings: Optional[list[int]]
-    has_favourited: Optional[bool]
-    beatmaps: Optional[list[Beatmap]]
+    nsfw: Optional[bool] = None
+    hype: Optional[BeatmapHype] = None
+    availability: Optional[BeatmapAvailability] = None
+    bpm: Optional[float] = None
+    can_be_hyped: Optional[bool] = None
+    discussion_enabled: Optional[bool] = None
+    discussion_locked: Optional[bool] = None
+    is_scoreable: Optional[bool] = None
+    last_updated: Optional[datetime] = None
+    legacy_thread_url: Optional[str] = None
+    nominations: Optional[BeatmapNominations] = None
+    current_nominations: Optional[list[BeatmapNomination]] = None
+    ranked_date: Optional[datetime] = None
+    storyboard: Optional[bool] = None
+    submitted_date: Optional[datetime] = None
+    tags: Optional[str] = None
+    pack_tags: Optional[str] = None
+    ratings: Optional[list[int]] = None
+    has_favourited: Optional[bool] = None
+    beatmaps: Optional[list[Beatmap]] = None
 
+    @computed_field  # type: ignore
     @property
     def url(self) -> str:
         return f"https://osu.ppy.sh/beatmapsets/{self.id}"
 
+    @computed_field  # type: ignore
     @property
     def discussion_url(self) -> str:
         return f"https://osu.ppy.sh/beatmapsets/{self.id}/discussion"
 
     @classmethod
     def _from_api_v1(cls, data: Any) -> Beatmapset:
-        return cls.parse_obj(
+        return cls.model_validate(
             {
                 "id": data["beatmapset_id"],
                 "artist": data["artist"],
                 "artist_unicode": data["artist"],
                 "covers": BeatmapCovers._from_api_v1(data),
                 "favourite_count": data["favourite_count"],
                 "creator": data["creator"],
@@ -376,95 +391,96 @@
 class BeatmapsetSearchResponse(CursorModel):
     beatmapsets: list[Beatmapset]
 
 
 class BeatmapUserPlaycount(BaseModel):
     count: int
     beatmap_id: int
-    beatmap: Optional[Beatmap]
-    beatmapset: Optional[Beatmapset]
+    beatmap: Optional[Beatmap] = None
+    beatmapset: Optional[Beatmapset] = None
 
 
 class BeatmapsetDiscussionPost(BaseModel):
     id: int
     user_id: int
     system: bool
     message: str
     created_at: datetime
-    beatmap_discussion_id: Optional[int]
-    last_editor_id: Optional[int]
-    deleted_by_id: Optional[int]
-    updated_at: Optional[datetime]
-    deleted_at: Optional[datetime]
+    beatmap_discussion_id: Optional[int] = None
+    last_editor_id: Optional[int] = None
+    deleted_by_id: Optional[int] = None
+    updated_at: Optional[datetime] = None
+    deleted_at: Optional[datetime] = None
 
 
 class BeatmapsetDiscussion(BaseModel):
     id: int
     beatmapset_id: int
     user_id: int
     message_type: BeatmapsetDisscussionType
     resolved: bool
     can_be_resolved: bool
     can_grant_kudosu: bool
     created_at: datetime
-    beatmap_id: Optional[int]
-    deleted_by_id: Optional[int]
-    parent_id: Optional[int]
-    timestamp: Optional[int]
-    updated_at: Optional[datetime]
-    deleted_at: Optional[datetime]
-    last_post_at: Optional[datetime]
-    kudosu_denied: Optional[bool]
-    starting_post: Optional[BeatmapsetDiscussionPost]
+    beatmap_id: Optional[int] = None
+    deleted_by_id: Optional[int] = None
+    parent_id: Optional[int] = None
+    timestamp: Optional[int] = None
+    updated_at: Optional[datetime] = None
+    deleted_at: Optional[datetime] = None
+    last_post_at: Optional[datetime] = None
+    kudosu_denied: Optional[bool] = None
+    starting_post: Optional[BeatmapsetDiscussionPost] = None
 
 
 class BeatmapsetVoteEvent(BaseModel):
     score: int
     user_id: int
-    id: Optional[int]
-    created_at: Optional[datetime]
-    updated_at: Optional[datetime]
-    beatmapset_discussion_id: Optional[int]
+    id: Optional[int] = None
+    created_at: Optional[datetime] = None
+    updated_at: Optional[datetime] = None
+    beatmapset_discussion_id: Optional[int] = None
 
 
 class BeatmapsetEventComment(BaseModel):
-    beatmap_discussion_id: Optional[int]
-    beatmap_discussion_post_id: Optional[int]
-    new_vote: Optional[BeatmapsetVoteEvent]
-    votes: Optional[list[BeatmapsetVoteEvent]]
-    mode: Optional[Gamemode]
-    reason: Optional[str]
-    source_user_id: Optional[int]
-    source_user_username: Optional[str]
-    nominator_ids: Optional[list[int]]
-    new: Optional[str]
-    old: Optional[str]
-    new_user_id: Optional[int]
-    new_user_username: Optional[str]
+    beatmap_discussion_id: Optional[int] = None
+    beatmap_discussion_post_id: Optional[int] = None
+    new_vote: Optional[BeatmapsetVoteEvent] = None
+    votes: Optional[list[BeatmapsetVoteEvent]] = None
+    mode: Optional[Gamemode] = None
+    reason: Optional[str] = None
+    source_user_id: Optional[int] = None
+    source_user_username: Optional[str] = None
+    nominator_ids: Optional[list[int]] = None
+    new: Optional[str] = None
+    old: Optional[str] = None
+    new_user_id: Optional[int] = None
+    new_user_username: Optional[str] = None
 
 
 class BeatmapsetEvent(BaseModel):
     id: int
     type: BeatmapsetEventType
     r"""Information on types: https://github.com/ppy/osu-web/blob/master/resources/assets/lib/interfaces/beatmapset-event-json.ts"""
     created_at: datetime
     user_id: int
-    beatmapset: Optional[Beatmapset]
-    discussion: Optional[BeatmapsetDiscussion]
-    comment: Optional[dict]
+    beatmapset: Optional[Beatmapset] = None
+    discussion: Optional[BeatmapsetDiscussion] = None
+    comment: Optional[dict] = None
 
 
 class BeatmapsetDiscussionResponse(CursorModel):
     beatmaps: list[Beatmap]
     discussions: list[BeatmapsetDiscussion]
     included_discussions: list[BeatmapsetDiscussion]
     users: list[User]
     max_blocks: int
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def _set_max_blocks(cls, values: dict[str, Any]) -> dict[str, Any]:
         values["max_blocks"] = values["reviews_config"]["max_blocks"]
         return values
 
 
 class BeatmapsetDiscussionPostResponse(CursorModel):
     beatmapsets: list[Beatmapset]
@@ -474,8 +490,8 @@
 
 class BeatmapsetDiscussionVoteResponse(CursorModel):
     votes: list[BeatmapsetVoteEvent]
     discussions: list[BeatmapsetDiscussion]
     users: list[User]
 
 
-Beatmap.update_forward_refs()
+Beatmap.model_rebuild()
```

### Comparing `aiosu-1.5.0/aiosu/models/chat.py` & `aiosu-2.0.0/aiosu/models/chat.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,39 +47,40 @@
 
 
 class ChatChannel(BaseModel):
     id: int = Field(alias="channel_id")
     type: ChatChannelTypes
     name: str
     moderated: bool
-    icon: Optional[str]
-    description: Optional[str]
-    last_message_id: Optional[int]
-    user_ids: Optional[list[int]] = Field(alias="users")
-    current_user_attributes: Optional[CurrentUserAttributes]
+    message_length_limit: int
+    icon: Optional[str] = None
+    description: Optional[str] = None
+    last_message_id: Optional[int] = None
+    user_ids: Optional[list[int]] = Field(default=None, alias="users")
+    current_user_attributes: Optional[CurrentUserAttributes] = None
 
 
 class ChatMessage(BaseModel):
     message_id: int
     sender_id: int
     channel_id: int
     timestamp: str
     content: str
     is_action: bool
-    uuid: Optional[str]
-    sender: Optional[User]
+    uuid: Optional[str] = None
+    sender: Optional[User] = None
 
 
 class ChatMessageCreateResponse(BaseModel):
     channel: ChatChannel
     message: ChatMessage
 
 
 class ChatUpdateResponse(BaseModel):
-    messages: Optional[list[ChatMessage]]
-    presence: Optional[list[ChatChannel]]
+    messages: Optional[list[ChatMessage]] = None
+    presence: Optional[list[ChatChannel]] = None
     silences: list
 
 
 class ChatChannelResponse(BaseModel):
     channel: ChatChannel
-    users: Optional[list[User]]
+    users: Optional[list[User]] = None
```

### Comparing `aiosu-1.5.0/aiosu/models/comment.py` & `aiosu-2.0.0/aiosu/models/comment.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,48 +19,48 @@
     "CommentSortType",
 )
 
 CommentSortType = Literal["new", "old", "top"]
 
 
 class Commentable(BaseModel):
-    id: Optional[int]
-    title: Optional[str]
-    url: Optional[str]
-    type: Optional[str]
-    owner_id: Optional[int]
-    owner_title: Optional[str]
-    current_user_attributes: Optional[CurrentUserAttributes]
+    id: Optional[int] = None
+    title: Optional[str] = None
+    url: Optional[str] = None
+    type: Optional[str] = None
+    owner_id: Optional[int] = None
+    owner_title: Optional[str] = None
+    current_user_attributes: Optional[CurrentUserAttributes] = None
 
 
 class Comment(BaseModel):
     id: int
     commentable_id: int
     commentable_type: str
     created_at: datetime
     updated_at: datetime
     pinned: bool
     votes_count: int
     replies_count: int
-    message: Optional[str]
-    message_html: Optional[str]
-    deleted_at: Optional[datetime]
-    edited_at: Optional[datetime]
-    edited_by_id: Optional[int]
-    parent_id: Optional[int]
-    legacy_name: Optional[str]
-    user_id: Optional[int]
+    message: Optional[str] = None
+    message_html: Optional[str] = None
+    deleted_at: Optional[datetime] = None
+    edited_at: Optional[datetime] = None
+    edited_by_id: Optional[int] = None
+    parent_id: Optional[int] = None
+    legacy_name: Optional[str] = None
+    user_id: Optional[int] = None
 
 
 class CommentBundle(CursorModel):
     commentable_meta: list[Commentable]
     comments: list[Comment]
     has_more: bool
     included_comments: list[Comment]
     sort: str
     user_follow: bool
     user_votes: list[int]
     users: list[User]
-    pinned_comments: Optional[list[Comment]]
-    total: Optional[int]
-    top_level_count: Optional[int]
-    has_more_id: Optional[int]
+    pinned_comments: Optional[list[Comment]] = None
+    total: Optional[int] = None
+    top_level_count: Optional[int] = None
+    has_more_id: Optional[int] = None
```

### Comparing `aiosu-1.5.0/aiosu/models/event.py` & `aiosu-2.0.0/aiosu/models/event.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,25 +52,25 @@
     title: str
     url: str
 
 
 class EventUser(BaseModel):
     username: str
     url: str
-    previous_username: Optional[str] = Field(alias="previousUsername")
+    previous_username: Optional[str] = Field(default=None, alias="previousUsername")
 
 
 class Event(BaseModel):
     created_at: datetime
     id: int
     type: EventType
     r"""Information on types: https://github.com/ppy/osu-web/blob/master/resources/assets/lib/interfaces/event-json.ts"""
-    parse_error: Optional[bool]
-    achievment: Optional[Achievement]
-    user: Optional[EventUser]
-    beatmap: Optional[EventBeatmap]
-    beatmapset: Optional[EventBeatmapset]
-    approval: Optional[BeatmapRankStatus]
-    count: Optional[int]
-    rank: Optional[int]
-    mode: Optional[Gamemode]
-    score_rank: Optional[str] = Field(alias="scoreRank")
+    parse_error: Optional[bool] = None
+    achievment: Optional[Achievement] = None
+    user: Optional[EventUser] = None
+    beatmap: Optional[EventBeatmap] = None
+    beatmapset: Optional[EventBeatmapset] = None
+    approval: Optional[BeatmapRankStatus] = None
+    count: Optional[int] = None
+    rank: Optional[int] = None
+    mode: Optional[Gamemode] = None
+    score_rank: Optional[str] = Field(default=None, alias="scoreRank")
```

### Comparing `aiosu-1.5.0/aiosu/models/forum.py` & `aiosu-2.0.0/aiosu/models/forum.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,55 +27,55 @@
     "announcement",
 ]
 
 
 class ForumPollOption(BaseModel):
     id: int
     text: HTMLBody
-    vote_count: Optional[int]
+    vote_count: Optional[int] = None
 
 
 class ForumPoll(BaseModel):
     allow_vote_change: bool
     hide_incomplete_results: bool
     max_votes: int
     total_vote_count: int
     options: list[ForumPollOption]
     started_at: datetime
     title: HTMLBody
-    ended_at: Optional[datetime]
-    last_vote_at: Optional[datetime]
+    ended_at: Optional[datetime] = None
+    last_vote_at: Optional[datetime] = None
 
 
 class ForumTopic(BaseModel):
     id: int
     title: str
     created_at: datetime
     first_post_id: int
     last_post_id: int
     forum_id: int
     is_locked: bool
     post_count: int
     type: ForumTopicType
     updated_at: datetime
     user_id: int
-    deleted_at: Optional[datetime]
-    poll: Optional[ForumPoll]
+    deleted_at: Optional[datetime] = None
+    poll: Optional[ForumPoll] = None
 
 
 class ForumPost(BaseModel):
     id: int
     created_at: datetime
     forum_id: int
     topic_id: int
     user_id: int
-    edited_by_id: Optional[int]
-    edited_at: Optional[datetime]
-    deleted_at: Optional[datetime]
-    body: Optional[HTMLBody]
+    edited_by_id: Optional[int] = None
+    edited_at: Optional[datetime] = None
+    deleted_at: Optional[datetime] = None
+    body: Optional[HTMLBody] = None
 
 
 class ForumTopicResponse(CursorModel):
     topic: ForumTopic
     posts: list[ForumPost]
```

### Comparing `aiosu-1.5.0/aiosu/models/gamemode.py` & `aiosu-2.0.0/aiosu/models/gamemode.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/models/kudosu.py` & `aiosu-2.0.0/aiosu/models/kudosu.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 class KudosuGiver(BaseModel):
     url: str
     username: str
 
 
 class KudosuPost(BaseModel):
     title: str
-    url: Optional[str]
+    url: Optional[str] = None
 
 
 class KudosuHistory(BaseModel):
     id: int
     action: KudosuAction
     created_at: datetime
     amount: int
     model: str
-    giver: Optional[KudosuGiver]
-    post: Optional[KudosuPost]
+    giver: Optional[KudosuGiver] = None
+    post: Optional[KudosuPost] = None
```

### Comparing `aiosu-1.5.0/aiosu/models/lazer.py` & `aiosu-2.0.0/aiosu/models/lazer.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 """
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
 from typing import Optional
 
+from pydantic import computed_field
 from pydantic import Field
-from pydantic import root_validator
+from pydantic import model_validator
 
 from .base import BaseModel
 from .beatmap import Beatmap
 from .beatmap import Beatmapset
 from .common import CurrentUserAttributes
 from .gamemode import Gamemode
 from .score import ScoreWeight
@@ -76,34 +77,40 @@
     small_bonus: int = 0
     small_tick_hit: int = 0
     small_tick_miss: int = 0
     good: int = 0
     perfect: int = 0
     legacy_combo_increase: int = 0
 
+    @computed_field  # type: ignore
     @property
     def count_300(self) -> int:
         return self.great
 
+    @computed_field  # type: ignore
     @property
     def count_100(self) -> int:
         return self.ok
 
+    @computed_field  # type: ignore
     @property
     def count_50(self) -> int:
         return self.meh
 
+    @computed_field  # type: ignore
     @property
     def count_miss(self) -> int:
         return self.miss
 
+    @computed_field  # type: ignore
     @property
     def count_geki(self) -> int:
         return self.perfect
 
+    @computed_field  # type: ignore
     @property
     def count_katu(self) -> int:
         return self.good
 
 
 class LazerReplayData(BaseModel):
     mods: list[LazerMod]
@@ -127,29 +134,32 @@
     user_id: int
     replay: bool
     type: str
     current_user_attributes: CurrentUserAttributes
     beatmap: Beatmap
     beatmapset: Beatmapset
     user: User
-    build_id: Optional[int]
-    started_at: Optional[datetime]
-    best_id: Optional[int]
-    legacy_perfect: Optional[bool]
-    pp: Optional[float]
-    weight: Optional[ScoreWeight]
+    build_id: Optional[int] = None
+    started_at: Optional[datetime] = None
+    best_id: Optional[int] = None
+    legacy_perfect: Optional[bool] = None
+    pp: Optional[float] = None
+    weight: Optional[ScoreWeight] = None
 
+    @computed_field  # type: ignore
     @property
     def mods_str(self) -> str:
         return "".join(str(mod) for mod in self.mods)
 
+    @computed_field  # type: ignore
     @property
     def created_at(self) -> datetime:
         return self.ended_at
 
+    @computed_field  # type: ignore
     @property
     def completion(self) -> float:
         """Beatmap completion.
 
         :raises ValueError: If beatmap is None
         :raises ValueError: If mode is unknown
         :return: Beatmap completion of a score (%). 100% for passes
@@ -159,22 +169,25 @@
             raise ValueError("Beatmap object is not set.")
 
         if self.passed:
             return 100.0
 
         return calculate_score_completion(self.statistics, self.beatmap)
 
+    @computed_field  # type: ignore
     @property
     def mode(self) -> Gamemode:
         return Gamemode(self.ruleset_id)
 
+    @computed_field  # type: ignore
     @property
     def score(self) -> int:
         return self.total_score
 
+    @computed_field  # type: ignore
     @property
     def score_url(self) -> Optional[str]:
         r"""Link to the score.
 
         :return: Link to the score on the osu! website
         :rtype: Optional[str]
         """
@@ -182,14 +195,15 @@
             return None
         return (
             f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
             if self.best_id
             else f"https://osu.ppy.sh/scores/{self.id}"
         )
 
+    @computed_field  # type: ignore
     @property
     def replay_url(self) -> Optional[str]:
         r"""Link to the replay.
 
         :return: Link to download the replay on the osu! website
         :rtype: Optional[str]
         """
@@ -197,12 +211,13 @@
             return None
         return (
             f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
             if self.best_id
             else f"https://osu.ppy.sh/scores/{self.id}/download"
         )
 
-    @root_validator
+    @model_validator(mode="before")
+    @classmethod
     def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
         if not values["passed"]:
             values["rank"] = "F"
         return values
```

### Comparing `aiosu-1.5.0/aiosu/models/mods.py` & `aiosu-2.0.0/aiosu/models/mods.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 """
 from __future__ import annotations
 
 from collections import UserList
 from enum import IntEnum
 from enum import unique
 from functools import reduce
+from typing import Type
 from typing import TYPE_CHECKING
 
+from pydantic import GetCoreSchemaHandler
+from pydantic_core import core_schema
+from pydantic_core import CoreSchema
 
-if TYPE_CHECKING:
-    from collections.abc import Generator
 
+if TYPE_CHECKING:
     from typing import Any
     from typing import Union
 
 __all__ = (
     "Mod",
     "Mods",
     "KeyMod",
@@ -150,14 +153,18 @@
         if isinstance(mods, int):  # Bitwise representation of mods
             self.data = [mod for mod in list(Mod) if mod & mods]
             return
         if isinstance(mods, str):  # string of mods
             mods = [mods[i : i + 2] for i in range(0, len(mods), 2)]
         if isinstance(mods, list) or isinstance(mods, Mods):  # List of Mod types
             self.data = [Mod(mod) for mod in mods]  # type: ignore
+            return
+        raise TypeError(
+            f"Mods must be a list of Mod types, a string, or an int. Not {type(mods)}",
+        )
 
     @property
     def bitwise(self) -> int:
         r"""Bitwise representation.
 
         :return: Bitwise representation of the mod combination
         :rtype: int
@@ -196,22 +203,27 @@
         if isinstance(__o, Mod):
             return int(self) | int(__o)
         if isinstance(__o, Mods):
             return int(self) | int(__o)
         raise ValueError(f"Object {__o!r} is of invalid type.")
 
     @classmethod
-    def __get_validators__(cls) -> Generator:
-        yield cls._validate
-
-    @classmethod
-    def _validate(cls, v: object) -> Mods:
-        if not isinstance(v, (list, str, int)):
-            raise TypeError("Invalid type specified ")
-        return cls(v)
+    def __get_pydantic_core_schema__(
+        cls,
+        source_type: Type[Any],
+        handler: GetCoreSchemaHandler,
+    ) -> CoreSchema:
+        return core_schema.no_info_before_validator_function(
+            cls,
+            core_schema.json_or_python_schema(
+                json_schema=core_schema.list_schema(),
+                python_schema=handler(source_type),
+            ),
+            serialization=core_schema.to_string_ser_schema(when_used="json"),
+        )
 
 
 KeyMod = (
     Mod.Key1
     | Mod.Key2
     | Mod.Key3
     | Mod.Key4
```

### Comparing `aiosu-1.5.0/aiosu/models/multiplayer.py` & `aiosu-2.0.0/aiosu/models/multiplayer.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datetime import datetime
 from typing import Any
 from typing import Literal
 from typing import Optional
 
 from pydantic import Field
-from pydantic import root_validator
+from pydantic import model_validator
 
 from .base import BaseModel
 from .beatmap import Beatmap
 from .common import CursorModel
 from .gamemode import Gamemode
 from .lazer import LazerMod
 from .lazer import LazerScoreStatistics
@@ -75,51 +75,52 @@
     total_score: int
     accuracy: float
     max_combo: int
     mods: list[LazerMod]
     passed: bool
     user: User
     statistics: LazerScoreStatistics
-    position: Optional[int]
-    scores_around: Optional[MultiplayerScoresAround]
+    position: Optional[int] = None
+    scores_around: Optional[MultiplayerScoresAround] = None
 
 
 class MultiplayerScoresResponse(CursorModel):
     scores: list[MultiplayerScore]
-    user_score: Optional[MultiplayerScore]
-    total: Optional[int]
+    user_score: Optional[MultiplayerScore] = None
+    total: Optional[int] = None
 
 
 class MultiplayerMatch(BaseModel):
     id: int
     name: str
     start_time: datetime
-    end_time: Optional[datetime]
+    end_time: Optional[datetime] = None
 
 
 class MultiplayerEvent(BaseModel):
     id: int
     timestamp: datetime
     type: MultiplayerEventTypes
-    user_id: Optional[int]
+    user_id: Optional[int] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def _set_type(cls, values: dict[str, Any]) -> dict[str, Any]:
         if "detail" in values:
             values["type"] = values["detail"]["type"]
         return values
 
 
 class MultiplayerMatchResponse(BaseModel):
     match: MultiplayerMatch
     events: list[MultiplayerEvent]
     users: list[User]
     first_event_id: int
     latest_event_id: int
-    current_game_id: Optional[int]
+    current_game_id: Optional[int] = None
 
 
 class MultiplayerMatchesResponse(CursorModel):
     matches: list[MultiplayerMatch]
 
 
 class MultiplayerPlaylistItem(BaseModel):
@@ -128,16 +129,16 @@
     beatmap_id: int
     mode: Gamemode = Field(alias="ruleset_id")
     allowed_mods: list[LazerMod]
     required_mods: list[LazerMod]
     expired: bool
     owner_id: int
     beatmap: Beatmap
-    playlist_order: Optional[int]
-    played_at: Optional[datetime]
+    playlist_order: Optional[int] = None
+    played_at: Optional[datetime] = None
 
 
 class MultiplayerRoom(BaseModel):
     id: int
     name: str
     category: MultiplayerRoomCategories
     type: MultiplayerRoomTypeGroups
@@ -146,37 +147,37 @@
     active: bool
     has_password: bool
     auto_skip: bool
     host: User
     queue_mode: MultiplayerQueueMode
     playlist: list[MultiplayerPlaylistItem]
     recent_participants: list[User]
-    participant_count: Optional[int]
-    starts_at: Optional[datetime]
-    ends_at: Optional[datetime]
-    max_attempts: Optional[int]
+    participant_count: Optional[int] = None
+    starts_at: Optional[datetime] = None
+    ends_at: Optional[datetime] = None
+    max_attempts: Optional[int] = None
 
 
 class MultiplayerLeaderboardItem(BaseModel):
     accuracy: float
     attempts: int
     completed: int
     pp: float
     room_id: int
     total_score: int
     user_id: int
     user: User
-    position: Optional[int]
+    position: Optional[int] = None
 
 
 class MultiplayerLeaderboardResponse(BaseModel):
     leaderboard: list[MultiplayerLeaderboardItem]
-    user_score: Optional[MultiplayerLeaderboardItem]
+    user_score: Optional[MultiplayerLeaderboardItem] = None
 
 
 class MultiplayerRoomsResponse(CursorModel):
     """Currently unused. Relevant for api-version >= 99999999"""
 
     rooms: list[MultiplayerRoom]
 
 
-MultiplayerScoresAround.update_forward_refs()
+MultiplayerScoresAround.model_rebuild()
```

### Comparing `aiosu-1.5.0/aiosu/models/news.py` & `aiosu-2.0.0/aiosu/models/news.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 
 class NewsSearch(BaseModel):
     limit: int
     sort: Literal["published_desc"]
 
 
 class Navigation(BaseModel):
-    newer: Optional[NewsPost]
-    older: Optional[NewsPost]
+    newer: Optional[NewsPost] = None
+    older: Optional[NewsPost] = None
 
 
 class NewsPost(BaseModel):
     id: int
     title: str
     slug: str
     author: str
     edit_url: str
     published_at: datetime
     updated_at: datetime
-    first_image: Optional[str]
-    content: Optional[str]
-    preview: Optional[str]
-    navigation: Optional[Navigation]
+    first_image: Optional[str] = None
+    content: Optional[str] = None
+    preview: Optional[str] = None
+    navigation: Optional[Navigation] = None
 
 
 class NewsSidebar(BaseModel):
     current_year: int
     years: list[int]
     news_posts: list[NewsPost]
 
 
 class NewsListing(CursorModel):
     news_posts: list[NewsPost]
     search: NewsSearch
     news_sidebar: NewsSidebar
 
 
-Navigation.update_forward_refs()
+Navigation.model_rebuild()
```

### Comparing `aiosu-1.5.0/aiosu/models/oauthtoken.py` & `aiosu-2.0.0/aiosu/models/oauthtoken.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,54 +5,59 @@
 
 from datetime import datetime
 from datetime import timedelta
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 import jwt
-from pydantic import root_validator
+from pydantic import computed_field
+from pydantic import model_validator
 
 from .base import FrozenModel
 from .scopes import Scopes
 
 if TYPE_CHECKING:
     from typing import Any
 
 __all__ = ("OAuthToken",)
 
 
-class OAuthToken(FrozenModel, keep_untouched=(cached_property,)):
+class OAuthToken(FrozenModel):
     token_type: str = "Bearer"
     """Defaults to 'Bearer'"""
     access_token: str = ""
     refresh_token: str = ""
     expires_on: datetime = datetime.utcfromtimestamp(0)
     """Can be a datetime.datetime object or a string. Alternatively, expires_in may be passed representing the number of seconds the token will be valid for."""
 
+    @computed_field  # type: ignore
     @cached_property
     def owner_id(self) -> int:
         if not self.access_token:
             return 0
         decoded = jwt.decode(self.access_token, options={"verify_signature": False})
         if decoded["sub"]:
             return int(decoded["sub"])
         return 0
 
+    @computed_field  # type: ignore
     @cached_property
     def scopes(self) -> Scopes:
         if not self.access_token:
             return Scopes.PUBLIC
         decoded = jwt.decode(self.access_token, options={"verify_signature": False})
         return Scopes.from_api_list(decoded["scopes"])
 
+    @computed_field  # type: ignore
     @cached_property
     def can_refresh(self) -> bool:
         """Returns True if the token can be refreshed."""
         return bool(self.refresh_token)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def _set_expires_on(cls, values: dict[str, Any]) -> dict[str, Any]:
         if isinstance(values.get("expires_in"), int):
             values["expires_on"] = datetime.utcnow() + timedelta(
                 seconds=values["expires_in"],
             )
         return values
```

### Comparing `aiosu-1.5.0/aiosu/models/performance.py` & `aiosu-2.0.0/aiosu/models/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/models/rankings.py` & `aiosu-2.0.0/aiosu/models/rankings.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 RankingFilter = Literal["all", "friends"]
 RankingType = Literal["performance", "score", "country", "charts"]
 RankingVariant = Literal["4k", "7k"]
 
 
 class Rankings(CursorModel):
     ranking: list[UserStats]
-    total: Optional[int]
-    spotlight: Optional[Spotlight]
-    beatmapsets: Optional[list[Beatmapset]]
+    total: Optional[int] = None
+    spotlight: Optional[Spotlight] = None
+    beatmapsets: Optional[list[Beatmapset]] = None
```

### Comparing `aiosu-1.5.0/aiosu/models/replay.py` & `aiosu-2.0.0/aiosu/models/replay.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 This module contains models for replays.
 """
 from __future__ import annotations
 
 from datetime import datetime
 from enum import IntFlag
 from enum import unique
-from typing import Any
 from typing import Optional
 
-from pydantic import root_validator
+from pydantic import model_validator
 
 from .base import BaseModel
 from .gamemode import Gamemode
 from .lazer import LazerReplayData
 from .mods import Mod
 from .mods import Mods
 from .score import ScoreStatistics
@@ -95,32 +94,34 @@
     score: int
     max_combo: int
     perfect_combo: bool
     mods: Mods
     statistics: ScoreStatistics
     replay_data: list[ReplayEvent]
     lifebar_data: list[ReplayLifebarEvent]
-    mod_extras: Optional[float]
-    skip_offset: Optional[int]
-    rng_seed: Optional[int]
-    lazer_replay_data: Optional[LazerReplayData]
+    mod_extras: Optional[float] = None
+    skip_offset: Optional[int] = None
+    rng_seed: Optional[int] = None
+    lazer_replay_data: Optional[LazerReplayData] = None
 
     def __repr__(self) -> str:
         return f"<Replay {self.player_name} {self.map_md5}>"
 
     def __str__(self) -> str:
         return f"{self.player_name} {self.played_at} {self.map_md5} +{self.mods}"
 
-    @root_validator
-    def _add_skip_offset(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if not values["skip_offset"]:
-            values["skip_offset"] = _parse_skip_offset(
-                values["replay_data"],
-                values["mods"],
+    @model_validator(mode="after")  # type: ignore
+    @classmethod
+    def _add_skip_offset(cls, obj: Replay) -> Replay:
+        if not obj.skip_offset:
+            obj.skip_offset = _parse_skip_offset(
+                obj.replay_data,
+                obj.mods,
             )
-        return values
+        return obj
 
-    @root_validator
-    def _add_rng_seed(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if not values["rng_seed"] and values["version"] >= 2013_03_19:
-            values["rng_seed"] = _parse_rng_seed(values["replay_data"])
-        return values
+    @model_validator(mode="after")  # type: ignore
+    @classmethod
+    def _add_rng_seed(cls, obj: Replay) -> Replay:
+        if not obj.rng_seed and obj.version >= 2013_03_19:
+            obj.rng_seed = _parse_rng_seed(obj.replay_data)
+        return obj
```

### Comparing `aiosu-1.5.0/aiosu/models/scopes.py` & `aiosu-2.0.0/aiosu/models/scopes.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/models/score.py` & `aiosu-2.0.0/aiosu/models/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from pydantic import root_validator
+from pydantic import computed_field
+from pydantic import model_validator
 
 from ..utils.accuracy import CatchAccuracyCalculator
 from ..utils.accuracy import ManiaAccuracyCalculator
 from ..utils.accuracy import OsuAccuracyCalculator
 from ..utils.accuracy import TaikoAccuracyCalculator
 from .base import BaseModel
 from .beatmap import Beatmap
@@ -101,25 +102,26 @@
     count_50: int
     count_100: int
     count_300: int
     count_miss: int
     count_geki: int
     count_katu: int
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def _convert_none_to_zero(cls, values: dict[str, Any]) -> dict[str, Any]:
         # Lazer API returns null for some statistics
         for key in values:
             if values[key] is None:
                 values[key] = 0
         return values
 
     @classmethod
     def _from_api_v1(cls, data: Any) -> ScoreStatistics:
-        return cls.parse_obj(
+        return cls.model_validate(
             {
                 "count_50": data["count50"],
                 "count_100": data["count100"],
                 "count_300": data["count300"],
                 "count_geki": data["countgeki"],
                 "count_katu": data["countkatu"],
                 "count_miss": data["countmiss"],
@@ -136,29 +138,30 @@
     passed: bool
     perfect: bool
     statistics: ScoreStatistics
     rank: str
     created_at: datetime
     mode: Gamemode
     replay: bool
-    id: Optional[int]
+    id: Optional[int] = None
     """Always present except for API v1 recent scores."""
     pp: Optional[float] = 0
-    best_id: Optional[int]
-    beatmap: Optional[Beatmap]
-    beatmapset: Optional[Beatmapset]
-    weight: Optional[ScoreWeight]
-    user: Optional[User]
-    rank_global: Optional[int]
-    rank_country: Optional[int]
-    type: Optional[str]
-    current_user_attributes: Optional[CurrentUserAttributes]
-    beatmap_id: Optional[int]
+    best_id: Optional[int] = None
+    beatmap: Optional[Beatmap] = None
+    beatmapset: Optional[Beatmapset] = None
+    weight: Optional[ScoreWeight] = None
+    user: Optional[User] = None
+    rank_global: Optional[int] = None
+    rank_country: Optional[int] = None
+    type: Optional[str] = None
+    current_user_attributes: Optional[CurrentUserAttributes] = None
+    beatmap_id: Optional[int] = None
     """Only present on API v1"""
 
+    @computed_field  # type: ignore
     @property
     def completion(self) -> float:
         """Beatmap completion.
 
         :raises ValueError: If beatmap is None
         :raises ValueError: If mode is unknown
         :return: Beatmap completion of a score (%). 100% for passes
@@ -168,14 +171,15 @@
             raise ValueError("Beatmap object is not set.")
 
         if self.passed:
             return 100.0
 
         return calculate_score_completion(self.mode, self.statistics, self.beatmap)
 
+    @computed_field  # type: ignore
     @property
     def score_url(self) -> Optional[str]:
         r"""Link to the score.
 
         :return: Link to the score on the osu! website
         :rtype: Optional[str]
         """
@@ -183,14 +187,15 @@
             return None
         return (
             f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
             if self.best_id
             else f"https://osu.ppy.sh/scores/{self.id}"
         )
 
+    @computed_field  # type: ignore
     @property
     def replay_url(self) -> Optional[str]:
         r"""Link to the replay.
 
         :return: Link to download the replay on the osu! website
         :rtype: Optional[str]
         """
@@ -198,15 +203,16 @@
             return None
         return (
             f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
             if self.best_id
             else f"https://osu.ppy.sh/scores/{self.id}/download"
         )
 
-    @root_validator
+    @model_validator(mode="before")
+    @classmethod
     def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
         if not values["passed"]:
             values["rank"] = "F"
         return values
 
     async def request_beatmap(self, client: v1.Client) -> None:
         r"""For v1 Scores: requests the beatmap from the API and sets it.
@@ -227,15 +233,15 @@
     @classmethod
     def _from_api_v1(
         cls,
         data: Any,
         mode: Gamemode,
     ) -> Score:
         statistics = ScoreStatistics._from_api_v1(data)
-        score = cls.parse_obj(
+        score = cls.model_validate(
             {
                 "id": data["score_id"],
                 "user_id": data["user_id"],
                 "accuracy": 0.0,
                 "mods": int(data["enabled_mods"]),
                 "score": data["score"],
                 "pp": data.get("pp", 0.0),
```

### Comparing `aiosu-1.5.0/aiosu/utils/accuracy.py` & `aiosu-2.0.0/aiosu/utils/accuracy.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/utils/auth.py` & `aiosu-2.0.0/aiosu/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     async with aiohttp.ClientSession(headers=headers) as temp_session:
         async with temp_session.post(url, data=data) as resp:
             try:
                 body = await resp.read()
                 json = orjson.loads(body)
                 if resp.status != 200:
                     raise APIException(resp.status, json.get("error", ""))
-                token = OAuthToken.parse_obj(json)
+                token = OAuthToken.model_validate(json)
                 return token
             except aiohttp.client_exceptions.ContentTypeError:
                 raise APIException(403, "Invalid code specified.")
 
 
 def generate_url(
     client_id: int,
```

### Comparing `aiosu-1.5.0/aiosu/utils/binary.py` & `aiosu-2.0.0/aiosu/utils/binary.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/utils/performance.py` & `aiosu-2.0.0/aiosu/utils/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/utils/replay.py` & `aiosu-2.0.0/aiosu/utils/replay.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,17 @@
         replay["online_id"] = unpack_long(file)
     elif replay["version"] >= 20121008:
         replay["online_id"] = unpack_int(file)
     if Mod.Target & replay["mods"]:
         replay["mod_extras"] = unpack_float64(file)
     if replay["version"] >= 30000001:
         lazer_replay_data_str = unpack_replay_data(file)
-        replay["lazer_replay_data"] = LazerReplayData.parse_raw(lazer_replay_data_str)
+        replay["lazer_replay_data"] = LazerReplayData.model_validate_json(
+            lazer_replay_data_str,
+        )
     return Replay(**replay)
 
 
 def parse_path(path: str) -> Replay:
     """Parse a replay file and return a dictionary with the replay data.
 
     :param path: The path to the replay file.
@@ -165,15 +167,18 @@
     elif replay.version >= 2012_10_08:
         pack_int(file, replay.online_id)
     if replay.mod_extras is not None:
         pack_float64(file, replay.mod_extras)
     if replay.lazer_replay_data is not None:
         pack_replay_data(
             file,
-            replay.lazer_replay_data.json(exclude_unset=True, exclude_none=True),
+            replay.lazer_replay_data.model_dump_json(
+                exclude_unset=True,
+                exclude_none=True,
+            ),
         )
 
 
 def write_path(path: str, replay: Replay) -> None:
     """Write a replay to a file.
 
     :param path: The path to the file to write to.
```

### Comparing `aiosu-1.5.0/aiosu/v1/client.py` & `aiosu-2.0.0/aiosu/v1/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,18 @@
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         await self.close()
 
     async def _request(
-        self, request_type: ClientRequestType, *args: Any, **kwargs: Any
+        self,
+        request_type: ClientRequestType,
+        *args: Any,
+        **kwargs: Any,
     ) -> Any:
         if self._session is None:
             self._session = aiohttp.ClientSession()
 
         req: dict[str, Callable] = {
             "GET": self._session.get,
             "POST": self._session.post,
@@ -163,15 +166,18 @@
         )
         json = await self._request("GET", url, params=params)
         if not json:
             raise APIException(404, "User not found")
         return User._from_api_v1(json[0])
 
     async def __get_type_scores(
-        self, user_query: Union[str, int], request_type: str, **kwargs: Any
+        self,
+        user_query: Union[str, int],
+        request_type: str,
+        **kwargs: Any,
     ) -> list[Score]:
         r"""INTERNAL: Get a user's scores by type
 
         :param user_query: Username or ID to search by
         :type user_query: Union[str, int]
         :param request_type: "recent" or "best"
         :type request_type: str
@@ -211,15 +217,17 @@
             converter=lambda x: UserQueryType(x).old_api_name,
         )
         json = await self._request("GET", url, params=params)
         score_conv = lambda x: Score._from_api_v1(x, mode)
         return from_list(score_conv, json)
 
     async def get_user_recents(
-        self, user_query: Union[str, int], **kwargs: Any
+        self,
+        user_query: Union[str, int],
+        **kwargs: Any,
     ) -> list[Score]:
         r"""Get a user's recent scores.
 
         :param user_query: Username or ID to search by
         :type user_query: Union[str, int]
         :param \**kwargs:
             See below
@@ -238,15 +246,17 @@
         :rtype: list[aiosu.models.score.Score]
         """
         if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
             raise ValueError("Invalid limit specified. Limit must be between 1 and 50")
         return await self.__get_type_scores(user_query, "recent", limit=limit, **kwargs)
 
     async def get_user_bests(
-        self, user_query: Union[str, int], **kwargs: Any
+        self,
+        user_query: Union[str, int],
+        **kwargs: Any,
     ) -> list[Score]:
         r"""Get a user's best scores.
 
         :param user_query: Username or ID to search by
         :type user_query: Union[str, int]
         :param \**kwargs:
             See below
@@ -391,15 +401,15 @@
         """
         url = f"{self.base_url}/api/get_match"
         params = {
             "k": self.token,
             "mp": match_id,
         }
         json = await self._request("GET", url, params=params)
-        return Match.parse_obj(json)
+        return Match.model_validate(json)
 
     async def get_replay(self, **kwargs: Any) -> ReplayCompact:
         r"""Gets data for a replay.
 
         :param \**kwargs:
             See below
 
@@ -444,15 +454,15 @@
             )
         if not added:
             raise ValueError(
                 "Either score_id or beatmap_id + user_id must be specified.",
             )
         add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
         json = await self._request("GET", url, params=params)
-        return ReplayCompact.parse_obj(json)
+        return ReplayCompact.model_validate(json)
 
     async def get_beatmap_osu(self, beatmap_id: int) -> StringIO:
         r"""Returns the Buffer of the beatmap file requested.
 
         :param beatmap_id: The ID of the beatmap
         :type beatmap_id: int
```

### Comparing `aiosu-1.5.0/aiosu/v2/client.py` & `aiosu-2.0.0/aiosu/v2/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     A decorator that checks the current token, to be used as:
     @check_token
     """
 
     @functools.wraps(func)
     async def _check_token(self: Client, *args: Any, **kwargs: Any) -> Any:
         token = await self.get_current_token()
-        if datetime.utcnow() > token.expires_on:
+        if datetime.utcnow().timestamp() > token.expires_on.timestamp():
             await self._refresh()
         return await func(self, *args, **kwargs)
 
     return cast(F, _check_token)
 
 
 def requires_scope(
@@ -307,15 +307,18 @@
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "grant_type": "client_credentials",
             "scope": "public",
         }
 
     async def _request(
-        self, request_type: ClientRequestType, *args: Any, **kwargs: Any
+        self,
+        request_type: ClientRequestType,
+        *args: Any,
+        **kwargs: Any,
     ) -> Any:
         await self._prepare_token()
 
         if self._session is None:
             self._session = aiohttp.ClientSession(headers=await self._get_headers())
 
         req: dict[str, Callable] = {
@@ -374,15 +377,15 @@
                                 f"Unhandled Content Type '{content_type}'",
                             )
                         json = orjson.loads(body)
                         if resp.status != 200:
                             raise APIException(resp.status, json.get("error", ""))
                         if self._session:
                             await self._session.close()
-                        new_token = OAuthToken.parse_obj(json)
+                        new_token = OAuthToken.model_validate(json)
                         await self._update_token(new_token)
                         self._session = aiohttp.ClientSession(
                             headers=await self._get_headers(),
                         )
                     except aiohttp.client_exceptions.ContentTypeError:
                         raise APIException(403, "Invalid token specified.")
 
@@ -430,15 +433,15 @@
         add_param(params, kwargs, key="length")
         add_param(params, kwargs, key="bpm")
         add_param(params, kwargs, key="query")
         add_param(params, kwargs, key="is_default_sort", converter=to_lower_str)
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url)
-        resp = ArtistResponse.parse_obj(json)
+        resp = ArtistResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_featured_artists, **kwargs)
         return resp
 
     @prepare_token
     async def get_seasonal_backgrounds(self) -> SeasonalBackgroundSet:
@@ -446,15 +449,15 @@
 
         :raises APIException: Contains status code and error message
         :return: Seasonal background set object
         :rtype: aiosu.models.backgrounds.SeasonalBackgroundSet
         """
         url = f"{self.base_url}/api/v2/seasonal-backgrounds"
         json = await self._request("GET", url)
-        return SeasonalBackgroundSet.parse_obj(json)
+        return SeasonalBackgroundSet.model_validate(json)
 
     @prepare_token
     async def get_changelog_listing(self, **kwargs: Any) -> ChangelogListing:
         r"""Gets the changelog listing.
 
         :param \**kwargs:
             See below
@@ -483,15 +486,15 @@
         }
         add_param(params, kwargs, key="from")
         add_param(params, kwargs, key="to")
         add_param(params, kwargs, key="max_id")
         add_param(params, kwargs, key="stream")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = ChangelogListing.parse_obj(json)
+        resp = ChangelogListing.model_validate(json)
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_changelog_listing, **kwargs)
         return resp
 
     @prepare_token
     async def get_changelog_build(self, stream: str, build: str) -> Build:
@@ -501,19 +504,21 @@
         :param build: The build to get
         :raises APIException: Contains status code and error message
         :return: Build object
         :rtype: aiosu.models.changelog.Build
         """
         url = f"{self.base_url}/api/v2/changelog/{stream}/{build}"
         json = await self._request("GET", url)
-        return Build.parse_obj(json)
+        return Build.model_validate(json)
 
     @prepare_token
     async def lookup_changelog_build(
-        self, changelog_query: Union[str, int], **kwargs: Any
+        self,
+        changelog_query: Union[str, int],
+        **kwargs: Any,
     ) -> Build:
         r"""Looks up a build from the changelog.
 
         :param changelog_query: The query to search for
         :type changelog_query: Union[str, int]
         :param \**kwargs:
             See below
@@ -531,15 +536,15 @@
         url = f"{self.base_url}/api/v2/changelog/{changelog_query}"
         params: dict[str, Any] = {
             "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
         }
         if "is_id" in kwargs or isinstance(changelog_query, int):
             params["key"] = "id"
         json = await self._request("GET", url, params=params)
-        return Build.parse_obj(json)
+        return Build.model_validate(json)
 
     @prepare_token
     async def get_news_listing(self, **kwargs: Any) -> NewsListing:
         r"""Gets the news listing.
 
         :param \**kwargs:
             See below
@@ -561,23 +566,25 @@
             raise ValueError("Invalid limit specified. Limit must be between 1 and 21")
         params: dict[str, Any] = {
             "limit": limit,
         }
         add_param(params, kwargs, key="year")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = NewsListing.parse_obj(json)
+        resp = NewsListing.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_news_listing, **kwargs)
         return resp
 
     @prepare_token
     async def get_news_post(
-        self, news_query: Union[str, int], **kwargs: Any
+        self,
+        news_query: Union[str, int],
+        **kwargs: Any,
     ) -> NewsPost:
         r"""Gets a news post.
 
         :param news_query: The query to search for
         :type news_query: Union[str, int]
         :param \**kwargs:
             See below
@@ -593,15 +600,15 @@
         url = f"{self.base_url}/api/v2/news/{news_query}"
         params: dict[str, Any] = {
             "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
         }
         if "is_id" in kwargs or isinstance(news_query, int):
             params["key"] = "id"
         json = await self._request("GET", url, params=params)
-        return NewsPost.parse_obj(json)
+        return NewsPost.model_validate(json)
 
     @prepare_token
     async def get_wiki_page(self, locale: str, path: str) -> WikiPage:
         r"""Gets a wiki page.
 
         :param locale: The locale of the wiki page
         :type locale: str
@@ -609,15 +616,15 @@
         :type path: str
         :raises APIException: Contains status code and error message
         :return: Wiki page object
         :rtype: aiosu.models.wiki.WikiPage
         """
         url = f"{self.base_url}/api/v2/wiki/{locale}/{path}"
         json = await self._request("GET", url)
-        return WikiPage.parse_obj(json)
+        return WikiPage.model_validate(json)
 
     @prepare_token
     async def get_comment(self, comment_id: int, **kwargs: Any) -> CommentBundle:
         r"""Gets a comment.
 
         :param comment_id: The ID of the comment
         :type comment_id: int
@@ -632,15 +639,15 @@
         :return: Comment bundle object
         :rtype: aiosu.models.comment.CommentBundle
         """
         url = f"{self.base_url}/api/v2/comments/{comment_id}"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = CommentBundle.parse_obj(json)
+        resp = CommentBundle.model_validate(json)
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_comment, comment_id=comment_id, **kwargs)
         return resp
 
     @prepare_token
     async def get_comments(self, **kwargs: Any) -> CommentBundle:
@@ -669,15 +676,15 @@
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="commentable_type")
         add_param(params, kwargs, key="commentable_id")
         add_param(params, kwargs, key="parent_id")
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = CommentBundle.parse_obj(json)
+        resp = CommentBundle.model_validate(json)
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_comments, **kwargs)
         return resp
 
     @prepare_token
     @check_token
@@ -703,15 +710,15 @@
         url = f"{self.base_url}/api/v2/search"
         params: dict[str, Any] = {
             "query": query,
             "mode": kwargs.pop("mode", "all"),
         }
         add_param(params, kwargs, key="page")
         json = await self._request("GET", url, params=params)
-        return SearchResponse.parse_obj(json)
+        return SearchResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_me(self, **kwargs: Any) -> User:
         r"""Gets the user who owns the current token
 
@@ -727,30 +734,30 @@
         :rtype: aiosu.models.user.User
         """
         url = f"{self.base_url}/api/v2/me"
         if "mode" in kwargs:
             mode = Gamemode(kwargs.pop("mode"))
             url += f"/{mode}"
         json = await self._request("GET", url)
-        return User.parse_obj(json)
+        return User.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FRIENDS_READ)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_own_friends(self) -> list[User]:
         r"""Gets the token owner's friend list
 
         :raises APIException: Contains status code and error message
         :return: List of friends
         :rtype: list[aiosu.models.user.User]
         """
         url = f"{self.base_url}/api/v2/friends"
         json = await self._request("GET", url)
-        return from_list(User.parse_obj, json)
+        return from_list(User.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
         r"""Gets a user by a query.
 
@@ -778,15 +785,15 @@
             params,
             kwargs,
             key="qtype",
             param_name="type",
             converter=lambda x: UserQueryType(x).new_api_name,
         )
         json = await self._request("GET", url, params=params)
-        return User.parse_obj(json)
+        return User.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_users(self, user_ids: list[int]) -> list[User]:
         r"""Get multiple user data.
 
@@ -797,15 +804,15 @@
         :rtype: list[aiosu.models.user.User]
         """
         url = f"{self.base_url}/api/v2/users"
         params: dict[str, Any] = {
             "ids": user_ids,
         }
         json = await self._request("GET", url, params=params)
-        return from_list(User.parse_obj, json.get("users", []))
+        return from_list(User.model_validate, json.get("users", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user_kudosu(self, user_id: int, **kwargs: Any) -> list[KudosuHistory]:
         r"""Get a user's kudosu history.
 
@@ -825,21 +832,24 @@
         :rtype: list[aiosu.models.kudosu.KudosuHistory]
         """
         url = f"{self.base_url}/api/v2/users/{user_id}/kudosu"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
-        return from_list(KudosuHistory.parse_obj, json)
+        return from_list(KudosuHistory.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def __get_type_scores(
-        self, user_id: int, request_type: str, **kwargs: Any
+        self,
+        user_id: int,
+        request_type: str,
+        **kwargs: Any,
     ) -> list[Union[Score, LazerScore]]:
         r"""INTERNAL: Get a user's scores by type
 
         :param user_id: User ID to search by
         :type user_id: int
         :param request_type: "recent", "best" or "firsts"
         :type request_type: str
@@ -862,15 +872,15 @@
         :raises ValueError: If type is invalid
         :raises APIException: Contains status code and error message
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
         """
         if not 1 <= (limit := kwargs.pop("limit", 100)) <= 100:
             raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
-        if request_type not in ("recent", "best", "firsts"):
+        if request_type not in ("recent", "best", "firsts", "pinned"):
             raise ValueError(
                 f'"{request_type}" is not a valid request_type. Valid options are: "recent", "best", "firsts"',
             )
         url = f"{self.base_url}/api/v2/users/{user_id}/scores/{request_type}"
         params: dict[str, Any] = {
             "include_fails": int(kwargs.pop("include_fails", False)),
             "limit": limit,
@@ -879,19 +889,21 @@
         add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
         headers = {}
         new_format = kwargs.pop("new_format", False)
         if new_format:
             headers = {"x-api-version": "20220705"}
         json = await self._request("GET", url, params=params, headers=headers)
         if new_format:
-            return from_list(LazerScore.parse_obj, json)
-        return from_list(Score.parse_obj, json)
+            return from_list(LazerScore.model_validate, json)
+        return from_list(Score.model_validate, json)
 
     async def get_user_recents(
-        self, user_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        **kwargs: Any,
     ) -> list[Union[Score, LazerScore]]:
         r"""Get a user's recent scores.
 
         :param user_id: User ID to search by
         :type user_id: int
         :param \**kwargs:
             See below
@@ -911,15 +923,17 @@
         :raises APIException: Contains status code and error message
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
         """
         return await self.__get_type_scores(user_id, "recent", **kwargs)
 
     async def get_user_bests(
-        self, user_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        **kwargs: Any,
     ) -> list[Union[Score, LazerScore]]:
         r"""Get a user's top scores.
 
         :param user_id: User ID to search by
         :type user_id: int
         :param \**kwargs:
             See below
@@ -937,15 +951,17 @@
         :raises APIException: Contains status code and error message
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
         """
         return await self.__get_type_scores(user_id, "best", **kwargs)
 
     async def get_user_firsts(
-        self, user_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        **kwargs: Any,
     ) -> list[Union[Score, LazerScore]]:
         r"""Get a user's first place scores.
 
         :param user_id: User ID to search by
         :type user_id: int
         :param \**kwargs:
             See below
@@ -962,19 +978,50 @@
 
         :raises APIException: Contains status code and error message
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
         """
         return await self.__get_type_scores(user_id, "firsts", **kwargs)
 
+    async def get_user_pinned(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""Get a user's pinned scores.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        return await self.__get_type_scores(user_id, "pinned", **kwargs)
+
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user_beatmap_scores(
-        self, user_id: int, beatmap_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        beatmap_id: int,
+        **kwargs: Any,
     ) -> list[Score]:
         r"""Get a user's scores on a specific beatmap.
 
         :param user_id: User ID to search by
         :type user_id: int
         :param beatmap_id: Beatmap ID to search by
         :type beatmap_id: int
@@ -989,23 +1036,26 @@
         :return: List of requested scores
         :rtype: list[aiosu.models.score.Score]
         """
         url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores/users/{user_id}/all"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
         json = await self._request("GET", url, params=params)
-        return from_list(Score.parse_obj, json.get("scores", []))
+        return from_list(Score.model_validate, json.get("scores", []))
 
     UserBeatmapType = Literal["favourite", "graveyard", "loved", "ranked", "pending"]
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user_beatmaps(
-        self, user_id: int, type: UserBeatmapType, **kwargs: Any
+        self,
+        user_id: int,
+        type: UserBeatmapType,
+        **kwargs: Any,
     ) -> list[Beatmapset]:
         r"""Get a user's beatmaps.
 
         :param user_id: ID of the user
         :type user_id: int
         :param type: Type of beatmaps to get
         :type type: UserBeatmapType
@@ -1023,21 +1073,23 @@
         :rtype: list[aiosu.models.beatmap.Beatmap]
         """
         url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/{type}"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
-        return from_list(Beatmapset.parse_obj, json)
+        return from_list(Beatmapset.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user_most_played(
-        self, user_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        **kwargs: Any,
     ) -> list[BeatmapUserPlaycount]:
         r"""Get a user's most played beatmaps.
 
         :param user_id: ID of the user
         :type user_id: int
         :param \**kwargs:
             See below
@@ -1053,21 +1105,23 @@
         :rtype: list[aiosu.models.beatmap.BeatmapUserPlaycount]
         """
         url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/most_played"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
-        return from_list(BeatmapUserPlaycount.parse_obj, json)
+        return from_list(BeatmapUserPlaycount.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_user_recent_activity(
-        self, user_id: int, **kwargs: Any
+        self,
+        user_id: int,
+        **kwargs: Any,
     ) -> list[Event]:
         r"""Get a user's recent activity.
 
         :param user_id: ID of the user
         :type user_id: int
         :param \**kwargs:
             See below
@@ -1083,15 +1137,15 @@
         :rtype: list[aiosu.models.event.Event]
         """
         url = f"{self.base_url}/api/v2/users/{user_id}/recent_activity"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="offset")
         json = await self._request("GET", url, params=params)
-        return from_list(Event.parse_obj, json)
+        return from_list(Event.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
         r"""Get scores submitted on a specific beatmap.
 
@@ -1114,15 +1168,15 @@
         """
         url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
         add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
         add_param(params, kwargs, key="type")
         json = await self._request("GET", url, params=params)
-        return from_list(Score.parse_obj, json.get("scores", []))
+        return from_list(Score.model_validate, json.get("scores", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmap(self, beatmap_id: int) -> Beatmap:
         r"""Get beatmap data.
 
@@ -1130,15 +1184,15 @@
         :type beatmap_id: int
         :raises APIException: Contains status code and error message
         :return: Beatmap data object
         :rtype: aiosu.models.beatmap.Beatmap
         """
         url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}"
         json = await self._request("GET", url)
-        return Beatmap.parse_obj(json)
+        return Beatmap.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmaps(self, beatmap_ids: list[int]) -> list[Beatmap]:
         r"""Get multiple beatmap data.
 
@@ -1149,15 +1203,15 @@
         :rtype: list[aiosu.models.beatmap.Beatmap]
         """
         url = f"{self.base_url}/api/v2/beatmaps"
         params: dict[str, Any] = {
             "ids": beatmap_ids,
         }
         json = await self._request("GET", url, params=params)
-        return from_list(Beatmap.parse_obj, json.get("beatmaps", []))
+        return from_list(Beatmap.model_validate, json.get("beatmaps", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def lookup_beatmap(self, **kwargs: Any) -> Beatmap:
         r"""Lookup beatmap data.
 
@@ -1181,21 +1235,23 @@
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="checksum")
         add_param(params, kwargs, key="filename")
         add_param(params, kwargs, key="id")
         if not params:
             raise ValueError("One of checksum, filename or id must be provided.")
         json = await self._request("GET", url, params=params)
-        return Beatmap.parse_obj(json)
+        return Beatmap.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmap_attributes(
-        self, beatmap_id: int, **kwargs: Any
+        self,
+        beatmap_id: int,
+        **kwargs: Any,
     ) -> BeatmapDifficultyAttributes:
         r"""Gets difficulty attributes for a beatmap.
 
         :param beatmap_id: The ID of the beatmap
         :type beatmap_id: int
         :param \**kwargs:
             See below
@@ -1217,15 +1273,15 @@
             kwargs,
             key="mode",
             param_name="ruleset_id",
             converter=lambda x: int(Gamemode(x)),
         )
         add_param(data, kwargs, key="mods", converter=lambda x: int(Mods(x)))
         json = await self._request("POST", url, json=data)
-        return BeatmapDifficultyAttributes.parse_obj(json.get("attributes"))
+        return BeatmapDifficultyAttributes.model_validate(json.get("attributes"))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
         r"""Get beatmapset data.
 
@@ -1233,15 +1289,15 @@
         :type beatmapset_id: int
         :raises APIException: Contains status code and error message
         :return: Beatmapset data object
         :rtype: aiosu.models.beatmap.Beatmapset
         """
         url = f"{self.base_url}/api/v2/beatmapsets/{beatmapset_id}"
         json = await self._request("GET", url)
-        return Beatmapset.parse_obj(json)
+        return Beatmapset.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def lookup_beatmapset(self, beatmap_id: int) -> Beatmapset:
         r"""Lookup beatmap data.
 
@@ -1253,15 +1309,15 @@
         :rtype: aiosu.models.beatmap.Beatmapset
         """
         url = f"{self.base_url}/api/v2/beatmapsets/lookup"
         params: dict[str, Any] = {
             "beatmap_id": beatmap_id,
         }
         json = await self._request("GET", url, params=params)
-        return Beatmapset.parse_obj(json)
+        return Beatmapset.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def search_beatmapsets(
         self,
         search_filter: Optional[str] = "",
@@ -1282,15 +1338,15 @@
         :return: Beatmapset search response
         :rtype: list[aiosu.models.beatmap.BeatmapsetSearchResponse]
         """
         url = f"{self.base_url}/api/v2/beatmapsets/search/{search_filter}"
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url)
-        resp = BeatmapsetSearchResponse.parse_obj(json)
+        resp = BeatmapsetSearchResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.search_beatmapsets, **kwargs)
         return resp
 
     @prepare_token
     @check_token
@@ -1324,21 +1380,22 @@
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="page")
         add_param(params, kwargs, key="user_id", param_name="user")
         add_param(params, kwargs, key="min_date")
         add_param(params, kwargs, key="max_date")
         add_param(params, kwargs, key="types")
         json = await self._request("GET", url, params=params)
-        return from_list(BeatmapsetEvent.parse_obj, json.get("events", []))
+        return from_list(BeatmapsetEvent.model_validate, json.get("events", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussions(
-        self, **kwargs: Any
+        self,
+        **kwargs: Any,
     ) -> BeatmapsetDiscussionResponse:
         r"""Get beatmapset discussions.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1379,25 +1436,26 @@
         add_param(params, kwargs, key="message_types")
         add_param(params, kwargs, key="only_unresolved", converter=to_lower_str)
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="user", param_name="user_id")
         add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionResponse.parse_obj(json)
+        resp = BeatmapsetDiscussionResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussions, **kwargs)
         return resp
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussion_posts(
-        self, **kwargs: Any
+        self,
+        **kwargs: Any,
     ) -> BeatmapsetDiscussionPostResponse:
         r"""Get beatmapset discussion posts.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1429,25 +1487,26 @@
         add_param(params, kwargs, key="page")
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="types")
         add_param(params, kwargs, key="user", param_name="user_id")
         add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionPostResponse.parse_obj(json)
+        resp = BeatmapsetDiscussionPostResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussion_posts, **kwargs)
         return resp
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_beatmapset_discussion_votes(
-        self, **kwargs: Any
+        self,
+        **kwargs: Any,
     ) -> BeatmapsetDiscussionVoteResponse:
         r"""Get beatmapset discussion votes.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -1482,15 +1541,15 @@
         add_param(params, kwargs, key="receiver", param_name="receiver_id")
         add_param(params, kwargs, key="score")
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="user", param_name="user_id")
         add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionVoteResponse.parse_obj(json)
+        resp = BeatmapsetDiscussionVoteResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_beatmapset_discussion_votes, **kwargs)
         return resp
 
     @prepare_token
     @check_token
@@ -1509,15 +1568,15 @@
 
         :raises APIException: Contains status code and error message
         :return: Score data object
         :rtype: aiosu.models.score.Score
         """
         url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}"
         json = await self._request("GET", url)
-        return Score.parse_obj(json)
+        return Score.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_score_replay(
         self,
@@ -1538,15 +1597,18 @@
         url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}/download"
         return await self._request("GET", url)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_rankings(
-        self, mode: Gamemode, type: RankingType, **kwargs: Any
+        self,
+        mode: Gamemode,
+        type: RankingType,
+        **kwargs: Any,
     ) -> Rankings:
         r"""Get rankings.
 
         :param mode: The gamemode to search for
         :type mode: aiosu.models.gamemode.Gamemode
         :param type: The ranking type to search for
         :type type: aiosu.models.rankings.RankingType
@@ -1573,15 +1635,15 @@
         params: dict[str, Any] = {}
         add_param(params, kwargs, key="country")
         add_param(params, kwargs, key="filter")
         add_param(params, kwargs, key="spotlight")
         add_param(params, kwargs, key="variant")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = Rankings.parse_obj(json)
+        resp = Rankings.model_validate(json)
         if resp.cursor_string:  # Unused: API does not return cursor_string
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_rankings, mode=mode, type=type, **kwargs)
         return resp
 
     @prepare_token
     @check_token
@@ -1591,15 +1653,15 @@
 
         :raises APIException: Contains status code and error message
         :return: List of spotlights
         :rtype: list[aiosu.models.spotlight.Spotlight]
         """
         url = f"{self.base_url}/api/v2/spotlights"
         json = await self._request("GET", url)
-        return from_list(Spotlight.parse_obj, json.get("spotlights", []))
+        return from_list(Spotlight.model_validate, json.get("spotlights", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_forum_topic(self, topic_id: int, **kwargs: Any) -> ForumTopicResponse:
         r"""Gets a forum topic.
 
@@ -1631,26 +1693,30 @@
             "limit": limit,
         }
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="start")
         add_param(params, kwargs, key="end")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = ForumTopicResponse.parse_obj(json)
+        resp = ForumTopicResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_forum_topic, topic_id, **kwargs)
         return resp
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def create_forum_topic(
-        self, forum_id: int, title: str, content: str, **kwargs: Any
+        self,
+        forum_id: int,
+        title: str,
+        content: str,
+        **kwargs: Any,
     ) -> ForumCreateTopicResponse:
         r"""Creates a forum topic.
 
         :param forum_id: The ID of the forum to create the topic in
         :type forum_id: int
         :param title: The title of the topic
         :type title: str
@@ -1698,15 +1764,15 @@
                 forum_topic_poll,
                 kwargs,
                 key="options",
                 param_name="poll_options",
             )
             data["forum_topic_poll"] = forum_topic_poll
         json = await self._request("POST", url, json=data)
-        return ForumCreateTopicResponse.parse_obj(json)
+        return ForumCreateTopicResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def reply_forum_topic(self, topic_id: int, content: str) -> ForumPost:
         r"""Replies to a forum topic.
@@ -1720,15 +1786,15 @@
         :rtype: aiosu.models.forum.ForumPost
         """
         url = f"{self.base_url}/api/v2/forums/topics/{topic_id}/reply"
         data: dict[str, str] = {
             "body": content,
         }
         json = await self._request("POST", url, json=data)
-        return ForumPost.parse_obj(json)
+        return ForumPost.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
     async def edit_forum_topic_title(self, topid_id: int, new_title: str) -> ForumTopic:
         r"""Edits a forum topic's title.
 
@@ -1743,15 +1809,15 @@
         url = f"{self.base_url}/api/v2/forums/topics/{topid_id}/title"
         data: dict[str, dict[str, str]] = {
             "forum_topic": {
                 "topic_title": new_title,
             },
         }
         json = await self._request("PUT", url, json=data)
-        return ForumTopic.parse_obj(json)
+        return ForumTopic.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.FORUM_WRITE)
     async def edit_forum_post(self, post_id: int, new_content: str) -> ForumPost:
         r"""Edits a forum post.
 
@@ -1764,15 +1830,15 @@
         :rtype: aiosu.models.forum.ForumPost
         """
         url = f"{self.base_url}/api/v2/forums/posts/{post_id}"
         data: dict[str, str] = {
             "body": new_content,
         }
         json = await self._request("PUT", url, json=data)
-        return ForumPost.parse_obj(json)
+        return ForumPost.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_chat_ack(self, **kwargs: Any) -> list[ChatUserSilence]:
         r"""Gets chat acknowledgement.
@@ -1791,15 +1857,15 @@
         :rtype: list[aiosu.models.chat.ChatUserSilence]
         """
         url = f"{self.base_url}/api/v2/chat/ack"
         data: dict[str, Any] = {}
         add_param(data, kwargs, key="since")
         add_param(data, kwargs, key="silence_id_since", param_name="history_since")
         json = await self._request("POST", url, json=data)
-        return from_list(ChatUserSilence.parse_obj, json.get("silences", []))
+        return from_list(ChatUserSilence.model_validate, json.get("silences", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_chat_updates(self, since: int, **kwargs: Any) -> ChatUpdateResponse:
         r"""Gets chat updates.
@@ -1831,15 +1897,15 @@
             "since": since,
             "limit:": limit,
         }
         add_param(params, kwargs, key="channel_id")
         add_param(params, kwargs, key="includes")
         add_param(params, kwargs, key="silence_id_since", param_name="history_since")
         json = await self._request("GET", url, params=params)
-        return ChatUpdateResponse.parse_obj(json)
+        return ChatUpdateResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channel(self, channel_id: int) -> ChatChannelResponse:
         r"""Gets channel.
@@ -1848,37 +1914,39 @@
         :type channel_id: int
         :raises APIException: Contains status code and error message
         :return: Chat channel object
         :rtype: aiosu.models.chat.ChatChannelResponse
         """
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}"
         json = await self._request("GET", url)
-        return ChatChannelResponse.parse_obj(json)
+        return ChatChannelResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channels(self) -> list[ChatChannel]:
         r"""Gets a list of joinable public channels.
 
         :raises APIException: Contains status code and error message
         :return: List of chat channel objects
         :rtype: list[aiosu.models.chat.ChatChannel]
         """
         url = f"{self.base_url}/api/v2/chat/channels"
         json = await self._request("GET", url)
-        return from_list(ChatChannel.parse_obj, json)
+        return from_list(ChatChannel.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_channel_messages(
-        self, channel_id: int, **kwargs: Any
+        self,
+        channel_id: int,
+        **kwargs: Any,
     ) -> list[ChatMessage]:
         r"""Gets channel messages.
 
         :param channel_id: The channel ID to get messages from
         :type channel_id: int
         :param \**kwargs:
             See below
@@ -1901,22 +1969,24 @@
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
         params: dict[str, Any] = {
             "limit:": limit,
         }
         add_param(params, kwargs, key="since")
         add_param(params, kwargs, key="until")
         json = await self._request("GET", url, params=params)
-        return from_list(ChatMessage.parse_obj, json)
+        return from_list(ChatMessage.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.CHAT_WRITE)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def create_chat_channel(
-        self, type: ChatChannelTypes, **kwargs: Any
+        self,
+        type: ChatChannelTypes,
+        **kwargs: Any,
     ) -> ChatChannel:
         r"""Creates a chat channel.
 
         :param type: The type of the channel.
         :type type: aiosu.models.chat.ChatChannelType
         :param \**kwargs:
             See below
@@ -1953,15 +2023,15 @@
                 raise ValueError("Missing message")
             channel = {
                 "name": kwargs["channel_name"],
                 "description": kwargs["channel_description"],
             }
             data["channel"] = channel
         json = await self._request("POST", url, json=data)
-        return ChatChannel.parse_obj(json)
+        return ChatChannel.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def join_channel(self, channel_id: int, user_id: int) -> ChatChannel:
         r"""Joins a channel.
@@ -1972,15 +2042,15 @@
         :type user_id: int
         :raises APIException: Contains status code and error message
         :return: Chat channel object
         :rtype: aiosu.models.chat.ChatChannel
         """
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
         json = await self._request("PUT", url)
-        return ChatChannel.parse_obj(json)
+        return ChatChannel.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.LAZER)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def leave_channel(self, channel_id: int, user_id: int) -> None:
         r"""Leaves a channel.
@@ -2034,22 +2104,26 @@
         """
         url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
         data: dict[str, Any] = {
             "message": message,
             "is_action": is_action,
         }
         json = await self._request("POST", url, json=data)
-        return ChatMessage.parse_obj(json)
+        return ChatMessage.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.CHAT_WRITE)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def send_private_message(
-        self, user_id: int, message: str, is_action: bool, **kwargs: Any
+        self,
+        user_id: int,
+        message: str,
+        is_action: bool,
+        **kwargs: Any,
     ) -> ChatMessageCreateResponse:
         r"""Sends a message to a user.
 
         :param user_id: The ID of the user
         :type user_id: int
         :param message: The message to send
         :type message: str
@@ -2070,21 +2144,22 @@
         data: dict[str, Any] = {
             "target_id": user_id,
             "message": message,
             "is_action": is_action,
         }
         add_param(data, kwargs, key="uuid")
         json = await self._request("POST", url, json=data)
-        return ChatMessageCreateResponse.parse_obj(json)
+        return ChatMessageCreateResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_matches(
-        self, **kwargs: Any
+        self,
+        **kwargs: Any,
     ) -> MultiplayerMatchesResponse:
         r"""Gets the multiplayer matches.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
@@ -2104,25 +2179,27 @@
             raise ValueError("Limit must be between 1 and 50")
         url = f"{self.base_url}/api/v2/matches"
         params: dict[str, Any] = {
             "limit": limit,
         }
         add_param(params, kwargs, key="sort")
         json = await self._request("GET", url, params=params)
-        resp = MultiplayerMatchesResponse.parse_obj(json)
+        resp = MultiplayerMatchesResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(self.get_multiplayer_matches, **kwargs)
         return resp
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_match(
-        self, match_id: int, **kwargs: Any
+        self,
+        match_id: int,
+        **kwargs: Any,
     ) -> MultiplayerMatchResponse:
         r"""Gets a multiplayer match.
 
         :param match_id: The ID of the match
         :type match_id: int
         :param \**kwargs:
             See below
@@ -2145,15 +2222,15 @@
         url = f"{self.base_url}/api/v2/matches/{match_id}"
         params: dict[str, Any] = {
             "limit": limit,
         }
         add_param(params, kwargs, key="before")
         add_param(params, kwargs, key="after")
         json = await self._request("GET", url)
-        return MultiplayerMatchResponse.parse_obj(json)
+        return MultiplayerMatchResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_multiplayer_rooms(self, **kwargs: Any) -> list[MultiplayerRoom]:
         r"""Gets the multiplayer rooms.
@@ -2187,15 +2264,15 @@
         params: dict[str, Any] = {
             "limit": limit,
         }
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="category")
         add_param(params, kwargs, key="type", param_name="type_group")
         json = await self._request("GET", url, params=params)
-        return from_list(MultiplayerRoom.parse_obj, json)
+        return from_list(MultiplayerRoom.model_validate, json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_room(self, room_id: int) -> MultiplayerRoom:
         r"""Gets a multiplayer room.
 
@@ -2204,22 +2281,24 @@
 
         :raises APIException: Contains status code and error message
         :return: Multiplayer room object
         :rtype: aiosu.models.multiplayer.MultiplayerRoom
         """
         url = f"{self.base_url}/api/v2/rooms/{room_id}"
         json = await self._request("GET", url)
-        return MultiplayerRoom.parse_obj(json)
+        return MultiplayerRoom.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
     async def get_multiplayer_leaderboard(
-        self, room_id: int, **kwargs: Any
+        self,
+        room_id: int,
+        **kwargs: Any,
     ) -> MultiplayerLeaderboardResponse:
         r"""Gets the multiplayer leaderboard for a room.
 
         :param room_id: The ID of the room
         :type room_id: int
         :param \**kwargs:
             See below
@@ -2236,21 +2315,24 @@
         if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
             raise ValueError("Limit must be between 1 and 50")
         url = f"{self.base_url}/api/v2/rooms/{room_id}/leaderboard"
         params: dict[str, Any] = {
             "limit": limit,
         }
         json = await self._request("GET", url, params=params)
-        return MultiplayerLeaderboardResponse.parse_obj(json)
+        return MultiplayerLeaderboardResponse.model_validate(json)
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
     async def get_multiplayer_scores(
-        self, room_id: int, playlist_id: int, **kwargs: Any
+        self,
+        room_id: int,
+        playlist_id: int,
+        **kwargs: Any,
     ) -> MultiplayerScoresResponse:
         r"""Gets the multiplayer scores for a room.
 
         :param room_id: The ID of the room
         :type room_id: int
         :param playlist_id: The ID of the playlist
         :type playlist_id: int
@@ -2275,19 +2357,22 @@
         url = f"{self.base_url}/api/v2/rooms/{room_id}/playlist/{playlist_id}/scores"
         params: dict[str, Any] = {
             "limit": limit,
         }
         add_param(params, kwargs, key="sort")
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
-        resp = MultiplayerScoresResponse.parse_obj(json)
+        resp = MultiplayerScoresResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
             resp.next = partial(
-                self.get_multiplayer_scores, room_id, playlist_id, **kwargs
+                self.get_multiplayer_scores,
+                room_id,
+                playlist_id,
+                **kwargs,
             )
         return resp
 
     @prepare_token
     @check_token
     async def revoke_token(self) -> None:
         r"""Revokes the current token and closes the session.
```

### Comparing `aiosu-1.5.0/aiosu/v2/clientstorage.py` & `aiosu-2.0.0/aiosu/v2/clientstorage.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/aiosu/v2/repository/oauthtoken.py` & `aiosu-2.0.0/aiosu/v2/repository/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-1.5.0/pyproject.toml` & `aiosu-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 check_untyped_defs = true
 warn_unused_ignores = true
 show_error_codes = true
 [tools.pytest.ini_options]
 testpaths = ["tests"]
 [tool.poetry]
 name = "aiosu"
-version = "1.5.0"
+version = "2.0.0"
 description = "Simple and fast osu! API v1 and v2 library"
 authors = ["Nice Aesthetics <nice@aesth.dev>"]
 license = "GPLv3+"
 readme = "README.rst"
 repository = "https://github.com/NiceAesth/aiosu"
 documentation = "https://aiosu.readthedocs.io/"
 keywords = ["osu!", "osu", "api"]
@@ -29,37 +29,37 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8.3"
 aiolimiter = "^1.0.0"
 emojiflags = "^0.1.1"
 orjson = "^3.8.3"
-pydantic = "^1.10.2"
+pydantic = "^2.0.3"
 pytest = {version="^7.2.0", optional = true}
 pytest-asyncio = {version="^0.21.0", optional = true}
 pytest-mock = {version="^3.10.0", optional = true}
 toml = {version="^0.10.2", optional = true}
-sphinx = {version="^6.0.0", optional = true}
-sphinx-rtd-theme = {version="^1.1.1", optional = true}
+sphinx = {version="^7.0.0", optional = true}
+furo = {version="^2023.5.20", optional = true}
 types-toml = {version = "^0.10.8.1", optional = true}
 pyjwt = "^2.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
 mypy = "^1.0"
 toml = "^0.10.2"
 types-toml = "^0.10.8.1"
-sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.2.0"
+sphinx = "^7.0.0"
+furo = "^2023.5.20"
 pytest-cov = "^4.0.0"
 black = {version = "^23.0.0", allow-prereleases = true}
 pre-commit = "^3.2.2"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
-docs = ["Sphinx", "sphinx-rtd-theme", "toml"]
+docs = ["Sphinx", "furo", "toml"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aiosu-1.5.0/PKG-INFO` & `aiosu-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosu
-Version: 1.5.0
+Version: 2.0.0
 Summary: Simple and fast osu! API v1 and v2 library
 Home-page: https://github.com/NiceAesth/aiosu
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Provides-Extra: test
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
 Requires-Dist: emojiflags (>=0.1.1,<0.2.0)
+Requires-Dist: furo (>=2023.5.20,<2024.0.0) ; extra == "docs"
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0) ; extra == "test"
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0) ; extra == "test"
-Requires-Dist: sphinx (>=6.0.0,<7.0.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx (>=7.0.0,<8.0.0) ; extra == "docs"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "test" or extra == "docs"
 Requires-Dist: types-toml (>=0.10.8.1,<0.11.0.0) ; extra == "test"
 Project-URL: Documentation, https://aiosu.readthedocs.io/
 Project-URL: Repository, https://github.com/NiceAesth/aiosu
 Description-Content-Type: text/x-rst
 
 aiosu
@@ -108,15 +108,15 @@
 
     import aiosu
     import asyncio
     import datetime
 
 
     async def main():
-        token = aiosu.models.OAuthToken.parse_obj(json_token_from_api)
+        token = aiosu.models.OAuthToken.model_validate(json_token_from_api)
 
         # or
 
         token = aiosu.models.OAuthToken(
             access_token="access token",
             refresh_token="refresh token",
             expires_on=datetime.datetime.utcnow()
```

