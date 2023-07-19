# Comparing `tmp/fast_transfer-0.1.3.tar.gz` & `tmp/fast_transfer-0.2.0.tar.gz`

## Comparing `fast_transfer-0.1.3.tar` & `fast_transfer-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0   207302 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/src/fast_transfer/static/bulma.min.css
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/src/fast_transfer/templates/index.html
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/LICENSE
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/README.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0   207302 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/src/fast_transfer/static/bulma.min.css
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/src/fast_transfer/templates/index.html
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/LICENSE
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/README.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fast_transfer-0.2.0/PKG-INFO
```

### Comparing `fast_transfer-0.1.3/src/fast_transfer/static/bulma.min.css` & `fast_transfer-0.2.0/src/fast_transfer/static/bulma.min.css`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.3/src/fast_transfer/templates/index.html` & `fast_transfer-0.2.0/src/fast_transfer/templates/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <title>Fast Transfer</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1">
     <link rel="stylesheet" href="/static/bulma.min.css" />
   </head>
   <body>
     <section class="section">
       <div class="container">
 	<div class="columns">
 	  <div class="column is-8 is-offset-2">
@@ -43,24 +44,24 @@
 	    </div>
 
 	    {% if links %}
 	    <div class="table-container">
 	      <table class="table is-fullwidth">
 		<thead>
 		  <tr>
-		    <th>File</th>
-		    <th>Size</th>
-		    <th>Created At</th>
-		    <th>Last Modified</th>
+		    <th>{% if sort == "-name" %}<a href="?dir={{dir}}&sort=name">Name &darr;</a>{% elif sort == "name" %}<a href="?dir={{dir}}&sort=-name">Name &uarr;</a>{% else %}<a href="?dir={{dir}}&sort=name">Name</a>{% endif %}</th>
+		    <th>{% if sort == "-size" %}<a href="?dir={{dir}}&sort=size">Size &darr;</a>{% elif sort == "size" %}<a href="?dir={{dir}}&sort=-size">Size &uarr;</a>{% else %}<a href="?dir={{dir}}&sort=size">Size</a>{% endif %}</th>
+		    <th>{% if sort == "-ctime" %}<a href="?dir={{dir}}&sort=ctime">Created At &darr;</a>{% elif sort == "ctime" %}<a href="?dir={{dir}}&sort=-ctime">Created At &uarr;</a>{% else %}<a href="?dir={{dir}}&sort=-ctime">Created At</a>{% endif %}</th>
+		    <th>{% if sort == "-mtime" %}<a href="?dir={{dir}}&sort=mtime">Last Modified &darr;</a>{% elif sort == "mtime" %}<a href="?dir={{dir}}&sort=-mtime">Last Modified &uarr;</a>{% else %}<a href="?dir={{dir}}&sort=-mtime">Last Modified</a>{% endif %}</th>
 		  </tr>
 		</thead>
 		<tbody>
 		  {% for link in links %}
 		    <tr>
-		      <td><a href="{{ link.link }}">{{ link.file }}</a></td>
+		      <td><a href="{{ link.link }}">{{ link.name }}</a></td>
 		      <td>{{link.size|filesizeformat}}</td>
 		      <td>{{link.ctime}}</td>
 		      <td>{{link.mtime}}</td>
 		    </tr>
 		  {% endfor %}
 		</tbody>
 	      </table>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+
 ****** Fast Transfer ******
 {% with messages = get_flashed_messages() %} {% if messages %} {% for message
 in messages %}
 {{message}}
 {% endfor %} {% endif %} {% endwith %}
 {% if dirs %}
     * Home
@@ -9,14 +10,16 @@
     * % if loop.last %} class="is-active"{% endif %}>
     * % if loop.last %}href="#" aria-current="page"{% else %}{% endif
       %}href="?dir={{dir.path}}">{{dir.name}}
 {% endfor %}
  {% endif %}
  [File]Upload
 {% if links %}
-File            Size                         Created At     Last Modified
-{{_link.file_}} {{link.size|filesizeformat}} {{link.ctime}} {{link.mtime}}
+{% if sort == "-name" %}Name_↓{% elif sort == "name" %}Name_↑{% else %}Name{% {% if sort == "-size" %}Size_↓{% elif sort == "size" %}Size_↑{% else %}Size{% {% if sort == "-ctime" %}Created_At_↓{% elif sort == "ctime" %}Created_At_↑{% {% if sort == "-mtime" %}Last_Modified_↓{% elif sort ==
+endif %}                                                                          endif %}                                                                          else %}Created_At{% endif %}                                                      "mtime" %}Last_Modified_↑{% else %}Last_Modified{% endif
+                                                                                                                                                                                                                                                      %}
+{{_link.name_}}                                                                   {{link.size|filesizeformat}}                                                      {{link.ctime}}                                                                    {{link.mtime}}
 {% else %}
 Empty
 {% endif %}
 
 Github
```

### Comparing `fast_transfer-0.1.3/.gitignore` & `fast_transfer-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.3/LICENSE` & `fast_transfer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.3/pyproject.toml` & `fast_transfer-0.2.0/pyproject.toml`

 * *Files identical despite different names*

