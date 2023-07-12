# Comparing `tmp/wireguard4netns-0.1.3.tar.gz` & `tmp/wireguard4netns-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireguard4netns-0.1.3.tar", max compression
+gzip compressed data, was "wireguard4netns-0.1.4.tar", max compression
```

## Comparing `wireguard4netns-0.1.3.tar` & `wireguard4netns-0.1.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0     1078 2022-12-09 15:19:51.836112 wireguard4netns-0.1.3/LICENSE
-drwxr-xr-x   0        0        0        0 2022-12-15 18:10:08.312459 wireguard4netns-0.1.3/LICENSES/
--rw-r--r--   0        0        0      643 2022-12-09 15:19:28.211695 wireguard4netns-0.1.3/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1078 2022-12-09 15:19:24.431628 wireguard4netns-0.1.3/LICENSES/MIT.txt
--rw-r--r--   0        0        0     4635 2023-02-09 15:54:53.762844 wireguard4netns-0.1.3/README.md
--rw-r--r--   0        0        0     4185 2022-12-18 03:55:57.217412 wireguard4netns-0.1.3/build.py
--rw-r--r--   0        0        0    42214 2023-02-10 00:34:43.625563 wireguard4netns-0.1.3/poetry.lock
--rw-r--r--   0        0        0     2516 2023-02-10 00:37:15.841784 wireguard4netns-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      226 2023-02-10 00:37:15.841784 wireguard4netns-0.1.3/src/wireguard4netns/__init__.py
--rw-r--r--   0        0        0      156 2022-12-09 17:59:39.090523 wireguard4netns-0.1.3/src/wireguard4netns/__main__.py
--rw-r--r--   0        0        0      886 2022-12-14 14:34:31.661183 wireguard4netns-0.1.3/src/wireguard4netns/cli.py
--rw-r--r--   0        0        0        0 2022-12-15 19:40:15.176427 wireguard4netns-0.1.3/src/wireguard4netns/py.typed
--rw-r--r--   0        0        0     1819 2022-12-13 16:18:05.542289 wireguard4netns-0.1.3/src/wireguard4netns/tundev.py
--rw-r--r--   0        0        0     1823 2023-02-09 15:56:20.849242 wireguard4netns-0.1.3/src/wireguard4netns/wireguard_daemon.py
--rw-r--r--   0        0        0        0 2022-12-09 14:02:56.423350 wireguard4netns-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      180 2022-12-18 03:37:41.404101 wireguard4netns-0.1.3/tests/test_version.py
--rw-r--r--   0        0        0       13 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/.gitignore
--rw-r--r--   0        0        0     1023 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/LICENSE
--rw-r--r--   0        0        0      827 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/Makefile
--rw-r--r--   0        0        0     3903 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/README.md
--rw-r--r--   0        0        0    11605 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/bind_linux.go
--rw-r--r--   0        0        0     4741 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/bind_std.go
--rw-r--r--   0        0        0    14560 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/bind_windows.go
--rw-r--r--   0        0        0     3041 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/bindtest/bindtest.go
--rw-r--r--   0        0        0      622 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/boundif_android.go
--rw-r--r--   0        0        0     3724 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/conn.go
--rw-r--r--   0        0        0      202 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/default.go
--rw-r--r--   0        0        0      227 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/mark_default.go
--rw-r--r--   0        0        0     1174 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/mark_unix.go
--rw-r--r--   0        0        0     7611 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/conn/winrio/rio_windows.go
--rw-r--r--   0        0        0     6745 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/allowedips.go
--rw-r--r--   0        0        0     2942 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/allowedips_rand_test.go
--rw-r--r--   0        0        0     6174 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/allowedips_test.go
--rw-r--r--   0        0        0     1039 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/bind_test.go
--rw-r--r--   0        0        0     3352 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/channels.go
--rw-r--r--   0        0        0     1233 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/constants.go
--rw-r--r--   0        0        0     4535 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/cookie.go
--rw-r--r--   0        0        0     6076 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/cookie_test.go
--rw-r--r--   0        0        0    13193 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/device.go
--rw-r--r--   0        0        0     9991 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/device_test.go
--rw-r--r--   0        0        0      446 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/devicestate_string.go
--rw-r--r--   0        0        0      992 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/endpoint_test.go
--rw-r--r--   0        0        0     1795 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/indextable.go
--rw-r--r--   0        0        0      380 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/ip.go
--rw-r--r--   0        0        0     2197 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/kdf_test.go
--rw-r--r--   0        0        0     1016 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/keypair.go
--rw-r--r--   0        0        0     1255 2022-12-09 15:26:03.082678 wireguard4netns-0.1.3/wireguard-go/device/logger.go
--rw-r--r--   0        0        0      560 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/mobilequirks.go
--rw-r--r--   0        0        0     2221 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/noise-helpers.go
--rw-r--r--   0        0        0    15067 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/noise-protocol.go
--rw-r--r--   0        0        0     1601 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/noise-types.go
--rw-r--r--   0        0        0     3452 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/noise_test.go
--rw-r--r--   0        0        0     6701 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/peer.go
--rw-r--r--   0        0        0     1912 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/pools.go
--rw-r--r--   0        0        0     1818 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/pools_test.go
--rw-r--r--   0        0        0      383 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/queueconstants_android.go
--rw-r--r--   0        0        0      478 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/queueconstants_default.go
--rw-r--r--   0        0        0      585 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/queueconstants_ios.go
--rw-r--r--   0        0        0      429 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/queueconstants_windows.go
--rw-r--r--   0        0        0      163 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/race_disabled_test.go
--rw-r--r--   0        0        0      161 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/race_enabled_test.go
--rw-r--r--   0        0        0    11836 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/receive.go
--rw-r--r--   0        0        0    12010 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/send.go
--rw-r--r--   0        0        0      227 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/sticky_default.go
--rw-r--r--   0        0        0     5498 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/sticky_linux.go
--rw-r--r--   0        0        0     6932 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/timers.go
--rw-r--r--   0        0        0     1194 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/tun.go
--rw-r--r--   0        0        0    11836 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/device/uapi.go
--rw-r--r--   0        0        0     1025 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/format_test.go
--rw-r--r--   0        0        0      455 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/go.mod
--rw-r--r--   0        0        0     1431 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/go.sum
--rw-r--r--   0        0        0     6523 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/file.go
--rw-r--r--   0        0        0    12765 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/namedpipe.go
--rw-r--r--   0        0        0    13594 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/namedpipe_test.go
--rw-r--r--   0        0        0     2606 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/uapi_bsd.go
--rw-r--r--   0        0        0      299 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/uapi_js.go
--rw-r--r--   0        0        0     2283 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/uapi_linux.go
--rw-r--r--   0        0        0     1428 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/uapi_unix.go
--rw-r--r--   0        0        0     1728 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ipc/uapi_windows.go
--rw-r--r--   0        0        0     6111 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/main.go
--rw-r--r--   0        0        0     2041 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/main_windows.go
--rw-r--r--   0        0        0     2617 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ratelimiter/ratelimiter.go
--rw-r--r--   0        0        0     2558 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/ratelimiter/ratelimiter_test.go
--rw-r--r--   0        0        0     1720 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/replay/replay.go
--rw-r--r--   0        0        0     2805 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/replay/replay_test.go
--rw-r--r--   0        0        0     2248 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/rwcancel/rwcancel.go
--rw-r--r--   0        0        0      130 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/rwcancel/rwcancel_stub.go
--rw-r--r--   0        0        0      858 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/tai64n/tai64n.go
--rw-r--r--   0        0        0     1187 2022-12-09 15:26:03.086679 wireguard4netns-0.1.3/wireguard-go/tai64n/tai64n_test.go
--rwxr-xr-x   0        0        0    18704 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tests/netns.sh
--rw-r--r--   0        0        0     1969 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/alignment_windows_test.go
--rw-r--r--   0        0        0     1181 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/http_client.go
--rw-r--r--   0        0        0     1326 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/http_server.go
--rw-r--r--   0        0        0     1858 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/ping_client.go
--rw-r--r--   0        0        0    25780 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/netstack/tun.go
--rw-r--r--   0        0        0      510 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/operateonfd.go
--rw-r--r--   0        0        0      903 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun.go
--rw-r--r--   0        0        0     6132 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun_darwin.go
--rw-r--r--   0        0        0     9755 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun_freebsd.go
--rw-r--r--   0        0        0    10563 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun_linux.go
--rw-r--r--   0        0        0     5938 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun_openbsd.go
--rw-r--r--   0        0        0     5738 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tun_windows.go
--rw-r--r--   0        0        0     3484 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/tun/tuntest/tuntest.go
--rw-r--r--   0        0        0       45 2022-12-09 15:26:03.090679 wireguard4netns-0.1.3/wireguard-go/version.go
--rw-r--r--   0        0        0     1045 2022-12-09 17:24:15.964340 wireguard4netns-0.1.3/wireguard-go.patch
--rw-r--r--   0        0        0     5765 1970-01-01 00:00:00.000000 wireguard4netns-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/LICENSE
+drwxr-xr-x   0        0        0        0 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/LICENSES/
+-rw-r--r--   0        0        0      643 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1078 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     4757 2023-07-12 21:09:08.880291 wireguard4netns-0.1.4/README.md
+-rw-r--r--   0        0        0     4260 2023-07-12 21:09:08.880291 wireguard4netns-0.1.4/build.py
+-rw-r--r--   0        0        0    44624 2023-07-12 21:16:47.649761 wireguard4netns-0.1.4/poetry.lock
+-rw-r--r--   0        0        0     2521 2023-07-12 21:17:50.115050 wireguard4netns-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-07-12 21:17:50.115050 wireguard4netns-0.1.4/src/wireguard4netns/__init__.py
+-rw-r--r--   0        0        0      156 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/src/wireguard4netns/__main__.py
+-rw-r--r--   0        0        0      886 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/src/wireguard4netns/cli.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/src/wireguard4netns/py.typed
+-rw-r--r--   0        0        0     1819 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/src/wireguard4netns/tundev.py
+-rw-r--r--   0        0        0     1828 2023-07-12 21:09:08.880291 wireguard4netns-0.1.4/src/wireguard4netns/wireguard_daemon.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      180 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/tests/test_version.py
+-rw-r--r--   0        0        0       13 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/.gitignore
+-rw-r--r--   0        0        0     1023 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/LICENSE
+-rw-r--r--   0        0        0      827 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/Makefile
+-rw-r--r--   0        0        0     3903 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/README.md
+-rw-r--r--   0        0        0    11605 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/bind_linux.go
+-rw-r--r--   0        0        0     4741 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/bind_std.go
+-rw-r--r--   0        0        0    14560 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/bind_windows.go
+-rw-r--r--   0        0        0     3041 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/bindtest/bindtest.go
+-rw-r--r--   0        0        0      622 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/boundif_android.go
+-rw-r--r--   0        0        0     3724 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/conn.go
+-rw-r--r--   0        0        0      202 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/default.go
+-rw-r--r--   0        0        0      227 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/mark_default.go
+-rw-r--r--   0        0        0     1174 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/mark_unix.go
+-rw-r--r--   0        0        0     7611 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/conn/winrio/rio_windows.go
+-rw-r--r--   0        0        0     6745 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/allowedips.go
+-rw-r--r--   0        0        0     2942 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/allowedips_rand_test.go
+-rw-r--r--   0        0        0     6174 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/allowedips_test.go
+-rw-r--r--   0        0        0     1039 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/bind_test.go
+-rw-r--r--   0        0        0     3352 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/channels.go
+-rw-r--r--   0        0        0     1233 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/constants.go
+-rw-r--r--   0        0        0     4535 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/cookie.go
+-rw-r--r--   0        0        0     6076 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/cookie_test.go
+-rw-r--r--   0        0        0    13193 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/device.go
+-rw-r--r--   0        0        0     9991 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/device_test.go
+-rw-r--r--   0        0        0      446 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/devicestate_string.go
+-rw-r--r--   0        0        0      992 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/endpoint_test.go
+-rw-r--r--   0        0        0     1795 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/indextable.go
+-rw-r--r--   0        0        0      380 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/ip.go
+-rw-r--r--   0        0        0     2197 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/kdf_test.go
+-rw-r--r--   0        0        0     1016 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/keypair.go
+-rw-r--r--   0        0        0     1255 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/logger.go
+-rw-r--r--   0        0        0      560 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/mobilequirks.go
+-rw-r--r--   0        0        0     2221 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/noise-helpers.go
+-rw-r--r--   0        0        0    15067 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/noise-protocol.go
+-rw-r--r--   0        0        0     1601 2023-07-12 21:11:34.403295 wireguard4netns-0.1.4/wireguard-go/device/noise-types.go
+-rw-r--r--   0        0        0     3452 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/noise_test.go
+-rw-r--r--   0        0        0     6701 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/peer.go
+-rw-r--r--   0        0        0     1912 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/pools.go
+-rw-r--r--   0        0        0     1818 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/pools_test.go
+-rw-r--r--   0        0        0      383 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/queueconstants_android.go
+-rw-r--r--   0        0        0      478 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/queueconstants_default.go
+-rw-r--r--   0        0        0      585 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/queueconstants_ios.go
+-rw-r--r--   0        0        0      429 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/queueconstants_windows.go
+-rw-r--r--   0        0        0      163 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/race_disabled_test.go
+-rw-r--r--   0        0        0      161 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/race_enabled_test.go
+-rw-r--r--   0        0        0    11836 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/receive.go
+-rw-r--r--   0        0        0    12010 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/send.go
+-rw-r--r--   0        0        0      227 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/sticky_default.go
+-rw-r--r--   0        0        0     5498 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/sticky_linux.go
+-rw-r--r--   0        0        0     6932 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/timers.go
+-rw-r--r--   0        0        0     1194 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/tun.go
+-rw-r--r--   0        0        0    11836 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/device/uapi.go
+-rw-r--r--   0        0        0     1025 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/format_test.go
+-rw-r--r--   0        0        0      455 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/go.mod
+-rw-r--r--   0        0        0     1431 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/go.sum
+-rw-r--r--   0        0        0     6523 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/file.go
+-rw-r--r--   0        0        0    12765 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/namedpipe.go
+-rw-r--r--   0        0        0    13594 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/namedpipe_test.go
+-rw-r--r--   0        0        0     2606 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/uapi_bsd.go
+-rw-r--r--   0        0        0      299 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/uapi_js.go
+-rw-r--r--   0        0        0     2283 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/uapi_linux.go
+-rw-r--r--   0        0        0     1428 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/uapi_unix.go
+-rw-r--r--   0        0        0     1728 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ipc/uapi_windows.go
+-rw-r--r--   0        0        0     6111 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/main.go
+-rw-r--r--   0        0        0     2041 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/main_windows.go
+-rw-r--r--   0        0        0     2617 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ratelimiter/ratelimiter.go
+-rw-r--r--   0        0        0     2558 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/ratelimiter/ratelimiter_test.go
+-rw-r--r--   0        0        0     1720 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/replay/replay.go
+-rw-r--r--   0        0        0     2805 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/replay/replay_test.go
+-rw-r--r--   0        0        0     2248 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/rwcancel/rwcancel.go
+-rw-r--r--   0        0        0      130 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/rwcancel/rwcancel_stub.go
+-rw-r--r--   0        0        0      858 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tai64n/tai64n.go
+-rw-r--r--   0        0        0     1187 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tai64n/tai64n_test.go
+-rwxr-xr-x   0        0        0    18704 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tests/netns.sh
+-rw-r--r--   0        0        0     1969 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/alignment_windows_test.go
+-rw-r--r--   0        0        0     1181 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/http_client.go
+-rw-r--r--   0        0        0     1326 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/http_server.go
+-rw-r--r--   0        0        0     1858 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/ping_client.go
+-rw-r--r--   0        0        0    25780 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/netstack/tun.go
+-rw-r--r--   0        0        0      510 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/operateonfd.go
+-rw-r--r--   0        0        0      903 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun.go
+-rw-r--r--   0        0        0     6132 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun_darwin.go
+-rw-r--r--   0        0        0     9755 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun_freebsd.go
+-rw-r--r--   0        0        0    10563 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun_linux.go
+-rw-r--r--   0        0        0     5938 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun_openbsd.go
+-rw-r--r--   0        0        0     5738 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tun_windows.go
+-rw-r--r--   0        0        0     3484 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/tun/tuntest/tuntest.go
+-rw-r--r--   0        0        0       45 2023-07-12 21:11:34.407295 wireguard4netns-0.1.4/wireguard-go/version.go
+-rw-r--r--   0        0        0     1045 2022-12-21 14:10:10.539778 wireguard4netns-0.1.4/wireguard-go.patch
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 wireguard4netns-0.1.4/PKG-INFO
```

### Comparing `wireguard4netns-0.1.3/LICENSE` & `wireguard4netns-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/LICENSES/0BSD.txt` & `wireguard4netns-0.1.4/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/LICENSES/MIT.txt` & `wireguard4netns-0.1.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/README.md` & `wireguard4netns-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,42 +27,47 @@
 root binary helper. However slirp4netns showed the path to an alternative
 approach, create a tuntap interface inside the unprivileged network namespace
 and pass the control socket back to the default namespace where (in our case) a
 userspace WireGuard implementation is started. All frontend traffic is then
 sent through the tunnel to a VPN endpoint on the nearby cloudlet which passes
 it along to the deployed namespace of the application's backend.
 
