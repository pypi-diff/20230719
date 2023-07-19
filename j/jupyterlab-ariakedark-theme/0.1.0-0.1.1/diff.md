# Comparing `tmp/jupyterlab_ariakedark_theme-0.1.0.tar.gz` & `tmp/jupyterlab_ariakedark_theme-0.1.1.tar.gz`

## Comparing `jupyterlab_ariakedark_theme-0.1.0.tar` & `jupyterlab_ariakedark_theme-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/RELEASE.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/install.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/tsconfig.json
--rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/yarn.lock
--rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/images/jupyterlab_ariakedark_1.png
--rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/images/jupyterlab_ariakedark_2.png
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/_version.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/build_log.json
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/package.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.2ebfe68e2fe0b4b5a318.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.2ebfe68e2fe0b4b5a318.js.map
--rw-r--r--   0        0        0    27153 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.07b3da75a921d95bcdfe.js
--rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.07b3da75a921d95bcdfe.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/static/style.js
--rw-r--r--   0        0        0    13844 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/src/index.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/style/index.css
--rw-r--r--   0        0        0    13632 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/LICENSE
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/README.md
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/install.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/yarn.lock
+-rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_1.png
+-rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_2.png
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/_version.py
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/package.json
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/568.a4c8391e2673163e5dd0.js
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.42430a68b18808d3cc76.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/src/index.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/style/index.css
+-rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/README.md
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.1/PKG-INFO
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/RELEASE.md` & `jupyterlab_ariakedark_theme-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/package.json` & `jupyterlab_ariakedark_theme-0.1.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -172,9 +172,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/tsconfig.json` & `jupyterlab_ariakedark_theme-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/yarn.lock` & `jupyterlab_ariakedark_theme-0.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/images/jupyterlab_ariakedark_1.png` & `jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_1.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/images/jupyterlab_ariakedark_2.png` & `jupyterlab_ariakedark_theme-0.1.1/images/jupyterlab_ariakedark_2.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/__init__.py` & `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/package.json` & `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.42430a68b18808d3cc76.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -97,15 +97,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/eduardotlc/jupyterlab_ariakedark_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.07b3da75a921d95bcdfe.js"
+            "load": "static/remoteEntry.42430a68b18808d3cc76.js"
         },
         "extension": true,
         "outputDir": "jupyterlab_ariakedark_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -176,9 +176,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css` & `jupyterlab_ariakedark_theme-0.1.1/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -155,18 +155,18 @@
   --jp-content-heading-line-height: 1;
   --jp-content-heading-margin-top: 1.2em;
   --jp-content-heading-margin-bottom: 0.8em;
   --jp-content-heading-font-weight: 500;
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: #a3bed8;
-  --jp-content-font-color1: #92b5d8; 
+  --jp-content-font-color1: #92b5d8;
   --jp-content-font-color2: #81acd8;
   --jp-content-font-color3: #5094d8;
-  --jp-content-link-color:  #7e7edd;
+  --jp-content-link-color: #7e7edd;
   --jp-content-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI',
     helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
     'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
@@ -214,37 +214,36 @@
   /* Brand/accent */
 
   --jp-brand-color0: #9aefea;
   --jp-brand-color1: #5245dd;
   --jp-brand-color2: #5fa6a7;
   --jp-brand-color3: #a7d3fb;
   --jp-accent-color0: #7e7edd;
-  --jp-accent-color1: #7a69dd; 
+  --jp-accent-color1: #7a69dd;
   --jp-accent-color2: #5245dd;
   --jp-accent-color3: #a398dd;
 
   /* State colors (warn, error, success, info) */
 
   --jp-warn-color0: #ce7c60;
   --jp-warn-color1: #cea26f;
   --jp-warn-color2: #cea486;
   --jp-warn-color3: #cea091;
   --jp-error-color0: #bf2b52;
-  --jp-error-color1: #bf3d64;;
+  --jp-error-color1: #bf3d64;
   --jp-error-color2: #bf4c67;
   --jp-error-color3: #bf5384;
   --jp-success-color0: #4acead;
   --jp-success-color1: #66ceb4;
   --jp-success-color2: #7dcec1;
   --jp-success-color3: #7fcea4;
   --jp-info-color0: #a571f4;
   --jp-info-color1: #a186f4;
   --jp-info-color2: #b7a3f4;
   --jp-info-color3: #c9b4f4;
-
   --jp-cell-padding: 5px;
   --jp-cell-collapser-width: 8px;
   --jp-cell-collapser-min-height: 20px;
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
   --jp-cell-editor-background: #2e323e;
   --jp-cell-editor-border-color: #292d36;
   --jp-cell-editor-box-shadow: inset 0 0 2px #23262a;
