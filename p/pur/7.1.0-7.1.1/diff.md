# Comparing `tmp/pur-7.1.0.tar.gz` & `tmp/pur-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pur-7.1.0.tar", last modified: Thu Mar  2 11:32:12 2023, max compression
+gzip compressed data, was "pur-7.1.1.tar", last modified: Wed Jul 19 01:52:37 2023, max compression
```

## Comparing `pur-7.1.0.tar` & `pur-7.1.1.tar`

### file list

```diff
@@ -1,594 +1,596 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.769248 pur-7.1.0/
--rw-r--r--   0 user       (501) staff       (20)      259 2016-06-28 02:40:49.000000 pur-7.1.0/AUTHORS
--rw-r--r--   0 user       (501) staff       (20)     5863 2023-03-02 11:30:11.000000 pur-7.1.0/HISTORY.rst
--rw-r--r--   0 user       (501) staff       (20)     1372 2016-05-09 13:13:52.000000 pur-7.1.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       96 2022-04-06 05:23:00.000000 pur-7.1.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1185 2016-05-11 16:30:52.000000 pur-7.1.0/NOTICE
--rw-r--r--   0 user       (501) staff       (20)     6258 2023-03-02 11:32:12.769026 pur-7.1.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     5345 2023-03-02 11:28:38.000000 pur-7.1.0/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.433775 pur-7.1.0/pur/
--rw-r--r--   0 user       (501) staff       (20)      382 2023-03-02 11:30:55.000000 pur-7.1.0/pur/__about__.py
--rw-r--r--   0 user       (501) staff       (20)    18587 2023-03-02 11:18:58.000000 pur-7.1.0/pur/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      288 2019-04-10 16:17:10.000000 pur-7.1.0/pur/__main__.py
--rw-r--r--   0 user       (501) staff       (20)      254 2016-09-10 09:02:52.000000 pur-7.1.0/pur/exceptions.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.436963 pur-7.1.0/pur/packages/
--rw-r--r--   0 user       (501) staff       (20)        0 2019-01-23 18:06:16.000000 pur-7.1.0/pur/packages/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.437834 pur-7.1.0/pur/packages/pip/
--rw-r--r--   0 user       (501) staff       (20)      360 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1198 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/__main__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.445003 pur-7.1.0/pur/packages/pip/_internal/
--rwxr-xr-x   0 user       (501) staff       (20)      573 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     9571 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/build_env.py
--rw-r--r--   0 user       (501) staff       (20)     9441 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cache.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.457026 pur-7.1.0/pur/packages/pip/_internal/cli/
--rw-r--r--   0 user       (501) staff       (20)      132 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_internal/cli/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6399 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0 user       (501) staff       (20)     8034 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/base_command.py
--rw-r--r--   0 user       (501) staff       (20)    28432 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0 user       (501) staff       (20)      760 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/command_context.py
--rw-r--r--   0 user       (501) staff       (20)     2472 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/main.py
--rw-r--r--   0 user       (501) staff       (20)     2614 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0 user       (501) staff       (20)    10788 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/parser.py
--rw-r--r--   0 user       (501) staff       (20)    10339 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0 user       (501) staff       (20)    17360 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/req_command.py
--rw-r--r--   0 user       (501) staff       (20)     5076 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/spinners.py
--rw-r--r--   0 user       (501) staff       (20)      116 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/cli/status_codes.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.470511 pur-7.1.0/pur/packages/pip/_internal/commands/
--rw-r--r--   0 user       (501) staff       (20)     3736 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     7524 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/cache.py
--rw-r--r--   0 user       (501) staff       (20)     1685 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/check.py
--rw-r--r--   0 user       (501) staff       (20)     2958 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/completion.py
--rw-r--r--   0 user       (501) staff       (20)     8944 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/configuration.py
--rw-r--r--   0 user       (501) staff       (20)     6629 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/debug.py
--rw-r--r--   0 user       (501) staff       (20)     4904 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/download.py
--rw-r--r--   0 user       (501) staff       (20)     2951 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/freeze.py
--rw-r--r--   0 user       (501) staff       (20)     1703 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/hash.py
--rw-r--r--   0 user       (501) staff       (20)     1132 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/help.py
--rw-r--r--   0 user       (501) staff       (20)     4762 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/index.py
--rw-r--r--   0 user       (501) staff       (20)    27851 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/install.py
--rw-r--r--   0 user       (501) staff       (20)    12134 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/list.py
--rw-r--r--   0 user       (501) staff       (20)     5697 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/search.py
--rw-r--r--   0 user       (501) staff       (20)     5859 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/show.py
--rw-r--r--   0 user       (501) staff       (20)     3526 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0 user       (501) staff       (20)     6168 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/commands/wheel.py
--rw-r--r--   0 user       (501) staff       (20)    13171 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/configuration.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.473888 pur-7.1.0/pur/packages/pip/_internal/distributions/
--rw-r--r--   0 user       (501) staff       (20)      858 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1172 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/distributions/base.py
--rw-r--r--   0 user       (501) staff       (20)      680 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/distributions/installed.py
--rw-r--r--   0 user       (501) staff       (20)     5511 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0 user       (501) staff       (20)     1115 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0 user       (501) staff       (20)    18783 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/exceptions.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.477162 pur-7.1.0/pur/packages/pip/_internal/index/
--rw-r--r--   0 user       (501) staff       (20)       30 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/index/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    17534 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/index/collector.py
--rw-r--r--   0 user       (501) staff       (20)    36538 2022-05-09 22:29:03.000000 pur-7.1.0/pur/packages/pip/_internal/index/package_finder.py
--rw-r--r--   0 user       (501) staff       (20)     6557 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/index/sources.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.484305 pur-7.1.0/pur/packages/pip/_internal/locations/
--rw-r--r--   0 user       (501) staff       (20)    17256 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/locations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5871 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0 user       (501) staff       (20)     7918 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0 user       (501) staff       (20)     1579 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/locations/base.py
--rw-r--r--   0 user       (501) staff       (20)      340 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/main.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.487505 pur-7.1.0/pur/packages/pip/_internal/metadata/
--rw-r--r--   0 user       (501) staff       (20)     2036 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    19429 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/metadata/base.py
--rw-r--r--   0 user       (501) staff       (20)     9456 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/metadata/pkg_resources.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.507507 pur-7.1.0/pur/packages/pip/_internal/models/
--rw-r--r--   0 user       (501) staff       (20)       63 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_internal/models/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      990 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/candidate.py
--rw-r--r--   0 user       (501) staff       (20)     6350 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/direct_url.py
--rw-r--r--   0 user       (501) staff       (20)     2520 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/format_control.py
--rw-r--r--   0 user       (501) staff       (20)     1030 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/index.py
--rw-r--r--   0 user       (501) staff       (20)     9817 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/link.py
--rw-r--r--   0 user       (501) staff       (20)      738 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/scheme.py
--rw-r--r--   0 user       (501) staff       (20)     4520 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/search_scope.py
--rw-r--r--   0 user       (501) staff       (20)     1907 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0 user       (501) staff       (20)     3858 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/target_python.py
--rw-r--r--   0 user       (501) staff       (20)     3500 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/models/wheel.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.513063 pur-7.1.0/pur/packages/pip/_internal/network/
--rw-r--r--   0 user       (501) staff       (20)       50 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    12190 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/auth.py
--rw-r--r--   0 user       (501) staff       (20)     2100 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/cache.py
--rw-r--r--   0 user       (501) staff       (20)     6062 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/download.py
--rw-r--r--   0 user       (501) staff       (20)     7627 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0 user       (501) staff       (20)    16729 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/session.py
--rw-r--r--   0 user       (501) staff       (20)     4059 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/utils.py
--rw-r--r--   0 user       (501) staff       (20)     1791 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/network/xmlrpc.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.515851 pur-7.1.0/pur/packages/pip/_internal/operations/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_internal/operations/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.520729 pur-7.1.0/pur/packages/pip/_internal/operations/build/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1119 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0 user       (501) staff       (20)     1177 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0 user       (501) staff       (20)     1945 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0 user       (501) staff       (20)     1405 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0 user       (501) staff       (20)     3047 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0 user       (501) staff       (20)     5109 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/check.py
--rw-r--r--   0 user       (501) staff       (20)     9770 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/freeze.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.523188 pur-7.1.0/pur/packages/pip/_internal/operations/install/
--rw-r--r--   0 user       (501) staff       (20)       51 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1298 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0 user       (501) staff       (20)     4158 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0 user       (501) staff       (20)    27412 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0 user       (501) staff       (20)    23838 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/operations/prepare.py
--rw-r--r--   0 user       (501) staff       (20)     6714 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/pyproject.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.528843 pur-7.1.0/pur/packages/pip/_internal/req/
--rw-r--r--   0 user       (501) staff       (20)     2793 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    16094 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/constructors.py
--rw-r--r--   0 user       (501) staff       (20)    17421 2022-05-10 00:31:42.000000 pur-7.1.0/pur/packages/pip/_internal/req/req_file.py
--rw-r--r--   0 user       (501) staff       (20)    32472 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/req_install.py
--rw-r--r--   0 user       (501) staff       (20)     7584 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/req_set.py
--rw-r--r--   0 user       (501) staff       (20)     4117 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/req_tracker.py
--rw-r--r--   0 user       (501) staff       (20)    23814 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/req/req_uninstall.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.530097 pur-7.1.0/pur/packages/pip/_internal/resolution/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      583 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/base.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.531047 pur-7.1.0/pur/packages/pip/_internal/resolution/legacy/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    18288 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/legacy/resolver.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.536804 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5220 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0 user       (501) staff       (20)    18115 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0 user       (501) staff       (20)    26828 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0 user       (501) staff       (20)     5705 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0 user       (501) staff       (20)     9915 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0 user       (501) staff       (20)     2526 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0 user       (501) staff       (20)     5455 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0 user       (501) staff       (20)    11235 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0 user       (501) staff       (20)     6718 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/self_outdated_check.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.552226 pur-7.1.0/pur/packages/pip/_internal/utils/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_internal/utils/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1015 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/_log.py
--rw-r--r--   0 user       (501) staff       (20)     1665 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0 user       (501) staff       (20)     1884 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/compat.py
--rw-r--r--   0 user       (501) staff       (20)     5377 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0 user       (501) staff       (20)      242 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/datetime.py
--rw-r--r--   0 user       (501) staff       (20)     3627 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0 user       (501) staff       (20)     3206 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0 user       (501) staff       (20)     1249 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0 user       (501) staff       (20)     2203 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0 user       (501) staff       (20)     1169 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/encoding.py
--rw-r--r--   0 user       (501) staff       (20)     1055 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0 user       (501) staff       (20)     5893 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0 user       (501) staff       (20)      716 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0 user       (501) staff       (20)     3110 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/glibc.py
--rw-r--r--   0 user       (501) staff       (20)     4811 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/hashes.py
--rw-r--r--   0 user       (501) staff       (20)      795 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0 user       (501) staff       (20)    11519 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/logging.py
--rw-r--r--   0 user       (501) staff       (20)    18392 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/misc.py
--rw-r--r--   0 user       (501) staff       (20)     1193 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/models.py
--rw-r--r--   0 user       (501) staff       (20)     2108 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/packaging.py
--rw-r--r--   0 user       (501) staff       (20)     4697 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0 user       (501) staff       (20)    10058 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0 user       (501) staff       (20)     7662 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0 user       (501) staff       (20)     8906 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0 user       (501) staff       (20)     1759 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/urls.py
--rw-r--r--   0 user       (501) staff       (20)     3459 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0 user       (501) staff       (20)     4549 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.555995 pur-7.1.0/pur/packages/pip/_internal/vcs/
--rw-r--r--   0 user       (501) staff       (20)      596 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2857 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0 user       (501) staff       (20)    17804 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/git.py
--rw-r--r--   0 user       (501) staff       (20)     4945 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0 user       (501) staff       (20)    11596 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0 user       (501) staff       (20)    22414 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0 user       (501) staff       (20)    12247 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_internal/wheel_builder.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.560484 pur-7.1.0/pur/packages/pip/_vendor/
--rw-r--r--   0 user       (501) staff       (20)     4708 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.568953 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 user       (501) staff       (20)      302 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1295 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0 user       (501) staff       (20)     4882 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 user       (501) staff       (20)      805 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/cache.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.571123 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 user       (501) staff       (20)       86 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4153 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 user       (501) staff       (20)      856 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 user       (501) staff       (20)      695 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 user       (501) staff       (20)    14149 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 user       (501) staff       (20)     2533 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 user       (501) staff       (20)     4070 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 user       (501) staff       (20)     7091 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 user       (501) staff       (20)      690 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/wrapper.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.573991 pur-7.1.0/pur/packages/pip/_vendor/certifi/
--rw-r--r--   0 user       (501) staff       (20)       62 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      255 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 user       (501) staff       (20)   259465 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0 user       (501) staff       (20)     2840 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/certifi/core.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.604106 pur-7.1.0/pur/packages/pip/_vendor/chardet/
--rw-r--r--   0 user       (501) staff       (20)     3271 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    31254 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 user       (501) staff       (20)     1757 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 user       (501) staff       (20)     9411 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 user       (501) staff       (20)     3839 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 user       (501) staff       (20)     5110 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.605099 pur-7.1.0/pur/packages/pip/_vendor/chardet/cli/
--rw-r--r--   0 user       (501) staff       (20)        1 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2747 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 user       (501) staff       (20)     3590 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 user       (501) staff       (20)     1200 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/compat.py
--rw-r--r--   0 user       (501) staff       (20)     1855 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 user       (501) staff       (20)     1661 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0 user       (501) staff       (20)     3950 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 user       (501) staff       (20)    10510 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 user       (501) staff       (20)     3749 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 user       (501) staff       (20)    13546 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 user       (501) staff       (20)     1748 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 user       (501) staff       (20)    31621 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 user       (501) staff       (20)     1747 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 user       (501) staff       (20)    20715 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 user       (501) staff       (20)     1754 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 user       (501) staff       (20)    13838 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 user       (501) staff       (20)    25777 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 user       (501) staff       (20)    19643 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0 user       (501) staff       (20)   105697 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 user       (501) staff       (20)    99571 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 user       (501) staff       (20)    98776 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 user       (501) staff       (20)   102498 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 user       (501) staff       (20)   131180 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0 user       (501) staff       (20)   103312 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 user       (501) staff       (20)    95946 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 user       (501) staff       (20)     5370 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 user       (501) staff       (20)     3413 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 user       (501) staff       (20)     2012 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 user       (501) staff       (20)    25481 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcssm.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.605949 pur-7.1.0/pur/packages/pip/_vendor/chardet/metadata/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    19474 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0 user       (501) staff       (20)     6136 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 user       (501) staff       (20)     4309 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 user       (501) staff       (20)     3774 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 user       (501) staff       (20)    12503 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 user       (501) staff       (20)     2766 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 user       (501) staff       (20)      242 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/chardet/version.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.609388 pur-7.1.0/pur/packages/pip/_vendor/colorama/
--rw-r--r--   0 user       (501) staff       (20)      239 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2522 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 user       (501) staff       (20)    10517 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 user       (501) staff       (20)     1915 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0 user       (501) staff       (20)     5404 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0 user       (501) staff       (20)     6438 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/colorama/winterm.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.621409 pur-7.1.0/pur/packages/pip/_vendor/distlib/
--rw-r--r--   0 user       (501) staff       (20)      581 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.624885 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/
--rw-r--r--   0 user       (501) staff       (20)      274 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      971 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0 user       (501) staff       (20)    25707 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0 user       (501) staff       (20)    26854 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0 user       (501) staff       (20)    92628 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0 user       (501) staff       (20)    41495 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0 user       (501) staff       (20)    51059 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/database.py
--rw-r--r--   0 user       (501) staff       (20)    20739 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/index.py
--rw-r--r--   0 user       (501) staff       (20)    51965 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0 user       (501) staff       (20)    14811 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 user       (501) staff       (20)     4989 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0 user       (501) staff       (20)    39109 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 user       (501) staff       (20)    10820 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0 user       (501) staff       (20)    17720 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 user       (501) staff       (20)    67766 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/util.py
--rw-r--r--   0 user       (501) staff       (20)    23513 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/version.py
--rw-r--r--   0 user       (501) staff       (20)    42943 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0 user       (501) staff       (20)    48414 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/distro.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.634157 pur-7.1.0/pur/packages/pip/_vendor/html5lib/
--rw-r--r--   0 user       (501) staff       (20)     1160 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    16728 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0 user       (501) staff       (20)    32353 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0 user       (501) staff       (20)    77040 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_tokenizer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.636101 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/
--rw-r--r--   0 user       (501) staff       (20)      109 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1013 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0 user       (501) staff       (20)     1775 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/py.py
--rw-r--r--   0 user       (501) staff       (20)     4931 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0 user       (501) staff       (20)    83464 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/constants.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.641218 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      919 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0 user       (501) staff       (20)      286 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0 user       (501) staff       (20)     2945 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0 user       (501) staff       (20)     3643 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0 user       (501) staff       (20)    10588 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0 user       (501) staff       (20)    26897 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0 user       (501) staff       (20)     1214 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0 user       (501) staff       (20)   117186 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0 user       (501) staff       (20)    15759 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/serializer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.643422 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/
--rw-r--r--   0 user       (501) staff       (20)      679 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1715 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0 user       (501) staff       (20)     1776 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/sax.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.647123 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/
--rw-r--r--   0 user       (501) staff       (20)     3592 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    14565 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0 user       (501) staff       (20)     8925 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0 user       (501) staff       (20)    12836 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0 user       (501) staff       (20)    14766 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.650940 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/
--rw-r--r--   0 user       (501) staff       (20)     5719 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     7476 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0 user       (501) staff       (20)     1413 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0 user       (501) staff       (20)     4551 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0 user       (501) staff       (20)     6357 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0 user       (501) staff       (20)     2309 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/genshi.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.656889 pur-7.1.0/pur/packages/pip/_vendor/idna/
--rw-r--r--   0 user       (501) staff       (20)      849 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3453 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/codec.py
--rw-r--r--   0 user       (501) staff       (20)      360 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/compat.py
--rw-r--r--   0 user       (501) staff       (20)    12826 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/core.py
--rw-r--r--   0 user       (501) staff       (20)    42350 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 user       (501) staff       (20)     1933 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0 user       (501) staff       (20)       21 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0 user       (501) staff       (20)   201849 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/idna/uts46data.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.661198 pur-7.1.0/pur/packages/pip/_vendor/msgpack/
--rw-r--r--   0 user       (501) staff       (20)     1118 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0 user       (501) staff       (20)       20 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/msgpack/_version.py
--rw-r--r--   0 user       (501) staff       (20)     1081 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0 user       (501) staff       (20)     6088 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0 user       (501) staff       (20)    38026 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/msgpack/fallback.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.667904 pur-7.1.0/pur/packages/pip/_vendor/packaging/
--rw-r--r--   0 user       (501) staff       (20)      661 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 user       (501) staff       (20)      497 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11488 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0 user       (501) staff       (20)     4378 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0 user       (501) staff       (20)     1629 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 user       (501) staff       (20)     8487 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0 user       (501) staff       (20)     4676 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 user       (501) staff       (20)    30964 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 user       (501) staff       (20)    15714 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0 user       (501) staff       (20)     4200 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0 user       (501) staff       (20)    14665 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/packaging/version.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.675733 pur-7.1.0/pur/packages/pip/_vendor/pep517/
--rw-r--r--   0 user       (501) staff       (20)      130 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3457 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/build.py
--rw-r--r--   0 user       (501) staff       (20)     6084 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/check.py
--rw-r--r--   0 user       (501) staff       (20)     4098 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0 user       (501) staff       (20)     1253 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/compat.py
--rw-r--r--   0 user       (501) staff       (20)     1129 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0 user       (501) staff       (20)     6100 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/envbuild.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.676767 pur-7.1.0/pur/packages/pip/_vendor/pep517/in_process/
--rw-r--r--   0 user       (501) staff       (20)      563 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11201 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0 user       (501) staff       (20)     2463 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0 user       (501) staff       (20)    13429 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pep517/wrappers.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.678819 pur-7.1.0/pur/packages/pip/_vendor/pkg_resources/
--rw-r--r--   0 user       (501) staff       (20)   108287 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      562 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/pkg_resources/py31compat.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.683741 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/
--rw-r--r--   0 user       (501) staff       (20)    12871 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1140 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0 user       (501) staff       (20)     3994 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0 user       (501) staff       (20)     4922 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0 user       (501) staff       (20)     2619 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0 user       (501) staff       (20)     6905 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0 user       (501) staff       (20)       80 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0 user       (501) staff       (20)     6416 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/platformdirs/windows.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.686573 pur-7.1.0/pur/packages/pip/_vendor/progress/
--rw-r--r--   0 user       (501) staff       (20)     5294 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/progress/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2942 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/progress/bar.py
--rw-r--r--   0 user       (501) staff       (20)     2655 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/progress/colors.py
--rw-r--r--   0 user       (501) staff       (20)     1613 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/progress/counter.py
--rw-r--r--   0 user       (501) staff       (20)     1461 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/progress/spinner.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.695388 pur-7.1.0/pur/packages/pip/_vendor/pygments/
--rw-r--r--   0 user       (501) staff       (20)     3013 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      353 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0 user       (501) staff       (20)    21693 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0 user       (501) staff       (20)     1697 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/console.py
--rw-r--r--   0 user       (501) staff       (20)     1938 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/filter.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.695754 pur-7.1.0/pur/packages/pip/_vendor/pygments/filters/
--rw-r--r--   0 user       (501) staff       (20)    40292 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2917 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatter.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.702701 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/
--rw-r--r--   0 user       (501) staff       (20)     5119 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6348 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 user       (501) staff       (20)     3314 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 user       (501) staff       (20)    34690 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0 user       (501) staff       (20)    21819 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0 user       (501) staff       (20)     5881 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0 user       (501) staff       (20)    18930 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0 user       (501) staff       (20)     5073 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0 user       (501) staff       (20)     2212 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0 user       (501) staff       (20)     5014 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0 user       (501) staff       (20)     7335 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0 user       (501) staff       (20)     4686 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0 user       (501) staff       (20)    11763 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 user       (501) staff       (20)    31554 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/lexer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.703983 pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/
--rw-r--r--   0 user       (501) staff       (20)    11307 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    68826 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 user       (501) staff       (20)    51988 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0 user       (501) staff       (20)      986 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0 user       (501) staff       (20)     1727 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0 user       (501) staff       (20)     3072 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0 user       (501) staff       (20)     3091 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0 user       (501) staff       (20)     4630 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0 user       (501) staff       (20)     6025 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/style.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.704479 pur-7.1.0/pur/packages/pip/_vendor/pygments/styles/
--rw-r--r--   0 user       (501) staff       (20)     3055 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6143 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/token.py
--rw-r--r--   0 user       (501) staff       (20)    63200 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0 user       (501) staff       (20)     9123 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pygments/util.py
--rw-r--r--   0 user       (501) staff       (20)   273394 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/pyparsing.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.711928 pur-7.1.0/pur/packages/pip/_vendor/requests/
--rw-r--r--   0 user       (501) staff       (20)     5130 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      441 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0 user       (501) staff       (20)     1096 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 user       (501) staff       (20)    21861 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0 user       (501) staff       (20)     6402 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/api.py
--rw-r--r--   0 user       (501) staff       (20)    10207 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/auth.py
--rw-r--r--   0 user       (501) staff       (20)      465 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/certs.py
--rw-r--r--   0 user       (501) staff       (20)     2114 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/compat.py
--rw-r--r--   0 user       (501) staff       (20)    18430 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0 user       (501) staff       (20)     3446 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 user       (501) staff       (20)     3972 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/help.py
--rw-r--r--   0 user       (501) staff       (20)      757 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0 user       (501) staff       (20)    35116 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/models.py
--rw-r--r--   0 user       (501) staff       (20)      695 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/packages.py
--rw-r--r--   0 user       (501) staff       (20)    29835 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0 user       (501) staff       (20)     4188 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 user       (501) staff       (20)     3005 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/structures.py
--rw-r--r--   0 user       (501) staff       (20)    33301 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.714154 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/
--rw-r--r--   0 user       (501) staff       (20)      537 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.714847 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/compat/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      156 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0 user       (501) staff       (20)     5872 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0 user       (501) staff       (20)     1583 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0 user       (501) staff       (20)    17592 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0 user       (501) staff       (20)     4794 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/resolvelib/structs.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.746221 pur-7.1.0/pur/packages/pip/_vendor/rich/
--rw-r--r--   0 user       (501) staff       (20)     5804 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     8895 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0 user       (501) staff       (20)    10096 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0 user       (501) staff       (20)   140235 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0 user       (501) staff       (20)     1064 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0 user       (501) staff       (20)      265 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0 user       (501) staff       (20)     7444 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0 user       (501) staff       (20)     3225 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0 user       (501) staff       (20)     1236 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0 user       (501) staff       (20)     1246 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_lru_cache.py
--rw-r--r--   0 user       (501) staff       (20)     7063 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0 user       (501) staff       (20)      423 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0 user       (501) staff       (20)     5472 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0 user       (501) staff       (20)    26521 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0 user       (501) staff       (20)      351 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0 user       (501) staff       (20)      417 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0 user       (501) staff       (20)     2089 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0 user       (501) staff       (20)     1804 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0 user       (501) staff       (20)      890 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/abc.py
--rw-r--r--   0 user       (501) staff       (20)    10425 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/align.py
--rw-r--r--   0 user       (501) staff       (20)     6676 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0 user       (501) staff       (20)     3264 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/bar.py
--rw-r--r--   0 user       (501) staff       (20)     9069 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/box.py
--rw-r--r--   0 user       (501) staff       (20)     3897 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/cells.py
--rw-r--r--   0 user       (501) staff       (20)    17285 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/color.py
--rw-r--r--   0 user       (501) staff       (20)     1054 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0 user       (501) staff       (20)     7131 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/columns.py
--rw-r--r--   0 user       (501) staff       (20)    80866 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/console.py
--rw-r--r--   0 user       (501) staff       (20)     1288 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0 user       (501) staff       (20)     5497 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/containers.py
--rw-r--r--   0 user       (501) staff       (20)     5298 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/control.py
--rw-r--r--   0 user       (501) staff       (20)     6872 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0 user       (501) staff       (20)      183 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0 user       (501) staff       (20)     2501 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0 user       (501) staff       (20)      642 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/errors.py
--rw-r--r--   0 user       (501) staff       (20)     1657 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0 user       (501) staff       (20)     2511 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0 user       (501) staff       (20)     4894 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0 user       (501) staff       (20)     5051 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/json.py
--rw-r--r--   0 user       (501) staff       (20)     2856 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0 user       (501) staff       (20)    14048 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/layout.py
--rw-r--r--   0 user       (501) staff       (20)    13933 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/live.py
--rw-r--r--   0 user       (501) staff       (20)     3670 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0 user       (501) staff       (20)    10862 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/logging.py
--rw-r--r--   0 user       (501) staff       (20)     8057 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/markup.py
--rw-r--r--   0 user       (501) staff       (20)     5258 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/measure.py
--rw-r--r--   0 user       (501) staff       (20)     4778 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/padding.py
--rw-r--r--   0 user       (501) staff       (20)      816 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/pager.py
--rw-r--r--   0 user       (501) staff       (20)     3396 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/palette.py
--rw-r--r--   0 user       (501) staff       (20)     8637 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/panel.py
--rw-r--r--   0 user       (501) staff       (20)    29525 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0 user       (501) staff       (20)    35926 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/progress.py
--rw-r--r--   0 user       (501) staff       (20)     7762 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0 user       (501) staff       (20)    11307 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0 user       (501) staff       (20)     1401 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0 user       (501) staff       (20)      166 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/region.py
--rw-r--r--   0 user       (501) staff       (20)     4309 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/repr.py
--rw-r--r--   0 user       (501) staff       (20)     4197 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/rule.py
--rw-r--r--   0 user       (501) staff       (20)     2842 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/scope.py
--rw-r--r--   0 user       (501) staff       (20)     1591 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/screen.py
--rw-r--r--   0 user       (501) staff       (20)    20722 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/segment.py
--rw-r--r--   0 user       (501) staff       (20)     4312 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0 user       (501) staff       (20)     4425 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/status.py
--rw-r--r--   0 user       (501) staff       (20)    26469 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/style.py
--rw-r--r--   0 user       (501) staff       (20)     1258 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/styled.py
--rw-r--r--   0 user       (501) staff       (20)    26548 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0 user       (501) staff       (20)    34771 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/table.py
--rw-r--r--   0 user       (501) staff       (20)     1700 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/tabulate.py
--rw-r--r--   0 user       (501) staff       (20)     1459 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0 user       (501) staff       (20)    41471 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/text.py
--rw-r--r--   0 user       (501) staff       (20)     3627 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/theme.py
--rw-r--r--   0 user       (501) staff       (20)      102 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/themes.py
--rw-r--r--   0 user       (501) staff       (20)    25896 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0 user       (501) staff       (20)     9122 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/rich/tree.py
--rw-r--r--   0 user       (501) staff       (20)    34549 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/six.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.750333 pur-7.1.0/pur/packages/pip/_vendor/tenacity/
--rw-r--r--   0 user       (501) staff       (20)    18257 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3314 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0 user       (501) staff       (20)     1944 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0 user       (501) staff       (20)     1496 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0 user       (501) staff       (20)     1376 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0 user       (501) staff       (20)     1908 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0 user       (501) staff       (20)     1383 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0 user       (501) staff       (20)     6645 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0 user       (501) staff       (20)     2790 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0 user       (501) staff       (20)     2145 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0 user       (501) staff       (20)     6691 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tenacity/wait.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.751385 pur-7.1.0/pur/packages/pip/_vendor/tomli/
--rw-r--r--   0 user       (501) staff       (20)      230 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    22415 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0 user       (501) staff       (20)     2681 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0 user       (501) staff       (20)   109284 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/typing_extensions.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.756762 pur-7.1.0/pur/packages/pip/_vendor/urllib3/
--rw-r--r--   0 user       (501) staff       (20)     2763 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    10811 2022-04-06 05:08:23.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0 user       (501) staff       (20)       63 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0 user       (501) staff       (20)    20076 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 user       (501) staff       (20)    39013 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.759319 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      957 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.760334 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    17632 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user       (501) staff       (20)    13922 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user       (501) staff       (20)    11034 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 user       (501) staff       (20)     4538 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user       (501) staff       (20)    16900 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user       (501) staff       (20)    34449 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 user       (501) staff       (20)     7097 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 user       (501) staff       (20)     8217 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 user       (501) staff       (20)     8579 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0 user       (501) staff       (20)     2440 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.760875 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.761485 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1417 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user       (501) staff       (20)    34666 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0 user       (501) staff       (20)    19763 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 user       (501) staff       (20)     5985 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0 user       (501) staff       (20)    28203 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.766552 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/
--rw-r--r--   0 user       (501) staff       (20)     1155 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4901 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 user       (501) staff       (20)     1605 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0 user       (501) staff       (20)      498 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0 user       (501) staff       (20)     4123 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 user       (501) staff       (20)     3510 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 user       (501) staff       (20)    22001 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 user       (501) staff       (20)    17177 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 user       (501) staff       (20)     5751 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user       (501) staff       (20)     6895 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0 user       (501) staff       (20)    10003 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 user       (501) staff       (20)    14047 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 user       (501) staff       (20)     5404 2022-01-23 20:23:57.000000 pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/wait.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.768612 pur-7.1.0/pur/packages/pip/_vendor/webencodings/
--rw-r--r--   0 user       (501) staff       (20)    10579 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     8979 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 user       (501) staff       (20)     1305 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 user       (501) staff       (20)     6563 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 user       (501) staff       (20)     4307 2022-01-21 15:48:11.000000 pur-7.1.0/pur/packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0 user       (501) staff       (20)    11025 2023-03-02 11:20:49.000000 pur-7.1.0/pur/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-02 11:32:12.436583 pur-7.1.0/pur.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     6258 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)    24365 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       41 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-03-02 10:55:30.000000 pur-7.1.0/pur.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)       13 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        4 2023-03-02 11:32:12.000000 pur-7.1.0/pur.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       13 2023-03-02 11:21:43.000000 pur-7.1.0/requirements.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-03-02 11:32:12.769357 pur-7.1.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1381 2022-04-05 22:04:28.000000 pur-7.1.0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.733487 pur-7.1.1/
+-rw-r--r--   0 user       (501) staff       (20)      259 2022-04-06 05:15:05.000000 pur-7.1.1/AUTHORS
+-rw-r--r--   0 user       (501) staff       (20)     5933 2023-07-19 01:49:57.000000 pur-7.1.1/HISTORY.rst
+-rw-r--r--   0 user       (501) staff       (20)     1372 2022-04-06 05:15:05.000000 pur-7.1.1/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       96 2022-04-06 05:15:05.000000 pur-7.1.1/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1185 2022-04-06 05:15:05.000000 pur-7.1.1/NOTICE
+-rw-r--r--   0 user       (501) staff       (20)     6215 2023-07-19 01:52:37.733066 pur-7.1.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     5264 2023-07-19 01:48:13.000000 pur-7.1.1/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.064971 pur-7.1.1/pur/
+-rw-r--r--   0 user       (501) staff       (20)      382 2023-07-19 01:50:22.000000 pur-7.1.1/pur/__about__.py
+-rw-r--r--   0 user       (501) staff       (20)    18587 2023-07-19 01:44:50.000000 pur-7.1.1/pur/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      288 2022-04-06 05:15:05.000000 pur-7.1.1/pur/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)      254 2022-04-06 05:15:05.000000 pur-7.1.1/pur/exceptions.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.067511 pur-7.1.1/pur/packages/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.068163 pur-7.1.1/pur/packages/pip/
+-rw-r--r--   0 user       (501) staff       (20)      360 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1198 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/__main__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.072815 pur-7.1.1/pur/packages/pip/_internal/
+-rwxr-xr-x   0 user       (501) staff       (20)      573 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9571 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/build_env.py
+-rw-r--r--   0 user       (501) staff       (20)     9441 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cache.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.114516 pur-7.1.1/pur/packages/pip/_internal/cli/
+-rw-r--r--   0 user       (501) staff       (20)      132 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6399 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 user       (501) staff       (20)     8034 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 user       (501) staff       (20)    28432 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 user       (501) staff       (20)      760 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 user       (501) staff       (20)     2472 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/main.py
+-rw-r--r--   0 user       (501) staff       (20)     2614 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 user       (501) staff       (20)    10788 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 user       (501) staff       (20)    10339 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 user       (501) staff       (20)    17360 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 user       (501) staff       (20)     5076 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 user       (501) staff       (20)      116 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.123292 pur-7.1.1/pur/packages/pip/_internal/commands/
+-rw-r--r--   0 user       (501) staff       (20)     3736 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7524 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 user       (501) staff       (20)     1685 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/check.py
+-rw-r--r--   0 user       (501) staff       (20)     2958 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 user       (501) staff       (20)     8944 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 user       (501) staff       (20)     6629 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 user       (501) staff       (20)     4904 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/download.py
+-rw-r--r--   0 user       (501) staff       (20)     2951 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 user       (501) staff       (20)     1703 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 user       (501) staff       (20)     1132 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/help.py
+-rw-r--r--   0 user       (501) staff       (20)     4762 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/index.py
+-rw-r--r--   0 user       (501) staff       (20)    27851 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/install.py
+-rw-r--r--   0 user       (501) staff       (20)    12134 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/list.py
+-rw-r--r--   0 user       (501) staff       (20)     5697 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/search.py
+-rw-r--r--   0 user       (501) staff       (20)     5859 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/show.py
+-rw-r--r--   0 user       (501) staff       (20)     3526 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 user       (501) staff       (20)     6168 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 user       (501) staff       (20)    13171 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/configuration.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.125912 pur-7.1.1/pur/packages/pip/_internal/distributions/
+-rw-r--r--   0 user       (501) staff       (20)      858 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1172 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 user       (501) staff       (20)      680 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 user       (501) staff       (20)     5511 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 user       (501) staff       (20)     1115 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 user       (501) staff       (20)    18783 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.128227 pur-7.1.1/pur/packages/pip/_internal/index/
+-rw-r--r--   0 user       (501) staff       (20)       30 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    17534 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/index/collector.py
+-rw-r--r--   0 user       (501) staff       (20)    36538 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 user       (501) staff       (20)     6557 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/index/sources.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.130176 pur-7.1.1/pur/packages/pip/_internal/locations/
+-rw-r--r--   0 user       (501) staff       (20)    17256 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     5871 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0 user       (501) staff       (20)     7918 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0 user       (501) staff       (20)     1579 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/locations/base.py
+-rw-r--r--   0 user       (501) staff       (20)      340 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/main.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.131767 pur-7.1.1/pur/packages/pip/_internal/metadata/
+-rw-r--r--   0 user       (501) staff       (20)     2036 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    19429 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/metadata/base.py
+-rw-r--r--   0 user       (501) staff       (20)     9456 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/metadata/pkg_resources.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.137546 pur-7.1.1/pur/packages/pip/_internal/models/
+-rw-r--r--   0 user       (501) staff       (20)       63 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      990 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 user       (501) staff       (20)     6350 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 user       (501) staff       (20)     2520 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 user       (501) staff       (20)     1030 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/index.py
+-rw-r--r--   0 user       (501) staff       (20)     9817 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/link.py
+-rw-r--r--   0 user       (501) staff       (20)      738 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 user       (501) staff       (20)     4520 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 user       (501) staff       (20)     1907 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 user       (501) staff       (20)     3858 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 user       (501) staff       (20)     3500 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.141672 pur-7.1.1/pur/packages/pip/_internal/network/
+-rw-r--r--   0 user       (501) staff       (20)       50 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    12190 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/auth.py
+-rw-r--r--   0 user       (501) staff       (20)     2100 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/cache.py
+-rw-r--r--   0 user       (501) staff       (20)     6062 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/download.py
+-rw-r--r--   0 user       (501) staff       (20)     7627 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 user       (501) staff       (20)    16729 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/session.py
+-rw-r--r--   0 user       (501) staff       (20)     4059 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/utils.py
+-rw-r--r--   0 user       (501) staff       (20)     1791 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.143680 pur-7.1.1/pur/packages/pip/_internal/operations/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.196465 pur-7.1.1/pur/packages/pip/_internal/operations/build/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1119 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 user       (501) staff       (20)     1177 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0 user       (501) staff       (20)     1945 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 user       (501) staff       (20)     1405 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0 user       (501) staff       (20)     3047 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 user       (501) staff       (20)     5109 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/check.py
+-rw-r--r--   0 user       (501) staff       (20)     9770 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.198622 pur-7.1.1/pur/packages/pip/_internal/operations/install/
+-rw-r--r--   0 user       (501) staff       (20)       51 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1298 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 user       (501) staff       (20)     4158 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 user       (501) staff       (20)    27412 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 user       (501) staff       (20)    23838 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 user       (501) staff       (20)     6714 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.202896 pur-7.1.1/pur/packages/pip/_internal/req/
+-rw-r--r--   0 user       (501) staff       (20)     2793 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    16094 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 user       (501) staff       (20)    17421 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 user       (501) staff       (20)    32472 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 user       (501) staff       (20)     7584 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 user       (501) staff       (20)     4117 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/req_tracker.py
+-rw-r--r--   0 user       (501) staff       (20)    23814 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.203829 pur-7.1.1/pur/packages/pip/_internal/resolution/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      583 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.204699 pur-7.1.1/pur/packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    18288 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.209859 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     5220 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 user       (501) staff       (20)    18115 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 user       (501) staff       (20)    26828 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 user       (501) staff       (20)     5705 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0 user       (501) staff       (20)     9915 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 user       (501) staff       (20)     2526 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0 user       (501) staff       (20)     5455 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 user       (501) staff       (20)    11235 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 user       (501) staff       (20)     6718 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.268581 pur-7.1.1/pur/packages/pip/_internal/utils/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1015 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/_log.py
+-rw-r--r--   0 user       (501) staff       (20)     1665 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 user       (501) staff       (20)     1884 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 user       (501) staff       (20)     5377 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 user       (501) staff       (20)      242 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 user       (501) staff       (20)     3627 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 user       (501) staff       (20)     3206 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     1249 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 user       (501) staff       (20)     2203 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0 user       (501) staff       (20)     1169 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 user       (501) staff       (20)     1055 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 user       (501) staff       (20)     5893 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 user       (501) staff       (20)      716 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 user       (501) staff       (20)     3110 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 user       (501) staff       (20)     4811 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 user       (501) staff       (20)      795 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 user       (501) staff       (20)    11519 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 user       (501) staff       (20)    18392 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 user       (501) staff       (20)     1193 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/models.py
+-rw-r--r--   0 user       (501) staff       (20)     2108 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 user       (501) staff       (20)     4697 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 user       (501) staff       (20)    10058 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 user       (501) staff       (20)     7662 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 user       (501) staff       (20)     8906 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 user       (501) staff       (20)     1759 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 user       (501) staff       (20)     3459 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 user       (501) staff       (20)     4549 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.271551 pur-7.1.1/pur/packages/pip/_internal/vcs/
+-rw-r--r--   0 user       (501) staff       (20)      596 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2857 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 user       (501) staff       (20)    17804 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 user       (501) staff       (20)     4945 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 user       (501) staff       (20)    11596 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 user       (501) staff       (20)    22414 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 user       (501) staff       (20)    12247 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.275048 pur-7.1.1/pur/packages/pip/_vendor/
+-rw-r--r--   0 user       (501) staff       (20)     4708 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.315103 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 user       (501) staff       (20)      302 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1295 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 user       (501) staff       (20)     4882 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 user       (501) staff       (20)      805 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.316082 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 user       (501) staff       (20)       86 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4153 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 user       (501) staff       (20)      856 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 user       (501) staff       (20)      695 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 user       (501) staff       (20)    14149 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 user       (501) staff       (20)     2533 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 user       (501) staff       (20)     4070 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 user       (501) staff       (20)     7091 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 user       (501) staff       (20)      690 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.319627 pur-7.1.1/pur/packages/pip/_vendor/certifi/
+-rw-r--r--   0 user       (501) staff       (20)       62 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      255 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)   259465 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0 user       (501) staff       (20)     2840 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.399367 pur-7.1.1/pur/packages/pip/_vendor/chardet/
+-rw-r--r--   0 user       (501) staff       (20)     3271 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    31254 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 user       (501) staff       (20)     1757 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 user       (501) staff       (20)     9411 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 user       (501) staff       (20)     3839 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 user       (501) staff       (20)     5110 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.400266 pur-7.1.1/pur/packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 user       (501) staff       (20)        1 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2747 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 user       (501) staff       (20)     3590 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 user       (501) staff       (20)     1200 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/compat.py
+-rw-r--r--   0 user       (501) staff       (20)     1855 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 user       (501) staff       (20)     1661 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 user       (501) staff       (20)     3950 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 user       (501) staff       (20)    10510 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 user       (501) staff       (20)     3749 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 user       (501) staff       (20)    13546 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 user       (501) staff       (20)     1748 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 user       (501) staff       (20)    31621 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 user       (501) staff       (20)     1747 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 user       (501) staff       (20)    20715 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 user       (501) staff       (20)     1754 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 user       (501) staff       (20)    13838 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 user       (501) staff       (20)    25777 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 user       (501) staff       (20)    19643 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 user       (501) staff       (20)   105697 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 user       (501) staff       (20)    99571 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 user       (501) staff       (20)    98776 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 user       (501) staff       (20)   102498 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 user       (501) staff       (20)   131180 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 user       (501) staff       (20)   103312 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 user       (501) staff       (20)    95946 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 user       (501) staff       (20)     5370 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 user       (501) staff       (20)     3413 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 user       (501) staff       (20)     2012 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 user       (501) staff       (20)    25481 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.401036 pur-7.1.1/pur/packages/pip/_vendor/chardet/metadata/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    19474 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 user       (501) staff       (20)     6136 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 user       (501) staff       (20)     4309 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 user       (501) staff       (20)     3774 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 user       (501) staff       (20)    12503 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 user       (501) staff       (20)     2766 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 user       (501) staff       (20)      242 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.403648 pur-7.1.1/pur/packages/pip/_vendor/colorama/
+-rw-r--r--   0 user       (501) staff       (20)      239 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2522 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 user       (501) staff       (20)    10517 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 user       (501) staff       (20)     1915 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0 user       (501) staff       (20)     5404 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 user       (501) staff       (20)     6438 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/colorama/winterm.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.410304 pur-7.1.1/pur/packages/pip/_vendor/distlib/
+-rw-r--r--   0 user       (501) staff       (20)      581 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.452312 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/
+-rw-r--r--   0 user       (501) staff       (20)      274 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      971 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0 user       (501) staff       (20)    25707 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 user       (501) staff       (20)    26854 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 user       (501) staff       (20)    92628 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 user       (501) staff       (20)    41495 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 user       (501) staff       (20)    51059 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 user       (501) staff       (20)    20739 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 user       (501) staff       (20)    51965 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 user       (501) staff       (20)    14811 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 user       (501) staff       (20)     4989 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 user       (501) staff       (20)    39109 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 user       (501) staff       (20)    10820 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 user       (501) staff       (20)    17720 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 user       (501) staff       (20)    67766 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 user       (501) staff       (20)    23513 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 user       (501) staff       (20)    42943 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0 user       (501) staff       (20)    48414 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/distro.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.456335 pur-7.1.1/pur/packages/pip/_vendor/html5lib/
+-rw-r--r--   0 user       (501) staff       (20)     1160 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    16728 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0 user       (501) staff       (20)    32353 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0 user       (501) staff       (20)    77040 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_tokenizer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.457761 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/
+-rw-r--r--   0 user       (501) staff       (20)      109 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1013 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0 user       (501) staff       (20)     1775 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0 user       (501) staff       (20)     4931 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0 user       (501) staff       (20)    83464 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/constants.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.462278 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      919 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0 user       (501) staff       (20)      286 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0 user       (501) staff       (20)     2945 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0 user       (501) staff       (20)     3643 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0 user       (501) staff       (20)    10588 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0 user       (501) staff       (20)    26897 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0 user       (501) staff       (20)     1214 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0 user       (501) staff       (20)   117186 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0 user       (501) staff       (20)    15759 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/serializer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.463619 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/
+-rw-r--r--   0 user       (501) staff       (20)      679 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1715 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0 user       (501) staff       (20)     1776 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/sax.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.465846 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/
+-rw-r--r--   0 user       (501) staff       (20)     3592 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    14565 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0 user       (501) staff       (20)     8925 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0 user       (501) staff       (20)    12836 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0 user       (501) staff       (20)    14766 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.468576 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/
+-rw-r--r--   0 user       (501) staff       (20)     5719 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7476 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0 user       (501) staff       (20)     1413 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0 user       (501) staff       (20)     4551 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0 user       (501) staff       (20)     6357 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0 user       (501) staff       (20)     2309 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/genshi.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.473087 pur-7.1.1/pur/packages/pip/_vendor/idna/
+-rw-r--r--   0 user       (501) staff       (20)      849 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3453 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 user       (501) staff       (20)      360 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 user       (501) staff       (20)    12826 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 user       (501) staff       (20)    42350 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 user       (501) staff       (20)     1933 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 user       (501) staff       (20)       21 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 user       (501) staff       (20)   201849 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/idna/uts46data.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.477755 pur-7.1.1/pur/packages/pip/_vendor/msgpack/
+-rw-r--r--   0 user       (501) staff       (20)     1118 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)       20 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/msgpack/_version.py
+-rw-r--r--   0 user       (501) staff       (20)     1081 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 user       (501) staff       (20)     6088 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 user       (501) staff       (20)    38026 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.513275 pur-7.1.1/pur/packages/pip/_vendor/packaging/
+-rw-r--r--   0 user       (501) staff       (20)      661 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 user       (501) staff       (20)      497 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11488 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 user       (501) staff       (20)     4378 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 user       (501) staff       (20)     1629 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 user       (501) staff       (20)     8487 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 user       (501) staff       (20)     4676 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 user       (501) staff       (20)    30964 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 user       (501) staff       (20)    15714 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 user       (501) staff       (20)     4200 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 user       (501) staff       (20)    14665 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.516905 pur-7.1.1/pur/packages/pip/_vendor/pep517/
+-rw-r--r--   0 user       (501) staff       (20)      130 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3457 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0 user       (501) staff       (20)     6084 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0 user       (501) staff       (20)     4098 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0 user       (501) staff       (20)     1253 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/compat.py
+-rw-r--r--   0 user       (501) staff       (20)     1129 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0 user       (501) staff       (20)     6100 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/envbuild.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.517851 pur-7.1.1/pur/packages/pip/_vendor/pep517/in_process/
+-rw-r--r--   0 user       (501) staff       (20)      563 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11201 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0 user       (501) staff       (20)     2463 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0 user       (501) staff       (20)    13429 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pep517/wrappers.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.519464 pur-7.1.1/pur/packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 user       (501) staff       (20)   108287 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      562 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.523097 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 user       (501) staff       (20)    12871 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1140 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)     3994 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0 user       (501) staff       (20)     4922 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0 user       (501) staff       (20)     2619 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0 user       (501) staff       (20)     6905 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0 user       (501) staff       (20)       80 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0 user       (501) staff       (20)     6416 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/platformdirs/windows.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.525393 pur-7.1.1/pur/packages/pip/_vendor/progress/
+-rw-r--r--   0 user       (501) staff       (20)     5294 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/progress/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2942 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/progress/bar.py
+-rw-r--r--   0 user       (501) staff       (20)     2655 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/progress/colors.py
+-rw-r--r--   0 user       (501) staff       (20)     1613 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/progress/counter.py
+-rw-r--r--   0 user       (501) staff       (20)     1461 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/progress/spinner.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.532928 pur-7.1.1/pur/packages/pip/_vendor/pygments/
+-rw-r--r--   0 user       (501) staff       (20)     3013 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      353 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)    21693 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0 user       (501) staff       (20)     1697 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0 user       (501) staff       (20)     1938 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/filter.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.533420 pur-7.1.1/pur/packages/pip/_vendor/pygments/filters/
+-rw-r--r--   0 user       (501) staff       (20)    40292 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2917 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatter.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.540533 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/
+-rw-r--r--   0 user       (501) staff       (20)     5119 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6348 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 user       (501) staff       (20)     3314 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 user       (501) staff       (20)    34690 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0 user       (501) staff       (20)    21819 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0 user       (501) staff       (20)     5881 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0 user       (501) staff       (20)    18930 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0 user       (501) staff       (20)     5073 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0 user       (501) staff       (20)     2212 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0 user       (501) staff       (20)     5014 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 user       (501) staff       (20)     7335 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0 user       (501) staff       (20)     4686 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 user       (501) staff       (20)    11763 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 user       (501) staff       (20)    31554 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/lexer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.543528 pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/
+-rw-r--r--   0 user       (501) staff       (20)    11307 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    68826 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 user       (501) staff       (20)    51988 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0 user       (501) staff       (20)      986 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0 user       (501) staff       (20)     1727 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)     3072 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0 user       (501) staff       (20)     3091 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0 user       (501) staff       (20)     4630 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0 user       (501) staff       (20)     6025 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/style.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.544452 pur-7.1.1/pur/packages/pip/_vendor/pygments/styles/
+-rw-r--r--   0 user       (501) staff       (20)     3055 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6143 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0 user       (501) staff       (20)    63200 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0 user       (501) staff       (20)     9123 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0 user       (501) staff       (20)   273394 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/pyparsing.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.589705 pur-7.1.1/pur/packages/pip/_vendor/requests/
+-rw-r--r--   0 user       (501) staff       (20)     5130 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      441 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 user       (501) staff       (20)     1096 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 user       (501) staff       (20)    21861 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 user       (501) staff       (20)     6402 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 user       (501) staff       (20)    10207 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 user       (501) staff       (20)      465 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 user       (501) staff       (20)     2114 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 user       (501) staff       (20)    18430 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 user       (501) staff       (20)     3446 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 user       (501) staff       (20)     3972 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 user       (501) staff       (20)      757 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 user       (501) staff       (20)    35116 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 user       (501) staff       (20)      695 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 user       (501) staff       (20)    29835 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 user       (501) staff       (20)     4188 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 user       (501) staff       (20)     3005 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 user       (501) staff       (20)    33301 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.592239 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 user       (501) staff       (20)      537 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.593109 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      156 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 user       (501) staff       (20)     5872 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 user       (501) staff       (20)     1583 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 user       (501) staff       (20)    17592 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 user       (501) staff       (20)     4794 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/resolvelib/structs.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.672993 pur-7.1.1/pur/packages/pip/_vendor/rich/
+-rw-r--r--   0 user       (501) staff       (20)     5804 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     8895 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0 user       (501) staff       (20)    10096 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0 user       (501) staff       (20)   140235 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0 user       (501) staff       (20)     1064 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0 user       (501) staff       (20)      265 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0 user       (501) staff       (20)     7444 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0 user       (501) staff       (20)     3225 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0 user       (501) staff       (20)     1236 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0 user       (501) staff       (20)     1246 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_lru_cache.py
+-rw-r--r--   0 user       (501) staff       (20)     7063 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0 user       (501) staff       (20)      423 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0 user       (501) staff       (20)     5472 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0 user       (501) staff       (20)    26521 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0 user       (501) staff       (20)      351 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0 user       (501) staff       (20)      417 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0 user       (501) staff       (20)     2089 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0 user       (501) staff       (20)     1804 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0 user       (501) staff       (20)      890 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0 user       (501) staff       (20)    10425 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/align.py
+-rw-r--r--   0 user       (501) staff       (20)     6676 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0 user       (501) staff       (20)     3264 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0 user       (501) staff       (20)     9069 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/box.py
+-rw-r--r--   0 user       (501) staff       (20)     3897 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0 user       (501) staff       (20)    17285 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/color.py
+-rw-r--r--   0 user       (501) staff       (20)     1054 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0 user       (501) staff       (20)     7131 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0 user       (501) staff       (20)    80866 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/console.py
+-rw-r--r--   0 user       (501) staff       (20)     1288 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0 user       (501) staff       (20)     5497 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0 user       (501) staff       (20)     5298 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/control.py
+-rw-r--r--   0 user       (501) staff       (20)     6872 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0 user       (501) staff       (20)      183 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0 user       (501) staff       (20)     2501 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0 user       (501) staff       (20)     1657 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0 user       (501) staff       (20)     2511 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0 user       (501) staff       (20)     4894 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0 user       (501) staff       (20)     5051 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/json.py
+-rw-r--r--   0 user       (501) staff       (20)     2856 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0 user       (501) staff       (20)    14048 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0 user       (501) staff       (20)    13933 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/live.py
+-rw-r--r--   0 user       (501) staff       (20)     3670 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0 user       (501) staff       (20)    10862 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0 user       (501) staff       (20)     8057 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0 user       (501) staff       (20)     5258 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0 user       (501) staff       (20)     4778 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0 user       (501) staff       (20)      816 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0 user       (501) staff       (20)     3396 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0 user       (501) staff       (20)     8637 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0 user       (501) staff       (20)    29525 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0 user       (501) staff       (20)    35926 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0 user       (501) staff       (20)     7762 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0 user       (501) staff       (20)    11307 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0 user       (501) staff       (20)     1401 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0 user       (501) staff       (20)      166 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/region.py
+-rw-r--r--   0 user       (501) staff       (20)     4309 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0 user       (501) staff       (20)     4197 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0 user       (501) staff       (20)     2842 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0 user       (501) staff       (20)     1591 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0 user       (501) staff       (20)    20722 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0 user       (501) staff       (20)     4312 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0 user       (501) staff       (20)     4425 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/status.py
+-rw-r--r--   0 user       (501) staff       (20)    26469 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/style.py
+-rw-r--r--   0 user       (501) staff       (20)     1258 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0 user       (501) staff       (20)    26548 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0 user       (501) staff       (20)    34771 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/table.py
+-rw-r--r--   0 user       (501) staff       (20)     1700 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/tabulate.py
+-rw-r--r--   0 user       (501) staff       (20)     1459 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0 user       (501) staff       (20)    41471 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/text.py
+-rw-r--r--   0 user       (501) staff       (20)     3627 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0 user       (501) staff       (20)      102 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0 user       (501) staff       (20)    25896 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0 user       (501) staff       (20)     9122 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0 user       (501) staff       (20)    34549 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/six.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.678211 pur-7.1.1/pur/packages/pip/_vendor/tenacity/
+-rw-r--r--   0 user       (501) staff       (20)    18257 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3314 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0 user       (501) staff       (20)     1944 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0 user       (501) staff       (20)     1496 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0 user       (501) staff       (20)     1376 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0 user       (501) staff       (20)     1908 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0 user       (501) staff       (20)     1383 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0 user       (501) staff       (20)     6645 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0 user       (501) staff       (20)     2790 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0 user       (501) staff       (20)     2145 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0 user       (501) staff       (20)     6691 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tenacity/wait.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.680293 pur-7.1.1/pur/packages/pip/_vendor/tomli/
+-rw-r--r--   0 user       (501) staff       (20)      230 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    22415 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0 user       (501) staff       (20)     2681 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0 user       (501) staff       (20)   109284 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/typing_extensions.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.686174 pur-7.1.1/pur/packages/pip/_vendor/urllib3/
+-rw-r--r--   0 user       (501) staff       (20)     2763 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    10811 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 user       (501) staff       (20)       63 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0 user       (501) staff       (20)    20076 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 user       (501) staff       (20)    39013 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.720716 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      957 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.721606 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    17632 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user       (501) staff       (20)    13922 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user       (501) staff       (20)    11034 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 user       (501) staff       (20)     4538 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user       (501) staff       (20)    16900 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user       (501) staff       (20)    34449 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user       (501) staff       (20)     7097 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 user       (501) staff       (20)     8217 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 user       (501) staff       (20)     8579 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 user       (501) staff       (20)     2440 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.722137 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.722790 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1417 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user       (501) staff       (20)    34666 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0 user       (501) staff       (20)    19763 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 user       (501) staff       (20)     5985 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 user       (501) staff       (20)    28203 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.729039 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 user       (501) staff       (20)     1155 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4901 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 user       (501) staff       (20)     1605 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 user       (501) staff       (20)      498 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 user       (501) staff       (20)     4123 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 user       (501) staff       (20)     3510 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 user       (501) staff       (20)    22001 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 user       (501) staff       (20)    17177 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 user       (501) staff       (20)     5751 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user       (501) staff       (20)     6895 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 user       (501) staff       (20)    10003 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 user       (501) staff       (20)    14047 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 user       (501) staff       (20)     5404 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/wait.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.731385 pur-7.1.1/pur/packages/pip/_vendor/webencodings/
+-rw-r--r--   0 user       (501) staff       (20)    10579 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     8979 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 user       (501) staff       (20)     1305 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 user       (501) staff       (20)     6563 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 user       (501) staff       (20)     4307 2022-04-06 05:15:05.000000 pur-7.1.1/pur/packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0 user       (501) staff       (20)    11025 2023-07-19 01:44:50.000000 pur-7.1.1/pur/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.067232 pur-7.1.1/pur.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     6215 2023-07-19 01:52:36.000000 pur-7.1.1/pur.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)    24382 2023-07-19 01:52:37.000000 pur-7.1.1/pur.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-19 01:52:36.000000 pur-7.1.1/pur.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       41 2023-07-19 01:52:36.000000 pur-7.1.1/pur.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-19 01:51:03.000000 pur-7.1.1/pur.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)       13 2023-07-19 01:52:36.000000 pur-7.1.1/pur.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        4 2023-07-19 01:52:36.000000 pur-7.1.1/pur.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       13 2022-04-06 05:15:05.000000 pur-7.1.1/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-19 01:52:37.733618 pur-7.1.1/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1431 2023-07-19 01:47:57.000000 pur-7.1.1/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-19 01:52:37.731851 pur-7.1.1/tests/
+-rw-r--r--   0 user       (501) staff       (20)    55767 2023-07-19 01:44:50.000000 pur-7.1.1/tests/test_pur.py
```

### Comparing `pur-7.1.0/HISTORY.rst` & `pur-7.1.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 
 History
 -------
 
 
