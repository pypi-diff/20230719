# Comparing `tmp/arraylake_client-0.4.3.tar.gz` & `tmp/arraylake_client-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake_client-0.4.3.tar", max compression
+gzip compressed data, was "arraylake_client-0.4.4.tar", max compression
```

## Comparing `arraylake_client-0.4.3.tar` & `arraylake_client-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      633 2023-07-11 00:45:35.236162 arraylake_client-0.4.3/README.md
--rw-r--r--   0        0        0      357 2023-06-07 16:41:28.210985 arraylake_client-0.4.3/arraylake_client/__init__.py
--rw-r--r--   0        0        0       70 2023-06-07 16:41:28.212174 arraylake_client-0.4.3/arraylake_client/__main__.py
--rw-r--r--   0        0        0    15553 2023-07-11 00:45:35.238345 arraylake_client-0.4.3/arraylake_client/api_utils.py
--rw-r--r--   0        0        0     2381 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/async_utils.py
--rw-r--r--   0        0        0      630 2023-06-07 16:41:28.212923 arraylake_client-0.4.3/arraylake_client/chunkstore/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-07 16:41:28.213251 arraylake_client-0.4.3/arraylake_client/chunkstore/abc.py
--rw-r--r--   0        0        0     5201 2023-06-07 16:41:28.213373 arraylake_client-0.4.3/arraylake_client/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2023-06-07 16:41:28.213456 arraylake_client-0.4.3/arraylake_client/cli/__init__.py
--rw-r--r--   0        0        0     3973 2023-07-11 00:45:35.238508 arraylake_client-0.4.3/arraylake_client/cli/auth.py
--rw-r--r--   0        0        0     4762 2023-06-07 16:41:28.213838 arraylake_client-0.4.3/arraylake_client/cli/config.py
--rw-r--r--   0        0        0     1155 2023-06-07 16:41:28.213908 arraylake_client-0.4.3/arraylake_client/cli/main.py
--rw-r--r--   0        0        0     3568 2023-06-22 20:23:42.539238 arraylake_client-0.4.3/arraylake_client/cli/repo.py
--rw-r--r--   0        0        0     3390 2023-06-07 16:41:28.214762 arraylake_client-0.4.3/arraylake_client/cli/utils.py
--rw-r--r--   0        0        0     7621 2023-07-11 00:45:35.239080 arraylake_client-0.4.3/arraylake_client/client.py
--rw-r--r--   0        0        0     7098 2023-06-13 00:03:11.755118 arraylake_client-0.4.3/arraylake_client/commits.py
--rw-r--r--   0        0        0      538 2023-06-07 16:41:28.215453 arraylake_client-0.4.3/arraylake_client/config.py
--rw-r--r--   0        0        0      105 2023-06-07 16:41:28.215671 arraylake_client-0.4.3/arraylake_client/config.yaml
--rw-r--r--   0        0        0      192 2023-06-07 18:29:47.978531 arraylake_client-0.4.3/arraylake_client/exceptions.py
--rw-r--r--   0        0        0     1110 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/log_util.py
--rw-r--r--   0        0        0      282 2023-06-22 20:23:42.540028 arraylake_client-0.4.3/arraylake_client/metastore/__init__.py
--rw-r--r--   0        0        0     8188 2023-07-08 00:39:33.338322 arraylake_client-0.4.3/arraylake_client/metastore/abc.py
--rw-r--r--   0        0        0    12667 2023-07-11 00:45:35.239261 arraylake_client-0.4.3/arraylake_client/metastore/http_metastore.py
--rw-r--r--   0        0        0    52115 2023-07-08 00:45:35.560450 arraylake_client-0.4.3/arraylake_client/repo.py
--rw-r--r--   0        0        0     1227 2023-06-22 20:23:42.540945 arraylake_client-0.4.3/arraylake_client/spec.py
--rw-r--r--   0        0        0     4550 2023-07-11 00:45:35.239407 arraylake_client-0.4.3/arraylake_client/token.py
--rw-r--r--   0        0        0     9753 2023-06-22 20:23:42.541106 arraylake_client-0.4.3/arraylake_client/types.py
--rw-r--r--   0        0        0    10315 2023-06-27 00:27:16.448369 arraylake_client-0.4.3/arraylake_client/virtual.py
--rw-r--r--   0        0        0      851 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/zarr_util.py
--rw-r--r--   0        0        0     2337 2023-07-11 00:49:57.966500 arraylake_client-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 arraylake_client-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/README.md
+-rw-r--r--   0        0        0      357 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/__main__.py
+-rw-r--r--   0        0        0    15553 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/api_utils.py
+-rw-r--r--   0        0        0     2381 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/async_utils.py
+-rw-r--r--   0        0        0      630 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/__init__.py
+-rw-r--r--   0        0        0     1534 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/abc.py
+-rw-r--r--   0        0        0     5201 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/__init__.py
+-rw-r--r--   0        0        0     3973 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/auth.py
+-rw-r--r--   0        0        0     4762 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/config.py
+-rw-r--r--   0        0        0     1155 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/main.py
+-rw-r--r--   0        0        0     3568 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/repo.py
+-rw-r--r--   0        0        0     3390 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/utils.py
+-rw-r--r--   0        0        0     7778 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/client.py
+-rw-r--r--   0        0        0     7098 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/commits.py
+-rw-r--r--   0        0        0      538 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/config.py
+-rw-r--r--   0        0        0      105 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/config.yaml
+-rw-r--r--   0        0        0      192 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/exceptions.py
+-rw-r--r--   0        0        0     1110 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/log_util.py
+-rw-r--r--   0        0        0      282 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/__init__.py
+-rw-r--r--   0        0        0     8943 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/abc.py
+-rw-r--r--   0        0        0    13035 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/http_metastore.py
+-rw-r--r--   0        0        0    53388 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/repo.py
+-rw-r--r--   0        0        0     1227 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/spec.py
+-rw-r--r--   0        0        0     4550 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/token.py
+-rw-r--r--   0        0        0     9753 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/types.py
+-rw-r--r--   0        0        0    10315 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/virtual.py
+-rw-r--r--   0        0        0      851 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/zarr_util.py
+-rw-r--r--   0        0        0     2337 2023-07-19 00:27:47.453407 arraylake_client-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 arraylake_client-0.4.4/PKG-INFO
```

### Comparing `arraylake_client-0.4.3/README.md` & `arraylake_client-0.4.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# arraylake-client
-
 <p align="center">
