# Comparing `tmp/xnbtd-0.0.7.tar.gz` & `tmp/xnbtd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.7.tar", max compression
+gzip compressed data, was "xnbtd-0.0.8.tar", max compression
```

## Comparing `xnbtd-0.0.7.tar` & `xnbtd-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.7/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.7/README.md
--rwxr-xr-x   0        0        0     3622 2023-07-18 17:18:43.240926 xnbtd-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.7/xnbtd/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.7/xnbtd/administration/__init__.py
--rwxr-xr-x   0        0        0      279 2023-07-18 16:22:18.242992 xnbtd-0.0.7/xnbtd/administration/admin.py
--rwxr-xr-x   0        0        0      157 2023-07-18 16:28:05.569856 xnbtd-0.0.7/xnbtd/administration/apps.py
--rwxr-xr-x   0        0        0     1403 2023-07-18 17:09:58.211602 xnbtd-0.0.7/xnbtd/administration/templates/xnbtd/admin/index.html
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.7/xnbtd/asgi.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.7/xnbtd/plannings/__init__.py
--rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.7/xnbtd/plannings/admin.py
--rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.7/xnbtd/plannings/apps.py
--rwxr-xr-x   0        0        0      581 2023-07-18 17:07:15.000000 xnbtd-0.0.7/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0      953 2023-07-18 17:06:20.379672 xnbtd-0.0.7/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.7/xnbtd/plannings/migrations/0001_initial.py
--rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.7/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
--rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.7/xnbtd/plannings/migrations/__init__.py
--rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.7/xnbtd/plannings/models.py
--rwxr-xr-x   0        0        0      324 2023-07-18 15:17:40.412906 xnbtd-0.0.7/xnbtd/plannings/templatetags/events.py
--rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.7/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.7/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5654 2023-07-18 16:47:07.219908 xnbtd-0.0.7/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.7/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.7/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.7/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.7/xnbtd/tours/__init__.py
--rwxr-xr-x   0        0        0     6654 2023-07-18 15:17:40.498280 xnbtd-0.0.7/xnbtd/tours/admin.py
--rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.7/xnbtd/tours/apps.py
--rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.7/xnbtd/tours/forms.py
--rwxr-xr-x   0        0        0     3731 2023-07-18 17:07:15.000000 xnbtd-0.0.7/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     6438 2023-07-18 17:06:20.302659 xnbtd-0.0.7/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.7/xnbtd/tours/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.7/xnbtd/tours/migrations/__init__.py
--rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.7/xnbtd/tours/models.py
--rwxr-xr-x   0        0        0      113 2023-07-18 13:08:06.430521 xnbtd-0.0.7/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.7/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.8/README.md
+-rwxr-xr-x   0        0        0     3622 2023-07-19 05:18:50.555078 xnbtd-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.8/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.8/xnbtd/administration/__init__.py
+-rwxr-xr-x   0        0        0      279 2023-07-18 16:22:18.242992 xnbtd-0.0.8/xnbtd/administration/admin.py
+-rwxr-xr-x   0        0        0      157 2023-07-18 16:28:05.569856 xnbtd-0.0.8/xnbtd/administration/apps.py
+-rwxr-xr-x   0        0        0     1656 2023-07-19 05:07:41.241082 xnbtd-0.0.8/xnbtd/administration/templates/xnbtd/admin/index.html
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.8/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.8/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.8/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.8/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-07-18 17:07:15.000000 xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      953 2023-07-18 17:06:20.379672 xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.8/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.8/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.8/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.8/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-0.0.8/xnbtd/plannings/templatetags/events.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.8/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.8/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5654 2023-07-18 16:47:07.219908 xnbtd-0.0.8/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.8/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.8/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.8/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.8/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0     6654 2023-07-18 15:17:40.498280 xnbtd-0.0.8/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.8/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.8/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     3731 2023-07-18 17:07:15.000000 xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     6438 2023-07-18 17:06:20.302659 xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.8/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.8/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.8/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      113 2023-07-18 13:08:06.430521 xnbtd-0.0.8/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.8/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.8/PKG-INFO
```

### Comparing `xnbtd-0.0.7/LICENSE` & `xnbtd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/README.md` & `xnbtd-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/pyproject.toml` & `xnbtd-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.7"
+version = "0.0.8"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-0.0.7/xnbtd/administration/templates/xnbtd/admin/index.html` & `xnbtd-0.0.8/xnbtd/administration/templates/xnbtd/admin/index.html`

 * *Files 21% similar despite different names*

```diff
@@ -18,26 +18,29 @@
 {% endblock %}
 
 {% block sidebar %}
 <div id="content-related">
     <div class="module" id="recent-events-module">
         <h2>Évènements à venir</h2>
         {% load events %}