+7.1.1 (2023-07-19)
+++++++++++++++++++
+
+- Format readme as markdown.
+
+
 7.1.0 (2023-03-02)
 ++++++++++++++++++
 
 - New command line options --skip-gt and --dry-run-changed.
   `#50 <https://github.com/alanhamlett/pip-update-requirements/issues/50>`_
```

### Comparing `pur-7.1.0/LICENSE` & `pur-7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/NOTICE` & `pur-7.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/PKG-INFO` & `pur-7.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pur
-Version: 7.1.0
+Version: 7.1.1
 Summary: Update packages in a requirements.txt file to latest versions.
 Home-page: https://github.com/alanhamlett/pip-update-requirements
 Author: Alan Hamlett
 Author-email: alan.hamlett@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,147 +15,121 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-.. image:: https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master
-    :target: https://github.com/alanhamlett/pip-update-requirements/actions
-    :alt: Tests
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master)](https://github.com/alanhamlett/pip-update-requirements/actions)
+[![Coverage](https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS)](https://codecov.io/gh/alanhamlett/pip-update-requirements)
+[![Version](https://img.shields.io/pypi/v/pur.svg)](https://pypi.python.org/pypi/pur)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pur.svg)](https://pypi.python.org/pypi/pur)
+[![WakaTime](https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg)](https://wakatime.com/)
 
-.. image:: https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS
-    :target: https://codecov.io/gh/alanhamlett/pip-update-requirements
-    :alt: Coverage
+# pip-update-requirements
 
-.. image:: https://img.shields.io/pypi/v/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Version
+Update the packages in a `requirements.txt` file.
 
-.. image:: https://img.shields.io/pypi/pyversions/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Supported Python Versions
+![Purring Cat](https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif)
 
-.. image:: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg
-    :target: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements
-
-
-pip-update-requirements
-=======================
-
-Update the packages in a ``requirements.txt`` file.
-
-.. image:: https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif
-    :alt: Purring Cat
-
-
-Installation
-------------
-
-::
+## Installation
 
     pip install pur
 
+## Usage
 
-Usage
------
-
-Give pur your ``requirements.txt`` file and it updates all your packages to
+Give pur your `requirements.txt` file and it updates all your packages to
 the latest versions.
 
-For example, given a ``requirements.txt`` file::
+For example, given a `requirements.txt` file:
 
     flask==0.9
     sqlalchemy==0.9.10
     alembic==0.8.4
 
-Running pur on that file updates the packages to current latest versions::
+Running pur on that file updates the packages to current latest versions:
 
     $ pur -r requirements.txt
     Updated flask: 0.9 -> 1.0.2
     Updated sqlalchemy: 0.9.10 -> 1.2.8
     Updated alembic: 0.8.4 -> 0.9.9
     All requirements up-to-date.
 
 
 Pur never modifies your environment or installed packages, it only modifies
-your ``requirements.txt`` file.
+your `requirements.txt` file.
 
-You can also use Pur directly from Python::
+You can also use Pur directly from Python:
 
     $ python
     Python 3.6.1
     >>> from pur import update_requirements
     >>> print([x[0]['message'] for x in update_requirements(input_file='requirements.txt').values()])
     ['Updated flask: 0.9 -> 1.0.2', 'Updated sqlalchemy: 0.9.10 -> 1.2.8', 'Updated alembic: 0.8.4 -> 0.9.9']
     >>> print(open('requirements.txt').read())
     flask==1.0.2
     sqlalchemy==1.2.8
     alembic==0.9.9
 
 
-Options
--------
-
--r, --requirement PATH   The requirements.txt file to update; Defaults to
-                         using requirements.txt from the current directory
-                         if it exist.
--o, --output PATH        Output updated packages to this file; Defaults to
-                         overwriting the input requirements.txt file.
---interactive            Interactively prompts before updating each package.
--f, --force              Force updating packages even when a package has no
-                         version specified in the input requirements.txt
-                         file.
--d, --dry-run            Output changes to STDOUT instead of overwriting the
-                         requirements.txt file.
---dry-run-changed        When running with --dry-run, only output packages
-                         with updates, not packages that are already the
-                         latest.
--n, --no-recursive       Prevents updating nested requirements files.
---skip TEXT              Comma separated list of packages to skip updating.
---skip-gt                Skip updating packages using > or >= spec, to allow
-                         specifying minimum supported versions of packages.
---index-url TEXT         Base URL of the Python Package Index. Can be
-                         provided multiple times for extra index urls.
---cert PATH              Path to PEM-encoded CA certificate bundle. If
-                         provided, overrides the default.
---no-ssl-verify          Disable verifying the server's TLS certificate.
---only TEXT              Comma separated list of packages. Only these
-                         packages will be updated.
---minor TEXT             Comma separated list of packages to only update
-                         minor versions, never major. Use "*" to limit every
-                         package to minor version updates.
---patch TEXT             Comma separated list of packages to only update
-                         patch versions, never major or minor. Use "*" to
-                         limit every package to patch version updates.
---pre TEXT               Comma separated list of packages to allow updating
-                         to pre-release versions. Use "*" to allow all
-                         packages to be updated to pre-release versions. By
-                         default packages are only updated to stable
-                         versions.
--z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
-                         0 when no packages updated, or a number greater
-                         than 1 when there was an error. By default, exit
-                         status 0 is used unless there was an error
-                         irregardless of whether packages were or not
-                         updated.
---version                Show the version and exit.
---help                   Show this message and exit.
+## Options
 
+    -r, --requirement PATH   The requirements.txt file to update; Defaults to
+                             using requirements.txt from the current directory
+                             if it exist.
+    -o, --output PATH        Output updated packages to this file; Defaults to
+                             overwriting the input requirements.txt file.
+    --interactive            Interactively prompts before updating each package.
+    -f, --force              Force updating packages even when a package has no
+                             version specified in the input requirements.txt
+                             file.
+    -d, --dry-run            Output changes to STDOUT instead of overwriting the
+                             requirements.txt file.
+    --dry-run-changed        When running with --dry-run, only output packages
+                             with updates, not packages that are already the
+                             latest.
+    -n, --no-recursive       Prevents updating nested requirements files.
+    --skip TEXT              Comma separated list of packages to skip updating.
+    --skip-gt                Skip updating packages using > or >= spec, to allow
+                             specifying minimum supported versions of packages.
+    --index-url TEXT         Base URL of the Python Package Index. Can be
+                             provided multiple times for extra index urls.
+    --cert PATH              Path to PEM-encoded CA certificate bundle. If
+                             provided, overrides the default.
+    --no-ssl-verify          Disable verifying the server's TLS certificate.
+    --only TEXT              Comma separated list of packages. Only these
+                             packages will be updated.
+    --minor TEXT             Comma separated list of packages to only update
+                             minor versions, never major. Use "*" to limit every
+                             package to minor version updates.
+    --patch TEXT             Comma separated list of packages to only update
+                             patch versions, never major or minor. Use "*" to
+                             limit every package to patch version updates.
+    --pre TEXT               Comma separated list of packages to allow updating
+                             to pre-release versions. Use "*" to allow all
+                             packages to be updated to pre-release versions. By
+                             default packages are only updated to stable
+                             versions.
+    -z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
+                             0 when no packages updated, or a number greater
+                             than 1 when there was an error. By default, exit
+                             status 0 is used unless there was an error
+                             irregardless of whether packages were or not
+                             updated.
+    --version                Show the version and exit.
+    --help                   Show this message and exit.
 
-Contributing
-------------
+## Contributing
 
-Before contributing a pull request, make sure tests pass::
+Before contributing a pull request, make sure tests pass:
 
     virtualenv venv
     . venv/bin/activate
     pip install tox
     tox
 
-Many thanks to all `contributors <https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS>`_!
-
-
+Many thanks to all [contributors](https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS)!
```

### Comparing `pur-7.1.0/README.rst` & `pur-7.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,109 @@
-.. image:: https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master
-    :target: https://github.com/alanhamlett/pip-update-requirements/actions
-    :alt: Tests
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master)](https://github.com/alanhamlett/pip-update-requirements/actions)
+[![Coverage](https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS)](https://codecov.io/gh/alanhamlett/pip-update-requirements)
+[![Version](https://img.shields.io/pypi/v/pur.svg)](https://pypi.python.org/pypi/pur)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pur.svg)](https://pypi.python.org/pypi/pur)
+[![WakaTime](https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg)](https://wakatime.com/)
 
-.. image:: https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS
-    :target: https://codecov.io/gh/alanhamlett/pip-update-requirements
-    :alt: Coverage
+# pip-update-requirements
 
-.. image:: https://img.shields.io/pypi/v/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Version
+Update the packages in a `requirements.txt` file.
 
-.. image:: https://img.shields.io/pypi/pyversions/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Supported Python Versions
+![Purring Cat](https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif)
 
-.. image:: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg
-    :target: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements
-
-
-pip-update-requirements
-=======================
-
-Update the packages in a ``requirements.txt`` file.
-
-.. image:: https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif
-    :alt: Purring Cat
-
-
-Installation
-------------
-
-::
+## Installation
 
     pip install pur
 
+## Usage
 
-Usage
------
-
-Give pur your ``requirements.txt`` file and it updates all your packages to
+Give pur your `requirements.txt` file and it updates all your packages to
 the latest versions.
 
-For example, given a ``requirements.txt`` file::
+For example, given a `requirements.txt` file:
 
     flask==0.9
     sqlalchemy==0.9.10
     alembic==0.8.4
 
-Running pur on that file updates the packages to current latest versions::
+Running pur on that file updates the packages to current latest versions:
 
     $ pur -r requirements.txt
     Updated flask: 0.9 -> 1.0.2
     Updated sqlalchemy: 0.9.10 -> 1.2.8
     Updated alembic: 0.8.4 -> 0.9.9
     All requirements up-to-date.
 
 
 Pur never modifies your environment or installed packages, it only modifies
-your ``requirements.txt`` file.
+your `requirements.txt` file.
 
-You can also use Pur directly from Python::
+You can also use Pur directly from Python:
 
     $ python
     Python 3.6.1
     >>> from pur import update_requirements
     >>> print([x[0]['message'] for x in update_requirements(input_file='requirements.txt').values()])
     ['Updated flask: 0.9 -> 1.0.2', 'Updated sqlalchemy: 0.9.10 -> 1.2.8', 'Updated alembic: 0.8.4 -> 0.9.9']
     >>> print(open('requirements.txt').read())
     flask==1.0.2
     sqlalchemy==1.2.8
     alembic==0.9.9
 
 
-Options
--------
-
--r, --requirement PATH   The requirements.txt file to update; Defaults to
-                         using requirements.txt from the current directory
-                         if it exist.
--o, --output PATH        Output updated packages to this file; Defaults to
-                         overwriting the input requirements.txt file.
---interactive            Interactively prompts before updating each package.
--f, --force              Force updating packages even when a package has no
-                         version specified in the input requirements.txt
-                         file.
--d, --dry-run            Output changes to STDOUT instead of overwriting the
-                         requirements.txt file.
---dry-run-changed        When running with --dry-run, only output packages
-                         with updates, not packages that are already the
-                         latest.
--n, --no-recursive       Prevents updating nested requirements files.
---skip TEXT              Comma separated list of packages to skip updating.
---skip-gt                Skip updating packages using > or >= spec, to allow
-                         specifying minimum supported versions of packages.
---index-url TEXT         Base URL of the Python Package Index. Can be
-                         provided multiple times for extra index urls.
---cert PATH              Path to PEM-encoded CA certificate bundle. If
-                         provided, overrides the default.
---no-ssl-verify          Disable verifying the server's TLS certificate.
---only TEXT              Comma separated list of packages. Only these
-                         packages will be updated.
---minor TEXT             Comma separated list of packages to only update
-                         minor versions, never major. Use "*" to limit every
-                         package to minor version updates.
---patch TEXT             Comma separated list of packages to only update
-                         patch versions, never major or minor. Use "*" to
-                         limit every package to patch version updates.
---pre TEXT               Comma separated list of packages to allow updating
-                         to pre-release versions. Use "*" to allow all
-                         packages to be updated to pre-release versions. By
-                         default packages are only updated to stable
-                         versions.
--z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
-                         0 when no packages updated, or a number greater
-                         than 1 when there was an error. By default, exit
-                         status 0 is used unless there was an error
-                         irregardless of whether packages were or not
-                         updated.
---version                Show the version and exit.
---help                   Show this message and exit.
+## Options
 
+    -r, --requirement PATH   The requirements.txt file to update; Defaults to
+                             using requirements.txt from the current directory
+                             if it exist.
+    -o, --output PATH        Output updated packages to this file; Defaults to
+                             overwriting the input requirements.txt file.
+    --interactive            Interactively prompts before updating each package.
+    -f, --force              Force updating packages even when a package has no
+                             version specified in the input requirements.txt
+                             file.
+    -d, --dry-run            Output changes to STDOUT instead of overwriting the
+                             requirements.txt file.
+    --dry-run-changed        When running with --dry-run, only output packages
+                             with updates, not packages that are already the
+                             latest.
+    -n, --no-recursive       Prevents updating nested requirements files.
+    --skip TEXT              Comma separated list of packages to skip updating.
+    --skip-gt                Skip updating packages using > or >= spec, to allow
+                             specifying minimum supported versions of packages.
+    --index-url TEXT         Base URL of the Python Package Index. Can be
+                             provided multiple times for extra index urls.
+    --cert PATH              Path to PEM-encoded CA certificate bundle. If
+                             provided, overrides the default.
+    --no-ssl-verify          Disable verifying the server's TLS certificate.
+    --only TEXT              Comma separated list of packages. Only these
+                             packages will be updated.
+    --minor TEXT             Comma separated list of packages to only update
+                             minor versions, never major. Use "*" to limit every
+                             package to minor version updates.
+    --patch TEXT             Comma separated list of packages to only update
+                             patch versions, never major or minor. Use "*" to
+                             limit every package to patch version updates.
+    --pre TEXT               Comma separated list of packages to allow updating
+                             to pre-release versions. Use "*" to allow all
+                             packages to be updated to pre-release versions. By
+                             default packages are only updated to stable
+                             versions.
+    -z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
+                             0 when no packages updated, or a number greater
+                             than 1 when there was an error. By default, exit
+                             status 0 is used unless there was an error
+                             irregardless of whether packages were or not
+                             updated.
+    --version                Show the version and exit.
+    --help                   Show this message and exit.
 
-Contributing
-------------
+## Contributing
 
-Before contributing a pull request, make sure tests pass::
+Before contributing a pull request, make sure tests pass:
 
     virtualenv venv
     . venv/bin/activate
     pip install tox
     tox
 
-Many thanks to all `contributors <https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS>`_!
+Many thanks to all [contributors](https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS)!
```

### Comparing `pur-7.1.0/pur/__init__.py` & `pur-7.1.1/pur/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/__main__.py` & `pur-7.1.1/pur/packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/build_env.py` & `pur-7.1.1/pur/packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cache.py` & `pur-7.1.1/pur/packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/autocompletion.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/base_command.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/cmdoptions.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/command_context.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/main.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/main_parser.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/parser.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/progress_bars.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/req_command.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/cli/spinners.py` & `pur-7.1.1/pur/packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/cache.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/check.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/completion.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/configuration.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/debug.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/download.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/freeze.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/hash.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/help.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/index.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/install.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/list.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/search.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/show.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/uninstall.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/commands/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/configuration.py` & `pur-7.1.1/pur/packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/distributions/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/distributions/base.py` & `pur-7.1.1/pur/packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/distributions/installed.py` & `pur-7.1.1/pur/packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/distributions/sdist.py` & `pur-7.1.1/pur/packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/distributions/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/exceptions.py` & `pur-7.1.1/pur/packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/index/collector.py` & `pur-7.1.1/pur/packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/index/package_finder.py` & `pur-7.1.1/pur/packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/index/sources.py` & `pur-7.1.1/pur/packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/locations/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/locations/_distutils.py` & `pur-7.1.1/pur/packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/locations/_sysconfig.py` & `pur-7.1.1/pur/packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/locations/base.py` & `pur-7.1.1/pur/packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/metadata/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/metadata/base.py` & `pur-7.1.1/pur/packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/metadata/pkg_resources.py` & `pur-7.1.1/pur/packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/candidate.py` & `pur-7.1.1/pur/packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/direct_url.py` & `pur-7.1.1/pur/packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/format_control.py` & `pur-7.1.1/pur/packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/index.py` & `pur-7.1.1/pur/packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/link.py` & `pur-7.1.1/pur/packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/scheme.py` & `pur-7.1.1/pur/packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/search_scope.py` & `pur-7.1.1/pur/packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/selection_prefs.py` & `pur-7.1.1/pur/packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/target_python.py` & `pur-7.1.1/pur/packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/models/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/auth.py` & `pur-7.1.1/pur/packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/cache.py` & `pur-7.1.1/pur/packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/download.py` & `pur-7.1.1/pur/packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/lazy_wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/session.py` & `pur-7.1.1/pur/packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/utils.py` & `pur-7.1.1/pur/packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/network/xmlrpc.py` & `pur-7.1.1/pur/packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata_editable.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/metadata_legacy.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel_editable.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/build/wheel_legacy.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/check.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/freeze.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/install/editable_legacy.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/install/legacy.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/install/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/operations/prepare.py` & `pur-7.1.1/pur/packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/pyproject.py` & `pur-7.1.1/pur/packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/constructors.py` & `pur-7.1.1/pur/packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/req_file.py` & `pur-7.1.1/pur/packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/req_install.py` & `pur-7.1.1/pur/packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/req_set.py` & `pur-7.1.1/pur/packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/req_tracker.py` & `pur-7.1.1/pur/packages/pip/_internal/req/req_tracker.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/req/req_uninstall.py` & `pur-7.1.1/pur/packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/base.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/legacy/resolver.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/base.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/candidates.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/factory.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/provider.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/reporter.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/requirements.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/resolution/resolvelib/resolver.py` & `pur-7.1.1/pur/packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/self_outdated_check.py` & `pur-7.1.1/pur/packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/_log.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/appdirs.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/compat.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/compatibility_tags.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/deprecation.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/direct_url_helpers.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/distutils_args.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/egg_link.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/encoding.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/entrypoints.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/filesystem.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/filetypes.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/glibc.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/hashes.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/inject_securetransport.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/logging.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/misc.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/models.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/packaging.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/setuptools_build.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/subprocess.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/temp_dir.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/unpacking.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/urls.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/virtualenv.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/utils/wheel.py` & `pur-7.1.1/pur/packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/__init__.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/bazaar.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/git.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/mercurial.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/subversion.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/vcs/versioncontrol.py` & `pur-7.1.1/pur/packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_internal/wheel_builder.py` & `pur-7.1.1/pur/packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/_cmd.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/adapter.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/cache.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/controller.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/filewrapper.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/heuristics.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/serialize.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/cachecontrol/wrapper.py` & `pur-7.1.1/pur/packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/certifi/cacert.pem` & `pur-7.1.1/pur/packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/certifi/core.py` & `pur-7.1.1/pur/packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/big5freq.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/big5prober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/chardistribution.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/charsetgroupprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/charsetprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/cli/chardetect.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/codingstatemachine.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/cp949prober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/enums.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/escprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/escsm.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/eucjpprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/euckrfreq.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/euckrprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/euctwfreq.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/euctwprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/gb2312freq.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/gb2312prober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/hebrewprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/jisfreq.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/jpcntx.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langgreekmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langhebrewmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langhungarianmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langrussianmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langthaimodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/langturkishmodel.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/latin1prober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcharsetprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/mbcssm.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/metadata/languages.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/sbcharsetprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/sjisprober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/universaldetector.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/chardet/utf8prober.py` & `pur-7.1.1/pur/packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/colorama/ansi.py` & `pur-7.1.1/pur/packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/colorama/ansitowin32.py` & `pur-7.1.1/pur/packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/colorama/initialise.py` & `pur-7.1.1/pur/packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/colorama/win32.py` & `pur-7.1.1/pur/packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/colorama/winterm.py` & `pur-7.1.1/pur/packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/misc.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/shutil.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/sysconfig.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/_backport/tarfile.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/database.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/index.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/locators.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/manifest.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/markers.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/metadata.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/resources.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/scripts.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/util.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/version.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distlib/wheel.py` & `pur-7.1.1/pur/packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/distro.py` & `pur-7.1.1/pur/packages/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_ihatexml.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_inputstream.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_tokenizer.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/_base.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_trie/py.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/_utils.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/constants.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/lint.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/optionaltags.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/sanitizer.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/filters/whitespace.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/html5parser.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/serializer.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/genshi.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treeadapters/sax.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/base.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/dom.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/etree.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/base.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/dom.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/etree.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/html5lib/treewalkers/genshi.py` & `pur-7.1.1/pur/packages/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/codec.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/core.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/idnadata.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/intranges.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/idna/uts46data.py` & `pur-7.1.1/pur/packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/msgpack/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/msgpack/exceptions.py` & `pur-7.1.1/pur/packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/msgpack/ext.py` & `pur-7.1.1/pur/packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/msgpack/fallback.py` & `pur-7.1.1/pur/packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/__about__.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/_manylinux.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/_musllinux.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/_structures.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/markers.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/requirements.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/specifiers.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/tags.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/utils.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/packaging/version.py` & `pur-7.1.1/pur/packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/build.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/check.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/colorlog.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/dirtools.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/envbuild.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/in_process/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/in_process/_in_process.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/meta.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pep517/wrappers.py` & `pur-7.1.1/pur/packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pkg_resources/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pkg_resources/py31compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/__main__.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/android.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/api.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/macos.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/unix.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/platformdirs/windows.py` & `pur-7.1.1/pur/packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/progress/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/progress/bar.py` & `pur-7.1.1/pur/packages/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/progress/colors.py` & `pur-7.1.1/pur/packages/pip/_vendor/progress/colors.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/progress/counter.py` & `pur-7.1.1/pur/packages/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/progress/spinner.py` & `pur-7.1.1/pur/packages/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/cmdline.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/console.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/filter.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/filters/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatter.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/_mapping.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/bbcode.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/html.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/img.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/irc.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/latex.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/other.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/rtf.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/svg.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/terminal.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/formatters/terminal256.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/lexer.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/_mapping.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/lexers/python.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/modeline.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/plugin.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/regexopt.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/scanner.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/sphinxext.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/style.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/styles/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/token.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/unistring.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pygments/util.py` & `pur-7.1.1/pur/packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/pyparsing.py` & `pur-7.1.1/pur/packages/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/_internal_utils.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/adapters.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/api.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/auth.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/compat.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/cookies.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/exceptions.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/help.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/hooks.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/models.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/packages.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/sessions.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/status_codes.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/structures.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/requests/utils.py` & `pur-7.1.1/pur/packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/resolvelib/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/resolvelib/providers.py` & `pur-7.1.1/pur/packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/resolvelib/reporters.py` & `pur-7.1.1/pur/packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/resolvelib/resolvers.py` & `pur-7.1.1/pur/packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/resolvelib/structs.py` & `pur-7.1.1/pur/packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/__main__.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_cell_widths.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_emoji_codes.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_emoji_replace.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_inspect.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_log_render.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_loop.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_lru_cache.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_palettes.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_ratio.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_spinners.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_windows.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/_wrap.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/abc.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/align.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/ansi.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/bar.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/box.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/cells.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/color.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/color_triplet.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/columns.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/console.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/constrain.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/containers.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/control.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/default_styles.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/emoji.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/errors.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/file_proxy.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/filesize.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/highlighter.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/json.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/jupyter.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/layout.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/live.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/live_render.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/logging.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/markup.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/measure.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/padding.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/pager.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/palette.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/panel.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/pretty.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/progress.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/progress_bar.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/prompt.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/protocol.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/repr.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/rule.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/scope.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/screen.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/segment.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/spinner.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/status.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/style.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/styled.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/syntax.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/table.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/tabulate.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/tabulate.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/terminal_theme.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/text.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/theme.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/traceback.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/rich/tree.py` & `pur-7.1.1/pur/packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/six.py` & `pur-7.1.1/pur/packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/_asyncio.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/_utils.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/after.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/before.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/before_sleep.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/nap.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/retry.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/stop.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/tornadoweb.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tenacity/wait.py` & `pur-7.1.1/pur/packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tomli/_parser.py` & `pur-7.1.1/pur/packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/tomli/_re.py` & `pur-7.1.1/pur/packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/typing_extensions.py` & `pur-7.1.1/pur/packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/_collections.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/connection.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/connectionpool.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/appengine.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/contrib/socks.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/exceptions.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/fields.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/filepost.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/packages/six.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/poolmanager.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/request.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/response.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/connection.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/proxy.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/request.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/response.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/retry.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssl_.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/ssltransport.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/timeout.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/url.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/urllib3/util/wait.py` & `pur-7.1.1/pur/packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/webencodings/__init__.py` & `pur-7.1.1/pur/packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/webencodings/labels.py` & `pur-7.1.1/pur/packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/webencodings/mklabels.py` & `pur-7.1.1/pur/packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/webencodings/tests.py` & `pur-7.1.1/pur/packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/packages/pip/_vendor/webencodings/x_user_defined.py` & `pur-7.1.1/pur/packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur/utils.py` & `pur-7.1.1/pur/utils.py`

 * *Files identical despite different names*

### Comparing `pur-7.1.0/pur.egg-info/PKG-INFO` & `pur-7.1.1/pur.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pur
-Version: 7.1.0
+Version: 7.1.1
 Summary: Update packages in a requirements.txt file to latest versions.
 Home-page: https://github.com/alanhamlett/pip-update-requirements
 Author: Alan Hamlett
 Author-email: alan.hamlett@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,147 +15,121 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-.. image:: https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master
-    :target: https://github.com/alanhamlett/pip-update-requirements/actions
-    :alt: Tests
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/pip-update-requirements/tests.yml?branch=master)](https://github.com/alanhamlett/pip-update-requirements/actions)
+[![Coverage](https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS)](https://codecov.io/gh/alanhamlett/pip-update-requirements)
+[![Version](https://img.shields.io/pypi/v/pur.svg)](https://pypi.python.org/pypi/pur)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pur.svg)](https://pypi.python.org/pypi/pur)
+[![WakaTime](https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg)](https://wakatime.com/)
 
-.. image:: https://codecov.io/gh/alanhamlett/pip-update-requirements/branch/master/graph/badge.svg?token=Ob1I7eMhiS
-    :target: https://codecov.io/gh/alanhamlett/pip-update-requirements
-    :alt: Coverage
+# pip-update-requirements
 
-.. image:: https://img.shields.io/pypi/v/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Version
+Update the packages in a `requirements.txt` file.
 
-.. image:: https://img.shields.io/pypi/pyversions/pur.svg
-    :target: https://pypi.python.org/pypi/pur
-    :alt: Supported Python Versions
+![Purring Cat](https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif)
 
-.. image:: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements.svg
-    :target: https://wakatime.com/badge/github/alanhamlett/pip-update-requirements
-
-
-pip-update-requirements
-=======================
-
-Update the packages in a ``requirements.txt`` file.
-
-.. image:: https://raw.githubusercontent.com/alanhamlett/pip-update-requirements/master/pur.gif
-    :alt: Purring Cat
-
-
-Installation
-------------
-
-::
+## Installation
 
     pip install pur
 
+## Usage
 
-Usage
------
-
-Give pur your ``requirements.txt`` file and it updates all your packages to
+Give pur your `requirements.txt` file and it updates all your packages to
 the latest versions.
 
-For example, given a ``requirements.txt`` file::
+For example, given a `requirements.txt` file:
 
     flask==0.9
     sqlalchemy==0.9.10
     alembic==0.8.4
 
-Running pur on that file updates the packages to current latest versions::
+Running pur on that file updates the packages to current latest versions:
 
     $ pur -r requirements.txt
     Updated flask: 0.9 -> 1.0.2
     Updated sqlalchemy: 0.9.10 -> 1.2.8
     Updated alembic: 0.8.4 -> 0.9.9
     All requirements up-to-date.
 
 
 Pur never modifies your environment or installed packages, it only modifies
-your ``requirements.txt`` file.
+your `requirements.txt` file.
 
-You can also use Pur directly from Python::
+You can also use Pur directly from Python:
 
     $ python
     Python 3.6.1
     >>> from pur import update_requirements
     >>> print([x[0]['message'] for x in update_requirements(input_file='requirements.txt').values()])
     ['Updated flask: 0.9 -> 1.0.2', 'Updated sqlalchemy: 0.9.10 -> 1.2.8', 'Updated alembic: 0.8.4 -> 0.9.9']
     >>> print(open('requirements.txt').read())
     flask==1.0.2
     sqlalchemy==1.2.8
     alembic==0.9.9
 
 
-Options
--------
-
--r, --requirement PATH   The requirements.txt file to update; Defaults to
-                         using requirements.txt from the current directory
-                         if it exist.
--o, --output PATH        Output updated packages to this file; Defaults to
-                         overwriting the input requirements.txt file.
---interactive            Interactively prompts before updating each package.
--f, --force              Force updating packages even when a package has no
-                         version specified in the input requirements.txt
-                         file.
--d, --dry-run            Output changes to STDOUT instead of overwriting the
-                         requirements.txt file.
---dry-run-changed        When running with --dry-run, only output packages
-                         with updates, not packages that are already the
-                         latest.
--n, --no-recursive       Prevents updating nested requirements files.
---skip TEXT              Comma separated list of packages to skip updating.
---skip-gt                Skip updating packages using > or >= spec, to allow
-                         specifying minimum supported versions of packages.
---index-url TEXT         Base URL of the Python Package Index. Can be
-                         provided multiple times for extra index urls.
---cert PATH              Path to PEM-encoded CA certificate bundle. If
-                         provided, overrides the default.
---no-ssl-verify          Disable verifying the server's TLS certificate.
---only TEXT              Comma separated list of packages. Only these
-                         packages will be updated.
---minor TEXT             Comma separated list of packages to only update
-                         minor versions, never major. Use "*" to limit every
-                         package to minor version updates.
---patch TEXT             Comma separated list of packages to only update
-                         patch versions, never major or minor. Use "*" to
-                         limit every package to patch version updates.
---pre TEXT               Comma separated list of packages to allow updating
-                         to pre-release versions. Use "*" to allow all
-                         packages to be updated to pre-release versions. By
-                         default packages are only updated to stable
-                         versions.
--z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
-                         0 when no packages updated, or a number greater
-                         than 1 when there was an error. By default, exit
-                         status 0 is used unless there was an error
-                         irregardless of whether packages were or not
-                         updated.
---version                Show the version and exit.
---help                   Show this message and exit.
+## Options
 
+    -r, --requirement PATH   The requirements.txt file to update; Defaults to
+                             using requirements.txt from the current directory
+                             if it exist.
+    -o, --output PATH        Output updated packages to this file; Defaults to
+                             overwriting the input requirements.txt file.
+    --interactive            Interactively prompts before updating each package.
+    -f, --force              Force updating packages even when a package has no
+                             version specified in the input requirements.txt
+                             file.
+    -d, --dry-run            Output changes to STDOUT instead of overwriting the
+                             requirements.txt file.
+    --dry-run-changed        When running with --dry-run, only output packages
+                             with updates, not packages that are already the
+                             latest.
+    -n, --no-recursive       Prevents updating nested requirements files.
+    --skip TEXT              Comma separated list of packages to skip updating.
+    --skip-gt                Skip updating packages using > or >= spec, to allow
+                             specifying minimum supported versions of packages.
+    --index-url TEXT         Base URL of the Python Package Index. Can be
+                             provided multiple times for extra index urls.
+    --cert PATH              Path to PEM-encoded CA certificate bundle. If
+                             provided, overrides the default.
+    --no-ssl-verify          Disable verifying the server's TLS certificate.
+    --only TEXT              Comma separated list of packages. Only these
+                             packages will be updated.
+    --minor TEXT             Comma separated list of packages to only update
+                             minor versions, never major. Use "*" to limit every
+                             package to minor version updates.
+    --patch TEXT             Comma separated list of packages to only update
+                             patch versions, never major or minor. Use "*" to
+                             limit every package to patch version updates.
+    --pre TEXT               Comma separated list of packages to allow updating
+                             to pre-release versions. Use "*" to allow all
+                             packages to be updated to pre-release versions. By
+                             default packages are only updated to stable
+                             versions.
+    -z, --nonzero-exit-code  Exit with status 1 when some packages were updated,
+                             0 when no packages updated, or a number greater
+                             than 1 when there was an error. By default, exit
+                             status 0 is used unless there was an error
+                             irregardless of whether packages were or not
+                             updated.
+    --version                Show the version and exit.
+    --help                   Show this message and exit.
 
-Contributing
-------------
+## Contributing
 
-Before contributing a pull request, make sure tests pass::
+Before contributing a pull request, make sure tests pass:
 
     virtualenv venv
     . venv/bin/activate
     pip install tox
     tox
 
-Many thanks to all `contributors <https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS>`_!
-
-
+Many thanks to all [contributors](https://github.com/alanhamlett/pip-update-requirements/blob/master/AUTHORS)!
```

### Comparing `pur-7.1.0/pur.egg-info/SOURCES.txt` & `pur-7.1.1/pur.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AUTHORS
 HISTORY.rst
 LICENSE
 MANIFEST.in
 NOTICE
-README.rst
+README.md
 requirements.txt
 setup.py
 pur/__about__.py
 pur/__init__.py
 pur/__main__.py
 pur/exceptions.py
 pur/utils.py
@@ -520,8 +520,9 @@
 pur/packages/pip/_vendor/urllib3/util/timeout.py
 pur/packages/pip/_vendor/urllib3/util/url.py
 pur/packages/pip/_vendor/urllib3/util/wait.py
 pur/packages/pip/_vendor/webencodings/__init__.py
 pur/packages/pip/_vendor/webencodings/labels.py
 pur/packages/pip/_vendor/webencodings/mklabels.py
 pur/packages/pip/_vendor/webencodings/tests.py
-pur/packages/pip/_vendor/webencodings/x_user_defined.py
+pur/packages/pip/_vendor/webencodings/x_user_defined.py
+tests/test_pur.py
```

### Comparing `pur-7.1.0/setup.py` & `pur-7.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 install_requires = [x.strip() for x in open('requirements.txt').readlines()]
 
 setup(
     name=about['__title__'],
     version=about['__version__'],
     license=about['__license__'],
     description=about['__description__'],
-    long_description=open('README.rst').read(),
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
     author=about['__author__'],
     author_email=about['__author_email__'],
     url=about['__url__'],
     packages=packages,
     package_dir={about['__title__']: about['__title__']},
     include_package_data=True,
     zip_safe=False,
```