+
 ## Building from source
 
-Make sure you initialize and update the wireguard-go git-submodule.
+The only executable that is needed is `patch`. The build will try to download a
+copy of golang and use that to build a custom `wireguard-go` binary.
+
+Make sure you have an initialized and updated wireguard-go git-submodule.
 
 ```sh
     git clone ... wireguard4netns
     cd wireguard4netns/
     git submodule update --init
     poetry build
 ```
 
-This will download a copy of golang and build a custom `wireguard-go` binary
-which will be placed at `src/wireguard4netns/wireguard-go`. As long as that
-binary is present it will not try to rebuild the wireguard-go code again.
+The `wireguard-go` binary is then placed at `src/wireguard4netns/wireguard-go`.
+As long as that binary is present in that location, the build will avoid
+rebuilding the wireguard-go code.
 
 We use a custom built version of wireguard-go because starting with an existing
 tunnel socket fd is really just an artifact of how the unmodified wireguard-go
 process sets up the tuntap device and uapi socket in the foreground and then
 daemonizes itself, passing along the already open file descriptors. With our
 approach the tuntap device ends up being created in a different network
-namespace and wireguard-go was unable to query or set the MTU. Our modification
-simply changes the code to not failing when MTU operations are not working and
-is in `wireguard-go.patch`.
+namespace and wireguard-go was unable to query or set the MTU.
+
+Our modifications simply change the code to not fail when MTU operations are
+not working and is in `wireguard-go.patch`.
 
 We also needed to make sure the UAPI socket is placed in a user-writable
