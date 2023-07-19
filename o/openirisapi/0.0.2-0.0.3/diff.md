# Comparing `tmp/openirisapi-0.0.2.tar.gz` & `tmp/openirisapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirisapi-0.0.2.tar", last modified: Wed Nov 23 14:05:39 2022, max compression
+gzip compressed data, was "openirisapi-0.0.3.tar", last modified: Wed Jul 19 11:30:15 2023, max compression
```

## Comparing `openirisapi-0.0.2.tar` & `openirisapi-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 14:05:39.786946 openirisapi-0.0.2/
--rw-rw-rw-   0        0        0     1100 2022-11-23 12:53:28.000000 openirisapi-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0     2114 2022-11-23 14:05:39.786946 openirisapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1497 2022-11-23 12:53:28.000000 openirisapi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-23 14:05:39.771314 openirisapi-0.0.2/openirisapi/
--rw-rw-rw-   0        0        0        0 2022-11-23 12:53:28.000000 openirisapi-0.0.2/openirisapi/__init__.py
--rw-rw-rw-   0        0        0    15286 2022-11-23 12:53:28.000000 openirisapi-0.0.2/openirisapi/openirisapi.py
--rw-rw-rw-   0        0        0     1126 2022-11-23 12:53:28.000000 openirisapi-0.0.2/openirisapi/utilities.py
-drwxrwxrwx   0        0        0        0 2022-11-23 14:05:39.771314 openirisapi-0.0.2/openirisapi.egg-info/
--rw-rw-rw-   0        0        0     2114 2022-11-23 14:05:39.000000 openirisapi-0.0.2/openirisapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2022-11-23 14:05:39.000000 openirisapi-0.0.2/openirisapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 14:05:39.000000 openirisapi-0.0.2/openirisapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-11-23 14:05:39.000000 openirisapi-0.0.2/openirisapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-23 14:05:39.000000 openirisapi-0.0.2/openirisapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2022-11-23 12:53:28.000000 openirisapi-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      701 2022-11-23 14:05:39.786946 openirisapi-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 11:30:15.214659 openirisapi-0.0.3/
+-rw-rw-rw-   0        0        0     1100 2022-11-23 12:53:28.000000 openirisapi-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0     2221 2023-07-19 11:30:15.214659 openirisapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-03-02 10:59:07.000000 openirisapi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 11:30:15.194140 openirisapi-0.0.3/openirisapi/
+-rw-rw-rw-   0        0        0        0 2022-11-23 12:53:28.000000 openirisapi-0.0.3/openirisapi/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 14:42:06.000000 openirisapi-0.0.3/openirisapi/io_analysis.py
+-rw-rw-rw-   0        0        0    21419 2023-07-19 11:21:04.000000 openirisapi-0.0.3/openirisapi/openirisapi.py
+-rw-rw-rw-   0        0        0     1454 2023-07-19 11:21:04.000000 openirisapi-0.0.3/openirisapi/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:30:15.214659 openirisapi-0.0.3/openirisapi.egg-info/
+-rw-rw-rw-   0        0        0     2221 2023-07-19 11:30:15.000000 openirisapi-0.0.3/openirisapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-19 11:30:15.000000 openirisapi-0.0.3/openirisapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:30:15.000000 openirisapi-0.0.3/openirisapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 11:30:15.000000 openirisapi-0.0.3/openirisapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 11:30:15.000000 openirisapi-0.0.3/openirisapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2022-11-23 12:53:28.000000 openirisapi-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      701 2023-07-19 11:30:15.214659 openirisapi-0.0.3/setup.cfg
```

### Comparing `openirisapi-0.0.2/LICENCE.txt` & `openirisapi-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `openirisapi-0.0.2/PKG-INFO` & `openirisapi-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openirisapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very basic API built upon requests for openiris.io
 Home-page: https://gitlab.in2p3.fr/sotirios.PAPADIAMANTIS/openirisAPI
 Author: Sotiris Papadiamantis
 Author-email: sotirios.papadiamantis@univ-amu.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ## OpenIRIS API
 
+[![Downloads](https://static.pepy.tech/badge/openirisapi/month)](https://pepy.tech/project/openirisapi)
+
 A simple API for [openiris.io](openiris.io). OpenIRIS is a free platform permitting the publishing and management of resources form microscopy units.
 
 This API was developped as part of a France BioImaging project and is offered for use to anyone in the scientific community.
 
 At the moment, there is no REST API published by the site's developpers. This package aims to provide a functional solution that permits PROVIDER ardministration to download data directly from the website's backend.
 
 To get your cookie you have to use the Dev tools of your browser, Network > Cookie script > Cookie. You must then format it into a python dictionary and store it in a .txt file.
```

