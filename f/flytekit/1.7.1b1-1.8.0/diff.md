# Comparing `tmp/flytekit-1.7.1b1.tar.gz` & `tmp/flytekit-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.7.1b1.tar", last modified: Tue Jun 27 22:00:44 2023, max compression
+gzip compressed data, was "flytekit-1.8.0.tar", last modified: Tue Jul 11 22:07:06 2023, max compression
```

## Comparing `flytekit-1.7.1b1.tar` & `flytekit-1.8.0.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 22:00:42.000000 flytekit-1.7.1b1/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/iterator/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/iterator/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 22:00:42.000000 flytekit-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 22:06:52.000000 flytekit-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-11 22:06:52.000000 flytekit-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-11 22:07:06.787602 flytekit-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-11 22:06:52.000000 flytekit-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.755602 flytekit-1.8.0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-11 22:07:04.000000 flytekit-1.8.0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.763602 flytekit-1.8.0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.763602 flytekit-1.8.0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.779602 flytekit-1.8.0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.779602 flytekit-1.8.0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87410 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/iterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/iterator/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-11 22:06:52.000000 flytekit-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 22:07:06.791602 flytekit-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-11 22:07:04.000000 flytekit-1.8.0/setup.py
```

### Comparing `flytekit-1.7.1b1/LICENSE` & `flytekit-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/MANIFEST.in` & `flytekit-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/PKG-INFO` & `flytekit-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.8.0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.1b1/README.md` & `flytekit-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/__init__.py` & `flytekit-1.8.0/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.7.1b1/flytekit/bin/entrypoint.py` & `flytekit-1.8.0/flytekit/bin/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     for k, v in output_file_dict.items():
         utils.write_proto_to_file(v.to_flyte_idl(), os.path.join(ctx.execution_state.engine_dir, k))
 
     ctx.file_access.put_data(ctx.execution_state.engine_dir, output_prefix, is_multipart=True)
     logger.info(f"Engine folder written successfully to the output prefix {output_prefix}")
 
-    if not task_def.disable_deck:
+    if not getattr(task_def, "disable_deck", True):
         _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
 
     logger.debug("Finished _dispatch_execute")
 
     if os.environ.get("FLYTE_FAIL_ON_ERROR", "").lower() == "true" and _constants.ERROR_FILE_NAME in output_file_dict:
         # This env is set by the flytepropeller
         # AWS batch job get the status from the exit code, so once we catch the error,
```

### Comparing `flytekit-1.7.1b1/flytekit/clients/auth/auth_client.py` & `flytekit-1.8.0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/auth/authenticator.py` & `flytekit-1.8.0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/auth/keyring.py` & `flytekit-1.8.0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/auth/token_client.py` & `flytekit-1.8.0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/auth_helper.py` & `flytekit-1.8.0/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/friendly.py` & `flytekit-1.8.0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.8.0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.8.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/helpers.py` & `flytekit-1.8.0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clients/raw.py` & `flytekit-1.8.0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/flyte_cli/main.py` & `flytekit-1.8.0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/helpers.py` & `flytekit-1.8.0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -815,19 +815,18 @@
     def get_command(self, ctx, filename):
         if ctx.obj:
             ctx.obj[RUN_LEVEL_PARAMS_KEY] = ctx.params
         return WorkflowCommand(filename, name=filename, help="Run a [workflow|task] in a file using script mode")
 
 
 _run_help = """
-This command can execute either a workflow or a task from the command line, for fully self-contained scripts.
-Tasks and workflows cannot be imported from other files currently. Please use ``pyflyte package`` or
-``pyflyte register`` to handle those and then launch from the Flyte UI or ``flytectl``.
+This command can execute either a workflow or a task from the command line, allowing for fully self-contained scripts.
+Tasks and workflows can be imported from other files.
 
-Note: This command only works on regular Python packages, not namespace packages. When determining
-the root of your project, it finds the first folder that does not have an ``__init__.py`` file.
+Note: This command is compatible with regular Python packages, but not with namespace packages.
+When determining the root of your project, it identifies the first folder without an ``__init__.py`` file.
 """
 
 run = RunCommand(
     name="run",
     help=_run_help,
 )
