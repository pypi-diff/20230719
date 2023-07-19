# Comparing `tmp/pydantic_core-2.2.0.tar.gz` & `tmp/pydantic_core-2.3.0.tar.gz`

## Comparing `pydantic_core-2.2.0.tar` & `pydantic_core-2.3.0.tar`

### file list

```diff
@@ -1,206 +1,206 @@
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 pydantic_core-2.2.0/Cargo.toml
--rw-r--r--   0     1001      123      312 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/.cargo/config.toml
--rw-r--r--   0     1001      123     1080 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/LICENSE
--rw-r--r--   0     1001      123     5052 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/Makefile
--rw-r--r--   0     1001      123     3704 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/README.md
--rw-r--r--   0     1001      123     1366 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/build.rs
--rw-r--r--   0     1001      123     8313 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/generate_self_schema.py
--rw-r--r--   0     1001      123     3340 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/pyproject.toml
--rw-r--r--   0     1001      123     3065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/argument_markers.rs
--rw-r--r--   0     1001      123     5811 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/build_tools.rs
--rw-r--r--   0     1001      123     4486 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/definitions.rs
--rw-r--r--   0     1001      123     5441 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/line_error.rs
--rw-r--r--   0     1001      123     7101 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/location.rs
--rw-r--r--   0     1001      123     1065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/mod.rs
--rw-r--r--   0     1001      123    33615 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/types.rs
--rw-r--r--   0     1001      123    17567 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/validation_exception.rs
--rw-r--r--   0     1001      123     5046 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/errors/value_exception.rs
--rw-r--r--   0     1001      123    13976 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/datetime.rs
--rw-r--r--   0     1001      123     8292 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_abstract.rs
--rw-r--r--   0     1001      123    18291 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_json.rs
--rw-r--r--   0     1001      123    26556 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/input_python.rs
--rw-r--r--   0     1001      123      981 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/mod.rs
--rw-r--r--   0     1001      123     7700 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/parse_json.rs
--rw-r--r--   0     1001      123    32794 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/return_enums.rs
--rw-r--r--   0     1001      123     3426 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/input/shared.rs
--rw-r--r--   0     1001      123     1756 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lazy_index_map.rs
--rw-r--r--   0     1001      123     3556 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lib.rs
--rw-r--r--   0     1001      123    17853 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/lookup_key.rs
--rw-r--r--   0     1001      123     2484 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/recursion_guard.rs
--rw-r--r--   0     1001      123     5605 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/computed_fields.rs
--rw-r--r--   0     1001      123     5486 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/config.rs
--rw-r--r--   0     1001      123     2779 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/errors.rs
--rw-r--r--   0     1001      123    11523 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/extra.rs
--rw-r--r--   0     1001      123    12294 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/fields.rs
--rw-r--r--   0     1001      123    14578 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/filter.rs
--rw-r--r--   0     1001      123    25393 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/infer.rs
--rw-r--r--   0     1001      123     7814 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/mod.rs
--rw-r--r--   0     1001      123    11222 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/ob_type.rs
--rw-r--r--   0     1001      123    14829 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/shared.rs
--rw-r--r--   0     1001      123     1419 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/any.rs
--rw-r--r--   0     1001      123     2507 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/bytes.rs
--rw-r--r--   0     1001      123     6558 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/dataclass.rs
--rw-r--r--   0     1001      123     3921 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/datetime_etc.rs
--rw-r--r--   0     1001      123     3226 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/definitions.rs
--rw-r--r--   0     1001      123     5250 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/dict.rs
--rw-r--r--   0     1001      123     6534 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/format.rs
--rw-r--r--   0     1001      123    22198 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/function.rs
--rw-r--r--   0     1001      123     7344 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/generator.rs
--rw-r--r--   0     1001      123     2961 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/json.rs
--rw-r--r--   0     1001      123     2196 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/json_or_python.rs
--rw-r--r--   0     1001      123     4053 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/list.rs
--rw-r--r--   0     1001      123     5517 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/literal.rs
--rw-r--r--   0     1001      123     1077 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/mod.rs
--rw-r--r--   0     1001      123     8181 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/model.rs
--rw-r--r--   0     1001      123     2388 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/nullable.rs
--rw-r--r--   0     1001      123     3513 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/other.rs
--rw-r--r--   0     1001      123     4489 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/set_frozenset.rs
--rw-r--r--   0     1001      123     5926 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/simple.rs
--rw-r--r--   0     1001      123     2576 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/string.rs
--rw-r--r--   0     1001      123     2464 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/timedelta.rs
--rw-r--r--   0     1001      123    12727 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/tuple.rs
--rw-r--r--   0     1001      123     2482 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/typed_dict.rs
--rw-r--r--   0     1001      123     6947 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/union.rs
--rw-r--r--   0     1001      123     3114 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/url.rs
--rw-r--r--   0     1001      123     2054 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/serializers/type_serializers/with_default.rs
--rw-r--r--   0     1001      123     2736 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/tools.rs
--rw-r--r--   0     1001      123    16394 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/url.rs
--rw-r--r--   0     1001      123     1468 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/any.rs
--rw-r--r--   0     1001      123    15665 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/arguments.rs
--rw-r--r--   0     1001      123     1662 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/bool.rs
--rw-r--r--   0     1001      123     3769 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/bytes.rs
--rw-r--r--   0     1001      123     4399 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/call.rs
--rw-r--r--   0     1001      123     1504 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/callable.rs
--rw-r--r--   0     1001      123     3391 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/chain.rs
--rw-r--r--   0     1001      123     3928 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/custom_error.rs
--rw-r--r--   0     1001      123    24975 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/dataclass.rs
--rw-r--r--   0     1001      123     7033 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/date.rs
--rw-r--r--   0     1001      123     9231 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/datetime.rs
--rw-r--r--   0     1001      123     6801 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/definitions.rs
--rw-r--r--   0     1001      123     6528 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/dict.rs
--rw-r--r--   0     1001      123     6276 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/float.rs
--rw-r--r--   0     1001      123     2035 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/frozenset.rs
--rw-r--r--   0     1001      123    18903 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/function.rs
--rw-r--r--   0     1001      123    11183 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/generator.rs
--rw-r--r--   0     1001      123     4929 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/int.rs
--rw-r--r--   0     1001      123     3256 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/is_instance.rs
--rw-r--r--   0     1001      123     2201 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/is_subclass.rs
--rw-r--r--   0     1001      123     2600 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/json.rs
--rw-r--r--   0     1001      123     2568 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/json_or_python.rs
--rw-r--r--   0     1001      123     2752 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/lax_or_strict.rs
--rw-r--r--   0     1001      123     5826 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/list.rs
--rw-r--r--   0     1001      123     6500 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/literal.rs
--rw-r--r--   0     1001      123    23341 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/mod.rs
--rw-r--r--   0     1001      123    14906 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/model.rs
--rw-r--r--   0     1001      123    17050 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/model_fields.rs
--rw-r--r--   0     1001      123     1477 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/none.rs
--rw-r--r--   0     1001      123     1953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/nullable.rs
--rw-r--r--   0     1001      123     3158 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/set.rs
--rw-r--r--   0     1001      123     6301 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/string.rs
--rw-r--r--   0     1001      123     3888 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/time.rs
--rw-r--r--   0     1001      123     3927 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/timedelta.rs
--rw-r--r--   0     1001      123     9993 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/tuple.rs
--rw-r--r--   0     1001      123    12699 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/typed_dict.rs
--rw-r--r--   0     1001      123    16840 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/union.rs
--rw-r--r--   0     1001      123    17932 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/url.rs
--rw-r--r--   0     1001      123     6970 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/src/validators/with_default.rs
--rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/__init__.py
--rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      123    15198 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/complete_schema.py
--rw-r--r--   0     1001      123     4950 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_complete_benchmark.py
--rw-r--r--   0     1001      123    38992 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_micro_benchmarks.py
--rw-r--r--   0     1001      123    14015 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/benchmarks/test_serialization_micro.py
--rw-r--r--   0     1001      123     4110 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/conftest.py
--rw-r--r--   0     1001      123     3272 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/emscripten_runner.js
--rw-r--r--   0     1001      123       72 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/requirements-linting.txt
--rw-r--r--   0     1001      123      190 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/requirements.txt
--rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/__init__.py
--rw-r--r--   0     1001      123    23747 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_any.py
--rw-r--r--   0     1001      123     4342 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_bytes.py
--rw-r--r--   0     1001      123     5571 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_dataclasses.py
--rw-r--r--   0     1001      123     4798 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_datetime.py
--rw-r--r--   0     1001      123     3901 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_definitions.py
--rw-r--r--   0     1001      123     4164 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_definitions_recursive.py
--rw-r--r--   0     1001      123     7509 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_dict.py
--rw-r--r--   0     1001      123     4659 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_format.py
--rw-r--r--   0     1001      123    22938 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_functions.py
--rw-r--r--   0     1001      123     5424 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_generator.py
--rw-r--r--   0     1001      123     1853 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_json.py
--rw-r--r--   0     1001      123      540 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_json_or_python.py
--rw-r--r--   0     1001      123    18385 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_list_tuple.py
--rw-r--r--   0     1001      123     2172 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_literal.py
--rw-r--r--   0     1001      123      517 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_misc.py
--rw-r--r--   0     1001      123    32725 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_model.py
--rw-r--r--   0     1001      123     5749 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_model_root.py
--rw-r--r--   0     1001      123      953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_none.py
--rw-r--r--   0     1001      123      566 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_nullable.py
--rw-r--r--   0     1001      123     2174 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_other.py
--rw-r--r--   0     1001      123     2052 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_set_frozenset.py
--rw-r--r--   0     1001      123     2334 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_simple.py
--rw-r--r--   0     1001      123     2503 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_string.py
--rw-r--r--   0     1001      123     1665 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_timedelta.py
--rw-r--r--   0     1001      123    12753 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_typed_dict.py
--rw-r--r--   0     1001      123    13375 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_union.py
--rw-r--r--   0     1001      123     4287 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/serializers/test_url.py
--rw-r--r--   0     1001      123     2065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test.rs
--rw-r--r--   0     1001      123     4764 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_build.py
--rw-r--r--   0     1001      123     4675 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_config.py
--rw-r--r--   0     1001      123     1246 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_docstrings.py
--rw-r--r--   0     1001      123    29152 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_errors.py
--rw-r--r--   0     1001      123     2187 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_garbage_collection.py
--rw-r--r--   0     1001      123     6159 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_hypothesis.py
--rw-r--r--   0     1001      123     2184 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_isinstance.py
--rw-r--r--   0     1001      123    11916 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_json.py
--rw-r--r--   0     1001      123     7069 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_misc.py
--rw-r--r--   0     1001      123    12707 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_schema_functions.py
--rw-r--r--   0     1001      123     1795 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_strict.py
--rw-r--r--   0     1001      123     9150 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_typing.py
--rw-r--r--   0     1001      123     5013 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/test_validation_context.py
--rw-r--r--   0     1001      123        0 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/__init__.py
--rw-r--r--   0     1001      123    35676 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_arguments.py
--rw-r--r--   0     1001      123     4108 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_bool.py
--rw-r--r--   0     1001      123     4396 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_bytes.py
--rw-r--r--   0     1001      123     7161 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_call.py
--rw-r--r--   0     1001      123     1492 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_callable.py
--rw-r--r--   0     1001      123     4083 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_chain.py
--rw-r--r--   0     1001      123     1699 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_custom_error.py
--rw-r--r--   0     1001      123    50588 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_dataclasses.py
--rw-r--r--   0     1001      123    12100 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_date.py
--rw-r--r--   0     1001      123    20109 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_datetime.py
--rw-r--r--   0     1001      123     4913 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_definitions.py
--rw-r--r--   0     1001      123    31995 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_definitions_recursive.py
--rw-r--r--   0     1001      123     9074 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_dict.py
--rw-r--r--   0     1001      123    11686 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_float.py
--rw-r--r--   0     1001      123    11389 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_frozenset.py
--rw-r--r--   0     1001      123    29953 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_function.py
--rw-r--r--   0     1001      123     6819 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_generator.py
--rw-r--r--   0     1001      123    13642 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_int.py
--rw-r--r--   0     1001      123     5119 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_is_instance.py
--rw-r--r--   0     1001      123     2065 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_is_subclass.py
--rw-r--r--   0     1001      123     5260 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_json.py
--rw-r--r--   0     1001      123     1027 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_json_or_python.py
--rw-r--r--   0     1001      123     1640 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_lax_or_strict.py
--rw-r--r--   0     1001      123    16913 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_list.py
--rw-r--r--   0     1001      123    12324 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_literal.py
--rw-r--r--   0     1001      123    39054 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model.py
--rw-r--r--   0     1001      123    62078 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_fields.py
--rw-r--r--   0     1001      123    13996 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_init.py
--rw-r--r--   0     1001      123     7108 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_model_root.py
--rw-r--r--   0     1001      123      760 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_none.py
--rw-r--r--   0     1001      123     1056 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_nullable.py
--rw-r--r--   0     1001      123    10405 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_set.py
--rw-r--r--   0     1001      123     9016 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_string.py
--rw-r--r--   0     1001      123    22574 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_tagged_union.py
--rw-r--r--   0     1001      123    12215 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_time.py
--rw-r--r--   0     1001      123    12659 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_timedelta.py
--rw-r--r--   0     1001      123    18166 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_tuple.py
--rw-r--r--   0     1001      123    41936 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_typed_dict.py
--rw-r--r--   0     1001      123    15403 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_union.py
--rw-r--r--   0     1001      123    56241 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_url.py
--rw-r--r--   0     1001      123    21767 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/tests/validators/test_with_default.py
--rw-r--r--   0     1001      123    16807 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/Cargo.lock
--rw-r--r--   0     1001      123        1 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/py.typed
--rw-r--r--   0     1001      123     9532 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0     1001      123   128560 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/core_schema.py
--rw-r--r--   0     1001      123     2190 2023-07-11 11:20:33.000000 pydantic_core-2.2.0/python/pydantic_core/__init__.py
--rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 pydantic_core-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydantic_core-2.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      312 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/.cargo/config.toml
+-rw-r--r--   0     1001      123     1080 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/LICENSE
+-rw-r--r--   0     1001      123     5052 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/Makefile
+-rw-r--r--   0     1001      123     3704 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/README.md
+-rw-r--r--   0     1001      123     1366 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/build.rs
+-rw-r--r--   0     1001      123     8313 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/generate_self_schema.py
+-rw-r--r--   0     1001      123     3340 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     3065 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/argument_markers.rs
+-rw-r--r--   0     1001      123     5811 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/build_tools.rs
+-rw-r--r--   0     1001      123     4486 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/definitions.rs
+-rw-r--r--   0     1001      123     5441 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/line_error.rs
+-rw-r--r--   0     1001      123     7101 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/location.rs
+-rw-r--r--   0     1001      123     1065 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/mod.rs
+-rw-r--r--   0     1001      123    33615 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/types.rs
+-rw-r--r--   0     1001      123    17567 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/validation_exception.rs
+-rw-r--r--   0     1001      123     5046 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/errors/value_exception.rs
+-rw-r--r--   0     1001      123    15380 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/datetime.rs
+-rw-r--r--   0     1001      123     9522 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/input_abstract.rs
+-rw-r--r--   0     1001      123    19917 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/input_json.rs
+-rw-r--r--   0     1001      123    27345 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/input_python.rs
+-rw-r--r--   0     1001      123     1007 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/mod.rs
+-rw-r--r--   0     1001      123     7700 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/parse_json.rs
+-rw-r--r--   0     1001      123    32794 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/return_enums.rs
+-rw-r--r--   0     1001      123     3426 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/input/shared.rs
+-rw-r--r--   0     1001      123     1756 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/lazy_index_map.rs
+-rw-r--r--   0     1001      123     3615 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    17853 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/lookup_key.rs
+-rw-r--r--   0     1001      123     2484 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/recursion_guard.rs
+-rw-r--r--   0     1001      123     5707 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/computed_fields.rs
+-rw-r--r--   0     1001      123     5528 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/config.rs
+-rw-r--r--   0     1001      123     2779 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/errors.rs
+-rw-r--r--   0     1001      123    11523 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/extra.rs
+-rw-r--r--   0     1001      123    12294 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/fields.rs
+-rw-r--r--   0     1001      123    14578 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/filter.rs
+-rw-r--r--   0     1001      123    25396 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/infer.rs
+-rw-r--r--   0     1001      123     7948 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/mod.rs
+-rw-r--r--   0     1001      123    11222 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/ob_type.rs
+-rw-r--r--   0     1001      123    14847 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/shared.rs
+-rw-r--r--   0     1001      123     1419 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/any.rs
+-rw-r--r--   0     1001      123     2507 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/bytes.rs
+-rw-r--r--   0     1001      123     6558 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/dataclass.rs
+-rw-r--r--   0     1001      123     3921 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/datetime_etc.rs
+-rw-r--r--   0     1001      123     3226 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/definitions.rs
+-rw-r--r--   0     1001      123     5250 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/dict.rs
+-rw-r--r--   0     1001      123     6534 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/format.rs
+-rw-r--r--   0     1001      123    22198 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/function.rs
+-rw-r--r--   0     1001      123     7344 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/generator.rs
+-rw-r--r--   0     1001      123     2961 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/json.rs
+-rw-r--r--   0     1001      123     2196 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/json_or_python.rs
+-rw-r--r--   0     1001      123     4053 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/list.rs
+-rw-r--r--   0     1001      123     5517 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/literal.rs
+-rw-r--r--   0     1001      123      987 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/mod.rs
+-rw-r--r--   0     1001      123     8181 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/model.rs
+-rw-r--r--   0     1001      123     2388 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/nullable.rs
+-rw-r--r--   0     1001      123     3513 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/other.rs
+-rw-r--r--   0     1001      123     4489 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/set_frozenset.rs
+-rw-r--r--   0     1001      123     5926 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/simple.rs
+-rw-r--r--   0     1001      123     2576 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/string.rs
+-rw-r--r--   0     1001      123     2464 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/timedelta.rs
+-rw-r--r--   0     1001      123    12727 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/tuple.rs
+-rw-r--r--   0     1001      123     2482 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/typed_dict.rs
+-rw-r--r--   0     1001      123     6947 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/union.rs
+-rw-r--r--   0     1001      123     3114 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/url.rs
+-rw-r--r--   0     1001      123     2054 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/serializers/type_serializers/with_default.rs
+-rw-r--r--   0     1001      123     2736 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/tools.rs
+-rw-r--r--   0     1001      123    16394 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/url.rs
+-rw-r--r--   0     1001      123     1468 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/any.rs
+-rw-r--r--   0     1001      123    15665 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/arguments.rs
+-rw-r--r--   0     1001      123     1662 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/bool.rs
+-rw-r--r--   0     1001      123     3769 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/bytes.rs
+-rw-r--r--   0     1001      123     4399 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/call.rs
+-rw-r--r--   0     1001      123     1504 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/callable.rs
+-rw-r--r--   0     1001      123     3391 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/chain.rs
+-rw-r--r--   0     1001      123     3928 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/custom_error.rs
+-rw-r--r--   0     1001      123    24975 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/dataclass.rs
+-rw-r--r--   0     1001      123     7105 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/date.rs
+-rw-r--r--   0     1001      123    10106 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/datetime.rs
+-rw-r--r--   0     1001      123     6801 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/definitions.rs
+-rw-r--r--   0     1001      123     6528 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/dict.rs
+-rw-r--r--   0     1001      123     6276 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/float.rs
+-rw-r--r--   0     1001      123     2035 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/frozenset.rs
+-rw-r--r--   0     1001      123    18903 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/function.rs
+-rw-r--r--   0     1001      123    11183 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/generator.rs
+-rw-r--r--   0     1001      123     4929 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/int.rs
+-rw-r--r--   0     1001      123     3256 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/is_instance.rs
+-rw-r--r--   0     1001      123     2201 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/is_subclass.rs
+-rw-r--r--   0     1001      123     2600 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/json.rs
+-rw-r--r--   0     1001      123     2568 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/json_or_python.rs
+-rw-r--r--   0     1001      123     2752 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/lax_or_strict.rs
+-rw-r--r--   0     1001      123     5826 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/list.rs
+-rw-r--r--   0     1001      123     6500 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/literal.rs
+-rw-r--r--   0     1001      123    23341 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/mod.rs
+-rw-r--r--   0     1001      123    15308 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/model.rs
+-rw-r--r--   0     1001      123    17766 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/model_fields.rs
+-rw-r--r--   0     1001      123     1477 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/none.rs
+-rw-r--r--   0     1001      123     1953 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/nullable.rs
+-rw-r--r--   0     1001      123     3158 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/set.rs
+-rw-r--r--   0     1001      123     6301 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/string.rs
+-rw-r--r--   0     1001      123     4132 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/time.rs
+-rw-r--r--   0     1001      123     4171 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/timedelta.rs
+-rw-r--r--   0     1001      123     9993 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/tuple.rs
+-rw-r--r--   0     1001      123    12699 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/typed_dict.rs
+-rw-r--r--   0     1001      123    16840 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/union.rs
+-rw-r--r--   0     1001      123    17932 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/url.rs
+-rw-r--r--   0     1001      123     6970 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/src/validators/with_default.rs
+-rw-r--r--   0     1001      123        0 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/__init__.py
+-rw-r--r--   0     1001      123        0 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123    15198 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/benchmarks/complete_schema.py
+-rw-r--r--   0     1001      123     4950 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/benchmarks/test_complete_benchmark.py
+-rw-r--r--   0     1001      123    38992 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/benchmarks/test_micro_benchmarks.py
+-rw-r--r--   0     1001      123    14015 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/benchmarks/test_serialization_micro.py
+-rw-r--r--   0     1001      123     4110 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/conftest.py
+-rw-r--r--   0     1001      123     3272 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/emscripten_runner.js
+-rw-r--r--   0     1001      123       72 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/requirements-linting.txt
+-rw-r--r--   0     1001      123      190 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/requirements.txt
+-rw-r--r--   0     1001      123        0 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/__init__.py
+-rw-r--r--   0     1001      123    23747 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_any.py
+-rw-r--r--   0     1001      123     4342 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_bytes.py
+-rw-r--r--   0     1001      123     5571 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_dataclasses.py
+-rw-r--r--   0     1001      123     4798 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_datetime.py
+-rw-r--r--   0     1001      123     3901 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_definitions.py
+-rw-r--r--   0     1001      123     4164 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     7509 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_dict.py
+-rw-r--r--   0     1001      123     4659 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_format.py
+-rw-r--r--   0     1001      123    22892 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_functions.py
+-rw-r--r--   0     1001      123     5424 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_generator.py
+-rw-r--r--   0     1001      123     1853 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_json.py
+-rw-r--r--   0     1001      123      540 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_json_or_python.py
+-rw-r--r--   0     1001      123    18385 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_list_tuple.py
+-rw-r--r--   0     1001      123     2172 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_literal.py
+-rw-r--r--   0     1001      123      517 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_misc.py
+-rw-r--r--   0     1001      123    34597 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_model.py
+-rw-r--r--   0     1001      123     5749 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_model_root.py
+-rw-r--r--   0     1001      123      953 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_none.py
+-rw-r--r--   0     1001      123      566 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_nullable.py
+-rw-r--r--   0     1001      123     2174 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_other.py
+-rw-r--r--   0     1001      123     2052 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_set_frozenset.py
+-rw-r--r--   0     1001      123     2334 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_simple.py
+-rw-r--r--   0     1001      123     2503 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_string.py
+-rw-r--r--   0     1001      123     1665 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_timedelta.py
+-rw-r--r--   0     1001      123    12753 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_typed_dict.py
+-rw-r--r--   0     1001      123    13375 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_union.py
+-rw-r--r--   0     1001      123     4287 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/serializers/test_url.py
+-rw-r--r--   0     1001      123     2065 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test.rs
+-rw-r--r--   0     1001      123     4764 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_build.py
+-rw-r--r--   0     1001      123     4675 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_config.py
+-rw-r--r--   0     1001      123     1246 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_docstrings.py
+-rw-r--r--   0     1001      123    29152 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_errors.py
+-rw-r--r--   0     1001      123     2187 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_garbage_collection.py
+-rw-r--r--   0     1001      123     6180 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_hypothesis.py
+-rw-r--r--   0     1001      123     2184 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_isinstance.py
+-rw-r--r--   0     1001      123    11916 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_json.py
+-rw-r--r--   0     1001      123     7069 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_misc.py
+-rw-r--r--   0     1001      123    13298 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_schema_functions.py
+-rw-r--r--   0     1001      123     1795 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_strict.py
+-rw-r--r--   0     1001      123     9150 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_typing.py
+-rw-r--r--   0     1001      123     5013 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/test_validation_context.py
+-rw-r--r--   0     1001      123        0 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/__init__.py
+-rw-r--r--   0     1001      123    35676 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_arguments.py
+-rw-r--r--   0     1001      123     4108 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_bool.py
+-rw-r--r--   0     1001      123     4396 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_bytes.py
+-rw-r--r--   0     1001      123     7161 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_call.py
+-rw-r--r--   0     1001      123     1492 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_callable.py
+-rw-r--r--   0     1001      123     4083 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_chain.py
+-rw-r--r--   0     1001      123     1699 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_custom_error.py
+-rw-r--r--   0     1001      123    50588 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_dataclasses.py
+-rw-r--r--   0     1001      123    12100 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_date.py
+-rw-r--r--   0     1001      123    21572 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_datetime.py
+-rw-r--r--   0     1001      123     4913 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_definitions.py
+-rw-r--r--   0     1001      123    31995 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_definitions_recursive.py
+-rw-r--r--   0     1001      123     9074 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_dict.py
+-rw-r--r--   0     1001      123    11686 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_float.py
+-rw-r--r--   0     1001      123    11389 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_frozenset.py
+-rw-r--r--   0     1001      123    30123 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_function.py
+-rw-r--r--   0     1001      123     6819 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_generator.py
+-rw-r--r--   0     1001      123    13642 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_int.py
+-rw-r--r--   0     1001      123     5119 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_is_instance.py
+-rw-r--r--   0     1001      123     2065 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_is_subclass.py
+-rw-r--r--   0     1001      123     5260 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_json.py
+-rw-r--r--   0     1001      123     1027 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_json_or_python.py
+-rw-r--r--   0     1001      123     1640 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_lax_or_strict.py
+-rw-r--r--   0     1001      123    16913 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_list.py
+-rw-r--r--   0     1001      123    12324 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_literal.py
+-rw-r--r--   0     1001      123    39219 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_model.py
+-rw-r--r--   0     1001      123    62255 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_model_fields.py
+-rw-r--r--   0     1001      123    13996 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_model_init.py
+-rw-r--r--   0     1001      123     7108 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_model_root.py
+-rw-r--r--   0     1001      123      760 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_none.py
+-rw-r--r--   0     1001      123     1056 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_nullable.py
+-rw-r--r--   0     1001      123    10405 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_set.py
+-rw-r--r--   0     1001      123     9016 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_string.py
+-rw-r--r--   0     1001      123    22574 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_tagged_union.py
+-rw-r--r--   0     1001      123    13038 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_time.py
+-rw-r--r--   0     1001      123    12659 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_timedelta.py
+-rw-r--r--   0     1001      123    18166 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_tuple.py
+-rw-r--r--   0     1001      123    41936 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_typed_dict.py
+-rw-r--r--   0     1001      123    15403 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_union.py
+-rw-r--r--   0     1001      123    56241 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_url.py
+-rw-r--r--   0     1001      123    21767 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/tests/validators/test_with_default.py
+-rw-r--r--   0     1001      123    17317 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/Cargo.lock
+-rw-r--r--   0     1001      123        1 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/python/pydantic_core/py.typed
+-rw-r--r--   0     1001      123    10163 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0     1001      123   129458 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/python/pydantic_core/core_schema.py
+-rw-r--r--   0     1001      123     2190 2023-07-13 19:14:39.000000 pydantic_core-2.3.0/python/pydantic_core/__init__.py
+-rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 pydantic_core-2.3.0/PKG-INFO
```