### Comparing `openirisapi-0.0.2/README.md` & `openirisapi-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## OpenIRIS API
 
+[![Downloads](https://static.pepy.tech/badge/openirisapi/month)](https://pepy.tech/project/openirisapi)
+
 A simple API for [openiris.io](openiris.io). OpenIRIS is a free platform permitting the publishing and management of resources form microscopy units.
 
 This API was developped as part of a France BioImaging project and is offered for use to anyone in the scientific community.
 
 At the moment, there is no REST API published by the site's developpers. This package aims to provide a functional solution that permits PROVIDER ardministration to download data directly from the website's backend.
 
 To get your cookie you have to use the Dev tools of your browser, Network > Cookie script > Cookie. You must then format it into a python dictionary and store it in a .txt file.
```

### Comparing `openirisapi-0.0.2/openirisapi/openirisapi.py` & `openirisapi-0.0.3/openirisapi/openirisapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Small API for openiris.io using Python Requests.
 Downstream flow only, no support for create and
 update operations for the time being.
 
 Author: Sotiris Papadiamantis
 """
 import requests
-from .utilities import data_from_raw, get_cookie
+from .utilities import data_from_raw
 import pandas as pd
 
 
 def getBookings(cookies, start="2002-03-07", end="2024-03-07"):
     """
     Downloads all bookings linked to a specific cookie
 
@@ -185,33 +185,33 @@
     # If flag save in csv form
     if to_csv:
         data.to_csv("resources.csv")
 
     return data
 
 
-def listRecourceIDs(cookies):
+def listResourceIDs(cookies):
     """
     Create a list of the IDs of all resources in any
     provider that you might administer
 
     Args:
         cookies: cookie used for the request
 
     Returns:
-        list of list of the IDs of all resources in any
+        list of the IDs of all resources in any
     provider that you might administer
     """
 
     # Request all resources dataframe and cast Resource id
     # column to list
     return getAllResources(cookies)["ResourceId"].tolist()
 
 
-def getResourceStatistics(cookies, resources=[], start="2021-03-07", end="2022-03-07"):
+def getResourceStatistics(cookies, resources, start="2021-03-07", end="2022-03-07"):
     """
     Download all resource usage statistics from Statistics
     page
 
     Args:
         cookies: cookie used for the request
         resources: list of resources to include in request
@@ -222,15 +222,15 @@
         Dataframe of statistics table
     """
 
     # If resources is empty
     if not resources:
 
         # Select all resources
-        resources = listRecourceIDs(cookies)
+        resources = listResourceIDs(cookies)
 
     # Set up request url
     url = "https://iris.science-it.ch/statistics/queryResourcesUtilization"
 
     # Get data in raw form
     raw_data = requests.post(
         url,
@@ -244,15 +244,15 @@
         cookies=cookies,
     )
 
     # Return formatted data
     return data_from_raw(raw_data.content, data_field=False)
 
 
-def getHeatmapData(cookies, resources=[], start="2021-03-07", end="2022-03-07"):
+def getHeatmapData(cookies, resources, start="2021-03-07", end="2022-03-07"):
     """
     Download all resource usage statistics from Statistics
     page in heatmap from
 
     Args:
         cookies: cookie used for the request
         resources: list of resources to include in request
@@ -263,30 +263,30 @@
         Dataframe of statistics table
     """
 
     # If resources is empty
     if not resources:
 
         # Select all resources
-        resources = listRecourceIDs(cookies)
+        resources = listResourceIDs(cookies)
 
     # Set up request url
     url = "https://iris.science-it.ch/statistics/queryHeatmapData"
 
     # Get data in raw form
     raw_data = requests.post(
         url, params={"resources": resources, "from": start, "to": end}, cookies=cookies
     )
 
     # Return formatted data
     return data_from_raw(raw_data.content, data_field=False)
 
 
 def getTotalsReportData(
-    cookies, resources=[], start="2021-03-07", end="2022-03-07", mode="user"
+    cookies, resources, start="2021-03-07", end="2022-03-07", mode="user"
 ):
     """
     Download all resource usage statistics from Statistics
     page using the usage total option
 
     Args:
         cookies: cookie used for the request
@@ -298,15 +298,15 @@
         Dataframe of statistics table
     """
 
     # If resources is empty
     if not resources:
 
         # Select all resources
-        resources = listRecourceIDs(cookies)
+        resources = listResourceIDs(cookies)
 
     # Set up request url
     url = "https://iris.science-it.ch/statistics/queryTotalsReportData"
 
     # Get data in raw form
     raw_data = requests.post(
         url,
@@ -315,56 +315,57 @@
     )
 
     # Return formatted data
     return data_from_raw(raw_data.content, data_field="OrganizationItems")
 
 
 def getResourceUsageByUser(
-    cookies, resources=[], start="2021-03-07", end="2022-03-07", mode="scheduled"
+    cookies, resources, start="2021-03-07", end="2022-03-07", mode="scheduled"
 ):
     """
     Download resource usage by user statistics from Statistics
     page
 
     Args:
         cookies: cookie used for the request
         resources: list of resources to include in request
         start: start date to filter results
         end: end date to filter results
+        mode: query mode parameter
 
     Returns:
         Dataframe of statistics table
     """
 
     # If resources is empty
     if not resources:
 
         # Select all resources
-        resources = listRecourceIDs(cookies)
+        resources = listResourceIDs(cookies)
 
     # Set up request url
     url = "https://iris.science-it.ch/statistics/queryResourceUsageByUser"
 
     # Get data in raw form
     raw_data = requests.post(
         url,
         params={"resources": resources, "from": start, "to": end, "mode": mode},
         cookies=cookies,
     )
     return data_from_raw(raw_data.content, data_field="Items")
 
 
-def getResourceTypes(cookies, providers=[]):
+def getResourceTypes(cookies, providers):
     """
     Get a dataframe with all resource types that
     appear in resource linked to your providers
 
     Args:
         cookies: cookie used for the request
-        resources: list of resources to include in request
+        providers: list of providers to include in request
 
     Returns:
         Dataframe of statistics table
     """
 
     # If resources list is empty
     if not providers:
@@ -463,15 +464,15 @@
         start: start date to filter results
         end: end date to filter results
         providerId: the provider concerned
         groupId: group concerned
         showByGroup: pagination selection
         includeTraining: include users that have been trained on your resources
         includeResourceAccess: include users that have access to at least one resource
-        includeProvdierAccess: include users that ha acess to your provider
+        includeProviderAccess: include users that have access to your provider
 
     Returns:
         Dataframe of resources that are visible
     """
 
     # Set up request url
     url = "https://openiris.io/admin-users?"
@@ -514,17 +515,18 @@
     Args:
         cookies: cookie used for the request
         start: start date to filter results
         end: end date to filter results
         providerId: the provider concerned
         includeUsers: group concerned
         includeGroupAdmins: pagination selection
-        includeGroupHeads: include users that have been trained on your resources
+        includeGroupHeads: include the group heads
+        includeTrainings: include users that have been trained on your resources
         includeResourceAccess: include users that have access to at least one resource
-        includeProvdierAccess: include users that ha acess to your provider
+        includeProviderAccess: include users that have access to your provider
 
     Returns:
         Dataframe of resources that are visible
     """
 
     # Set up request url
     url = "https://openiris.io/admin-users/distribution"
@@ -545,7 +547,210 @@
             "includeResourceAccess": includeResourceAccess,
             "includeProviderAccess": includeProviderAccess,
         },
         cookies=cookies,
     )
 
     return data_from_raw(raw_data.content, data_field="DistributionList")
