# Comparing `tmp/nidaqmx-0.8.0.tar.gz` & `tmp/nidaqmx-0.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidaqmx-0.8.0.tar", max compression
+gzip compressed data, was "nidaqmx-0.8.0.dev0.tar", max compression
```

## Comparing `nidaqmx-0.8.0.tar` & `nidaqmx-0.8.0.dev0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      640 2023-06-30 20:45:34.915990 nidaqmx-0.8.0/generated/nidaqmx/__init__.py
--rw-r--r--   0        0        0    61393 2023-07-10 21:22:26.518154 nidaqmx-0.8.0/generated/nidaqmx/_base_interpreter.py
--rw-r--r--   0        0        0     1505 2023-06-30 20:45:34.916989 nidaqmx-0.8.0/generated/nidaqmx/_bitfield_utils.py
--rw-r--r--   0        0        0   167908 2023-07-10 21:22:26.519152 nidaqmx-0.8.0/generated/nidaqmx/_grpc_interpreter.py
--rw-r--r--   0        0        0     6060 2023-07-12 19:06:55.391248 nidaqmx-0.8.0/generated/nidaqmx/_lib.py
--rw-r--r--   0        0        0   259462 2023-07-10 21:22:26.521152 nidaqmx-0.8.0/generated/nidaqmx/_library_interpreter.py
--rw-r--r--   0        0        0       34 2023-07-10 21:22:26.521152 nidaqmx-0.8.0/generated/nidaqmx/_stubs/__init__.py
--rw-r--r--   0        0        0   573921 2023-07-10 21:22:26.524153 nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2.py
--rw-r--r--   0        0        0  1643650 2023-07-10 21:22:26.533156 nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2.pyi
--rw-r--r--   0        0        0   671385 2023-07-10 21:22:26.537155 nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.py
--rw-r--r--   0        0        0   158814 2023-07-10 21:22:26.539157 nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.pyi
--rw-r--r--   0        0        0     4248 2023-07-10 21:22:26.540175 nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2.py
--rw-r--r--   0        0        0     8974 2023-07-10 21:22:26.541155 nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2.pyi
--rw-r--r--   0        0        0     9124 2023-07-10 21:22:26.542193 nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0     2923 2023-07-10 21:22:26.542193 nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.409211 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/__init__.py
--rw-r--r--   0        0        0   178850 2023-07-10 21:22:26.543192 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ai_channel_collection.py
--rw-r--r--   0        0        0     7596 2023-07-10 21:22:26.544189 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ao_channel_collection.py
--rw-r--r--   0        0        0     4276 2023-06-30 20:45:34.917990 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channel_collection.py
--rw-r--r--   0        0        0      512 2023-04-03 18:57:20.410211 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/__init__.py
--rw-r--r--   0        0        0   142396 2023-07-10 21:22:26.545191 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ai_channel.py
--rw-r--r--   0        0        0    33120 2023-07-10 21:22:26.546154 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ao_channel.py
--rw-r--r--   0        0        0    10280 2023-07-10 21:22:26.547155 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/channel.py
--rw-r--r--   0        0        0   181156 2023-07-10 21:22:26.548153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ci_channel.py
--rw-r--r--   0        0        0    26347 2023-07-10 21:22:26.549153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/co_channel.py
--rw-r--r--   0        0        0    12499 2023-07-10 21:22:26.549153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/di_channel.py
--rw-r--r--   0        0        0    13754 2023-07-10 21:22:26.550153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/do_channel.py
--rw-r--r--   0        0        0    46387 2023-07-10 21:22:26.550153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ci_channel_collection.py
--rw-r--r--   0        0        0     8612 2023-07-10 21:22:26.551153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/co_channel_collection.py
--rw-r--r--   0        0        0     4096 2023-07-10 21:22:26.551153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/di_channel_collection.py
--rw-r--r--   0        0        0     4094 2023-07-10 21:22:26.552154 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/do_channel_collection.py
--rw-r--r--   0        0        0    36299 2023-07-10 21:22:26.553152 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/export_signals.py
--rw-r--r--   0        0        0    48904 2023-07-10 21:22:26.553152 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/in_stream.py
--rw-r--r--   0        0        0    21499 2023-07-10 21:22:26.554154 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/out_stream.py
--rw-r--r--   0        0        0    53479 2023-07-10 21:22:26.555153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/timing.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.411212 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/__init__.py
--rw-r--r--   0        0        0     7885 2023-07-10 21:22:26.555153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py
--rw-r--r--   0        0        0     2118 2023-07-10 21:22:26.556153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py
--rw-r--r--   0        0        0    22198 2023-07-10 21:22:26.556153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py
--rw-r--r--   0        0        0    42343 2023-07-10 21:22:26.557153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py
--rw-r--r--   0        0        0    39696 2023-07-10 21:22:26.557153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/start_trigger.py
--rw-r--r--   0        0        0     3368 2023-07-10 21:22:26.558153 nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggers.py
--rw-r--r--   0        0        0    50249 2023-07-10 21:21:26.919343 nidaqmx-0.8.0/generated/nidaqmx/constants.py
--rw-r--r--   0        0        0    93605 2023-07-10 21:21:26.891726 nidaqmx-0.8.0/generated/nidaqmx/error_codes.py
--rw-r--r--   0        0        0     5869 2023-06-30 20:45:34.917990 nidaqmx-0.8.0/generated/nidaqmx/errors.py
--rw-r--r--   0        0        0     3587 2023-06-30 20:45:34.917990 nidaqmx-0.8.0/generated/nidaqmx/grpc_session_options.py
--rw-r--r--   0        0        0    22198 2023-07-10 21:22:26.558153 nidaqmx-0.8.0/generated/nidaqmx/scale.py
--rw-r--r--   0        0        0   119899 2023-06-30 20:45:34.918990 nidaqmx-0.8.0/generated/nidaqmx/stream_readers.py
--rw-r--r--   0        0        0    68185 2023-06-30 20:45:34.919989 nidaqmx-0.8.0/generated/nidaqmx/stream_writers.py
--rw-r--r--   0        0        0      426 2023-04-03 18:57:20.415213 nidaqmx-0.8.0/generated/nidaqmx/system/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.415213 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/__init__.py
--rw-r--r--   0        0        0     3579 2023-06-30 20:45:34.919989 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/device_collection.py
--rw-r--r--   0        0        0     3840 2023-06-30 20:45:34.920990 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_channel_collection.py
--rw-r--r--   0        0        0     3700 2023-06-30 20:45:34.920990 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_scale_collection.py
--rw-r--r--   0        0        0     3635 2023-06-30 20:45:34.921990 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_task_collection.py
--rw-r--r--   0        0        0     7366 2023-06-30 20:45:34.921990 nidaqmx-0.8.0/generated/nidaqmx/system/_collections/physical_channel_collection.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.419223 nidaqmx-0.8.0/generated/nidaqmx/system/_watchdog_modules/__init__.py
--rw-r--r--   0        0        0     6072 2023-07-10 21:22:26.559153 nidaqmx-0.8.0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py
--rw-r--r--   0        0        0     1473 2023-06-30 20:45:34.922990 nidaqmx-0.8.0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py
--rw-r--r--   0        0        0    39429 2023-07-10 21:22:26.560153 nidaqmx-0.8.0/generated/nidaqmx/system/device.py
--rw-r--r--   0        0        0    24660 2023-07-10 21:22:26.560153 nidaqmx-0.8.0/generated/nidaqmx/system/physical_channel.py
--rw-r--r--   0        0        0      275 2023-04-03 18:57:20.420224 nidaqmx-0.8.0/generated/nidaqmx/system/storage/__init__.py
--rw-r--r--   0        0        0     3159 2023-06-30 20:45:34.922990 nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_channel.py
--rw-r--r--   0        0        0     3426 2023-06-30 20:45:34.922990 nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_scale.py
--rw-r--r--   0        0        0     3560 2023-06-30 20:45:34.923990 nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_task.py
--rw-r--r--   0        0        0    26836 2023-07-10 21:22:26.561153 nidaqmx-0.8.0/generated/nidaqmx/system/system.py
--rw-r--r--   0        0        0    16001 2023-07-10 21:22:26.562152 nidaqmx-0.8.0/generated/nidaqmx/system/watchdog.py
--rw-r--r--   0        0        0    54236 2023-06-30 20:45:34.923990 nidaqmx-0.8.0/generated/nidaqmx/task.py
--rw-r--r--   0        0        0     1430 2023-04-03 18:57:20.423214 nidaqmx-0.8.0/generated/nidaqmx/types.py
--rw-r--r--   0        0        0     9543 2023-06-30 20:45:34.924991 nidaqmx-0.8.0/generated/nidaqmx/utils.py
--rw-r--r--   0        0        0     1213 2022-05-26 20:15:36.274851 nidaqmx-0.8.0/LICENSE
--rw-r--r--   0        0        0     5026 2023-07-12 19:07:10.293581 nidaqmx-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7076 2023-04-05 15:42:42.306919 nidaqmx-0.8.0/README.rst
--rw-r--r--   0        0        0     8896 1970-01-01 00:00:00.000000 nidaqmx-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      640 2023-06-30 20:45:34.816394 nidaqmx-0.8.0.dev0/generated/nidaqmx/__init__.py
+-rw-r--r--   0        0        0    61393 2023-06-30 20:45:34.817435 nidaqmx-0.8.0.dev0/generated/nidaqmx/_base_interpreter.py
+-rw-r--r--   0        0        0     1505 2023-06-30 20:45:34.818394 nidaqmx-0.8.0.dev0/generated/nidaqmx/_bitfield_utils.py
+-rw-r--r--   0        0        0   167908 2023-06-30 20:45:34.819411 nidaqmx-0.8.0.dev0/generated/nidaqmx/_grpc_interpreter.py
+-rw-r--r--   0        0        0     6060 2023-06-30 20:45:34.819411 nidaqmx-0.8.0.dev0/generated/nidaqmx/_lib.py
+-rw-r--r--   0        0        0   259462 2023-06-30 20:45:34.820394 nidaqmx-0.8.0.dev0/generated/nidaqmx/_library_interpreter.py
+-rw-r--r--   0        0        0       34 2023-06-30 20:45:34.821432 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/__init__.py
+-rw-r--r--   0        0        0   573921 2023-06-30 20:45:34.824422 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.py
+-rw-r--r--   0        0        0  1643650 2023-06-30 20:45:34.831990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.pyi
+-rw-r--r--   0        0        0   671385 2023-06-30 20:45:34.836990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.py
+-rw-r--r--   0        0        0   158814 2023-06-30 20:45:34.838017 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4248 2023-06-30 20:45:34.838991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.py
+-rw-r--r--   0        0        0     8974 2023-06-30 20:45:34.838991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     9124 2023-06-30 20:45:34.839991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0     2923 2023-06-30 20:45:34.839991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.409211 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/__init__.py
+-rw-r--r--   0        0        0   178850 2023-06-30 20:45:34.842018 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ai_channel_collection.py
+-rw-r--r--   0        0        0     7596 2023-06-30 20:45:34.842018 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ao_channel_collection.py
+-rw-r--r--   0        0        0     4276 2023-06-30 20:45:34.842991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channel_collection.py
+-rw-r--r--   0        0        0      512 2023-04-03 18:57:20.410211 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/__init__.py
+-rw-r--r--   0        0        0   142396 2023-06-30 20:45:34.844009 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ai_channel.py
+-rw-r--r--   0        0        0    33120 2023-06-30 20:45:34.845010 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ao_channel.py
+-rw-r--r--   0        0        0    10280 2023-06-30 20:45:34.845989 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/channel.py
+-rw-r--r--   0        0        0   181156 2023-06-30 20:45:34.847009 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ci_channel.py
+-rw-r--r--   0        0        0    26347 2023-06-30 20:45:34.847991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/co_channel.py
+-rw-r--r--   0        0        0    12499 2023-06-30 20:45:34.847991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/di_channel.py
+-rw-r--r--   0        0        0    13754 2023-06-30 20:45:34.848991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/do_channel.py
+-rw-r--r--   0        0        0    46387 2023-06-30 20:45:34.848991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ci_channel_collection.py
+-rw-r--r--   0        0        0     8612 2023-06-30 20:45:34.849990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/co_channel_collection.py
+-rw-r--r--   0        0        0     4096 2023-06-30 20:45:34.849990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/di_channel_collection.py
+-rw-r--r--   0        0        0     4094 2023-06-30 20:45:34.850991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/do_channel_collection.py
+-rw-r--r--   0        0        0    36299 2023-06-30 20:45:34.850991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/export_signals.py
+-rw-r--r--   0        0        0    48904 2023-06-30 20:45:34.851991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/in_stream.py
+-rw-r--r--   0        0        0    21499 2023-06-30 20:45:34.852990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/out_stream.py
+-rw-r--r--   0        0        0    53479 2023-06-30 20:45:34.852990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/timing.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.411212 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/__init__.py
+-rw-r--r--   0        0        0     7885 2023-06-30 20:45:34.853991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py
+-rw-r--r--   0        0        0     2118 2023-06-30 20:45:34.853991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py
+-rw-r--r--   0        0        0    22198 2023-06-30 20:45:34.854991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py
+-rw-r--r--   0        0        0    42343 2023-06-30 20:45:34.854991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py
+-rw-r--r--   0        0        0    39696 2023-06-30 20:45:34.855991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/start_trigger.py
+-rw-r--r--   0        0        0     3368 2023-06-30 20:45:34.856990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggers.py
+-rw-r--r--   0        0        0    50249 2023-04-03 19:47:30.482012 nidaqmx-0.8.0.dev0/generated/nidaqmx/constants.py
+-rw-r--r--   0        0        0    93605 2023-04-03 19:47:30.466051 nidaqmx-0.8.0.dev0/generated/nidaqmx/error_codes.py
+-rw-r--r--   0        0        0     5869 2023-06-30 20:45:34.856990 nidaqmx-0.8.0.dev0/generated/nidaqmx/errors.py
+-rw-r--r--   0        0        0     3587 2023-06-30 20:45:34.857990 nidaqmx-0.8.0.dev0/generated/nidaqmx/grpc_session_options.py
+-rw-r--r--   0        0        0    22198 2023-06-30 20:45:34.857990 nidaqmx-0.8.0.dev0/generated/nidaqmx/scale.py
+-rw-r--r--   0        0        0   119899 2023-06-30 20:45:34.858991 nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_readers.py
+-rw-r--r--   0        0        0    68185 2023-06-30 20:45:34.859991 nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_writers.py
+-rw-r--r--   0        0        0      426 2023-04-03 18:57:20.415213 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.415213 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/__init__.py
+-rw-r--r--   0        0        0     3579 2023-06-30 20:45:34.860991 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/device_collection.py
+-rw-r--r--   0        0        0     3840 2023-06-30 20:45:34.860991 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_channel_collection.py
+-rw-r--r--   0        0        0     3700 2023-06-30 20:45:34.861989 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_scale_collection.py
+-rw-r--r--   0        0        0     3635 2023-06-30 20:45:34.861989 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_task_collection.py
+-rw-r--r--   0        0        0     7366 2023-06-30 20:45:34.862990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/physical_channel_collection.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.419223 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/__init__.py
+-rw-r--r--   0        0        0     6072 2023-06-30 20:45:34.862990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py
+-rw-r--r--   0        0        0     1473 2023-06-30 20:45:34.863990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py
+-rw-r--r--   0        0        0    39429 2023-06-30 20:45:34.863990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/device.py
+-rw-r--r--   0        0        0    24660 2023-06-30 20:45:34.864990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/physical_channel.py
+-rw-r--r--   0        0        0      275 2023-04-03 18:57:20.420224 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/__init__.py
+-rw-r--r--   0        0        0     3159 2023-06-30 20:45:34.864990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_channel.py
+-rw-r--r--   0        0        0     3426 2023-06-30 20:45:34.865990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_scale.py
+-rw-r--r--   0        0        0     3560 2023-06-30 20:45:34.865990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_task.py
+-rw-r--r--   0        0        0    26836 2023-06-30 20:45:34.866990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/system.py
+-rw-r--r--   0        0        0    16001 2023-06-30 20:45:34.866990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/watchdog.py
+-rw-r--r--   0        0        0    54236 2023-06-30 20:45:34.867990 nidaqmx-0.8.0.dev0/generated/nidaqmx/task.py
+-rw-r--r--   0        0        0     1430 2023-04-03 18:57:20.423214 nidaqmx-0.8.0.dev0/generated/nidaqmx/types.py
+-rw-r--r--   0        0        0     9543 2023-06-30 20:45:34.868989 nidaqmx-0.8.0.dev0/generated/nidaqmx/utils.py
+-rw-r--r--   0        0        0     1213 2022-05-26 20:15:36.274851 nidaqmx-0.8.0.dev0/LICENSE
+-rw-r--r--   0        0        0     5029 2023-06-30 20:45:34.869989 nidaqmx-0.8.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7076 2023-04-05 15:42:42.306919 nidaqmx-0.8.0.dev0/README.rst
+-rw-r--r--   0        0        0     8901 1970-01-01 00:00:00.000000 nidaqmx-0.8.0.dev0/PKG-INFO
```

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/__init__.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/__init__.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_base_interpreter.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_base_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_bitfield_utils.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_bitfield_utils.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_grpc_interpreter.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_grpc_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_lib.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_lib.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_library_interpreter.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2.pyi` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.pyi` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2.pyi` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2_grpc.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_stubs/session_pb2_grpc.pyi` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ai_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ai_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ao_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ao_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/__init__.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ai_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ai_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ao_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ao_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/ci_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ci_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/co_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/co_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/di_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/di_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/channels/do_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/do_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/ci_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ci_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/co_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/co_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/di_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/di_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/do_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/do_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/export_signals.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/export_signals.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/in_stream.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/in_stream.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/out_stream.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/out_stream.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/timing.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/timing.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggering/start_trigger.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/start_trigger.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/_task_modules/triggers.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggers.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/constants.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/constants.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/error_codes.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/error_codes.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/errors.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/errors.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/grpc_session_options.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/scale.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/scale.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/stream_readers.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_readers.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/stream_writers.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_writers.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_collections/device_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/device_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_scale_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_scale_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_collections/persisted_task_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_task_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_collections/physical_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/physical_channel_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/device.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/device.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/physical_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/physical_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_channel.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_scale.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_scale.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/storage/persisted_task.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_task.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/system.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/system.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/system/watchdog.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/watchdog.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/task.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/task.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/types.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/types.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/generated/nidaqmx/utils.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/utils.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/LICENSE` & `nidaqmx-0.8.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/pyproject.toml` & `nidaqmx-0.8.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nidaqmx"
-version = "0.8.0"
+version = "0.8.0-dev0"
 license = "MIT"
 description = "NI-DAQmx Python API"
 authors = ["NI <opensource@ni.com>"]
 maintainers = ["Zach Hindes <zach.hindes@ni.com>", "Maxx Boehme <maxx.boehme@ni.com>"]
 readme = "README.rst"
 repository = "https://github.com/ni/nidaqmx-python"
 documentation = "https://nidaqmx-python.readthedocs.io"
@@ -120,8 +120,8 @@
 [[tool.mypy.overrides]]
 module = [
   "deprecation",
   "grpc.experimental.*",
   "importlib_metadata",
   "mako.*"
 ]
-ignore_missing_imports = true
+ignore_missing_imports = true
```

### Comparing `nidaqmx-0.8.0/README.rst` & `nidaqmx-0.8.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.8.0/PKG-INFO` & `nidaqmx-0.8.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidaqmx
-Version: 0.8.0
+Version: 0.8.0.dev0
 Summary: NI-DAQmx Python API
 Home-page: https://github.com/ni/nidaqmx-python
 License: MIT
 Keywords: nidaqmx,nidaq,daqmx,daq
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: Zach Hindes
```

