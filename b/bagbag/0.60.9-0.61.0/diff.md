# Comparing `tmp/bagbag-0.60.9.tar.gz` & `tmp/bagbag-0.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.60.9.tar", max compression
+gzip compressed data, was "bagbag-0.61.0.tar", max compression
```

## Comparing `bagbag-0.60.9.tar` & `bagbag-0.61.0.tar`

### file list

```diff
@@ -1,253 +1,261 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.60.9/LICENSE
--rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.60.9/README.md
--rw-r--r--   0        0        0     2244 2023-06-15 08:44:30.864112 bagbag-0.60.9/pyproject.toml
--rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.60.9/src/bagbag/Base64/__init__.py
--rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.60.9/src/bagbag/Base64/src.py
--rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.60.9/src/bagbag/Cmd/__init__.py
--rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.60.9/src/bagbag/Cmd/src.py
--rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.60.9/src/bagbag/Cryptoo/__init__.py
--rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.60.9/src/bagbag/Cryptoo/src.py
--rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.60.9/src/bagbag/File/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-02 17:04:32.821610 bagbag-0.60.9/src/bagbag/File/src.py
--rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.60.9/src/bagbag/Funcs/CutSentenceStopWords_src.py
--rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.60.9/src/bagbag/Funcs/CutSentence_src.py
--rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.60.9/src/bagbag/Funcs/FakeIdentity_src.py
--rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.60.9/src/bagbag/Funcs/FileType_src.py
--rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.60.9/src/bagbag/Funcs/Format/__init__.py
--rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.60.9/src/bagbag/Funcs/Format/src.py
--rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.60.9/src/bagbag/Funcs/GetPublicIP_src.py
--rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.60.9/src/bagbag/Funcs/IPAddressConvert_src.py
--rw-r--r--   0        0        0      227 2023-05-12 12:35:25.858029 bagbag-0.60.9/src/bagbag/Funcs/Markdown_src.py
--rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.60.9/src/bagbag/Funcs/Ping_src.py
--rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.60.9/src/bagbag/Funcs/ResizeImage_src.py
--rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.60.9/src/bagbag/Funcs/UUID_src.py
--rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.60.9/src/bagbag/Funcs/Wget_src.py
--rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.60.9/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.60.9/src/bagbag/Hash/__init__.py
--rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.60.9/src/bagbag/Hash/src.py
--rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.60.9/src/bagbag/Http/__init__.py
--rw-r--r--   0        0        0    13444 2023-05-16 06:55:50.470768 bagbag-0.60.9/src/bagbag/Http/src.py
--rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.60.9/src/bagbag/Json/__init__.py
--rw-r--r--   0        0        0     3271 2023-05-16 06:24:06.059824 bagbag-0.60.9/src/bagbag/Json/src.py
--rw-r--r--   0        0        0    10860 2023-06-01 07:11:48.733272 bagbag-0.60.9/src/bagbag/Lg.py
--rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.60.9/src/bagbag/Math/__init__.py
--rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.60.9/src/bagbag/Math/src.py
--rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.60.9/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-15 13:15:56.167334 bagbag-0.60.9/src/bagbag/Os/Path/src.py
--rw-r--r--   0        0        0      859 2023-05-16 12:14:50.048628 bagbag-0.60.9/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     2933 2023-05-12 12:35:25.859730 bagbag-0.60.9/src/bagbag/Os/src.py
--rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.60.9/src/bagbag/Process/__init__.py
--rw-r--r--   0        0        0      958 2023-06-01 07:09:48.165713 bagbag-0.60.9/src/bagbag/Process/src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.60.9/src/bagbag/Python/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 08:44:09.543096 bagbag-0.60.9/src/bagbag/Python/src.py
--rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.60.9/src/bagbag/Random/__init__.py
--rw-r--r--   0        0        0      700 2023-06-01 06:55:49.958227 bagbag-0.60.9/src/bagbag/Random/src.py
--rw-r--r--   0        0        0      379 2023-05-12 12:35:25.860322 bagbag-0.60.9/src/bagbag/Socket/TCP/__init__.py
--rw-r--r--   0        0        0     4850 2023-05-12 12:35:25.860244 bagbag-0.60.9/src/bagbag/Socket/TCP/src.py
--rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.60.9/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.60.9/src/bagbag/String/__init__.py
--rw-r--r--   0        0        0    16761 2023-06-01 06:54:57.084155 bagbag-0.60.9/src/bagbag/String/src.py
--rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.60.9/src/bagbag/Thread/__init__.py
--rw-r--r--   0        0        0      437 2023-06-01 07:09:39.456063 bagbag-0.60.9/src/bagbag/Thread/src.py
--rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.60.9/src/bagbag/Time/__init__.py
--rw-r--r--   0        0        0     6061 2023-06-15 06:30:18.558975 bagbag-0.60.9/src/bagbag/Time/src.py
--rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.60.9/src/bagbag/Tools/Argparser_src.py
--rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
--rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
--rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    23255 2023-05-12 12:35:25.824849 bagbag-0.60.9/src/bagbag/Tools/BlockChain/Tron/src.py
--rw-r--r--   0        0        0      393 2023-05-12 12:35:25.824665 bagbag-0.60.9/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-05 15:36:04.503828 bagbag-0.60.9/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     4615 2023-06-09 06:22:43.542806 bagbag-0.60.9/src/bagbag/Tools/Cache.py
--rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.60.9/src/bagbag/Tools/Chan_src.py
--rw-r--r--   0        0        0    32941 2023-05-29 11:13:19.619696 bagbag-0.60.9/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3238 2023-05-29 11:10:20.747420 bagbag-0.60.9/src/bagbag/Tools/Crontab_src.py
--rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.60.9/src/bagbag/Tools/Database/__init__.py
--rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.60.9/src/bagbag/Tools/Database/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.60.9/src/bagbag/Tools/Database/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.60.9/src/bagbag/Tools/Database/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.60.9/src/bagbag/Tools/Database/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.60.9/src/bagbag/Tools/Database/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.60.9/src/bagbag/Tools/Database/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/url.py
--rw-r--r--   0        0        0    33340 2023-05-17 12:21:58.241698 bagbag-0.60.9/src/bagbag/Tools/Database/src.py
--rw-r--r--   0        0        0     5250 2023-05-29 11:10:33.731697 bagbag-0.60.9/src/bagbag/Tools/DistributedLock_src.py
--rw-r--r--   0        0        0     4674 2023-05-29 11:10:40.751258 bagbag-0.60.9/src/bagbag/Tools/Elasticsearch_src.py
--rw-r--r--   0        0        0     4312 2023-05-29 11:10:51.912539 bagbag-0.60.9/src/bagbag/Tools/Github_src.py
--rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.60.9/src/bagbag/Tools/JavaScript_src.py
--rw-r--r--   0        0        0    10096 2023-06-09 08:35:54.469473 bagbag-0.60.9/src/bagbag/Tools/Kafka_src.py
--rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.60.9/src/bagbag/Tools/Lock_src.py
--rw-r--r--   0        0        0     6634 2023-05-29 11:11:12.945317 bagbag-0.60.9/src/bagbag/Tools/MatrixBot_src.py
--rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.60.9/src/bagbag/Tools/Nslookup_src.py
--rw-r--r--   0        0        0     2364 2023-05-29 11:11:50.231133 bagbag-0.60.9/src/bagbag/Tools/OCR_src.py
--rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.60.9/src/bagbag/Tools/ProgressBar_src.py
--rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.60.9/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3337 2023-06-07 15:52:43.922791 bagbag-0.60.9/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.60.9/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.60.9/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2607 2023-05-29 11:12:14.997684 bagbag-0.60.9/src/bagbag/Tools/Queue_src.py
--rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.60.9/src/bagbag/Tools/RSS/Feed.py
--rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.60.9/src/bagbag/Tools/RSS/Opml.py
--rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.60.9/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.60.9/src/bagbag/Tools/Ratelimit_src.py
--rw-r--r--   0        0        0    18451 2023-05-29 11:12:03.251797 bagbag-0.60.9/src/bagbag/Tools/Redis_src.py
--rw-r--r--   0        0        0     5565 2023-05-12 12:35:25.820157 bagbag-0.60.9/src/bagbag/Tools/SSH_src.py
--rw-r--r--   0        0        0    34161 2023-06-06 10:04:38.686181 bagbag-0.60.9/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.60.9/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.60.9/src/bagbag/Tools/TelegramBotOfficial_src.py
--rw-r--r--   0        0        0     3069 2023-06-14 11:27:42.444891 bagbag-0.60.9/src/bagbag/Tools/TelegramBot_src.py
--rw-r--r--   0        0        0    24676 2023-06-13 19:08:29.204793 bagbag-0.60.9/src/bagbag/Tools/Telegram_src.py
--rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.60.9/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.60.9/src/bagbag/Tools/Translater_src.py
--rw-r--r--   0        0        0     6622 2023-06-06 11:56:02.475141 bagbag-0.60.9/src/bagbag/Tools/Twitter/Browser_src.py
--rw-r--r--   0        0        0    11332 2023-06-15 08:09:28.766900 bagbag-0.60.9/src/bagbag/Tools/Twitter/Elevated_src.py
--rw-r--r--   0        0        0     2093 2023-05-26 13:18:47.657372 bagbag-0.60.9/src/bagbag/Tools/Twitter/Essential_src.py
--rw-r--r--   0        0        0      794 2023-06-15 07:42:19.924782 bagbag-0.60.9/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.60.9/src/bagbag/Tools/URL_src.py
--rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.60.9/src/bagbag/Tools/WaitGroup_src.py
--rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.60.9/src/bagbag/Tools/WebCrawler_src.py
--rw-r--r--   0        0        0     5572 2023-05-12 12:35:25.818682 bagbag-0.60.9/src/bagbag/Tools/WebServer_src.py
--rw-r--r--   0        0        0     1702 2023-05-12 12:35:25.819763 bagbag-0.60.9/src/bagbag/Tools/XPath_src.py
--rw-r--r--   0        0        0     3235 2023-05-16 08:49:31.768572 bagbag-0.60.9/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     3522 2023-06-15 06:42:23.529284 bagbag-0.60.9/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0     4553 2023-06-15 08:44:21.499293 bagbag-0.60.9/src/bagbag/__init__.py
--rw-r--r--   0        0        0    19722 1970-01-01 00:00:00.000000 bagbag-0.60.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.61.0/LICENSE
+-rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.61.0/README.md
+-rw-r--r--   0        0        0     2244 2023-07-19 12:53:58.434599 bagbag-0.61.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.61.0/src/bagbag/Base64/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.61.0/src/bagbag/Base64/src.py
+-rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.61.0/src/bagbag/Cmd/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.61.0/src/bagbag/Cmd/src.py
+-rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.61.0/src/bagbag/Cryptoo/__init__.py
+-rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.61.0/src/bagbag/Cryptoo/src.py
+-rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.61.0/src/bagbag/File/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-02 17:04:32.821610 bagbag-0.61.0/src/bagbag/File/src.py
+-rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.61.0/src/bagbag/Funcs/CutSentenceStopWords_src.py
+-rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.61.0/src/bagbag/Funcs/CutSentence_src.py
+-rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.61.0/src/bagbag/Funcs/FakeIdentity_src.py
+-rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.61.0/src/bagbag/Funcs/FileType_src.py
+-rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.61.0/src/bagbag/Funcs/Format/__init__.py
+-rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.61.0/src/bagbag/Funcs/Format/src.py
+-rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.61.0/src/bagbag/Funcs/GetPublicIP_src.py
+-rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.61.0/src/bagbag/Funcs/IPAddressConvert_src.py
+-rw-r--r--   0        0        0      227 2023-05-12 12:35:25.858029 bagbag-0.61.0/src/bagbag/Funcs/Markdown_src.py
+-rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.61.0/src/bagbag/Funcs/Ping_src.py
+-rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.61.0/src/bagbag/Funcs/ResizeImage_src.py
+-rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.61.0/src/bagbag/Funcs/UUID_src.py
+-rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.61.0/src/bagbag/Funcs/Wget_src.py
+-rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.61.0/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.61.0/src/bagbag/Hash/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.61.0/src/bagbag/Hash/src.py
+-rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.61.0/src/bagbag/Http/__init__.py
+-rw-r--r--   0        0        0    13444 2023-07-19 11:28:27.616005 bagbag-0.61.0/src/bagbag/Http/src.py
+-rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.61.0/src/bagbag/Json/__init__.py
+-rw-r--r--   0        0        0     3271 2023-05-16 06:24:06.059824 bagbag-0.61.0/src/bagbag/Json/src.py
+-rw-r--r--   0        0        0    10860 2023-06-16 14:21:52.035937 bagbag-0.61.0/src/bagbag/Lg.py
+-rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.61.0/src/bagbag/Math/__init__.py
+-rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.61.0/src/bagbag/Math/src.py
+-rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.61.0/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-15 13:15:56.167334 bagbag-0.61.0/src/bagbag/Os/Path/src.py
+-rw-r--r--   0        0        0      917 2023-06-16 05:44:53.093812 bagbag-0.61.0/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     3257 2023-06-16 05:44:20.429520 bagbag-0.61.0/src/bagbag/Os/src.py
+-rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.61.0/src/bagbag/Process/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-15 09:27:23.720590 bagbag-0.61.0/src/bagbag/Process/src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.61.0/src/bagbag/Python/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 08:44:09.543096 bagbag-0.61.0/src/bagbag/Python/src.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.61.0/src/bagbag/Random/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-01 06:55:49.958227 bagbag-0.61.0/src/bagbag/Random/src.py
+-rw-r--r--   0        0        0      379 2023-05-12 12:35:25.860322 bagbag-0.61.0/src/bagbag/Socket/TCP/__init__.py
+-rw-r--r--   0        0        0     4850 2023-05-12 12:35:25.860244 bagbag-0.61.0/src/bagbag/Socket/TCP/src.py
+-rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.61.0/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.61.0/src/bagbag/String/__init__.py
+-rw-r--r--   0        0        0    16972 2023-07-18 06:50:49.901739 bagbag-0.61.0/src/bagbag/String/src.py
+-rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.61.0/src/bagbag/Thread/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-15 09:24:51.853905 bagbag-0.61.0/src/bagbag/Thread/src.py
+-rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.61.0/src/bagbag/Time/__init__.py
+-rw-r--r--   0        0        0     6061 2023-06-15 06:30:18.558975 bagbag-0.61.0/src/bagbag/Time/src.py
+-rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.61.0/src/bagbag/Tools/Argparser_src.py
+-rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
+-rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    24277 2023-07-06 05:43:43.753694 bagbag-0.61.0/src/bagbag/Tools/BlockChain/Tron/src.py
+-rw-r--r--   0        0        0      381 2023-07-04 14:12:42.665691 bagbag-0.61.0/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-05 15:36:04.503828 bagbag-0.61.0/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     4615 2023-06-09 06:22:43.542806 bagbag-0.61.0/src/bagbag/Tools/Cache.py
+-rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.61.0/src/bagbag/Tools/Chan_src.py
+-rw-r--r--   0        0        0    32941 2023-05-29 11:13:19.619696 bagbag-0.61.0/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3238 2023-05-29 11:10:20.747420 bagbag-0.61.0/src/bagbag/Tools/Crontab_src.py
+-rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.61.0/src/bagbag/Tools/Database/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.61.0/src/bagbag/Tools/Database/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.61.0/src/bagbag/Tools/Database/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.61.0/src/bagbag/Tools/Database/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.61.0/src/bagbag/Tools/Database/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.61.0/src/bagbag/Tools/Database/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.61.0/src/bagbag/Tools/Database/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/url.py
+-rw-r--r--   0        0        0    33362 2023-07-03 09:42:07.366549 bagbag-0.61.0/src/bagbag/Tools/Database/src.py
+-rw-r--r--   0        0        0     5250 2023-05-29 11:10:33.731697 bagbag-0.61.0/src/bagbag/Tools/DistributedLock_src.py
+-rw-r--r--   0        0        0     4674 2023-05-29 11:10:40.751258 bagbag-0.61.0/src/bagbag/Tools/Elasticsearch_src.py
+-rw-r--r--   0        0        0     4312 2023-05-29 11:10:51.912539 bagbag-0.61.0/src/bagbag/Tools/Github_src.py
+-rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.61.0/src/bagbag/Tools/JavaScript_src.py
+-rw-r--r--   0        0        0    10096 2023-06-09 08:35:54.469473 bagbag-0.61.0/src/bagbag/Tools/Kafka_src.py
+-rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.61.0/src/bagbag/Tools/Lock_src.py
+-rw-r--r--   0        0        0     6634 2023-05-29 11:11:12.945317 bagbag-0.61.0/src/bagbag/Tools/MatrixBot_src.py
+-rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.61.0/src/bagbag/Tools/Nslookup_src.py
+-rw-r--r--   0        0        0     2364 2023-05-29 11:11:50.231133 bagbag-0.61.0/src/bagbag/Tools/OCR_src.py
+-rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.61.0/src/bagbag/Tools/ProgressBar_src.py
+-rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.61.0/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3337 2023-06-07 15:52:43.922791 bagbag-0.61.0/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.61.0/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.61.0/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2607 2023-05-29 11:12:14.997684 bagbag-0.61.0/src/bagbag/Tools/Queue_src.py
+-rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.61.0/src/bagbag/Tools/RSS/Feed.py
+-rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.61.0/src/bagbag/Tools/RSS/Opml.py
+-rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.61.0/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.61.0/src/bagbag/Tools/Ratelimit_src.py
+-rw-r--r--   0        0        0    18451 2023-05-29 11:12:03.251797 bagbag-0.61.0/src/bagbag/Tools/Redis_src.py
+-rw-r--r--   0        0        0     5609 2023-07-09 07:33:46.935788 bagbag-0.61.0/src/bagbag/Tools/SSH_src.py
+-rw-r--r--   0        0        0    34757 2023-07-18 07:42:48.217790 bagbag-0.61.0/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.61.0/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.61.0/src/bagbag/Tools/TelegramBotOfficial_src.py
+-rw-r--r--   0        0        0     3069 2023-06-14 11:27:42.444891 bagbag-0.61.0/src/bagbag/Tools/TelegramBot_src.py
+-rw-r--r--   0        0        0    24676 2023-06-13 19:08:29.204793 bagbag-0.61.0/src/bagbag/Tools/Telegram_src.py
+-rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.61.0/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.61.0/src/bagbag/Tools/Translater_src.py
+-rw-r--r--   0        0        0    14103 2023-06-19 07:22:24.505061 bagbag-0.61.0/src/bagbag/Tools/Twitter/Browser_src.py
+-rw-r--r--   0        0        0    12718 2023-07-18 12:42:14.412719 bagbag-0.61.0/src/bagbag/Tools/Twitter/Elevated_src.py
+-rw-r--r--   0        0        0     2093 2023-05-26 13:18:47.657372 bagbag-0.61.0/src/bagbag/Tools/Twitter/Essential_src.py
+-rw-r--r--   0        0        0    20615 2023-07-19 12:52:48.687542 bagbag-0.61.0/src/bagbag/Tools/Twitter/Nitter_src.py
+-rw-r--r--   0        0        0     2744 2023-06-16 08:15:42.223073 bagbag-0.61.0/src/bagbag/Tools/Twitter/Utils.py
+-rw-r--r--   0        0        0     1070 2023-07-19 12:53:41.487474 bagbag-0.61.0/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0    21999 2023-07-17 13:14:08.084943 bagbag-0.61.0/src/bagbag/Tools/Twitter/tweet.html
+-rw-r--r--   0        0        0     6518 2023-07-18 07:38:02.613302 bagbag-0.61.0/src/bagbag/Tools/Twitter/user.1.html
+-rw-r--r--   0        0        0    39119 2023-07-19 07:32:27.254484 bagbag-0.61.0/src/bagbag/Tools/Twitter/user.2.html
+-rw-r--r--   0        0        0      548 2023-07-19 11:32:50.558274 bagbag-0.61.0/src/bagbag/Tools/Twitter/user.3.html
+-rw-r--r--   0        0        0    38911 2023-07-19 06:43:56.243558 bagbag-0.61.0/src/bagbag/Tools/Twitter/user.html
+-rw-r--r--   0        0        0   529900 2023-07-18 12:17:16.113734 bagbag-0.61.0/src/bagbag/Tools/Twitter/user.json
+-rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.61.0/src/bagbag/Tools/URL_src.py
+-rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.61.0/src/bagbag/Tools/WaitGroup_src.py
+-rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.61.0/src/bagbag/Tools/WebCrawler_src.py
+-rw-r--r--   0        0        0     7040 2023-07-16 17:07:37.080346 bagbag-0.61.0/src/bagbag/Tools/WebServer_src.py
+-rw-r--r--   0        0        0     2434 2023-07-19 07:21:05.031779 bagbag-0.61.0/src/bagbag/Tools/XPath_src.py
+-rw-r--r--   0        0        0     3235 2023-05-16 08:49:31.768572 bagbag-0.61.0/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     3528 2023-07-04 14:13:58.807237 bagbag-0.61.0/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0     4555 2023-06-17 10:44:24.595347 bagbag-0.61.0/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    19722 1970-01-01 00:00:00.000000 bagbag-0.61.0/PKG-INFO
```

### Comparing `bagbag-0.60.9/LICENSE` & `bagbag-0.61.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/README.md` & `bagbag-0.61.0/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/pyproject.toml` & `bagbag-0.61.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.60.9"
+version = "0.61.0"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
```

### Comparing `bagbag-0.60.9/src/bagbag/Cmd/src.py` & `bagbag-0.61.0/src/bagbag/Cmd/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Cryptoo/src.py` & `bagbag-0.61.0/src/bagbag/Cryptoo/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/File/src.py` & `bagbag-0.61.0/src/bagbag/File/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/CutSentenceStopWords_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/CutSentenceStopWords_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/CutSentence_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/CutSentence_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/FakeIdentity_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/FakeIdentity_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/FileType_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/FileType_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/Format/src.py` & `bagbag-0.61.0/src/bagbag/Funcs/Format/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/GetPublicIP_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/GetPublicIP_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/Ping_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/Ping_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/ResizeImage_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/ResizeImage_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/Wget_src.py` & `bagbag-0.61.0/src/bagbag/Funcs/Wget_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Funcs/__init__.py` & `bagbag-0.61.0/src/bagbag/Funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Hash/__init__.py` & `bagbag-0.61.0/src/bagbag/Hash/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Hash/src.py` & `bagbag-0.61.0/src/bagbag/Hash/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Http/__init__.py` & `bagbag-0.61.0/src/bagbag/Http/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Http/src.py` & `bagbag-0.61.0/src/bagbag/Http/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Json/src.py` & `bagbag-0.61.0/src/bagbag/Json/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Lg.py` & `bagbag-0.61.0/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Math/src.py` & `bagbag-0.61.0/src/bagbag/Math/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Os/Path/__init__.py` & `bagbag-0.61.0/src/bagbag/Os/Path/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Os/Path/src.py` & `bagbag-0.61.0/src/bagbag/Os/Path/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Os/__init__.py` & `bagbag-0.61.0/src/bagbag/Os/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         "Getcwd",
         "Unlink",
         "Move",
         "Copy",
         "GetLoginUserName",
         "Walk",
         "GetUID",