```

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.8.0/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/configuration/__init__.py` & `flytekit-1.8.0/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/configuration/default_images.py` & `flytekit-1.8.0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/configuration/feature_flags.py` & `flytekit-1.8.0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/configuration/file.py` & `flytekit-1.8.0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/configuration/internal.py` & `flytekit-1.8.0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/annotation.py` & `flytekit-1.8.0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/base_sql_task.py` & `flytekit-1.8.0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/base_task.py` & `flytekit-1.8.0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/checkpointer.py` & `flytekit-1.8.0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/class_based_resolver.py` & `flytekit-1.8.0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/condition.py` & `flytekit-1.8.0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/constants.py` & `flytekit-1.8.0/flytekit/core/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 INPUT_FILE_NAME = "inputs.pb"
 OUTPUT_FILE_NAME = "outputs.pb"
 FUTURES_FILE_NAME = "futures.pb"
 ERROR_FILE_NAME = "error.pb"
+REQUIREMENTS_FILE_NAME = "requirements.txt"
 
 
 class SdkTaskType(object):
     PYTHON_TASK = "python-task"
     DYNAMIC_TASK = "dynamic-task"
     CONTAINER_ARRAY_TASK = "container_array"
     SPARK_TASK = "spark"
```

### Comparing `flytekit-1.7.1b1/flytekit/core/container_task.py` & `flytekit-1.8.0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/context_manager.py` & `flytekit-1.8.0/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/data_persistence.py` & `flytekit-1.8.0/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/docstring.py` & `flytekit-1.8.0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.8.0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/gate.py` & `flytekit-1.8.0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/interface.py` & `flytekit-1.8.0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/launch_plan.py` & `flytekit-1.8.0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/local_cache.py` & `flytekit-1.8.0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/map_task.py` & `flytekit-1.8.0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/mock_stats.py` & `flytekit-1.8.0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/node.py` & `flytekit-1.8.0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/node_creation.py` & `flytekit-1.8.0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/notification.py` & `flytekit-1.8.0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/pod_template.py` & `flytekit-1.8.0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/promise.py` & `flytekit-1.8.0/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/python_auto_container.py` & `flytekit-1.8.0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/python_customized_container_task.py` & `flytekit-1.8.0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/python_function_task.py` & `flytekit-1.8.0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/reference.py` & `flytekit-1.8.0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/reference_entity.py` & `flytekit-1.8.0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/resources.py` & `flytekit-1.8.0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/schedule.py` & `flytekit-1.8.0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/shim_task.py` & `flytekit-1.8.0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/task.py` & `flytekit-1.8.0/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/testing.py` & `flytekit-1.8.0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/tracker.py` & `flytekit-1.8.0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/type_engine.py` & `flytekit-1.8.0/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/type_helpers.py` & `flytekit-1.8.0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/utils.py` & `flytekit-1.8.0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/core/workflow.py` & `flytekit-1.8.0/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/deck/deck.py` & `flytekit-1.8.0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/deck/html/template.html` & `flytekit-1.8.0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/deck/renderer.py` & `flytekit-1.8.0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/exceptions/scopes.py` & `flytekit-1.8.0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/exceptions/system.py` & `flytekit-1.8.0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/exceptions/user.py` & `flytekit-1.8.0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extend/__init__.py` & `flytekit-1.8.0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extend/backend/agent_service.py` & `flytekit-1.8.0/flytekit/extend/backend/agent_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extend/backend/base_agent.py` & `flytekit-1.8.0/flytekit/extend/backend/base_agent.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.8.0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/pytorch/__init__.py` & `flytekit-1.8.0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.8.0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/pytorch/native.py` & `flytekit-1.8.0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/sklearn/__init__.py` & `flytekit-1.8.0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/sklearn/native.py` & `flytekit-1.8.0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/sqlite3/task.py` & `flytekit-1.8.0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/tasks/shell.py` & `flytekit-1.8.0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.8.0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/tensorflow/model.py` & `flytekit-1.8.0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/extras/tensorflow/record.py` & `flytekit-1.8.0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/image_spec/image_spec.py` & `flytekit-1.8.0/flytekit/image_spec/image_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import hashlib
 import os
+import pathlib
 import typing
 from abc import abstractmethod
 from copy import copy
 from dataclasses import asdict, dataclass
 from functools import lru_cache
 from typing import List, Optional
 
