# Comparing `tmp/nopasaran-0.2.7.tar.gz` & `tmp/nopasaran-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.7.tar", last modified: Tue Jul 11 10:33:52 2023, max compression
+gzip compressed data, was "nopasaran-0.2.8.tar", last modified: Wed Jul 12 13:04:24 2023, max compression
```

## Comparing `nopasaran-0.2.7.tar` & `nopasaran-0.2.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.221585 nopasaran-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 10:33:43.000000 nopasaran-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-11 10:33:52.217585 nopasaran-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-11 10:33:43.000000 nopasaran-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.201585 nopasaran-0.2.7/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.205585 nopasaran-0.2.7/nopasaran/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/errors/parsing_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.209585 nopasaran-0.2.7/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.213585 nopasaran-0.2.7/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/action_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/action_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/control_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/dns_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/event_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/io_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/ip_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/nested_machine_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/tcp_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/action_primitives/udp_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/condition_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/condition_primitives/variable_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/assignment_transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/primitives/transition_primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-11 10:33:43.000000 nopasaran-0.2.7/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.201585 nopasaran-0.2.7/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:33:52.000000 nopasaran-0.2.7/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:33:52.221585 nopasaran-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 10:33:51.000000 nopasaran-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:52.217585 nopasaran-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:33:43.000000 nopasaran-0.2.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 13:04:16.000000 nopasaran-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-12 13:04:24.588588 nopasaran-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-12 13:04:16.000000 nopasaran-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/errors/parsing_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/action_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/action_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/control_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/dns_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/event_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/io_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/ip_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/nested_machine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/tcp_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/udp_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/condition_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/variable_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/assignment_transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:04:24.588588 nopasaran-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 13:04:23.000000 nopasaran-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/tests/__init__.py
```

### Comparing `nopasaran-0.2.7/LICENSE` & `nopasaran-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/PKG-INFO` & `nopasaran-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.7
+Version: 0.2.8
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.7/README.md` & `nopasaran-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/__main__.py` & `nopasaran-0.2.8/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/controllers/controller.py` & `nopasaran-0.2.8/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/controllers/factory.py` & `nopasaran-0.2.8/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/controllers/protocol.py` & `nopasaran-0.2.8/nopasaran/controllers/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import logging
+import base64
+import pickle
 
 from twisted.internet.protocol import Protocol
 
 from nopasaran.definitions.control_channel import JSONMessage, Status
 
 
 class WorkerProtocol(Protocol):
@@ -41,16 +43,22 @@
             self.remote_status = data[JSONMessage.STATUS.name]
             if self.local_status == Status.CONNECTED.name and self.remote_status == Status.CONNECTED.name:
                 self.local_status = Status.READY.name
                 self.transport.write(self.get_current_state_json())
             if self.local_status == Status.DISCONNECTING.name and self.remote_status == Status.DISCONNECTING.name:
                 self.is_active = False
                 self.transport.loseConnection()
+        if JSONMessage.SYNC.name in data:
+            encoded_data = data[JSONMessage.SYNC.name]
+            serialized_data = base64.b64decode(encoded_data)
+            content = pickle.loads(serialized_data)
+            self.queue.append(content)
         logging.info("[Control Channel] Status: %s, %s", self.local_status, self.remote_status)
         logging.info("[Control Channel] Received: %s", data)
+        
 
     def disconnecting(self):
         """
         Initiate the disconnection process.
         
         This method sets the local status to DISCONNECTING and sends the current state to the remote endpoint.
         """
@@ -75,15 +83,17 @@
         Send a sync message to the remote endpoint.
         
         This method sends a sync message with the specified content to the remote endpoint.
         
         Args:
             content: The content of the sync message.
         """
-        self.transport.write(json.dumps({JSONMessage.SYNC.name: content}).encode())
+        serialized_data = pickle.dumps(content)
+        encoded_data = base64.b64encode(serialized_data).decode("utf-8")
+        self.transport.write(json.dumps({JSONMessage.SYNC.name: encoded_data}).encode())
         logging.info("[Control Channel] Sync message sent: %s", content)
 
 
 class WorkerClientProtocol(WorkerProtocol):
     """
     Protocol for worker clients.
```

### Comparing `nopasaran-0.2.7/nopasaran/decorators.py` & `nopasaran-0.2.8/nopasaran/decorators.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.8/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/errors/parsing_error.py` & `nopasaran-0.2.8/nopasaran/errors/parsing_error.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.8/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.8/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.8/nopasaran/interpreters/interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.8/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.8/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/machines/action_queue.py` & `nopasaran-0.2.8/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/machines/state_machine.py` & `nopasaran-0.2.8/nopasaran/machines/state_machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.8/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.8/nopasaran/parsers/state_machine_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/action_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/action_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/control_channel_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/control_channel_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,16 @@
             state_machine: The state machine object.
 
         Returns:
             None
         """
         controller_protocol = state_machine.get_variable_value(inputs[0])
         if controller_protocol:
-            controller_protocol.send_sync(inputs[1:])
+            data_to_send = [state_machine.get_variable_value(input_value) for input_value in inputs[1:]]
+            controller_protocol.send_sync(data_to_send)
             state_machine.trigger_event(EventNames.SYNC_SENT.name)
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0, optional_outputs=True)
     def wait_sync_signal(inputs, outputs, state_machine):
         """
         Wait for a synchronization message to be available in the controller protocol's queue.
@@ -239,9 +240,9 @@
             if time.time() - start_time > float(state_machine.get_variable_value(inputs[1])):
                 timeout = True
                 break
         if timeout:
             state_machine.trigger_event(EventNames.TIMEOUT.name)
         else:
             for index in range(len(outputs)):
-                state_machine.set_variable_value(outputs[index], sync_message[JSONMessage.SYNC.name][index])
+                state_machine.set_variable_value(outputs[index], sync_message[index])
             state_machine.trigger_event(EventNames.SYNC_AVAILABLE.name)
```

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_channel_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_channel_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/data_manipulation.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/dns_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/dns_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/event_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/event_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/io_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/io_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/ip_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/ip_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/nested_machine_utils.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/nested_machine_utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/tcp_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/tcp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/action_primitives/udp_primitives.py` & `nopasaran-0.2.8/nopasaran/primitives/action_primitives/udp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/condition_primitives/variable_comparisons.py` & `nopasaran-0.2.8/nopasaran/primitives/condition_primitives/variable_comparisons.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/primitives/transition_primitives/assignment_transitions.py` & `nopasaran-0.2.8/nopasaran/primitives/transition_primitives/assignment_transitions.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.8/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran/utils.py` & `nopasaran-0.2.8/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.8/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.7
+Version: 0.2.8
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.7/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.8/nopasaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.7/setup.py` & `nopasaran-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.7',
+    version='0.2.8',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