-        {% get_upcoming_events 10 as upcoming_events %}
+        {% get_upcoming_events_grouped 10 as upcoming_events %}
         {% if not upcoming_events %}
             <p>Aucun évènement à venir</p>
         {% else %}
             <ul class="actionlist">
-                {% for event in upcoming_events %}
-                    <li class="eventlink">
-                        <a href="{% url 'admin:plannings_event_change' event.id %}">
-                            {{ event.title }}
-                        </a>
-                        <br>
-                        <span class="mini quiet">{{ event.date }}</span>
-                    </li>
+                {% for date, events in upcoming_events.items %}
+                    <h3 style="padding: 0px; margin: 0px; margin-bottom: 8px;">{{ date }}</h3>
+                    <ul style="margin-left: 0px; ">
+                        {% for event in events %}
+                            <li style="padding-left: 0px; margin-bottom: 0px;">
+                                <a href="{% url 'admin:plannings_event_change' event.id %}">
+                                    - {{ event.title }}
+                                </a>
+                            </li>
+                        {% endfor %}
+                    </ul>
                 {% endfor %}
             </ul>
         {% endif %}
     </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,17 +4,19 @@
 block bodyclass %}{{ block.super }} dashboard{% endblock %} {% block nav-
 breadcrumbs %}{% endblock %} {% block nav-sidebar %}{% endblock %} {% block
 content %}
 {% include "admin/app_list.html" with app_list=app_list show_changelinks=True
 %}
 {% endblock %} {% block sidebar %}
 ***** ÃvÃ¨nements Ã  venir *****
-{% load events %} {% get_upcoming_events 10 as upcoming_events %} {% if not
-upcoming_events %}
+{% load events %} {% get_upcoming_events_grouped 10 as upcoming_events %} {% if
+not upcoming_events %}
 Aucun Ã©vÃ¨nement Ã  venir
 {% else %}
-    * {% for event in upcoming_events %}
-    * {{_event.title_}}
-      {{ event.date }}
+    * {% for date, events in upcoming_events.items %}
+**** {{ date }} ****
+    * {% for event in events %}
+    * -_{{_event.title_}}
     * {% endfor %}
+{% endfor %}
 {% endif %}
 {% endblock %}
```

### Comparing `xnbtd-0.0.7/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/plannings/migrations/0001_initial.py` & `xnbtd-0.0.8/xnbtd/plannings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py` & `xnbtd-0.0.8/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/publish.py` & `xnbtd-0.0.8/xnbtd/publish.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/settings/base.py` & `xnbtd-0.0.8/xnbtd/settings/base.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/settings/local.py` & `xnbtd-0.0.8/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/tours/admin.py` & `xnbtd-0.0.8/xnbtd/tours/admin.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/tours/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/tours/migrations/0001_initial.py` & `xnbtd-0.0.8/xnbtd/tours/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/xnbtd/tours/models.py` & `xnbtd-0.0.8/xnbtd/tours/models.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.7/PKG-INFO` & `xnbtd-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.7
+Version: 0.0.8
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

