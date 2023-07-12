# Comparing `tmp/jaseci-1.4.1.4.tar.gz` & `tmp/jaseci-1.4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.1.4.tar", last modified: Mon Jul  3 02:04:21 2023, max compression
+gzip compressed data, was "jaseci-1.4.1.5.tar", last modified: Wed Jul 12 14:48:13 2023, max compression
```

## Comparing `jaseci-1.4.1.4.tar` & `jaseci-1.4.1.5.tar`

### file list

```diff
@@ -1,208 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.939410 jaseci-1.4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 02:04:21.939410 jaseci-1.4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.899409 jaseci-1.4.1.4/jaseci/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.903409 jaseci-1.4.1.4/jaseci/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/cli_tools/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/cli_tools/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.903409 jaseci-1.4.1.4/jaseci/cli_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/cli_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/cli_tools/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.903409 jaseci-1.4.1.4/jaseci/extens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.911409 jaseci-1.4.1.4/jaseci/extens/act_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.915409 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/act_lib/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.919409 jaseci-1.4.1.4/jaseci/extens/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.919409 jaseci-1.4.1.4/jaseci/extens/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_uncommon.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/extens/svc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/elastic_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/kube_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/prome_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/redis_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/stripe_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/task_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/extens/svc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    66743 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.923409 jaseci-1.4.1.4/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.927409 jaseci-1.4.1.4/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.927409 jaseci-1.4.1.4/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.927409 jaseci-1.4.1.4/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.927409 jaseci-1.4.1.4/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.927409 jaseci-1.4.1.4/jaseci/jsorc/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/jsorc_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/jsorc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/live_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.931409 jaseci-1.4.1.4/jaseci/jsorc/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/manifests/database.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/manifests/elastic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/manifests/prometheus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/manifests/redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.931409 jaseci-1.4.1.4/jaseci/jsorc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/jsorc/tests/test_jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.931409 jaseci-1.4.1.4/jaseci/prim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/architype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/super_master.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/prim/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.935409 jaseci-1.4.1.4/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.935409 jaseci-1.4.1.4/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.939410 jaseci-1.4.1.4/jaseci/utils/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/actions/actions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/actions/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/actions/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/gprof2dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:04:21.903409 jaseci-1.4.1.4/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 02:04:21.000000 jaseci-1.4.1.4/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:04:21.939410 jaseci-1.4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 02:04:05.000000 jaseci-1.4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.748683 jaseci-1.4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 14:48:13.748683 jaseci-1.4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.712684 jaseci-1.4.1.5/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.716683 jaseci-1.4.1.5/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.716683 jaseci-1.4.1.5/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.716683 jaseci-1.4.1.5/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.720683 jaseci-1.4.1.5/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.720683 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.724683 jaseci-1.4.1.5/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.728683 jaseci-1.4.1.5/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_uncommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.728683 jaseci-1.4.1.5/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.728683 jaseci-1.4.1.5/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.732683 jaseci-1.4.1.5/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67003 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.732683 jaseci-1.4.1.5/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.732683 jaseci-1.4.1.5/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.732683 jaseci-1.4.1.5/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.732683 jaseci-1.4.1.5/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:47.000000 jaseci-1.4.1.5/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.736683 jaseci-1.4.1.5/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.736683 jaseci-1.4.1.5/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.736683 jaseci-1.4.1.5/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.736683 jaseci-1.4.1.5/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.740683 jaseci-1.4.1.5/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.740683 jaseci-1.4.1.5/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.740683 jaseci-1.4.1.5/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.744683 jaseci-1.4.1.5/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.744683 jaseci-1.4.1.5/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.744683 jaseci-1.4.1.5/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.748683 jaseci-1.4.1.5/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:13.716683 jaseci-1.4.1.5/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 14:48:13.000000 jaseci-1.4.1.5/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:48:13.748683 jaseci-1.4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-12 14:47:48.000000 jaseci-1.4.1.5/setup.py
```

### Comparing `jaseci-1.4.1.4/LICENSE` & `jaseci-1.4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/__init__.py` & `jaseci-1.4.1.5/jaseci/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,11 @@
     import jaseci.extens.act_lib.internal  # noqa
     import jaseci.extens.act_lib.zip  # noqa
     import jaseci.extens.act_lib.webtool  # noqa
     import jaseci.extens.act_lib.elastic  # noqa
     import jaseci.extens.act_lib.url  # noqa
     import jaseci.extens.act_lib.stripe  # noqa
     import jaseci.extens.act_lib.regex  # noqa