-<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="200" alt="Arraylake">
+<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="80%" alt="Arraylake">
 </p>
 
 <p align="center">
   <a href="https://earthmover.io" rel="nofollow">earthmover.io</a> -
   <a href="https://docs.earthmover.io" rel="nofollow">documentation</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
-# arraylake-client
                                   [Arraylake]
                          earthmover.io - documentation
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Checkout the [documentation](https://
 docs.earthmover.io) to get started. ## Install ``` pip install
 "arraylake_client[cli]" ```
```

### Comparing `arraylake_client-0.4.3/arraylake_client/api_utils.py` & `arraylake_client-0.4.4/arraylake_client/api_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/async_utils.py` & `arraylake_client-0.4.4/arraylake_client/async_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/chunkstore/__init__.py` & `arraylake_client-0.4.4/arraylake_client/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/chunkstore/abc.py` & `arraylake_client-0.4.4/arraylake_client/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/chunkstore/s3chunkstore.py` & `arraylake_client-0.4.4/arraylake_client/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/cli/auth.py` & `arraylake_client-0.4.4/arraylake_client/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/cli/config.py` & `arraylake_client-0.4.4/arraylake_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/cli/main.py` & `arraylake_client-0.4.4/arraylake_client/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/cli/repo.py` & `arraylake_client-0.4.4/arraylake_client/cli/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/cli/utils.py` & `arraylake_client-0.4.4/arraylake_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/client.py` & `arraylake_client-0.4.4/arraylake_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     """
 
     service_uri: Optional[str] = None
     token: Optional[str] = field(default=None, repr=False)
     auth_org: Optional[str] = None
 
     def __post_init__(self):
+        if self.token is not None and not self.token.startswith("ema_"):
+            raise ValueError("Invalid token provided. Tokens must start with ema_")
         if self.service_uri is None:
             self.service_uri = config.get("service.uri")
         self.auth_org = self.auth_org or config.get("user.org", None)
 
     # TODO: replace the return type with a stricted type around repo listing object
     async def list_repos(self, org: str) -> Sequence[dict]:
         """List all repositories for the specified org
```

### Comparing `arraylake_client-0.4.3/arraylake_client/commits.py` & `arraylake_client-0.4.4/arraylake_client/commits.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/config.py` & `arraylake_client-0.4.4/arraylake_client/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/log_util.py` & `arraylake_client-0.4.4/arraylake_client/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/metastore/abc.py` & `arraylake_client-0.4.4/arraylake_client/metastore/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,35 @@
         Returns
         -------
         CommitID
         """
         ...
 
     @abstractmethod
