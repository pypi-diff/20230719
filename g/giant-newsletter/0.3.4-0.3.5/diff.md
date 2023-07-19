# Comparing `tmp/giant_newsletter-0.3.4.tar.gz` & `tmp/giant_newsletter-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_newsletter-0.3.4.tar", max compression
+gzip compressed data, was "giant_newsletter-0.3.5.tar", max compression
```

## Comparing `giant_newsletter-0.3.4.tar` & `giant_newsletter-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1069 2022-12-07 11:32:17.376691 giant_newsletter-0.3.4/LICENSE
--rw-r--r--   0        0        0     1667 2022-12-07 11:32:17.376691 giant_newsletter-0.3.4/README.md
--rw-r--r--   0        0        0       22 2022-12-07 12:16:40.289896 giant_newsletter-0.3.4/newsletter/__init__.py
--rw-r--r--   0        0        0     1064 2022-12-07 12:16:40.313229 giant_newsletter-0.3.4/newsletter/admin.py
--rw-r--r--   0        0        0       95 2022-12-07 12:16:40.313229 giant_newsletter-0.3.4/newsletter/apps.py
--rw-r--r--   0        0        0      437 2022-12-07 12:16:40.316562 giant_newsletter-0.3.4/newsletter/cms_apps.py
--rw-r--r--   0        0        0      826 2022-12-07 12:16:40.316562 giant_newsletter-0.3.4/newsletter/cms_plugins.py
--rw-r--r--   0        0        0      123 2022-12-07 12:16:40.319896 giant_newsletter-0.3.4/newsletter/context_processors.py
--rw-r--r--   0        0        0     1222 2022-12-07 12:16:40.319896 giant_newsletter-0.3.4/newsletter/forms.py
--rw-r--r--   0        0        0     1283 2022-12-07 12:16:40.323229 giant_newsletter-0.3.4/newsletter/migrations/0001_initial.py
--rw-r--r--   0        0        0      724 2022-12-07 12:16:40.323229 giant_newsletter-0.3.4/newsletter/migrations/0002_auto_20200623_1442.py
--rw-r--r--   0        0        0      529 2022-12-07 12:16:40.326562 giant_newsletter-0.3.4/newsletter/migrations/0003_auto_20200916_0730.py
--rw-r--r--   0        0        0      573 2022-12-07 12:16:40.326562 giant_newsletter-0.3.4/newsletter/migrations/0004_add_climatecare_fields.py
--rw-r--r--   0        0        0        0 2022-12-07 12:16:40.326562 giant_newsletter-0.3.4/newsletter/migrations/__init__.py
--rw-r--r--   0        0        0      706 2022-12-07 12:16:40.329896 giant_newsletter-0.3.4/newsletter/models.py
--rw-r--r--   0        0        0        0 2022-12-07 12:16:40.333229 giant_newsletter-0.3.4/newsletter/templates/base.html
--rw-r--r--   0        0        0       64 2022-12-07 12:16:40.333229 giant_newsletter-0.3.4/newsletter/templates/newsletter/index.html
--rw-r--r--   0        0        0      393 2022-12-07 12:16:40.333229 giant_newsletter-0.3.4/newsletter/templates/newsletter/plugin.html
--rw-r--r--   0        0        0        0 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/__init__.py
--rw-r--r--   0        0        0      196 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/conftest.py
--rw-r--r--   0        0        0      305 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/test_cms_apps.py
--rw-r--r--   0        0        0      285 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/test_models.py
--rw-r--r--   0        0        0      892 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/test_views.py
--rw-r--r--   0        0        0      162 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/tests/urls.py
--rw-r--r--   0        0        0      135 2022-12-07 12:16:40.336562 giant_newsletter-0.3.4/newsletter/urls.py
--rw-r--r--   0        0        0      760 2022-12-07 12:16:40.339896 giant_newsletter-0.3.4/newsletter/views.py
--rw-r--r--   0        0        0     1122 2022-12-07 12:18:31.329890 giant_newsletter-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 giant_newsletter-0.3.4/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 giant_newsletter-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-19 14:28:11.401804 giant_newsletter-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1667 2023-07-19 14:28:11.401865 giant_newsletter-0.3.5/README.md
+-rw-r--r--   0        0        0       22 2023-07-19 14:28:11.402002 giant_newsletter-0.3.5/newsletter/__init__.py
+-rw-r--r--   0        0        0     1064 2023-07-19 14:28:11.402066 giant_newsletter-0.3.5/newsletter/admin.py
+-rw-r--r--   0        0        0       95 2023-07-19 14:28:11.402115 giant_newsletter-0.3.5/newsletter/apps.py
+-rw-r--r--   0        0        0      437 2023-07-19 14:28:11.402167 giant_newsletter-0.3.5/newsletter/cms_apps.py
+-rw-r--r--   0        0        0      826 2023-07-19 14:28:11.402221 giant_newsletter-0.3.5/newsletter/cms_plugins.py
+-rw-r--r--   0        0        0      123 2023-07-19 14:28:11.402276 giant_newsletter-0.3.5/newsletter/context_processors.py
+-rw-r--r--   0        0        0     1222 2023-07-19 14:28:11.402337 giant_newsletter-0.3.5/newsletter/forms.py
+-rw-r--r--   0        0        0     1283 2023-07-19 14:28:11.402438 giant_newsletter-0.3.5/newsletter/migrations/0001_initial.py
+-rw-r--r--   0        0        0      724 2023-07-19 14:28:11.402505 giant_newsletter-0.3.5/newsletter/migrations/0002_auto_20200623_1442.py
+-rw-r--r--   0        0        0      529 2023-07-19 14:28:11.402561 giant_newsletter-0.3.5/newsletter/migrations/0003_auto_20200916_0730.py
+-rw-r--r--   0        0        0      573 2023-07-19 14:28:11.402612 giant_newsletter-0.3.5/newsletter/migrations/0004_add_climatecare_fields.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:28:11.402633 giant_newsletter-0.3.5/newsletter/migrations/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-19 14:28:11.402708 giant_newsletter-0.3.5/newsletter/models.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:28:11.402767 giant_newsletter-0.3.5/newsletter/templates/base.html
+-rw-r--r--   0        0        0      105 2023-07-19 14:28:11.402881 giant_newsletter-0.3.5/newsletter/templates/newsletter/index.html
+-rw-r--r--   0        0        0      283 2023-07-19 14:32:52.630373 giant_newsletter-0.3.5/newsletter/templates/newsletter/plugin.html
+-rw-r--r--   0        0        0        0 2023-07-19 14:28:11.403008 giant_newsletter-0.3.5/newsletter/tests/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-19 14:28:11.403088 giant_newsletter-0.3.5/newsletter/tests/conftest.py
+-rw-r--r--   0        0        0      305 2023-07-19 14:28:11.403164 giant_newsletter-0.3.5/newsletter/tests/test_cms_apps.py
+-rw-r--r--   0        0        0      285 2023-07-19 14:28:11.403239 giant_newsletter-0.3.5/newsletter/tests/test_models.py
+-rw-r--r--   0        0        0      892 2023-07-19 14:28:11.403303 giant_newsletter-0.3.5/newsletter/tests/test_views.py
+-rw-r--r--   0        0        0      162 2023-07-19 14:28:11.403366 giant_newsletter-0.3.5/newsletter/tests/urls.py
+-rw-r--r--   0        0        0      135 2023-07-19 14:28:11.403435 giant_newsletter-0.3.5/newsletter/urls.py
+-rw-r--r--   0        0        0      826 2023-07-19 14:32:52.630647 giant_newsletter-0.3.5/newsletter/views.py
+-rw-r--r--   0        0        0     1095 2023-07-19 14:32:52.630895 giant_newsletter-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 giant_newsletter-0.3.5/PKG-INFO
```

### Comparing `giant_newsletter-0.3.4/LICENSE` & `giant_newsletter-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/README.md` & `giant_newsletter-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/admin.py` & `giant_newsletter-0.3.5/newsletter/admin.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/cms_plugins.py` & `giant_newsletter-0.3.5/newsletter/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/forms.py` & `giant_newsletter-0.3.5/newsletter/forms.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/migrations/0001_initial.py` & `giant_newsletter-0.3.5/newsletter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/migrations/0002_auto_20200623_1442.py` & `giant_newsletter-0.3.5/newsletter/migrations/0002_auto_20200623_1442.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/migrations/0003_auto_20200916_0730.py` & `giant_newsletter-0.3.5/newsletter/migrations/0003_auto_20200916_0730.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/migrations/0004_add_climatecare_fields.py` & `giant_newsletter-0.3.5/newsletter/migrations/0004_add_climatecare_fields.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/models.py` & `giant_newsletter-0.3.5/newsletter/models.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/tests/test_views.py` & `giant_newsletter-0.3.5/newsletter/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `giant_newsletter-0.3.4/newsletter/views.py` & `giant_newsletter-0.3.5/newsletter/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from django.urls import reverse
 from django.conf import settings
 from django.shortcuts import redirect, render
+from django.views.decorators.csrf import csrf_exempt
 
 from . import forms
 
 
+@csrf_exempt
 def index(request):
     """
     Index view for newsletter app
     """
     form = forms.SubscriptionForm(data=request.POST or None)
 
     success_url = getattr(settings, "NEWSLETTER_SUCCESS_URL", "newsletter:index")
```

