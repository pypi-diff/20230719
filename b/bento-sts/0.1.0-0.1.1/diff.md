# Comparing `tmp/bento_sts-0.1.0.tar.gz` & `tmp/bento_sts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_sts-0.1.0.tar", max compression
+gzip compressed data, was "bento_sts-0.1.1.tar", max compression
```

## Comparing `bento_sts-0.1.0.tar` & `bento_sts-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,84 @@
--rw-r--r--   0        0        0     1079 2020-10-19 17:56:24.008960 bento_sts-0.1.0/LICENSE
--rw-r--r--   0        0        0      415 2023-07-08 22:03:48.092764 bento_sts-0.1.0/README.md
--rw-r--r--   0        0        0     3301 2023-07-08 22:05:03.033626 bento_sts-0.1.0/nginx/sts.conf
--rw-r--r--   0        0        0     1924 2023-07-14 00:55:09.223254 bento_sts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       51 2023-07-09 19:32:46.361891 bento_sts-0.1.0/src/bento_sts/__init__.py
--rw-r--r--   0        0        0       84 2023-07-09 19:16:57.363182 bento_sts-0.1.0/src/bento_sts/api/__init__.py
--rw-r--r--   0        0        0     3941 2023-07-09 19:39:48.617466 bento_sts-0.1.0/src/bento_sts/api/routes.py
--rw-r--r--   0        0        0       28 2023-07-07 02:01:31.478631 bento_sts-0.1.0/src/bento_sts/cli.py
--rw-r--r--   0        0        0      855 2023-07-09 20:05:36.333841 bento_sts-0.1.0/src/bento_sts/config.py
--rw-r--r--   0        0        0        0 2022-02-25 02:56:46.496832 bento_sts-0.1.0/src/bento_sts/config_sts/__init__.py
--rw-r--r--   0        0        0     5687 2022-02-25 02:56:46.497407 bento_sts-0.1.0/src/bento_sts/config_sts/query_paths.yml
--rw-r--r--   0        0        0       82 2023-07-09 19:34:07.790210 bento_sts-0.1.0/src/bento_sts/errors/__init__.py
--rw-r--r--   0        0        0      390 2023-07-09 20:07:09.565949 bento_sts-0.1.0/src/bento_sts/errors/handlers.py
--rw-r--r--   0        0        0       87 2023-07-09 19:16:54.204908 bento_sts-0.1.0/src/bento_sts/main/__init__.py
--rw-r--r--   0        0        0      813 2023-07-07 02:01:31.476646 bento_sts-0.1.0/src/bento_sts/main/forms.py
--rw-r--r--   0        0        0    10606 2023-07-09 19:39:26.445559 bento_sts-0.1.0/src/bento_sts/main/routes.py
--rw-r--r--   0        0        0    11389 2023-07-10 00:51:42.244256 bento_sts-0.1.0/src/bento_sts/mdb.py
--rw-r--r--   0        0        0    13167 2023-07-07 02:01:31.473919 bento_sts-0.1.0/src/bento_sts/mdb_tags.py
--rw-r--r--   0        0        0    14611 2023-07-07 02:01:31.473005 bento_sts-0.1.0/src/bento_sts/mdb_update.py
--rw-r--r--   0        0        0      673 2023-07-07 02:01:31.472418 bento_sts-0.1.0/src/bento_sts/static/loading.gif
--rw-r--r--   0        0        0      282 2023-07-07 02:01:31.471927 bento_sts-0.1.0/src/bento_sts/static/sts.css
--rw-r--r--   0        0        0     1892 2023-07-09 20:15:02.823333 bento_sts-0.1.0/src/bento_sts/sts.py
--rw-r--r--   0        0        0     4422 2023-07-07 02:01:31.470911 bento_sts-0.1.0/src/bento_sts/templates/_intro.html
--rw-r--r--   0        0        0      175 2023-07-07 02:01:31.470494 bento_sts-0.1.0/src/bento_sts/templates/about-mdb.html
--rw-r--r--   0        0        0     1083 2023-07-09 20:12:17.632256 bento_sts-0.1.0/src/bento_sts/templates/about-sts.html
--rw-r--r--   0        0        0     3920 2023-07-09 20:16:17.668929 bento_sts-0.1.0/src/bento_sts/templates/base.html
--rw-r--r--   0        0        0      188 2023-07-07 02:01:31.468445 bento_sts-0.1.0/src/bento_sts/templates/errors/400.html
--rw-r--r--   0        0        0      163 2023-07-07 02:01:31.467946 bento_sts-0.1.0/src/bento_sts/templates/errors/404.html
--rw-r--r--   0        0        0      234 2023-07-07 02:01:31.467192 bento_sts-0.1.0/src/bento_sts/templates/errors/500.html
--rw-r--r--   0        0        0      756 2023-07-09 20:12:27.105105 bento_sts-0.1.0/src/bento_sts/templates/explore.html
--rw-r--r--   0        0        0     2132 2023-07-09 20:11:04.493347 bento_sts-0.1.0/src/bento_sts/templates/index.html
--rw-r--r--   0        0        0     1172 2023-07-09 20:12:08.555392 bento_sts-0.1.0/src/bento_sts/templates/mdb-model.html
--rw-r--r--   0        0        0     1422 2023-07-09 20:11:41.928393 bento_sts-0.1.0/src/bento_sts/templates/mdb-node-list.html
--rw-r--r--   0        0        0     3524 2023-07-07 02:01:31.463259 bento_sts-0.1.0/src/bento_sts/templates/mdb-node.html
--rw-r--r--   0        0        0      602 2023-07-07 02:01:31.462192 bento_sts-0.1.0/src/bento_sts/templates/mdb-origin.html
--rw-r--r--   0        0        0     3532 2023-07-07 02:01:31.461399 bento_sts-0.1.0/src/bento_sts/templates/mdb-property.html
--rw-r--r--   0        0        0     1611 2023-07-07 02:01:31.460557 bento_sts-0.1.0/src/bento_sts/templates/mdb-tag.html
--rw-r--r--   0        0        0     1745 2023-07-07 02:01:31.459307 bento_sts-0.1.0/src/bento_sts/templates/mdb-term.html
--rw-r--r--   0        0        0     1789 2023-07-09 20:12:03.737714 bento_sts-0.1.0/src/bento_sts/templates/mdb-valueset.html
--rw-r--r--   0        0        0     4004 2023-07-09 20:10:58.458009 bento_sts-0.1.0/src/bento_sts/templates/mdb.html
--rw-r--r--   0        0        0     2589 2023-07-09 20:12:31.308854 bento_sts-0.1.0/src/bento_sts/templates/reports.html
--rw-r--r--   0        0        0     1872 2023-07-07 02:01:31.455624 bento_sts-0.1.0/src/bento_sts/templates/search.html
--rw-r--r--   0        0        0      495 2023-07-09 20:12:22.063962 bento_sts-0.1.0/src/bento_sts/templates/version-history-report.html
--rw-r--r--   0        0        0      500 2023-07-09 20:12:13.305029 bento_sts-0.1.0/src/bento_sts/templates/version-history.html
--rw-r--r--   0        0        0      204 2023-07-07 02:01:31.454103 bento_sts-0.1.0/src/bento_sts/util.py
--rw-r--r--   0        0        0    10852 2023-07-07 02:01:31.309361 bento_sts-0.1.0/swagger/nodejs-server-server-generated.zip
--rw-r--r--   0        0        0    18747 2022-02-13 00:11:34.563708 bento_sts-0.1.0/swagger/pysts-api.yaml
--rw-r--r--   0        0        0      885 2023-07-07 02:01:31.310135 bento_sts-0.1.0/swagger/python-flask-server/.dockerignore
--rw-r--r--   0        0        0      786 2023-07-07 02:01:31.310787 bento_sts-0.1.0/swagger/python-flask-server/.gitignore
--rw-r--r--   0        0        0        6 2023-07-07 02:01:31.312195 bento_sts-0.1.0/swagger/python-flask-server/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     1030 2023-07-07 02:01:31.311497 bento_sts-0.1.0/swagger/python-flask-server/.swagger-codegen-ignore
--rw-r--r--   0        0        0      246 2023-07-07 02:01:31.313276 bento_sts-0.1.0/swagger/python-flask-server/Dockerfile
--rw-r--r--   0        0        0     1115 2023-07-14 01:07:14.515754 bento_sts-0.1.0/swagger/python-flask-server/README.md
--rw-r--r--   0        0        0     1628 2023-07-07 02:01:31.314846 bento_sts-0.1.0/swagger/python-flask-server/git_push.sh
--rw-r--r--   0        0        0       65 2023-07-14 01:15:29.318240 bento_sts-0.1.0/swagger/python-flask-server/requirements.txt
--rw-r--r--   0        0        0     1253 2023-07-07 02:01:31.315777 bento_sts-0.1.0/swagger/python-flask-server/setup.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.315951 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/__init__.py
--rw-r--r--   0        0        0      353 2023-07-07 02:01:31.316657 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.316976 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      346 2023-07-07 02:01:31.318229 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/id_controller.py
--rw-r--r--   0        0        0     5910 2023-07-07 02:01:31.319216 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/model_controller.py
--rw-r--r--   0        0        0      426 2023-07-07 02:01:31.320206 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/models_controller.py
--rw-r--r--   0        0        0     1081 2023-07-07 02:01:31.321098 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/tag_controller.py
--rw-r--r--   0        0        0      356 2023-07-07 02:01:31.321801 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/tags_controller.py
--rw-r--r--   0        0        0      608 2023-07-07 02:01:31.322521 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/encoder.py
--rw-r--r--   0        0        0      393 2023-07-07 02:01:31.323225 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-07 02:01:31.323881 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     2291 2023-07-07 02:01:31.324334 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/entity.py
--rw-r--r--   0        0        0     3551 2023-07-07 02:01:31.324767 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/model.py
--rw-r--r--   0        0        0     6112 2023-07-07 02:01:31.325214 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/model_property.py
--rw-r--r--   0        0        0     2978 2023-07-07 02:01:31.325734 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/node.py
--rw-r--r--   0        0        0     2885 2023-07-07 02:01:31.326336 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/tag.py
--rw-r--r--   0        0        0     4604 2023-07-07 02:01:31.326925 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/term.py
--rw-r--r--   0        0        0    21512 2023-07-07 02:01:31.327834 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      415 2023-07-07 02:01:31.328553 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/__init__.py
--rw-r--r--   0        0        0      716 2023-07-07 02:01:31.329053 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_id_controller.py
--rw-r--r--   0        0        0     5798 2023-07-07 02:01:31.329691 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_model_controller.py
--rw-r--r--   0        0        0     1029 2023-07-07 02:01:31.330310 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_models_controller.py
--rw-r--r--   0        0        0     1688 2023-07-07 02:01:31.331002 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_tag_controller.py
--rw-r--r--   0        0        0      952 2023-07-07 02:01:31.331519 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_tags_controller.py
--rw-r--r--   0        0        0     3384 2023-07-07 02:01:31.332007 bento_sts-0.1.0/swagger/python-flask-server/swagger_server/util.py
--rw-r--r--   0        0        0       90 2023-07-07 02:01:31.332560 bento_sts-0.1.0/swagger/python-flask-server/test-requirements.txt
--rw-r--r--   0        0        0      143 2023-07-07 02:01:31.333171 bento_sts-0.1.0/swagger/python-flask-server/tox.ini
--rw-r--r--   0        0        0      584 2023-07-07 02:01:31.451313 bento_sts-0.1.0/sysd/sts.service
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bento_sts-0.1.0/setup.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 bento_sts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-10-19 17:56:24.008960 bento_sts-0.1.1/LICENSE
+-rw-r--r--   0        0        0      415 2023-07-08 22:03:48.092764 bento_sts-0.1.1/README.md
+-rw-r--r--   0        0        0     1908 2023-07-19 14:03:32.194118 bento_sts-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-09 19:32:46.361891 bento_sts-0.1.1/src/bento_sts/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-09 19:16:57.363182 bento_sts-0.1.1/src/bento_sts/api/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-09 19:39:48.617466 bento_sts-0.1.1/src/bento_sts/api/routes.py
+-rw-r--r--   0        0        0       28 2023-07-07 02:01:31.478631 bento_sts-0.1.1/src/bento_sts/cli.py
+-rw-r--r--   0        0        0      855 2023-07-09 20:05:36.333841 bento_sts-0.1.1/src/bento_sts/config.py
+-rw-r--r--   0        0        0        0 2022-02-25 02:56:46.496832 bento_sts-0.1.1/src/bento_sts/config_sts/__init__.py
+-rw-r--r--   0        0        0     5687 2022-02-25 02:56:46.497407 bento_sts-0.1.1/src/bento_sts/config_sts/query_paths.yml
+-rw-r--r--   0        0        0       82 2023-07-09 19:34:07.790210 bento_sts-0.1.1/src/bento_sts/errors/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-09 20:07:09.565949 bento_sts-0.1.1/src/bento_sts/errors/handlers.py
+-rw-r--r--   0        0        0       87 2023-07-09 19:16:54.204908 bento_sts-0.1.1/src/bento_sts/main/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-07 02:01:31.476646 bento_sts-0.1.1/src/bento_sts/main/forms.py
+-rw-r--r--   0        0        0    10631 2023-07-19 13:57:43.363802 bento_sts-0.1.1/src/bento_sts/main/routes.py
+-rw-r--r--   0        0        0    11492 2023-07-19 01:58:03.297841 bento_sts-0.1.1/src/bento_sts/mdb.py
+-rw-r--r--   0        0        0    13185 2023-07-19 14:00:20.242576 bento_sts-0.1.1/src/bento_sts/mdb_tags.py
+-rw-r--r--   0        0        0    14611 2023-07-07 02:01:31.473005 bento_sts-0.1.1/src/bento_sts/mdb_update.py
+-rw-r--r--   0        0        0      673 2023-07-07 02:01:31.472418 bento_sts-0.1.1/src/bento_sts/static/loading.gif
+-rw-r--r--   0        0        0      282 2023-07-07 02:01:31.471927 bento_sts-0.1.1/src/bento_sts/static/sts.css
+-rw-r--r--   0        0        0     1892 2023-07-09 20:15:02.823333 bento_sts-0.1.1/src/bento_sts/sts.py
+-rw-r--r--   0        0        0     4422 2023-07-07 02:01:31.470911 bento_sts-0.1.1/src/bento_sts/templates/_intro.html
+-rw-r--r--   0        0        0      175 2023-07-07 02:01:31.470494 bento_sts-0.1.1/src/bento_sts/templates/about-mdb.html
+-rw-r--r--   0        0        0     1083 2023-07-09 20:12:17.632256 bento_sts-0.1.1/src/bento_sts/templates/about-sts.html
+-rw-r--r--   0        0        0     3920 2023-07-09 20:16:17.668929 bento_sts-0.1.1/src/bento_sts/templates/base.html
+-rw-r--r--   0        0        0      188 2023-07-07 02:01:31.468445 bento_sts-0.1.1/src/bento_sts/templates/errors/400.html
+-rw-r--r--   0        0        0      163 2023-07-07 02:01:31.467946 bento_sts-0.1.1/src/bento_sts/templates/errors/404.html
+-rw-r--r--   0        0        0      234 2023-07-07 02:01:31.467192 bento_sts-0.1.1/src/bento_sts/templates/errors/500.html
+-rw-r--r--   0        0        0      756 2023-07-09 20:12:27.105105 bento_sts-0.1.1/src/bento_sts/templates/explore.html
+-rw-r--r--   0        0        0     2132 2023-07-09 20:11:04.493347 bento_sts-0.1.1/src/bento_sts/templates/index.html
+-rw-r--r--   0        0        0     1172 2023-07-09 20:12:08.555392 bento_sts-0.1.1/src/bento_sts/templates/mdb-model.html
+-rw-r--r--   0        0        0     1422 2023-07-09 20:11:41.928393 bento_sts-0.1.1/src/bento_sts/templates/mdb-node-list.html
+-rw-r--r--   0        0        0     3524 2023-07-07 02:01:31.463259 bento_sts-0.1.1/src/bento_sts/templates/mdb-node.html
+-rw-r--r--   0        0        0      602 2023-07-07 02:01:31.462192 bento_sts-0.1.1/src/bento_sts/templates/mdb-origin.html
+-rw-r--r--   0        0        0     3532 2023-07-07 02:01:31.461399 bento_sts-0.1.1/src/bento_sts/templates/mdb-property.html
+-rw-r--r--   0        0        0     1611 2023-07-07 02:01:31.460557 bento_sts-0.1.1/src/bento_sts/templates/mdb-tag.html
+-rw-r--r--   0        0        0     1745 2023-07-07 02:01:31.459307 bento_sts-0.1.1/src/bento_sts/templates/mdb-term.html
+-rw-r--r--   0        0        0     1789 2023-07-09 20:12:03.737714 bento_sts-0.1.1/src/bento_sts/templates/mdb-valueset.html
+-rw-r--r--   0        0        0     4004 2023-07-09 20:10:58.458009 bento_sts-0.1.1/src/bento_sts/templates/mdb.html
+-rw-r--r--   0        0        0     2589 2023-07-09 20:12:31.308854 bento_sts-0.1.1/src/bento_sts/templates/reports.html
+-rw-r--r--   0        0        0     1872 2023-07-07 02:01:31.455624 bento_sts-0.1.1/src/bento_sts/templates/search.html
+-rw-r--r--   0        0        0      495 2023-07-09 20:12:22.063962 bento_sts-0.1.1/src/bento_sts/templates/version-history-report.html
+-rw-r--r--   0        0        0      500 2023-07-09 20:12:13.305029 bento_sts-0.1.1/src/bento_sts/templates/version-history.html
+-rw-r--r--   0        0        0      204 2023-07-07 02:01:31.454103 bento_sts-0.1.1/src/bento_sts/util.py
+-rw-r--r--   0        0        0    10852 2023-07-07 02:01:31.309361 bento_sts-0.1.1/swagger/nodejs-server-server-generated.zip
+-rw-r--r--   0        0        0    18715 2023-07-18 16:42:04.940479 bento_sts-0.1.1/swagger/pysts-api.yaml
+-rw-r--r--   0        0        0      885 2023-07-07 02:01:31.310135 bento_sts-0.1.1/swagger/python-flask-server/.dockerignore
+-rw-r--r--   0        0        0      786 2023-07-07 02:01:31.310787 bento_sts-0.1.1/swagger/python-flask-server/.gitignore
+-rw-r--r--   0        0        0        6 2023-07-07 02:01:31.312195 bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     1030 2023-07-07 02:01:31.311497 bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen-ignore
+-rw-r--r--   0        0        0      246 2023-07-07 02:01:31.313276 bento_sts-0.1.1/swagger/python-flask-server/Dockerfile
+-rw-r--r--   0        0        0     1115 2023-07-14 01:07:14.515754 bento_sts-0.1.1/swagger/python-flask-server/README.md
+-rw-r--r--   0        0        0     1628 2023-07-07 02:01:31.314846 bento_sts-0.1.1/swagger/python-flask-server/git_push.sh
+-rw-r--r--   0        0        0       65 2023-07-14 01:15:29.318240 bento_sts-0.1.1/swagger/python-flask-server/requirements.txt
+-rw-r--r--   0        0        0     1253 2023-07-07 02:01:31.315777 bento_sts-0.1.1/swagger/python-flask-server/setup.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:01:31.315951 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-07 02:01:31.316657 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:01:31.316976 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-07 02:01:31.318229 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/id_controller.py
+-rw-r--r--   0        0        0     5910 2023-07-07 02:01:31.319216 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/model_controller.py
+-rw-r--r--   0        0        0      426 2023-07-07 02:01:31.320206 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/models_controller.py
+-rw-r--r--   0        0        0     1081 2023-07-07 02:01:31.321098 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tag_controller.py
+-rw-r--r--   0        0        0      356 2023-07-07 02:01:31.321801 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tags_controller.py
+-rw-r--r--   0        0        0      608 2023-07-07 02:01:31.322521 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/encoder.py
+-rw-r--r--   0        0        0      393 2023-07-07 02:01:31.323225 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-07 02:01:31.323881 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     2291 2023-07-07 02:01:31.324334 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/entity.py
+-rw-r--r--   0        0        0     3551 2023-07-07 02:01:31.324767 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model.py
+-rw-r--r--   0        0        0     6112 2023-07-07 02:01:31.325214 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model_property.py
+-rw-r--r--   0        0        0     2978 2023-07-07 02:01:31.325734 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/node.py
+-rw-r--r--   0        0        0     2885 2023-07-07 02:01:31.326336 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/tag.py
+-rw-r--r--   0        0        0     4604 2023-07-07 02:01:31.326925 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/term.py
+-rw-r--r--   0        0        0    21512 2023-07-07 02:01:31.327834 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      415 2023-07-07 02:01:31.328553 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-07 02:01:31.329053 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_id_controller.py
+-rw-r--r--   0        0        0     5798 2023-07-07 02:01:31.329691 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_model_controller.py
+-rw-r--r--   0        0        0     1029 2023-07-07 02:01:31.330310 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_models_controller.py
+-rw-r--r--   0        0        0     1688 2023-07-07 02:01:31.331002 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tag_controller.py
+-rw-r--r--   0        0        0      952 2023-07-07 02:01:31.331519 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tags_controller.py
+-rw-r--r--   0        0        0     3384 2023-07-07 02:01:31.332007 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/util.py
+-rw-r--r--   0        0        0       90 2023-07-07 02:01:31.332560 bento_sts-0.1.1/swagger/python-flask-server/test-requirements.txt
+-rw-r--r--   0        0        0      143 2023-07-07 02:01:31.333171 bento_sts-0.1.1/swagger/python-flask-server/tox.ini
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bento_sts-0.1.1/setup.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 bento_sts-0.1.1/PKG-INFO
```

### Comparing `bento_sts-0.1.0/LICENSE` & `bento_sts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/pyproject.toml` & `bento_sts-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-sts"
-version = "0.1.0"
+version = "0.1.1"
 author = "Mark Benson"
 author_email = "mark.benson@nih.gov"
 maintainer = "Mark A. Jensen"
 maintainer_email = "mark.jensen@nih.gov"
 description = "Bento Simple Terminology Server"
 requires-python = ">=3.8"
 classifiers = [
@@ -19,23 +19,23 @@
 #[options]
 #    package_dir =
 #        = app
 #    packages = find:
 
 [tool.poetry]
 name = "bento-sts"
-version = "0.1.0"
+version = "0.1.1"
 description = "Bento Simple Terminology Server"
 authors = [
 	"Mark Benson <mark.benson@nih.gov>",
 	"Mark A. Jensen <mark.jensen@nih.gov>",
 ]
 license = "Apache 2.0"
 readme = "README.md"
-include = ["swagger", "nginx","sysd"]
+include = ["swagger"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 bento-meta = ">=0.0.32"
 importlib_resources = ">=5.4.0"
 Flask-WTF =  ">=0.14.3"
 Bootstrap-Flask =  ">=1.5.2"
```

### Comparing `bento_sts-0.1.0/src/bento_sts/api/routes.py` & `bento_sts-0.1.1/src/bento_sts/api/routes.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/config.py` & `bento_sts-0.1.1/src/bento_sts/config.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/config_sts/query_paths.yml` & `bento_sts-0.1.1/src/bento_sts/config_sts/query_paths.yml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/main/forms.py` & `bento_sts-0.1.1/src/bento_sts/main/forms.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/main/routes.py` & `bento_sts-0.1.1/src/bento_sts/main/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,16 +270,17 @@
     if format == 'json':
         return jsonify(ents)
 
     pg_tot = 0
     if thing == "terms":
         pg_tot = len(ents)
     elif thing == "models":
-        pg_tot = max(len(ents["nodes"]), len(ents["properties"]),
-                     len(ents["relationships"]))
+        if ents:
+            pg_tot = max(len(ents["nodes"]), len(ents["properties"]),
+                         len(ents["relationships"]))
     else:
         pass
     pagination = Pagination(
         page=request.args.get("page", 1, type=int),
         record_name="Hits",
         total=pg_tot,
         per_page=current_app.config["HITS_PER_PAGE"],
```

### Comparing `bento_sts-0.1.0/src/bento_sts/mdb.py` & `bento_sts-0.1.1/src/bento_sts/mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,33 +73,34 @@
                     "link": url_for("main.entities", entities='properties',
                                     id=p["nanoid"]),
                     "value_domain": p["value_domain"]
                     })
         if (edges_result):
             for e in edges_result:
                 node = e["far_node"]
-                rln = e["rln"]
-                add_to = None
-                if e["far_type"] == "has_src":
-                    add_to = from_nodes
-                elif e["far_type"] == "has_dst":
-                    add_to = to_nodes
-                else:
-                    RuntimeError("What?")
-                add_to[node["nanoid"]] = {
-                    "id": node["nanoid"],
-                    "handle": node["handle"],
-                    "link": url_for("main.entities", entities='nodes',
-                                    id=node["nanoid"]),
-                    "type": "node",
-                    "relationship": {
-                        "id": rln["nanoid"],
-                        "handle": rln["handle"],
-                        "link": "/relationships/{}".format(rln["nanoid"]),
-                        "type": "relationship"
+                if (node):
+                    rln = e["rln"]
+                    add_to = None
+                    if e["far_type"] == "has_src":
+                        add_to = from_nodes
+                    elif e["far_type"] == "has_dst":
+                        add_to = to_nodes
+                    else:
+                        RuntimeError("What?")
+                    add_to[node["nanoid"]] = {
+                        "id": node["nanoid"],
+                        "handle": node["handle"],
+                        "link": url_for("main.entities", entities='nodes',
+                                        id=node["nanoid"]),
+                        "type": "node",
+                        "relationship": {
+                            "id": rln["nanoid"],
+                            "handle": rln["handle"],
+                            "link": "/relationships/{}".format(rln["nanoid"]),
+                            "type": "relationship"
                         }
                     }
             result["has_relationship_to_nodes"].extend(to_nodes.values())
             result["has_relationship_from_nodes"].extend(from_nodes.values())
         return result
 
     # ----------------------------------------------------------------------- #
```

### Comparing `bento_sts-0.1.0/src/bento_sts/mdb_tags.py` & `bento_sts-0.1.1/src/bento_sts/mdb_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
         current_app.logger.warn('yup... using model {}'.format(model))
 
         query_against_all_models = """
                 MATCH (n:node) -[:has_property]->(p:property)-[:has_tag]->(t:tag)
                 WHERE n._to IS NULL 
                 AND   p._to IS NULL
-                RETURN n.handle, n.nanoid, p.handle, p.nanoid, t.key, t.value;
+                RETURN distinct n.handle, n.nanoid, p.handle, p.nanoid, t.key, t.value;
                 """
         query_against_specific_model = """
                 MATCH (n:node) -[:has_property]->(p:property)-[:has_tag]->(t:tag)
                 WHERE n._to IS NULL 
                 AND   p._to IS NULL
                 WHERE toLower(n.model) = toLower($model)
-                RETURN n.handle, n.nanoid, p.handle, p.nanoid, t.key, t.value;
+                RETURN distinct n.handle, n.nanoid, p.handle, p.nanoid, t.key, t.value;
                 """
 
         db_records = None
         if model is None:
             db_records = tx.run(query_against_all_models,)
             current_app.logger.warn(' point 2 ... using model {}'.format(model))
         else:
```

### Comparing `bento_sts-0.1.0/src/bento_sts/mdb_update.py` & `bento_sts-0.1.1/src/bento_sts/mdb_update.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/static/loading.gif` & `bento_sts-0.1.1/src/bento_sts/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/sts.py` & `bento_sts-0.1.1/src/bento_sts/sts.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/_intro.html` & `bento_sts-0.1.1/src/bento_sts/templates/_intro.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/about-sts.html` & `bento_sts-0.1.1/src/bento_sts/templates/about-sts.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/base.html` & `bento_sts-0.1.1/src/bento_sts/templates/base.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/explore.html` & `bento_sts-0.1.1/src/bento_sts/templates/explore.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/index.html` & `bento_sts-0.1.1/src/bento_sts/templates/index.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-model.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-model.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-node-list.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-node-list.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-node.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-node.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-origin.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-origin.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-property.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-property.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-tag.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-tag.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-term.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-term.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb-valueset.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb-valueset.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/mdb.html` & `bento_sts-0.1.1/src/bento_sts/templates/mdb.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/reports.html` & `bento_sts-0.1.1/src/bento_sts/templates/reports.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/src/bento_sts/templates/search.html` & `bento_sts-0.1.1/src/bento_sts/templates/search.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/nodejs-server-server-generated.zip` & `bento_sts-0.1.1/swagger/nodejs-server-server-generated.zip`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/pysts-api.yaml` & `bento_sts-0.1.1/swagger/pysts-api.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -697,11 +697,7 @@
         type: string
       nanoid:
         type: string
     required:
       - key
       - value
       - nanoid
-        
-    
-        
-
```

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/.dockerignore` & `bento_sts-0.1.1/swagger/python-flask-server/.dockerignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/.gitignore` & `bento_sts-0.1.1/swagger/python-flask-server/.gitignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/.swagger-codegen-ignore` & `bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/README.md` & `bento_sts-0.1.1/swagger/python-flask-server/README.md`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/git_push.sh` & `bento_sts-0.1.1/swagger/python-flask-server/git_push.sh`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/setup.py` & `bento_sts-0.1.1/swagger/python-flask-server/setup.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/model_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/controllers/tag_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/encoder.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/base_model_.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/entity.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/entity.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/model.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/model_property.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model_property.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/node.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/node.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/tag.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/tag.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/models/term.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/term.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/swagger/swagger.yaml` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/swagger/swagger.yaml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_id_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_id_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_model_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_models_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_models_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_tag_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/test/test_tags_controller.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tags_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/swagger/python-flask-server/swagger_server/util.py` & `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.0/setup.py` & `bento_sts-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'requests>=2.20.0',
  'six>=1.15.0',
  'urllib3>=1.26.5',
  'visitor>=0.1.3']
 
 setup_kwargs = {
     'name': 'bento-sts',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Bento Simple Terminology Server',
     'long_description': '# Welcome to bento-sts\n\nThis is a flask-based implementation of the Simple Terminology Service (STS) for the Bento Metadatabase (MDB).\n\n## Install\n\n\t$ git clone https://github.com/CBIIT/bento-sts.git\n\t$ cd pysts\n\t$ virtualenv sts-venv\n\t$ source sts-venv/bin/activate\n\t$ pip install -r requirements.txt\n\t$ flask run\n\n## Dependencies\n\n`bento-sts` requires a Neo4j-based [MDB](https://github.com/CBIIT/bento-meta).\n\n\n\n',
     'author': 'Mark Benson',
     'author_email': 'mark.benson@nih.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bento_sts-0.1.0/PKG-INFO` & `bento_sts-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-sts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bento Simple Terminology Server
 License: Apache 2.0
 Author: Mark Benson
 Author-email: mark.benson@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

