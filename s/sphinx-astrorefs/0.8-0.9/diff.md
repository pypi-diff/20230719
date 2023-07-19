# Comparing `tmp/sphinx-astrorefs-0.8.tar.gz` & `tmp/sphinx-astrorefs-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bovy/Repos/sphinx-astrorefs/dist/tmppxyp1jj_/sphinx-astrorefs-0.8.tar", last modified: Thu Jul  7 01:01:39 2022, max compression
+gzip compressed data, was "sphinx-astrorefs-0.9.tar", last modified: Wed Jul 19 00:59:55 2023, max compression
```

## Comparing `sphinx-astrorefs-0.8.tar` & `sphinx-astrorefs-0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 bovy       (501) staff       (20)        0 2022-07-07 01:01:39.431572 sphinx-astrorefs-0.8/
--rw-r--r--   0 bovy       (501) staff       (20)     1064 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/LICENSE
--rw-r--r--   0 bovy       (501) staff       (20)       79 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/MANIFEST.in
--rw-r--r--   0 bovy       (501) staff       (20)     3548 2022-07-07 01:01:39.431333 sphinx-astrorefs-0.8/PKG-INFO
--rw-r--r--   0 bovy       (501) staff       (20)     3309 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/README.md
--rw-r--r--   0 bovy       (501) staff       (20)       90 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/pyproject.toml
--rw-r--r--   0 bovy       (501) staff       (20)       38 2022-07-07 01:01:39.431731 sphinx-astrorefs-0.8/setup.cfg
--rw-r--r--   0 bovy       (501) staff       (20)      606 2022-07-07 01:00:04.000000 sphinx-astrorefs-0.8/setup.py
-drwxr-xr-x   0 bovy       (501) staff       (20)        0 2022-07-07 01:01:39.429463 sphinx-astrorefs-0.8/sphinx_astrorefs/
--rw-r--r--   0 bovy       (501) staff       (20)     1018 2022-07-07 01:00:04.000000 sphinx-astrorefs-0.8/sphinx_astrorefs/__init__.py
-drwxr-xr-x   0 bovy       (501) staff       (20)        0 2022-07-07 01:01:39.431018 sphinx-astrorefs-0.8/sphinx_astrorefs/_static/
--rw-r--r--   0 bovy       (501) staff       (20)      526 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs/_static/sphinx_astrorefs.css
--rw-r--r--   0 bovy       (501) staff       (20)     7211 2022-07-07 00:41:09.000000 sphinx-astrorefs-0.8/sphinx_astrorefs/pybtex_astro.py
--rw-r--r--   0 bovy       (501) staff       (20)     9439 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs/reformat.py
--rw-r--r--   0 bovy       (501) staff       (20)     3576 2022-07-07 00:24:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs/resolve_aas.py
-drwxr-xr-x   0 bovy       (501) staff       (20)        0 2022-07-07 01:01:39.430770 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/
--rw-r--r--   0 bovy       (501) staff       (20)     3548 2022-07-07 01:01:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/PKG-INFO
--rw-r--r--   0 bovy       (501) staff       (20)      421 2022-07-07 01:01:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/SOURCES.txt
--rw-r--r--   0 bovy       (501) staff       (20)        1 2022-07-07 01:01:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/dependency_links.txt
--rw-r--r--   0 bovy       (501) staff       (20)       53 2022-07-07 01:01:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/requires.txt
--rw-r--r--   0 bovy       (501) staff       (20)       17 2022-07-07 01:01:39.000000 sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:55.070147 sphinx-astrorefs-0.9/sphinx_astrorefs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/sphinx_astrorefs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/sphinx_astrorefs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/sphinx_astrorefs/_static/sphinx_astrorefs.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/sphinx_astrorefs/pybtex_astro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/sphinx_astrorefs/reformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/sphinx_astrorefs/resolve_aas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-19 00:59:55.000000 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-19 00:59:55.000000 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 00:59:55.000000 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 00:59:55.000000 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 00:59:55.000000 sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:55.074147 sphinx-astrorefs-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-19 00:59:46.000000 sphinx-astrorefs-0.9/tests/test_resolve_aas.py
```

### Comparing `sphinx-astrorefs-0.8/LICENSE` & `sphinx-astrorefs-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-astrorefs-0.8/PKG-INFO` & `sphinx-astrorefs-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-astrorefs
-Version: 0.8
+Version: 0.9
 Summary: Astro-style references in Sphinx documents
 Author: Jo Bovy
 Author-email: bovy@astro.utoronto.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,24 +20,26 @@
 ``sphinx-astrorefs`` is a Sphinx extension for formatting citations and references in a style similar to that used in the astrophysics literature. It is built on top of [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex), a Sphinx extension for including bibtex citations in Sphinx documents. By pre- and post-processing the input and output from Sphinx and sphinxcontrib-bibtex, ``sphinx-astrorefs`` allows you to obtain citations in the astro-specific style in the HTML and LaTeX rendering of your Sphinx documents.
 
 * Author: Jo Bovy - bovy at astro dot utoronto dot ca
 * Documentation: [https://sphinx-astrorefs.readthedocs.io/](https://sphinx-astrorefs.readthedocs.io/)
 
 ## Changelog
 
+* **2023/07/23**: Version 0.9: Perform better formatting of book, proceedings, and PhD thesis references that is also more consistent with how articles are formatted.
+* **2022/07/06**: Version 0.8: Pin ``sphinxcontrib.bibtex`` version to 2.1.4, because this code doesn't work for more recent versions (yet). Also allow the ``arxiv.org`` part of the arXiv URL to be changed through the ``astrorefs_arxiv_url`` configuration parameter.
 * **2021/01/06**: Version 0.7: Further changes for ``sphinxcontrib.bibtex`` version 2.1, because those in version 0.6 were not correct. As in version 0.6, this package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2021/01/06**: Version 0.6: Small changes for ``sphinxcontrib.bibtex`` version 2.1 (no longer required to run sphinx twice or to commit ``bibtex.json``). This package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2020/12/19**: Version 0.5: Minor bug fixes (missing volume fields, latex preambe) and changes for ``sphinxcontrib.bibtex`` version 2.
 * **2020/08/25**: Version 0.4: Adds correct dealing with duplicate labels by adding a letter ('a', 'b', ...) to the year and added the remainder of the AAS macros so they are now all correctly resolved.
 * **2020/08/09**: Version 0.3: Fixes a minor bug in 0.2 that caused multiple \citealt-style citations in a single line be parsed incorrectly. All reference replacements are now done one at a time, so multi-citation lines should now be handled correctly for all citation types.
 * **2020/07/22**: Version 0.2: Removes printing the Sphinx builder's name and makes the bibtex label invisible in the HTML reference section without removing the element entirely and thus removing the id link, thus fixing the HTML rendering of the reference section.
 * **2020/07/01**: Version 0.1.
 
 ## Development notes
 
 To release a new version, do the following
 
 * ``bumpversion release`` and commit the result with ``git commit -m "Bump version to next release" .``
 * ``git tag `python -c "import sphinx_astrorefs; print(sphinx_astrorefs.__version__)"` && git push --tags``
-* `` rm -rf build && rm -rf dist/* && python setup.py sdist bdist_wheel``
-* ``twine upload dist/*`` for uploading to PyPI
+* Create a release on GitHub --> this triggers the GitHub action that will build the package and upload it to PyPI
+* Update default version on readthedocs.
 * ``bumpversion minor`` for setting up development version of next minor release or ``bumpversion major`` for a next major release. Then commit the result with ``git commit -m "Bump version to next development version" .``
```

### Comparing `sphinx-astrorefs-0.8/README.md` & `sphinx-astrorefs-0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 ``sphinx-astrorefs`` is a Sphinx extension for formatting citations and references in a style similar to that used in the astrophysics literature. It is built on top of [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex), a Sphinx extension for including bibtex citations in Sphinx documents. By pre- and post-processing the input and output from Sphinx and sphinxcontrib-bibtex, ``sphinx-astrorefs`` allows you to obtain citations in the astro-specific style in the HTML and LaTeX rendering of your Sphinx documents.
 
 * Author: Jo Bovy - bovy at astro dot utoronto dot ca
 * Documentation: [https://sphinx-astrorefs.readthedocs.io/](https://sphinx-astrorefs.readthedocs.io/)
 
 ## Changelog
 
+* **2023/07/23**: Version 0.9: Perform better formatting of book, proceedings, and PhD thesis references that is also more consistent with how articles are formatted.
+* **2022/07/06**: Version 0.8: Pin ``sphinxcontrib.bibtex`` version to 2.1.4, because this code doesn't work for more recent versions (yet). Also allow the ``arxiv.org`` part of the arXiv URL to be changed through the ``astrorefs_arxiv_url`` configuration parameter.
 * **2021/01/06**: Version 0.7: Further changes for ``sphinxcontrib.bibtex`` version 2.1, because those in version 0.6 were not correct. As in version 0.6, this package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2021/01/06**: Version 0.6: Small changes for ``sphinxcontrib.bibtex`` version 2.1 (no longer required to run sphinx twice or to commit ``bibtex.json``). This package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2020/12/19**: Version 0.5: Minor bug fixes (missing volume fields, latex preambe) and changes for ``sphinxcontrib.bibtex`` version 2.
 * **2020/08/25**: Version 0.4: Adds correct dealing with duplicate labels by adding a letter ('a', 'b', ...) to the year and added the remainder of the AAS macros so they are now all correctly resolved.
 * **2020/08/09**: Version 0.3: Fixes a minor bug in 0.2 that caused multiple \citealt-style citations in a single line be parsed incorrectly. All reference replacements are now done one at a time, so multi-citation lines should now be handled correctly for all citation types.
 * **2020/07/22**: Version 0.2: Removes printing the Sphinx builder's name and makes the bibtex label invisible in the HTML reference section without removing the element entirely and thus removing the id link, thus fixing the HTML rendering of the reference section.
 * **2020/07/01**: Version 0.1.
 
 ## Development notes
 
 To release a new version, do the following
 
 * ``bumpversion release`` and commit the result with ``git commit -m "Bump version to next release" .``
 * ``git tag `python -c "import sphinx_astrorefs; print(sphinx_astrorefs.__version__)"` && git push --tags``
-* `` rm -rf build && rm -rf dist/* && python setup.py sdist bdist_wheel``
-* ``twine upload dist/*`` for uploading to PyPI
+* Create a release on GitHub --> this triggers the GitHub action that will build the package and upload it to PyPI
+* Update default version on readthedocs.
 * ``bumpversion minor`` for setting up development version of next minor release or ``bumpversion major`` for a next major release. Then commit the result with ``git commit -m "Bump version to next development version" .``
```

### Comparing `sphinx-astrorefs-0.8/setup.py` & `sphinx-astrorefs-0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphinx-astrorefs",
-    version="0.8",
+    version="0.9",
     author="Jo Bovy",
     author_email="bovy@astro.utoronto.ca",
     description="Astro-style references in Sphinx documents",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=["sphinx_astrorefs"],
```

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs/__init__.py` & `sphinx-astrorefs-0.9/sphinx_astrorefs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from . import pybtex_astro
 from . import reformat
 from . import resolve_aas
-__version__= "0.8"
+__version__= "0.9"
 
 def append_static_path(app,config):
     config.html_static_path.append(
         str(Path(__file__).parent.joinpath("_static").absolute()))
 
 def setup(app):
     app.add_config_value('astrorefs_arxiv_url','arxiv.org','env')
```

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs/_static/sphinx_astrorefs.css` & `sphinx-astrorefs-0.9/sphinx_astrorefs/_static/sphinx_astrorefs.css`

 * *Files identical despite different names*

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs/pybtex_astro.py` & `sphinx-astrorefs-0.9/sphinx_astrorefs/pybtex_astro.py`

 * *Files 22% similar despite different names*

```diff
@@ -116,14 +116,42 @@
                 join [
                     'https://doi.org/',
                     field('doi', raw=True)
                     ],
                 field('journal')
                 ]
 
+    def format_btitle(self,e, which_field, as_sentence=True):
+        formatted_title = tag('em') [ field(which_field) ]
+        if 'doi' not in e.fields and 'adsurl' in e.fields:
+            url  = field('adsurl',raw=True)
+        elif 'doi' in e.fields:
+            url = join [
+                'https://doi.org/',
+                field('doi', raw=True)
+                ]
+        else:
+            url = None
+        if url is None and as_sentence:
+            return sentence [formatted_title ]
+        elif url is None:
+            return formatted_title
+        elif as_sentence:
+            return sentence [
+                href [
+                    url,
+                    formatted_title
+                    ]
+                ]
+        else:
+            return href [
+                url,
+                formatted_title
+                ]
+
     def format_volume(self,e):
         if 'adsurl' not in e.fields:
             return field('volume')
         else:
             return href [ field('adsurl',raw=True),
                           field('volume')]
 
@@ -135,14 +163,55 @@
                 join [
                     f'https://{_arxiv_url}/abs/',
                     field('eprint', raw=True)
                     ],
                 field('pages',apply_func=dashify)
                 ]
 
+    def format_publisher(self,e):
+        if 'doi' not in e.fields:
+            return field('publisher')
+        else:
+            return href [
+                join [
+                    'https://doi.org/',
+                    field('doi', raw=True)
+                    ],
+                field('publisher')
+                ]
+
+    def format_publisher_address(self,e):
+        if 'adsurl' not in e.fields:
+            return field('address')
+        else:
+            return href [ 
+                field('adsurl',raw=True),
+                field('address')
+                ]
+        
+    def format_volume_and_series(self, e, as_sentence=True):
+        if as_sentence:
+            return sentence [
+                join [
+                    optional [ 
+                        field('series') ,
+                        ' ',
+                        tag('strong') [ field('volume') ] 
+                    ]
+                ]
+            ]
+        else:
+            return join [
+                optional [ 
+                    field('series') ,
+                    ' ',
+                    tag('strong') [ field('volume') ]
+                ]
+            ]
+        
     def get_article_template(self, e):
         if 'volume' not in e.fields:
             journal_and_volume = tag('em') [self.format_journal(e)]
         else:
             journal_and_volume = join [
                 tag('em') [self.format_journal(e)],' ',
                 tag('strong') [self.format_volume(e)]
@@ -162,22 +231,69 @@
     def get_book_template(self, e):
         template = toplevel [
             self.format_author_or_editor(e),
             self.format_btitle(e, 'title'),
             self.format_volume_and_series(e),
             sentence [
                 join [
-                    field('publisher'),
-                    optional [', ',field('address')],
+                    self.format_publisher(e),
+                    ', ',
+                    self.format_publisher_address(e),
                     ' (',field('year'),')']
                 ],
             optional[ sentence [ self.format_isbn(e) ] ],
-            self.format_web_refs(e),
+            optional [ self.format_eprint(e) ],
         ]
         return template
+    
+    def get_inproceedings_template(self, e):
+        template = toplevel [
+            sentence [self.format_names('author')],
+            self.format_title(e, 'title'),
+            words [
+                'In',
+                sentence [
+                    optional[ self.format_editor(e, as_sentence=False) ],
+                    self.format_btitle(e, 'booktitle', as_sentence=False),
+                    optional [
+                        href [
+                            field('adsurl',raw=True),
+                            self.format_volume_and_series(e, as_sentence=False)
+                        ]
+                        if 'adsurl' in e.fields and 'doi' in e.fields
+                        else
+                        self.format_volume_and_series(e, as_sentence=False)
+                    ],
+                    join [
+                        optional[ self.format_pages(e) ],
+                        ' (',field('year'),')'
+                    ]
+                ],
+            ]
+        ]
+        return template
+    
+    def get_phdthesis_template(self, e):
+        template = toplevel [
+            sentence [self.format_names('author')],
+            self.format_btitle(e, 'title'),
+            sentence[
+                first_of [
+                    optional_field('type'),
+                    'PhD thesis',
+                ],
+                join [
+                    field('school'),
+                    ', ' if 'address' in e.fields else '',
+                    optional_field('address'),
+                    ' (',field('year'),')',
+                ]
+            ]
+        ]
+        return template    
 
 def register():
     logger.info("Registering astro-style pybtex formatting...")
     register_plugin('pybtex.style.formatting', 'astrostyle', AstroStyle)
 
 def register_with_config(app,config):
     logger.info("Registering astro-style pybtex formatting...")
```

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs/reformat.py` & `sphinx-astrorefs-0.9/sphinx_astrorefs/reformat.py`

 * *Files identical despite different names*

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs/resolve_aas.py` & `sphinx-astrorefs-0.9/sphinx_astrorefs/resolve_aas.py`

 * *Files identical despite different names*

### Comparing `sphinx-astrorefs-0.8/sphinx_astrorefs.egg-info/PKG-INFO` & `sphinx-astrorefs-0.9/sphinx_astrorefs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-astrorefs
-Version: 0.8
+Version: 0.9
 Summary: Astro-style references in Sphinx documents
 Author: Jo Bovy
 Author-email: bovy@astro.utoronto.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,24 +20,26 @@
 ``sphinx-astrorefs`` is a Sphinx extension for formatting citations and references in a style similar to that used in the astrophysics literature. It is built on top of [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex), a Sphinx extension for including bibtex citations in Sphinx documents. By pre- and post-processing the input and output from Sphinx and sphinxcontrib-bibtex, ``sphinx-astrorefs`` allows you to obtain citations in the astro-specific style in the HTML and LaTeX rendering of your Sphinx documents.
 
 * Author: Jo Bovy - bovy at astro dot utoronto dot ca
 * Documentation: [https://sphinx-astrorefs.readthedocs.io/](https://sphinx-astrorefs.readthedocs.io/)
 
 ## Changelog
 
+* **2023/07/23**: Version 0.9: Perform better formatting of book, proceedings, and PhD thesis references that is also more consistent with how articles are formatted.
+* **2022/07/06**: Version 0.8: Pin ``sphinxcontrib.bibtex`` version to 2.1.4, because this code doesn't work for more recent versions (yet). Also allow the ``arxiv.org`` part of the arXiv URL to be changed through the ``astrorefs_arxiv_url`` configuration parameter.
 * **2021/01/06**: Version 0.7: Further changes for ``sphinxcontrib.bibtex`` version 2.1, because those in version 0.6 were not correct. As in version 0.6, this package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2021/01/06**: Version 0.6: Small changes for ``sphinxcontrib.bibtex`` version 2.1 (no longer required to run sphinx twice or to commit ``bibtex.json``). This package is compatible with ``sphinxcontrib.bibtex`` v1 and v2.1 and beyond, but not v2.0.
 * **2020/12/19**: Version 0.5: Minor bug fixes (missing volume fields, latex preambe) and changes for ``sphinxcontrib.bibtex`` version 2.
 * **2020/08/25**: Version 0.4: Adds correct dealing with duplicate labels by adding a letter ('a', 'b', ...) to the year and added the remainder of the AAS macros so they are now all correctly resolved.
 * **2020/08/09**: Version 0.3: Fixes a minor bug in 0.2 that caused multiple \citealt-style citations in a single line be parsed incorrectly. All reference replacements are now done one at a time, so multi-citation lines should now be handled correctly for all citation types.
 * **2020/07/22**: Version 0.2: Removes printing the Sphinx builder's name and makes the bibtex label invisible in the HTML reference section without removing the element entirely and thus removing the id link, thus fixing the HTML rendering of the reference section.
 * **2020/07/01**: Version 0.1.
 
 ## Development notes
 
 To release a new version, do the following
 
 * ``bumpversion release`` and commit the result with ``git commit -m "Bump version to next release" .``
 * ``git tag `python -c "import sphinx_astrorefs; print(sphinx_astrorefs.__version__)"` && git push --tags``
-* `` rm -rf build && rm -rf dist/* && python setup.py sdist bdist_wheel``
-* ``twine upload dist/*`` for uploading to PyPI
+* Create a release on GitHub --> this triggers the GitHub action that will build the package and upload it to PyPI
+* Update default version on readthedocs.
 * ``bumpversion minor`` for setting up development version of next minor release or ``bumpversion major`` for a next major release. Then commit the result with ``git commit -m "Bump version to next development version" .``
```