@@ -255,15 +254,15 @@
   --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 0.5;
   --jp-cell-prompt-not-active-font-color: #656772;
 
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
-  --jp-cell-inprompt-font-color: #93DDFB;
+  --jp-cell-inprompt-font-color: #93ddfb;
 
   /* A custom blend of MD grey and orange 600
    * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
   --jp-cell-outprompt-font-color: #dda2f6;
 
   /* Notebook specific styles */
 
@@ -318,31 +317,31 @@
   --jp-input-border-color: #343d46;
   --jp-input-active-border-color: #232830;
 
   /* General editor styles */
 
   --jp-editor-selected-background: #4f5b66;
   --jp-editor-selected-focused-background: #343d46;
-  --jp-editor-cursor-color :#c0c5ce;
+  --jp-editor-cursor-color: #c0c5ce;
 
   /* Code mirror specific styles */
 
   --jp-mirror-editor-keyword-color: #7e7edd;
   --jp-mirror-editor-atom-color: #93ddfb;
   --jp-mirror-editor-number-color: #dda2f6;
   --jp-mirror-editor-def-color: #85b1e0;
   --jp-mirror-editor-variable-color: #dda2f6;
   --jp-mirror-editor-variable-2-color: #85b1e0;
   --jp-mirror-editor-variable-3-color: #4d8acb;
-  --jp-mirror-editor-punctuation-color: #93DDFB;
+  --jp-mirror-editor-punctuation-color: #93ddfb;
   --jp-mirror-editor-property-color: #85b1e0;
   --jp-mirror-editor-operator-color: #de97f2;
-  --jp-mirror-editor-comment-color: #555C77;
+  --jp-mirror-editor-comment-color: #555c77;
   --jp-mirror-editor-string-color: #9aefea;
-  --jp-mirror-editor-string-2-color: #93DDFB;
+  --jp-mirror-editor-string-2-color: #93ddfb;
   --jp-mirror-editor-meta-color: #a571f4;
   --jp-mirror-editor-qualifier-color: #7e7edd;
   --jp-mirror-editor-builtin-color: #7673d0;
   --jp-mirror-editor-bracket-color: #6363ab;
   --jp-mirror-editor-tag-color: #85b1e0;
   --jp-mirror-editor-attribute-color: #7ea6d2;
   --jp-mirror-editor-header-color: #4f5b66;
@@ -350,37 +349,34 @@
   --jp-mirror-editor-link-color: #7e7edd;
   --jp-mirror-editor-error-color: #e05252;
   --jp-mirror-editor-hr-color: #9aefea;
 
   /* User colors */
 
   --jp-collaborator-color1: #7e7edd;
-  --jp-collaborator-color2: #A571F4;
-  --jp-collaborator-color3: #9AEFEA;
+  --jp-collaborator-color2: #a571f4;
+  --jp-collaborator-color3: #9aefea;
   --jp-collaborator-color4: #dda2f6;
   --jp-collaborator-color5: #b9bed5;
   --jp-collaborator-color6: #b9bed5;
   --jp-collaborator-color7: #85b1e0;
 
   /* File or activity icons and switch semantic variables */
-
-
-  --jp-jupyter-icon-color: #de97f2; 
+  --jp-jupyter-icon-color: #de97f2;
   --jp-notebook-icon-color: #de97f2;
   --jp-json-icon-color: #dda2f6;
   --jp-console-icon-background-color: #3b5364;
   --jp-console-icon-color: #7673d0;
   --jp-terminal-icon-background-color: #4e5155;
   --jp-terminal-icon-color: #85b1e0;
   --jp-text-editor-icon-color: #93ddfb;
   --jp-inspector-icon-color: #65737f;
   --jp-switch-color: #a2b8d0;
   --jp-switch-true-position-color: #dda2f6;
   --jp-switch-cursor-color: #4f5b66;
