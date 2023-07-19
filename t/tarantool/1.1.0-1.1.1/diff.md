# Comparing `tmp/tarantool-1.1.0.tar.gz` & `tmp/tarantool-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarantool-1.1.0.tar", last modified: Fri Jun 30 09:38:46 2023, max compression
+gzip compressed data, was "tarantool-1.1.1.tar", last modified: Wed Jul 19 14:29:36 2023, max compression
```

## Comparing `tarantool-1.1.0.tar` & `tarantool-1.1.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-30 09:38:29.000000 tarantool-1.1.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-30 09:38:29.000000 tarantool-1.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/scripts/remove_source_code.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)    15987 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/packing.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/reusable_testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12038 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-30 09:38:29.000000 tarantool-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-30 09:38:29.000000 tarantool-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-30 09:38:29.000000 tarantool-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-30 09:38:29.000000 tarantool-1.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-30 09:38:29.000000 tarantool-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-30 09:38:29.000000 tarantool-1.1.0/INSTALL
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-06-30 09:38:29.000000 tarantool-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-30 09:38:29.000000 tarantool-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-30 09:38:29.000000 tarantool-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-06-30 09:38:46.814899 tarantool-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-06-30 09:38:29.000000 tarantool-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-30 09:38:29.000000 tarantool-1.1.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/debian/
--rw-r--r--   0 runner    (1001) docker     (122)    27953 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        3 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/compat
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)      517 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/debian/source/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/source/options
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.798899 tarantool-1.1.0/docs/source/_static/favicon/
--rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (122)    14138 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (122)     5571 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-76x76.png
--rwxr-xr-x   0 runner    (1001) docker     (122)      266 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/generate-png.sh
--rw-r--r--   0 runner    (1001) docker     (122)    11989 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)    21876 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-196x196.png
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     7747 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.802899 tarantool-1.1.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/module-tarantool.rst
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-connection-pool.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-connection.rst
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-crud.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-dbapi.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-error.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-mesh-connection.rst
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-msgpack-ext-types.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-msgpack-ext.rst
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-request.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-response.rst
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-schema.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-space.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-types.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-utils.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10929 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/dev-guide.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    14953 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/quick-start.rst
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-30 09:38:29.000000 tarantool-1.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-30 09:38:29.000000 tarantool-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/rpm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.802899 tarantool-1.1.0/rpm/SPECS/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-30 09:38:29.000000 tarantool-1.1.0/rpm/SPECS/python-tarantool.spec
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 09:38:46.814899 tarantool-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     3136 2023-06-30 09:38:29.000000 tarantool-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/
--rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   105958 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    56825 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/crud.py
--rw-r--r--   0 runner    (1001) docker     (122)    12894 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    20552 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/error.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/mesh_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10336 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/packer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/types/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26310 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     6527 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2254 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh
--rw-r--r--   0 runner    (1001) docker     (122)    48588 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/timezones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/unpacker.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)    17713 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/request.py
--rw-r--r--   0 runner    (1001) docker     (122)    10967 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/response.py
--rw-r--r--   0 runner    (1001) docker     (122)    13804 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/space.py
--rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.810899 tarantool-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.810899 tarantool-1.1.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/ca.crt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/empty
--rwxr-xr-x   0 runner    (1001) docker     (122)     1702 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/generate.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/invalidhost.crt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/invalidpasswords
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.crt
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.enc.key
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.key
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/passwords
--rwxr-xr-x   0 runner    (1001) docker     (122)     1176 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/setup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/test/suites/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/box.lua
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/crud_server.lua
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/test/suites/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/remote_tarantool_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     9432 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/skip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_python_ci.lua
--rw-r--r--   0 runner    (1001) docker     (122)    11383 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (122)    30563 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    19668 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)    19641 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_dml.py
--rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_error_ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     6153 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)     8583 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_reconnect.py
--rw-r--r--   0 runner    (1001) docker     (122)    26049 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    33077 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.836157 tarantool-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-19 14:29:27.000000 tarantool-1.1.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-19 14:29:27.000000 tarantool-1.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-07-19 14:29:27.000000 tarantool-1.1.1/.github/scripts/remove_source_code.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)    15987 2023-07-19 14:29:27.000000 tarantool-1.1.1/.github/workflows/packing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-19 14:29:27.000000 tarantool-1.1.1/.github/workflows/reusable_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12038 2023-07-19 14:29:27.000000 tarantool-1.1.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-19 14:29:27.000000 tarantool-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-07-19 14:29:27.000000 tarantool-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-19 14:29:27.000000 tarantool-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-07-19 14:29:27.000000 tarantool-1.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    15037 2023-07-19 14:29:27.000000 tarantool-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-19 14:29:27.000000 tarantool-1.1.1/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-07-19 14:29:27.000000 tarantool-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-19 14:29:27.000000 tarantool-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-19 14:29:27.000000 tarantool-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-07-19 14:29:36.836157 tarantool-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-07-19 14:29:27.000000 tarantool-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-19 14:29:27.000000 tarantool-1.1.1/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)    28565 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (122)      517 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-19 14:29:27.000000 tarantool-1.1.1/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.828158 tarantool-1.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.828158 tarantool-1.1.1/docs/source/_static/favicon/
+-rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14138 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5571 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-76x76.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)      266 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/generate-png.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    11989 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21876 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon-196x196.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7747 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/_static/favicon/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.828158 tarantool-1.1.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/module-tarantool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-connection-pool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-crud.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-dbapi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-error.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-mesh-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-msgpack-ext-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-msgpack-ext.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-request.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-response.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-schema.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-space.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/api/submodule-utils.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10929 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14953 2023-07-19 14:29:27.000000 tarantool-1.1.1/docs/source/quick-start.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-19 14:29:27.000000 tarantool-1.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-19 14:29:27.000000 tarantool-1.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.824157 tarantool-1.1.1/rpm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.828158 tarantool-1.1.1/rpm/SPECS/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-19 14:29:27.000000 tarantool-1.1.1/rpm/SPECS/python-tarantool.spec
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 14:29:36.836157 tarantool-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3136 2023-07-19 14:29:27.000000 tarantool-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.828158 tarantool-1.1.1/tarantool/
+-rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105958 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56825 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12894 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20552 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/mesh_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/tarantool/msgpack_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10336 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/packer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/tarantool/msgpack_ext/types/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26310 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8271 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2254 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/gen-timezones.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    48588 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/unpacker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/msgpack_ext/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17713 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10967 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13804 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/space.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-07-19 14:29:27.000000 tarantool-1.1.1/tarantool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/tarantool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-07-19 14:29:36.000000 tarantool-1.1.1/tarantool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-07-19 14:29:36.000000 tarantool-1.1.1/tarantool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 14:29:36.000000 tarantool-1.1.1/tarantool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-19 14:29:36.000000 tarantool-1.1.1/tarantool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-19 14:29:36.000000 tarantool-1.1.1/tarantool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.832157 tarantool-1.1.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/empty
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1702 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/invalidhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/invalidpasswords
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/localhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/localhost.enc.key
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/localhost.key
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/data/passwords
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1176 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/setup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.836157 tarantool-1.1.1/test/suites/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/box.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/crud_server.lua
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:36.836157 tarantool-1.1.1/test/suites/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/remote_tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9432 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/skip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/tarantool_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/tarantool_python_ci.lua
+-rw-r--r--   0 runner    (1001) docker     (122)    11383 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/lib/tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30851 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19668 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19645 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_dml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_error_ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37698 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6153 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8583 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_reconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26049 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33077 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-07-19 14:29:27.000000 tarantool-1.1.1/test/suites/test_uuid.py
```

### Comparing `tarantool-1.1.0/.github/workflows/packing.yml` & `tarantool-1.1.1/.github/workflows/packing.yml`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/.github/workflows/reusable_testing.yml` & `tarantool-1.1.1/.github/workflows/reusable_testing.yml`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/.github/workflows/testing.yml` & `tarantool-1.1.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/.gitignore` & `tarantool-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/AUTHORS` & `tarantool-1.1.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/CHANGELOG.md` & `tarantool-1.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.1 - 2023-07-19
+
+### Changed
+- Validate `tarantool.Interval` limits with the same rules as in Tarantool (PR #302).
+
+### Fixed
+- `tarantool.Interval` arithmetic with weeks (PR #302).
+- `tarantool.Interval` weeks display in `str()` and `repr()` (PR #302).
+
 ## 1.1.0 - 2023-06-30
 
 ### Added
 - Allow to require specific server protocol version and features (#267).
 
 ### Changed
 - Drop `msgpack-python` support. Use `msgpack` instead.
@@ -194,15 +203,15 @@
 - Backport ConnectionPool support for Python 3.6.
 - Support extra information for iproto errors (#232).
 - Error extension type support (#232).
 
 - Support pandas way to build datetime from timestamp (PR #252).
 
   `timestamp_since_utc_epoch` is a parameter to set timestamp
-  convertion behavior for timezone-aware datetimes.
+  conversion behavior for timezone-aware datetimes.
 
   If ``False`` (default), behaves similar to Tarantool `datetime.new()`:
 
   ```python
   >>> dt = tarantool.Datetime(timestamp=1640995200, timestamp_since_utc_epoch=False)
   >>> dt
   datetime: Timestamp('2022-01-01 00:00:00'), tz: ""
@@ -214,15 +223,15 @@
   datetime: Timestamp('2022-01-01 00:00:00+0300', tz='Europe/Moscow'), tz: "Europe/Moscow"
   >>> dt.timestamp
   1640984400.0
   ```
 
   Thus, if ``False``, datetime is computed from timestamp
   since epoch and then timezone is applied without any
-  convertion. In that case, `dt.timestamp` won't be equal to
+  conversion. In that case, `dt.timestamp` won't be equal to
   initialization `timestamp` for all timezones with non-zero offset.
 
   If ``True``, behaves similar to `pandas.Timestamp`:
 
   ```python
   >>> dt = tarantool.Datetime(timestamp=1640995200, timestamp_since_utc_epoch=True)
   >>> dt
```

### Comparing `tarantool-1.1.0/LICENSE` & `tarantool-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/Makefile` & `tarantool-1.1.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .PHONY: install
 install:
 	pip3 install --editable .
 
 
 PYTHON_FILES=tarantool test setup.py docs/source/conf.py
-TEXT_FILES=README.rst docs/source/*.rst
+TEXT_FILES=README.rst CHANGELOG.md docs/source/*.rst
 .PHONY: lint
 lint:
 	python3 -m pylint --recursive=y $(PYTHON_FILES)
 	python3 -m flake8 $(PYTHON_FILES)
 	codespell $(PYTHON_FILES) $(TEXT_FILES)
```

### Comparing `tarantool-1.1.0/PKG-INFO` & `tarantool-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarantool
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client library for Tarantool
 Home-page: https://github.com/tarantool/tarantool-python
 Author: tarantool-python AUTHORS
 Author-email: admin@tarantool.org
 License: BSD
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `tarantool-1.1.0/README.rst` & `tarantool-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/debian/changelog` & `tarantool-1.1.1/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+python3-tarantool (1.1.1-0) unstable; urgency=medium
+
+    ## Overview
+
+    This release introduces various datetime interval fixes and quality of life
+    improvements.
+
+    ## Breaking changes
+    - Forbid to create datetime intervals out of Tarantool limits (PR #302).
+
+    ## Changed
+    - Validate `tarantool.Interval` limits with the same rules as in Tarantool (PR #302).
+
+    ## Fixed
+    - `tarantool.Interval` arithmetic with weeks (PR #302).
+    - `tarantool.Interval` weeks display in `str()` and `repr()` (PR #302).
+
+ -- Georgy Moiseev <georgy.moiseev@tarantool.org>  Wed, 19 Jul 2023 18:00:00 +0300
+
 python3-tarantool (1.1.0-0) unstable; urgency=medium
 
     ## Overview
 
     This release introduces API to request server protocol version and
     feature, as well as introduce decimal bugfix.
```

### Comparing `tarantool-1.1.0/debian/control` & `tarantool-1.1.1/debian/control`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/debian/rules` & `tarantool-1.1.1/debian/rules`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-114x114.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-120x120.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-144x144.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-152x152.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-57x57.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-60x60.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-72x72.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-76x76.png` & `tarantool-1.1.1/docs/source/_static/favicon/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon-128x128.png` & `tarantool-1.1.1/docs/source/_static/favicon/icon-128x128.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon-16x16.png` & `tarantool-1.1.1/docs/source/_static/favicon/icon-16x16.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon-196x196.png` & `tarantool-1.1.1/docs/source/_static/favicon/icon-196x196.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon-32x32.png` & `tarantool-1.1.1/docs/source/_static/favicon/icon-32x32.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon-96x96.png` & `tarantool-1.1.1/docs/source/_static/favicon/icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/_static/favicon/icon.svg` & `tarantool-1.1.1/docs/source/_static/favicon/icon.svg`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/api/module-tarantool.rst` & `tarantool-1.1.1/docs/source/api/module-tarantool.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/api/submodule-connection.rst` & `tarantool-1.1.1/docs/source/api/submodule-connection.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/api/submodule-mesh-connection.rst` & `tarantool-1.1.1/docs/source/api/submodule-mesh-connection.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/api/submodule-msgpack-ext-types.rst` & `tarantool-1.1.1/docs/source/api/submodule-msgpack-ext-types.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/api/submodule-msgpack-ext.rst` & `tarantool-1.1.1/docs/source/api/submodule-msgpack-ext.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/conf.py` & `tarantool-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/dev-guide.rst` & `tarantool-1.1.1/docs/source/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/index.rst` & `tarantool-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/docs/source/quick-start.rst` & `tarantool-1.1.1/docs/source/quick-start.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/rpm/SPECS/python-tarantool.spec` & `tarantool-1.1.1/rpm/SPECS/python-tarantool.spec`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/setup.py` & `tarantool-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/__init__.py` & `tarantool-1.1.1/tarantool/__init__.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/connection.py` & `tarantool-1.1.1/tarantool/connection.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/connection_pool.py` & `tarantool-1.1.1/tarantool/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/const.py` & `tarantool-1.1.1/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/crud.py` & `tarantool-1.1.1/tarantool/crud.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/dbapi.py` & `tarantool-1.1.1/tarantool/dbapi.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/error.py` & `tarantool-1.1.1/tarantool/error.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/mesh_connection.py` & `tarantool-1.1.1/tarantool/mesh_connection.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/datetime.py` & `tarantool-1.1.1/tarantool/msgpack_ext/datetime.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/decimal.py` & `tarantool-1.1.1/tarantool/msgpack_ext/decimal.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/error.py` & `tarantool-1.1.1/tarantool/msgpack_ext/error.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/interval.py` & `tarantool-1.1.1/tarantool/msgpack_ext/interval.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/packer.py` & `tarantool-1.1.1/tarantool/msgpack_ext/packer.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/types/datetime.py` & `tarantool-1.1.1/tarantool/msgpack_ext/types/datetime.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh` & `tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/gen-timezones.sh`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/timezones.py` & `tarantool-1.1.1/tarantool/msgpack_ext/types/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/unpacker.py` & `tarantool-1.1.1/tarantool/msgpack_ext/unpacker.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/msgpack_ext/uuid.py` & `tarantool-1.1.1/tarantool/msgpack_ext/uuid.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/request.py` & `tarantool-1.1.1/tarantool/request.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/response.py` & `tarantool-1.1.1/tarantool/response.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/schema.py` & `tarantool-1.1.1/tarantool/schema.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/space.py` & `tarantool-1.1.1/tarantool/space.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/types.py` & `tarantool-1.1.1/tarantool/types.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool/utils.py` & `tarantool-1.1.1/tarantool/utils.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/tarantool.egg-info/PKG-INFO` & `tarantool-1.1.1/tarantool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarantool
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client library for Tarantool
 Home-page: https://github.com/tarantool/tarantool-python
 Author: tarantool-python AUTHORS
 Author-email: admin@tarantool.org
 License: BSD
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `tarantool-1.1.0/tarantool.egg-info/SOURCES.txt` & `tarantool-1.1.1/tarantool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/ca.crt` & `tarantool-1.1.1/test/data/ca.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/generate.sh` & `tarantool-1.1.1/test/data/generate.sh`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/invalidhost.crt` & `tarantool-1.1.1/test/data/invalidhost.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/localhost.crt` & `tarantool-1.1.1/test/data/localhost.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/localhost.enc.key` & `tarantool-1.1.1/test/data/localhost.enc.key`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/data/localhost.key` & `tarantool-1.1.1/test/data/localhost.key`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/setup_command.py` & `tarantool-1.1.1/test/setup_command.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/__init__.py` & `tarantool-1.1.1/test/suites/__init__.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/box.lua` & `tarantool-1.1.1/test/suites/box.lua`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/crud_server.lua` & `tarantool-1.1.1/test/suites/crud_server.lua`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/lib/remote_tarantool_server.py` & `tarantool-1.1.1/test/suites/lib/remote_tarantool_server.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/lib/skip.py` & `tarantool-1.1.1/test/suites/lib/skip.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/lib/tarantool_admin.py` & `tarantool-1.1.1/test/suites/lib/tarantool_admin.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/lib/tarantool_python_ci.lua` & `tarantool-1.1.1/test/suites/lib/tarantool_python_ci.lua`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/lib/tarantool_server.py` & `tarantool-1.1.1/test/suites/lib/tarantool_server.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_connection.py` & `tarantool-1.1.1/test/suites/test_connection.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_crud.py` & `tarantool-1.1.1/test/suites/test_crud.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_datetime.py` & `tarantool-1.1.1/test/suites/test_datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,14 +476,20 @@
         },
         'month_overflow_last_day_last_adjust': {
             'arg_1': tarantool.Datetime(year=2009, month=2, day=28),
             'arg_2': tarantool.Interval(month=1, adjust=tarantool.IntervalAdjust.LAST),
             'res_add': tarantool.Datetime(year=2009, month=3, day=31),
             'res_sub': tarantool.Datetime(year=2009, month=1, day=31),
         },
+        'week': {
+            'arg_1': tarantool.Datetime(year=2008, month=2, day=3),
+            'arg_2': tarantool.Interval(week=1),
+            'res_add': tarantool.Datetime(year=2008, month=2, day=10),
+            'res_sub': tarantool.Datetime(year=2008, month=1, day=27),
+        },
     }
 
     def test_python_interval_addition(self):
         for name, case in self.interval_arithmetic_cases.items():
             with self.subTest(msg=name):
                 self.assertEqual(case['arg_1'] + case['arg_2'], case['res_add'])
```

### Comparing `tarantool-1.1.0/test/suites/test_dbapi.py` & `tarantool-1.1.1/test/suites/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_decimal.py` & `tarantool-1.1.1/test/suites/test_decimal.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_dml.py` & `tarantool-1.1.1/test/suites/test_dml.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             self.assertEqual(len(ans[0]), 1)
             self.assertIsInstance(ans[0][0], int)
             ans = con.call('uuid.str')
             self.assertEqual(len(ans), 1)
             self.assertEqual(len(ans[0]), 1)
             self.assertIsInstance(ans[0][0], str)
 
-            self.assertSequenceEqual(con.call('box.tuple.new', [1, 2, 3, 'fld_1']),
+            self.assertSequenceEqual(con.call('box.tuple.new', [[1, 2, 3, 'fld_1']]),
                                      [[1, 2, 3, 'fld_1']])
             self.assertSequenceEqual(con.call('box.tuple.new', 'fld_1'), [['fld_1']])
         finally:
             con.close()
 
     def test_07_call_17(self):
         con = tarantool.Connection(self.srv.host, self.srv.args['primary'])
@@ -232,15 +232,15 @@
         ans = con.call('fiber.time64')
         self.assertEqual(len(ans), 1)
         self.assertIsInstance(ans[0], int)
         ans = con.call('uuid.str')
         self.assertEqual(len(ans), 1)
         self.assertIsInstance(ans[0], str)
 
-        self.assertSequenceEqual(con.call('box.tuple.new', [1, 2, 3, 'fld_1']),
+        self.assertSequenceEqual(con.call('box.tuple.new', [[1, 2, 3, 'fld_1']]),
                                  [[1, 2, 3, 'fld_1']])
         self.assertSequenceEqual(con.call('box.tuple.new', 'fld_1'), [['fld_1']])
 
         con.close()
 
     def test_08_eval(self):
         self.assertSequenceEqual(self.con.eval('return json.decode(...)',
```

### Comparing `tarantool-1.1.0/test/suites/test_encoding.py` & `tarantool-1.1.1/test/suites/test_encoding.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_error_ext.py` & `tarantool-1.1.1/test/suites/test_error_ext.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_execute.py` & `tarantool-1.1.1/test/suites/test_execute.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_mesh.py` & `tarantool-1.1.1/test/suites/test_mesh.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_package.py` & `tarantool-1.1.1/test/suites/test_package.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_pool.py` & `tarantool-1.1.1/test/suites/test_pool.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_protocol.py` & `tarantool-1.1.1/test/suites/test_protocol.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_push.py` & `tarantool-1.1.1/test/suites/test_push.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_reconnect.py` & `tarantool-1.1.1/test/suites/test_reconnect.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_schema.py` & `tarantool-1.1.1/test/suites/test_schema.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_ssl.py` & `tarantool-1.1.1/test/suites/test_ssl.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.1.0/test/suites/test_uuid.py` & `tarantool-1.1.1/test/suites/test_uuid.py`

 * *Files identical despite different names*