@@ -24,35 +25,39 @@
         name: name of the image.
         python_version: python version of the image. Use default python in the base image if None.
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
+        requirements: path to the requirements.txt file.
         apt_packages: list of apt packages to install.
         cuda: version of cuda to install.
         cudnn: version of cudnn to install.
         base_image: base image of the image.
         platform: Specify the target platforms for the build output (for example, windows/amd64 or linux/amd64,darwin/arm64
         pip_index: Specify the custom pip index url
+        registry_config: Specify the path to a JSON registry config file
     """
 
     name: str = "flytekit"
     python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
+    requirements: Optional[str] = None
     apt_packages: Optional[List[str]] = None
     cuda: Optional[str] = None
     cudnn: Optional[str] = None
     base_image: Optional[str] = None
     platform: str = "linux/amd64"
     pip_index: Optional[str] = None
+    registry_config: Optional[str] = None
 
     def image_name(self) -> str:
         """
         return full image name with tag.
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
@@ -125,38 +130,45 @@
 
 class ImageBuildEngine:
     """
     ImageBuildEngine contains a list of builders that can be used to build an ImageSpec.
     """
 
     _REGISTRY: typing.Dict[str, ImageSpecBuilder] = {}
+    _BUILT_IMAGES: typing.Set[str] = set()
 
     @classmethod
     def register(cls, builder_type: str, image_spec_builder: ImageSpecBuilder):
         cls._REGISTRY[builder_type] = image_spec_builder
 
     @classmethod
     def build(cls, image_spec: ImageSpec):
         if image_spec.builder not in cls._REGISTRY:
             raise Exception(f"Builder {image_spec.builder} is not registered.")
-        if not image_spec.exist():
-            click.secho(f"Image {image_spec.image_name()} not found. Building...", fg="blue")
-            cls._REGISTRY[image_spec.builder].build_image(image_spec)
+        img_name = image_spec.image_name()
+        if img_name in cls._BUILT_IMAGES or image_spec.exist():
+            click.secho(f"Image {img_name} found. Skip building.", fg="blue")
         else:
-            click.secho(f"Image {image_spec.image_name()} found. Skip building.", fg="blue")
+            click.secho(f"Image {img_name} not found. Building...", fg="blue")
+            cls._REGISTRY[image_spec.builder].build_image(image_spec)
+            cls._BUILT_IMAGES.add(img_name)
 
 
 @lru_cache
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
     # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
     spec = copy(image_spec)
     spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
+    if spec.requirements:
+        spec.requirements = hashlib.sha1(pathlib.Path(spec.requirements).read_bytes()).hexdigest()
+    # won't rebuild the image if we change the registry_config path
+    spec.registry_config = None
     image_spec_bytes = asdict(spec).__str__().encode("utf-8")
     tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
     # replace "=" with "." and replace "-" with "_" to make it a valid tag
     return tag.replace("=", ".").replace("-", "_")
 
 
 def hash_directory(path):
```

### Comparing `flytekit-1.7.1b1/flytekit/interaction/parse_stdin.py` & `flytekit-1.8.0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.8.0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/interfaces/random.py` & `flytekit-1.8.0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/interfaces/stats/client.py` & `flytekit-1.8.0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/interfaces/stats/taggable.py` & `flytekit-1.8.0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/lazy_import/lazy_module.py` & `flytekit-1.8.0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/loggers.py` & `flytekit-1.8.0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/admin/common.py` & `flytekit-1.8.0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/admin/task_execution.py` & `flytekit-1.8.0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/admin/workflow.py` & `flytekit-1.8.0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/annotation.py` & `flytekit-1.8.0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/array_job.py` & `flytekit-1.8.0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/common.py` & `flytekit-1.8.0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/catalog.py` & `flytekit-1.8.0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/compiler.py` & `flytekit-1.8.0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/condition.py` & `flytekit-1.8.0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/errors.py` & `flytekit-1.8.0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/execution.py` & `flytekit-1.8.0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/identifier.py` & `flytekit-1.8.0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/types.py` & `flytekit-1.8.0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/core/workflow.py` & `flytekit-1.8.0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/documentation.py` & `flytekit-1.8.0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/dynamic_job.py` & `flytekit-1.8.0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/execution.py` & `flytekit-1.8.0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/filters.py` & `flytekit-1.8.0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/interface.py` & `flytekit-1.8.0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/launch_plan.py` & `flytekit-1.8.0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/literals.py` & `flytekit-1.8.0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/matchable_resource.py` & `flytekit-1.8.0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/named_entity.py` & `flytekit-1.8.0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/node_execution.py` & `flytekit-1.8.0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/presto.py` & `flytekit-1.8.0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/project.py` & `flytekit-1.8.0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/qubole.py` & `flytekit-1.8.0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/schedule.py` & `flytekit-1.8.0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/security.py` & `flytekit-1.8.0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/task.py` & `flytekit-1.8.0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/types.py` & `flytekit-1.8.0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/models/workflow_closure.py` & `flytekit-1.8.0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/__init__.py` & `flytekit-1.8.0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/backfill.py` & `flytekit-1.8.0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/entities.py` & `flytekit-1.8.0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/executions.py` & `flytekit-1.8.0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/lazy_entity.py` & `flytekit-1.8.0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/remote/remote.py` & `flytekit-1.8.0/flytekit/remote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,18 +74,19 @@
     FlyteControlPlaneEntity,
     FlyteLocalEntity,
     Options,
     get_serializable,
     get_serializable_launch_plan,
 )
 