-location instead of `/var/run/wireguard`, this `socketDirectory` path is
-customized through a custom linker flag that is set in `build.py` when we
-build the binary.
+location instead of `/var/run/wireguard`. This `socketDirectory` path is
+customized through a custom linker flag that we set in `build.py` at the time
+we build the binary.
 
 
 ## Licenses
 
 wireguard4netns is MIT licensed
 
     Copyright (c) 2022-2023 Carnegie Mellon University
```

### Comparing `wireguard4netns-0.1.3/build.py` & `wireguard4netns-0.1.4/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 #
 # wireguard4netns
 #
-# Copyright (c) 2022 Carnegie Mellon University
+# Copyright (c) 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: MIT
 #
 
 import os
 import shutil
 import subprocess
 import sys
@@ -25,14 +25,15 @@
 
     if dest.exists():
         print(f"{dest} already exists, skipping build")
         return
 
     go = shutil.which("go")
     patch = shutil.which("patch")
+    assert patch is not None, "Could not find the `patch` executable"
 
     # copy wireguard-go source into a temporary directory, patch and compile
     with TemporaryDirectory() as tmp:
         if go is None:
             # fetch + extract go compiler
             print(f"Downloading golang-v{GOLANG_VERSION}")
             stream = urllib.request.urlopen(GOLANG.format(GOLANG_VERSION))
```

### Comparing `wireguard4netns-0.1.3/poetry.lock` & `wireguard4netns-0.1.4/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 description = "Atomic file writes."
 category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 
 [[package]]
 name = "attrs"
-version = "22.2.0"
+version = "23.1.0"
 description = "Classes Without Boilerplate"
 category = "main"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
