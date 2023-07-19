# Comparing `tmp/essentials_openapi-1.0.7.tar.gz` & `tmp/essentials_openapi-1.0.8.tar.gz`

## Comparing `essentials_openapi-1.0.7.tar` & `essentials_openapi-1.0.8.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/.pytest_cache/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/common.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/logs.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/main.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/v2.py
--rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/v3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/commands/__init__.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/commands/docs.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/__init__.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/common.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/contents.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/generate.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/jinja.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/md.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/texts.py
--rw-r--r--   0        0        0    21375 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/examples.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/layout.html
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/type.html
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/__init__.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/layout.html
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/type.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/layout.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/layout.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/__init__.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/source.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/web.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/LICENSE
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/README.md
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/common.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/logs.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/main.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/v2.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/v3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/commands/__init__.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/commands/docs.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/common.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/contents.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/md.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/utils/__init__.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/utils/source.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/openapidocs/utils/web.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/LICENSE
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/README.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 essentials_openapi-1.0.8/PKG-INFO
```

### Comparing `essentials_openapi-1.0.7/CHANGELOG.md` & `essentials_openapi-1.0.8/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.8] - 2023-07-19 :cat:
+- Fixes example generation breaks on explicitly enumerated array elements #31,
+  by @jjedele.
+
 ## [1.0.7] - 2023-05-01 :toolbox:
 - Fixes [Markdown missing a newline after simple response types](https://github.com/Neoteroi/essentials-openapi/issues/27).
 - Fixes [Empty header when operations don't have any tag.](https://github.com/Neoteroi/essentials-openapi/issues/28).
 - When operations don't have any tag, the `h2` element
 - Improves tests.
 - Adopts `pyproject.toml`.
 - Workflow maintenance.
```

### Comparing `essentials_openapi-1.0.7/openapidocs/common.py` & `essentials_openapi-1.0.8/openapidocs/common.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/main.py` & `essentials_openapi-1.0.8/openapidocs/main.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/v2.py` & `essentials_openapi-1.0.8/openapidocs/v2.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/v3.py` & `essentials_openapi-1.0.8/openapidocs/v3.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/commands/docs.py` & `essentials_openapi-1.0.8/openapidocs/commands/docs.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/__init__.py` & `essentials_openapi-1.0.8/openapidocs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/common.py` & `essentials_openapi-1.0.8/openapidocs/mk/common.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/contents.py` & `essentials_openapi-1.0.8/openapidocs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/generate.py` & `essentials_openapi-1.0.8/openapidocs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/jinja.py` & `essentials_openapi-1.0.8/openapidocs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/md.py` & `essentials_openapi-1.0.8/openapidocs/mk/md.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/texts.py` & `essentials_openapi-1.0.8/openapidocs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/__init__.py` & `essentials_openapi-1.0.8/openapidocs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/examples.py` & `essentials_openapi-1.0.8/openapidocs/mk/v3/examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,19 @@
         Example:
           type: array
           items:
             $ref: '#/components/schemas/ReleaseNodeDownload'
           nullable: true
         """
         items = schema["items"]
-        return [get_example_from_schema(items) for _ in range(1)]
+
+        if not isinstance(items, list):
+            items = [items]
+
+        return [get_example_from_schema(item) for item in items]
 
 
 def get_subclasses(cls) -> Iterable[Type]:
     for subclass in cls.__subclasses__():
         yield from get_subclasses(subclass)
         yield subclass
```

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/layout.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-parameters.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-responses.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/info.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/path-items.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-responses.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/schema-repr.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/layout.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/info.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/path-items.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-body.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/type.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/layout.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/layout.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `essentials_openapi-1.0.8/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/utils/source.py` & `essentials_openapi-1.0.8/openapidocs/utils/source.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/openapidocs/utils/web.py` & `essentials_openapi-1.0.8/openapidocs/utils/web.py`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/LICENSE` & `essentials_openapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/README.md` & `essentials_openapi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/pyproject.toml` & `essentials_openapi-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `essentials_openapi-1.0.7/PKG-INFO` & `essentials_openapi-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: essentials-openapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Classes to generate OpenAPI Documentation v3 and v2, in JSON and YAML.
 Project-URL: Homepage, https://github.com/Neoteroi/essentials-openapi
 Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-openapi/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: Markdown,api,docs,documentation,json,openapi,swagger,v2,v3,yaml
 Classifier: Development Status :: 5 - Production/Stable
```

