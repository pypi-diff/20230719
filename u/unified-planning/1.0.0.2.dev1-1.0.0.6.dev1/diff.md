# Comparing `tmp/unified_planning-1.0.0.2.dev1.tar.gz` & `tmp/unified_planning-1.0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-1.0.0.2.dev1.tar", last modified: Thu Jul 13 09:50:20 2023, max compression
+gzip compressed data, was "unified_planning-1.0.0.6.dev1.tar", last modified: Mon Jul 17 07:51:10 2023, max compression
```

## Comparing `unified_planning-1.0.0.2.dev1.tar` & `unified_planning-1.0.0.6.dev1.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.545091 unified_planning-1.0.0.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-13 09:50:20.545091 unified_planning-1.0.0.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:50:20.545091 unified_planning-1.0.0.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.501092 unified_planning-1.0.0.2.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.501092 unified_planning-1.0.0.2.dev1/unified_planning/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/cmd/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/cmd/up.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/state_invariants_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/pddl_anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35416 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.505092 unified_planning-1.0.0.2.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.509092 unified_planning-1.0.0.2.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    41471 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39290 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    77329 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40589 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.509092 unified_planning-1.0.0.2.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    28717 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.509092 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.509092 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.509092 unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/problem_kind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.513092 unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.513092 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.517092 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24752 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.521092 unified_planning-1.0.0.2.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plans/time_triggered_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.521092 unified_planning-1.0.0.2.dev1/unified_planning/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plot/causal_graph_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plot/plan_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30679 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.533092 unified_planning-1.0.0.2.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.533092 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.497092 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.533092 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.533092 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/realistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.501092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.537092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.541092 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.545091 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.545091 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    27054 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25431 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_state_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 09:50:18.000000 unified_planning-1.0.0.2.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:50:20.501092 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 09:50:20.000000 unified_planning-1.0.0.2.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/up.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48595 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35416 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41471 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39290 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40589 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28717 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24752 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/time_triggered_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.045088 unified_planning-1.0.0.6.dev1/unified_planning/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/causal_graph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/plan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30679 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.049088 unified_planning-1.0.0.6.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.021088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/realistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.021088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    27054 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25431 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-17 07:51:10.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-1.0.0.2.dev1/LICENSE` & `unified_planning-1.0.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/PKG-INFO` & `unified_planning-1.0.0.6.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 1.0.0.2.dev1
+Version: 1.0.0.6.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.0.0.2.dev1/README.md` & `unified_planning-1.0.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/setup.py` & `unified_planning-1.0.0.6.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     install_requires=["pyparsing", "networkx"],
     extras_require={
         "dev": ["tarski[arithmetic]", "pytest", "pytest-cov", "mypy"],
         "grpc": ["grpcio", "grpcio-tools", "grpc-stubs"],
         "tarski": ["tarski[arithmetic]"],
         "pyperplan": ["up-pyperplan==1.0.0"],
         "tamer": ["up-tamer==1.0.0"],
-        "enhsp": ["up-enhsp==0.0.15"],
+        "enhsp": ["up-enhsp==0.0.16"],
         "fast-downward": ["up-fast-downward==0.2.3"],
         "lpg": ["up-lpg==0.0.7"],
         "fmap": ["up-fmap==0.0.7"],
         "aries": ["up-aries>=0.0.8"],
         "symk": ["up-symk>=0.0.3"],
         "engines": [
             "tarski[arithmetic]",
             "up-pyperplan==1.0.0",
             "up-tamer==1.0.0",
-            "up-enhsp==0.0.15",
+            "up-enhsp==0.0.16",
             "up-fast-downward==0.2.3",
             "up-lpg==0.0.7",
             "up-fmap==0.0.7",
             "up-aries>=0.0.8",
             "up-symk>=0.0.3",
         ],
         "plot": ["plotly", "matplotlib", "kaleido", "pygraphviz", "pandas"],
```

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/cmd/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/cmd/arg_parser.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/arg_parser.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/cmd/up.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/up.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/state_invariants_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/state_invariants_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/credits.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/engine.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/factory.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 DEFAULT_ENGINES = {
     "fast-downward": ("up_fast_downward", "FastDownwardPDDLPlanner"),
     "fast-downward-opt": ("up_fast_downward", "FastDownwardOptimalPDDLPlanner"),
     "symk": ("up_symk", "SymKPDDLPlanner"),
     "symk-opt": ("up_symk", "SymKOptimalPDDLPlanner"),
     "pyperplan": ("up_pyperplan.engine", "EngineImpl"),
     "pyperplan-opt": ("up_pyperplan.engine", "OptEngineImpl"),
-    "enhsp": ("up_enhsp.enhsp_planner", "ENHSPSatEngine"),
+    "enhsp": ("up_enhsp.enhsp_planner", "ENHSPEngine"),
     "enhsp-opt": ("up_enhsp.enhsp_planner", "ENHSPOptEngine"),
     "enhsp-any": ("up_enhsp.enhsp_planner", "ENHSPAnytimeEngine"),
     "tamer": ("up_tamer.engine", "EngineImpl"),
     "lpg": ("up_lpg.lpg_planner", "LPGEngine"),
     "lpg-anytime": ("up_lpg.lpg_planner", "LPGAnytimeEngine"),
     "lpg-repairer": ("up_lpg.lpg_planner", "LPGPlanRepairer"),
     "fmap": ("up_fmap.fmap_planner", "FMAPsolver"),
```

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/parallel.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/pddl_anytime_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/results.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/results.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/environment.py` & `unified_planning-1.0.0.6.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/exceptions.py` & `unified_planning-1.0.0.6.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/converter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/interop/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_grammar.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/anml_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/anml_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/io/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/action.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/delta_stn.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/effect.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/effect.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/expression.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/fluent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/fluent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/fnode.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/method.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/task.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/time_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/object.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/operators.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/parameter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/problem_kind.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/problem_kind.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/state.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/action.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/objects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/path.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/path.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/tamp/types.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/timing.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/type_manager.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/types.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/variable.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/variable.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/any.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/free_vars.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/generic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/contingent_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/schedule.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/schedule.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/sequential_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plot/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plot/causal_graph_plot.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/causal_graph_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plot/plan_plot.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/plan_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/plot/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/shortcuts.py` & `unified_planning-1.0.0.6.dev1/unified_planning/shortcuts.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/minimals.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/realistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/examples.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/scheduling/jobshop.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_anytime.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_credits.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_dnf.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_factory.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_htn.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_htn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_infix_notation.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_ma_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_model.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_state_invariants.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_state_invariants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_tamp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_temporal.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/test/test_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 1.0.0.2.dev1
+Version: 1.0.0.6.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.2.dev1/unified_planning.egg-info/requires.txt` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 pytest-cov
 mypy
 
 [engines]
 tarski[arithmetic]
 up-pyperplan==1.0.0
 up-tamer==1.0.0
-up-enhsp==0.0.15
+up-enhsp==0.0.16
 up-fast-downward==0.2.3
 up-lpg==0.0.7
 up-fmap==0.0.7
 up-aries>=0.0.8
 up-symk>=0.0.3
 
 [enhsp]
-up-enhsp==0.0.15
+up-enhsp==0.0.16
 
 [fast-downward]
 up-fast-downward==0.2.3
 
 [fmap]
 up-fmap==0.0.7
```