-        "Args"
+        "Args",
+        "GetCurrentThreadID"
     ],
     "Path": ["Path"]
 }
 
 if TYPE_CHECKING:
     from .src import (
         Exit,
@@ -34,15 +35,16 @@
         Getcwd,
         Unlink,
         Move,
         Copy,
         GetLoginUserName,
         Walk,
         GetUID,
-        Args
+        Args,
+        GetCurrentThreadID
     )
     from . import Path
 else:
     sys.modules[__name__] = LazyImporter(
         __name__,
         globals()["__file__"],
         _import_structure,
```

### Comparing `bagbag-0.60.9/src/bagbag/Os/src.py` & `bagbag-0.61.0/src/bagbag/Os/src.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import sys 
 import shutil
 import glob
 import subprocess
+import threading
+import multiprocessing
+import re
 
 print("load os")
 
 def Exit(num:int=0):
     sys.exit(num)
 
 def System(cmd:str) -> int:
@@ -99,13 +102,16 @@
         elif type == "d":
             for name in dirs:
                 yield os.path.join(root, name)
 
 def GetUID() -> int:
     return os.getuid()
 
+def GetCurrentThreadID() -> str:
+    return multiprocessing.current_process().name.replace("Process-", "P").replace("MainProcess", "MP") + re.sub("\([a-zA-Z0-9]+\)", "", threading.current_thread().name.replace("Thread-", "T").replace(" ", "").replace("MainThread", "MT")) 
+
 if __name__ == "__main__":
     # Move("a", "b") # 移动当前目录的a到b
     # Move("b", "c/d/e") # 移动b到c/d/e, 会先递归创建目录c/d
     # Move("c/d/e", "d") # 移动c/d/e文件到d目录, 没有指定文件名就自动使用原来的文件名
     for i in Walk(".", type="d"):
         print(i)
```

### Comparing `bagbag-0.60.9/src/bagbag/Python/src.py` & `bagbag-0.61.0/src/bagbag/Python/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Random/src.py` & `bagbag-0.61.0/src/bagbag/Random/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Socket/TCP/src.py` & `bagbag-0.61.0/src/bagbag/Socket/TCP/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/String/src.py` & `bagbag-0.61.0/src/bagbag/String/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ## print("load string")
+import typing 
 
 sentimentAnalyzer = None
 
 addrPattern = {
     "xmr":      "4[0-9AB][1-9A-HJ-NP-Za-km-z]{93}",
     "bech32":   "bc(0([ac-hj-np-z02-9]{39}|[ac-hj-np-z02-9]{59})|1[ac-hj-np-z02-9]{8,87})",
     "eth":      "(0x)[a-zA-Z0-9]{40}",
@@ -73,21 +74,23 @@
     def __repr__(self) -> str:
         return f"sentimentResult(Negative={self.Negative} Neutral={self.Neutral} Positive={self.Positive} Compound={self.Compound})"
 
     def __str__(self) -> str:
         return f"sentimentResult(Negative={self.Negative} Neutral={self.Neutral} Positive={self.Positive} Compound={self.Compound})"
 
 class String():
-    def __init__(self, string:str):
-        self.string = string 
-    
-        """
-        > If there are any Chinese characters in the string, return `True`. Otherwise, return `False`
-        :return: A boolean value.
-        """
+    def __init__(self, string:typing.Any):
+        self.string = str(string)
+
+    def IsDigit(self) -> bool:
+        try:
+            float(self.string)
+            return True
+        except ValueError:
+            return False
     
     def Sentiment(self) -> sentimentResult:
         global sentimentAnalyzer
         if sentimentAnalyzer == None:
             from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
             sentimentAnalyzer = SentimentIntensityAnalyzer()
 
@@ -249,14 +252,22 @@
         import pypinyin
         res = pypinyin.lazy_pinyin(self.string, style=pypinyin.Style.TONE3)
         py = String(('-'.join(res)).replace(" ", "-")).Filter('1234567890qwertyuioplkjhgfdsazxcvbnmQWERTYUIOPLKJHGFDSAZXCVBNM -').replace('--', '-')
         return py
     
     def EnsureUTF8(self) -> str:
         return self.string.encode('utf-8', errors='ignore').decode('utf-8')
+    
+    def HTMLDecode(self) -> str:
+        import html
+        return html.unescape(self.string)
+    
+    def HTMLEncode(self) -> str:
+        import html
+        return html.escape(self.string)
 
     def URLEncode(self) -> str:
         from urllib.parse import quote_plus
         return quote_plus(self.string)
     
     def URLDecode(self) -> str:
         from urllib.parse import unquote
```

### Comparing `bagbag-0.60.9/src/bagbag/Time/__init__.py` & `bagbag-0.61.0/src/bagbag/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Time/src.py` & `bagbag-0.61.0/src/bagbag/Time/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Argparser_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Argparser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py` & `bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py` & `bagbag-0.61.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/BlockChain/Tron/src.py` & `bagbag-0.61.0/src/bagbag/Tools/BlockChain/Tron/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
         self.GitHub:str = None 
         self.TotalSupplyWithDecimals:int = None 
         self.GreyTag:str = None 
         self.RedTag:str = None 
         self.PublicTag:str = None 
         self.BlueTag:str = None 
         self.TokenType:str = None 
+        self.Reputation:str = None 
         # self.TokenInfo:tronContractTokenInfo = None 
     
     def __str__(self) -> str:
         m = "tronContractInfo("
         m += f"ContractAddress={self.ContractAddress} "
         m += f"ContractName={self.ContractName} "
         m += f"Symbol={self.Symbol} "
@@ -192,26 +193,34 @@
         m += f"WhitePaper={self.WhitePaper} "
         m += f"GitHub={self.GitHub} "
         m += f"TotalSupplyWithDecimals={self.TotalSupplyWithDecimals} "
         m += f"GreyTag={self.GreyTag} "
         m += f"RedTag={self.RedTag} "
         m += f"PublicTag={self.PublicTag} "
         m += f"BlueTag={self.BlueTag} "
-        m += f"TokenType={self.TokenType}"
+        m += f"TokenType={self.TokenType} "
+        m += f"Reputation={self.Reputation}"
         # m += f"TokenInfo={self.TokenInfo}"
         m += ")"
 
         return m
     
     def __repr__(self) -> str:
         return self.__str__()
 
 class TronContract():
     def __init__(self, address:str) -> None:
         self.address = address 
+        self.ReputationMap = {
+            0: "Unknown",
+            1: "Neutral",
+            2: "OK",
+            3: "Suspicious",
+            4: "Unsafe"
+        }
     
     def Address(self) -> str:
         return self.address 
     
     def Info(self) -> tronContractInfo:
         hresp = Http.Get("https://apilist.tronscanapi.com/api/token_trc20?contract=%s&showAll=1" % self.address, timeoutRetryTimes=999)
         content = hresp.Content
@@ -224,15 +233,15 @@
 
         rd = None 
         for rd in contentj['trc20_tokens']:
             if self.address == rd['contract_address']:
                 break 
 
         if rd != None:
-            troncontractinfo.raw_data = contentj
+            troncontractinfo.raw_data = [contentj]
 
             troncontractinfo.ContractAddress = rd['contract_address']
             troncontractinfo.ContractName = rd['contract_name']
             troncontractinfo.Symbol = rd['symbol']
             troncontractinfo.Name = rd['name']
             troncontractinfo.IssueAddress = rd['issue_address']
             troncontractinfo.IssueTime = Time.Strptime(rd['issue_time'])
@@ -245,14 +254,31 @@
             troncontractinfo.GitHub = rd['git_hub']
             troncontractinfo.TotalSupplyWithDecimals = rd['total_supply_with_decimals'] 
             troncontractinfo.GreyTag = rd["greyTag"]
             troncontractinfo.RedTag = rd["redTag"]
             troncontractinfo.PublicTag = rd['publicTag']
             troncontractinfo.BlueTag = rd['blueTag']
             troncontractinfo.TokenType = rd['tokenType']
+
+            content = Http.Get("https://apilist.tronscanapi.com/api/contract?contract=%s&type=contract" % self.address, timeoutRetryTimes=999).Content
+            contentj = Json.Loads(content)
+
+            troncontractinfo.raw_data.append(contentj)
+
+            rd = None 
+            for rr in contentj['data']:
+                if self.address == rr['address']:
+                    rd = rr
+                    break 
+            
+            try:
+                troncontractinfo.Reputation = self.ReputationMap[int(rd['tokenInfo']['tokenLevel'])]
+            except:
+                pass 
+
         else:
             content = Http.Get("https://apilist.tronscanapi.com/api/contract?contract=%s&type=contract" % self.address, timeoutRetryTimes=999).Content
             contentj = Json.Loads(content)
 
             rd = None 
             for rr in contentj['data']:
                 if self.address == rr['address']:
@@ -269,14 +295,19 @@
                 troncontractinfo.IssueTime = rd['date_created'] / 1000
                 troncontractinfo.IssueAddress = rd['creator']['address']
                 troncontractinfo.Name = rd['name']
                 troncontractinfo.GreyTag = rd["greyTag"]
                 troncontractinfo.RedTag = rd["redTag"]
                 troncontractinfo.PublicTag = rd['publicTag']
                 troncontractinfo.BlueTag = rd['blueTag']
+
+                try:
+                    troncontractinfo.Reputation = self.ReputationMap[int(rd['tokenInfo']['tokenLevel'])]
+                except:
+                    pass 
                 
                 # ti = tronContractTokenInfo()
 
                 # if 'tokenInfo' in rd:
                 #     tidi = rd['tokenInfo']
                 #     ti.raw_data = tidi
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/CSV.py` & `bagbag-0.61.0/src/bagbag/Tools/CSV.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Cache.py` & `bagbag-0.61.0/src/bagbag/Tools/Cache.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Chan_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Chan_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.61.0/src/bagbag/Tools/ComputerVision.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Crontab_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Crontab_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/__init__.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/application.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/models/make_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/connection.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/connection_interface.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/mysql_connection.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/postgres_connection.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/connection_factory.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/connector.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/database_manager.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/column.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/column_diff.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/comparator.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/index.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/schema_manager.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/table.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/dbal/table_diff.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/events/__init__.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/connectors.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/exceptions/orm.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/migration_creator.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/migrator.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/migrations/stubs.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/builder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/collection.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/factory.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/factory_builder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/model.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_one.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/pivot.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/relation.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/result.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/orm/utils.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/base.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/pagination/paginator.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/builder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/join_clause.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/query/processors/processor.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/blueprint.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/builder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/mysql_builder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/schema/schema.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/seeds/seeder.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/fluent.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/support/grammar.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/__init__.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/command_formatter.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/helpers.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/qmarker.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/orator/utils/url.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Database/src.py` & `bagbag-0.61.0/src/bagbag/Tools/Database/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,16 @@
 
     @initTableObj
     def OrWhereIn(self, key:str, value: list) -> mySQLSQLiteTable:
         self.table[self._id()] = self.table[self._id()].or_where_in(key, value)
         return self
 
     @initTableObj
-    def OrderBy(self, *key:str) -> mySQLSQLiteTable:
-        self.table[self._id()] = self.table[self._id()].order_by(*key)
+    def OrderBy(self, key:str, order:str="asc") -> mySQLSQLiteTable:
+        self.table[self._id()] = self.table[self._id()].order_by(key, order)
         return self 
 
     @initTableObj
     def Limit(self, num:int) -> mySQLSQLiteTable:
         self.table[self._id()] = self.table[self._id()].limit(num)
         return self
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/DistributedLock_src.py` & `bagbag-0.61.0/src/bagbag/Tools/DistributedLock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Elasticsearch_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Elasticsearch_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Github_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Github_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/JavaScript_src.py` & `bagbag-0.61.0/src/bagbag/Tools/JavaScript_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Kafka_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Kafka_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Lock_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Lock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/MatrixBot_src.py` & `bagbag-0.61.0/src/bagbag/Tools/MatrixBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/OCR_src.py` & `bagbag-0.61.0/src/bagbag/Tools/OCR_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/ProgressBar_src.py` & `bagbag-0.61.0/src/bagbag/Tools/ProgressBar_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.61.0/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.61.0/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.61.0/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Queue_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Queue_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/RSS/Feed.py` & `bagbag-0.61.0/src/bagbag/Tools/RSS/Feed.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/RSS/Opml.py` & `bagbag-0.61.0/src/bagbag/Tools/RSS/Opml.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Ratelimit_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Ratelimit_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Redis_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Redis_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/SSH_src.py` & `bagbag-0.61.0/src/bagbag/Tools/SSH_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         # 自动接收Host Key
         self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
         self.sshcfg = paramiko.SSHConfig()
         # 载入~/.ssh/config 
         if Os.Getenv("HOME"):
             cfgpath = Os.Path.Join(Os.Getenv("HOME"), ".ssh/config")
-            self.sshcfg.parse(open(cfgpath))
+            if Os.Path.Exists(cfgpath):
+                self.sshcfg.parse(open(cfgpath))
 
         hostcfg = self.sshcfg.lookup(host)
 
         # 用配置文件解析一下host的ip, 如果配置文件没写就用传入的参数
         host = hostcfg["hostname"]
         # print(f"host: {host}")
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Selenium.py` & `bagbag-0.61.0/src/bagbag/Tools/Selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from seleniumwire import webdriver as seleniumwirewebdriver
 from seleniumwire.utils import decode as decodeResponseBody
 
 import time
 import random
 import typing
+import copy
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 from ..Http import useragents 
 from .. import Lg
 from ..Thread import Thread
 from .URL_src import URL
@@ -513,15 +514,15 @@
         :return: The index of the xpath that is found.
         """
         if type(xpath[0]) == list:
             xpath = xpath[0]
             
         for _ in range(timeout*2):
             for x in range(len(xpath)):
-                if self._find(xpath[x], 0, scrollIntoElement=False):
+                if self._find(xpath[x], 0, scrollIntoElement=False) != None:
                     return x
             time.sleep(0.5)
 
         return None 
     
     def SwitchTabByID(self, number:int):
         """
@@ -685,22 +686,22 @@
         body = String(String(self.Body).Repr()).Ommit(80)
         return f"seleniumFlowResponse(Time={self.Time}, StatusCode={self.StatusCode}, Headers={self.Headers} Body={body})"
 
     def __str__(self) -> str:
         body = String(String(self.Body).Repr()).Ommit(80)
         return f"seleniumFlowResponse(Time={self.Time}, StatusCode={self.StatusCode}, Headers={self.Headers} Body={body})"
 
-class seleniumFlow():
+class SeleniumFlow():
     def __init__(self,id:str, req:seleniumFlowRequest, resp:seleniumFlowResponse) -> None:
         self.Request = req
         self.Response = resp
         self.ID = id
     
     def __repr__(self) -> str:
-        return f"seleniumFlow(\n\tID={self.ID} \n\tRequest={self.Request} \n\tResponse={self.Response}\n)" 
+        return f"SeleniumFlow(\n\tID={self.ID} \n\tRequest={self.Request} \n\tResponse={self.Response}\n)" 
 
 class ChromeWire(seleniumBase):
     def __init__(self, 
             blockSuffix:tuple[str]=seleniumChromeWireSkipFilesSuffix,
             maxRequests:int=None, 
             requestStorage:str="disk", # memory
             urlFilterRegex:list[str]=[], 
@@ -797,26 +798,44 @@
         
         self.ResizeWindow(1400, 1400)
         
         self.browserName = "chromewire"
         self.browserRemote = False
         self.closed = False
         self.blockSuffix = blockSuffix
+
+        self.tmpCacheFlows = []
     
-    def Flows(self, clean:bool=True) -> typing.Iterable[seleniumFlow]:
+    def Flows(self, clean:bool=True) -> typing.Iterable[SeleniumFlow]:
         """
-        > It iterates through all the requests made by the browser, and returns a `seleniumFlow` object
+        > It iterates through all the requests made by the browser, and returns a `SeleniumFlow` object
         for each request. 
         这个方法迭代现有的队列里面的数据, 当到达末尾的时候就结束迭代. 
         可以多次调用这个方法来获取新的flow. 
         注意打开某些页面之后, 浏览器会隔一段时间就发起一次请求, 及时没有新Get页面, 也会有新的flow出现. 
         如果是发起了请求, 但是还在等待回复, 或者正在传送大的回复回来, 则response为None, 在控制台看到的是在pending. 拿到完整的回复才会显示, 一瞬间刷出来.
         如果是连接出错, 有request, 但response也还是为None. 
         """
-        for req in self.driver.requests:
+        while True:
+            Lg.Trace()
+            # for req in self.tmpCacheFlows:
+            if len(self.tmpCacheFlows) == 0:
+                time.sleep(1)
+                if len(self.driver.requests) == 0:
+                    break 
+
+                self.tmpCacheFlows = copy.deepcopy(self.driver.requests)
+                Lg.Trace()
+                if clean:
+                    Lg.Trace()
+                    del(self.driver.requests)
+                Lg.Trace()
+            
+            req = self.tmpCacheFlows.pop(0)
+
             if self.blockSuffix != None and len(self.blockSuffix) != 0:
                 if req.path.lower().endswith(self.blockSuffix):
                     continue
 
             resp = req.response
 
             freq = seleniumFlowRequest()
@@ -860,18 +879,20 @@
                     #     else:
                     #         Lg.Warn("未知的 Content-Encoding:", fresp.Headers['content-encoding'])
                     #         fresp.Body = resp.body.decode(errors="ignore")
                     #         fresp.BodyBytes = resp.body 
             else:
                 fresp = None 
 
-            yield seleniumFlow(req.id, freq, fresp)
-        
-        if clean:
-            del(self.driver.requests)
+            Lg.Trace()
+            yield SeleniumFlow(req.id, freq, fresp)
+
+            if len(self.tmpCacheFlows) == 0:
+                Lg.Trace()
+                break 
 
 if __name__ == "__main__":
     # Local 
     # with Chrome() as se:
     # Remote 
     # with Chrome("http://127.0.0.1:4444") as se:
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.61.0/src/bagbag/Tools/TelegramAsync.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/TelegramBotOfficial_src.py` & `bagbag-0.61.0/src/bagbag/Tools/TelegramBotOfficial_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/TelegramBot_src.py` & `bagbag-0.61.0/src/bagbag/Tools/TelegramBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Telegram_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Telegram_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Translater_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Translater_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Twitter/Elevated_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Twitter/Elevated_src.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import tweepy
 import typing 
+from . import Utils
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class ElevatedTwitterUser():
     def __init__(self) -> None:
         # https://developer.twitter.com/en/docs/twitter-api/v1/data-dictionary/object-model/user
         self.ID:int = None 
@@ -13,25 +14,26 @@
         self.Location:str = None 
         self.RegisterTime:int = None 
         self.Description:str = None 
         self.URL:str = None
         self.FollowersCount:int = None 
         self.StatusesCount:int = None 
         self.Verified:bool = None 
-        self.ListedCount:int = None 
+        self.ListedCount:int = None # The number of public lists that this user is a member of.
         self.FavoriteCount:int = None 
+        self.FriendsCount:int = None # 当前用户去follow别人的个数
         self.raw_data:dict = None 
 
     # def Tweet(self, )
         
     def __repr__(self) -> str:
-        return f"ElevatedTwitterUser(ID={self.ID} Name={self.Name} ScreenName={self.ScreenName} Location={self.Location} RegisterTime={self.RegisterTime} URL={self.URL} Description={self.Description} FollowersCount={self.FollowersCount} StatusesCount={self.StatusesCount} Verified={self.Verified})"
+        return f"ElevatedTwitterUser(ID={self.ID} Name={self.Name} ScreenName={self.ScreenName} Location={self.Location} RegisterTime={self.RegisterTime} URL={self.URL} Description={self.Description} FollowersCount={self.FollowersCount} StatusesCount={self.StatusesCount} Verified={self.Verified} ListedCount={self.ListedCount} FavoriteCount={self.FavoriteCount})"
 
     def __str__(self) -> str:
-        return f"ElevatedTwitterUser(ID={self.ID} Name={self.Name} ScreenName={self.ScreenName} Location={self.Location} RegisterTime={self.RegisterTime} URL={self.URL} Description={self.Description} FollowersCount={self.FollowersCount} StatusesCount={self.StatusesCount} Verified={self.Verified})"
+        return f"ElevatedTwitterUser(ID={self.ID} Name={self.Name} ScreenName={self.ScreenName} Location={self.Location} RegisterTime={self.RegisterTime} URL={self.URL} Description={self.Description} FollowersCount={self.FollowersCount} StatusesCount={self.StatusesCount} Verified={self.Verified} ListedCount={self.ListedCount} FavoriteCount={self.FavoriteCount})"
 
 class ElevatedTwitterUserMention():
     def __init__(self) -> None:
         self.ScreenName:str = None 
         self.Name:str = None 
         self.ID:int = None 
     
@@ -69,47 +71,61 @@
 
     def InReplyToTweet(self) -> ElevatedTweet | None:
         if self.in_reply_to_tweet_id == None:
             return None 
         
         return self.twitter.Tweet(self.in_reply_to_tweet_id)
 
-    def Replies(self) -> list[ElevatedTweet]:
-        res = []
+    def Replies(self, checkcount:int=None) -> typing.Iterator[ElevatedTweet]:
+        """
+        通过采集回复当前发这个推文的用户的推文, 来筛选这个推文是否是回复当前这条推文的推文.
+        checkcount是最大采集多少条"回复当前发这个推文的用户的推文", 不是会返回的推文条数.
+        """
         # print(75, "to:" + self.User.ScreenName)
+        count = 0
         for t in self.twitter.Search("to:" + self.User.ScreenName):
             # print(77, t)
             # print(t.in_reply_to_status_id, self.ID)
             # print(type(t.in_reply_to_status_id), type(self.ID))
             if t.in_reply_to_tweet_id == self.ID:
-                res.append(t)
+                yield t
             # print('')
-
-        return res
+            count += 1
+            if checkcount != None and count > checkcount:
+                return 
 
 class Elevated():
     def __init__(self, consumer_key:str, consumer_secret:str) -> None:
         auth = tweepy.OAuth2AppHandler(consumer_key, consumer_secret)
 
         self.api = tweepy.API(auth, wait_on_rate_limit=True)
     
     def _wrapUser(self, user) -> ElevatedTwitterUser:
         u = ElevatedTwitterUser()
         u.ID = user.id
         u.Name = user.name
         u.ScreenName = user.screen_name
         u.Location = user.location
         u.Description = user.description
-        u.URL = user.url
+        if type(user.url) == str:
+            if user.url.startswith("https://t.co/") or user.url.startswith("http://t.co/"):
+                realurl = Utils.GetRealUrl(user.url)
+                if realurl == None:
+                    u.URL = user.url
+                else:
+                    u.URL = realurl
+            else:
+                u.URL = user.url
         u.RegisterTime = int(user.created_at.timestamp())
         u.FollowersCount = user.followers_count
         u.StatusesCount = user.statuses_count
         u.Verified = user.verified
         u.ListedCount = user.listed_count
         u.FavoriteCount = user.favourites_count
+        u.FriendsCount = user.friends_count
         u.raw_data = user._json
 
         # import ipdb
         # ipdb.set_trace()
 
         return u
     
@@ -230,26 +246,37 @@
     
     def Followers(self, screename:str, countPerRequest:int=40) -> typing.Iterable[ElevatedTwitterUser]:
         for user in tweepy.Cursor(self.api.get_followers, screen_name=screename, count=countPerRequest).items():
             # import ipdb
             # ipdb.set_trace()
             yield self._wrapUser(user)
     
-    def User(self, screenameOrID:str|int) -> ElevatedTwitterUser:
+    def User(self, screenameOrID:str|int) -> ElevatedTwitterUser | None:
         """
         It takes a screen name or id and returns a ElevatedTwitterUser object
         
         :param screename: The screen name of the user for whom to return results for
         :type screename: str
         :return: A ElevatedTwitterUser object
         """
-        if type(screenameOrID) == str:
-            user = self.api.get_user(screen_name=screenameOrID)
-        elif type(screenameOrID) == int:
-            user = self.api.get_user(user_id=screenameOrID)
+        try:
+            if type(screenameOrID) == str:
+                user = self.api.get_user(screen_name=screenameOrID)
+            elif type(screenameOrID) == int:
+                user = self.api.get_user(user_id=screenameOrID)
+            else:
+                return None 
+        except tweepy.errors.Forbidden as e:
+            if 'User has been suspended' in str(e):
+                return None 
+            else:
+                raise e
+        except tweepy.errors.NotFound:
+            return None 
+            
         # import ipdb
         # ipdb.set_trace()
         return self._wrapUser(user)
 
     def Tweet(self, tid:int) -> ElevatedTweet:
         return self._wrapStatus(self.api.get_status(tid, tweet_mode = "extended"))
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Twitter/Essential_src.py` & `bagbag-0.61.0/src/bagbag/Tools/Twitter/Essential_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/URL_src.py` & `bagbag-0.61.0/src/bagbag/Tools/URL_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/WaitGroup_src.py` & `bagbag-0.61.0/src/bagbag/Tools/WaitGroup_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/WebCrawler_src.py` & `bagbag-0.61.0/src/bagbag/Tools/WebCrawler_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/WebServer_src.py` & `bagbag-0.61.0/src/bagbag/Tools/WebServer_src.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from flask import Flask
+from __future__ import annotations
+
+from flask import Flask, Blueprint
 from flask import request
 import flask
 from flask import abort, redirect
 from flask import render_template, send_file
 
-try:
-    from .. import Random
-    from ..Thread import Thread
-    from .. import Lg
-except:
-    import sys 
-    sys.path.append("..")
-    import Random
-    from Thread import Thread
-    import Lg
+from .. import Random
+from ..Thread import Thread
+from .. import Lg
+from .. import String
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 import logging 
     
 class LoggingMiddleware(object):
     def __init__(self, app):
@@ -79,14 +75,20 @@
     
     def Data(self) -> str:
         return request.get_data().decode("utf-8")
 
     def DataBytes(self) -> bytes:
         return request.get_data()
 
+class Prefix():
+    def __init__(self, webserver:WebServer, path:str) -> None:
+        self.webserver = webserver
+        self.path = path 
+        self.Route = self.webserver.blueprints[self.path].route
+
 class WebServer():
     def __init__(self, debug:bool=True, additionDebug:bool=False, name:str=None):
         """
         It creates a Flask app with a random name.
         
         :param debug: If set to True, the server will reload itself on code changes and provide a
         helpful debugger in case of application errors, defaults to True
@@ -99,36 +101,53 @@
         if not name:
             name = Random.String()
 
         self.app = Flask(name)
         self.Route = self.app.route 
         self.Request = Request()
         self.Response = Response()
+        self.BeforeRequest = self.app.before_request
+        self.AfterRequest = self.app.after_request
 
         if debug == False:
             log = logging.getLogger('werkzeug')
             log.disabled = True
         
         if additionDebug:
             self.app.wsgi_app = LoggingMiddleware(self.app.wsgi_app)
         
+        self.blueprints:dict[str, Blueprint] = {}
+    
+    def Prefix(self, path:str) -> Prefix:
+        blueprint = Blueprint(String(path).Filter(), __name__)
+        self.blueprints[path] = blueprint
+
+        # self.app.register_blueprint(blueprint, url_prefix=path) # 注册之后再添加的url路由是不生效的
+
+        prefix = Prefix(self, path)
+        return prefix
+        
     def Run(self, host:str="0.0.0.0", port:int=None, block:bool=True):
         """
         Runs the Flask app on the specified host and port, optionally in a separate thread
         If block is False then debug will always be False
         
         :param host: The hostname to listen on. Set this to '0.0.0.0' to have the server available
         externally as well. Defaults to '127.0.0.1' or 'localhost'
         :type host: str
         :param port: The port to run the server on
         :type port: int
         :param block: If True, the server will run in the main thread. If False, it will run in a
         separate thread, defaults to True
         :type block: bool (optional)
         """
+
+        for path in self.blueprints:
+            self.app.register_blueprint(self.blueprints[path], url_prefix=path)
+
         if not port:
             port = Random.Int(10000, 60000)
             
         if block:
             self.app.run(host, port, False)
         else:
             Thread(self.app.run, host, port, False)
@@ -177,8 +196,31 @@
     w2 = WebServer()
 
     @w2.Route("/")
     def index2():
         # print(w.Request.Headers())
         return "Hello World 2!" 
     
+    prefix = w2.Prefix("/a/test/prefix")
+
+    @prefix.Route("suffix")
+    def prefix():
+        return "prefix"
+    
+    prefix = w2.Prefix("/prefix")
+
+    @prefix.Route("/suffix") # /prefix/suffix
+    def suffix():
+        return "suffix"
+    
+    @w2.BeforeRequest
+    def beforereq():
+        Lg.Trace("before request")
+        # return "200 OK" # 返回非None的值则直接返回这个response给client, 不再执行之后的handler
+        return None # 返回None则执行之后的handler
+        
+    @w2.AfterRequest
+    def afterreq(response): # 其他handler返回的response
+        Lg.Trace("after request:", response)
+        return response # 一定要回一个response, 否则报错500
+        
     w2.Run("0.0.0.0", 8081) # Block here
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/XPath_src.py` & `bagbag-0.61.0/src/bagbag/Tools/XPath_src.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,59 @@
 from __future__ import annotations
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 import lxml.html 
+import lxml.html.soupparser
 
 class XPath():
     def __init__(self, html:str|lxml.html.HtmlElement):
         if type(html) == str:
-            self.root = lxml.html.fromstring(html)
+            try:
+                self.root = lxml.html.fromstring(html)
+            except:
+                self.root = lxml.html.soupparser.fromstring(html)
         elif type(html) == lxml.html.HtmlElement:
             self.root = html 
         else:
             raise Exception("Unsupport type: ", str(type(html)))
     
-    def Find(self, xpath:str) -> XPath | None:
+    def _find(self, xpath:str) -> XPath | None:
         """
         > If the xpath is found, return the first matched XPath object, otherwise return None
         
         :param xpath: The XPath expression to search for
         :type xpath: str
         :return: XPath object
         """
         res = self.root.xpath(xpath)
         if len(res) == 0:
             return None 
         else:
-            return XPath(res[0])
+            return XPath(lxml.html.tostring(res[0]).decode('utf-8'))
+    
+    def Find(self, xpath:str|list) -> XPath | None:
+        if type(xpath) == str:
+            return self._find(xpath)
+        else:
+            idx = self.Except(xpath)
+            if idx == None:
+                return None 
+            else:
+                return self._find(xpath[idx])
+    
+    def Except(self, *xpath:str|list) -> int | None:
+        if type(xpath[0]) == list:
+            xpath = xpath[0]
+            
+        for x in range(len(xpath)):
+            if self._find(xpath[x]) != None:
+                return x
+
+        return None 
     
     def Attribute(self, name:str) -> str | None:
         """
         If the attribute name is in the element, return the attribute value, otherwise return None
         
         :param name: The name of the attribute to get
         :type name: str
```

### Comparing `bagbag-0.60.9/src/bagbag/Tools/Xlsx.py` & `bagbag-0.61.0/src/bagbag/Tools/Xlsx.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.60.9/src/bagbag/Tools/__init__.py` & `bagbag-0.61.0/src/bagbag/Tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "BlockChain": ["BlockChain"], 
     "JavaScript": ["JavaScript"],
     # from . import ComputerVision
     "ComputerVision": ["ComputerVision"],
     "WebCrawler_src": ["WebCrawler"],
     "OCR_src": ["OCR"],
     # "File_src": ["File"],
-    "Selenium": ["Selenium"],
+    "Selenium": ["Selenium", "SeleniumFlow"],
     "CSV": ["CSV"],
     "Prometheus": ['Prometheus'],
     "Cache": ["Cache"]
 }
 
 if TYPE_CHECKING:
     # from ..File_src import File
@@ -86,15 +86,15 @@
     from .Queue_src import Queue
     from .RSS import RSS
     from .MatrixBot_src import MatrixBot
     from .Nslookup_src import Nslookup
     from . import Twitter
     from .DistributedLock_src import DistributedLock
     # from .Test import Test
-    from .BlockChain import BlockChain
+    from . import BlockChain
     from .JavaScript_src import JavaScript
     from .ComputerVision import ComputerVision
     from .WebCrawler_src import WebCrawler
     from .OCR_src import OCR
 else:
     sys.modules[__name__] = LazyImporter(
         __name__,
```

### Comparing `bagbag-0.60.9/src/bagbag/__init__.py` & `bagbag-0.61.0/src/bagbag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # Lg.Trace(Size(process.memory_info().rss))
 
 from . import Funcs
 # Lg.Trace(Size(process.memory_info().rss))
 from . import Tools
 # Lg.Trace(Size(process.memory_info().rss))
 
-from .File import File
+# from .File import File
 
 # 
 # 如果导入包是from bagbag import * 则lazyimport无效, 如果是import bagbag 就有效
 # 
 # from typing import TYPE_CHECKING
 # from lazy_imports import LazyImporter
 # import sys
```

### Comparing `bagbag-0.60.9/PKG-INFO` & `bagbag-0.61.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.60.9
+Version: 0.61.0
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

