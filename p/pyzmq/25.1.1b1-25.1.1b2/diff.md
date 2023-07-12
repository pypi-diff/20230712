# Comparing `tmp/pyzmq-25.1.1b1.tar.gz` & `tmp/pyzmq-25.1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzmq-25.1.1b1.tar", last modified: Wed May 31 11:36:34 2023, max compression
+gzip compressed data, was "pyzmq-25.1.1b2.tar", last modified: Wed Jul 12 05:02:08 2023, max compression
```

## Comparing `pyzmq-25.1.1b1.tar` & `pyzmq-25.1.1b2.tar`

### file list

```diff
@@ -1,689 +1,690 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.086069 pyzmq-25.1.1b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.mailmap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/.obs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.obs/workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/LICENSE.BSD
--rw-r--r--   0 runner    (1001) docker     (123)    36008 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-31 11:36:34.086069 pyzmq-25.1.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/RELICENSE/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/chrislaws.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/ellisonbg.md
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/frankwiles.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/juliantaylor.md
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/ledgerx.md
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/lothiraldan.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/minrk.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/takluyver.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/RELICENSE/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-bsd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-mplv2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/buildutils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/_cffi.c
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/build_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/check_sys_un.c
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/dummy.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.014068 pyzmq-25.1.1b1/buildutils/include_darwin/
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_darwin/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/include_freebsd/
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_freebsd/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/include_linux/
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_linux/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/include_linux-armv/
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_linux-armv/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/include_linux-musl/
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_linux-musl/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/include_win32/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_win32/platform.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/include_win32/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/initlibzmq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/buildutils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/templates/constant_enums.pxi
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/templates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/buildutils/vers.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:33.994067 pyzmq-25.1.1b1/bundled/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/bundled/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:33.994067 pyzmq-25.1.1b1/bundled/zeromq/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67905 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/wepoll.c
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/wepoll.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.018068 pyzmq-25.1.1b1/bundled/zeromq/include/
--rw-r--r--   0 runner    (1001) docker     (123)    30485 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/include/zmq.h
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/include/zmq_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.050068 pyzmq-25.1.1b1/bundled/zeromq/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/array.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/atomic_counter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/atomic_ptr.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/blob.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/channel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/channel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/client.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/clock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/clock.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/command.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/compat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/condition_variable.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/config.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ctx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ctx.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_client.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_client_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/curve_server.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dbuffer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dealer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dealer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/decoder_allocators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/decoder_allocators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/devpoll.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/devpoll.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dgram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dgram.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dish.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dish.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/dist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/endpoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/endpoint.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/epoll.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/epoll.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/err.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/err.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/fd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/fq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/fq.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gather.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gather.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/generic_mtrie.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25261 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/generic_mtrie_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_client.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_server.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/i_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/i_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/i_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/i_mailbox.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/i_poll_events.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/io_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/io_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/io_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/io_thread.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ip.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ip.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ip_resolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ip_resolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ipc_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/kqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/kqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/lb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/lb.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/libzmq.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/libzmq.vers
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/likely.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mailbox.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mailbox.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mailbox_safe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mailbox_safe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mechanism.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mechanism.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/metadata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/metadata.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/msg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/msg.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mtrie.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mtrie.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/mutex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/norm_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/norm_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/null_mechanism.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/null_mechanism.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    38451 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/own.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/own.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pair.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pair.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/peer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/peer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_receiver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_receiver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_sender.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_sender.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_socket.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pgm_socket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17813 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pipe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pipe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/plain_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/plain_client.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/plain_common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/plain_server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/plain_server.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/platform.hpp.in
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/poll.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/poll.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/poller.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/poller_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/poller_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/polling_util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/polling_util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pollset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pollset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/precompiled.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/precompiled.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/proxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pub.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pub.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pull.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/pull.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/push.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/push.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/radio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/radio.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/radix_tree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/radix_tree.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/random.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/raw_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/reaper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/reaper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/rep.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/rep.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/req.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/req.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/router.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/router.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/scatter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/scatter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/secure_allocator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/select.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/select.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/server.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24036 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/session_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/session_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/signaler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/signaler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    69471 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socket_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socket_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socket_poller.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socket_poller.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socks.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socks_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/socks_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stdint.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_connecter_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_connecter_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_engine_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_engine_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_listener_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/stream_listener_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/sub.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/sub.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tcp_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/thread.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/timers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/timers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tipc_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/trie.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/trie.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tweetnacl.c
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/tweetnacl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/udp_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/udp_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17943 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/udp_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/udp_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v1_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v1_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v1_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v1_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v2_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v2_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v2_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v2_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v2_protocol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v3_1_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/v3_1_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/version.rc.in
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/vmci_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/windows.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/wire.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ws_protocol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/wss_address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/wss_address.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/wss_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/wss_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/xpub.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/xpub.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/xsub.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/xsub.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ypipe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ypipe_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/ypipe_conflate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/yqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zap_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zap_client.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    43610 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zmq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zmq_draft.h
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zmq_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zmtp_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/bundled/zeromq/src/zmtp_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.054068 pyzmq-25.1.1b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/autogen_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.054068 pyzmq-25.1.1b1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.054068 pyzmq-25.1.1b1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/_static/zeromq.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.054068 pyzmq-25.1.1b1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.auth.asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.auth.ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.auth.thread.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.eventloop.future.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.eventloop.ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.eventloop.zmqstream.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.green.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.log.handlers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.ssh.tunnel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.utils.jsonapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.utils.monitor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.utils.win32.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/api/zmq.utils.z85.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38453 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.054068 pyzmq-25.1.1b1/docs/source/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/devices.md
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/draft.md
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/eventloop.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/logging.md
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/morethanbindings.md
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/serialization.md
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/howto/ssh.md
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/docs/source/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/notes/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/notes/pyversions.md
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/docs/source/notes/unicode.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/asyncio/coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/asyncio/helloworld_pubsub_dealerrouter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/asyncio/router_router.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/asyncio/tornado_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/chat/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/chat/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/cython/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/cython/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/cython/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/cython/cyzmq.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/cython/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/device/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/draft/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/draft/client-server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/draft/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/draft/radio-dish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/eventloop/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/eventloop/asyncweb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/eventloop/coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/eventloop/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/eventloop/echofuture.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/eventloop/echostream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/gevent/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/gevent/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/gevent/reqrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/gevent/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/heartbeat/heart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/heartbeat/heartbeater.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/heartbeat/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/heartbeat/pong.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/logger/zmqlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.058069 pyzmq-25.1.1b1/examples/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/mongodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/mongodb/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/monitoring/simple_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/monitoring/zmq_monitor_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/poll/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/poll/pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/poll/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/poll/reqrep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/pubsub/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/pubsub/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/pubsub/subscriber.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/pubsub/topics_pub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/pubsub/topics_sub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/security/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/asyncio-ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/generate_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/grasslands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/ioloop-ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/stonehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/strawhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/security/woodhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/serialization/serialsocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/examples/win32-interrupt/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/win32-interrupt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/examples/win32-interrupt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/mypy_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/mypy_tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/mypy_tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/mypy_tests/test_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.002067 pyzmq-25.1.1b1/packaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/packaging/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/pyzmq.dsc.obs
--rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/packaging/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/packaging/obs/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/obs/_service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.062069 pyzmq-25.1.1b1/packaging/redhat/
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/packaging/redhat/python-pyzmq.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/perf/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/perf/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/perf/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/perf/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)   167790 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/perf/perf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/perf/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/pyzmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/pyzmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/pyzmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/pyzmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:36:21.000000 pyzmq-25.1.1b1/pyzmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/pyzmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/pyzmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:36:34.086069 pyzmq-25.1.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/setup.cfg.android
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/setup.cfg.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    46521 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/backend_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/install_libzmq.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/run_with_env.cmd
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/showvcvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/test_sdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/test_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/tools/wheel-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/zmq/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/auth/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.066069 pyzmq-25.1.1b1/zmq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.070069 pyzmq-25.1.1b1/zmq/backend/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/_cdefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cffi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.074069 pyzmq-25.1.1b1/zmq/backend/cython/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   235785 2023-05-31 11:36:19.000000 pyzmq-25.1.1b1/zmq/backend/cython/_device.c
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/_device.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   301006 2023-05-31 11:36:19.000000 pyzmq-25.1.1b1/zmq/backend/cython/_poll.c
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/_poll.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   221323 2023-05-31 11:36:19.000000 pyzmq-25.1.1b1/zmq/backend/cython/_proxy_steerable.c
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/_proxy_steerable.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   141259 2023-05-31 11:36:20.000000 pyzmq-25.1.1b1/zmq/backend/cython/_version.c
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/_version.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/checkrc.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/constant_enums.pxi
--rw-r--r--   0 runner    (1001) docker     (123)   288736 2023-05-31 11:36:20.000000 pyzmq-25.1.1b1/zmq/backend/cython/context.c
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/context.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/context.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   147308 2023-05-31 11:36:20.000000 pyzmq-25.1.1b1/zmq/backend/cython/error.c
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/error.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/libzmq.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   469218 2023-05-31 11:36:20.000000 pyzmq-25.1.1b1/zmq/backend/cython/message.c
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/message.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/message.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   655194 2023-05-31 11:36:21.000000 pyzmq-25.1.1b1/zmq/backend/cython/socket.c
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/socket.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/socket.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   190998 2023-05-31 11:36:21.000000 pyzmq-25.1.1b1/zmq/backend/cython/utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/cython/utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/backend/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)   293507 2023-05-31 11:36:21.000000 pyzmq-25.1.1b1/zmq/devices/monitoredqueue.c
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/monitoredqueue.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/monitoredqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/monitoredqueue.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/monitoredqueuedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/proxydevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/devices/proxysteerabledevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/eventloop/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/eventloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/eventloop/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/eventloop/future.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/eventloop/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/eventloop/zmqstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/green/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/green/eventloop/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/eventloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/eventloop/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/eventloop/zmqstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/green/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/log/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/log/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/ssh/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/ssh/tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.078069 pyzmq-25.1.1b1/zmq/sugar/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/attrsettr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/sugar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.082069 pyzmq-25.1.1b1/zmq/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/cython_ext.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_cffi_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_cython.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_draft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_etc.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_ioloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_monqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_proxy_steerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_reqrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_retry_eintr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    23610 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_win32_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_z85.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/tests/test_zmqstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:34.086069 pyzmq-25.1.1b1/zmq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/buffers.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/zmq/utils/compiler.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 11:36:33.000000 pyzmq-25.1.1b1/zmq/utils/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/garbage.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/getpid_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/ipcmaxlen.h
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/jsonapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/pyversion_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/strtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/win32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/z85.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmq/utils/zmq_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-31 11:36:02.000000 pyzmq-25.1.1b1/zmqversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.582718 pyzmq-25.1.1b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.mailmap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/.obs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.obs/workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/LICENSE.BSD
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-12 05:02:08.582718 pyzmq-25.1.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.486712 pyzmq-25.1.1b2/RELICENSE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/chrislaws.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/ellisonbg.md
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/frankwiles.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/juliantaylor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/ledgerx.md
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/lothiraldan.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/minrk.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/takluyver.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/RELICENSE/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-mplv2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/_cffi.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/check_sys_un.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/dummy.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_darwin/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_freebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_freebsd/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_linux/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_linux-armv/
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_linux-armv/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_linux-musl/
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_linux-musl/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/include_win32/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_win32/platform.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/include_win32/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/initlibzmq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/buildutils/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/templates/constant_enums.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/templates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/buildutils/vers.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.478711 pyzmq-25.1.1b2/bundled/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.490712 pyzmq-25.1.1b2/bundled/zeromq/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/COPYING.LESSER
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.478711 pyzmq-25.1.1b2/bundled/zeromq/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.494712 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67905 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/wepoll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/wepoll.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.494712 pyzmq-25.1.1b2/bundled/zeromq/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    30485 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/include/zmq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/include/zmq_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.530715 pyzmq-25.1.1b2/bundled/zeromq/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/array.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/atomic_counter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/atomic_ptr.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/blob.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/channel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/channel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/clock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/clock.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/command.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/compat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/condition_variable.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ctx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ctx.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_client_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/curve_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dbuffer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dealer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dealer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/decoder_allocators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/decoder_allocators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/devpoll.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/devpoll.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dgram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dgram.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dish.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dish.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/dist.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/endpoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/endpoint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/epoll.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/epoll.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/err.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/err.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/fd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/fq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/fq.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gather.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gather.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/generic_mtrie.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25261 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/generic_mtrie_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/i_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/i_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/i_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/i_mailbox.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/i_poll_events.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/io_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/io_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/io_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/io_thread.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ip.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ip.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ip_resolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ip_resolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ipc_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/kqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/kqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/lb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/lb.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/libzmq.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/libzmq.vers
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/likely.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mailbox.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mailbox.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mailbox_safe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mailbox_safe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mechanism.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mechanism.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/metadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/metadata.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/msg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/msg.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mtrie.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mtrie.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/mutex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/norm_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/norm_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/null_mechanism.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/null_mechanism.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38451 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/own.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/own.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pair.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pair.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/peer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/peer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_receiver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_receiver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_sender.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_sender.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_socket.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pgm_socket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17813 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pipe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pipe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/plain_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/plain_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/plain_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/plain_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/plain_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/platform.hpp.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/poll.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/poll.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/poller.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/poller_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/poller_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/polling_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/polling_util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pollset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pollset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/precompiled.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/precompiled.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/proxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/proxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pub.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pub.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pull.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/pull.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/push.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/push.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/radio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/radio.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/radix_tree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/radix_tree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/random.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/raw_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/reaper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/reaper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/rep.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/rep.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/req.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/req.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/router.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/router.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/scatter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/scatter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/secure_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/select.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/select.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/server.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/server.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24036 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/session_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/session_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/signaler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/signaler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    69471 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socket_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socket_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socket_poller.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socket_poller.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socks.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socks_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/socks_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stdint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_connecter_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_connecter_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_engine_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_engine_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_listener_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/stream_listener_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/sub.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/sub.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tcp_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/thread.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/timers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/timers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tipc_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/trie.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/trie.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tweetnacl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/tweetnacl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/udp_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/udp_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17943 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/udp_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/udp_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v1_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v1_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v1_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v1_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v2_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v2_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v2_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v2_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v2_protocol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v3_1_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/v3_1_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/version.rc.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/vmci_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/windows.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/wire.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ws_protocol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/wss_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/wss_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/wss_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/wss_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/xpub.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/xpub.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/xsub.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/xsub.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ypipe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ypipe_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/ypipe_conflate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/yqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zap_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zap_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43610 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zmq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zmq_draft.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zmq_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zmtp_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/bundled/zeromq/src/zmtp_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.530715 pyzmq-25.1.1b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/autogen_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.534715 pyzmq-25.1.1b2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.534715 pyzmq-25.1.1b2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/_static/zeromq.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.534715 pyzmq-25.1.1b2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.auth.asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.auth.ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.auth.thread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.eventloop.future.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.eventloop.ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.eventloop.zmqstream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.green.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.log.handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.ssh.tunnel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.utils.jsonapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.utils.monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.utils.win32.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/api/zmq.utils.z85.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38453 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.534715 pyzmq-25.1.1b2/docs/source/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/devices.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/draft.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/eventloop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/logging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/morethanbindings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/serialization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/howto/ssh.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/docs/source/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/notes/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/notes/pyversions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/docs/source/notes/unicode.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/asyncio/coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/asyncio/helloworld_pubsub_dealerrouter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/asyncio/router_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/asyncio/tornado_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/chat/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/chat/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/cython/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/cython/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/cython/cyzmq.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/cython/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/device/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/draft/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/draft/client-server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/draft/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/draft/radio-dish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/eventloop/asyncweb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/eventloop/coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/eventloop/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/eventloop/echofuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/eventloop/echostream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/gevent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/gevent/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/gevent/reqrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/gevent/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/heartbeat/heart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/heartbeat/heartbeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/heartbeat/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/heartbeat/pong.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/logger/zmqlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.538715 pyzmq-25.1.1b2/examples/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/mongodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/mongodb/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/monitoring/simple_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/monitoring/zmq_monitor_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/poll/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/poll/pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/poll/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/poll/reqrep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/pubsub/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/pubsub/subscriber.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/pubsub/topics_pub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/pubsub/topics_sub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/asyncio-ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/generate_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/grasslands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/ioloop-ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/stonehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/strawhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/security/woodhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/serialization/serialsocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/examples/win32-interrupt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/win32-interrupt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/examples/win32-interrupt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/mypy_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/mypy_tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/mypy_tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/mypy_tests/test_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.482712 pyzmq-25.1.1b2/packaging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/packaging/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/pyzmq.dsc.obs
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/packaging/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/packaging/obs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/obs/_service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.542715 pyzmq-25.1.1b2/packaging/redhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/packaging/redhat/python-pyzmq.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.546716 pyzmq-25.1.1b2/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/perf/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/perf/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/perf/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167790 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/perf/perf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/perf/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.546716 pyzmq-25.1.1b2/pyzmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/pyzmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/pyzmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/pyzmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:01:56.000000 pyzmq-25.1.1b2/pyzmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/pyzmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/pyzmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:02:08.582718 pyzmq-25.1.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/setup.cfg.android
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/setup.cfg.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47961 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.546716 pyzmq-25.1.1b2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/backend_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/install_libzmq.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/run_with_env.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/showvcvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/test_sdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/test_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/tools/wheel-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.546716 pyzmq-25.1.1b2/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.550716 pyzmq-25.1.1b2/zmq/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/auth/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.550716 pyzmq-25.1.1b2/zmq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.550716 pyzmq-25.1.1b2/zmq/backend/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/_cdefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cffi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.558716 pyzmq-25.1.1b2/zmq/backend/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   235931 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/_device.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/_device.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   301152 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/_poll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/_poll.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   221469 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/_proxy_steerable.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/_proxy_steerable.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   141405 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/_version.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/_version.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/checkrc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/constant_enums.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)   288896 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/context.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   147454 2023-07-12 05:01:54.000000 pyzmq-25.1.1b2/zmq/backend/cython/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/error.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/libzmq.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   469392 2023-07-12 05:01:55.000000 pyzmq-25.1.1b2/zmq/backend/cython/message.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/message.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/message.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   655354 2023-07-12 05:01:55.000000 pyzmq-25.1.1b2/zmq/backend/cython/socket.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/socket.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/socket.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   191144 2023-07-12 05:01:55.000000 pyzmq-25.1.1b2/zmq/backend/cython/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/cython/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/backend/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.562717 pyzmq-25.1.1b2/zmq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)   293653 2023-07-12 05:01:56.000000 pyzmq-25.1.1b2/zmq/devices/monitoredqueue.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/monitoredqueue.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/monitoredqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/monitoredqueue.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/monitoredqueuedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/proxydevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/devices/proxysteerabledevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.562717 pyzmq-25.1.1b2/zmq/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/eventloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/eventloop/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/eventloop/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/eventloop/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/eventloop/zmqstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.562717 pyzmq-25.1.1b2/zmq/green/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.566717 pyzmq-25.1.1b2/zmq/green/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/eventloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/eventloop/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/eventloop/zmqstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/green/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.566717 pyzmq-25.1.1b2/zmq/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/log/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/log/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.566717 pyzmq-25.1.1b2/zmq/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/ssh/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/ssh/tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.570717 pyzmq-25.1.1b2/zmq/sugar/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/attrsettr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/sugar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.578718 pyzmq-25.1.1b2/zmq/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/cython_ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_cffi_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_cython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-12 05:01:38.000000 pyzmq-25.1.1b2/zmq/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_monqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_proxy_steerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_reqrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_retry_eintr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23610 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_win32_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_z85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/tests/test_zmqstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:02:08.582718 pyzmq-25.1.1b2/zmq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/buffers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/zmq/utils/compiler.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 05:02:08.000000 pyzmq-25.1.1b2/zmq/utils/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/garbage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/getpid_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/pyversion_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/strtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/win32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/z85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmq/utils/zmq_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-12 05:01:39.000000 pyzmq-25.1.1b2/zmqversion.py
```

### Comparing `pyzmq-25.1.1b1/.circleci/config.yml` & `pyzmq-25.1.1b2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/.github/ISSUE_TEMPLATE/bug.yml` & `pyzmq-25.1.1b2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/.github/ISSUE_TEMPLATE/config.yml` & `pyzmq-25.1.1b2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/.github/workflows/test.yml` & `pyzmq-25.1.1b2/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   # only affects Windows, but easiest to set here for now
   SETUPTOOLS_ENABLE_FEATURES: "legacy-editable"
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 20
+    continue-on-error: ${{ matrix.zmq == 'head' }}
 
     env:
       MACOSX_DEPLOYMENT_TARGET: "10.14"
 
     strategy:
       fail-fast: true
       matrix:
```

### Comparing `pyzmq-25.1.1b1/.github/workflows/wheels.yml` & `pyzmq-25.1.1b2/.github/workflows/wheels.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     branches-ignore:
       - "dependabot/**"
       - "pre-commit-ci-update-config"
     tags:
       - "**"
   pull_request:
     paths:
+      - pyproject.toml
       - setup.py
       - buildutils/**
       - .github/workflows/wheels.yml
       - tools/install_libzmq.sh
       - zmq/utils/*.h
 
 concurrency:
```

### Comparing `pyzmq-25.1.1b1/.mailmap` & `pyzmq-25.1.1b2/.mailmap`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/.pre-commit-config.yaml` & `pyzmq-25.1.1b2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,40 +20,40 @@
       - id: mdformat
         # Optionally add plugins
         additional_dependencies:
           - mdformat-black
           - mdformat-myst
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: autoflake
         args:
           - --in-place
         exclude: zmq/tests/test_imports.py
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         exclude: ^buildutils/templates/
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         files: zmq/.*
         # mypy gets the wrong results
         # if we pass specific files instead of the zmq dir
         # no idea why
         pass_filenames: false
         args: [zmq]
         additional_dependencies:
           - types-paramiko
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
         args:
           - --py36-plus
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
```

### Comparing `pyzmq-25.1.1b1/AUTHORS.md` & `pyzmq-25.1.1b2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/CONTRIBUTING.md` & `pyzmq-25.1.1b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/LICENSE.BSD` & `pyzmq-25.1.1b2/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/LICENSE.LESSER` & `pyzmq-25.1.1b2/bundled/zeromq/COPYING`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-                    GNU GENERAL PUBLIC LICENSE
+                      GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
   The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
@@ -641,15 +641,15 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
     <program>  Copyright (C) <year>  <name of author>
@@ -660,31 +660,15 @@
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
+<http://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
-
---------------------------------------------------------------------------------
-
-           SPECIAL EXCEPTION GRANTED BY COPYRIGHT HOLDERS
-
-As a special exception, copyright holders give you permission to link this
-library with independent modules to produce an executable, regardless of
-the license terms of these independent modules, and to copy and distribute
-the resulting executable under terms of your choice, provided that you also
-meet, for each linked independent module, the terms and conditions of
-the license of that module. An independent module is a module which is not
-derived from or based on this library. If you modify this library, you must
-extend this exception to your version of the library.
-
-Note: this exception relieves you of any obligations under sections 4 and 5
-of this license, and section 6 of the GNU General Public License.
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `pyzmq-25.1.1b1/PKG-INFO` & `pyzmq-25.1.1b2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 25.1.1b1
+Version: 25.1.1b2
 Summary: Python bindings for 0MQ
 Home-page: https://pyzmq.readthedocs.org
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-email: zeromq-dev@lists.zeromq.org
 License: LGPL+BSD
 Project-URL: Source, https://github.com/zeromq/pyzmq
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,17 @@
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.BSD
 License-File: LICENSE.LESSER
 License-File: AUTHORS.md
 
 # PyZMQ: Python bindings for ØMQ
```

### Comparing `pyzmq-25.1.1b1/README.md` & `pyzmq-25.1.1b2/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/README.md` & `pyzmq-25.1.1b2/RELICENSE/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/authors.py` & `pyzmq-25.1.1b2/RELICENSE/authors.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/chrislaws.md` & `pyzmq-25.1.1b2/RELICENSE/chrislaws.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/ellisonbg.md` & `pyzmq-25.1.1b2/RELICENSE/ellisonbg.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/frankwiles.md` & `pyzmq-25.1.1b2/RELICENSE/frankwiles.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/juliantaylor.md` & `pyzmq-25.1.1b2/RELICENSE/juliantaylor.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/ledgerx.md` & `pyzmq-25.1.1b2/RELICENSE/ledgerx.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/lothiraldan.md` & `pyzmq-25.1.1b2/RELICENSE/lothiraldan.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/minrk.md` & `pyzmq-25.1.1b2/RELICENSE/minrk.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/takluyver.md` & `pyzmq-25.1.1b2/RELICENSE/takluyver.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-bsd.txt` & `pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-bsd.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt` & `pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/RELICENSE/templates/relicense-template-mplv2.txt` & `pyzmq-25.1.1b2/RELICENSE/templates/relicense-template-mplv2.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/SECURITY.md` & `pyzmq-25.1.1b2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/Vagrantfile` & `pyzmq-25.1.1b2/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/_cffi.c` & `pyzmq-25.1.1b2/buildutils/_cffi.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/build_cffi.py` & `pyzmq-25.1.1b2/buildutils/build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/bundle.py` & `pyzmq-25.1.1b2/buildutils/bundle.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/config.py` & `pyzmq-25.1.1b2/buildutils/config.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/constants.py` & `pyzmq-25.1.1b2/buildutils/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/detect.py` & `pyzmq-25.1.1b2/buildutils/detect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_darwin/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_darwin/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_freebsd/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_freebsd/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_linux/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_linux/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_linux-armv/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_linux-armv/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_linux-musl/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_linux-musl/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/include_win32/platform.hpp` & `pyzmq-25.1.1b2/buildutils/include_win32/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/initlibzmq.cpp` & `pyzmq-25.1.1b2/buildutils/initlibzmq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/misc.py` & `pyzmq-25.1.1b2/buildutils/misc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/msg.py` & `pyzmq-25.1.1b2/buildutils/msg.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/buildutils/patch.py` & `pyzmq-25.1.1b2/buildutils/patch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/README.md` & `pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/license.txt` & `pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/license.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/wepoll.c` & `pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/wepoll.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/external/wepoll/wepoll.h` & `pyzmq-25.1.1b2/bundled/zeromq/external/wepoll/wepoll.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/include/zmq.h` & `pyzmq-25.1.1b2/bundled/zeromq/include/zmq.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/include/zmq_utils.h` & `pyzmq-25.1.1b2/bundled/zeromq/include/zmq_utils.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/array.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/array.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/atomic_counter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/atomic_counter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/atomic_ptr.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/atomic_ptr.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/blob.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/blob.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/channel.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/channel.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/channel.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/channel.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/client.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/client.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/clock.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/clock.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/clock.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/clock.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/command.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/command.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/compat.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/compat.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/condition_variable.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/condition_variable.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/config.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/config.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ctx.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ctx.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ctx.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ctx.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_client.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_client.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_client_tools.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_client_tools.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_mechanism_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_mechanism_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_server.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/curve_server.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/curve_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dbuffer.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dbuffer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dealer.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dealer.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dealer.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dealer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/decoder_allocators.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/decoder_allocators.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/decoder_allocators.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/decoder_allocators.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/devpoll.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/devpoll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/devpoll.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/devpoll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dgram.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dgram.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dgram.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dgram.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dish.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dish.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dish.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dish.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dist.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dist.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/dist.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/dist.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/endpoint.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/endpoint.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/endpoint.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/endpoint.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/epoll.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/epoll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/epoll.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/epoll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/err.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/err.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/err.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/err.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/fd.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/fd.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/fq.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/fq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/fq.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/fq.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gather.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gather.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gather.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gather.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/generic_mtrie.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/generic_mtrie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/generic_mtrie_impl.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/generic_mtrie_impl.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_client.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_client.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_mechanism_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_mechanism_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_server.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/gssapi_server.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/gssapi_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/i_decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/i_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/i_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/i_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/i_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/i_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/i_mailbox.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/i_mailbox.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/i_poll_events.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/i_poll_events.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/io_object.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/io_object.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/io_object.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/io_object.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/io_thread.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/io_thread.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/io_thread.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/io_thread.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ip.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ip.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ip.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ip.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ip_resolver.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ip_resolver.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ip_resolver.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ip_resolver.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_listener.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ipc_listener.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ipc_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/kqueue.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/kqueue.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/kqueue.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/kqueue.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/lb.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/lb.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/lb.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/lb.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/likely.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/likely.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/macros.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/macros.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mailbox.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mailbox.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mailbox.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mailbox.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mailbox_safe.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mailbox_safe.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mailbox_safe.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mailbox_safe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mechanism.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mechanism.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mechanism.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mechanism.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mechanism_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mechanism_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/metadata.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/metadata.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/metadata.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/metadata.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/msg.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/msg.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/msg.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/msg.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mtrie.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mtrie.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mtrie.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mtrie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/mutex.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/mutex.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/norm_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/norm_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/norm_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/norm_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/null_mechanism.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/null_mechanism.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/null_mechanism.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/null_mechanism.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/object.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/object.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/object.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/object.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/options.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/options.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/options.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/options.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/own.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/own.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/own.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/own.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pair.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pair.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pair.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pair.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/peer.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/peer.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/peer.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/peer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_receiver.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_receiver.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_receiver.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_receiver.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_sender.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_sender.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_sender.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_sender.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_socket.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_socket.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pgm_socket.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pgm_socket.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pipe.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pipe.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pipe.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pipe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/plain_client.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/plain_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/plain_client.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/plain_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/plain_common.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/plain_common.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/plain_server.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/plain_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/plain_server.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/plain_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/platform.hpp.in` & `pyzmq-25.1.1b2/bundled/zeromq/src/platform.hpp.in`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/poll.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/poll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/poll.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/poll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/poller.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/poller.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/poller_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/poller_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/poller_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/poller_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/polling_util.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/polling_util.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/polling_util.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/polling_util.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pollset.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pollset.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pollset.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pollset.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/precompiled.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/precompiled.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/precompiled.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/precompiled.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/proxy.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/proxy.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/proxy.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/proxy.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pub.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pub.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pull.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pull.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/pull.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/pull.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/push.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/push.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/push.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/push.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/radio.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/radio.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/radio.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/radio.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/radix_tree.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/radix_tree.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/radix_tree.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/radix_tree.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/random.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/random.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/random.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/random.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_decoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_encoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/raw_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/raw_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/reaper.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/reaper.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/reaper.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/reaper.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/rep.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/rep.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/rep.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/rep.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/req.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/req.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/req.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/req.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/router.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/router.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/router.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/router.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/scatter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/scatter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/scatter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/scatter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/secure_allocator.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/secure_allocator.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/select.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/select.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/select.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/select.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/server.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/server.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/session_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/session_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/session_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/session_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/signaler.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/signaler.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/signaler.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/signaler.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socket_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socket_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socket_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socket_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socket_poller.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socket_poller.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socket_poller.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socket_poller.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socks.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socks.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socks.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socks.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socks_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socks_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/socks_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/socks_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stdint.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stdint.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_connecter_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_connecter_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_connecter_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_connecter_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_engine_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_engine_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_engine_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_engine_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_listener_base.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_listener_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/stream_listener_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/stream_listener_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/sub.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/sub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/sub.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/sub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_listener.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tcp_listener.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tcp_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/thread.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/thread.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/thread.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/thread.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/timers.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/timers.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/timers.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/timers.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_listener.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tipc_listener.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/tipc_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/trie.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/trie.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/trie.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/trie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tweetnacl.c` & `pyzmq-25.1.1b2/bundled/zeromq/src/tweetnacl.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/tweetnacl.h` & `pyzmq-25.1.1b2/bundled/zeromq/src/tweetnacl.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/udp_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/udp_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/udp_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/udp_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/udp_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/udp_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/udp_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/udp_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v1_decoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v1_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v1_decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v1_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v1_encoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v1_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v1_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v1_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v2_decoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v2_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v2_decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v2_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v2_encoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v2_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v2_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v2_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v2_protocol.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v2_protocol.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v3_1_encoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v3_1_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/v3_1_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/v3_1_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/version.rc.in` & `pyzmq-25.1.1b2/bundled/zeromq/src/version.rc.in`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_listener.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/vmci_listener.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/vmci_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/windows.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/windows.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/wire.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/wire.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_connecter.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_connecter.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_decoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_decoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_encoder.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_encoder.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_listener.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_listener.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ws_protocol.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ws_protocol.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/wss_address.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/wss_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/wss_address.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/wss_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/wss_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/wss_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/wss_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/wss_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/xpub.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/xpub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/xpub.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/xpub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/xsub.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/xsub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/xsub.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/xsub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ypipe.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ypipe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ypipe_base.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ypipe_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/ypipe_conflate.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/ypipe_conflate.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/yqueue.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/yqueue.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zap_client.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zap_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zap_client.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zap_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zmq.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zmq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zmq_draft.h` & `pyzmq-25.1.1b2/bundled/zeromq/src/zmq_draft.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zmq_utils.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zmq_utils.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zmtp_engine.cpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zmtp_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/bundled/zeromq/src/zmtp_engine.hpp` & `pyzmq-25.1.1b2/bundled/zeromq/src/zmtp_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/Makefile` & `pyzmq-25.1.1b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/autogen_api.py` & `pyzmq-25.1.1b2/docs/autogen_api.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/_static/logo.png` & `pyzmq-25.1.1b2/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/_static/zeromq.ico` & `pyzmq-25.1.1b2/docs/source/_static/zeromq.ico`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/api/zmq.asyncio.rst` & `pyzmq-25.1.1b2/docs/source/api/zmq.asyncio.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/api/zmq.devices.rst` & `pyzmq-25.1.1b2/docs/source/api/zmq.devices.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/api/zmq.eventloop.future.rst` & `pyzmq-25.1.1b2/docs/source/api/zmq.eventloop.future.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/api/zmq.rst` & `pyzmq-25.1.1b2/docs/source/api/zmq.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/api/zmq.ssh.tunnel.rst` & `pyzmq-25.1.1b2/docs/source/api/zmq.ssh.tunnel.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/changelog.md` & `pyzmq-25.1.1b2/docs/source/changelog.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/conf.py` & `pyzmq-25.1.1b2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/devices.md` & `pyzmq-25.1.1b2/docs/source/howto/devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/draft.md` & `pyzmq-25.1.1b2/docs/source/howto/draft.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/eventloop.md` & `pyzmq-25.1.1b2/docs/source/howto/eventloop.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/logging.md` & `pyzmq-25.1.1b2/docs/source/howto/logging.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/morethanbindings.md` & `pyzmq-25.1.1b2/docs/source/howto/morethanbindings.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/serialization.md` & `pyzmq-25.1.1b2/docs/source/howto/serialization.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/howto/ssh.md` & `pyzmq-25.1.1b2/docs/source/howto/ssh.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/index.md` & `pyzmq-25.1.1b2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/notes/pyversions.md` & `pyzmq-25.1.1b2/docs/source/notes/pyversions.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/docs/source/notes/unicode.md` & `pyzmq-25.1.1b2/docs/source/notes/unicode.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/asyncio/coroutines.py` & `pyzmq-25.1.1b2/examples/asyncio/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/asyncio/helloworld_pubsub_dealerrouter.py` & `pyzmq-25.1.1b2/examples/asyncio/helloworld_pubsub_dealerrouter.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/asyncio/router_router.py` & `pyzmq-25.1.1b2/examples/asyncio/router_router.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/asyncio/tornado_asyncio.py` & `pyzmq-25.1.1b2/examples/asyncio/tornado_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/chat/display.py` & `pyzmq-25.1.1b2/examples/chat/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/chat/prompt.py` & `pyzmq-25.1.1b2/examples/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/cython/README.md` & `pyzmq-25.1.1b2/examples/cython/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/cython/cyzmq.pyx` & `pyzmq-25.1.1b2/examples/cython/cyzmq.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/cython/example.py` & `pyzmq-25.1.1b2/examples/cython/example.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/device/device.py` & `pyzmq-25.1.1b2/examples/device/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/draft/client-server.py` & `pyzmq-25.1.1b2/examples/draft/client-server.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/draft/install.sh` & `pyzmq-25.1.1b2/examples/draft/install.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/draft/radio-dish.py` & `pyzmq-25.1.1b2/examples/draft/radio-dish.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/eventloop/asyncweb.py` & `pyzmq-25.1.1b2/examples/eventloop/asyncweb.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/eventloop/coroutines.py` & `pyzmq-25.1.1b2/examples/eventloop/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/eventloop/echo.py` & `pyzmq-25.1.1b2/examples/eventloop/echo.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/gevent/poll.py` & `pyzmq-25.1.1b2/examples/gevent/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/gevent/reqrep.py` & `pyzmq-25.1.1b2/examples/gevent/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/gevent/simple.py` & `pyzmq-25.1.1b2/examples/gevent/simple.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/heartbeat/heart.py` & `pyzmq-25.1.1b2/examples/heartbeat/heart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/heartbeat/heartbeater.py` & `pyzmq-25.1.1b2/examples/heartbeat/heartbeater.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/heartbeat/ping.py` & `pyzmq-25.1.1b2/examples/heartbeat/ping.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/heartbeat/pong.py` & `pyzmq-25.1.1b2/examples/heartbeat/pong.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/logger/zmqlogger.py` & `pyzmq-25.1.1b2/examples/logger/zmqlogger.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/mongodb/client.py` & `pyzmq-25.1.1b2/examples/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/mongodb/controller.py` & `pyzmq-25.1.1b2/examples/mongodb/controller.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/monitoring/simple_monitor.py` & `pyzmq-25.1.1b2/examples/monitoring/simple_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/monitoring/zmq_monitor_class.py` & `pyzmq-25.1.1b2/examples/monitoring/zmq_monitor_class.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/poll/pair.py` & `pyzmq-25.1.1b2/examples/poll/pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/poll/pubsub.py` & `pyzmq-25.1.1b2/examples/poll/pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/poll/reqrep.py` & `pyzmq-25.1.1b2/examples/poll/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/pubsub/publisher.py` & `pyzmq-25.1.1b2/examples/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/pubsub/subscriber.py` & `pyzmq-25.1.1b2/examples/pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/pubsub/topics_pub.py` & `pyzmq-25.1.1b2/examples/pubsub/topics_pub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/pubsub/topics_sub.py` & `pyzmq-25.1.1b2/examples/pubsub/topics_sub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/asyncio-ironhouse.py` & `pyzmq-25.1.1b2/examples/security/asyncio-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/generate_certificates.py` & `pyzmq-25.1.1b2/examples/security/generate_certificates.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/grasslands.py` & `pyzmq-25.1.1b2/examples/security/grasslands.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/ioloop-ironhouse.py` & `pyzmq-25.1.1b2/examples/security/ioloop-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/ironhouse.py` & `pyzmq-25.1.1b2/examples/security/ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/stonehouse.py` & `pyzmq-25.1.1b2/examples/security/stonehouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/strawhouse.py` & `pyzmq-25.1.1b2/examples/security/strawhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/security/woodhouse.py` & `pyzmq-25.1.1b2/examples/security/woodhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/serialization/serialsocket.py` & `pyzmq-25.1.1b2/examples/serialization/serialsocket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/win32-interrupt/display.py` & `pyzmq-25.1.1b2/examples/win32-interrupt/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/examples/win32-interrupt/prompt.py` & `pyzmq-25.1.1b2/examples/win32-interrupt/prompt.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/debian/control` & `pyzmq-25.1.1b2/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/debian/copyright` & `pyzmq-25.1.1b2/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/debian/pyzmq.dsc.obs` & `pyzmq-25.1.1b2/packaging/debian/pyzmq.dsc.obs`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/debian/rules` & `pyzmq-25.1.1b2/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/obs/_service` & `pyzmq-25.1.1b2/packaging/obs/_service`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/packaging/redhat/python-pyzmq.spec` & `pyzmq-25.1.1b2/packaging/redhat/python-pyzmq.spec`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/perf/Makefile` & `pyzmq-25.1.1b2/perf/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/perf/collect.py` & `pyzmq-25.1.1b2/perf/collect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/perf/perf.ipynb` & `pyzmq-25.1.1b2/perf/perf.ipynb`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/perf/perf.py` & `pyzmq-25.1.1b2/perf/perf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/pyproject.toml` & `pyzmq-25.1.1b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 requires = [
     "setuptools",
     "setuptools_scm[toml]",
     "wheel",
     "packaging",
     "cffi; implementation_name == 'pypy'",
     "cython>=0.29; implementation_name == 'cpython'",
-    "cython>=3.0.0b3; implementation_name == 'cpython' and python_version >= '3.12'",
+    "cython>=0.29.35; implementation_name == 'cpython' and python_version >= '3.12'",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/zeromq/pyzmq"
 
 [tool.tbump.version]
-current = "25.1.1b1"
+current = "25.1.1b2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc|)\d+)|.dev\d*|)
```

### Comparing `pyzmq-25.1.1b1/pyzmq.egg-info/PKG-INFO` & `pyzmq-25.1.1b2/pyzmq.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 25.1.1b1
+Version: 25.1.1b2
 Summary: Python bindings for 0MQ
 Home-page: https://pyzmq.readthedocs.org
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-email: zeromq-dev@lists.zeromq.org
 License: LGPL+BSD
 Project-URL: Source, https://github.com/zeromq/pyzmq
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,17 @@
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.BSD
 License-File: LICENSE.LESSER
 License-File: AUTHORS.md
 
 # PyZMQ: Python bindings for ØMQ
```

### Comparing `pyzmq-25.1.1b1/pyzmq.egg-info/SOURCES.txt` & `pyzmq-25.1.1b2/pyzmq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 buildutils/include_linux-armv/platform.hpp
 buildutils/include_linux-musl/platform.hpp
 buildutils/include_win32/platform.hpp
 buildutils/include_win32/stdint.h
 buildutils/templates/constant_enums.pxi
 buildutils/templates/constants.py
 bundled/zeromq/COPYING
+bundled/zeromq/COPYING.LESSER
 bundled/zeromq/external/wepoll/README.md
 bundled/zeromq/external/wepoll/license.txt
 bundled/zeromq/external/wepoll/version.txt
 bundled/zeromq/external/wepoll/wepoll.c
 bundled/zeromq/external/wepoll/wepoll.h
 bundled/zeromq/include/zmq.h
 bundled/zeromq/include/zmq_utils.h
```

### Comparing `pyzmq-25.1.1b1/setup.cfg.template` & `pyzmq-25.1.1b2/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/setup.py` & `pyzmq-25.1.1b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from traceback import print_exc
 
 from packaging.version import Version as V
 from setuptools import Command, setup
 from setuptools.command.bdist_egg import bdist_egg
 from setuptools.command.build_ext import build_ext
 from setuptools.command.sdist import sdist
+from setuptools.errors import OptionError
 from setuptools.extension import Extension
 
 # local script imports:
 sys.path.insert(0, os.path.dirname(__file__))
 
 from buildutils import (
     bundled_version,
@@ -1103,14 +1104,26 @@
         with fix_cxx(self.compiler, ext):
             super().build_extension(ext)
 
         ext_path = self.get_ext_fullpath(ext.name)
         patch_lib_paths(ext_path, self.compiler.library_dirs)
 
     def finalize_options(self):
+        # this is normally done by super().finalize_options() but it
+        # needs to be done *before* we call configure if cython,
+        # numpy and pythran are all installed; and we can't call it
+        # after finalize_options() because that breaks pypy builds
+        # on Windows; logic copied from distutils/command/build_ext.py
+        # https://github.com/zeromq/pyzmq/pull/1872
+        if isinstance(self.parallel, str):
+            try:
+                self.parallel = int(self.parallel)
+            except ValueError:
+                raise OptionError("parallel should be an integer")
+
         # check version, to prevent confusing undefined constant errors
         self.distribution.run_command("configure")
         return super().finalize_options()
 
 
 class ConstantsCommand(Command):
     """Rebuild templated files for constants
@@ -1251,14 +1264,26 @@
         def build_extension(self, ext):
             with fix_cxx(self.compiler, ext):
                 super().build_extension(ext)
             ext_path = self.get_ext_fullpath(ext.name)
             patch_lib_paths(ext_path, self.compiler.library_dirs)
 
         def finalize_options(self):
+            # this is normally done by super().finalize_options() but it
+            # needs to be done *before* we call configure if cython,
+            # numpy and pythran are all installed; and we can't call it
+            # after finalize_options() because that breaks pypy builds
+            # on Windows; logic copied from distutils/command/build_ext.py
+            # https://github.com/zeromq/pyzmq/pull/1872
+            if isinstance(self.parallel, str):
+                try:
+                    self.parallel = int(self.parallel)
+                except ValueError:
+                    raise OptionError("parallel should be an integer")
+
             self.distribution.run_command("configure")
             return super().finalize_options()
 
     cmdclass["cython"] = CythonCommand
     cmdclass["build_ext"] = zbuild_ext
 
 extensions = []
@@ -1318,15 +1343,15 @@
 # -----------------------------------------------------------------------------
 
 with open('README.md', encoding='utf-8') as f:
     long_desc = f.read()
 
 setup_args = dict(
     name="pyzmq",
-    version="25.1.1b1",
+    version="25.1.1b2",
     packages=find_packages(),
     ext_modules=extensions,
     cffi_modules=cffi_modules,
     package_data=package_data,
     author="Brian E. Granger, Min Ragan-Kelley",
     author_email="zeromq-dev@lists.zeromq.org",
     url="https://pyzmq.readthedocs.org",
@@ -1351,14 +1376,17 @@
         "Topic :: System :: Networking",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     zip_safe=False,
     python_requires=">=3.6",
     install_requires=[
         "cffi; implementation_name == 'pypy'",
     ],
 )
```

### Comparing `pyzmq-25.1.1b1/test-requirements.txt` & `pyzmq-25.1.1b2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/tools/install_libzmq.sh` & `pyzmq-25.1.1b2/tools/install_libzmq.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/tools/run_with_env.cmd` & `pyzmq-25.1.1b2/tools/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/tools/test_sdist.py` & `pyzmq-25.1.1b2/tools/test_sdist.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 
 @pytest.mark.parametrize(
     "path",
     [
         # bundled zeromq
         "bundled/zeromq/COPYING",
+        "bundled/zeromq/COPYING.LESSER",
         "bundled/zeromq/include/zmq.h",
         "bundled/zeromq/src/zmq.cpp",
         "bundled/zeromq/external/wepoll/license.txt",
         "bundled/zeromq/external/wepoll/wepoll.h",
         # Cython-generated files
         "zmq/backend/cython/socket.c",
     ],
```

### Comparing `pyzmq-25.1.1b1/tools/test_wheel.py` & `pyzmq-25.1.1b2/tools/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/__init__.py` & `pyzmq-25.1.1b2/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/__init__.pyi` & `pyzmq-25.1.1b2/zmq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/_future.py` & `pyzmq-25.1.1b2/zmq/_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/asyncio.py` & `pyzmq-25.1.1b2/zmq/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/auth/asyncio.py` & `pyzmq-25.1.1b2/zmq/auth/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/auth/base.py` & `pyzmq-25.1.1b2/zmq/auth/base.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/auth/certs.py` & `pyzmq-25.1.1b2/zmq/auth/certs.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/auth/ioloop.py` & `pyzmq-25.1.1b2/zmq/auth/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/auth/thread.py` & `pyzmq-25.1.1b2/zmq/auth/thread.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/__init__.py` & `pyzmq-25.1.1b2/zmq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/__init__.pyi` & `pyzmq-25.1.1b2/zmq/backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/__init__.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/_cdefs.h` & `pyzmq-25.1.1b2/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/_poll.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/context.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/devices.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/devices.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/message.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/socket.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cffi/utils.py` & `pyzmq-25.1.1b2/zmq/backend/cffi/utils.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/__init__.py` & `pyzmq-25.1.1b2/zmq/backend/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_device.c` & `pyzmq-25.1.1b2/zmq/backend/cython/_device.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1387,30 +1389,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -3016,38 +3018,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4387,18 +4389,18 @@
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -4444,22 +4446,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_device.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/_device.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_poll.c` & `pyzmq-25.1.1b2/zmq/backend/cython/_poll.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1454,30 +1456,30 @@
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -3709,39 +3711,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(2, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(2, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(2, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(3, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5424,18 +5426,18 @@
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -5481,22 +5483,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_poll.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/_poll.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_proxy_steerable.c` & `pyzmq-25.1.1b2/zmq/backend/cython/_proxy_steerable.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1387,30 +1389,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2673,38 +2675,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4028,18 +4030,18 @@
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -4085,22 +4087,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_proxy_steerable.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/_proxy_steerable.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_version.c` & `pyzmq-25.1.1b2/zmq/backend/cython/_version.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/_version.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/_version.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/checkrc.pxd` & `pyzmq-25.1.1b2/zmq/backend/cython/checkrc.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/constant_enums.pxi` & `pyzmq-25.1.1b2/zmq/backend/cython/constant_enums.pxi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/context.c` & `pyzmq-25.1.1b2/zmq/backend/cython/context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/getpid_compat.h",
             "zmq/utils/pyversion_compat.h",
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -101,15 +101,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -385,17 +385,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -465,14 +462,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1354,30 +1356,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
@@ -3434,15 +3436,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3zmq_7backend_6cython_7context_Context(PyObject *o) {
   struct __pyx_obj_3zmq_7backend_6cython_7context_Context *p = (struct __pyx_obj_3zmq_7backend_6cython_7context_Context *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   if (p->__weakref__) PyObject_ClearWeakRefs(o);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -3823,29 +3825,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5417,18 +5419,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -5474,22 +5476,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/context.pxd` & `pyzmq-25.1.1b2/zmq/backend/cython/context.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/context.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/context.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/error.c` & `pyzmq-25.1.1b2/zmq/backend/cython/error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/error.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/error.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/libzmq.pxd` & `pyzmq-25.1.1b2/zmq/backend/cython/libzmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/message.c` & `pyzmq-25.1.1b2/zmq/backend/cython/message.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/mutex.h",
             "zmq/utils/pyversion_compat.h",
@@ -26,16 +26,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,15 +102,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -386,17 +386,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -466,14 +463,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1408,30 +1410,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
@@ -7115,15 +7117,15 @@
   p->peers = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_3zmq_7backend_6cython_7message_MessageTracker(PyObject *o) {
   struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker *p = (struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->events);
   Py_CLEAR(p->peers);
   (*Py_TYPE(o)->tp_free)(o);
@@ -7248,15 +7250,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3zmq_7backend_6cython_7message_Frame(PyObject *o) {
   struct __pyx_obj_3zmq_7backend_6cython_7message_Frame *p = (struct __pyx_obj_3zmq_7backend_6cython_7message_Frame *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -7863,29 +7865,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -9673,18 +9675,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -9730,22 +9732,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/message.pxd` & `pyzmq-25.1.1b2/zmq/backend/cython/message.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/message.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/message.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/socket.c` & `pyzmq-25.1.1b2/zmq/backend/cython/socket.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/getpid_compat.h",
             "zmq/utils/ipcmaxlen.h",
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,15 +103,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -387,17 +387,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -467,14 +464,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1565,30 +1567,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -11048,15 +11050,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_3zmq_7backend_6cython_6socket_Socket(PyObject *o) {
   struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket *p = (struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   if (p->__weakref__) PyObject_ClearWeakRefs(o);
   Py_CLEAR(p->context);
   (*Py_TYPE(o)->tp_free)(o);
@@ -11826,39 +11828,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(7, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(9, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(9, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.message"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.message", "MessageTracker", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker) __PYX_ERR(4, 34, __pyx_L1_error)
-  __pyx_ptype_3zmq_7backend_6cython_7message_Frame = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.message", "Frame", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7message_Frame) __PYX_ERR(4, 40, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.message", "MessageTracker", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker) __PYX_ERR(4, 34, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7message_Frame = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.message", "Frame", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7message_Frame) __PYX_ERR(4, 40, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7message_Frame = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7message_Frame*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7message_Frame->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7message_Frame)) __PYX_ERR(4, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -14018,18 +14020,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -14075,22 +14077,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/socket.pxd` & `pyzmq-25.1.1b2/zmq/backend/cython/socket.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/socket.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/socket.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/utils.c` & `pyzmq-25.1.1b2/zmq/backend/cython/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,15 +100,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -384,17 +384,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -464,14 +461,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
```

### Comparing `pyzmq-25.1.1b1/zmq/backend/cython/utils.pyx` & `pyzmq-25.1.1b2/zmq/backend/cython/utils.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/backend/select.py` & `pyzmq-25.1.1b2/zmq/backend/select.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/constants.py` & `pyzmq-25.1.1b2/zmq/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/decorators.py` & `pyzmq-25.1.1b2/zmq/decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/__init__.py` & `pyzmq-25.1.1b2/zmq/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/basedevice.py` & `pyzmq-25.1.1b2/zmq/devices/basedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/monitoredqueue.c` & `pyzmq-25.1.1b2/zmq/devices/monitoredqueue.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -101,15 +101,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -385,17 +385,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -465,14 +462,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1389,30 +1391,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -4702,38 +4704,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(7, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_36(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(7, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(7, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -6085,18 +6087,18 @@
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -6142,22 +6144,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `pyzmq-25.1.1b1/zmq/devices/monitoredqueue.pxd` & `pyzmq-25.1.1b2/zmq/devices/monitoredqueue.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/monitoredqueue.py` & `pyzmq-25.1.1b2/zmq/devices/monitoredqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/monitoredqueue.pyx` & `pyzmq-25.1.1b2/zmq/devices/monitoredqueue.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/monitoredqueuedevice.py` & `pyzmq-25.1.1b2/zmq/devices/monitoredqueuedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/proxydevice.py` & `pyzmq-25.1.1b2/zmq/devices/proxydevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/devices/proxysteerabledevice.py` & `pyzmq-25.1.1b2/zmq/devices/proxysteerabledevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/error.py` & `pyzmq-25.1.1b2/zmq/error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/eventloop/_deprecated.py` & `pyzmq-25.1.1b2/zmq/eventloop/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/eventloop/future.py` & `pyzmq-25.1.1b2/zmq/eventloop/future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/eventloop/ioloop.py` & `pyzmq-25.1.1b2/zmq/eventloop/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/eventloop/zmqstream.py` & `pyzmq-25.1.1b2/zmq/eventloop/zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/green/__init__.py` & `pyzmq-25.1.1b2/zmq/green/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/green/core.py` & `pyzmq-25.1.1b2/zmq/green/core.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/green/device.py` & `pyzmq-25.1.1b2/zmq/green/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/green/poll.py` & `pyzmq-25.1.1b2/zmq/green/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/log/__main__.py` & `pyzmq-25.1.1b2/zmq/log/__main__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/log/handlers.py` & `pyzmq-25.1.1b2/zmq/log/handlers.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/ssh/forward.py` & `pyzmq-25.1.1b2/zmq/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/ssh/tunnel.py` & `pyzmq-25.1.1b2/zmq/ssh/tunnel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/__init__.py` & `pyzmq-25.1.1b2/zmq/sugar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/attrsettr.py` & `pyzmq-25.1.1b2/zmq/sugar/attrsettr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/context.py` & `pyzmq-25.1.1b2/zmq/sugar/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/frame.py` & `pyzmq-25.1.1b2/zmq/sugar/frame.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/poll.py` & `pyzmq-25.1.1b2/zmq/sugar/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/socket.py` & `pyzmq-25.1.1b2/zmq/sugar/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/stopwatch.py` & `pyzmq-25.1.1b2/zmq/sugar/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/tracker.py` & `pyzmq-25.1.1b2/zmq/sugar/tracker.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/sugar/version.py` & `pyzmq-25.1.1b2/zmq/sugar/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 from typing import Match, Tuple, Union, cast
 
 from zmq.backend import zmq_version_info
 
-__version__: str = "25.1.1b1"
+__version__: str = "25.1.1b2"
 _version_pat = re.compile(r"(\d+)\.(\d+)\.(\d+)(.*)")
 _match = cast(Match, _version_pat.match(__version__))
 _version_groups = _match.groups()
 
 VERSION_MAJOR = int(_version_groups[0])
 VERSION_MINOR = int(_version_groups[1])
 VERSION_PATCH = int(_version_groups[2])
```

### Comparing `pyzmq-25.1.1b1/zmq/tests/__init__.py` & `pyzmq-25.1.1b2/zmq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/conftest.py` & `pyzmq-25.1.1b2/zmq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/cython_ext.pyx` & `pyzmq-25.1.1b2/zmq/tests/cython_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_asyncio.py` & `pyzmq-25.1.1b2/zmq/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_auth.py` & `pyzmq-25.1.1b2/zmq/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_cffi_backend.py` & `pyzmq-25.1.1b2/zmq/tests/test_cffi_backend.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_constants.py` & `pyzmq-25.1.1b2/zmq/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_context.py` & `pyzmq-25.1.1b2/zmq/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_cython.py` & `pyzmq-25.1.1b2/zmq/tests/test_cython.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_decorators.py` & `pyzmq-25.1.1b2/zmq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_device.py` & `pyzmq-25.1.1b2/zmq/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_draft.py` & `pyzmq-25.1.1b2/zmq/tests/test_draft.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_error.py` & `pyzmq-25.1.1b2/zmq/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_etc.py` & `pyzmq-25.1.1b2/zmq/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_ext.py` & `pyzmq-25.1.1b2/zmq/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_future.py` & `pyzmq-25.1.1b2/zmq/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_imports.py` & `pyzmq-25.1.1b2/zmq/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_includes.py` & `pyzmq-25.1.1b2/zmq/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_ioloop.py` & `pyzmq-25.1.1b2/zmq/tests/test_ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_log.py` & `pyzmq-25.1.1b2/zmq/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_message.py` & `pyzmq-25.1.1b2/zmq/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_monitor.py` & `pyzmq-25.1.1b2/zmq/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_monqueue.py` & `pyzmq-25.1.1b2/zmq/tests/test_monqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_multipart.py` & `pyzmq-25.1.1b2/zmq/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_mypy.py` & `pyzmq-25.1.1b2/zmq/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_pair.py` & `pyzmq-25.1.1b2/zmq/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_poll.py` & `pyzmq-25.1.1b2/zmq/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_proxy_steerable.py` & `pyzmq-25.1.1b2/zmq/tests/test_proxy_steerable.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_pubsub.py` & `pyzmq-25.1.1b2/zmq/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_reqrep.py` & `pyzmq-25.1.1b2/zmq/tests/test_reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_retry_eintr.py` & `pyzmq-25.1.1b2/zmq/tests/test_retry_eintr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_security.py` & `pyzmq-25.1.1b2/zmq/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_socket.py` & `pyzmq-25.1.1b2/zmq/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_version.py` & `pyzmq-25.1.1b2/zmq/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_win32_shim.py` & `pyzmq-25.1.1b2/zmq/tests/test_win32_shim.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_z85.py` & `pyzmq-25.1.1b2/zmq/tests/test_z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/tests/test_zmqstream.py` & `pyzmq-25.1.1b2/zmq/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/buffers.pxd` & `pyzmq-25.1.1b2/zmq/utils/buffers.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/garbage.py` & `pyzmq-25.1.1b2/zmq/utils/garbage.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/interop.py` & `pyzmq-25.1.1b2/zmq/utils/interop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/ipcmaxlen.h` & `pyzmq-25.1.1b2/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/jsonapi.py` & `pyzmq-25.1.1b2/zmq/utils/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/monitor.py` & `pyzmq-25.1.1b2/zmq/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/mutex.h` & `pyzmq-25.1.1b2/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/strtypes.py` & `pyzmq-25.1.1b2/zmq/utils/strtypes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/win32.py` & `pyzmq-25.1.1b2/zmq/utils/win32.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/z85.py` & `pyzmq-25.1.1b2/zmq/utils/z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmq/utils/zmq_compat.h` & `pyzmq-25.1.1b2/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.1.1b1/zmqversion.py` & `pyzmq-25.1.1b2/zmqversion.py`

 * *Files identical despite different names*