-try:
-    from IPython.core.display import HTML
-except ImportError:
-    ...
+if typing.TYPE_CHECKING:
+    try:
+        from IPython.core.display import HTML
+    except ImportError:
+        ...
 
 ExecutionDataResponse = typing.Union[WorkflowExecutionGetDataResponse, NodeExecutionGetDataResponse]
 
 MOST_RECENT_FIRST = admin_common_models.Sort("created_at", admin_common_models.Sort.Direction.DESCENDING)
 
 
 class RegistrationSkipped(Exception):
@@ -249,14 +250,16 @@
                     raise ValueError(f"Flyte url {flyte_uri} resolved to empty download link")
                 d = data_response.pre_signed_urls.signed_url[0]
                 remote_logger.debug(f"Download link is {d}")
                 fs = ctx.file_access.get_filesystem_for_path(d)
 
                 # If the venv has IPython, then return IPython's HTML
                 if ipython_check():
+                    from IPython.core.display import HTML
+
                     remote_logger.debug(f"IPython found, returning HTML from {flyte_uri}")
                     with fs.open(d, "rb") as r:
                         html = HTML(str(r.read()))
                         return html
                 # If not return bytes
                 else:
                     remote_logger.debug(f"IPython not found, returning HTML as bytes from {flyte_uri}")
```

### Comparing `flytekit-1.7.1b1/flytekit/remote/remote_callable.py` & `flytekit-1.8.0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/testing/__init__.py` & `flytekit-1.8.0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/fast_registration.py` & `flytekit-1.8.0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/ignore.py` & `flytekit-1.8.0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/module_loader.py` & `flytekit-1.8.0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/repo.py` & `flytekit-1.8.0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/script_mode.py` & `flytekit-1.8.0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/serialize_helpers.py` & `flytekit-1.8.0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/subprocess.py` & `flytekit-1.8.0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/tools/translator.py` & `flytekit-1.8.0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/directory/__init__.py` & `flytekit-1.8.0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/directory/types.py` & `flytekit-1.8.0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/file/__init__.py` & `flytekit-1.8.0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/file/file.py` & `flytekit-1.8.0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/iterator/iterator.py` & `flytekit-1.8.0/flytekit/types/iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/numpy/ndarray.py` & `flytekit-1.8.0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/pickle/pickle.py` & `flytekit-1.8.0/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/schema/types.py` & `flytekit-1.8.0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/schema/types_pandas.py` & `flytekit-1.8.0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/structured/__init__.py` & `flytekit-1.8.0/flytekit/types/structured/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
     StructuredDatasetTransformerEngine,
 )
 
 
+def register_csv_handlers():
+
+    from .basic_dfs import CSVToPandasDecodingHandler, PandasToCSVEncodingHandler
+
+    StructuredDatasetTransformerEngine.register(PandasToCSVEncodingHandler(), default_format_for_type=True)
+    StructuredDatasetTransformerEngine.register(CSVToPandasDecodingHandler(), default_format_for_type=True)
+
+
 def register_pandas_handlers():
     import pandas as pd
 
     from .basic_dfs import PandasToParquetEncodingHandler, ParquetToPandasDecodingHandler
 
     StructuredDatasetTransformerEngine.register(PandasToParquetEncodingHandler(), default_format_for_type=True)
     StructuredDatasetTransformerEngine.register(ParquetToPandasDecodingHandler(), default_format_for_type=True)