### Comparing `pydantic_core-2.2.0/Cargo.toml` & `pydantic_core-2.3.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pydantic-core"
-version = "2.2.0"
+version = "2.3.0"
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pydantic/pydantic-core"
 repository = "https://github.com/pydantic/pydantic-core.git"
 readme = "README.md"
 include = [
     "/pyproject.toml",
@@ -31,15 +31,15 @@
 strum = { version = "0.25.0", features = ["derive"] }
 strum_macros = "0.24.3"
 serde_json = {version = "1.0.87", features = ["arbitrary_precision", "preserve_order"]}
 enum_dispatch = "0.3.8"
 serde = { version = "1.0.147", features = ["derive"] }
 # disabled for benchmarks since it makes microbenchmark performance more flakey
 mimalloc = { version = "0.1.30", optional = true, default-features = false, features = ["local_dynamic_tls"] }
-speedate = "0.9.1"
+speedate = "0.11.0"
 ahash = "0.8.0"
 url = "2.3.1"
 # idna is already required by url, added here to be explicit
 idna = "0.3.0"
 base64 = "0.13.1"
 num-bigint = "0.4.3"
 python3-dll-a = "0.2.7"
```

### Comparing `pydantic_core-2.2.0/LICENSE` & `pydantic_core-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/Makefile` & `pydantic_core-2.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/README.md` & `pydantic_core-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/build.rs` & `pydantic_core-2.3.0/build.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/generate_self_schema.py` & `pydantic_core-2.3.0/generate_self_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/pyproject.toml` & `pydantic_core-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/argument_markers.rs` & `pydantic_core-2.3.0/src/argument_markers.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/build_tools.rs` & `pydantic_core-2.3.0/src/build_tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/definitions.rs` & `pydantic_core-2.3.0/src/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/line_error.rs` & `pydantic_core-2.3.0/src/errors/line_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/location.rs` & `pydantic_core-2.3.0/src/errors/location.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/mod.rs` & `pydantic_core-2.3.0/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/types.rs` & `pydantic_core-2.3.0/src/errors/types.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/validation_exception.rs` & `pydantic_core-2.3.0/src/errors/validation_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/errors/value_exception.rs` & `pydantic_core-2.3.0/src/errors/value_exception.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/input/datetime.rs` & `pydantic_core-2.3.0/src/input/datetime.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 use pyo3::intern;
 use pyo3::prelude::*;
+
 use pyo3::types::{PyDate, PyDateTime, PyDelta, PyDeltaAccess, PyDict, PyTime, PyTzInfo};
-use speedate::{Date, DateTime, Duration, ParseError, Time};
+use speedate::MicrosecondsPrecisionOverflowBehavior;
+use speedate::{Date, DateTime, Duration, ParseError, Time, TimeConfig};
 use std::borrow::Cow;
-use strum::EnumMessage;
 
-use crate::errors::{ErrorType, ValError, ValResult};
+use strum::EnumMessage;
 
 use super::Input;
+use crate::errors::{ErrorType, ValError, ValResult};
 
 #[cfg_attr(debug_assertions, derive(Debug))]
 pub enum EitherDate<'a> {
     Raw(Date),
     Py(&'a PyDate),
 }
 
@@ -260,28 +262,48 @@
                 error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
             },
             input,
         )),
     }
 }
 