+
+
+def createGroup(cookies,
+                name,
+                shortName,
+                contactEmail,
+                organization,
+                isADIntegrated="false",
+                adGroupName="",
+                autoApprove="false",
+                groupHead="",
+                admins="",
+                members="",
+                emailsEnabled="false",
+                orgTypeId="",
+                validate="true",
+                ):
+    """
+      Creates a group
+
+      Args:
+          cookies: cookie used for the request
+          name: group name
+          shortName: group short name,
+          contactEmail: contact email for group,
+          organization: organization ID to affiliate the group to,
+          isADIntegrated: boolean for AD integration
+          adGroupName: AD integration group name
+          autoApprove: auto approve boolean
+          groupHead: group head user ID
+          admins: list of administrators
+          members: list of members
+          emailsEnabled: emails enabled boolean
+          orgTypeId: type of organization ID
+          validate: validate group boolean
+
+      Returns:
+          a json instance with Status:Ok and the newly created Group ID
+    """
+
+    # Verify if org id is string or integer
+    if not isinstance(organization, str):
+        organization = str(organization)
+
+    # Set up request url
+    url = "https://openiris.io/groups/create"
+
+    # Get data in raw form
+    raw_data = requests.post(
+        url,
+        params={
+            "name": name,
+            "shortName": shortName,
+            "contactEmail": contactEmail,
+            "organization": organization,
+            "isADIntegrated": isADIntegrated,
+            "adGroupName": adGroupName,
+            "autoApprove": autoApprove,
+            "groupHead": groupHead,
+            "admins": admins,
+            "members": members,
+            "emailsEnabled": emailsEnabled,
+            "orgTypeId": orgTypeId,
+            "validate": validate,
+        },
+        cookies=cookies,
+    )
+
+
+
+
+def updateGroup(cookies,
+                id,
+                name,
+                shortName,
+                contactEmail,
+                organizationName,
+                organizationId,
+                affiliatedDepartment,
+                isADIntegrated="false",
+                adGroupName="",
+                autoApprove="false",
+                groupHead="",
+                orgTypeId="",
+                allowDifferentOrganizations="false",
+                linkUrl="",
+                nickname="",
+                isOrgAdmin="false",
+                isInactive="false",
+                isInactiveShowToAdmins="false",
+                ):
+
+    """
+      Updates a group
+
+      Args:
+          cookies: cookie used for the request
+          id: id of the group
+          name: group name
+          shortName: group short name,
+          contactEmail: contact email for group,
+          organizationName: organization Name,
+          organizationId: organization ID,
+          affiliatedDepartment: id of affiliated department,
+          isADIntegrated: boolean for AD integration
+          adGroupName: AD integration group name
+          autoApprove: auto approve boolean
+          groupHead: group head user ID
+          orgTypeId: type of organization ID
+          allowDifferentOrganizations: boolean to allow users from outside org
+          linkUrl url to group page
+          nickname: group nickname string
+          isOrgAdmin: is the requester org admin boolean
+          isInactive: is the group inactive boolean
+          isInactiveShowToAdmins: show to admin if inactive
+
+      Returns:
+          a json instance with Status:Ok if successful
+    """
+
+    # Set up request url
+    url = "https://openiris.io/groups/edit"
+
+    # Get data in raw form
+    raw_data = requests.post(
+        url,
+        params={
+            "id": id,
+            "name": name,
+            "shortName": shortName,
+            "contactEmail": contactEmail,
+            "organizationName": organizationName,
+            "organizationId": organizationId,
+            "affiliatedDepartment": affiliatedDepartment,
+            "isADIntegrated": isADIntegrated,
+            "adGroupName": adGroupName,
+            "autoApprove": autoApprove,
+            "groupHead": groupHead,
+            "orgTypeId": orgTypeId,
+            "allowDifferentOrganizations": allowDifferentOrganizations,
+            "linkUrl": linkUrl,
+            "nickname": nickname,
+            "isOrgAdmin": isOrgAdmin,
+            "isInactive": isInactive,
+            "isInactiveShowToAdmins": isInactiveShowToAdmins,
+        },
+        cookies=cookies,
+    )
+
+    status = data_from_raw(raw_data.content, data_field="Status")
+    if status == "OK":
+        return True
+    else:
+        return False
+
+
+def deleteGroups(cookies, groupId):
+    """
+    Deletes a group
+
+       Args:
+              cookies: cookie used for the request
+              groupId: groupId to delete
+
+        Returns:
+              a json instance with Status:"OK" if successful
+    """
+
+    # Set up request url
+    url = "https://openiris.io/groups/delete"
+
+    # Get data in raw form
+    raw_data = requests.post(url, params={"groupId": groupId}, cookies=cookies)
+
+    status = data_from_raw(raw_data.content, data_field="Status")
+    if status == "OK":
+        return True
+    else:
+        return False
+
+
+def addAdmin(cookies, groupId, userId):
+    """
+    Adds admin to a group
+
+       Args:
+              cookies: cookie used for the request
+              groupId: groupId to delete
+              userId: user to add as admin
+
+        Returns:
+              a json instance with Status:"OK" if successful
+    """
+
+    url = 'https://openiris.io/groups/addadmin'
+
+    raw_data = requests.post(url, params={'groupId': groupId, 'userId': userId}, cookies=cookies)
+
+    return raw_data.content
+
+
+
+
```

### Comparing `openirisapi-0.0.2/openirisapi/utilities.py` & `openirisapi-0.0.3/openirisapi/utilities.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Simple utility module used for the OpenIrisAPI
 
 Author: Sotiris Papadiamantis
 """
 import pandas as pd
 import json
 import ast
+import requests
+
 
 
 def data_from_raw(data, data_field=" "):
     """
     Simple data extraction function from request response
 
     Args:
@@ -23,14 +25,25 @@
     if data_field == " ":
         return pd.DataFrame.from_dict(json.loads(dict_str))
     elif data_field == "Data":
         return pd.DataFrame.from_dict(json.loads(dict_str)["Data"])
     else:
         return pd.DataFrame.from_dict(json.loads(dict_str)[data_field])
 
+def get_cookie_from_login(email='',password=''):
+
+    # Set up request url
+    url = "https://openiris.io/account/login"
+    session = requests.Session()
+    raw_data = session.post(url,params={
+        "email": email,
+        "password": password}
+        )
+
+    return session.cookies.get_dict()
 
 def get_cookie(filepath="cookie.txt"):
     """
     Read cookie stored in filepath
 
     Args:
         filepath: filepath of txt file storing login cookie
```

### Comparing `openirisapi-0.0.2/openirisapi.egg-info/PKG-INFO` & `openirisapi-0.0.3/openirisapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openirisapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very basic API built upon requests for openiris.io
 Home-page: https://gitlab.in2p3.fr/sotirios.PAPADIAMANTIS/openirisAPI
 Author: Sotiris Papadiamantis
 Author-email: sotirios.papadiamantis@univ-amu.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ## OpenIRIS API
 
+[![Downloads](https://static.pepy.tech/badge/openirisapi/month)](https://pepy.tech/project/openirisapi)
+
 A simple API for [openiris.io](openiris.io). OpenIRIS is a free platform permitting the publishing and management of resources form microscopy units.
 
 This API was developped as part of a France BioImaging project and is offered for use to anyone in the scientific community.
 
 At the moment, there is no REST API published by the site's developpers. This package aims to provide a functional solution that permits PROVIDER ardministration to download data directly from the website's backend.
 
 To get your cookie you have to use the Dev tools of your browser, Network > Cookie script > Cookie. You must then format it into a python dictionary and store it in a .txt file.
```

### Comparing `openirisapi-0.0.2/setup.cfg` & `openirisapi-0.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 7065 6e69 7269 7361 7069 0d0a   = openirisapi..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 320d  version = 0.0.2.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 330d  version = 0.0.3.
 00000030: 0a61 7574 686f 7220 3d20 536f 7469 7269  .author = Sotiri
 00000040: 7320 5061 7061 6469 616d 616e 7469 730d  s Papadiamantis.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 736f 7469 7269 6f73 2e70 6170 6164 6961  sotirios.papadia
 00000070: 6d61 6e74 6973 4075 6e69 762d 616d 752e  mantis@univ-amu.
 00000080: 6672 0d0a 6465 7363 7269 7074 696f 6e20  fr..description 
 00000090: 3d20 4120 7665 7279 2062 6173 6963 2041  = A very basic A
```