+
+[package.dependencies]
+importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [package.extras]
-cov = ["attrs[tests]", "coverage-enable-subprocess", "coverage[toml] (>=5.3)"]
-dev = ["attrs[docs,tests]"]
-docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope.interface"]
-tests = ["attrs[tests-no-zope]", "zope.interface"]
-tests-no-zope = ["cloudpickle", "cloudpickle", "hypothesis", "hypothesis", "mypy (>=0.971,<0.990)", "mypy (>=0.971,<0.990)", "pympler", "pympler", "pytest (>=4.3.0)", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-mypy-plugins", "pytest-xdist[psutil]", "pytest-xdist[psutil]"]
+cov = ["attrs[tests]", "coverage[toml] (>=5.3)"]
+dev = ["attrs[docs,tests]", "pre-commit"]
+docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope-interface"]
+tests = ["attrs[tests-no-zope]", "zope-interface"]
+tests-no-zope = ["cloudpickle", "hypothesis", "mypy (>=1.1.1)", "pympler", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-xdist[psutil]"]
 
 [[package]]
 name = "black"
 version = "22.12.0"
 description = "The uncompromising code formatter."
 category = "dev"
 optional = false
@@ -63,15 +66,15 @@
 [package.dependencies]
 colorama = ">=0.4.1,<0.5.0"
 tabulate = ">=0.8.3,<0.9.0"
 unidecode = ">=1.0.23,<2.0.0"
 
 [[package]]
 name = "click"
-version = "8.1.3"
+version = "8.1.4"
 description = "Composable command line interface toolkit"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
@@ -107,55 +110,55 @@
 description = "Pythonic argument parser, that will make you smile"
 category = "dev"
 optional = false
 python-versions = "*"
 
 [[package]]
 name = "filelock"
-version = "3.9.0"
+version = "3.12.2"
 description = "A platform independent file lock."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-testing = ["covdefaults (>=2.2.2)", "coverage (>=7.0.1)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+testing = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "diff-cover (>=7.5)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)", "pytest-timeout (>=2.1)"]
 
 [[package]]
 name = "identify"
-version = "2.5.17"
+version = "2.5.24"
 description = "File identification library for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.extras]
 license = ["ukkonen"]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.0.0"
+version = "6.7.0"
 description = "Read metadata from Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
 typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
 zipp = ">=0.5"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 perf = ["ipython"]
-testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
 name = "importlib-resources"
-version = "5.10.2"
+version = "5.12.0"
 description = "Read resources from Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
 zipp = {version = ">=3.1.0", markers = "python_version < \"3.10\""}
@@ -198,26 +201,26 @@
 description = "Type system extensions for programs checked with the mypy type checker."
 category = "dev"
 optional = false
 python-versions = ">=3.5"
 
 [[package]]
 name = "nodeenv"
-version = "1.7.0"
+version = "1.8.0"
 description = "Node.js virtual environment builder"
 category = "dev"
 optional = false
 python-versions = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*"
 
 [package.dependencies]
 setuptools = "*"
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 description = "Core utilities for Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [[package]]
 name = "pastel"
@@ -225,42 +228,42 @@
 description = "Bring colors to your terminal."
 category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 
 [[package]]
 name = "pathspec"
-version = "0.11.0"
+version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [[package]]
 name = "platformdirs"
-version = "3.0.0"
+version = "3.8.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
-typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
+typing-extensions = {version = ">=4.6.3", markers = "python_version < \"3.8\""}
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
-version = "1.0.0"
+version = "1.2.0"
 description = "plugin and hook calling mechanisms for python"
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 
 [package.dependencies]
 importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
@@ -302,15 +305,15 @@
 description = "library with cross-python path, ini-parsing, io, code, log facilities"
 category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 
 [[package]]
 name = "pyroute2"
-version = "0.7.4"
+version = "0.7.9"
 description = "Python Netlink library"
 category = "main"
 optional = false
 python-versions = "*"
 
 [package.dependencies]
 importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
@@ -336,15 +339,15 @@
 toml = "*"
 
 [package.extras]
 testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "requests", "xmlschema"]
 
 [[package]]
 name = "pytest-mock"
-version = "3.10.0"
+version = "3.11.1"
 description = "Thin-wrapper around the mock package for easier use with pytest"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
 pytest = ">=5.0"
@@ -377,23 +380,23 @@
 description = "QR Code and Micro QR Code generator for Python 2 and Python 3"
 category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
 
 [[package]]
 name = "setuptools"
-version = "67.2.0"
+version = "68.0.0"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
-testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
+testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-ruff", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
 [[package]]
 name = "tabulate"
 version = "0.8.10"
 description = "Pretty-print tabular data"
 category = "dev"
@@ -401,25 +404,25 @@
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 
 [package.extras]
 widechars = ["wcwidth"]
 
 [[package]]
 name = "tbump"
-version = "6.9.0"
+version = "6.10.0"
 description = "Bump software releases"
 category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 
 [package.dependencies]
 cli-ui = ">=0.10.3"
 docopt = ">=0.6.2,<0.7.0"
 schema = ">=0.7.1,<0.8.0"
-tomlkit = ">=0.5.8"
+tomlkit = ">=0.11,<0.12"
 
 [[package]]
 name = "toml"
 version = "0.10.2"
 description = "Python Library for Tom's Obvious, Minimal Language"
 category = "dev"
 optional = false
@@ -431,31 +434,31 @@
 description = "A lil' TOML parser"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [[package]]
 name = "tomlkit"
-version = "0.11.6"
+version = "0.11.8"
 description = "Style preserving TOML library"
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 
 [[package]]
 name = "typed-ast"
-version = "1.5.4"
+version = "1.5.5"
 description = "a fork of Python 2 and 3 ast modules with type comment support"
 category = "dev"
 optional = false
 python-versions = ">=3.6"
 
 [[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 
 [[package]]
 name = "unidecode"
@@ -463,75 +466,75 @@
 description = "ASCII transliterations of Unicode text"
 category = "dev"
 optional = false
 python-versions = ">=3.5"
 
 [[package]]
 name = "virtualenv"
-version = "20.19.0"
+version = "20.23.1"
 description = "Virtual Python Environment builder"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.dependencies]
 distlib = ">=0.3.6,<1"
-filelock = ">=3.4.1,<4"
-importlib-metadata = {version = ">=4.8.3", markers = "python_version < \"3.8\""}
-platformdirs = ">=2.4,<4"
+filelock = ">=3.12,<4"
+importlib-metadata = {version = ">=6.6", markers = "python_version < \"3.8\""}
+platformdirs = ">=3.5.1,<4"
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=22.12)"]
-test = ["covdefaults (>=2.2.2)", "coverage (>=7.1)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23)", "pytest (>=7.2.1)", "pytest-env (>=0.8.1)", "pytest-freezegun (>=0.4.2)", "pytest-mock (>=3.10)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+test = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23.1)", "pytest (>=7.3.1)", "pytest-env (>=0.8.1)", "pytest-freezer (>=0.4.6)", "pytest-mock (>=3.10)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)", "setuptools (>=67.8)", "time-machine (>=2.9)"]
 
 [[package]]
 name = "win-inet-pton"
 version = "1.1.0"
 description = "Native inet_pton and inet_ntop implementation for Python on Windows (with ctypes)."
 category = "main"
 optional = false
 python-versions = "*"
 
 [[package]]
 name = "wireguard-tools"
-version = "0.4.0"
+version = "0.4.4"
 description = "Pure python reimplementation of wireguard-tools"
 category = "main"
 optional = false
 python-versions = ">=3.7,<4.0"
 
 [package.dependencies]
 attrs = ">=22.1.0"
 pyroute2 = ">=0.7.3,<0.8.0"
 segno = ">=1.5.2,<2.0.0"
 
 [[package]]
 name = "zipp"
-version = "3.12.1"
+version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["flake8 (<5)", "func-timeout", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "1.1"
 python-versions = "^3.7"
 content-hash = "df69bda8a448e2dfad8b997564c7f1ada0bae67b976819e3403f0d397db5c0c7"
 
 [metadata.files]
 atomicwrites = [
     {file = "atomicwrites-1.4.1.tar.gz", hash = "sha256:81b2c9071a49367a7f770170e5eec8cb66567cfbbc8c73d20ce5ca4a8d71cf11"},
 ]
 attrs = [
-    {file = "attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
-    {file = "attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
+    {file = "attrs-23.1.0-py3-none-any.whl", hash = "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04"},
+    {file = "attrs-23.1.0.tar.gz", hash = "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"},
 ]
 black = [
     {file = "black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
     {file = "black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
     {file = "black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
     {file = "black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
     {file = "black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
@@ -548,16 +551,16 @@
     {file = "cfgv-3.3.1.tar.gz", hash = "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"},
 ]
 cli-ui = [
     {file = "cli-ui-0.17.2.tar.gz", hash = "sha256:2f67e50cf474e76ad160c3e660bbad98bf8b8dfb8d847765f3a261b7e13c05fa"},
     {file = "cli_ui-0.17.2-py3-none-any.whl", hash = "sha256:6a1ebdbbcd83a0fa06b2f63f4434082a3ba8664aebedd91f1ff86b9e4289d53e"},
 ]
 click = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
+    {file = "click-8.1.4-py3-none-any.whl", hash = "sha256:2739815aaa5d2c986a88f1e9230c55e17f0caad3d958a5e13ad0797c166db9e3"},
+    {file = "click-8.1.4.tar.gz", hash = "sha256:b97d0c74955da062a7d4ef92fadb583806a585b2ea81958a81bd72726cbb8e37"},
 ]
 colorama = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 contextlib2 = [
     {file = "contextlib2-21.6.0-py2.py3-none-any.whl", hash = "sha256:3fbdb64466afd23abaf6c977627b75b6139a5a3e8ce38405c5b413aed7a0471f"},
@@ -567,28 +570,28 @@
     {file = "distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
     {file = "distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
 ]
 docopt = [
     {file = "docopt-0.6.2.tar.gz", hash = "sha256:49b3a825280bd66b3aa83585ef59c4a8c82f2c8a522dbe754a8bc8d08c85c491"},
 ]
 filelock = [
-    {file = "filelock-3.9.0-py3-none-any.whl", hash = "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"},
-    {file = "filelock-3.9.0.tar.gz", hash = "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de"},
+    {file = "filelock-3.12.2-py3-none-any.whl", hash = "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"},
+    {file = "filelock-3.12.2.tar.gz", hash = "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81"},
 ]
 identify = [
-    {file = "identify-2.5.17-py2.py3-none-any.whl", hash = "sha256:7d526dd1283555aafcc91539acc061d8f6f59adb0a7bba462735b0a318bff7ed"},
-    {file = "identify-2.5.17.tar.gz", hash = "sha256:93cc61a861052de9d4c541a7acb7e3dcc9c11b398a2144f6e52ae5285f5f4f06"},
+    {file = "identify-2.5.24-py2.py3-none-any.whl", hash = "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"},
+    {file = "identify-2.5.24.tar.gz", hash = "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4"},
 ]
 importlib-metadata = [
-    {file = "importlib_metadata-6.0.0-py3-none-any.whl", hash = "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad"},
-    {file = "importlib_metadata-6.0.0.tar.gz", hash = "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"},
+    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
+    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
 ]
 importlib-resources = [
-    {file = "importlib_resources-5.10.2-py3-none-any.whl", hash = "sha256:7d543798b0beca10b6a01ac7cafda9f822c54db9e8376a6bf57e0cbd74d486b6"},
-    {file = "importlib_resources-5.10.2.tar.gz", hash = "sha256:e4a96c8cc0339647ff9a5e0550d9f276fc5a01ffa276012b58ec108cfd7b8484"},
+    {file = "importlib_resources-5.12.0-py3-none-any.whl", hash = "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"},
+    {file = "importlib_resources-5.12.0.tar.gz", hash = "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6"},
 ]
 iniconfig = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 mypy = [
     {file = "mypy-0.991-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab"},
@@ -623,60 +626,60 @@
     {file = "mypy-0.991.tar.gz", hash = "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06"},
 ]
 mypy-extensions = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 nodeenv = [
-    {file = "nodeenv-1.7.0-py2.py3-none-any.whl", hash = "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e"},
-    {file = "nodeenv-1.7.0.tar.gz", hash = "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"},
+    {file = "nodeenv-1.8.0-py2.py3-none-any.whl", hash = "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"},
+    {file = "nodeenv-1.8.0.tar.gz", hash = "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2"},
 ]
 packaging = [
-    {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
-    {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
+    {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 pastel = [
     {file = "pastel-0.2.1-py2.py3-none-any.whl", hash = "sha256:4349225fcdf6c2bb34d483e523475de5bb04a5c10ef711263452cb37d7dd4364"},
     {file = "pastel-0.2.1.tar.gz", hash = "sha256:e6581ac04e973cac858828c6202c1e1e81fee1dc7de7683f3e1ffe0bfd8a573d"},
 ]
 pathspec = [
-    {file = "pathspec-0.11.0-py3-none-any.whl", hash = "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229"},
-    {file = "pathspec-0.11.0.tar.gz", hash = "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"},
+    {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
+    {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 platformdirs = [
-    {file = "platformdirs-3.0.0-py3-none-any.whl", hash = "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"},
-    {file = "platformdirs-3.0.0.tar.gz", hash = "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9"},
+    {file = "platformdirs-3.8.1-py3-none-any.whl", hash = "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c"},
+    {file = "platformdirs-3.8.1.tar.gz", hash = "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"},
 ]
 pluggy = [
-    {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
-    {file = "pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
+    {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
+    {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 poethepoet = [
     {file = "poethepoet-0.16.5-py3-none-any.whl", hash = "sha256:493d5d47b4cb0894dde6a69d14129ba39ef3f124fabda1f83ebb39bbf737a40e"},
     {file = "poethepoet-0.16.5.tar.gz", hash = "sha256:3c958792ce488661ba09df67ba832a1b3141aa640236505ee60c23f4b1db4dbc"},
 ]
 pre-commit = [
     {file = "pre_commit-2.21.0-py2.py3-none-any.whl", hash = "sha256:e2f91727039fc39a92f58a588a25b87f936de6567eed4f0e673e0507edc75bad"},
     {file = "pre_commit-2.21.0.tar.gz", hash = "sha256:31ef31af7e474a8d8995027fefdfcf509b5c913ff31f2015b4ec4beb26a6f658"},
 ]
 py = [
     {file = "py-1.11.0-py2.py3-none-any.whl", hash = "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"},
     {file = "py-1.11.0.tar.gz", hash = "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719"},
 ]
 pyroute2 = [
-    {file = "pyroute2-0.7.4-py3-none-any.whl", hash = "sha256:144351f01795499477f9bf58e5c1ed3f3c01059a76e1dd99dce530ee40cac289"},
-    {file = "pyroute2-0.7.4.tar.gz", hash = "sha256:775acefef4d2ace7591e620000bdf383c70c8b7969804870f6c2d8204fa217e0"},
+    {file = "pyroute2-0.7.9-py3-none-any.whl", hash = "sha256:3ef5cfdd18dedf5cb156eac9c63a2e67de4c430ef48c073aac0a911374b3ca89"},
+    {file = "pyroute2-0.7.9.tar.gz", hash = "sha256:b69d82f140b0774317d7ba40f6c5fa1d755098ba3f3eb619982d16e750dc631a"},
 ]
 pytest = [
     {file = "pytest-6.2.5-py3-none-any.whl", hash = "sha256:7310f8d27bc79ced999e760ca304d69f6ba6c6649c0b60fb0e04a4a77cacc134"},
     {file = "pytest-6.2.5.tar.gz", hash = "sha256:131b36680866a76e6781d13f101efb86cf674ebb9762eb70d3082b6f29889e89"},
 ]
 pytest-mock = [
-    {file = "pytest-mock-3.10.0.tar.gz", hash = "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"},
-    {file = "pytest_mock-3.10.0-py3-none-any.whl", hash = "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b"},
+    {file = "pytest-mock-3.11.1.tar.gz", hash = "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"},
+    {file = "pytest_mock-3.11.1-py3-none-any.whl", hash = "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39"},
 ]
 pyyaml = [
     {file = "PyYAML-6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53"},
     {file = "PyYAML-6.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"},
@@ -721,80 +724,97 @@
     {file = "schema-0.7.5.tar.gz", hash = "sha256:f06717112c61895cabc4707752b88716e8420a8819d71404501e114f91043197"},
 ]
 segno = [
     {file = "segno-1.5.2-py2.py3-none-any.whl", hash = "sha256:b17ace8171aad3987e01bb4aeadf7e0450c40674024c4c57b4da54028e55f1e9"},
     {file = "segno-1.5.2.tar.gz", hash = "sha256:983424b296e62189d70fc73460cd946cf56dcbe82b9bda18c066fc1b24371cdc"},
 ]
 setuptools = [
-    {file = "setuptools-67.2.0-py3-none-any.whl", hash = "sha256:16ccf598aab3b506593c17378473978908a2734d7336755a8769b480906bec1c"},
-    {file = "setuptools-67.2.0.tar.gz", hash = "sha256:b440ee5f7e607bb8c9de15259dba2583dd41a38879a7abc1d43a71c59524da48"},
+    {file = "setuptools-68.0.0-py3-none-any.whl", hash = "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f"},
+    {file = "setuptools-68.0.0.tar.gz", hash = "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"},
 ]
 tabulate = [
     {file = "tabulate-0.8.10-py3-none-any.whl", hash = "sha256:0ba055423dbaa164b9e456abe7920c5e8ed33fcc16f6d1b2f2d152c8e1e8b4fc"},
     {file = "tabulate-0.8.10.tar.gz", hash = "sha256:6c57f3f3dd7ac2782770155f3adb2db0b1a269637e42f27599925e64b114f519"},
 ]
 tbump = [
-    {file = "tbump-6.9.0-py3-none-any.whl", hash = "sha256:683eab2e5a4d4861b6928c422d9e51e1d3aeccbbd69d0281fab2c374345e1d9f"},
-    {file = "tbump-6.9.0.tar.gz", hash = "sha256:cf711835b155eaefcf2023ca8963200d893cb40998c9393684df020e6ab1c0b3"},
+    {file = "tbump-6.10.0-py3-none-any.whl", hash = "sha256:170a4395d167daee357cb96af5e874119c470feaba9f605e73f3426e768c2542"},
+    {file = "tbump-6.10.0.tar.gz", hash = "sha256:9ebf5d69bc92ca8be1afb13a80f51e374526cb9988f4c3b167036a9e8a10a684"},
 ]
 toml = [
     {file = "toml-0.10.2-py2.py3-none-any.whl", hash = "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"},
     {file = "toml-0.10.2.tar.gz", hash = "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"},
 ]
 tomli = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 tomlkit = [
-    {file = "tomlkit-0.11.6-py3-none-any.whl", hash = "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b"},
-    {file = "tomlkit-0.11.6.tar.gz", hash = "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"},
+    {file = "tomlkit-0.11.8-py3-none-any.whl", hash = "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171"},
+    {file = "tomlkit-0.11.8.tar.gz", hash = "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"},
 ]
 typed-ast = [
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe"},
-    {file = "typed_ast-1.5.4-cp310-cp310-win_amd64.whl", hash = "sha256:a9916d2bb8865f973824fb47436fa45e1ebf2efd920f2b9f99342cb7fab93f72"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:79b1e0869db7c830ba6a981d58711c88b6677506e648496b1f64ac7d15633aec"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a94d55d142c9265f4ea46fab70977a1944ecae359ae867397757d836ea5a3f47"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-win_amd64.whl", hash = "sha256:639c5f0b21776605dd6c9dbe592d5228f021404dafd377e2b7ac046b0349b1a1"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:cf4afcfac006ece570e32d6fa90ab74a17245b83dfd6655a6f68568098345ff6"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:6778e1b2f81dfc7bc58e4b259363b83d2e509a65198e85d5700dfae4c6c8ff1c"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-win_amd64.whl", hash = "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2efae9db7a8c05ad5547d522e7dbe62c83d838d3906a3716d1478b6c1d61388d"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7d5d014b7daa8b0bf2eaef684295acae12b036d79f54178b92a2b6a56f92278f"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:370788a63915e82fd6f212865a596a0fefcbb7d408bbbb13dea723d971ed8bdc"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:4e964b4ff86550a7a7d56345c7864b18f403f5bd7380edf44a3c1fb4ee7ac6c6"},
-    {file = "typed_ast-1.5.4-cp38-cp38-win_amd64.whl", hash = "sha256:683407d92dc953c8a7347119596f0b0e6c55eb98ebebd9b23437501b28dcbb8e"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4879da6c9b73443f97e731b617184a596ac1235fe91f98d279a7af36c796da35"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3e123d878ba170397916557d31c8f589951e353cc95fb7f24f6bb69adc1a8a97"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebd9d7f80ccf7a82ac5f88c521115cc55d84e35bf8b446fcd7836eb6b98929a3"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
-    {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
-    {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
+    {file = "typed_ast-1.5.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4bc1efe0ce3ffb74784e06460f01a223ac1f6ab31c6bc0376a21184bf5aabe3b"},
+    {file = "typed_ast-1.5.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5f7a8c46a8b333f71abd61d7ab9255440d4a588f34a21f126bbfc95f6049e686"},
+    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:597fc66b4162f959ee6a96b978c0435bd63791e31e4f410622d19f1686d5e769"},
+    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d41b7a686ce653e06c2609075d397ebd5b969d821b9797d029fccd71fdec8e04"},
+    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:5fe83a9a44c4ce67c796a1b466c270c1272e176603d5e06f6afbc101a572859d"},
+    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d5c0c112a74c0e5db2c75882a0adf3133adedcdbfd8cf7c9d6ed77365ab90a1d"},
+    {file = "typed_ast-1.5.5-cp310-cp310-win_amd64.whl", hash = "sha256:e1a976ed4cc2d71bb073e1b2a250892a6e968ff02aa14c1f40eba4f365ffec02"},
+    {file = "typed_ast-1.5.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c631da9710271cb67b08bd3f3813b7af7f4c69c319b75475436fcab8c3d21bee"},
+    {file = "typed_ast-1.5.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b445c2abfecab89a932b20bd8261488d574591173d07827c1eda32c457358b18"},
+    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cc95ffaaab2be3b25eb938779e43f513e0e538a84dd14a5d844b8f2932593d88"},
+    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61443214d9b4c660dcf4b5307f15c12cb30bdfe9588ce6158f4a005baeb167b2"},
+    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6eb936d107e4d474940469e8ec5b380c9b329b5f08b78282d46baeebd3692dc9"},
+    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e48bf27022897577d8479eaed64701ecaf0467182448bd95759883300ca818c8"},
+    {file = "typed_ast-1.5.5-cp311-cp311-win_amd64.whl", hash = "sha256:83509f9324011c9a39faaef0922c6f720f9623afe3fe220b6d0b15638247206b"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:44f214394fc1af23ca6d4e9e744804d890045d1643dd7e8229951e0ef39429b5"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:118c1ce46ce58fda78503eae14b7664163aa735b620b64b5b725453696f2a35c"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be4919b808efa61101456e87f2d4c75b228f4e52618621c77f1ddcaae15904fa"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:fc2b8c4e1bc5cd96c1a823a885e6b158f8451cf6f5530e1829390b4d27d0807f"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:16f7313e0a08c7de57f2998c85e2a69a642e97cb32f87eb65fbfe88381a5e44d"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-win_amd64.whl", hash = "sha256:2b946ef8c04f77230489f75b4b5a4a6f24c078be4aed241cfabe9cbf4156e7e5"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2188bc33d85951ea4ddad55d2b35598b2709d122c11c75cffd529fbc9965508e"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0635900d16ae133cab3b26c607586131269f88266954eb04ec31535c9a12ef1e"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57bfc3cf35a0f2fdf0a88a3044aafaec1d2f24d8ae8cd87c4f58d615fb5b6311"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:fe58ef6a764de7b4b36edfc8592641f56e69b7163bba9f9c8089838ee596bfb2"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d09d930c2d1d621f717bb217bf1fe2584616febb5138d9b3e8cdd26506c3f6d4"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-win_amd64.whl", hash = "sha256:d40c10326893ecab8a80a53039164a224984339b2c32a6baf55ecbd5b1df6431"},
+    {file = "typed_ast-1.5.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:fd946abf3c31fb50eee07451a6aedbfff912fcd13cf357363f5b4e834cc5e71a"},
+    {file = "typed_ast-1.5.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ed4a1a42df8a3dfb6b40c3d2de109e935949f2f66b19703eafade03173f8f437"},
+    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:045f9930a1550d9352464e5149710d56a2aed23a2ffe78946478f7b5416f1ede"},
+    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:381eed9c95484ceef5ced626355fdc0765ab51d8553fec08661dce654a935db4"},
+    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bfd39a41c0ef6f31684daff53befddae608f9daf6957140228a08e51f312d7e6"},
+    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8c524eb3024edcc04e288db9541fe1f438f82d281e591c548903d5b77ad1ddd4"},
+    {file = "typed_ast-1.5.5-cp38-cp38-win_amd64.whl", hash = "sha256:7f58fabdde8dcbe764cef5e1a7fcb440f2463c1bbbec1cf2a86ca7bc1f95184b"},
+    {file = "typed_ast-1.5.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:042eb665ff6bf020dd2243307d11ed626306b82812aba21836096d229fdc6a10"},
+    {file = "typed_ast-1.5.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:622e4a006472b05cf6ef7f9f2636edc51bda670b7bbffa18d26b255269d3d814"},
+    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1efebbbf4604ad1283e963e8915daa240cb4bf5067053cf2f0baadc4d4fb51b8"},
+    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0aefdd66f1784c58f65b502b6cf8b121544680456d1cebbd300c2c813899274"},
+    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:48074261a842acf825af1968cd912f6f21357316080ebaca5f19abbb11690c8a"},
+    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:429ae404f69dc94b9361bb62291885894b7c6fb4640d561179548c849f8492ba"},
+    {file = "typed_ast-1.5.5-cp39-cp39-win_amd64.whl", hash = "sha256:335f22ccb244da2b5c296e6f96b06ee9bed46526db0de38d2f0e5a6597b81155"},
+    {file = "typed_ast-1.5.5.tar.gz", hash = "sha256:94282f7a354f36ef5dbce0ef3467ebf6a258e370ab33d5b40c249fa996e590dd"},
 ]
 typing-extensions = [
-    {file = "typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {file = "typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 unidecode = [
     {file = "Unidecode-1.3.6-py3-none-any.whl", hash = "sha256:547d7c479e4f377b430dd91ac1275d593308dce0fc464fb2ab7d41f82ec653be"},
     {file = "Unidecode-1.3.6.tar.gz", hash = "sha256:fed09cf0be8cf415b391642c2a5addfc72194407caee4f98719e40ec2a72b830"},
 ]
 virtualenv = [
-    {file = "virtualenv-20.19.0-py3-none-any.whl", hash = "sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1"},
-    {file = "virtualenv-20.19.0.tar.gz", hash = "sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590"},
+    {file = "virtualenv-20.23.1-py3-none-any.whl", hash = "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419"},
+    {file = "virtualenv-20.23.1.tar.gz", hash = "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"},
 ]
 win-inet-pton = [
     {file = "win_inet_pton-1.1.0-py2.py3-none-any.whl", hash = "sha256:eaf0193cbe7152ac313598a0da7313fb479f769343c0c16c5308f64887dc885b"},
     {file = "win_inet_pton-1.1.0.tar.gz", hash = "sha256:dd03d942c0d3e2b1cf8bab511844546dfa5f74cb61b241699fa379ad707dea4f"},
 ]
 wireguard-tools = [
-    {file = "wireguard_tools-0.4.0-py3-none-any.whl", hash = "sha256:49274b9498adffe5568413c78ecdf939c5d96f7977eabbc9358b914b80dcf0e3"},
-    {file = "wireguard_tools-0.4.0.tar.gz", hash = "sha256:6f99e0b8cb36e9853d2116bb257434831877fb36b5f1cf85a3cc3be0f4e50248"},
+    {file = "wireguard_tools-0.4.4-py3-none-any.whl", hash = "sha256:e56f906128111ac83ba75850530a754abe01afc8ffd83431c51668a3870b7005"},
+    {file = "wireguard_tools-0.4.4.tar.gz", hash = "sha256:94938a82b9a647f3bb3a98101c3818cdc9c75a7bae293ae169232ecb85ddb11b"},
 ]
 zipp = [
-    {file = "zipp-3.12.1-py3-none-any.whl", hash = "sha256:6c4fe274b8f85ec73c37a8e4e3fa00df9fb9335da96fb789e3b96b318e5097b3"},
-    {file = "zipp-3.12.1.tar.gz", hash = "sha256:a3cac813d40993596b39ea9e93a18e8a2076d5c378b8bc88ec32ab264e04ad02"},
+    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
+    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
```

### Comparing `wireguard4netns-0.1.3/pyproject.toml` & `wireguard4netns-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# SPDX-FileCopyrightText: 2022 Carnegie Mellon University
+# SPDX-FileCopyrightText: 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "wireguard4netns"
-version = "0.1.3"
+version = "0.1.4"
 description = "WireGuard VPN networking for unprivileged network namespaces"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `wireguard4netns-0.1.3/src/wireguard4netns/cli.py` & `wireguard4netns-0.1.4/src/wireguard4netns/cli.py`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/src/wireguard4netns/tundev.py` & `wireguard4netns-0.1.4/src/wireguard4netns/tundev.py`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/src/wireguard4netns/wireguard_daemon.py` & `wireguard4netns-0.1.4/src/wireguard4netns/wireguard_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # wireguard4netns
 #
-# Copyright (c) 2022 Carnegie Mellon University
+# Copyright (c) 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: MIT
 #
 """Fork wireguard-go process and configure the tunnel"""
 
 from __future__ import annotations
 
 import os
```

### Comparing `wireguard4netns-0.1.3/wireguard-go/LICENSE` & `wireguard4netns-0.1.4/wireguard-go/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/Makefile` & `wireguard4netns-0.1.4/wireguard-go/Makefile`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/README.md` & `wireguard4netns-0.1.4/wireguard-go/README.md`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/bind_linux.go` & `wireguard4netns-0.1.4/wireguard-go/conn/bind_linux.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/bind_std.go` & `wireguard4netns-0.1.4/wireguard-go/conn/bind_std.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/bind_windows.go` & `wireguard4netns-0.1.4/wireguard-go/conn/bind_windows.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/bindtest/bindtest.go` & `wireguard4netns-0.1.4/wireguard-go/conn/bindtest/bindtest.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/boundif_android.go` & `wireguard4netns-0.1.4/wireguard-go/conn/boundif_android.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/conn.go` & `wireguard4netns-0.1.4/wireguard-go/conn/conn.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/mark_unix.go` & `wireguard4netns-0.1.4/wireguard-go/conn/mark_unix.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/conn/winrio/rio_windows.go` & `wireguard4netns-0.1.4/wireguard-go/conn/winrio/rio_windows.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/allowedips.go` & `wireguard4netns-0.1.4/wireguard-go/device/allowedips.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/allowedips_rand_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/allowedips_rand_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/allowedips_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/allowedips_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/bind_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/bind_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/channels.go` & `wireguard4netns-0.1.4/wireguard-go/device/channels.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/constants.go` & `wireguard4netns-0.1.4/wireguard-go/device/constants.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/cookie.go` & `wireguard4netns-0.1.4/wireguard-go/device/cookie.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/cookie_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/cookie_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/device.go` & `wireguard4netns-0.1.4/wireguard-go/device/device.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/device_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/device_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/endpoint_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/endpoint_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/indextable.go` & `wireguard4netns-0.1.4/wireguard-go/device/indextable.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/kdf_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/kdf_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/keypair.go` & `wireguard4netns-0.1.4/wireguard-go/device/keypair.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/logger.go` & `wireguard4netns-0.1.4/wireguard-go/device/logger.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/mobilequirks.go` & `wireguard4netns-0.1.4/wireguard-go/device/mobilequirks.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/noise-helpers.go` & `wireguard4netns-0.1.4/wireguard-go/device/noise-helpers.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/noise-protocol.go` & `wireguard4netns-0.1.4/wireguard-go/device/noise-protocol.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/noise-types.go` & `wireguard4netns-0.1.4/wireguard-go/device/noise-types.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/noise_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/noise_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/peer.go` & `wireguard4netns-0.1.4/wireguard-go/device/peer.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/pools.go` & `wireguard4netns-0.1.4/wireguard-go/device/pools.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/pools_test.go` & `wireguard4netns-0.1.4/wireguard-go/device/pools_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/queueconstants_ios.go` & `wireguard4netns-0.1.4/wireguard-go/device/queueconstants_ios.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/receive.go` & `wireguard4netns-0.1.4/wireguard-go/device/receive.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/send.go` & `wireguard4netns-0.1.4/wireguard-go/device/send.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/sticky_linux.go` & `wireguard4netns-0.1.4/wireguard-go/device/sticky_linux.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/timers.go` & `wireguard4netns-0.1.4/wireguard-go/device/timers.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/tun.go` & `wireguard4netns-0.1.4/wireguard-go/device/tun.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/device/uapi.go` & `wireguard4netns-0.1.4/wireguard-go/device/uapi.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/format_test.go` & `wireguard4netns-0.1.4/wireguard-go/format_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/go.sum` & `wireguard4netns-0.1.4/wireguard-go/go.sum`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/file.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/file.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/namedpipe.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/namedpipe.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/namedpipe/namedpipe_test.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/namedpipe/namedpipe_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/uapi_bsd.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/uapi_bsd.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/uapi_linux.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/uapi_linux.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/uapi_unix.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/uapi_unix.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ipc/uapi_windows.go` & `wireguard4netns-0.1.4/wireguard-go/ipc/uapi_windows.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/main.go` & `wireguard4netns-0.1.4/wireguard-go/main.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/main_windows.go` & `wireguard4netns-0.1.4/wireguard-go/main_windows.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ratelimiter/ratelimiter.go` & `wireguard4netns-0.1.4/wireguard-go/ratelimiter/ratelimiter.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/ratelimiter/ratelimiter_test.go` & `wireguard4netns-0.1.4/wireguard-go/ratelimiter/ratelimiter_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/replay/replay.go` & `wireguard4netns-0.1.4/wireguard-go/replay/replay.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/replay/replay_test.go` & `wireguard4netns-0.1.4/wireguard-go/replay/replay_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/rwcancel/rwcancel.go` & `wireguard4netns-0.1.4/wireguard-go/rwcancel/rwcancel.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tai64n/tai64n.go` & `wireguard4netns-0.1.4/wireguard-go/tai64n/tai64n.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tai64n/tai64n_test.go` & `wireguard4netns-0.1.4/wireguard-go/tai64n/tai64n_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tests/netns.sh` & `wireguard4netns-0.1.4/wireguard-go/tests/netns.sh`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/alignment_windows_test.go` & `wireguard4netns-0.1.4/wireguard-go/tun/alignment_windows_test.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/http_client.go` & `wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/http_client.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/http_server.go` & `wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/http_server.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/netstack/examples/ping_client.go` & `wireguard4netns-0.1.4/wireguard-go/tun/netstack/examples/ping_client.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/netstack/tun.go` & `wireguard4netns-0.1.4/wireguard-go/tun/netstack/tun.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun_darwin.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun_darwin.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun_freebsd.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun_freebsd.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun_linux.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun_linux.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun_openbsd.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun_openbsd.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tun_windows.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tun_windows.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go/tun/tuntest/tuntest.go` & `wireguard4netns-0.1.4/wireguard-go/tun/tuntest/tuntest.go`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/wireguard-go.patch` & `wireguard4netns-0.1.4/wireguard-go.patch`

 * *Files identical despite different names*

### Comparing `wireguard4netns-0.1.3/PKG-INFO` & `wireguard4netns-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireguard4netns
-Version: 0.1.3
+Version: 0.1.4
 Summary: WireGuard VPN networking for unprivileged network namespaces
 Home-page: https://github.com/cmusatyalab/wireguard4netns
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -54,42 +54,47 @@
 root binary helper. However slirp4netns showed the path to an alternative
 approach, create a tuntap interface inside the unprivileged network namespace
 and pass the control socket back to the default namespace where (in our case) a
 userspace WireGuard implementation is started. All frontend traffic is then
 sent through the tunnel to a VPN endpoint on the nearby cloudlet which passes
 it along to the deployed namespace of the application's backend.
 
+
 ## Building from source
 
-Make sure you initialize and update the wireguard-go git-submodule.
+The only executable that is needed is `patch`. The build will try to download a
+copy of golang and use that to build a custom `wireguard-go` binary.
+
+Make sure you have an initialized and updated wireguard-go git-submodule.
 
 ```sh
     git clone ... wireguard4netns
     cd wireguard4netns/
     git submodule update --init
     poetry build
 ```
 
-This will download a copy of golang and build a custom `wireguard-go` binary
-which will be placed at `src/wireguard4netns/wireguard-go`. As long as that
-binary is present it will not try to rebuild the wireguard-go code again.
+The `wireguard-go` binary is then placed at `src/wireguard4netns/wireguard-go`.
+As long as that binary is present in that location, the build will avoid
+rebuilding the wireguard-go code.
 
 We use a custom built version of wireguard-go because starting with an existing
 tunnel socket fd is really just an artifact of how the unmodified wireguard-go
 process sets up the tuntap device and uapi socket in the foreground and then
 daemonizes itself, passing along the already open file descriptors. With our
 approach the tuntap device ends up being created in a different network
-namespace and wireguard-go was unable to query or set the MTU. Our modification
-simply changes the code to not failing when MTU operations are not working and
-is in `wireguard-go.patch`.
+namespace and wireguard-go was unable to query or set the MTU.
+
+Our modifications simply change the code to not fail when MTU operations are
+not working and is in `wireguard-go.patch`.
 
 We also needed to make sure the UAPI socket is placed in a user-writable
-location instead of `/var/run/wireguard`, this `socketDirectory` path is
-customized through a custom linker flag that is set in `build.py` when we
-build the binary.
+location instead of `/var/run/wireguard`. This `socketDirectory` path is
+customized through a custom linker flag that we set in `build.py` at the time
+we build the binary.
 
 
 ## Licenses
 
 wireguard4netns is MIT licensed
 
     Copyright (c) 2022-2023 Carnegie Mellon University
```