-pub fn bytes_as_time<'a>(input: &'a impl Input<'a>, bytes: &[u8]) -> ValResult<'a, EitherTime<'a>> {
-    match Time::parse_bytes(bytes) {
+pub fn bytes_as_time<'a>(
+    input: &'a impl Input<'a>,
+    bytes: &[u8],
+    microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+) -> ValResult<'a, EitherTime<'a>> {
+    match Time::parse_bytes_with_config(
+        bytes,
+        &TimeConfig {
+            microseconds_precision_overflow_behavior: microseconds_overflow_behavior,
+            unix_timestamp_offset: Some(0),
+        },
+    ) {
         Ok(date) => Ok(date.into()),
         Err(err) => Err(ValError::new(
             ErrorType::TimeParsing {
                 error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
             },
             input,
         )),
     }
 }
 
-pub fn bytes_as_datetime<'a, 'b>(input: &'a impl Input<'a>, bytes: &'b [u8]) -> ValResult<'a, EitherDateTime<'a>> {
-    match DateTime::parse_bytes(bytes) {
+pub fn bytes_as_datetime<'a, 'b>(
+    input: &'a impl Input<'a>,
+    bytes: &'b [u8],
+    microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+) -> ValResult<'a, EitherDateTime<'a>> {
+    match DateTime::parse_bytes_with_config(
+        bytes,
+        &TimeConfig {
+            microseconds_precision_overflow_behavior: microseconds_overflow_behavior,
+            unix_timestamp_offset: Some(0),
+        },
+    ) {
         Ok(dt) => Ok(dt.into()),
         Err(err) => Err(ValError::new(
             ErrorType::DatetimeParsing {
                 error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
             },
             input,
         )),
@@ -289,15 +311,22 @@
 }
 
 pub fn int_as_datetime<'a>(
     input: &'a impl Input<'a>,
     timestamp: i64,
     timestamp_microseconds: u32,
 ) -> ValResult<EitherDateTime> {
-    match DateTime::from_timestamp(timestamp, timestamp_microseconds) {
+    match DateTime::from_timestamp_with_config(
+        timestamp,
+        timestamp_microseconds,
+        &TimeConfig {
+            unix_timestamp_offset: Some(0),
+            ..Default::default()
+        },
+    ) {
         Ok(dt) => Ok(dt.into()),
         Err(err) => Err(ValError::new(
             ErrorType::DatetimeParsing {
                 error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
             },
             input,
         )),
@@ -358,15 +387,22 @@
             ));
         }
         // continue and use the speedate error for >86400
         t if t > MAX_U32 => u32::MAX,
         // ok
         t => t as u32,
     };
-    match Time::from_timestamp(time_timestamp, timestamp_microseconds) {
+    match Time::from_timestamp_with_config(
+        time_timestamp,
+        timestamp_microseconds,
+        &TimeConfig {
+            unix_timestamp_offset: Some(0),
+            ..Default::default()
+        },
+    ) {
         Ok(dt) => Ok(dt.into()),
         Err(err) => Err(ValError::new(
             ErrorType::TimeParsing {
                 error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
             },
             input,
         )),
@@ -385,16 +421,26 @@
         ErrorType::TimeDeltaParsing {
             error: Cow::Borrowed(err.get_documentation().unwrap_or_default()),
         },
         input,
     )
 }
 
-pub fn bytes_as_timedelta<'a, 'b>(input: &'a impl Input<'a>, bytes: &'b [u8]) -> ValResult<'a, EitherTimedelta<'a>> {
-    match Duration::parse_bytes(bytes) {
+pub fn bytes_as_timedelta<'a, 'b>(
+    input: &'a impl Input<'a>,
+    bytes: &'b [u8],
+    microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+) -> ValResult<'a, EitherTimedelta<'a>> {
+    match Duration::parse_bytes_with_config(
+        bytes,
+        &TimeConfig {
+            microseconds_precision_overflow_behavior: microseconds_overflow_behavior,
+            unix_timestamp_offset: Some(0),
+        },
+    ) {
         Ok(dt) => Ok(dt.into()),
         Err(err) => Err(map_timedelta_err(input, err)),
     }
 }
 
 pub fn int_as_duration<'a>(input: &'a impl Input<'a>, total_seconds: i64) -> ValResult<Duration> {
     let positive = total_seconds >= 0;
@@ -415,15 +461,15 @@
     Duration::new(positive, days, seconds as u32, microsecond.round() as u32)
         .map_err(|err| map_timedelta_err(input, err))
 }
 
 #[pyclass(module = "pydantic_core._pydantic_core", extends = PyTzInfo)]
 #[derive(Clone)]
 #[cfg_attr(debug_assertions, derive(Debug))]
-struct TzInfo {
+pub struct TzInfo {
     seconds: i32,
 }
 
 #[pymethods]
 impl TzInfo {
     #[new]
     fn new(seconds: i32) -> Self {
@@ -454,8 +500,14 @@
             format!("{:+03}:{:02}", mins / 60, (mins % 60).abs())
         }
     }
 
     fn __deepcopy__(&self, py: Python, _memo: &PyDict) -> PyResult<Py<Self>> {
         Py::new(py, self.clone())
     }
+
+    pub fn __reduce__(&self, py: Python) -> PyResult<PyObject> {
+        let args = (self.seconds,);
+        let cls = Py::new(py, self.clone())?.getattr(py, "__class__")?;
+        Ok((cls, args).into_py(py))
+    }
 }
```

### Comparing `pydantic_core-2.2.0/src/input/input_abstract.rs` & `pydantic_core-2.3.0/src/input/input_abstract.rs`

 * *Files 10% similar despite different names*

```diff
@@ -234,46 +234,76 @@
     }
     fn strict_date(&self) -> ValResult<EitherDate>;
     #[cfg_attr(has_no_coverage, no_coverage)]
     fn lax_date(&self) -> ValResult<EitherDate> {
         self.strict_date()
     }
 
-    fn validate_time(&self, strict: bool) -> ValResult<EitherTime> {
+    fn validate_time(
+        &self,
+        strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
         if strict {
-            self.strict_time()
+            self.strict_time(microseconds_overflow_behavior)
         } else {
-            self.lax_time()
+            self.lax_time(microseconds_overflow_behavior)
         }
     }
-    fn strict_time(&self) -> ValResult<EitherTime>;
+    fn strict_time(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime>;
     #[cfg_attr(has_no_coverage, no_coverage)]
-    fn lax_time(&self) -> ValResult<EitherTime> {
-        self.strict_time()
+    fn lax_time(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
+        self.strict_time(microseconds_overflow_behavior)
     }
 
-    fn validate_datetime(&self, strict: bool) -> ValResult<EitherDateTime> {
+    fn validate_datetime(
+        &self,
+        strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
         if strict {
-            self.strict_datetime()
+            self.strict_datetime(microseconds_overflow_behavior)
         } else {
-            self.lax_datetime()
+            self.lax_datetime(microseconds_overflow_behavior)
         }
     }
-    fn strict_datetime(&self) -> ValResult<EitherDateTime>;
+    fn strict_datetime(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime>;
     #[cfg_attr(has_no_coverage, no_coverage)]
-    fn lax_datetime(&self) -> ValResult<EitherDateTime> {
-        self.strict_datetime()
+    fn lax_datetime(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
+        self.strict_datetime(microseconds_overflow_behavior)
     }
 
-    fn validate_timedelta(&self, strict: bool) -> ValResult<EitherTimedelta> {
+    fn validate_timedelta(
+        &self,
+        strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
         if strict {
-            self.strict_timedelta()
+            self.strict_timedelta(microseconds_overflow_behavior)
         } else {
-            self.lax_timedelta()
+            self.lax_timedelta(microseconds_overflow_behavior)
         }
     }
-    fn strict_timedelta(&self) -> ValResult<EitherTimedelta>;
+    fn strict_timedelta(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta>;
     #[cfg_attr(has_no_coverage, no_coverage)]
-    fn lax_timedelta(&self) -> ValResult<EitherTimedelta> {
-        self.strict_timedelta()
+    fn lax_timedelta(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
+        self.strict_timedelta(microseconds_overflow_behavior)
     }
 }
```

### Comparing `pydantic_core-2.2.0/src/input/input_json.rs` & `pydantic_core-2.3.0/src/input/input_json.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use std::borrow::Cow;
 
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
+use speedate::MicrosecondsPrecisionOverflowBehavior;
 use strum::EnumMessage;
 
 use crate::errors::{ErrorType, InputValue, LocItem, ValError, ValResult};
 
 use super::datetime::{
     bytes_as_date, bytes_as_datetime, bytes_as_time, bytes_as_timedelta, float_as_datetime, float_as_duration,
     float_as_time, int_as_datetime, int_as_duration, int_as_time, EitherDate, EitherDateTime, EitherTime,
@@ -260,23 +261,26 @@
     // NO custom `lax_date` implementation, if strict_date fails, the validator will fallback to lax_datetime
     // then check there's no remainder
     #[cfg_attr(has_no_coverage, no_coverage)]
     fn strict_date(&self) -> ValResult<EitherDate> {
         self.validate_date(false)
     }
 
-    fn strict_time(&self) -> ValResult<EitherTime> {
+    fn strict_time(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
         match self {
-            JsonInput::String(v) => bytes_as_time(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_time(self, v.as_bytes(), microseconds_overflow_behavior),
             _ => Err(ValError::new(ErrorType::TimeType, self)),
         }
     }
-    fn lax_time(&self) -> ValResult<EitherTime> {
+    fn lax_time(&self, microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior) -> ValResult<EitherTime> {
         match self {
-            JsonInput::String(v) => bytes_as_time(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_time(self, v.as_bytes(), microseconds_overflow_behavior),
             JsonInput::Int(v) => int_as_time(self, *v, 0),
             JsonInput::Float(v) => float_as_time(self, *v),
             JsonInput::BigInt(_) => Err(ValError::new(
                 ErrorType::TimeParsing {
                     error: Cow::Borrowed(
                         speedate::ParseError::TimeTooLarge
                             .get_documentation()
@@ -285,38 +289,50 @@
                 },
                 self,
             )),
             _ => Err(ValError::new(ErrorType::TimeType, self)),
         }
     }
 
-    fn strict_datetime(&self) -> ValResult<EitherDateTime> {
+    fn strict_datetime(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
         match self {
-            JsonInput::String(v) => bytes_as_datetime(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_datetime(self, v.as_bytes(), microseconds_overflow_behavior),
             _ => Err(ValError::new(ErrorType::DatetimeType, self)),
         }
     }
-    fn lax_datetime(&self) -> ValResult<EitherDateTime> {
+    fn lax_datetime(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
         match self {
-            JsonInput::String(v) => bytes_as_datetime(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_datetime(self, v.as_bytes(), microseconds_overflow_behavior),
             JsonInput::Int(v) => int_as_datetime(self, *v, 0),
             JsonInput::Float(v) => float_as_datetime(self, *v),
             _ => Err(ValError::new(ErrorType::DatetimeType, self)),
         }
     }
 
-    fn strict_timedelta(&self) -> ValResult<EitherTimedelta> {
+    fn strict_timedelta(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
         match self {
-            JsonInput::String(v) => bytes_as_timedelta(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_timedelta(self, v.as_bytes(), microseconds_overflow_behavior),
             _ => Err(ValError::new(ErrorType::TimeDeltaType, self)),
         }
     }
-    fn lax_timedelta(&self) -> ValResult<EitherTimedelta> {
+    fn lax_timedelta(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
         match self {
-            JsonInput::String(v) => bytes_as_timedelta(self, v.as_bytes()),
+            JsonInput::String(v) => bytes_as_timedelta(self, v.as_bytes(), microseconds_overflow_behavior),
             JsonInput::Int(v) => Ok(int_as_duration(self, *v)?.into()),
             JsonInput::Float(v) => Ok(float_as_duration(self, *v)?.into()),
             _ => Err(ValError::new(ErrorType::TimeDeltaType, self)),
         }
     }
 }
 
@@ -458,35 +474,56 @@
         bytes_as_date(self, self.as_bytes())
     }
     #[cfg_attr(has_no_coverage, no_coverage)]
     fn strict_date(&self) -> ValResult<EitherDate> {
         self.validate_date(false)
     }
 
-    fn validate_time(&self, _strict: bool) -> ValResult<EitherTime> {
-        bytes_as_time(self, self.as_bytes())
-    }
-    #[cfg_attr(has_no_coverage, no_coverage)]
-    fn strict_time(&self) -> ValResult<EitherTime> {
-        self.validate_time(false)
-    }
-
-    fn validate_datetime(&self, _strict: bool) -> ValResult<EitherDateTime> {
-        bytes_as_datetime(self, self.as_bytes())
-    }
-    #[cfg_attr(has_no_coverage, no_coverage)]
-    fn strict_datetime(&self) -> ValResult<EitherDateTime> {
-        self.validate_datetime(false)
-    }
-
-    fn validate_timedelta(&self, _strict: bool) -> ValResult<EitherTimedelta> {
-        bytes_as_timedelta(self, self.as_bytes())
-    }
-    #[cfg_attr(has_no_coverage, no_coverage)]
-    fn strict_timedelta(&self) -> ValResult<EitherTimedelta> {
-        self.validate_timedelta(false)
+    fn validate_time(
+        &self,
+        _strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
+        bytes_as_time(self, self.as_bytes(), microseconds_overflow_behavior)
+    }
+    #[cfg_attr(has_no_coverage, no_coverage)]
+    fn strict_time(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
+        self.validate_time(false, microseconds_overflow_behavior)
+    }
+
+    fn validate_datetime(
+        &self,
+        _strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
+        bytes_as_datetime(self, self.as_bytes(), microseconds_overflow_behavior)
+    }
+    #[cfg_attr(has_no_coverage, no_coverage)]
+    fn strict_datetime(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
+        self.validate_datetime(false, microseconds_overflow_behavior)
+    }
+
+    fn validate_timedelta(
+        &self,
+        _strict: bool,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
+        bytes_as_timedelta(self, self.as_bytes(), microseconds_overflow_behavior)
+    }
+    #[cfg_attr(has_no_coverage, no_coverage)]
+    fn strict_timedelta(
+        &self,
+        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
+        self.validate_timedelta(false, microseconds_overflow_behavior)
     }
 }
 
 fn string_to_vec(s: &str) -> JsonArray {
     s.chars().map(|c| JsonInput::String(c.to_string())).collect()
 }
```

### Comparing `pydantic_core-2.2.0/src/input/input_python.rs` & `pydantic_core-2.3.0/src/input/input_python.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use pyo3::types::{
     PyBool, PyByteArray, PyBytes, PyDate, PyDateTime, PyDelta, PyDict, PyFloat, PyFrozenSet, PyInt, PyIterator, PyList,
     PyMapping, PySequence, PySet, PyString, PyTime, PyTuple, PyType,
 };
 #[cfg(not(PyPy))]
 use pyo3::types::{PyDictItems, PyDictKeys, PyDictValues};
 use pyo3::{intern, AsPyPointer, PyTypeInfo};
+use speedate::MicrosecondsPrecisionOverflowBehavior;
 
 use crate::errors::{ErrorType, InputValue, LocItem, ValError, ValResult};
 use crate::tools::{extract_i64, safe_repr};
 use crate::{ArgsKwargs, PyMultiHostUrl, PyUrl};
 
 use super::datetime::{
     bytes_as_date, bytes_as_datetime, bytes_as_time, bytes_as_timedelta, date_as_datetime, float_as_datetime,
@@ -542,86 +543,101 @@
         } else if let Ok(py_bytes) = self.downcast::<PyBytes>() {
             bytes_as_date(self, py_bytes.as_bytes())
         } else {
             Err(ValError::new(ErrorType::DateType, self))
         }
     }
 
-    fn strict_time(&self) -> ValResult<EitherTime> {
+    fn strict_time(
+        &self,
+        _microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTime> {
         if let Ok(time) = self.downcast::<PyTime>() {
             Ok(time.into())
         } else {
             Err(ValError::new(ErrorType::TimeType, self))
         }
     }
 
-    fn lax_time(&self) -> ValResult<EitherTime> {
+    fn lax_time(&self, microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior) -> ValResult<EitherTime> {
         if let Ok(time) = self.downcast::<PyTime>() {
             Ok(time.into())
         } else if let Ok(py_str) = self.downcast::<PyString>() {
             let str = py_string_str(py_str)?;
-            bytes_as_time(self, str.as_bytes())
+            bytes_as_time(self, str.as_bytes(), microseconds_overflow_behavior)
         } else if let Ok(py_bytes) = self.downcast::<PyBytes>() {
-            bytes_as_time(self, py_bytes.as_bytes())
+            bytes_as_time(self, py_bytes.as_bytes(), microseconds_overflow_behavior)
         } else if PyBool::is_exact_type_of(self) {
             Err(ValError::new(ErrorType::TimeType, self))
         } else if let Ok(int) = extract_i64(self) {
             int_as_time(self, int, 0)
         } else if let Ok(float) = self.extract::<f64>() {
             float_as_time(self, float)
         } else {
             Err(ValError::new(ErrorType::TimeType, self))
         }
     }
 
-    fn strict_datetime(&self) -> ValResult<EitherDateTime> {
+    fn strict_datetime(
+        &self,
+        _microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
         if let Ok(dt) = self.downcast::<PyDateTime>() {
             Ok(dt.into())
         } else {
             Err(ValError::new(ErrorType::DatetimeType, self))
         }
     }
 
-    fn lax_datetime(&self) -> ValResult<EitherDateTime> {
+    fn lax_datetime(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherDateTime> {
         if let Ok(dt) = self.downcast::<PyDateTime>() {
             Ok(dt.into())
         } else if let Ok(py_str) = self.downcast::<PyString>() {
             let str = py_string_str(py_str)?;
-            bytes_as_datetime(self, str.as_bytes())
+            bytes_as_datetime(self, str.as_bytes(), microseconds_overflow_behavior)
         } else if let Ok(py_bytes) = self.downcast::<PyBytes>() {
-            bytes_as_datetime(self, py_bytes.as_bytes())
+            bytes_as_datetime(self, py_bytes.as_bytes(), microseconds_overflow_behavior)
         } else if PyBool::is_exact_type_of(self) {
             Err(ValError::new(ErrorType::DatetimeType, self))
         } else if let Ok(int) = extract_i64(self) {
             int_as_datetime(self, int, 0)
         } else if let Ok(float) = self.extract::<f64>() {
             float_as_datetime(self, float)
         } else if let Ok(date) = self.downcast::<PyDate>() {
             Ok(date_as_datetime(date)?)
         } else {
             Err(ValError::new(ErrorType::DatetimeType, self))
         }
     }
 
-    fn strict_timedelta(&self) -> ValResult<EitherTimedelta> {
+    fn strict_timedelta(
+        &self,
+        _microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
         if let Ok(dt) = self.downcast::<PyDelta>() {
             Ok(dt.into())
         } else {
             Err(ValError::new(ErrorType::TimeDeltaType, self))
         }
     }
 
-    fn lax_timedelta(&self) -> ValResult<EitherTimedelta> {
+    fn lax_timedelta(
+        &self,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
+    ) -> ValResult<EitherTimedelta> {
         if let Ok(dt) = self.downcast::<PyDelta>() {
             Ok(dt.into())
         } else if let Ok(py_str) = self.downcast::<PyString>() {
             let str = py_string_str(py_str)?;
-            bytes_as_timedelta(self, str.as_bytes())
+            bytes_as_timedelta(self, str.as_bytes(), microseconds_overflow_behavior)
         } else if let Ok(py_bytes) = self.downcast::<PyBytes>() {
-            bytes_as_timedelta(self, py_bytes.as_bytes())
+            bytes_as_timedelta(self, py_bytes.as_bytes(), microseconds_overflow_behavior)
         } else if let Ok(int) = extract_i64(self) {
             Ok(int_as_duration(self, int)?.into())
         } else if let Ok(float) = self.extract::<f64>() {
             Ok(float_as_duration(self, float)?.into())
         } else {
             Err(ValError::new(ErrorType::TimeDeltaType, self))
         }
```

### Comparing `pydantic_core-2.2.0/src/input/mod.rs` & `pydantic_core-2.3.0/src/input/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 mod input_abstract;
 mod input_json;
 mod input_python;
 mod parse_json;
 mod return_enums;
 mod shared;
 
+pub use datetime::TzInfo;
 pub(crate) use datetime::{
     duration_as_pytimedelta, pydate_as_date, pydatetime_as_datetime, pytime_as_time, pytimedelta_as_duration,
     EitherDate, EitherDateTime, EitherTime, EitherTimedelta,
 };
 pub(crate) use input_abstract::{Input, InputType};
 pub(crate) use parse_json::{JsonInput, JsonObject};
 pub(crate) use return_enums::{
```

### Comparing `pydantic_core-2.2.0/src/input/parse_json.rs` & `pydantic_core-2.3.0/src/input/parse_json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/input/return_enums.rs` & `pydantic_core-2.3.0/src/input/return_enums.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/input/shared.rs` & `pydantic_core-2.3.0/src/input/shared.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/lazy_index_map.rs` & `pydantic_core-2.3.0/src/lazy_index_map.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/lib.rs` & `pydantic_core-2.3.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 mod recursion_guard;
 mod serializers;
 mod tools;
 mod url;
 mod validators;
 
 // required for benchmarks
+pub use self::input::TzInfo;
 pub use self::url::{PyMultiHostUrl, PyUrl};
 pub use argument_markers::{ArgsKwargs, PydanticUndefinedType};
 pub use build_tools::SchemaError;
 pub use errors::{
     list_all_errors, PydanticCustomError, PydanticKnownError, PydanticOmit, PydanticUseDefault, ValidationError,
 };
 pub use serializers::{
@@ -89,14 +90,15 @@
     m.add_class::<PydanticUseDefault>()?;
     m.add_class::<PydanticSerializationError>()?;
     m.add_class::<PydanticSerializationUnexpectedValue>()?;
     m.add_class::<PyUrl>()?;
     m.add_class::<PyMultiHostUrl>()?;
     m.add_class::<ArgsKwargs>()?;
     m.add_class::<SchemaSerializer>()?;
+    m.add_class::<TzInfo>()?;
     m.add_function(wrap_pyfunction!(to_json, m)?)?;
     m.add_function(wrap_pyfunction!(to_jsonable_python, m)?)?;
     m.add_function(wrap_pyfunction!(list_all_errors, m)?)?;
 
     #[cfg(not(feature = "mimalloc"))]
     m.setattr("__pydantic_core_default_allocator__", true)?; // uses setattr so this is not in __all__
```

### Comparing `pydantic_core-2.2.0/src/lookup_key.rs` & `pydantic_core-2.3.0/src/lookup_key.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/recursion_guard.rs` & `pydantic_core-2.3.0/src/recursion_guard.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/computed_fields.rs` & `pydantic_core-2.3.0/src/serializers/computed_fields.rs`

 * *Files 4% similar despite different names*

```diff
@@ -131,14 +131,17 @@
 
         if let Some((next_include, next_exclude)) = filter.key_filter(property_name_py, include, exclude)? {
             let next_value = model.getattr(property_name_py)?;
 
             let value = self
                 .serializer
                 .to_python(next_value, next_include, next_exclude, extra)?;
+            if extra.exclude_none && value.is_none(py) {
+                return Ok(());
+            }
             let key = match extra.by_alias {
                 true => self.alias_py.as_ref(py),
                 false => property_name_py,
             };
             output_dict.set_item(key, value)?;
         }
         Ok(())
```

### Comparing `pydantic_core-2.2.0/src/serializers/config.rs` & `pydantic_core-2.3.0/src/serializers/config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,17 @@
             ),
         }
     }
 }
 
 impl TimedeltaMode {
     pub fn from_config(config: Option<&PyDict>) -> PyResult<Self> {
-        let Some(config_dict) = config else { return Ok(Self::default()) };
+        let Some(config_dict) = config else {
+            return Ok(Self::default());
+        };
         let raw_mode = config_dict.get_as::<&str>(intern!(config_dict.py(), "ser_json_timedelta"))?;
         raw_mode.map_or_else(|| Ok(Self::default()), Self::from_str)
     }
 
     fn total_seconds(py_timedelta: &PyDelta) -> PyResult<&PyAny> {
         py_timedelta.call_method0(intern!(py_timedelta.py(), "total_seconds"))
     }
@@ -132,15 +134,17 @@
         };
         Ok(Self { base64_config })
     }
 }
 
 impl BytesMode {
     pub fn from_config(config: Option<&PyDict>) -> PyResult<Self> {
-        let Some(config_dict) = config else { return Ok(Self::default()) };
+        let Some(config_dict) = config else {
+            return Ok(Self::default());
+        };
         let raw_mode = config_dict.get_as::<&str>(intern!(config_dict.py(), "ser_json_bytes"))?;
         raw_mode.map_or_else(|| Ok(Self::default()), Self::from_str)
     }
 
     pub fn bytes_to_string<'py>(&self, py: Python, bytes: &'py [u8]) -> PyResult<Cow<'py, str>> {
         if let Some(config) = self.base64_config {
             Ok(Cow::Owned(base64::encode_config(bytes, config)))
```

### Comparing `pydantic_core-2.2.0/src/serializers/errors.rs` & `pydantic_core-2.3.0/src/serializers/errors.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/extra.rs` & `pydantic_core-2.3.0/src/serializers/extra.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/fields.rs` & `pydantic_core-2.3.0/src/serializers/fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/filter.rs` & `pydantic_core-2.3.0/src/serializers/filter.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/infer.rs` & `pydantic_core-2.3.0/src/serializers/infer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             }
         }
         Ok::<PyObject, PyErr>(new_dict.into_py(py))
     };
 
     let serialize_with_serializer = || {
         let py_serializer = value.getattr(intern!(py, "__pydantic_serializer__"))?;
-        let serializer: SchemaSerializer = py_serializer.extract()?;
+        let serializer: PyRef<SchemaSerializer> = py_serializer.extract()?;
         let extra = serializer.build_extra(
             py,
             extra.mode,
             extra.by_alias,
             extra.warnings,
             extra.exclude_unset,
             extra.exclude_defaults,
@@ -254,15 +254,15 @@
                 new_dict.into_py(py)
             }
             ObType::PydanticSerializable => serialize_with_serializer()?,
             ObType::Dataclass => serialize_dict(dataclass_to_dict(value)?)?,
             ObType::Generator => {
                 let iter = super::type_serializers::generator::SerializationIterator::new(
                     value.downcast()?,
-                    super::type_serializers::any::AnySerializer::default().into(),
+                    super::type_serializers::any::AnySerializer.into(),
                     SchemaFilter::default(),
                     include,
                     exclude,
                     extra,
                 );
                 iter.into_py(py)
             }
@@ -460,15 +460,15 @@
             serializer.serialize_str(&py_url.__str__())
         }
         ObType::PydanticSerializable => {
             let py = value.py();
             let py_serializer = value
                 .getattr(intern!(py, "__pydantic_serializer__"))
                 .map_err(py_err_se_err)?;
-            let extracted_serializer: SchemaSerializer = py_serializer.extract().map_err(py_err_se_err)?;
+            let extracted_serializer: PyRef<SchemaSerializer> = py_serializer.extract().map_err(py_err_se_err)?;
             let extra = extracted_serializer.build_extra(
                 py,
                 extra.mode,
                 extra.by_alias,
                 extra.warnings,
                 extra.exclude_unset,
                 extra.exclude_defaults,
```

### Comparing `pydantic_core-2.2.0/src/serializers/mod.rs` & `pydantic_core-2.3.0/src/serializers/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::fmt::Debug;
+use std::sync::atomic::{AtomicUsize, Ordering};
 
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyDict};
 use pyo3::{PyTraverseError, PyVisit};
 
 use crate::definitions::DefinitionsBuilder;
 use crate::validators::SelfValidator;
@@ -22,19 +23,19 @@
 mod filter;
 mod infer;
 mod ob_type;
 mod shared;
 mod type_serializers;
 
 #[pyclass(module = "pydantic_core._pydantic_core")]
-#[derive(Debug, Clone)]
+#[derive(Debug)]
 pub struct SchemaSerializer {
     serializer: CombinedSerializer,
     definitions: Vec<CombinedSerializer>,
-    json_size: usize,
+    expected_json_size: AtomicUsize,
     config: SerializationConfig,
 }
 
 impl SchemaSerializer {
     #[allow(clippy::too_many_arguments)]
     pub(crate) fn build_extra<'b, 'a: 'b>(
         &'b self,
@@ -76,15 +77,15 @@
         let schema = self_validator.validate_schema(py, schema)?;
         let mut definitions_builder = DefinitionsBuilder::new();
 
         let serializer = CombinedSerializer::build(schema.downcast()?, config, &mut definitions_builder)?;
         Ok(Self {
             serializer,
             definitions: definitions_builder.finish()?,
-            json_size: 1024,
+            expected_json_size: AtomicUsize::new(1024),
             config: SerializationConfig::from_config(config)?,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     #[pyo3(signature = (value, *, mode = None, include = None, exclude = None, by_alias = true,
         exclude_unset = false, exclude_defaults = false, exclude_none = false, round_trip = false, warnings = true,
@@ -126,15 +127,15 @@
     }
 
     #[allow(clippy::too_many_arguments)]
     #[pyo3(signature = (value, *, indent = None, include = None, exclude = None, by_alias = true,
         exclude_unset = false, exclude_defaults = false, exclude_none = false, round_trip = false, warnings = true,
         fallback = None))]
     pub fn to_json(
-        &mut self,
+        &self,
         py: Python,
         value: &PyAny,
         indent: Option<usize>,
         include: Option<&PyAny>,
         exclude: Option<&PyAny>,
         by_alias: bool,
         exclude_unset: bool,
@@ -162,20 +163,20 @@
         let bytes = to_json_bytes(
             value,
             &self.serializer,
             include,
             exclude,
             &extra,
             indent,
-            self.json_size,
+            self.expected_json_size.load(Ordering::Relaxed),
         )?;
 
         warnings.final_check(py)?;
 
-        self.json_size = bytes.len();
+        self.expected_json_size.store(bytes.len(), Ordering::Relaxed);
         let py_bytes = PyBytes::new(py, &bytes);
         Ok(py_bytes.into())
     }
 
     pub fn __repr__(&self) -> String {
         format!(
             "SchemaSerializer(serializer={:#?}, definitions={:#?})",
@@ -224,15 +225,15 @@
         &SerMode::Json,
         by_alias,
         exclude_none,
         round_trip,
         serialize_unknown,
         fallback,
     );
-    let serializer = type_serializers::any::AnySerializer::default().into();
+    let serializer = type_serializers::any::AnySerializer.into();
     let bytes = to_json_bytes(value, &serializer, include, exclude, &extra, indent, 1024)?;
     state.final_check(py)?;
     let py_bytes = PyBytes::new(py, &bytes);
     Ok(py_bytes.into())
 }
 
 #[allow(clippy::too_many_arguments)]
```

### Comparing `pydantic_core-2.2.0/src/serializers/ob_type.rs` & `pydantic_core-2.3.0/src/serializers/ob_type.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/shared.rs` & `pydantic_core-2.3.0/src/serializers/shared.rs`

 * *Files 0% similar despite different names*

```diff
@@ -304,19 +304,19 @@
 pub(crate) fn to_json_bytes(
     value: &PyAny,
     serializer: &CombinedSerializer,
     include: Option<&PyAny>,
     exclude: Option<&PyAny>,
     extra: &Extra,
     indent: Option<usize>,
-    json_size: usize,
+    expected_json_size: usize,
 ) -> PyResult<Vec<u8>> {
     let serializer = PydanticSerializer::new(value, serializer, include, exclude, extra);
 
-    let writer: Vec<u8> = Vec::with_capacity(json_size);
+    let writer: Vec<u8> = Vec::with_capacity(expected_json_size);
     let bytes = match indent {
         Some(indent) => {
             let indent = vec![b' '; indent];
             let formatter = PrettyFormatter::with_indent(&indent);
             let mut ser = serde_json::Serializer::with_formatter(writer, formatter);
             serializer.serialize(&mut ser).map_err(se_err_py_err)?;
             ser.into_inner()
```

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/any.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/bytes.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/dataclass.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/datetime_etc.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/datetime_etc.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/definitions.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/dict.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/format.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/format.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/function.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/generator.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/json.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/json_or_python.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/list.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/literal.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/mod.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 pub mod timedelta;
 pub mod tuple;
 pub mod typed_dict;
 pub mod union;
 pub mod url;
 pub mod with_default;
 
-pub(self) use super::computed_fields::ComputedFields;
-pub(self) use super::config::utf8_py_error;
-pub(self) use super::errors::{py_err_se_err, PydanticSerializationError};
-pub(self) use super::extra::{Extra, ExtraOwned, SerCheck, SerMode};
-pub(self) use super::fields::{FieldsMode, GeneralFieldsSerializer, SerField};
-pub(self) use super::filter::{AnyFilter, SchemaFilter};
-pub(self) use super::infer::{infer_json_key, infer_json_key_known, infer_serialize, infer_to_python};
-pub(self) use super::ob_type::{IsType, ObType};
-pub(self) use super::shared::{to_json_bytes, BuildSerializer, CombinedSerializer, PydanticSerializer, TypeSerializer};
+use super::computed_fields::ComputedFields;
+use super::config::utf8_py_error;
+use super::errors::{py_err_se_err, PydanticSerializationError};
+use super::extra::{Extra, ExtraOwned, SerCheck, SerMode};
+use super::fields::{FieldsMode, GeneralFieldsSerializer, SerField};
+use super::filter::{AnyFilter, SchemaFilter};
+use super::infer::{infer_json_key, infer_json_key_known, infer_serialize, infer_to_python};
+use super::ob_type::{IsType, ObType};
+use super::shared::{to_json_bytes, BuildSerializer, CombinedSerializer, PydanticSerializer, TypeSerializer};
```

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/model.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/nullable.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/other.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/other.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/set_frozenset.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/set_frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/simple.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/simple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/string.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/timedelta.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/tuple.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/typed_dict.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/union.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/url.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/serializers/type_serializers/with_default.rs` & `pydantic_core-2.3.0/src/serializers/type_serializers/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/tools.rs` & `pydantic_core-2.3.0/src/tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/url.rs` & `pydantic_core-2.3.0/src/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/any.rs` & `pydantic_core-2.3.0/src/validators/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/arguments.rs` & `pydantic_core-2.3.0/src/validators/arguments.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/bool.rs` & `pydantic_core-2.3.0/src/validators/bool.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/bytes.rs` & `pydantic_core-2.3.0/src/validators/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/call.rs` & `pydantic_core-2.3.0/src/validators/call.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/callable.rs` & `pydantic_core-2.3.0/src/validators/callable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/chain.rs` & `pydantic_core-2.3.0/src/validators/chain.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/custom_error.rs` & `pydantic_core-2.3.0/src/validators/custom_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/dataclass.rs` & `pydantic_core-2.3.0/src/validators/dataclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/date.rs` & `pydantic_core-2.3.0/src/validators/date.rs`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 /// In lax mode, if the input is not a date, we try parsing the input as a datetime, then check it is an
 /// "exact date", e.g. has a zero time component.
 fn date_from_datetime<'data>(
     input: &'data impl Input<'data>,
     date_err: ValError<'data>,
 ) -> ValResult<'data, EitherDate<'data>> {
-    let either_dt = match input.validate_datetime(false) {
+    let either_dt = match input.validate_datetime(false, speedate::MicrosecondsPrecisionOverflowBehavior::Truncate) {
         Ok(dt) => dt,
         Err(dt_err) => {
             return match dt_err {
                 ValError::LineErrors(mut line_errors) => {
                     // if we got a errors while parsing the datetime,
                     // convert DateTimeParsing -> DateFromDatetimeParsing but keep the rest of the error unchanged
                     for line_error in &mut line_errors {
@@ -149,15 +149,15 @@
     };
     let dt = either_dt.as_raw()?;
     let zero_time = Time {
         hour: 0,
         minute: 0,
         second: 0,
         microsecond: 0,
-        tz_offset: None,
+        tz_offset: dt.time.tz_offset,
     };
     if dt.time == zero_time {
         Ok(EitherDate::Raw(dt.date))
     } else {
         Err(ValError::new(ErrorType::DateFromDatetimeInexact, input))
     }
 }
```

### Comparing `pydantic_core-2.2.0/src/validators/datetime.rs` & `pydantic_core-2.3.0/src/validators/datetime.rs`

 * *Files 9% similar despite different names*

```diff
@@ -2,55 +2,73 @@
 use pyo3::once_cell::GILOnceCell;
 use pyo3::prelude::*;
 use pyo3::types::{PyDateTime, PyDict, PyString};
 use speedate::DateTime;
 use std::cmp::Ordering;
 use strum::EnumMessage;
 
-use crate::build_tools::py_schema_err;
 use crate::build_tools::{is_strict, py_schema_error_type};
+use crate::build_tools::{py_schema_err, schema_or_config_same};
 use crate::errors::{py_err_string, ErrorType, ValError, ValResult};
 use crate::input::{EitherDateTime, Input};
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::SchemaDict;
 
 use super::{BuildValidator, CombinedValidator, Definitions, DefinitionsBuilder, Extra, Validator};
 
 #[derive(Debug, Clone)]
 pub struct DateTimeValidator {
     strict: bool,
     constraints: Option<DateTimeConstraints>,
+    microseconds_precision: speedate::MicrosecondsPrecisionOverflowBehavior,
+}
+
+pub(crate) fn extract_microseconds_precision(
+    schema: &PyDict,
+    config: Option<&PyDict>,
+) -> PyResult<speedate::MicrosecondsPrecisionOverflowBehavior> {
+    schema_or_config_same(schema, config, intern!(schema.py(), "microseconds_precision"))?
+        .map_or(
+            Ok(speedate::MicrosecondsPrecisionOverflowBehavior::Truncate),
+            |v: &PyString| {
+                speedate::MicrosecondsPrecisionOverflowBehavior::try_from(String::extract(v).unwrap().as_str())
+            },
+        )
+        .map_err(|_| {
+            py_schema_error_type!("Invalid `microseconds_precision`, must be one of \"truncate\" or \"error\"")
+        })
 }
 
 impl BuildValidator for DateTimeValidator {
     const EXPECTED_TYPE: &'static str = "datetime";
 
     fn build(
         schema: &PyDict,
         config: Option<&PyDict>,
         _definitions: &mut DefinitionsBuilder<CombinedValidator>,
     ) -> PyResult<CombinedValidator> {
         Ok(Self {
             strict: is_strict(schema, config)?,
             constraints: DateTimeConstraints::from_py(schema)?,
+            microseconds_precision: extract_microseconds_precision(schema, config)?,
         }
         .into())
     }
 }
 
 impl Validator for DateTimeValidator {
     fn validate<'s, 'data>(
         &'s self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         extra: &Extra,
         _definitions: &'data Definitions<CombinedValidator>,
         _recursion_guard: &'s mut RecursionGuard,
     ) -> ValResult<'data, PyObject> {
-        let datetime = input.validate_datetime(extra.strict.unwrap_or(self.strict))?;
+        let datetime = input.validate_datetime(extra.strict.unwrap_or(self.strict), self.microseconds_precision)?;
         if let Some(constraints) = &self.constraints {
             // if we get an error from as_speedate, it's probably because the input datetime was invalid
             // specifically had an invalid tzinfo, hence here we return a validation error
             let speedate_dt = match datetime.as_raw() {
                 Ok(dt) => dt,
                 Err(err) => {
                     let error = py_err_string(py, err);
```

### Comparing `pydantic_core-2.2.0/src/validators/definitions.rs` & `pydantic_core-2.3.0/src/validators/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/dict.rs` & `pydantic_core-2.3.0/src/validators/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/float.rs` & `pydantic_core-2.3.0/src/validators/float.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/frozenset.rs` & `pydantic_core-2.3.0/src/validators/frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/function.rs` & `pydantic_core-2.3.0/src/validators/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/generator.rs` & `pydantic_core-2.3.0/src/validators/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/int.rs` & `pydantic_core-2.3.0/src/validators/int.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/is_instance.rs` & `pydantic_core-2.3.0/src/validators/is_instance.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/is_subclass.rs` & `pydantic_core-2.3.0/src/validators/is_subclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/json.rs` & `pydantic_core-2.3.0/src/validators/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/json_or_python.rs` & `pydantic_core-2.3.0/src/validators/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/lax_or_strict.rs` & `pydantic_core-2.3.0/src/validators/lax_or_strict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/list.rs` & `pydantic_core-2.3.0/src/validators/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/literal.rs` & `pydantic_core-2.3.0/src/validators/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/mod.rs` & `pydantic_core-2.3.0/src/validators/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/model.rs` & `pydantic_core-2.3.0/src/validators/model.rs`

 * *Files 3% similar despite different names*

```diff
@@ -179,40 +179,49 @@
                     .validator
                     .validate(py, field_value, &field_extra, definitions, recursion_guard)?;
 
                 force_setattr(py, model, intern!(py, ROOT_FIELD), output)?;
                 Ok(model.into_py(py))
             };
         }
-        let dict: &PyDict = model.getattr(intern!(py, DUNDER_DICT))?.downcast()?;
+        let old_dict: &PyDict = model.getattr(intern!(py, DUNDER_DICT))?.downcast()?;
 
-        let new_dict = dict.copy()?;
-        new_dict.set_item(field_name, field_value)?;
+        let input_dict = old_dict.copy()?;
+        let old_extra: Option<&PyDict> = model.getattr(intern!(py, DUNDER_MODEL_EXTRA_KEY))?.downcast().ok();
+        if let Some(old_extra) = old_extra {
+            input_dict.update(old_extra.as_mapping())?;
+        }
+        input_dict.set_item(field_name, field_value)?;
 
         let output = self.validator.validate_assignment(
             py,
-            new_dict,
+            input_dict,
             field_name,
             field_value,
             extra,
             definitions,
             recursion_guard,
         )?;
 
-        let (output, _, updated_fields_set): (&PyDict, &PyAny, &PySet) = output.extract(py)?;
+        let (validated_dict, validated_extra, validated_fields_set): (&PyDict, &PyAny, &PySet) = output.extract(py)?;
 
         if let Ok(fields_set) = model.getattr(intern!(py, DUNDER_FIELDS_SET_KEY)) {
             let fields_set: &PySet = fields_set.downcast()?;
-            for field_name in updated_fields_set {
+            for field_name in validated_fields_set {
                 fields_set.add(field_name)?;
             }
         }
-        let output = output.to_object(py);
 
-        force_setattr(py, model, intern!(py, DUNDER_DICT), output)?;
+        force_setattr(py, model, intern!(py, DUNDER_DICT), validated_dict.to_object(py))?;
+        force_setattr(
+            py,
+            model,
+            intern!(py, DUNDER_MODEL_EXTRA_KEY),
+            validated_extra.to_object(py),
+        )?;
         Ok(model.into_py(py))
     }
 
     fn different_strict_behavior(
         &self,
         definitions: Option<&DefinitionsBuilder<CombinedValidator>>,
         ultra_strict: bool,
```

### Comparing `pydantic_core-2.2.0/src/validators/model_fields.rs` & `pydantic_core-2.3.0/src/validators/model_fields.rs`

 * *Files 6% similar despite different names*

```diff
@@ -298,21 +298,21 @@
         field_value: &'data PyAny,
         extra: &Extra,
         definitions: &'data Definitions<CombinedValidator>,
         recursion_guard: &'s mut RecursionGuard,
     ) -> ValResult<'data, PyObject> {
         let dict: &PyDict = obj.downcast()?;
 
-        let ok = |output: PyObject| {
+        let get_updated_dict = |output: PyObject| {
             dict.set_item(field_name, output)?;
-            Ok(dict.to_object(py))
+            Ok(dict)
         };
 
         let prepare_result = |result: ValResult<'data, PyObject>| match result {
-            Ok(output) => ok(output),
+            Ok(output) => get_updated_dict(output),
             Err(ValError::LineErrors(line_errors)) => {
                 let errors = line_errors
                     .into_iter()
                     .map(|e| e.with_outer_location(field_name.to_string().into()))
                     .collect();
                 Err(ValError::LineErrors(errors))
             }
@@ -354,30 +354,46 @@
             // For models / typed dicts we forbid assigning extra attributes
             // unless the user explicitly set extra_behavior to 'allow'
             match self.extra_behavior {
                 ExtraBehavior::Allow => match self.extra_validator {
                     Some(ref validator) => {
                         prepare_result(validator.validate(py, field_value, &extra, definitions, recursion_guard))
                     }
-                    None => ok(field_value.to_object(py)),
+                    None => get_updated_dict(field_value.to_object(py)),
                 },
                 ExtraBehavior::Forbid | ExtraBehavior::Ignore => {
                     return Err(ValError::new_with_loc(
                         ErrorType::NoSuchAttribute {
                             attribute: field_name.to_string(),
                         },
                         field_value,
                         field_name.to_string(),
                     ))
                 }
             }
         }?;
 
+        let new_extra = match &self.extra_behavior {
+            ExtraBehavior::Allow => {
+                let non_extra_data = PyDict::new(py);
+                self.fields.iter().for_each(|f| {
+                    let popped_value = PyAny::get_item(new_data, &f.name).unwrap();
+                    new_data.del_item(&f.name).unwrap();
+                    non_extra_data.set_item(&f.name, popped_value).unwrap();
+                });
+                let new_extra = new_data.copy()?;
+                new_data.clear();
+                new_data.update(non_extra_data.as_mapping())?;
+                new_extra.to_object(py)
+            }
+            _ => py.None(),
+        };
+
         let fields_set: &PySet = PySet::new(py, &[field_name.to_string()])?;
-        Ok((new_data, py.None(), fields_set.to_object(py)).to_object(py))
+        Ok((new_data.to_object(py), new_extra, fields_set.to_object(py)).to_object(py))
     }
 
     fn different_strict_behavior(
         &self,
         definitions: Option<&DefinitionsBuilder<CombinedValidator>>,
         ultra_strict: bool,
     ) -> bool {
```

### Comparing `pydantic_core-2.2.0/src/validators/none.rs` & `pydantic_core-2.3.0/src/validators/none.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/nullable.rs` & `pydantic_core-2.3.0/src/validators/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/set.rs` & `pydantic_core-2.3.0/src/validators/set.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/string.rs` & `pydantic_core-2.3.0/src/validators/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/time.rs` & `pydantic_core-2.3.0/src/validators/time.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,49 +6,52 @@
 
 use crate::build_tools::is_strict;
 use crate::errors::{ErrorType, ValError, ValResult};
 use crate::input::{EitherTime, Input};
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::SchemaDict;
 
+use super::datetime::extract_microseconds_precision;
 use super::datetime::TZConstraint;
 use super::{BuildValidator, CombinedValidator, Definitions, DefinitionsBuilder, Extra, Validator};
 
 #[derive(Debug, Clone)]
 pub struct TimeValidator {
     strict: bool,
     constraints: Option<TimeConstraints>,
+    microseconds_precision: speedate::MicrosecondsPrecisionOverflowBehavior,
 }
 
 impl BuildValidator for TimeValidator {
     const EXPECTED_TYPE: &'static str = "time";
 
     fn build(
         schema: &PyDict,
         config: Option<&PyDict>,
         _definitions: &mut DefinitionsBuilder<CombinedValidator>,
     ) -> PyResult<CombinedValidator> {
         let s = Self {
             strict: is_strict(schema, config)?,
             constraints: TimeConstraints::from_py(schema)?,
+            microseconds_precision: extract_microseconds_precision(schema, config)?,
         };
         Ok(s.into())
     }
 }
 
 impl Validator for TimeValidator {
     fn validate<'s, 'data>(
         &'s self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         extra: &Extra,
         _definitions: &'data Definitions<CombinedValidator>,
         _recursion_guard: &'s mut RecursionGuard,
     ) -> ValResult<'data, PyObject> {
-        let time = input.validate_time(extra.strict.unwrap_or(self.strict))?;
+        let time = input.validate_time(extra.strict.unwrap_or(self.strict), self.microseconds_precision)?;
         if let Some(constraints) = &self.constraints {
             let raw_time = time.as_raw()?;
 
             macro_rules! check_constraint {
                 ($constraint:ident, $error:ident) => {
                     if let Some(constraint) = &constraints.$constraint {
                         if !raw_time.$constraint(constraint) {
```

### Comparing `pydantic_core-2.2.0/src/validators/timedelta.rs` & `pydantic_core-2.3.0/src/validators/timedelta.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 use crate::build_tools::is_strict;
 use crate::errors::{ErrorType, ValError, ValResult};
 use crate::input::{duration_as_pytimedelta, pytimedelta_as_duration, Input};
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::SchemaDict;
 
+use super::datetime::extract_microseconds_precision;
 use super::{BuildValidator, CombinedValidator, Definitions, DefinitionsBuilder, Extra, Validator};
 
 #[derive(Debug, Clone)]
 pub struct TimeDeltaValidator {
     strict: bool,
     constraints: Option<TimedeltaConstraints>,
+    microseconds_precision: speedate::MicrosecondsPrecisionOverflowBehavior,
 }
 
 #[derive(Debug, Clone)]
 struct TimedeltaConstraints {
     le: Option<Duration>,
     lt: Option<Duration>,
     ge: Option<Duration>,
@@ -52,29 +54,30 @@
         Ok(Self {
             strict: is_strict(schema, config)?,
             constraints: (constraints.le.is_some()
                 || constraints.lt.is_some()
                 || constraints.ge.is_some()
                 || constraints.gt.is_some())
             .then_some(constraints),
+            microseconds_precision: extract_microseconds_precision(schema, config)?,
         }
         .into())
     }
 }
 
 impl Validator for TimeDeltaValidator {
     fn validate<'s, 'data>(
         &'s self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         extra: &Extra,
         _definitions: &'data Definitions<CombinedValidator>,
         _recursion_guard: &'s mut RecursionGuard,
     ) -> ValResult<'data, PyObject> {
-        let timedelta = input.validate_timedelta(extra.strict.unwrap_or(self.strict))?;
+        let timedelta = input.validate_timedelta(extra.strict.unwrap_or(self.strict), self.microseconds_precision)?;
         let py_timedelta = timedelta.try_into_py(py)?;
         if let Some(constraints) = &self.constraints {
             let raw_timedelta = timedelta.as_raw();
 
             macro_rules! check_constraint {
                 ($constraint:ident, $error:ident) => {
                     if let Some(constraint) = &constraints.$constraint {
```

### Comparing `pydantic_core-2.2.0/src/validators/tuple.rs` & `pydantic_core-2.3.0/src/validators/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/typed_dict.rs` & `pydantic_core-2.3.0/src/validators/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/union.rs` & `pydantic_core-2.3.0/src/validators/union.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/url.rs` & `pydantic_core-2.3.0/src/validators/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/src/validators/with_default.rs` & `pydantic_core-2.3.0/src/validators/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/benchmarks/complete_schema.py` & `pydantic_core-2.3.0/tests/benchmarks/complete_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/benchmarks/test_complete_benchmark.py` & `pydantic_core-2.3.0/tests/benchmarks/test_complete_benchmark.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/benchmarks/test_micro_benchmarks.py` & `pydantic_core-2.3.0/tests/benchmarks/test_micro_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/benchmarks/test_serialization_micro.py` & `pydantic_core-2.3.0/tests/benchmarks/test_serialization_micro.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/conftest.py` & `pydantic_core-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/emscripten_runner.js` & `pydantic_core-2.3.0/tests/emscripten_runner.js`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_any.py` & `pydantic_core-2.3.0/tests/serializers/test_any.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_bytes.py` & `pydantic_core-2.3.0/tests/serializers/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_dataclasses.py` & `pydantic_core-2.3.0/tests/serializers/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_datetime.py` & `pydantic_core-2.3.0/tests/serializers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_definitions.py` & `pydantic_core-2.3.0/tests/serializers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_definitions_recursive.py` & `pydantic_core-2.3.0/tests/serializers/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_dict.py` & `pydantic_core-2.3.0/tests/serializers/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_format.py` & `pydantic_core-2.3.0/tests/serializers/test_format.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_functions.py` & `pydantic_core-2.3.0/tests/serializers/test_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,17 +623,15 @@
     # insert_assert(str(exc_info.value))
     assert str(exc_info.value) == 'Error calling function `bad_recursive`: RecursionError'
 
     with pytest.raises(PydanticSerializationError) as exc_info:
         s.to_json(42)
     # insert_assert(str(exc_info.value))
     assert str(exc_info.value) == (
-        'Error serializing to JSON: '
-        'PydanticSerializationError: Error calling function `bad_recursive`: '
-        'RuntimeError: Already mutably borrowed'
+        'Error serializing to JSON: PydanticSerializationError: Error calling function `bad_recursive`: RecursionError'
     )
 
 
 def test_serialize_pattern():
     ser = core_schema.plain_serializer_function_ser_schema(
         attrgetter('pattern'), when_used='json', return_schema=core_schema.str_schema()
     )
```

### Comparing `pydantic_core-2.2.0/tests/serializers/test_generator.py` & `pydantic_core-2.3.0/tests/serializers/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_json.py` & `pydantic_core-2.3.0/tests/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_json_or_python.py` & `pydantic_core-2.3.0/tests/serializers/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_list_tuple.py` & `pydantic_core-2.3.0/tests/serializers/test_list_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_literal.py` & `pydantic_core-2.3.0/tests/serializers/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_misc.py` & `pydantic_core-2.3.0/tests/serializers/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_model.py` & `pydantic_core-2.3.0/tests/serializers/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,30 @@
     j = s.to_json(BasicModel(bar=b'more', foo=1, __pydantic_extra__=dict(c=3)))
     if on_pypy:
         assert j == IsJson({'bar': 'more', 'foo': 1, 'c': 3})
     else:
         assert j == b'{"bar":"more","foo":1,"c":3}'
 
 
+def test_model_recursive_in_extra():
+    # See https://github.com/pydantic/pydantic/issues/6571
+
+    class Model(BasicModel):
+        __slots__ = '__pydantic_extra__'
+
+    s = SchemaSerializer(
+        core_schema.model_schema(
+            Model, core_schema.model_fields_schema({}, extra_behavior='allow'), extra_behavior='allow'
+        )
+    )
+    Model.__pydantic_serializer__ = s
+
+    assert s.to_json(Model(__pydantic_extra__=dict(other=Model(__pydantic_extra__={})))) == b'{"other":{}}'
+
+
 @pytest.mark.parametrize(
     'params',
     [
         dict(include=None, exclude=None, expected={'a': 0, 'b': 1, 'c': 2, 'd': 3}),
         dict(include={'a', 'b'}, exclude=None, expected={'a': 0, 'b': 1}),
         dict(include={'a': ..., 'b': ...}, exclude=None, expected={'a': 0, 'b': 1}),
         dict(include={'a': {1}, 'b': {1}}, exclude=None, expected={'a': 0, 'b': 1}),
@@ -585,14 +601,54 @@
         )
     )
     assert s.to_python(Model(3, 4)) == {'width': 3, 'height': 4, 'Area': 12, 'volume': 48}
     assert s.to_python(Model(3, 4), mode='json') == {'width': 3, 'height': 4, 'Area': 12, 'volume': 48}
     assert s.to_json(Model(3, 4)) == b'{"width":3,"height":4,"Area":12,"volume":48}'
 
 
+def test_computed_field_to_python_exclude_none():
+    @dataclasses.dataclass
+    class Model:
+        width: int
+        height: int
+
+        @property
+        def area(self) -> int:
+            return self.width * self.height
+
+        @property
+        def volume(self) -> None:
+            return None
+
+    s = SchemaSerializer(
+        core_schema.model_schema(
+            Model,
+            core_schema.model_fields_schema(
+                {
+                    'width': core_schema.model_field(core_schema.int_schema()),
+                    'height': core_schema.model_field(core_schema.int_schema()),
+                },
+                computed_fields=[
+                    core_schema.computed_field('area', core_schema.int_schema(), alias='Area'),
+                    core_schema.computed_field('volume', core_schema.int_schema()),
+                ],
+            ),
+        )
+    )
+    assert s.to_python(Model(3, 4), exclude_none=False) == {'width': 3, 'height': 4, 'Area': 12, 'volume': None}
+    assert s.to_python(Model(3, 4), exclude_none=True) == {'width': 3, 'height': 4, 'Area': 12}
+    assert s.to_python(Model(3, 4), mode='json', exclude_none=False) == {
+        'width': 3,
+        'height': 4,
+        'Area': 12,
+        'volume': None,
+    }
+    assert s.to_python(Model(3, 4), mode='json', exclude_none=True) == {'width': 3, 'height': 4, 'Area': 12}
+
+
 @pytest.mark.skipif(cached_property is None, reason='cached_property is not available')
 def test_cached_property_alias():
     @dataclasses.dataclass
     class Model:
         width: int
         height: int
```

### Comparing `pydantic_core-2.2.0/tests/serializers/test_model_root.py` & `pydantic_core-2.3.0/tests/serializers/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_none.py` & `pydantic_core-2.3.0/tests/serializers/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_nullable.py` & `pydantic_core-2.3.0/tests/serializers/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_other.py` & `pydantic_core-2.3.0/tests/serializers/test_other.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_set_frozenset.py` & `pydantic_core-2.3.0/tests/serializers/test_set_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_simple.py` & `pydantic_core-2.3.0/tests/serializers/test_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_string.py` & `pydantic_core-2.3.0/tests/serializers/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_timedelta.py` & `pydantic_core-2.3.0/tests/serializers/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_typed_dict.py` & `pydantic_core-2.3.0/tests/serializers/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_union.py` & `pydantic_core-2.3.0/tests/serializers/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/serializers/test_url.py` & `pydantic_core-2.3.0/tests/serializers/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test.rs` & `pydantic_core-2.3.0/tests/test.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_build.py` & `pydantic_core-2.3.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_config.py` & `pydantic_core-2.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_docstrings.py` & `pydantic_core-2.3.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_errors.py` & `pydantic_core-2.3.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_garbage_collection.py` & `pydantic_core-2.3.0/tests/test_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_hypothesis.py` & `pydantic_core-2.3.0/tests/test_hypothesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 tzinfo=None, microsecond=microsecond
             )
         else:
             expected = datetime.fromtimestamp(data, tz=timezone.utc).replace(tzinfo=None)
     except OverflowError:
         pytest.skip('OverflowError, see pyodide/pyodide#2841, this can happen on 32-bit systems')
     else:
-        assert datetime_schema.validate_python(data) == expected, data
+        assert datetime_schema.validate_python(data).replace(tzinfo=None) == expected, data
 
 
 @given(strategies.binary())
 def test_datetime_binary(datetime_schema, data):
     try:
         datetime_schema.validate_python(data)
     except ValidationError as exc:
```

### Comparing `pydantic_core-2.2.0/tests/test_isinstance.py` & `pydantic_core-2.3.0/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_json.py` & `pydantic_core-2.3.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_misc.py` & `pydantic_core-2.3.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_schema_functions.py` & `pydantic_core-2.3.0/tests/test_schema_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,32 @@
     (core_schema.float_schema, args(multiple_of=5, gt=1.2), {'type': 'float', 'multiple_of': 5, 'gt': 1.2}),
     (core_schema.str_schema, args(), {'type': 'str'}),
     (core_schema.str_schema, args(min_length=5, max_length=10), {'type': 'str', 'min_length': 5, 'max_length': 10}),
     (core_schema.bytes_schema, args(), {'type': 'bytes'}),
     (core_schema.bytes_schema, args(min_length=5, ref='xx'), {'type': 'bytes', 'min_length': 5, 'ref': 'xx'}),
     (core_schema.date_schema, args(), {'type': 'date'}),
     (core_schema.date_schema, args(gt=date(2020, 1, 1)), {'type': 'date', 'gt': date(2020, 1, 1)}),
-    (core_schema.time_schema, args(), {'type': 'time'}),
-    (core_schema.datetime_schema, args(), {'type': 'datetime'}),
-    (core_schema.timedelta_schema, args(), {'type': 'timedelta'}),
+    (core_schema.time_schema, args(), {'type': 'time', 'microseconds_precision': 'truncate'}),
+    (core_schema.datetime_schema, args(), {'type': 'datetime', 'microseconds_precision': 'truncate'}),
+    (core_schema.timedelta_schema, args(), {'type': 'timedelta', 'microseconds_precision': 'truncate'}),
+    (
+        core_schema.time_schema,
+        args(microseconds_precision='error'),
+        {'type': 'time', 'microseconds_precision': 'error'},
+    ),
+    (
+        core_schema.datetime_schema,
+        args(microseconds_precision='error'),
+        {'type': 'datetime', 'microseconds_precision': 'error'},
+    ),
+    (
+        core_schema.timedelta_schema,
+        args(microseconds_precision='error'),
+        {'type': 'timedelta', 'microseconds_precision': 'error'},
+    ),
     (core_schema.literal_schema, args(['a', 'b']), {'type': 'literal', 'expected': ['a', 'b']}),
     (core_schema.is_instance_schema, args(int), {'type': 'is-instance', 'cls': int}),
     (core_schema.callable_schema, args(), {'type': 'callable'}),
     (core_schema.list_schema, args(), {'type': 'list'}),
     (core_schema.list_schema, args({'type': 'int'}), {'type': 'list', 'items_schema': {'type': 'int'}}),
     (
         core_schema.tuple_positional_schema,
```

### Comparing `pydantic_core-2.2.0/tests/test_strict.py` & `pydantic_core-2.3.0/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_typing.py` & `pydantic_core-2.3.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/test_validation_context.py` & `pydantic_core-2.3.0/tests/test_validation_context.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_arguments.py` & `pydantic_core-2.3.0/tests/validators/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_bool.py` & `pydantic_core-2.3.0/tests/validators/test_bool.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_bytes.py` & `pydantic_core-2.3.0/tests/validators/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_call.py` & `pydantic_core-2.3.0/tests/validators/test_call.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_callable.py` & `pydantic_core-2.3.0/tests/validators/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_chain.py` & `pydantic_core-2.3.0/tests/validators/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_custom_error.py` & `pydantic_core-2.3.0/tests/validators/test_custom_error.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_dataclasses.py` & `pydantic_core-2.3.0/tests/validators/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_date.py` & `pydantic_core-2.3.0/tests/validators/test_date.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_datetime.py` & `pydantic_core-2.3.0/tests/validators/test_datetime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import copy
 import json
+import pickle
 import platform
 import re
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from decimal import Decimal
+from typing import Dict
 
 import pytest
 import pytz
 
 from pydantic_core import SchemaError, SchemaValidator, ValidationError, core_schema
 
 from ..conftest import Err, PyAndJson
@@ -15,25 +17,25 @@
 
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         (datetime(2022, 6, 8, 12, 13, 14), datetime(2022, 6, 8, 12, 13, 14)),
         (date(2022, 6, 8), datetime(2022, 6, 8)),
         ('2022-06-08T12:13:14', datetime(2022, 6, 8, 12, 13, 14)),
-        ('1000000000000', datetime(2001, 9, 9, 1, 46, 40)),
+        ('1000000000000', datetime(2001, 9, 9, 1, 46, 40, tzinfo=timezone.utc)),
         (b'2022-06-08T12:13:14', datetime(2022, 6, 8, 12, 13, 14)),
         (b'2022-06-08T12:13:14Z', datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone.utc)),
         ((1,), Err('Input should be a valid datetime [type=datetime_type')),
         (time(1, 2, 3), Err('Input should be a valid datetime [type=datetime_type')),
-        (Decimal('1654646400'), datetime(2022, 6, 8)),
-        ('1654646400', datetime(2022, 6, 8)),
-        (Decimal('1654646400.123456'), datetime(2022, 6, 8, 0, 0, 0, 123456)),
-        (Decimal('1654646400.1234564'), datetime(2022, 6, 8, 0, 0, 0, 123456)),
-        (Decimal('1654646400.1234568'), datetime(2022, 6, 8, 0, 0, 0, 123457)),
-        ('1654646400.1234568', datetime(2022, 6, 8, 0, 0, 0, 123457)),
+        (Decimal('1654646400'), datetime(2022, 6, 8, tzinfo=timezone.utc)),
+        ('1654646400', datetime(2022, 6, 8, tzinfo=timezone.utc)),
+        (Decimal('1654646400.123456'), datetime(2022, 6, 8, 0, 0, 0, 123456, tzinfo=timezone.utc)),
+        (Decimal('1654646400.1234564'), datetime(2022, 6, 8, 0, 0, 0, 123456, tzinfo=timezone.utc)),
+        (Decimal('1654646400.1234568'), datetime(2022, 6, 8, 0, 0, 0, 123457, tzinfo=timezone.utc)),
+        ('1654646400.1234568', datetime(2022, 6, 8, 0, 0, 0, 123457, tzinfo=timezone.utc)),
         (253_402_300_800_000, Err('should be a valid datetime, dates after 9999 are not supported as unix timestamps')),
         (-20_000_000_000, Err('should be a valid datetime, dates before 1600 are not supported as unix timestamps')),
         (float('nan'), Err('Input should be a valid datetime, NaN values not permitted [type=datetime_parsing,')),
         (float('inf'), Err('Input should be a valid datetime, dates after 9999')),
         (float('-inf'), Err('Input should be a valid datetime, dates before 1600')),
     ],
 )
@@ -108,16 +110,16 @@
             '2022-06-08T12:13:14+12:15',
             datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone(timedelta(hours=12, minutes=15))),
         ),
         (
             '2022-06-08T12:13:14+23:59',
             datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone(timedelta(hours=23, minutes=59))),
         ),
-        (1655205632, datetime(2022, 6, 14, 11, 20, 32)),
-        (1655205632.331557, datetime(2022, 6, 14, 11, 20, 32, microsecond=331557)),
+        (1655205632, datetime(2022, 6, 14, 11, 20, 32, tzinfo=timezone.utc)),
+        (1655205632.331557, datetime(2022, 6, 14, 11, 20, 32, microsecond=331557, tzinfo=timezone.utc)),
         (
             '2022-06-08T12:13:14+24:00',
             Err('Input should be a valid datetime, timezone offset must be less than 24 hours [type=datetime_parsing,'),
         ),
         (True, Err('Input should be a valid datetime [type=datetime_type')),
         (None, Err('Input should be a valid datetime [type=datetime_type')),
         ([1, 2, 3], Err('Input should be a valid datetime [type=datetime_type')),
@@ -286,15 +288,15 @@
 
 
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         ('2022-06-08T12:13:14', datetime(2022, 6, 8, 12, 13, 14)),
         ('2022-06-08T12:13:14Z', datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone.utc)),
-        (1655205632, datetime(2022, 6, 14, 11, 20, 32)),
+        (1655205632, datetime(2022, 6, 14, 11, 20, 32, tzinfo=timezone.utc)),
         ('2068-06-08T12:13:14', Err('Input should be in the past [type=datetime_past,')),
         (3105730800, Err('Input should be in the past [type=datetime_past,')),
     ],
 )
 def test_datetime_past(py_and_json: PyAndJson, input_value, expected):
     v = py_and_json(core_schema.datetime_schema(now_utc_offset=0, now_op='past'))
     if isinstance(expected, Err):
@@ -329,15 +331,15 @@
 
 
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         ('2068-06-08T12:13:14', datetime(2068, 6, 8, 12, 13, 14)),
         ('2068-06-08T12:13:14Z', datetime(2068, 6, 8, 12, 13, 14, tzinfo=timezone.utc)),
-        (3105730800, datetime(2068, 5, 31, 23, 0)),
+        (3105730800, datetime(2068, 5, 31, 23, 0, tzinfo=timezone.utc)),
         ('2022-06-08T12:13:14', Err('Input should be in the future [type=datetime_future,')),
         (1655205632, Err('Input should be in the future [type=datetime_future,')),
     ],
 )
 def test_datetime_future(py_and_json: PyAndJson, input_value, expected):
     v = py_and_json(core_schema.datetime_schema(now_utc_offset=0, now_op='future'))
     if isinstance(expected, Err):
@@ -472,7 +474,42 @@
     with pytest.raises(SchemaError, match='OverflowError: Python int too large to convert to C long'):
         SchemaValidator(core_schema.datetime_schema(tz_constraint=2**64))
 
 
 def test_tz_constraint_wrong():
     with pytest.raises(SchemaError, match="Input should be 'aware' or 'naive"):
         SchemaValidator(core_schema.datetime_schema(tz_constraint='wrong'))
+
+
+def test_tz_pickle() -> None:
+    """
+    https://github.com/pydantic/pydantic-core/issues/589
+    """
+    v = SchemaValidator(core_schema.datetime_schema())
+    original = datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone(timedelta(hours=-12, minutes=-15)))
+    validated = v.validate_python('2022-06-08T12:13:14-12:15')
+    assert validated == original
+    assert pickle.loads(pickle.dumps(validated)) == validated == original
+
+
+def test_tz_hash() -> None:
+    v = SchemaValidator(core_schema.datetime_schema())
+    lookup: Dict[datetime, str] = {}
+    for day in range(1, 10):
+        input_str = f'2022-06-{day:02}T12:13:14-12:15'
+        validated = v.validate_python(input_str)
+        lookup[validated] = input_str
+
+    assert len(lookup) == 9
+    assert (
+        lookup[datetime(2022, 6, 8, 12, 13, 14, tzinfo=timezone(timedelta(hours=-12, minutes=-15)))]
+        == '2022-06-08T12:13:14-12:15'
+    )
+
+
+def test_tz_cmp() -> None:
+    v = SchemaValidator(core_schema.datetime_schema())
+    validated1 = v.validate_python('2022-06-08T12:13:14-12:15')
+    validated2 = v.validate_python('2022-06-08T12:13:14-12:14')
+
+    assert validated1 > validated2
+    assert validated2 < validated1
```

### Comparing `pydantic_core-2.2.0/tests/validators/test_definitions.py` & `pydantic_core-2.3.0/tests/validators/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_definitions_recursive.py` & `pydantic_core-2.3.0/tests/validators/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_dict.py` & `pydantic_core-2.3.0/tests/validators/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_float.py` & `pydantic_core-2.3.0/tests/validators/test_float.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_frozenset.py` & `pydantic_core-2.3.0/tests/validators/test_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_function.py` & `pydantic_core-2.3.0/tests/validators/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,27 +457,31 @@
         input_value.more = 'foobar'
         return input_value
 
     class Model:
         __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__', '__pydantic_private__'
         field_a: str
 
+        def __init__(self):
+            self.__pydantic_extra__ = None  # this attribute must be present for validate_assignment
+
     v = SchemaValidator(
         core_schema.no_info_after_validator_function(
             f,
             core_schema.model_schema(
                 Model, core_schema.model_fields_schema({'field_a': core_schema.model_field(core_schema.str_schema())})
             ),
         )
     )
     m = v.validate_python({'field_a': 'test'})
     assert isinstance(m, Model)
     assert m.field_a == 'test'
     assert m.__pydantic_fields_set__ == {'field_a'}
     assert m.__dict__ == {'field_a': 'test', 'more': 'foobar'}
+    assert m.__pydantic_extra__ is None
 
     m2 = Model()
     m2.field_a = 'test'
     assert v.validate_assignment(m2, 'field_a', b'abc') is m2
     assert m2.__dict__ == {'field_a': 'abc', 'more': 'foobar'}
     assert not hasattr(m2, '__pydantic_fields_set__')
```

### Comparing `pydantic_core-2.2.0/tests/validators/test_generator.py` & `pydantic_core-2.3.0/tests/validators/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_int.py` & `pydantic_core-2.3.0/tests/validators/test_int.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_is_instance.py` & `pydantic_core-2.3.0/tests/validators/test_is_instance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_is_subclass.py` & `pydantic_core-2.3.0/tests/validators/test_is_subclass.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_json.py` & `pydantic_core-2.3.0/tests/validators/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_json_or_python.py` & `pydantic_core-2.3.0/tests/validators/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_lax_or_strict.py` & `pydantic_core-2.3.0/tests/validators/test_lax_or_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_list.py` & `pydantic_core-2.3.0/tests/validators/test_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_literal.py` & `pydantic_core-2.3.0/tests/validators/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_model.py` & `pydantic_core-2.3.0/tests/validators/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -939,14 +939,17 @@
 def test_validate_assignment():
     class MyModel:
         # this is not required, but it avoids `__pydantic_fields_set__` being included in `__dict__`
         __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__', '__pydantic_private__'
         field_a: str
         field_b: int
 
+        def __init__(self):
+            self.__pydantic_extra__ = None
+
     v = SchemaValidator(
         {
             'type': 'model',
             'cls': MyModel,
             'schema': {
                 'type': 'model-fields',
                 'fields': {
@@ -1015,15 +1018,18 @@
         "ValidationInfo(config=None, context=None, data={'field_a': 'x'}, field_name='field_b')",
         "ValidationInfo(config=None, context=None, data={'field_a': 'x', 'field_c': 456}, field_name='field_b')",
     ]
 
 
 def test_validate_assignment_no_fields_set():
     class MyModel:
-        __slots__ = ('__dict__',)
+        __slots__ = ('__dict__', '__pydantic_extra__')
+
+        def __init__(self):
+            self.__pydantic_extra__ = None
 
     v = SchemaValidator(
         {
             'type': 'model',
             'cls': MyModel,
             'schema': {
                 'type': 'model-fields',
```

### Comparing `pydantic_core-2.2.0/tests/validators/test_model_fields.py` & `pydantic_core-2.3.0/tests/validators/test_model_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,16 +343,16 @@
             'extra_behavior': 'allow',
         }
     )
 
     assert v.validate_python({'field_a': 'test'}) == ({'field_a': 'test'}, {}, {'field_a'})
 
     assert v.validate_assignment({'field_a': 'test'}, 'other_field', 456) == (
-        {'field_a': 'test', 'other_field': 456},
-        None,
+        {'field_a': 'test'},
+        {'other_field': 456},
         {'other_field'},
     )
 
 
 def test_validate_assignment_allow_extra_validate():
     v = SchemaValidator(
         {
@@ -360,16 +360,16 @@
             'fields': {'field_a': {'type': 'model-field', 'schema': {'type': 'str'}}},
             'extra_validator': {'type': 'int'},
             'extra_behavior': 'allow',
         }
     )
 
     assert v.validate_assignment({'field_a': 'test'}, 'other_field', '456') == (
-        {'field_a': 'test', 'other_field': 456},
-        None,
+        {'field_a': 'test'},
+        {'other_field': 456},
         {'other_field'},
     )
 
     with pytest.raises(ValidationError) as exc_info:
         assert v.validate_assignment({'field_a': 'test'}, 'other_field', 'xyz')
     assert exc_info.value.errors(include_url=False) == [
         {
@@ -1678,18 +1678,20 @@
 
     m, model_extra, fields_set = v.validate_python({'f': 'x', 'extra_field': '123'})
     assert m == {'f': 'x'}
     assert model_extra == {'extra_field': expected_extra_value}
     assert fields_set == {'f', 'extra_field'}
 
     v.validate_assignment(m, 'f', 'y')
-    assert m['f'] == 'y'
+    assert m == {'f': 'y'}
 
-    v.validate_assignment(m, 'not_f', '123')
-    assert m['not_f'] == expected_extra_value
+    new_m, new_model_extra, new_fields_set = v.validate_assignment({**m, **model_extra}, 'not_f', '123')
+    assert new_m == {'f': 'y'}
+    assert new_model_extra == {'extra_field': expected_extra_value, 'not_f': expected_extra_value}
+    assert new_fields_set == {'not_f'}
 
 
 @pytest.mark.parametrize(
     'config,schema_extra_behavior_kw',
     [
         (core_schema.CoreConfig(extra_fields_behavior='forbid'), {}),
         (core_schema.CoreConfig(extra_fields_behavior='forbid'), {'extra_behavior': None}),
```

### Comparing `pydantic_core-2.2.0/tests/validators/test_model_init.py` & `pydantic_core-2.3.0/tests/validators/test_model_init.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_model_root.py` & `pydantic_core-2.3.0/tests/validators/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_none.py` & `pydantic_core-2.3.0/tests/validators/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_nullable.py` & `pydantic_core-2.3.0/tests/validators/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_set.py` & `pydantic_core-2.3.0/tests/validators/test_set.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_string.py` & `pydantic_core-2.3.0/tests/validators/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_tagged_union.py` & `pydantic_core-2.3.0/tests/validators/test_tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_time.py` & `pydantic_core-2.3.0/tests/validators/test_time.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
         pytest.param(time(12, 13, 14, tzinfo=timezone.utc), time(12, 13, 14, tzinfo=timezone.utc), id='time-tz'),
         pytest.param('12:13:14', time(12, 13, 14), id='str'),
         pytest.param('12:13:14Z', time(12, 13, 14, tzinfo=timezone.utc), id='str-tz'),
         pytest.param(b'12:13:14', time(12, 13, 14), id='bytes'),
         pytest.param((1,), Err('Input should be a valid time [type=time_type'), id='tuple'),
         pytest.param(date(2022, 6, 8), Err('Input should be a valid time [type=time_type'), id='date'),
         pytest.param(datetime(2022, 6, 8), Err('Input should be a valid time [type=time_type'), id='datetime'),
-        pytest.param(123, time(0, 2, 3), id='int'),
+        pytest.param(123, time(0, 2, 3, tzinfo=timezone.utc), id='int'),
         pytest.param(float('nan'), Err('valid time format, NaN values not permitted [type=time_parsing,'), id='nan'),
         pytest.param(float('inf'), Err('valid time format, numeric times may not exceed 86,399 seconds'), id='inf'),
         pytest.param(float('-inf'), Err('valid time format, time in seconds should be positive'), id='-inf'),
-        pytest.param(Decimal('123'), time(0, 2, 3), id='decimal'),
-        pytest.param(Decimal('123.123456'), time(0, 2, 3, 123456), id='decimal-6dig'),
-        pytest.param(Decimal('123.1234562'), time(0, 2, 3, 123456), id='decimal-7dig-up'),
-        pytest.param(Decimal('123.1234568'), time(0, 2, 3, 123457), id='decimal-7dig-down'),
+        pytest.param(Decimal('123'), time(0, 2, 3, tzinfo=timezone.utc), id='decimal'),
+        pytest.param(Decimal('123.123456'), time(0, 2, 3, 123456, tzinfo=timezone.utc), id='decimal-6dig'),
+        pytest.param(Decimal('123.1234562'), time(0, 2, 3, 123456, tzinfo=timezone.utc), id='decimal-7dig-up'),
+        pytest.param(Decimal('123.1234568'), time(0, 2, 3, 123457, tzinfo=timezone.utc), id='decimal-7dig-down'),
     ],
 )
 def test_time(input_value, expected):
     v = SchemaValidator({'type': 'time'})
     if isinstance(expected, Err):
         with pytest.raises(ValidationError, match=re.escape(expected.message)):
             v.validate_python(input_value)
@@ -45,26 +45,19 @@
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         pytest.param('12:13:14', time(12, 13, 14), id='str'),
         pytest.param('12:13:14.123', time(12, 13, 14, 123_000), id='str-micro'),
         pytest.param('12:13:14.123456', time(12, 13, 14, 123_456), id='str-micro-6dig'),
         pytest.param('12:13:14.123456', time(12, 13, 14, 123_456), id='str-micro-6dig'),
-        pytest.param(
-            '12:13:14.1234561',
-            Err(
-                'Input should be in a valid time format, '
-                'second fraction value is more than 6 digits long [type=time_parsing'
-            ),
-            id='str-micro-7dig',
-        ),
-        pytest.param(123, time(0, 2, 3), id='int'),
-        pytest.param(123.4, time(0, 2, 3, 400_000), id='float'),
-        pytest.param(123.0, time(0, 2, 3), id='float.0'),
-        pytest.param(0, time(0), id='int-zero'),
+        pytest.param('12:13:14.1234561', time(12, 13, 14, 123_456), id='str-micro-7dig'),
+        pytest.param(123, time(0, 2, 3, tzinfo=timezone.utc), id='int'),
+        pytest.param(123.4, time(0, 2, 3, 400_000, tzinfo=timezone.utc), id='float'),
+        pytest.param(123.0, time(0, 2, 3, tzinfo=timezone.utc), id='float.0'),
+        pytest.param(0, time(0, tzinfo=timezone.utc), id='int-zero'),
         pytest.param(
             86400,
             Err(
                 'Input should be in a valid time format, numeric times may not exceed 86,399 seconds [type=time_parsing'
             ),
             id='too-high',
         ),
@@ -83,14 +76,35 @@
         with pytest.raises(ValidationError, match=re.escape(expected.message)):
             v.validate_test(input_value)
     else:
         output = v.validate_test(input_value)
         assert output == expected
 
 
+def test_time_error_microseconds_overflow(py_and_json: PyAndJson) -> None:
+    v = py_and_json(core_schema.time_schema(microseconds_precision='error'))
+
+    with pytest.raises(ValidationError) as exc_info:
+        v.validate_test('00:00:00.1234567')
+
+    # insert_assert(exc_info.value.errors(include_url=False))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'time_parsing',
+            'loc': (),
+            'msg': 'Input should be in a valid time format, second fraction value is more than 6 digits long',
+            'input': '00:00:00.1234567',
+            'ctx': {'error': 'second fraction value is more than 6 digits long'},
+        }
+    ]
+
+    # insert_assert(v.validate_test('00:00:00.123456'))
+    assert v.validate_test('00:00:00.123456') == time(0, 0, 0, 123456)
+
+
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         (time(12, 13, 14, 15), time(12, 13, 14, 15)),
         ('12:13:14', Err('Input should be a valid time [type=time_type')),
         (b'12:13:14', Err('Input should be a valid time [type=time_type')),
         (1654646400, Err('Input should be a valid time [type=time_type')),
```

### Comparing `pydantic_core-2.2.0/tests/validators/test_timedelta.py` & `pydantic_core-2.3.0/tests/validators/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_tuple.py` & `pydantic_core-2.3.0/tests/validators/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_typed_dict.py` & `pydantic_core-2.3.0/tests/validators/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_union.py` & `pydantic_core-2.3.0/tests/validators/test_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_url.py` & `pydantic_core-2.3.0/tests/validators/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/tests/validators/test_with_default.py` & `pydantic_core-2.3.0/tests/validators/test_with_default.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/Cargo.lock` & `pydantic_core-2.3.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -51,49 +51,55 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.11"
+version = "0.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f36e95862220b211a6e2aa5eca09b4fa391b13cd52ceb8035a24bf65a79de2"
+checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.25",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -104,56 +110,66 @@
 checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
 dependencies = [
- "autocfg",
+ "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.30"
+version = "0.1.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8c7cbf8b89019683667e347572e6d55a7df7ea36b0c4ce69961b0cde67b174"
+checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memchr"
@@ -168,17 +184,17 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.34"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcb174b18635f7561a0c6c9fc2ce57218ac7523cf72c50af80e2d79ab8f3ba1"
+checksum = "4e2894987a3459f3ffb755608bd82188f8ed00d0ae077f1edea29c068d639d98"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.3"
@@ -207,64 +223,64 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pydantic-core"
-version = "2.2.0"
+version = "2.3.0"
 dependencies = [
  "ahash",
  "base64",
  "enum_dispatch",
- "idna",
+ "idna 0.3.0",
  "mimalloc",
  "num-bigint",
  "pyo3",
  "pyo3-build-config",
  "python3-dll-a",
  "regex",
  "serde",
@@ -345,120 +361,132 @@
 checksum = "d5f07cd4412be8fa09a721d40007c483981bbe072cd6a21f2e83e04ec8f8343f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "speedate"
-version = "0.9.1"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb4daf811c41c4deda029974aac9583eab5cb4e1b6aef14c3cc23539e310faf6"
+checksum = "e54e4ea42510cf6cb46223f6974670faf58ef49e82040e924a295aa3f0c8eaa2"
 dependencies = [
  "strum",
- "strum_macros 0.25.0",
+ "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "strum"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
 dependencies = [
- "strum_macros 0.25.0",
+ "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
@@ -468,23 +496,23 @@
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "strum_macros"
-version = "0.25.0"
+version = "0.25.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe9f3bd7d2e45dcc5e265fbb88d6513e4747d8ef9444cf01a533119bce28a157"
+checksum = "6069ca09d878a33f883cc06aaa9718ede171841d3832450354410b718b097232"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -492,28 +520,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
@@ -530,17 +558,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -551,20 +579,20 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
- "idna",
+ "idna 0.4.0",
  "percent-encoding",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -573,71 +601,62 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `pydantic_core-2.2.0/python/pydantic_core/_pydantic_core.pyi` & `pydantic_core-2.3.0/python/pydantic_core/_pydantic_core.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import datetime
 import decimal
 import sys
 from typing import Any, Callable, Generic, Optional, Type, TypeVar
 
 from pydantic_core import ErrorDetails, ErrorTypeInfo, InitErrorDetails, MultiHostHost
 from pydantic_core.core_schema import CoreConfig, CoreSchema, ErrorType
 
@@ -39,14 +40,15 @@
     'PydanticSerializationUnexpectedValue',
     'PydanticUndefined',
     'PydanticUndefinedType',
     'Some',
     'to_json',
     'to_jsonable_python',
     'list_all_errors',
+    'TzInfo',
 ]
 __version__: str
 build_profile: str
 build_info: str
 _recursion_limit: int
 
 _T = TypeVar('_T', default=Any, covariant=True)
@@ -67,44 +69,47 @@
     def title(self) -> str: ...
     def validate_python(
         self,
         input: Any,
         *,
         strict: bool | None = None,
         from_attributes: bool | None = None,
-        context: Any = None,
+        context: 'dict[str, Any] | None' = None,
         self_instance: Any | None = None,
     ) -> Any: ...
     def isinstance_python(
         self,
         input: Any,
         *,
         strict: bool | None = None,
         from_attributes: bool | None = None,
-        context: Any = None,
+        context: 'dict[str, Any] | None' = None,
         self_instance: Any | None = None,
     ) -> bool: ...
     def validate_json(
         self,
         input: str | bytes | bytearray,
         *,
         strict: bool | None = None,
-        context: Any = None,
+        context: 'dict[str, Any] | None' = None,
         self_instance: Any | None = None,
     ) -> Any: ...
     def validate_assignment(
         self,
         obj: Any,
         field_name: str,
         field_value: Any,
         *,
         strict: bool | None = None,
         from_attributes: bool | None = None,
-        context: Any = None,
-    ) -> dict[str, Any]: ...
+        context: 'dict[str, Any] | None' = None,
+    ) -> dict[str, Any] | tuple[dict[str, Any], dict[str, Any] | None, set[str]]:
+        """
+        ModelValidator and ModelFieldsValidator will return a tuple of (fields data, extra data, fields set)
+        """
     def get_default_value(self, *, strict: bool | None = None, context: Any = None) -> Some | None: ...
 
 _IncEx: TypeAlias = set[int] | set[str] | dict[int, _IncEx] | dict[str, _IncEx] | None
 
 @final
 class SchemaSerializer:
     def __new__(cls, schema: CoreSchema, config: CoreConfig | None = None) -> Self: ...
@@ -319,7 +324,14 @@
 
 PydanticUndefined: PydanticUndefinedType
 
 def list_all_errors() -> list[ErrorTypeInfo]:
     """
     Get information about all built-in errors.
     """
+
+@final
+class TzInfo(datetime.tzinfo):
+    def tzname(self, _dt: datetime.datetime | None) -> str | None: ...
+    def utcoffset(self, _dt: datetime.datetime | None) -> datetime.timedelta: ...
+    def dst(self, _dt: datetime.datetime | None) -> datetime.timedelta: ...
+    def __deepcopy__(self, _memo: dict[Any, Any]) -> 'TzInfo': ...
```

### Comparing `pydantic_core-2.2.0/python/pydantic_core/core_schema.py` & `pydantic_core-2.3.0/python/pydantic_core/core_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,27 +844,29 @@
     type: Required[Literal['time']]
     strict: bool
     le: time
     ge: time
     lt: time
     gt: time
     tz_constraint: Union[Literal['aware', 'naive'], int]
+    microseconds_precision: Literal['truncate', 'error']
     ref: str
     metadata: Any
     serialization: SerSchema
 
 
 def time_schema(
     *,
     strict: bool | None = None,
     le: time | None = None,
     ge: time | None = None,
     lt: time | None = None,
     gt: time | None = None,
     tz_constraint: Literal['aware', 'naive'] | int | None = None,
+    microseconds_precision: Literal['truncate', 'error'] = 'truncate',
     ref: str | None = None,
     metadata: Any = None,
     serialization: SerSchema | None = None,
 ) -> TimeSchema:
     """
     Returns a schema that matches a time value, e.g.:
 
@@ -880,26 +882,28 @@
     Args:
         strict: Whether the value should be a time or a value that can be converted to a time
         le: The value must be less than or equal to this time
         ge: The value must be greater than or equal to this time
         lt: The value must be strictly less than this time
         gt: The value must be strictly greater than this time
         tz_constraint: The value must be timezone aware or naive, or an int to indicate required tz offset
+        microseconds_precision: The behavior when seconds have more than 6 digits or microseconds is too large
         ref: optional unique identifier of the schema, used to reference the schema in other places
         metadata: Any other information you want to include with the schema, not used by pydantic-core
         serialization: Custom serialization schema
     """
     return _dict_not_none(
         type='time',
         strict=strict,
         le=le,
         ge=ge,
         lt=lt,
         gt=gt,
         tz_constraint=tz_constraint,
+        microseconds_precision=microseconds_precision,
         ref=ref,
         metadata=metadata,
         serialization=serialization,
     )
 
 
 class DatetimeSchema(TypedDict, total=False):
@@ -910,14 +914,15 @@
     lt: datetime
     gt: datetime
     now_op: Literal['past', 'future']
     tz_constraint: Union[Literal['aware', 'naive'], int]
     # defaults to current local utc offset from `time.localtime().tm_gmtoff`
     # value is restricted to -86_400 < offset < 86_400 by bounds in generate_self_schema.py
     now_utc_offset: int
+    microseconds_precision: Literal['truncate', 'error'] = ('truncate',)
     ref: str
     metadata: Any
     serialization: SerSchema
 
 
 def datetime_schema(
     *,
@@ -925,14 +930,15 @@
     le: datetime | None = None,
     ge: datetime | None = None,
     lt: datetime | None = None,
     gt: datetime | None = None,
     now_op: Literal['past', 'future'] | None = None,
     tz_constraint: Literal['aware', 'naive'] | int | None = None,
     now_utc_offset: int | None = None,
+    microseconds_precision: Literal['truncate', 'error'] = 'truncate',
     ref: str | None = None,
     metadata: Any = None,
     serialization: SerSchema | None = None,
 ) -> DatetimeSchema:
     """
     Returns a schema that matches a datetime value, e.g.:
 
@@ -952,53 +958,57 @@
         ge: The value must be greater than or equal to this datetime
         lt: The value must be strictly less than this datetime
         gt: The value must be strictly greater than this datetime
         now_op: The value must be in the past or future relative to the current datetime
         tz_constraint: The value must be timezone aware or naive, or an int to indicate required tz offset
             TODO: use of a tzinfo where offset changes based on the datetime is not yet supported
         now_utc_offset: The value must be in the past or future relative to the current datetime with this utc offset
+        microseconds_precision: The behavior when seconds have more than 6 digits or microseconds is too large
         ref: optional unique identifier of the schema, used to reference the schema in other places
         metadata: Any other information you want to include with the schema, not used by pydantic-core
         serialization: Custom serialization schema
     """
     return _dict_not_none(
         type='datetime',
         strict=strict,
         le=le,
         ge=ge,
         lt=lt,
         gt=gt,
         now_op=now_op,
         tz_constraint=tz_constraint,
         now_utc_offset=now_utc_offset,
+        microseconds_precision=microseconds_precision,
         ref=ref,
         metadata=metadata,
         serialization=serialization,
     )
 
 
 class TimedeltaSchema(TypedDict, total=False):
     type: Required[Literal['timedelta']]
     strict: bool
     le: timedelta
     ge: timedelta
     lt: timedelta
     gt: timedelta
+    microseconds_precision: Literal['truncate', 'error']
     ref: str
     metadata: Any
     serialization: SerSchema
 
 
 def timedelta_schema(
     *,
     strict: bool | None = None,
     le: timedelta | None = None,
     ge: timedelta | None = None,
     lt: timedelta | None = None,
     gt: timedelta | None = None,
+    microseconds_precision: Literal['truncate', 'error'] = 'truncate',
     ref: str | None = None,
     metadata: Any = None,
     serialization: SerSchema | None = None,
 ) -> TimedeltaSchema:
     """
     Returns a schema that matches a timedelta value, e.g.:
 
@@ -1013,25 +1023,27 @@
 
     Args:
         strict: Whether the value should be a timedelta or a value that can be converted to a timedelta
         le: The value must be less than or equal to this timedelta
         ge: The value must be greater than or equal to this timedelta
         lt: The value must be strictly less than this timedelta
         gt: The value must be strictly greater than this timedelta
+        microseconds_precision: The behavior when seconds have more than 6 digits or microseconds is too large
         ref: optional unique identifier of the schema, used to reference the schema in other places
         metadata: Any other information you want to include with the schema, not used by pydantic-core
         serialization: Custom serialization schema
     """
     return _dict_not_none(
         type='timedelta',
         strict=strict,
         le=le,
         ge=ge,
         lt=lt,
         gt=gt,
+        microseconds_precision=microseconds_precision,
         ref=ref,
         metadata=metadata,
         serialization=serialization,
     )
 
 
 class LiteralSchema(TypedDict, total=False):
```

### Comparing `pydantic_core-2.2.0/python/pydantic_core/__init__.py` & `pydantic_core-2.3.0/python/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.2.0/PKG-INFO` & `pydantic_core-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_core
-Version: 2.2.0
+Version: 2.3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