+    import jaseci.extens.act_lib.maths  # noqa
 
 
 load_standard()
```

### Comparing `jaseci-1.4.1.4/jaseci/cli_tools/book_tools.py` & `jaseci-1.4.1.5/jaseci/cli_tools/book_tools.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/cli_tools/jsctl.py` & `jaseci-1.4.1.5/jaseci/cli_tools/jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/cli_tools/tests/test_jsctl.py` & `jaseci-1.4.1.5/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -414,16 +414,22 @@
 
     def test_jsctl_graph_can(self):
         self.call(f"actions load local {self.infer_loc}")
         r = self.call(
             f"sentinel register "
             f"{os.path.dirname(__file__)}/graph_can.jac -name gc -set_active true"
         )
-        r = self.call("walker run go")
+        r = self.call("walker run go1")
         self.assertEqual(r.split()[0], "2020-01-01T00:00:00")
+        r = self.call("walker run go2")
+        self.assertEqual(r.split()[0], "2020-07-01T00:00:00")
+        r = self.call("walker run go3")
+        self.assertEqual(r.split()[0], "2020-01-01T00:00:00")
+        self.assertEqual(r.split()[1], "2020-07-01T00:00:00")
+        self.assertEqual(r.split()[2], "2020-07-10T00:00:00")
 
     def test_jsctl_action_call(self):
         self.call(f"actions load local {self.infer_loc}")
         r = self.call(f"actions call infer.date_now")
         r = json.loads(r)
         import datetime
 
@@ -508,16 +514,16 @@
 
     def test_jsctl_pretty_profiles(self):
         self.call(f"actions load local {self.infer_loc}")
         r = self.call(
             f"sentinel register "
             f"{os.path.dirname(__file__)}/graph_can.jac -name gc -set_active true"
         )
