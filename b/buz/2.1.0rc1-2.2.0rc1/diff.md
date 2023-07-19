# Comparing `tmp/buz-2.1.0rc1.tar.gz` & `tmp/buz-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buz-2.1.0rc1.tar", max compression
+gzip compressed data, was "buz-2.2.0rc1.tar", max compression
```

## Comparing `buz-2.1.0rc1.tar` & `buz-2.2.0rc1.tar`

### file list

```diff
@@ -1,129 +1,128 @@
--rw-r--r--   0        0        0     1062 2023-06-06 15:02:30.658161 buz-2.1.0rc1/LICENSE
--rw-r--r--   0        0        0      104 2023-06-06 15:02:30.658161 buz-2.1.0rc1/README.md
--rw-r--r--   0        0        0     1325 2023-06-06 15:02:30.658161 buz-2.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/__init__.py
--rw-r--r--   0        0        0      223 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/__init__.py
--rw-r--r--   0        0        0      271 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/__init__.py
--rw-r--r--   0        0        0      709 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/base_command_handler.py
--rw-r--r--   0        0        0      181 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/command_bus.py
--rw-r--r--   0        0        0      330 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/command_handler.py
--rw-r--r--   0        0        0      409 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/middleware/__init__.py
--rw-r--r--   0        0        0      788 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      449 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1147 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      134 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py
--rw-r--r--   0        0        0      193 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/command.py
--rw-r--r--   0        0        0      554 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/more_than_one_command_handler_related_exception.py
--rw-r--r--   0        0        0      268 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/__init__.py
--rw-r--r--   0        0        0      708 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/base_command_handler.py
--rw-r--r--   0        0        0      175 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/command_bus.py
--rw-r--r--   0        0        0      316 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/command_handler.py
--rw-r--r--   0        0        0      406 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/middleware/__init__.py
--rw-r--r--   0        0        0      774 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      420 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1133 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      133 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1153 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py
--rw-r--r--   0        0        0      133 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/synced_async/__init__.py
--rw-r--r--   0        0        0      459 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/command/synchronous/synced_async/synced_async_command_bus.py
--rw-r--r--   0        0        0      256 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/__init__.py
--rw-r--r--   0        0        0      645 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/base_subscriber.py
--rw-r--r--   0        0        0      189 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/event.py
--rw-r--r--   0        0        0      293 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/event_bus.py
--rw-r--r--   0        0        0      656 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/__init__.py
--rw-r--r--   0        0        0      263 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
--rw-r--r--   0        0        0      179 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
--rw-r--r--   0        0        0      756 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
--rw-r--r--   0        0        0      215 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/event_not_published_exception.py
--rw-r--r--   0        0        0      302 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/event_restore_exception.py
--rw-r--r--   0        0        0      258 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
--rw-r--r--   0        0        0      192 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
--rw-r--r--   0        0        0      429 2023-06-06 15:02:30.658161 buz-2.1.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
--rw-r--r--   0        0        0     5529 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/kombu_consumer.py
--rw-r--r--   0        0        0     3251 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/kombu_event_bus.py
--rw-r--r--   0        0        0      285 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
--rw-r--r--   0        0        0      382 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
--rw-r--r--   0        0        0      309 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
--rw-r--r--   0        0        0      894 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/__init__.py
--rw-r--r--   0        0        0      361 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/consume_retrier.py
--rw-r--r--   0        0        0      229 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
--rw-r--r--   0        0        0      449 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
--rw-r--r--   0        0        0     1332 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
--rw-r--r--   0        0        0      230 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
--rw-r--r--   0        0        0      993 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
--rw-r--r--   0        0        0      241 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/reject_callback.py
--rw-r--r--   0        0        0     1236 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
--rw-r--r--   0        0        0       75 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/serializer_enum.py
--rw-r--r--   0        0        0      695 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
--rw-r--r--   0        0        0      742 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/kombu/worker.py
--rw-r--r--   0        0        0      773 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/__init__.py
--rw-r--r--   0        0        0      651 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/base_consume_middleware.py
--rw-r--r--   0        0        0      531 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/base_publish_middleware.py
--rw-r--r--   0        0        0      363 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/consume_middleware.py
--rw-r--r--   0        0        0     1021 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
--rw-r--r--   0        0        0      315 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/publish_middleware.py
--rw-r--r--   0        0        0      949 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
--rw-r--r--   0        0        0      303 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/subscriber.py
--rw-r--r--   0        0        0       91 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/sync/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/sync/sync_event_bus.py
--rw-r--r--   0        0        0     1209 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/__init__.py
--rw-r--r--   0        0        0      506 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
--rw-r--r--   0        0        0      779 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
--rw-r--r--   0        0        0      515 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
--rw-r--r--   0        0        0      860 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_record.py
--rw-r--r--   0        0        0      281 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
--rw-r--r--   0        0        0      708 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
--rw-r--r--   0        0        0      509 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
--rw-r--r--   0        0        0       89 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
--rw-r--r--   0        0        0      903 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
--rw-r--r--   0        0        0     2415 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
--rw-r--r--   0        0        0      272 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/handler.py
--rw-r--r--   0        0        0      293 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/__init__.py
--rw-r--r--   0        0        0      206 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/locator.py
--rw-r--r--   0        0        0      206 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/message_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/pypendency/__init__.py
--rw-r--r--   0        0        0     3517 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/pypendency/container_locator.py
--rw-r--r--   0        0        0      246 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/pypendency/handler_already_registered_exception.py
--rw-r--r--   0        0        0      240 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
--rw-r--r--   0        0        0      235 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
--rw-r--r--   0        0        0      370 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/sync/__init__.py
--rw-r--r--   0        0        0      245 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
--rw-r--r--   0        0        0      234 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
--rw-r--r--   0        0        0     2082 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/locator/sync/instance_locator.py
--rw-r--r--   0        0        0     1359 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/message.py
--rw-r--r--   0        0        0      176 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/middleware/__init__.py
--rw-r--r--   0        0        0       54 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/middleware/middleware.py
--rw-r--r--   0        0        0     1002 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/middleware/middleware_chain_builder.py
--rw-r--r--   0        0        0        0 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/py.typed
--rw-r--r--   0        0        0      274 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/__init__.py
--rw-r--r--   0        0        0      247 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/__init__.py
--rw-r--r--   0        0        0      675 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/base_query_handler.py
--rw-r--r--   0        0        0      404 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/middleware/__init__.py
--rw-r--r--   0        0        0      874 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      462 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1148 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      195 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/query_bus.py
--rw-r--r--   0        0        0      334 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/query_handler.py
--rw-r--r--   0        0        0      126 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1223 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py
--rw-r--r--   0        0        0      516 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/more_than_one_query_handler_related_exception.py
--rw-r--r--   0        0        0      189 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/query.py
--rw-r--r--   0        0        0      153 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/query_response.py
--rw-r--r--   0        0        0      244 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/__init__.py
--rw-r--r--   0        0        0      674 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/base_query_handler.py
--rw-r--r--   0        0        0      400 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/middleware/__init__.py
--rw-r--r--   0        0        0      846 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      433 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1095 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      189 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/query_bus.py
--rw-r--r--   0        0        0      328 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/query_handler.py
--rw-r--r--   0        0        0      125 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py
--rw-r--r--   0        0        0      125 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/synced_async/__init__.py
--rw-r--r--   0        0        0      470 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/query/synchronous/synced_async/synced_async_query_bus.py
--rw-r--r--   0        0        0       77 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/wrapper/__init__.py
--rw-r--r--   0        0        0      698 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/wrapper/async_to_sync.py
--rw-r--r--   0        0        0      266 2023-06-06 15:02:30.662162 buz-2.1.0rc1/src/buz/wrapper/event_loop.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 buz-2.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-19 09:32:56.853313 buz-2.2.0rc1/LICENSE
+-rw-r--r--   0        0        0      104 2023-07-19 09:32:56.853313 buz-2.2.0rc1/README.md
+-rw-r--r--   0        0        0     1325 2023-07-19 09:32:56.853313 buz-2.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/__init__.py
+-rw-r--r--   0        0        0      709 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/base_command_handler.py
+-rw-r--r--   0        0        0      181 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/command_bus.py
+-rw-r--r--   0        0        0      330 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/command_handler.py
+-rw-r--r--   0        0        0      409 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      788 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      449 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1147 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      134 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      193 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/command.py
+-rw-r--r--   0        0        0      554 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/more_than_one_command_handler_related_exception.py
+-rw-r--r--   0        0        0      268 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/base_command_handler.py
+-rw-r--r--   0        0        0      175 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/command_bus.py
+-rw-r--r--   0        0        0      316 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/command_handler.py
+-rw-r--r--   0        0        0      406 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      774 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      420 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1133 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      133 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1153 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      133 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      459 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/command/synchronous/synced_async/synced_async_command_bus.py
+-rw-r--r--   0        0        0      256 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/base_subscriber.py
+-rw-r--r--   0        0        0      189 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/event.py
+-rw-r--r--   0        0        0      293 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/event_bus.py
+-rw-r--r--   0        0        0      656 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/__init__.py
+-rw-r--r--   0        0        0      263 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
+-rw-r--r--   0        0        0      179 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
+-rw-r--r--   0        0        0      756 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
+-rw-r--r--   0        0        0      215 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/event_not_published_exception.py
+-rw-r--r--   0        0        0      302 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/event_restore_exception.py
+-rw-r--r--   0        0        0      258 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
+-rw-r--r--   0        0        0      429 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
+-rw-r--r--   0        0        0     5529 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/kombu_consumer.py
+-rw-r--r--   0        0        0     3251 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/kombu_event_bus.py
+-rw-r--r--   0        0        0      285 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
+-rw-r--r--   0        0        0      382 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
+-rw-r--r--   0        0        0      309 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
+-rw-r--r--   0        0        0      894 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/consume_retrier.py
+-rw-r--r--   0        0        0      229 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
+-rw-r--r--   0        0        0      449 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
+-rw-r--r--   0        0        0     1332 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
+-rw-r--r--   0        0        0      230 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
+-rw-r--r--   0        0        0      993 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
+-rw-r--r--   0        0        0      241 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/reject_callback.py
+-rw-r--r--   0        0        0     1236 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
+-rw-r--r--   0        0        0       75 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/serializer_enum.py
+-rw-r--r--   0        0        0      695 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
+-rw-r--r--   0        0        0      742 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/kombu/worker.py
+-rw-r--r--   0        0        0      773 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/__init__.py
+-rw-r--r--   0        0        0      651 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/base_consume_middleware.py
+-rw-r--r--   0        0        0      531 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/base_publish_middleware.py
+-rw-r--r--   0        0        0      363 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/consume_middleware.py
+-rw-r--r--   0        0        0     1021 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      315 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/publish_middleware.py
+-rw-r--r--   0        0        0      949 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      303 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/subscriber.py
+-rw-r--r--   0        0        0       91 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/sync/__init__.py
+-rw-r--r--   0        0        0     1413 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/sync/sync_event_bus.py
+-rw-r--r--   0        0        0     1209 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
+-rw-r--r--   0        0        0      779 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
+-rw-r--r--   0        0        0      515 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
+-rw-r--r--   0        0        0      860 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_record.py
+-rw-r--r--   0        0        0      281 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
+-rw-r--r--   0        0        0      708 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
+-rw-r--r--   0        0        0      509 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
+-rw-r--r--   0        0        0       89 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
+-rw-r--r--   0        0        0      903 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
+-rw-r--r--   0        0        0     2415 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
+-rw-r--r--   0        0        0      272 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/handler.py
+-rw-r--r--   0        0        0      293 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/__init__.py
+-rw-r--r--   0        0        0      206 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/locator.py
+-rw-r--r--   0        0        0      206 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/message_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      365 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/pypendency/__init__.py
+-rw-r--r--   0        0        0     3432 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/pypendency/container_locator.py
+-rw-r--r--   0        0        0      240 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
+-rw-r--r--   0        0        0      235 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
+-rw-r--r--   0        0        0      370 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/sync/__init__.py
+-rw-r--r--   0        0        0      245 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      234 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
+-rw-r--r--   0        0        0     2082 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/locator/sync/instance_locator.py
+-rw-r--r--   0        0        0     1359 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/message.py
+-rw-r--r--   0        0        0      176 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/middleware/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/middleware/middleware.py
+-rw-r--r--   0        0        0     1002 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/middleware/middleware_chain_builder.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/py.typed
+-rw-r--r--   0        0        0      274 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/query/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/query/asynchronous/__init__.py
+-rw-r--r--   0        0        0      675 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/query/asynchronous/base_query_handler.py
+-rw-r--r--   0        0        0      404 2023-07-19 09:32:56.853313 buz-2.2.0rc1/src/buz/query/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      874 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      462 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1148 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      195 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/query_bus.py
+-rw-r--r--   0        0        0      334 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/query_handler.py
+-rw-r--r--   0        0        0      126 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      516 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/more_than_one_query_handler_related_exception.py
+-rw-r--r--   0        0        0      189 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/query.py
+-rw-r--r--   0        0        0      153 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/query_response.py
+-rw-r--r--   0        0        0      244 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/base_query_handler.py
+-rw-r--r--   0        0        0      400 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      846 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      433 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1095 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      189 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/query_bus.py
+-rw-r--r--   0        0        0      328 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/query_handler.py
+-rw-r--r--   0        0        0      125 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      125 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      470 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/query/synchronous/synced_async/synced_async_query_bus.py
+-rw-r--r--   0        0        0       77 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/wrapper/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/wrapper/async_to_sync.py
+-rw-r--r--   0        0        0      266 2023-07-19 09:32:56.857313 buz-2.2.0rc1/src/buz/wrapper/event_loop.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 buz-2.2.0rc1/PKG-INFO
```

### Comparing `buz-2.1.0rc1/LICENSE` & `buz-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/pyproject.toml` & `buz-2.2.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "buz"
-version = "2.1.0rc1"
+version = "2.2.0rc1"
 description = "Buz is a set of light, simple and extensible implementations of event, command and query buses."
 readme = "README.md"
 authors = ["Luis Pintado Lozano <luis.pintado.lozano@gmail.com>"]
 maintainers = ["Fever - Platform Squad <platform@feverup.com>"]
 license = "MIT License"
 classifiers=[
     "Intended Audience :: Developers",
```

### Comparing `buz-2.1.0rc1/src/buz/command/asynchronous/base_command_handler.py` & `buz-2.2.0rc1/src/buz/command/asynchronous/base_command_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py` & `buz-2.2.0rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py` & `buz-2.2.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/more_than_one_command_handler_related_exception.py` & `buz-2.2.0rc1/src/buz/command/more_than_one_command_handler_related_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/synchronous/base_command_handler.py` & `buz-2.2.0rc1/src/buz/command/synchronous/base_command_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py` & `buz-2.2.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py` & `buz-2.2.0rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/base_subscriber.py` & `buz-2.2.0rc1/src/buz/event/base_subscriber.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/__init__.py` & `buz-2.2.0rc1/src/buz/event/kombu/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py` & `buz-2.2.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/kombu_consumer.py` & `buz-2.2.0rc1/src/buz/event/kombu/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/kombu_event_bus.py` & `buz-2.2.0rc1/src/buz/event/kombu/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/retry/__init__.py` & `buz-2.2.0rc1/src/buz/event/kombu/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py` & `buz-2.2.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py` & `buz-2.2.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py` & `buz-2.2.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py` & `buz-2.2.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/kombu/worker.py` & `buz-2.2.0rc1/src/buz/event/kombu/worker.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/middleware/__init__.py` & `buz-2.2.0rc1/src/buz/event/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/middleware/base_consume_middleware.py` & `buz-2.2.0rc1/src/buz/event/middleware/base_consume_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/middleware/base_publish_middleware.py` & `buz-2.2.0rc1/src/buz/event/middleware/base_publish_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/sync/sync_event_bus.py` & `buz-2.2.0rc1/src/buz/event/sync/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/__init__.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_record.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_record.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py` & `buz-2.2.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/locator/locator.py` & `buz-2.2.0rc1/src/buz/locator/locator.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/locator/pypendency/container_locator.py` & `buz-2.2.0rc1/src/buz/locator/pypendency/container_locator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
-from typing import List, DefaultDict, Generic, TypeVar, Type, cast
+from threading import Lock
+from typing import List, DefaultDict, Generic, TypeVar, Type, cast, Set
 
 from pypendency.container import AbstractContainer
 
 from buz import Handler
 from buz import Message
 from buz.locator import Locator, HandlerFqnNotFoundException, MessageFqnNotFoundException
-from buz.locator.pypendency import HandlerAlreadyRegisteredException
 from buz.locator.pypendency import HandlerNotFoundException
 from buz.locator.pypendency import HandlerNotRegisteredException
 
 K = TypeVar("K", bound=Message)
 V = TypeVar("V", bound=Handler)
 MessageFqn = str
 
@@ -19,28 +19,26 @@
     CHECK_MODE_REGISTER_TIME = "register"
     CHECK_MODE_GET_TIME = "get"
 
     def __init__(self, container: AbstractContainer, check_mode: str = CHECK_MODE_REGISTER_TIME) -> None:
         self.__container = container
         self.__check_mode = check_mode
         self.__mapping: DefaultDict[MessageFqn, List[V]] = defaultdict(list)
-        self.__handler_ids: List[str] = []
+        self.__handler_ids: Set[str] = set()
         self.__handlers_resolved = False
+        self.__lock = Lock()
 
     def register(self, handler_id: str) -> None:
-        self.__guard_handler_already_registered(handler_id)
+        if handler_id in self.__handler_ids:
+            return
         if self.__check_mode == self.CHECK_MODE_REGISTER_TIME:
             self.__guard_handler_not_found(handler_id)
-        self.__handler_ids.append(handler_id)
+        self.__handler_ids.add(handler_id)
         self.__handlers_resolved = False
 
-    def __guard_handler_already_registered(self, handler_id: str) -> None:
-        if handler_id in self.__handler_ids:
-            raise HandlerAlreadyRegisteredException(handler_id)
-
     def __guard_handler_not_found(self, handler_id: str) -> None:
         if not self.__container.has(handler_id):
             raise HandlerNotFoundException(handler_id)
 
     def unregister(self, handler_id: str) -> None:
         self.__guard_handler_not_registered(handler_id)
         self.__handler_ids.remove(handler_id)
@@ -51,18 +49,22 @@
             raise HandlerNotRegisteredException(handler_id)
 
     def get(self, message: K) -> List[V]:
         self.__ensure_handlers_resolved()
         return self.__mapping.get(message.fqn(), [])
 
     def __ensure_handlers_resolved(self) -> None:
-        if not self.__handlers_resolved:
-            self.__resolve_handlers()
+        self.__lock.acquire()
+        try:
+            if self.__handlers_resolved is False:
+                self._resolve_handlers()
+        finally:
+            self.__lock.release()
 
-    def __resolve_handlers(self) -> None:
+    def _resolve_handlers(self) -> None:
         self.__mapping = defaultdict(list)
         for handler_id in self.__handler_ids:
             if self.__check_mode == self.CHECK_MODE_GET_TIME:
                 self.__guard_handler_not_found(handler_id)
             handler: V = self.__container.get(handler_id)
             message_fqn = handler.handles().fqn()
             self.__mapping[message_fqn].append(handler)
```

### Comparing `buz-2.1.0rc1/src/buz/locator/sync/instance_locator.py` & `buz-2.2.0rc1/src/buz/locator/sync/instance_locator.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/message.py` & `buz-2.2.0rc1/src/buz/message.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/middleware/middleware_chain_builder.py` & `buz-2.2.0rc1/src/buz/middleware/middleware_chain_builder.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/asynchronous/base_query_handler.py` & `buz-2.2.0rc1/src/buz/query/asynchronous/base_query_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py` & `buz-2.2.0rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py` & `buz-2.2.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/more_than_one_query_handler_related_exception.py` & `buz-2.2.0rc1/src/buz/query/more_than_one_query_handler_related_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/synchronous/base_query_handler.py` & `buz-2.2.0rc1/src/buz/query/synchronous/base_query_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py` & `buz-2.2.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.2.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py` & `buz-2.2.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/src/buz/wrapper/async_to_sync.py` & `buz-2.2.0rc1/src/buz/wrapper/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `buz-2.1.0rc1/PKG-INFO` & `buz-2.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buz
-Version: 2.1.0rc1
+Version: 2.2.0rc1
 Summary: Buz is a set of light, simple and extensible implementations of event, command and query buses.
 License: MIT
 Author: Luis Pintado Lozano
 Author-email: luis.pintado.lozano@gmail.com
 Maintainer: Fever - Platform Squad
 Maintainer-email: platform@feverup.com
 Requires-Python: >=3.8.0,<4.0.0
```