-
   --jp-vega-background: #1c1f26;
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/src/index.ts` & `jupyterlab_ariakedark_theme-0.1.1/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,17 @@
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab_ariakedark_theme:plugin',
   description: 'An ariake dark palette based JupyterLab theme extension.',
   autoStart: true,
   requires: [IThemeManager],
   activate: (app: JupyterFrontEnd, manager: IThemeManager) => {
-    console.log('JupyterLab extension jupyterlab_ariakedark_theme is activated!');
+    console.log(
+      'JupyterLab extension jupyterlab_ariakedark_theme is activated!'
+    );
     const style = 'jupyterlab_ariakedark_theme/index.css';
 
     manager.register({
       name: 'jupyterlab_ariakedark_theme',
       isLight: false,
       load: () => manager.loadCSS(style),
       unload: () => Promise.resolve(undefined)
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/style/variables.css` & `jupyterlab_ariakedark_theme-0.1.1/style/variables.css`

 * *Files 2% similar despite different names*

```diff
@@ -155,18 +155,18 @@
   --jp-content-heading-line-height: 1;
   --jp-content-heading-margin-top: 1.2em;
   --jp-content-heading-margin-bottom: 0.8em;
   --jp-content-heading-font-weight: 500;
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: #a3bed8;
-  --jp-content-font-color1: #92b5d8; 
+  --jp-content-font-color1: #92b5d8;
   --jp-content-font-color2: #81acd8;
   --jp-content-font-color3: #5094d8;
-  --jp-content-link-color:  #7e7edd;
+  --jp-content-link-color: #7e7edd;
   --jp-content-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI',
     helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
     'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
@@ -214,37 +214,36 @@
   /* Brand/accent */
 
   --jp-brand-color0: #9aefea;
   --jp-brand-color1: #5245dd;
   --jp-brand-color2: #5fa6a7;
   --jp-brand-color3: #a7d3fb;
   --jp-accent-color0: #7e7edd;
-  --jp-accent-color1: #7a69dd; 
+  --jp-accent-color1: #7a69dd;
   --jp-accent-color2: #5245dd;
   --jp-accent-color3: #a398dd;
 
   /* State colors (warn, error, success, info) */
 
   --jp-warn-color0: #ce7c60;
   --jp-warn-color1: #cea26f;
   --jp-warn-color2: #cea486;
   --jp-warn-color3: #cea091;
   --jp-error-color0: #bf2b52;
-  --jp-error-color1: #bf3d64;;
+  --jp-error-color1: #bf3d64;
   --jp-error-color2: #bf4c67;
   --jp-error-color3: #bf5384;
   --jp-success-color0: #4acead;
   --jp-success-color1: #66ceb4;
   --jp-success-color2: #7dcec1;
   --jp-success-color3: #7fcea4;
   --jp-info-color0: #a571f4;
   --jp-info-color1: #a186f4;
   --jp-info-color2: #b7a3f4;
   --jp-info-color3: #c9b4f4;
-
   --jp-cell-padding: 5px;
   --jp-cell-collapser-width: 8px;
   --jp-cell-collapser-min-height: 20px;
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
   --jp-cell-editor-background: #2e323e;
   --jp-cell-editor-border-color: #292d36;
   --jp-cell-editor-box-shadow: inset 0 0 2px #23262a;
@@ -255,15 +254,15 @@
   --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 0.5;
   --jp-cell-prompt-not-active-font-color: #656772;
 
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
-  --jp-cell-inprompt-font-color: #93DDFB;
+  --jp-cell-inprompt-font-color: #93ddfb;
 
   /* A custom blend of MD grey and orange 600
    * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
   --jp-cell-outprompt-font-color: #dda2f6;
 
   /* Notebook specific styles */
 
@@ -318,31 +317,31 @@
   --jp-input-border-color: #343d46;
   --jp-input-active-border-color: #232830;
 
   /* General editor styles */
 
   --jp-editor-selected-background: #4f5b66;
   --jp-editor-selected-focused-background: #343d46;
-  --jp-editor-cursor-color :#c0c5ce;
+  --jp-editor-cursor-color: #c0c5ce;
 
   /* Code mirror specific styles */
 
   --jp-mirror-editor-keyword-color: #7e7edd;
   --jp-mirror-editor-atom-color: #93ddfb;
   --jp-mirror-editor-number-color: #dda2f6;
   --jp-mirror-editor-def-color: #85b1e0;
   --jp-mirror-editor-variable-color: #dda2f6;
   --jp-mirror-editor-variable-2-color: #85b1e0;
   --jp-mirror-editor-variable-3-color: #4d8acb;
-  --jp-mirror-editor-punctuation-color: #93DDFB;
+  --jp-mirror-editor-punctuation-color: #93ddfb;
   --jp-mirror-editor-property-color: #85b1e0;
   --jp-mirror-editor-operator-color: #de97f2;
-  --jp-mirror-editor-comment-color: #555C77;
+  --jp-mirror-editor-comment-color: #555c77;
   --jp-mirror-editor-string-color: #9aefea;
-  --jp-mirror-editor-string-2-color: #93DDFB;
+  --jp-mirror-editor-string-2-color: #93ddfb;
   --jp-mirror-editor-meta-color: #a571f4;
   --jp-mirror-editor-qualifier-color: #7e7edd;
   --jp-mirror-editor-builtin-color: #7673d0;
   --jp-mirror-editor-bracket-color: #6363ab;
   --jp-mirror-editor-tag-color: #85b1e0;
   --jp-mirror-editor-attribute-color: #7ea6d2;
   --jp-mirror-editor-header-color: #4f5b66;
@@ -350,36 +349,33 @@
   --jp-mirror-editor-link-color: #7e7edd;
   --jp-mirror-editor-error-color: #e05252;
   --jp-mirror-editor-hr-color: #9aefea;
 
   /* User colors */
 
   --jp-collaborator-color1: #7e7edd;
-  --jp-collaborator-color2: #A571F4;
-  --jp-collaborator-color3: #9AEFEA;
+  --jp-collaborator-color2: #a571f4;
+  --jp-collaborator-color3: #9aefea;
   --jp-collaborator-color4: #dda2f6;
   --jp-collaborator-color5: #b9bed5;
   --jp-collaborator-color6: #b9bed5;
   --jp-collaborator-color7: #85b1e0;
 
   /* File or activity icons and switch semantic variables */
-
-
-  --jp-jupyter-icon-color: #de97f2; 
+  --jp-jupyter-icon-color: #de97f2;
   --jp-notebook-icon-color: #de97f2;
   --jp-json-icon-color: #dda2f6;
   --jp-console-icon-background-color: #3b5364;
   --jp-console-icon-color: #7673d0;
   --jp-terminal-icon-background-color: #4e5155;
   --jp-terminal-icon-color: #85b1e0;
   --jp-text-editor-icon-color: #93ddfb;
   --jp-inspector-icon-color: #65737f;
   --jp-switch-color: #a2b8d0;
   --jp-switch-true-position-color: #dda2f6;
   --jp-switch-cursor-color: #4f5b66;
-
   --jp-vega-background: #1c1f26;
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/.gitignore` & `jupyterlab_ariakedark_theme-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/LICENSE` & `jupyterlab_ariakedark_theme-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/README.md` & `jupyterlab_ariakedark_theme-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 # jupyterlab_ariakedark_theme
 
-[![Github Actions Status](https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg)](https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml)
-An ariake dark palette based JupyterLab theme extension.
+**An ariake dark palette based JupyterLab theme extension.**
 
-[eduardotcampos@usp.br] [2023]
+|       build       |         PyPi          |
+| :---------------: | :-------------------: |
+| [![ci-badge]][ci] | [![pypi-badge]][pypi] |
+
+[ci-badge]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg
+[ci]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml
+[pypi-badge]: https://badge.fury.io/py/jupyterlab-ariakedark-theme.svg
+[pypi]: https://badge.fury.io/py/jupyterlab-ariakedark-theme
+
+eduardotcampos@usp.br [2023]
 
 ## Appearance
 
-![Example 1](/images/jupyterlab_ariakedark_1.png)
+![Example 1](./images/jupyterlab_ariakedark_1.png)
 
-![Example 2](/images/jupyterlab_ariakedark_2.png)
+![Example 2](./images/jupyterlab_ariakedark_2.png)
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
```

### Comparing `jupyterlab_ariakedark_theme-0.1.0/pyproject.toml` & `jupyterlab_ariakedark_theme-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.0/PKG-INFO` & `jupyterlab_ariakedark_theme-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_ariakedark_theme
-Version: 0.1.0
+Version: 0.1.1
 Summary: An ariake dark palette based JupyterLab theme extension.
 Project-URL: Homepage, https://github.com/eduardotlc/jupyterlab_ariakedark_theme
 Project-URL: Bug Tracker, https://github.com/eduardotlc/jupyterlab_ariakedark_theme/issues
 Project-URL: Repository, https://github.com/eduardotlc/jupyterlab_ariakedark_theme.git
 Author-email: Eduardo Campos <eduardotcampos@usp.br>
 License: BSD 3-Clause License
         
@@ -49,24 +49,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # jupyterlab_ariakedark_theme
 
-[![Github Actions Status](https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg)](https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml)
-An ariake dark palette based JupyterLab theme extension.
+**An ariake dark palette based JupyterLab theme extension.**
 
-[eduardotcampos@usp.br] [2023]
+|       build       |         PyPi          |
+| :---------------: | :-------------------: |
+| [![ci-badge]][ci] | [![pypi-badge]][pypi] |
+
+[ci-badge]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg
+[ci]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml
+[pypi-badge]: https://badge.fury.io/py/jupyterlab-ariakedark-theme.svg
+[pypi]: https://badge.fury.io/py/jupyterlab-ariakedark-theme
+
+eduardotcampos@usp.br [2023]
 
 ## Appearance
 
-![Example 1](/images/jupyterlab_ariakedark_1.png)
+![Example 1](./images/jupyterlab_ariakedark_1.png)
 
-![Example 2](/images/jupyterlab_ariakedark_2.png)
+![Example 2](./images/jupyterlab_ariakedark_2.png)
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
```