### Comparing `giant_newsletter-0.3.4/pyproject.toml` & `giant_newsletter-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-newsletter"
-version = "0.3.4"
+version = "0.3.5"
 description = "A small reusable package that adds a Newsletter app to a project"
 authors = ["Will-Hoey <will.hoey@giantmade.com>", "Ben-Armstead <ben.armstead@giantmade.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-newsletter"
 repository = "https://github.com/giantmade/giant-newsletter"
 keywords = ["newsletter", "app"]
@@ -19,25 +19,25 @@
     "LICENSE",
 ]
 packages = [
     { include = "newsletter" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.9"
 giant-mixins = "*"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-django = "2.2"
-django-cms = "^3.7.2"
-black = "^19.10b0"
-pytest-cov = "^2.10.1"
-pytest-django = "^3.10.0"
-six = "^1.15.0"
+pytest = "~7"
+django = "~3"
+django-cms = "~3"
+black = "~22"
+pytest-cov = "~4"
+pytest-django = "~3"
+six = "~1"
 
 [[tool.poetry.source]]
 name = "TestPyPi"
 url = "https://test.pypi.org/simple/"
 secondary = true
 
 [build-system]
```

### Comparing `giant_newsletter-0.3.4/setup.py` & `giant_newsletter-0.3.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,50 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['newsletter', 'newsletter.migrations', 'newsletter.tests']
-
-package_data = \
-{'': ['*'], 'newsletter': ['templates/*', 'templates/newsletter/*']}
-
-install_requires = \
-['giant-mixins']
-
-setup_kwargs = {
-    'name': 'giant-newsletter',
-    'version': '0.3.4',
-    'description': 'A small reusable package that adds a Newsletter app to a project',
-    'long_description': '# Giant Newsletter\n\nA re-usable package which can be used in any project that requires a generic `Newletter` app. \n\nThis will include the basic formatting and functionality such as model creation via the admin and email sending.\n\n## Installation\n\nTo install with the package manager, run:\n\n    $ poetry add giant-newsletter\n\nYou should then add `"newsletter"` to the `INSTALLED_APPS` in your settings file and to the `Makefile`.  \n\nIn `base.py` there should also be a `DEFAULT_FROM_EMAIL` and a `DEFAULT_TO_EMAIL`. This is used by the email sending method.\n\n ## Context Processor\n If you wish to use the Contact form with the context processor you will need to add `newsletter.context_processors.subscription_form` into the `TEMPLATES` context processors list. This will allow you to access the form in templates.\n \n ## Configuration\n\n- `NEWSLETTER_FORM_FIELDS` allows the user to customise what fields are displayed on the form. This must be a list\n- `NEWSLETTER_FORM_FIELD_PLACEHOLDERS` allows the user to customise the field placeholder text. This must be a dict containing the fieldnames\n- `NEWSLETTER_FORM_REQUIRED_FIELDS` allows the user to customise what fields are required on the form. This must be a list\n- `NEWSLETTER_FORM_LABELS` allows the user to customise what the field labels are on the form. This must be a dict of field names and their corresponding label\n- `NEWSLETTER_FORM_WIDGETS` allows the user to customise what the field widgets are on the form. This must be a dict of field names and their corresponding widget\n- `NEWSLETTER_HTTP_REFERER` allows the user to customise the success url and return the user to the referer page after submission',
-    'author': 'Will-Hoey',
-    'author_email': 'will.hoey@giantmade.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/giantmade/giant-newsletter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: giant-newsletter
+Version: 0.3.5
+Summary: A small reusable package that adds a Newsletter app to a project
+Home-page: https://github.com/giantmade/giant-newsletter
+License: MIT
+Keywords: newsletter,app
+Author: Will-Hoey
+Author-email: will.hoey@giantmade.com
+Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: giant-mixins
+Project-URL: Repository, https://github.com/giantmade/giant-newsletter
+Description-Content-Type: text/markdown
+
+# Giant Newsletter
+
+A re-usable package which can be used in any project that requires a generic `Newletter` app. 
+
+This will include the basic formatting and functionality such as model creation via the admin and email sending.
+
+## Installation
+
+To install with the package manager, run:
+
+    $ poetry add giant-newsletter
+
+You should then add `"newsletter"` to the `INSTALLED_APPS` in your settings file and to the `Makefile`.  
+
+In `base.py` there should also be a `DEFAULT_FROM_EMAIL` and a `DEFAULT_TO_EMAIL`. This is used by the email sending method.
+
+ ## Context Processor
+ If you wish to use the Contact form with the context processor you will need to add `newsletter.context_processors.subscription_form` into the `TEMPLATES` context processors list. This will allow you to access the form in templates.
+ 
+ ## Configuration
+
+- `NEWSLETTER_FORM_FIELDS` allows the user to customise what fields are displayed on the form. This must be a list
+- `NEWSLETTER_FORM_FIELD_PLACEHOLDERS` allows the user to customise the field placeholder text. This must be a dict containing the fieldnames
+- `NEWSLETTER_FORM_REQUIRED_FIELDS` allows the user to customise what fields are required on the form. This must be a list
+- `NEWSLETTER_FORM_LABELS` allows the user to customise what the field labels are on the form. This must be a dict of field names and their corresponding label
+- `NEWSLETTER_FORM_WIDGETS` allows the user to customise what the field widgets are on the form. This must be a dict of field names and their corresponding widget
+- `NEWSLETTER_HTTP_REFERER` allows the user to customise the success url and return the user to the referer page after submission
```

