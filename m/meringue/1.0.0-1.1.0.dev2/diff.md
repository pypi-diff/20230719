# Comparing `tmp/meringue-1.0.0.tar.gz` & `tmp/meringue-1.1.0.dev2.tar.gz`

## Comparing `meringue-1.0.0.tar` & `meringue-1.1.0.dev2.tar`

### file list

```diff
@@ -1,24 +1,29 @@
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/__init__.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/conf/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/apps.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/managers.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/options.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 meringue-1.0.0/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.0.0/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.0.0/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.0.0/LICENSE
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 meringue-1.0.0/README.md
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 meringue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 meringue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/handlers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/utils.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/README.md
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/PKG-INFO
```

### Comparing `meringue-1.0.0/meringue/conf/__init__.py` & `meringue-1.1.0.dev2/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/meringue/core/models.py` & `meringue-1.1.0.dev2/meringue/core/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+# ruff: noqa: RUF012
+
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from meringue.core.managers import PublicationDatesManager
-from meringue.core.managers import PublicationManager
-from meringue.core.managers import SortingManager
+from meringue.core.query import UniversalQuerySet
 
 
 class CMTimeMixin(models.Model):
     """
     A simple mixin to add _ctime_ and _mtime_ fields.
     """
 
@@ -25,15 +25,15 @@
 
     sorting = models.SmallIntegerField(
         verbose_name=_("Sorting"),
         help_text=_("Sorting order."),
         default=0,
     )
 
-    objects = SortingManager()
+    objects = UniversalQuerySet.as_manager()
 
     class Meta:
         ordering = [
             "sorting",
         ]
         abstract = True
 
@@ -50,15 +50,15 @@
     is_published = models.BooleanField(
         verbose_name=_("Publication"),
         help_text=_("Show/Hide"),
         default=True,
         db_index=True,
     )
 
-    objects = PublicationManager()
+    objects = UniversalQuerySet.as_manager()
 
     class Meta:
         abstract = True
 
 
 class PublicationDatesMixin(models.Model):
     """
@@ -78,11 +78,11 @@
     date_to = models.DateTimeField(
         verbose_name=_("Date to"),
         help_text=_("Date and time when to hide."),
         blank=True,
         null=True,
     )
 
-    objects = PublicationDatesManager()
+    objects = UniversalQuerySet.as_manager()
 
     class Meta:
         abstract = True
```

### Comparing `meringue-1.0.0/meringue/core/query.py` & `meringue-1.1.0.dev2/meringue/core/query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from django.db.models import Q
 from django.db.models.query import QuerySet
 from django.utils import timezone
 
 
 class SortingQuerySet(QuerySet):
+    """
+    QuerySet with methods for working with sorted positions
+    """
+
     def correction_sorting(self):
         """
         This is a method to update/fix the sorting of the selected list of items.
 
         The sorting will be done according to the `queryset` sorting, so sorting can be controlled
         by executing `.order_by()` before calling the `correction_sorting` method.
 
@@ -21,44 +25,54 @@
                 items.append(item)
             sorting += 1
 
         return self.bulk_update(items, ["sorting"])
 
 
 class PublicationQuerySet(QuerySet):
+    """
+    QuerySet with methods for fetching published and unpublished elements.
+    """
+
     def published(self, *args, **kwargs):
         """
         Method to getting published items.
         """
-        kwargs["is_published"] = True
-        return self.filter(*args, **kwargs)
+        from meringue.core.models import PublicationDatesMixin
+        from meringue.core.models import PublicationMixin
 
-    def unpublished(self, *args, **kwargs):
-        """
-        Method for getting unpublished items.
-        """
-        kwargs["is_published"] = False
-        return self.filter(*args, **kwargs)
+        if issubclass(self.model, PublicationMixin):
+            kwargs["is_published"] = True
 
+        if issubclass(self.model, PublicationDatesMixin):
+            now = timezone.now()
+            args = (
+                *args,
+                Q(date_from__lte=now, date_to__gt=now)
+                | Q(date_from__isnull=True, date_to__gt=now)
+                | Q(date_from__lte=now, date_to__isnull=True)
+                | Q(date_from__isnull=True, date_to__isnull=True),
+            )
 