+    async def rebase(self, commit_id: CommitID, upstream_branch: BranchName) -> CommitID:
+        """Determine if a commit_id can cleanly be updated to a target branch HEAD.
+
+        Clean update means that there are no conflicting path updates in intermediate commits between
+        commit_id and the HEAD commit of the upstream_branch. If the update can be performed cleanly,
+        return the target branch commit_id to the caller, else raise an exception.
+
+        Note: This is a read-only operations, it should not create or modify commits or branch states.
+
+        Returns
+        -------
+        CommitID
+
+        Raises
+        ------
+        ValueError
+            if clean update is not possible
+        """
+        ...
+
+    @abstractmethod
     async def update_branch(
         self, branch: BranchName, *, base_commit: Optional[CommitID], new_commit: CommitID, new_branch: bool = False
     ) -> None:
         """Update a branch reference in an atomic transaction.
 
         Parameters
         ----------
```

### Comparing `arraylake_client-0.4.3/arraylake_client/metastore/http_metastore.py` & `arraylake_client-0.4.4/arraylake_client/metastore/http_metastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,20 @@
 
     async def new_commit(self, commit_info: NewCommit) -> CommitID:
         response = await self._request("PUT", f"{self._repo_path}/commits", content=commit_info.json())
         handle_response(response)
 
         return PyObjectId(response.json()["_id"])
 
+    async def rebase(self, commit_id: CommitID, upstream_branch: BranchName) -> CommitID:
+        body = {"commit_id": str(commit_id) if commit_id else None, "branch_name": upstream_branch}
+        response = await self._request("POST", f"{self._repo_path}/rebase", params=body)
+        handle_response(response)
+        return CommitID(response.json()["commit_id"])
+
     async def update_branch(
         self, branch: BranchName, *, base_commit: Optional[CommitID], new_commit: CommitID, new_branch: bool = False
     ) -> None:
         body = UpdateBranchBody(branch=branch, new_commit=new_commit, base_commit=base_commit, new_branch=new_branch)
         response = await self._request("PUT", f"{self._repo_path}/branches", content=body.json())
         handle_response(response)
```

### Comparing `arraylake_client-0.4.3/arraylake_client/repo.py` & `arraylake_client-0.4.4/arraylake_client/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import datetime
 import functools
 import json
+import random
 import uuid
 import warnings
 from dataclasses import dataclass
 from html import escape
 from typing import (
     AsyncGenerator,
     Awaitable,
@@ -36,14 +37,15 @@
     TypeVar,
 )
 
 import zarr
 from zarr._storage.store import StoreV3
 from zarr.util import normalize_storage_path
 
+from arraylake_client import config as config_obj
 from arraylake_client.async_utils import (
     BlockingPortal,
     BlockingPortalGenerator,
     cached_portal,
 )
 from arraylake_client.chunkstore import Chunkstore
 from arraylake_client.commits import CommitData, CommitLog
@@ -273,24 +275,20 @@
         Args:
             message: Commit message
             auto_ff: Whether to automatically fast-forward the repo and retry if the commit fails
 
         Returns:
             new_commit: ID of new commit
         """
-        try:
-            return await self._single_commit(message)
-        except CommitFailedError:
-            if auto_ff:
-                await self.fast_forward()
-                return await self._single_commit(message)
-            else:
-                raise
+        return await self._single_commit(message)
 