-        r = self.call("walker run go -profiling true")
-        self.assertIn("walker::go", r)
+        r = self.call("walker run go1 -profiling true")
+        self.assertIn("walker::go1", r)
         self.assertIn("cumtime", r)
         self.assertIn("cum_time", r)
 
 
 class JsctlTestWithSession(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
```

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/date.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/elastic.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/file.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/file.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/jaseci.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/jaseci.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/net.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/net.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/rand.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/rand.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/regex.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/request.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/request.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/std.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/stripe.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/std_test_code.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_date.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_elastic.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_file_lib.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_mail_lib.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_mail_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_net_lib.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_regex.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_std.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_std_lib.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_url.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_vector.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_webtool.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/tests/test_zlib.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/url.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/vector.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/webtool.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/act_lib/zip.py` & `jaseci-1.4.1.5/jaseci/extens/act_lib/zip.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/actions_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/alias_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/alias_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/architype_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/config_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/config_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/global_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/graph_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/interface.py` & `jaseci-1.4.1.5/jaseci/extens/api/interface.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/jac_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/jac_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/jsorc_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/jsorc_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/logger_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/master_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/master_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/object_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/prometheus_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/sentinel_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/super_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/super_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_architype_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_global_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_graph_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_logger_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_object_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_sentinel_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_user_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/tests/test_walker_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/tests/test_walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/user_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/walker_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/api/webhook_api.py` & `jaseci-1.4.1.5/jaseci/extens/api/webhook_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,32 +23,34 @@
             stripe_service = JsOrc.svc("stripe", StripeService)
             stripe = stripe_service.poke(_stripe)
 
             # to be updated
             stripe_service.get_event(_raw_req_ctx, _req_ctx["headers"])
 
             payload_obj = req_body.get("data").get("object")
-            customer_id = payload_obj.get("customer")
+            payload_meta = payload_obj.get("metadata")
 
-            if customer_id:
-                customer = stripe.Customer.retrieve(id=customer_id)
-                metadata = customer.get("metadata")
-            else:
-                metadata = payload_obj.get("metadata")
+            customer_id = payload_obj.get("customer")
+            customer_meta = (
+                stripe.Customer.retrieve(id=customer_id).get("metadata")
+                if customer_id
+                else {}
+            )
 
-            master_id = metadata.get("master")
+            master_id = payload_meta.get("master") or customer_meta.get("master")
             master = self._h.get_obj(master_id, master_id)
 
-            node_id = metadata.get("node")
+            node_id = payload_meta.get("node") or customer_meta.get("node")
             if not node_id:
                 node_id = master.active_gph_id
             node = self._h.get_obj(master_id, node_id)
 
             sentinel_id = (
-                metadata.get("sentinel")
+                payload_meta.get("sentinel")
+                or customer_meta.get("sentinel")
                 or master.active_snt_id
                 or self._h.get_glob("GLOB_SENTINEL")
             )
             sentinel = self._h.get_obj(
                 master_id,
                 self._h.get_glob("GLOB_SENTINEL")
                 if sentinel_id == "global"
```

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/elastic_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/elastic_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/kube_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/kube_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/mail_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/prome_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/prome_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/redis_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/redis_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/stripe_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/stripe_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/task_svc.py` & `jaseci-1.4.1.5/jaseci/extens/svc/task_svc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from celery import Celery
+from celery.schedules import crontab
 from celery.app.trace import build_tracer
 from celery.app.control import Inspect
 from celery.backends.base import DisabledBackend
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.jsorc.jsorc_utils import ManifestType
 from .tasks import Queue, ScheduledWalker, ScheduledSequence
@@ -103,18 +104,52 @@
     #                     QUEUING                     #
     ###################################################
 
     def add_queue(self, wlk, nd, *args):
         return self.queue.delay(wlk.jid, nd.jid, args).task_id
 
     ###################################################
+    #                SCHEDULED QUEUING                #
+    ###################################################
+
+    def add_scheduled_queue(
+        self, queue_type: object, name: str, schedule: dict, body: dict
+    ):
+        return None
+
+    def get_scheduled_queues(
+        self,
+        limit: int = 10,
+        offset: int = 0,
+        asc: bool = True,
+        name: str = None,
+        master=False,
+    ):
+        return []
+
+    def delete_scheduled_queue(self, scheduled_queue_id: int, master):
+        return None
+
+    ###################################################
     #                     CLEANER                     #
     ###################################################
 
     def failed(self, error):
         super().failed(error)
         self.terminate_daemon("worker", "scheduler")
 
     # ---------------- PROXY EVENTS ----------------- #
 
     def on_delete(self):
         self.terminate_daemon("worker", "scheduler")
+
+    ###################################################
+    #                      UTILS                      #
+    ###################################################
+
+    def get_task_name(self, task):
+        cls = type(task)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module is not None and module != "__builtin__":
+            name = module + "." + name
+        return name
```

### Comparing `jaseci-1.4.1.4/jaseci/extens/svc/tasks.py` & `jaseci-1.4.1.5/jaseci/extens/svc/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from requests.exceptions import HTTPError
 from jaseci.jsorc.jsorc import JsOrc
 
 DEFAULT_MSG = "Skipping scheduled walker!"
 
 
 class Queue(Task):
-    def run(self, wlk, nd, args):
+    def run(self, wlk: str, nd: str, args):
         hook = JsOrc.hook()
 
         wlk = hook.get_obj_from_store(wlk)
         wlk._to_await = True
 
         nd = hook.get_obj_from_store(nd)
         resp = wlk.run(nd, *args)
@@ -30,15 +30,15 @@
         return {"anchor": wlk.anchor_value(), "response": resp}
 
 
 class ScheduledWalker(Task):
     def get_obj(self, jid):
         return self.hook.get_obj_from_store(jid)
 
-    def run(self, mst, wlk, ctx, nd=None, snt=None):
+    def run(self, mst, wlk="init", ctx: dict = {}, nd: str = None, snt: str = None):
         self.hook = JsOrc.hook()
 
         if mst:
             mst = self.get_obj(mst)
         else:
             return f"{DEFAULT_MSG} mst (Master) is required!"
```

### Comparing `jaseci-1.4.1.4/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.1.5/jaseci/jac/interpreter/architype_interp.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,17 @@
         graph_block:
             LBRACE has_root can_block KW_SPAWN code_block RBRACE
             | COLON has_root can_block KW_SPAWN code_block SEMI;
         """
         kid = self.set_cur_ast(jac_ast)
         root_name = self.run_has_root(kid[1])
         try:
+            for ability in self.get_all_abilities().obj_list():
+                self._jac_scope.add_action(ability)
+
             self.run_code_block(kid[4])
         except Exception as e:
             self.rt_error(f"Internal Exception: {e}", self._cur_jac_ast)
         local_state = self._jac_scope.local_scope
         if root_name in local_state.keys():
             obj = local_state[root_name]
             if not isinstance(obj, Node):
```

### Comparing `jaseci-1.4.1.4/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.1.5/jaseci/jac/interpreter/interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,15 +871,17 @@
                     kid[0],
                 )
         # may want to remove 'here" node from return below
         elif typ.value == Node:
             if isinstance(atom_res.value, Node):
                 return atom_res
             elif isinstance(atom_res.value, Edge):
-                return JacValue(self, value=self.obj_set_to_jac_set(atom_res.nodes()))
+                return JacValue(
+                    self, value=self.obj_set_to_jac_set(atom_res.value.nodes())
+                )
             elif isinstance(atom_res.value, JacSet):
                 res = JacSet()
                 for i in atom_res.value.obj_list():
                     if isinstance(i, Edge):
                         res.add_obj(i.to_node())
                         res.add_obj(i.from_node())
                     elif isinstance(i, Node):
@@ -1233,16 +1235,21 @@
         """
         kid = self.set_cur_ast(jac_ast)
         if not is_spawn:
             result = JacSet()
             viable_nodes = self.visibility_prune(viable_nodes)
             if len(kid) > 1:
                 for i in viable_nodes.obj_list():
-                    if i.get_architype().is_instance(kid[-1].token_text()):
-                        result.add_obj(i)
+                    try:
+                        if i.get_architype().is_instance(kid[-1].token_text()):
+                            result.add_obj(i)
+                    except:
+                        self.rt_warn(
+                            f"Error occured while getting architype {i.name}. Skipping..."
+                        )
             else:
                 result += viable_nodes
         else:
             result = self.parent().run_architype(
                 kid[-1].token_text(), kind="node", caller=self
             )
         return result
```

### Comparing `jaseci-1.4.1.4/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.1.5/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.1.5/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.1.5/jaseci/jac/interpreter/walker_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/ast.py` & `jaseci-1.4.1.5/jaseci/jac/ir/ast.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.1.5/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.1.5/jaseci/jac/ir/jac_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.1.5/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.1.5/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.1.5/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.1.5/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.1.5/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jac.g4` & `jaseci-1.4.1.5/jaseci/jac/jac.g4`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.1.5/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.1.5/jaseci/jac/jac_parse/jacListener.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.1.5/jaseci/jac/jac_parse/jacParser.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jac_set.py` & `jaseci-1.4.1.5/jaseci/jac/jac_set.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.1.5/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.1.5/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.1.5/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.1.5/jaseci/jac/jsci_vm/op_codes.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.1.5/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.1.5/jaseci/jac/machine/jac_scope.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.1.5/jaseci/jac/machine/jac_value.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.1.5/jaseci/jac/machine/machine_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/tests/book_code.py` & `jaseci-1.4.1.5/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/tests/test_book.py` & `jaseci-1.4.1.5/jaseci/jac/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.1.5/jaseci/jac/tests/test_lang_14.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/jsorc.py` & `jaseci-1.4.1.5/jaseci/jsorc/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/jsorc_settings.py` & `jaseci-1.4.1.5/jaseci/jsorc/jsorc_settings.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/jsorc_utils.py` & `jaseci-1.4.1.5/jaseci/jsorc/jsorc_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/live_actions.py` & `jaseci-1.4.1.5/jaseci/jsorc/live_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,27 +235,35 @@
                 "date",
                 "jaseci",
                 "internal",
                 "zip",
                 "webtool",
                 "url",
                 "regex",
+                "maths",
             ]:
                 if name[0] not in glob_act_group:
                     glob_act_group[name[0]] = {}
                 glob_act_group[name[0]][name[1]] = Ability(
                     m_id=0,
                     h=glob_act_hook,
                     mode="public",
                     name=i,
                     kind="ability",
                     value=i,
                     persist=False,
                 )
-    return glob_act_group
+
+    # second layer copy and this will use the same Ability object
+    # deepcopy will be much expensive and will also use new Ability Objects
+    temp_glob_act_group = {}
+    for key, value in glob_act_group.items():
+        temp_glob_act_group[key] = value.copy()
+
+    return temp_glob_act_group
 
 
 def unload_remote_actions(url):
     """
     Get the list of actions from the given URL and then unload them.
     """
     headers = {"content-type": "application/json"}
```

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/manifests/database.yaml` & `jaseci-1.4.1.5/jaseci/jsorc/manifests/database.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/manifests/elastic.yaml` & `jaseci-1.4.1.5/jaseci/jsorc/manifests/elastic.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/manifests/prometheus.yaml` & `jaseci-1.4.1.5/jaseci/jsorc/manifests/prometheus.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/manifests/redis.yaml` & `jaseci-1.4.1.5/jaseci/jsorc/manifests/redis.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/memory.py` & `jaseci-1.4.1.5/jaseci/jsorc/memory.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/redis.py` & `jaseci-1.4.1.5/jaseci/jsorc/redis.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/remote_actions.py` & `jaseci-1.4.1.5/jaseci/jsorc/remote_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/tests/test_actions.py` & `jaseci-1.4.1.5/jaseci/jsorc/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/jsorc/tests/test_jsorc.py` & `jaseci-1.4.1.5/jaseci/jsorc/tests/test_jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/ability.py` & `jaseci-1.4.1.5/jaseci/prim/ability.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/architype.py` & `jaseci-1.4.1.5/jaseci/prim/architype.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/edge.py` & `jaseci-1.4.1.5/jaseci/prim/edge.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/element.py` & `jaseci-1.4.1.5/jaseci/prim/element.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/graph.py` & `jaseci-1.4.1.5/jaseci/prim/graph.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/master.py` & `jaseci-1.4.1.5/jaseci/prim/master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/node.py` & `jaseci-1.4.1.5/jaseci/prim/node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/obj_mixins.py` & `jaseci-1.4.1.5/jaseci/prim/obj_mixins.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/sentinel.py` & `jaseci-1.4.1.5/jaseci/prim/sentinel.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/super_master.py` & `jaseci-1.4.1.5/jaseci/prim/super_master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/prim/walker.py` & `jaseci-1.4.1.5/jaseci/prim/walker.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/infer.py` & `jaseci-1.4.1.5/jaseci/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/jac_test_code.py` & `jaseci-1.4.1.5/jaseci/tests/jac_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.1.5/jaseci/tests/jac_test_progs.py`

 * *Files 2% similar despite different names*

```diff
@@ -751,7 +751,21 @@
 walker json_casting {
     with entry {
         report {"test": 1}.str;
         report '{"test2": 2}'.dict;
     }
 }
 """
+
+edge_to_node_casting = """
+node a {}
+
+walker edge_to_node_casting {
+    root {
+        spawn here ++> node::a;
+        edges = --> node::a.edge;
+        report edges;
+        report edges.node;
+        report edges[0].node;
+    }
+}
+"""
```

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_core.py` & `jaseci-1.4.1.5/jaseci/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_jac.py` & `jaseci-1.4.1.5/jaseci/tests/test_jac.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_node.py` & `jaseci-1.4.1.5/jaseci/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_progs.py` & `jaseci-1.4.1.5/jaseci/tests/test_progs.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,7 +665,30 @@
         )
 
         self.assertTrue(res["success"])
         self.assertEqual(
             res["report"],
             ['{"test": 1}', {"test2": 2}],
         )
+
+    def test_edge_to_node_casting(self):
+        mast = JsOrc.master()
+        mast.sentinel_register(name="test", code=jtp.edge_to_node_casting, auto_run="")
+
+        res = mast.general_interface_to_api(
+            api_name="walker_run",
+            params={"name": "edge_to_node_casting", "ctx": {}},
+        )
+
+        self.assertTrue(res["success"])
+
+        edges = res["report"][0]
+        self.assertEqual(1, len(edges))
+        self.assertEqual("edge", edges[0]["kind"])
+
+        nodes = res["report"][1]
+        self.assertEqual(2, len(nodes))
+
+        self.assertEqual(edges[0]["to_node_id"], nodes[0]["jid"])
+        self.assertEqual("a", nodes[0]["name"])
+        self.assertEqual(edges[0]["from_node_id"], nodes[1]["jid"])
+        self.assertEqual("root", nodes[1]["name"])
```

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_stack.py` & `jaseci-1.4.1.5/jaseci/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/tests/test_stripe.py` & `jaseci-1.4.1.5/jaseci/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/actions/actions_manager.py` & `jaseci-1.4.1.5/jaseci/utils/actions/actions_manager.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/actions/actions_optimizer.py` & `jaseci-1.4.1.5/jaseci/utils/actions/actions_optimizer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/actions/actions_state.py` & `jaseci-1.4.1.5/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/gprof2dot.py` & `jaseci-1.4.1.5/jaseci/utils/gprof2dot.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/id_list.py` & `jaseci-1.4.1.5/jaseci/utils/id_list.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/json_handler.py` & `jaseci-1.4.1.5/jaseci/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/log_utils.py` & `jaseci-1.4.1.5/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/test_core.py` & `jaseci-1.4.1.5/jaseci/utils/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci/utils/utils.py` & `jaseci-1.4.1.5/jaseci/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.4/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.1.5/jaseci.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 jaseci/extens/act_lib/__init__.py
 jaseci/extens/act_lib/date.py
 jaseci/extens/act_lib/elastic.py
 jaseci/extens/act_lib/file.py
 jaseci/extens/act_lib/internal.py
 jaseci/extens/act_lib/jaseci.py
 jaseci/extens/act_lib/mail.py
+jaseci/extens/act_lib/maths.py
 jaseci/extens/act_lib/net.py
 jaseci/extens/act_lib/rand.py
 jaseci/extens/act_lib/regex.py
 jaseci/extens/act_lib/request.py
 jaseci/extens/act_lib/std.py
 jaseci/extens/act_lib/stripe.py
 jaseci/extens/act_lib/task.py
@@ -35,14 +36,15 @@
 jaseci/extens/act_lib/zip.py
 jaseci/extens/act_lib/tests/__init__.py
 jaseci/extens/act_lib/tests/std_test_code.py
 jaseci/extens/act_lib/tests/test_date.py
 jaseci/extens/act_lib/tests/test_elastic.py
 jaseci/extens/act_lib/tests/test_file_lib.py
 jaseci/extens/act_lib/tests/test_mail_lib.py
+jaseci/extens/act_lib/tests/test_maths.py
 jaseci/extens/act_lib/tests/test_net_lib.py
 jaseci/extens/act_lib/tests/test_regex.py
 jaseci/extens/act_lib/tests/test_std.py
 jaseci/extens/act_lib/tests/test_std_lib.py
 jaseci/extens/act_lib/tests/test_url.py
 jaseci/extens/act_lib/tests/test_vector.py
 jaseci/extens/act_lib/tests/test_webtool.py
```

### Comparing `jaseci-1.4.1.4/setup.py` & `jaseci-1.4.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "fastapi[all]>=0.75.0,<1.0.0",
         "requests",
         "redis",
         "celery>=5,<6",
         "flake8",
         "pep8-naming",
         "stripe",
-        "pydantic",
+        "pydantic==1.10.11",
         "docstring-parser",
         "prometheus_api_client==0.5.1",
         "prometheus-client==0.14.1",
         "kubernetes==23.6.0",
         "pytest",
         "pytest-xdist",
         "pytest-cov",
```