```

### Comparing `flytekit-1.7.1b1/flytekit/types/structured/basic_dfs.py` & `flytekit-1.8.0/flytekit/types/structured/basic_dfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from flytekit import FlyteContext, logger
 from flytekit.configuration import DataConfig
 from flytekit.core.data_persistence import s3_setup_args
 from flytekit.models import literals
 from flytekit.models.literals import StructuredDatasetMetadata
 from flytekit.models.types import StructuredDatasetType
 from flytekit.types.structured.structured_dataset import (
+    CSV,
     PARQUET,
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
 )
 
 T = TypeVar("T")
@@ -31,14 +32,62 @@
     if protocol == "s3":
         kwargs = s3_setup_args(cfg.s3, anon)
         if kwargs:
             return kwargs
     return None
 
 
+class PandasToCSVEncodingHandler(StructuredDatasetEncoder):
+    def __init__(self):
+        super().__init__(pd.DataFrame, None, CSV)
+
+    def encode(
+        self,
+        ctx: FlyteContext,
+        structured_dataset: StructuredDataset,
+        structured_dataset_type: StructuredDatasetType,
+    ) -> literals.StructuredDataset:
+        uri = typing.cast(str, structured_dataset.uri) or ctx.file_access.get_random_remote_directory()
+        if not ctx.file_access.is_remote(uri):
+            Path(uri).mkdir(parents=True, exist_ok=True)
+        path = os.path.join(uri, ".csv")
+        df = typing.cast(pd.DataFrame, structured_dataset.dataframe)
+        df.to_csv(
+            path,
+            index=False,
+            storage_options=get_storage_options(ctx.file_access.data_config, path),
+        )
+        structured_dataset_type.format = CSV
+        return literals.StructuredDataset(uri=uri, metadata=StructuredDatasetMetadata(structured_dataset_type))
+
+
+class CSVToPandasDecodingHandler(StructuredDatasetDecoder):
+    def __init__(self):
+        super().__init__(pd.DataFrame, None, CSV)
+
+    def decode(
+        self,
+        ctx: FlyteContext,
+        flyte_value: literals.StructuredDataset,
+        current_task_metadata: StructuredDatasetMetadata,
+    ) -> pd.DataFrame:
+        uri = flyte_value.uri
+        columns = None
+        kwargs = get_storage_options(ctx.file_access.data_config, uri)
+        path = os.path.join(uri, ".csv")
+        if current_task_metadata.structured_dataset_type and current_task_metadata.structured_dataset_type.columns:
+            columns = [c.name for c in current_task_metadata.structured_dataset_type.columns]
+        try:
+            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
+        except NoCredentialsError:
+            logger.debug("S3 source detected, attempting anonymous S3 access")
+            kwargs = get_storage_options(ctx.file_access.data_config, uri, anon=True)
+            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
+
+
 class PandasToParquetEncodingHandler(StructuredDatasetEncoder):
     def __init__(self):
         super().__init__(pd.DataFrame, None, PARQUET)
 
     def encode(
         self,
         ctx: FlyteContext,
```

### Comparing `flytekit-1.7.1b1/flytekit/types/structured/bigquery.py` & `flytekit-1.8.0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit/types/structured/structured_dataset.py` & `flytekit-1.8.0/flytekit/types/structured/structured_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 DF = typing.TypeVar("DF")  # Dataframe type
 
 # For specifying the storage formats of StructuredDatasets. It's just a string, nothing fancy.
 StructuredDatasetFormat: TypeAlias = str
 
 # Storage formats
 PARQUET: StructuredDatasetFormat = "parquet"
+CSV: StructuredDatasetFormat = "csv"
 GENERIC_FORMAT: StructuredDatasetFormat = ""
 GENERIC_PROTOCOL: str = "generic protocol"
 
 
 @dataclass_json
 @dataclass
 class StructuredDataset(object):
```

### Comparing `flytekit-1.7.1b1/flytekit.egg-info/PKG-INFO` & `flytekit-1.8.0/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.8.0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.1b1/flytekit.egg-info/SOURCES.txt` & `flytekit-1.8.0/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit.egg-info/requires.txt` & `flytekit-1.8.0/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.8.0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b1/setup.py` & `flytekit-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