-    async def _single_commit(self, message: str) -> CommitID:
+    async def _single_commit(self, message: str, attempt=0) -> CommitID:
+        """Create a new commit based on current state and attempt to write to branch."""
+        max_attempts = int(config_obj.config.get("max_commit_attempts", 50))
+        max_jitter = 5  # seconds
         if self.session["branch"] is None:
             raise RuntimeError("You are not on a branch tip, so you can't commit changes.")
 
         commit_metadata = NewCommit(
             session_id=self.session["id"],
             session_start_time=self.session["start_time"],
             parent_commit=self.session.get("base_commit", None),
@@ -312,22 +310,45 @@
                 raise err
 
         new_branch = (self.session["branch"] not in (await self.commit_data()).branches) or (self.session["base_commit"] is None)
         try:
             await self.db.update_branch(
                 self.session["branch"], base_commit=self.session["base_commit"], new_commit=new_commit, new_branch=new_branch
             )
-        except Exception:
-            raise CommitFailedError(f"Failed to update branch {self.session['branch']} to point to commit {new_commit}")
+        # TODO: fix metastore impl. inconsistency around error classes here
+        except (ValueError, RuntimeError) as err:
+            if not (str(err).startswith("Failed to update branch") or str(err).startswith("Cannot create branch")):
+                raise
+            else:
+                if attempt < max_attempts:
+                    await logger.ainfo(f"Encountered commit conflict {attempt}, retrying")
+                    # add a small amount of jitter to avoid dos
+                    delay = random.uniform(0, max_jitter)
+                    await asyncio.sleep(delay)
+                    await self._rebase(new_commit)
+                    return await self._single_commit(message, attempt=attempt + 1)
+                else:
+                    raise CommitFailedError(f"Failed to update branch {self.session['branch']} to point to commit {new_commit}")
 
         # reset session parameters
         checked_out_commit = await self.checkout(self.session["branch"])
         assert checked_out_commit == new_commit, "These should always match"
         return new_commit
 
+    async def _rebase(self, commit_id: CommitID):
+        """Update the session base commit to branch HEAD, if possible."""
+        branch = self.session["branch"]
+        try:
+            latest_branch_commit_id = await self.db.rebase(commit_id, branch)
+            self._session["base_commit"] = latest_branch_commit_id
+            await self._refresh_commit_data()
+        except ValueError as err:
+            if not str(err).startswith("Branch does not exist"):
+                raise
+
     async def fast_forward(self):
         """Fast-forward the session.
         Attempts to update the session base commit to the latest branch tip.
         Will fail if the same paths have been modified in the current session and on the branch.
         """
         try:
             latest_commit = await self._try_fast_forward()
```

### Comparing `arraylake_client-0.4.3/arraylake_client/spec.py` & `arraylake_client-0.4.4/arraylake_client/spec.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/token.py` & `arraylake_client-0.4.4/arraylake_client/token.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/types.py` & `arraylake_client-0.4.4/arraylake_client/types.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/virtual.py` & `arraylake_client-0.4.4/arraylake_client/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/arraylake_client/zarr_util.py` & `arraylake_client-0.4.4/arraylake_client/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.3/pyproject.toml` & `arraylake_client-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake-client"
-version = "0.4.3"  # placeholder
+version = "0.4.4"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake_client"}]
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `arraylake_client-0.4.3/PKG-INFO` & `arraylake_client-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylake-client
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,18 +29,16 @@
 Requires-Dist: s3fs (>=2022.11.0) ; extra == "virtual"
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: typer (>=0.6.1,<1.0) ; extra == "cli"
 Requires-Dist: types-aiobotocore (>=2.4.0,<3.0.0)
 Requires-Dist: zarr (>=2.14,<2.15)
 Description-Content-Type: text/markdown
 
-# arraylake-client
-
 <p align="center">
-<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="200" alt="Arraylake">
+<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="80%" alt="Arraylake">
 </p>
 
 <p align="center">
   <a href="https://earthmover.io" rel="nofollow">earthmover.io</a> -
   <a href="https://docs.earthmover.io" rel="nofollow">documentation</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.3 Summary: Python
+Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.4 Summary: Python
 client for ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cli Provides-Extra: virtual Provides-Extra: widgets Requires-
 Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: anyio (>=3.6.1,<4.0.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0) Requires-Dist: donfig (>=0.7,<1.0)
@@ -12,15 +12,15 @@
 kerchunk (>=0.1,<1.0) ; extra == "virtual" Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: pydantic[email] (>=1.10,<2.0) Requires-Dist: pymongo
 (>=4.2.0,<5.0.0) Requires-Dist: rich (>=12.6,<14.0) ; extra == "cli" Requires-
 Dist: ruamel-yaml (>=0.17,<1.0) ; extra == "cli" Requires-Dist: s3fs
 (>=2022.11.0) ; extra == "virtual" Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: typer (>=0.6.1,<1.0) ; extra == "cli" Requires-Dist: types-
 aiobotocore (>=2.4.0,<3.0.0) Requires-Dist: zarr (>=2.14,<2.15) Description-
-Content-Type: text/markdown # arraylake-client
+Content-Type: text/markdown
                                   [Arraylake]
                          earthmover.io - documentation
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Checkout the [documentation](https://
 docs.earthmover.io) to get started. ## Install ``` pip install
 "arraylake_client[cli]" ```
```