-class PublicationDatesQuerySet(QuerySet):
-    def published(self, *args, **kwargs):
-        """
-        Method to getting published items.
-        """
-        now = timezone.localtime()
-        args = (
-            *args,
-            Q(date_from__lte=now, date_to__gt=now)
-            | Q(date_from__isnull=True, date_to__gt=now)
-            | Q(date_from__lte=now, date_to__isnull=True)
-            | Q(date_from__isnull=True, date_to__isnull=True),
-        )
         return self.filter(*args, **kwargs)
 
     def unpublished(self, *args, **kwargs):
         """
         Method for getting unpublished items.
         """
-        now = timezone.localtime()
-        args = (*args, Q(date_from__gt=now) | Q(date_to__lte=now))
+        from meringue.core.models import PublicationDatesMixin
+        from meringue.core.models import PublicationMixin
+
+        if issubclass(self.model, PublicationMixin):
+            kwargs["is_published"] = False
+
+        if issubclass(self.model, PublicationDatesMixin):
+            now = timezone.now()
+            args = (*args, Q(date_from__gt=now) | Q(date_to__lte=now))
+
         return self.filter(*args, **kwargs)
+
+
+class UniversalQuerySet(SortingQuerySet, PublicationQuerySet):
+    """
+    Generic QuerySet containing methods of all other QuerySets
+    """
```

### Comparing `meringue-1.0.0/meringue/core/translation.py` & `meringue-1.1.0.dev2/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/meringue/core/upload_handlers.py` & `meringue-1.1.0.dev2/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.1.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.1.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/meringue/core/templatetags/meringue_base.py` & `meringue-1.1.0.dev2/meringue/core/templatetags/meringue_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 register = template.Library()
 
 
 @register.simple_tag
 def cop_year() -> str:
     """
-    A tag that displays the year or range of years for the copyright string in YYYY-YYYY format.
+    A tag that displays the year or range of years for the copyright string in `YYYY-YYYY` format.
 
     For the tag to work, you must fill in the `COP_YEAR` parameter in the settings.
 
     Examples:
         ```jinja
         <p>Copyright © {% cop_year %} My company</p>
         ```
@@ -45,19 +45,20 @@
 
     return mark_safe(f"{m_settings.COP_YEAR}&mdash;{year}")  # noqa: S308
 
 
 @register.simple_tag
 def date_range(date_start: dt.date, date_end: dt.date) -> str:
     """
-    return range of date in one of the following formats:
-        DD.MM.YYYY - DD.MM.YYYY
-        DD.MM - DD.MM.YYYY
-        DD - DD.MM.YYYY
-        DD.MM.YYYY
+    Return range of date in one of the following formats:
+
+    * `DD.MM.YYYY - DD.MM.YYYY`
+    * `DD.MM - DD.MM.YYYY`
+    * `DD - DD.MM.YYYY`
+    * `DD.MM.YYYY`
 
     Attributes:
         date_start: Period start date.
         date_end: Period end date.
 
     Examples:
         ```jinja
```

### Comparing `meringue-1.0.0/meringue/core/utils/datetime.py` & `meringue-1.1.0.dev2/meringue/core/utils/datetime.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     delimiter: str = "-",
 ) -> str:
     """
     Method to display date period.
 
     Possible output formats depending on the input data:
 
-    * DD.MM.YYYY - DD.MM.YYYY
-    * DD.MM - DD.MM.YYYY
-    * DD - DD.MM.YYYY
-    * DD.MM.YYYY
+    * `DD.MM.YYYY - DD.MM.YYYY`
+    * `DD.MM - DD.MM.YYYY`
+    * `DD - DD.MM.YYYY`
+    * `DD.MM.YYYY`
 
     Examples:
         ```pycon
         >>> print(format_date_from_to(dt.date(2020, 1, 1), dt.date(2020, 2, 1)))
         01.01 - 01.02.2020
         ```
```

### Comparing `meringue-1.0.0/LICENSE` & `meringue-1.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.0.0/README.md` & `meringue-1.1.0.dev2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 	</a>
 	<!-- <a href="https://pypi.org/project/meringue">
 		<img src="https://img.shields.io/pypi/format/meringue.svg" alt="PyPI - Format" />
 	</a> -->
 </p>
 <p align="center">
 	<a href="https://github.com/dd/Meringue/actions/workflows/mkdocs-release.yml" >
-		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=Docs" alt="Documentation - Release" />
+		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=docs" alt="Documentation - Release" />
 	</a>
 	<a href="https://github.com/dd/Meringue/actions/workflows/test.yml" >
-		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=Tests" alt="Tests - Running" />
+		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=tests" alt="Tests - Running" />
 	</a>
 	<a href="https://codecov.io/gh/dd/Meringue" >
 		<img src="https://codecov.io/gh/dd/Meringue/branch/release/1.0.0/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
 	</a>
 </p>
 <p align="center">
 	<a href="https://github.com/pypa/hatch" target="_blank">
@@ -48,42 +48,44 @@
 		<img src="https://img.shields.io/badge/types-Mypy-blue.svg" alt="types - Mypy" />
 	</a> -->
 	<a href="https://raw.githubusercontent.com/dd/Meringue/master/LICENSE" target="_blank">
 		<img src="https://img.shields.io/pypi/l/meringue?color=008033" alt="License - GNU Lesser General Public License v3.0" />
 	</a>
 </p>
 
+Full documentation for the project is available at [dd.github.io/Meringue](https://dd.github.io/Meringue/).
+
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* Universal manager worked with all abstract models
-* Tests of all functionality
-* Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
-* Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
-* [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+* [x] Universal manager worked with all abstract models
+* [x] Tests of all functionality
+* [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
+* [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
+* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
  generating form based on response from api).
-* Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
-* Authorization backend for authorization by a pair of email and password.
-* Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
-* Functionality for working with images.
-	* Image editor like easy_thumbnails.
-	* A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
-* Functionality similar to that described in the previous paragraph only for video.
-* Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* Exception handler for drf that returns an error code in addition to the error text
+* [ ] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
+* [ ] Authorization backend for authorization by a pair of email and password.
+* [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [ ] Functionality for working with images.
+	* [ ] Image editor like easy_thumbnails.
+	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+* [ ] Functionality similar to that described in the previous paragraph only for video.
+* [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
+* [x] Exception handler for drf that returns an error code in addition to the error text
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,50 +1,52 @@
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
-Package with various functional (such as mixins, form utils, upload handlers
-and other) for Django Framework. This library is a set of various functionality
-that I use from project to project. The main task of this package is to clean
-up this functionality, test it, and also organize the documentation so that
-colleagues can understand how and what works. However, if someone decides to
-use this functionality in their project, and even more so to add functionality
-or change the implementation to a more correct, beautiful or understandable
-one, I will only be happy, do not worry and feel free to write to me by [mail]
-(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
-issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
-(https://github.com/dd/Meringue). ## Roadmap Adding new functionality. Can
-change. * Universal manager worked with all abstract models * Tests of all
-functionality * Methods for encrypting and decrypting text content (To create
-various secrets, such as a link to change your password or activate your
-profile). * Functionality for obtaining absolute links to resources presented
-on the front, located on another domain (When working through api) (utils
-methods, template tags and filters). * [drf](https://www.django-rest-
-framework.org/) serializer serializer for automatic form generation on the
-front when working through rest api. (An npm package on [vuejs](https://
-vuejs.org/) will also be developed generating form based on response from api).
-* Extended [drf router](https://www.django-rest-framework.org/api-guide/
-routers/) that allows you to add resources like `/profile` returning the
-profile data of an authorized user without his id. * Authorization backend for
-authorization by a pair of email and password. * Helpers to extend
-documentation generated by [drf-spectacular](https://drf-
-spectacular.readthedocs.io/) - just a small helper to easily add links to
-different deployed environments (production, test, local, etc.) or let's say
-for more digestible tags instead of initially generated ones * Functionality
-for working with images. * Image editor like easy_thumbnails. * A field for the
-drf serializer that returns a set of images (for example, a standard image and
-a double-sized image for a retina screen), as well as in different formats (for
-example, in the original format and in webp). * Functionality similar to that
-described in the previous paragraph only for video. * Functionality for loading
-private files available through [nginx internal](http://nginx.org/en/docs/http/
-ngx_http_core_module.html#internal). * Exception handler for drf that returns
-an error code in addition to the error text ## Contributing - [x] Use Git Flow
-(read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://
-www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
+Full documentation for the project is available at [dd.github.io/Meringue]
+(https://dd.github.io/Meringue/). Package with various functional (such as
+mixins, form utils, upload handlers and other) for Django Framework. This
+library is a set of various functionality that I use from project to project.
+The main task of this package is to clean up this functionality, test it, and
+also organize the documentation so that colleagues can understand how and what
+works. However, if someone decides to use this functionality in their project,
+and even more so to add functionality or change the implementation to a more
+correct, beautiful or understandable one, I will only be happy, do not worry
+and feel free to write to me by [mail](mailto:dd@manin.space), create an
+[issue](https://github.com/dd/Meringue/issues) or [pull request](https://
+github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
+Roadmap Adding new functionality. Can change. * [x] Universal manager worked
+with all abstract models * [x] Tests of all functionality * [x] Methods for
+encrypting and decrypting text content (To create various secrets, such as a
+link to change your password or activate your profile). * [x] Functionality for
+obtaining absolute links to resources presented on the front, located on
+another domain (When working through api) (utils methods, template tags and
+filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
+serializer for automatic form generation on the front when working through rest
+api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+generating form based on response from api). * [ ] Extended [drf router](https:
+//www.django-rest-framework.org/api-guide/routers/) that allows you to add
+resources like `/profile` returning the profile data of an authorized user
+without his id. * [ ] Authorization backend for authorization by a pair of
+email and password. * [ ] Helpers to extend documentation generated by [drf-
+spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
+easily add links to different deployed environments (production, test, local,
+etc.) or let's say for more digestible tags instead of initially generated ones
+* [ ] Functionality for working with images. * [ ] Image editor like
+easy_thumbnails. * [ ] A field for the drf serializer that returns a set of
+images (for example, a standard image and a double-sized image for a retina
+screen), as well as in different formats (for example, in the original format
+and in webp). * [ ] Functionality similar to that described in the previous
+paragraph only for video. * [ ] Functionality for loading private files
+available through [nginx internal](http://nginx.org/en/docs/http/
+ngx_http_core_module.html#internal). * [x] Exception handler for drf that
+returns an error code in addition to the error text ## Contributing - [x] Use
+Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https:
+//www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
 resolve the versioning - [x] Linter with a [Ruff](https://github.com/
 charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
 black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
 [Conventional Commits](https://www.conventionalcommits.org/) - [x]
 Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
 (https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
 (https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
```

### Comparing `meringue-1.0.0/pyproject.toml` & `meringue-1.1.0.dev2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,26 @@
 	"AUTHORS",
 ]
 exclude = [
 	"docs",
 	"hooks",
 	".gitignore",
 	"CHANGELOG.md",
+	"CONTRIBUTING.md",
 	"tests",
 ]
 
 [tool.hatch.envs.default]
 description = "Dev environment"
 python = "3.11"
 dependencies = [
-	"pre-commit==3.3.2",
+	"pre-commit==3.3.3",
+	"ipython==8.14.0",
+	"pycryptodome==3.18.0",
+	"djangorestframework==3.14.0",
 ]
 [tool.hatch.envs.default.scripts]
 precommit_install = "pre-commit install {args}"
 precommit_uninstall = "pre-commit uninstall {args}"
 init = [
 	"git config --local gitflow.branch.master \"master\"",
 	"git config --local gitflow.branch.develop \"dev\"",
@@ -93,86 +97,94 @@
 	"git config --local gitflow.prefix.release \"release/\"",
 	"git config --local gitflow.prefix.hotfix \"hotfix/\"",
 	"git config --local gitflow.prefix.support \"support/\"",
 	"git config --local gitflow.prefix.versiontag \"v\"",
 	"git config --local gitflow.path.hooks $(pwd)\"/.git/hooks\"",
 	"precommit_install",
 ]
-remove = ["precommit_uninstall"]
+remove = [
+	"precommit_uninstall",
+]
 makemessages = [
 	"cd meringue/core && django-admin makemessages -l en -l ru --no-obsolete {args}",
 ]
 compilemessages = "cd meringue && django-admin compilemessages -l en -l ru {args}"
 
 [tool.hatch.envs.lint]
 description = "Lint environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"ruff==0.0.275",
-	"black==23.3.0",
+	"ruff==0.0.278",
+	"black==23.7.0",
 ]
 [tool.hatch.envs.lint.scripts]
 check = [
 	"ruff {args:.}",
 	"black --check --diff --exclude=\".*migrations\\/.*$\" {args:.}",
 ]
 format = [
 	"ruff --fix {args:.}",
-	"black {args:.}",
+	"black --exclude=\".*migrations\\/.*$\" {args:.}",
 ]
 
 [tool.hatch.envs.test]
 description = "Tests environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"pytest==7.3.2",
+	"pytest==7.4.0",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",
-	"Faker==18.11.1",
+	"Faker==19.1.0",
 	"django==4.2",
 	"pytz==2023.3",
-	"django-modeltranslation==0.18.10",
+	"django-modeltranslation==0.18.11",
+	"pycryptodome==3.18.0",
+	"djangorestframework==3.14.0",
 ]
 [tool.hatch.envs.test.env-vars]
 DJANGO_SETTINGS_MODULE = 'test_project.settings'
 PYTHONPATH  = '.'
 [tool.hatch.envs.test.scripts]
 check = "pytest {args:--cov=meringue --cov-report term-missing}"
 makemigrations = "django-admin makemigrations {args}"
 
 [tool.hatch.envs.mtest]
 description = "Test matrix environment"
 detached = true
 dependencies = [
-	"pytest==7.3.2",
+	"pytest==7.4.0",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",  # for ci tests with cover
-	"Faker==18.11.1",
+	"Faker==19.1.0",
 	"pytz==2023.3",
+	"pycryptodome==3.18.0",
 ]
 [tool.hatch.envs.mtest.overrides]
 matrix.django.dependencies = [
 	{ value = "django~={matrix:django}" },
 	{ value = "django-modeltranslation=={matrix:modeltranslation}" },
+	{ value = "djangorestframework=={matrix:djangorestframework}" },
 ]
 [tool.hatch.envs.mtest.env-vars]
 DJANGO_SETTINGS_MODULE = 'test_project.settings'
 PYTHONPATH  = '.'
 [tool.hatch.envs.mtest.scripts]
 check = "pytest {args:-q}"
 [[tool.hatch.envs.mtest.matrix]]
 python = ["3.10", "3.11"]
 django = ["2.0"]
 modeltranslation = ["0.17.7"]
+djangorestframework = ["3.13.1"]
 [[tool.hatch.envs.mtest.matrix]]
 python = ["3.10", "3.11"]
 django = ["3.0", "4.0"]
-modeltranslation = ["0.18.10"]
+modeltranslation = ["0.18.11"]
+djangorestframework = ["3.14.0"]
 
 [tool.hatch.envs.docs]
 description = "Docs environment"
 detached = true
 python = "3.11"
 dependencies = [
 	"mkdocs[i18n]==1.4.3",
@@ -214,15 +226,14 @@
 	"A",
 	"B",
 	"C",
 	"DTZ",
 	"E",
 	"EM",
 	"F",
-	"FBT",
 	"I",
 	"ICN",
 	"ISC",
 	"N",
 	"PLC",
 	"PLE",
 	"PLR",
@@ -237,18 +248,16 @@
 	"W",
 	"YTT",
 ]
 ignore = [
 	"RUF001",  # Allow similar characters like latin `c` and cyrillic `с`
 	"RUF002",  # Allow russian at docstrings
 	"RUF003",  # Allow russian at comment
-	"FBT001",  # Allow boolean args
-	"FBT002",  # Allow boolean positional argument define
-	"FBT003",  # Allow boolean positional values in function calls, like `dict.get(... True)`
 	"PLR0913",  # Allow any number of function arguments
+	"E741",  # Allow variables of like "l", "O",  "i"
 	# # Allow non-abstract empty methods in abstract base classes
 	# "B027",
 	# # Ignore checks for possible passwords
 	# "S105", "S106", "S107",
 	# # Ignore complexity
 	# "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 	# "PLC1901", # empty string comparisons
@@ -257,17 +266,18 @@
 ]
 # unfixable = [
 # 	# Don't touch unused imports
 # 	"F401",
 # ]
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401", "F403"]
-"test_*.py" = ["S101", "PLR2004"]
+"test_*.py" = ["S101", "PLR2004", "DTZ001"]
 "*/migrations/*" = ["I", "E", "Q", "RUF"]
 "test_project/*models.py" = ["RUF012"]
+"test_project/*views.py" = ["RUF012"]
 [tool.ruff.flake8-import-conventions]
 [tool.ruff.flake8-import-conventions.extend-aliases]
 "datetime" = "dt"
 # [tool.ruff.flake8-quotes]
 # inline-quotes = "single"
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
```

### Comparing `meringue-1.0.0/PKG-INFO` & `meringue-1.1.0.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.0.0
+Version: 1.1.0.dev2
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
@@ -69,18 +69,18 @@
 	</a>
 	<!-- <a href="https://pypi.org/project/meringue">
 		<img src="https://img.shields.io/pypi/format/meringue.svg" alt="PyPI - Format" />
 	</a> -->
 </p>
 <p align="center">
 	<a href="https://github.com/dd/Meringue/actions/workflows/mkdocs-release.yml" >
-		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=Docs" alt="Documentation - Release" />
+		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=docs" alt="Documentation - Release" />
 	</a>
 	<a href="https://github.com/dd/Meringue/actions/workflows/test.yml" >
-		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=Tests" alt="Tests - Running" />
+		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=tests" alt="Tests - Running" />
 	</a>
 	<a href="https://codecov.io/gh/dd/Meringue" >
 		<img src="https://codecov.io/gh/dd/Meringue/branch/release/1.0.0/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
 	</a>
 </p>
 <p align="center">
 	<a href="https://github.com/pypa/hatch" target="_blank">
@@ -99,42 +99,44 @@
 		<img src="https://img.shields.io/badge/types-Mypy-blue.svg" alt="types - Mypy" />
 	</a> -->
 	<a href="https://raw.githubusercontent.com/dd/Meringue/master/LICENSE" target="_blank">
 		<img src="https://img.shields.io/pypi/l/meringue?color=008033" alt="License - GNU Lesser General Public License v3.0" />
 	</a>
 </p>
 
+Full documentation for the project is available at [dd.github.io/Meringue](https://dd.github.io/Meringue/).
+
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* Universal manager worked with all abstract models
-* Tests of all functionality
-* Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
-* Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
-* [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+* [x] Universal manager worked with all abstract models
+* [x] Tests of all functionality
+* [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
+* [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
+* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
  generating form based on response from api).
-* Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
-* Authorization backend for authorization by a pair of email and password.
-* Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
-* Functionality for working with images.
-	* Image editor like easy_thumbnails.
-	* A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
-* Functionality similar to that described in the previous paragraph only for video.
-* Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* Exception handler for drf that returns an error code in addition to the error text
+* [ ] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
+* [ ] Authorization backend for authorization by a pair of email and password.
+* [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [ ] Functionality for working with images.
+	* [ ] Image editor like easy_thumbnails.
+	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+* [ ] Functionality similar to that described in the previous paragraph only for video.
+* [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
+* [x] Exception handler for drf that returns an error code in addition to the error text
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.0.0 Summary: A set of various
-functionality for a Django based web application. Project-URL: Homepage, https:
-//github.com/dd/Meringue Project-URL: Documentation, https://dd.github.io/
-Meringue/ Project-URL: Repository, https://github.com/dd/Meringue Project-URL:
-Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md Project-URL:
-Bug Tracker, https://github.com/dd/Meringue/issues Author-email: Dmitry
-Dobrynin
+Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev2 Summary: A set of
+various functionality for a Django based web application. Project-URL:
+Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
+dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
+Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
+Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
 LICENSE Keywords: django,utils Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Plugins Classifier: Environment ::
 Web Environment Classifier: Framework :: Django Classifier: Framework :: Django
 :: 1 Classifier: Framework :: Django :: 1.11 Classifier: Framework :: Django ::
 2 Classifier: Framework :: Django :: 2.0 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3
@@ -29,52 +29,54 @@
 Development :: Libraries Requires-Python: >=3.10 Requires-Dist: django>=1.11.17
 Description-Content-Type: text/markdown
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
-Package with various functional (such as mixins, form utils, upload handlers
-and other) for Django Framework. This library is a set of various functionality
-that I use from project to project. The main task of this package is to clean
-up this functionality, test it, and also organize the documentation so that
-colleagues can understand how and what works. However, if someone decides to
-use this functionality in their project, and even more so to add functionality
-or change the implementation to a more correct, beautiful or understandable
-one, I will only be happy, do not worry and feel free to write to me by [mail]
-(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
-issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
-(https://github.com/dd/Meringue). ## Roadmap Adding new functionality. Can
-change. * Universal manager worked with all abstract models * Tests of all
-functionality * Methods for encrypting and decrypting text content (To create
-various secrets, such as a link to change your password or activate your
-profile). * Functionality for obtaining absolute links to resources presented
-on the front, located on another domain (When working through api) (utils
-methods, template tags and filters). * [drf](https://www.django-rest-
-framework.org/) serializer serializer for automatic form generation on the
-front when working through rest api. (An npm package on [vuejs](https://
-vuejs.org/) will also be developed generating form based on response from api).
-* Extended [drf router](https://www.django-rest-framework.org/api-guide/
-routers/) that allows you to add resources like `/profile` returning the
-profile data of an authorized user without his id. * Authorization backend for
-authorization by a pair of email and password. * Helpers to extend
-documentation generated by [drf-spectacular](https://drf-
-spectacular.readthedocs.io/) - just a small helper to easily add links to
-different deployed environments (production, test, local, etc.) or let's say
-for more digestible tags instead of initially generated ones * Functionality
-for working with images. * Image editor like easy_thumbnails. * A field for the
-drf serializer that returns a set of images (for example, a standard image and
-a double-sized image for a retina screen), as well as in different formats (for
-example, in the original format and in webp). * Functionality similar to that
-described in the previous paragraph only for video. * Functionality for loading
-private files available through [nginx internal](http://nginx.org/en/docs/http/
-ngx_http_core_module.html#internal). * Exception handler for drf that returns
-an error code in addition to the error text ## Contributing - [x] Use Git Flow
-(read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://
-www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
+Full documentation for the project is available at [dd.github.io/Meringue]
+(https://dd.github.io/Meringue/). Package with various functional (such as
+mixins, form utils, upload handlers and other) for Django Framework. This
+library is a set of various functionality that I use from project to project.
+The main task of this package is to clean up this functionality, test it, and
+also organize the documentation so that colleagues can understand how and what
+works. However, if someone decides to use this functionality in their project,
+and even more so to add functionality or change the implementation to a more
+correct, beautiful or understandable one, I will only be happy, do not worry
+and feel free to write to me by [mail](mailto:dd@manin.space), create an
+[issue](https://github.com/dd/Meringue/issues) or [pull request](https://
+github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
+Roadmap Adding new functionality. Can change. * [x] Universal manager worked
+with all abstract models * [x] Tests of all functionality * [x] Methods for
+encrypting and decrypting text content (To create various secrets, such as a
+link to change your password or activate your profile). * [x] Functionality for
+obtaining absolute links to resources presented on the front, located on
+another domain (When working through api) (utils methods, template tags and
+filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
+serializer for automatic form generation on the front when working through rest
+api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+generating form based on response from api). * [ ] Extended [drf router](https:
+//www.django-rest-framework.org/api-guide/routers/) that allows you to add
+resources like `/profile` returning the profile data of an authorized user
+without his id. * [ ] Authorization backend for authorization by a pair of
+email and password. * [ ] Helpers to extend documentation generated by [drf-
+spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
+easily add links to different deployed environments (production, test, local,
+etc.) or let's say for more digestible tags instead of initially generated ones
+* [ ] Functionality for working with images. * [ ] Image editor like
+easy_thumbnails. * [ ] A field for the drf serializer that returns a set of
+images (for example, a standard image and a double-sized image for a retina
+screen), as well as in different formats (for example, in the original format
+and in webp). * [ ] Functionality similar to that described in the previous
+paragraph only for video. * [ ] Functionality for loading private files
+available through [nginx internal](http://nginx.org/en/docs/http/
+ngx_http_core_module.html#internal). * [x] Exception handler for drf that
+returns an error code in addition to the error text ## Contributing - [x] Use
+Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https:
+//www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
 resolve the versioning - [x] Linter with a [Ruff](https://github.com/
 charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
 black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
 [Conventional Commits](https://www.conventionalcommits.org/) - [x]
 Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
 (https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
 (https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
```

