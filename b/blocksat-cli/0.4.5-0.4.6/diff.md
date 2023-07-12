# Comparing `tmp/blocksat-cli-0.4.5.tar.gz` & `tmp/blocksat-cli-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blocksat-cli-0.4.5.tar", last modified: Fri Mar  3 14:50:25 2023, max compression
+gzip compressed data, was "blocksat-cli-0.4.6.tar", last modified: Wed Jul 12 11:01:38 2023, max compression
```

## Comparing `blocksat-cli-0.4.5.tar` & `blocksat-cli-0.4.6.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.284509 blocksat-cli-0.4.5/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      608 2023-03-03 14:50:25.284509 blocksat-cli-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3766 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.272509 blocksat-cli-0.4.5/blocksat_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      608 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2759 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-03 14:50:25.000000 blocksat-cli-0.4.5/blocksat_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.276509 blocksat-cli-0.4.5/blocksatcli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:50:13.000000 blocksat-cli-0.4.5/blocksatcli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.276509 blocksat-cli-0.4.5/blocksatcli/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:50:13.000000 blocksat-cli-0.4.5/blocksatcli/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29710 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/bidding.py
--rwxrwxrwx   0 root         (0) root         (0)    10687 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/demorx.py
--rw-rw-rw-   0 root         (0) root         (0)    14677 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/fec.py
--rw-rw-rw-   0 root         (0) root         (0)     9067 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/gpg.py
--rw-rw-rw-   0 root         (0) root         (0)     8393 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/listen.py
--rw-rw-rw-   0 root         (0) root         (0)    23842 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/msg.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/net.py
--rw-rw-rw-   0 root         (0) root         (0)    16393 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/order.py
--rw-rw-rw-   0 root         (0) root         (0)    14070 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/pkt.py
--rw-rw-rw-   0 root         (0) root         (0)     2142 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_bidding.py
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_fec.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_gpg.py
--rw-rw-rw-   0 root         (0) root         (0)     6879 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_listen.py
--rw-rw-rw-   0 root         (0) root         (0)    18977 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_msg.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_net.py
--rw-rw-rw-   0 root         (0) root         (0)     3024 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_order.py
--rw-rw-rw-   0 root         (0) root         (0)     8366 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/api/test_pkt.py
--rw-rw-rw-   0 root         (0) root         (0)     6277 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/bitcoin.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    29369 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/defs.py
--rw-rw-rw-   0 root         (0) root         (0)    28899 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)    11824 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/firewall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.276509 blocksat-cli-0.4.5/blocksatcli/gpg/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/gpg/87D07253F69E4CD8629B0A21A94A007EC9D4458C.gpg
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/gqrx.py
--rw-rw-rw-   0 root         (0) root         (0)    16025 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/instructions.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/ip.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.276509 blocksat-cli-0.4.5/blocksatcli/mib/
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/NOVRA-MIB.mib
--rw-rw-rw-   0 root         (0) root         (0)    30862 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/NOVRA-s400-MIB.mib
--rw-rw-rw-   0 root         (0) root         (0)     3067 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/RFC1155-SMI.txt
--rw-rw-rw-   0 root         (0) root         (0)     8263 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-CONF.txt
--rw-rw-rw-   0 root         (0) root         (0)     8924 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-SMI.txt
--rw-rw-rw-   0 root         (0) root         (0)    38034 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-TC.txt
--rw-rw-rw-   0 root         (0) root         (0)    17370 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/monitoring.py
--rw-rw-rw-   0 root         (0) root         (0)    29936 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/monitoring_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5928 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/rp.py
--rw-rw-rw-   0 root         (0) root         (0)    29903 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/satip.py
--rw-rw-rw-   0 root         (0) root         (0)    23416 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/sdr.py
--rw-rw-rw-   0 root         (0) root         (0)    25757 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/standalone.py
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_bitcoin.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3963 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_gqrx.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15184 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_monitoring.py
--rw-rw-rw-   0 root         (0) root         (0)    17119 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_monitoring_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3670 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_satip.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_tsp.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_update.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_usb.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)     6135 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/tsp.py
--rw-rw-rw-   0 root         (0) root         (0)     6190 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/update.py
--rw-rw-rw-   0 root         (0) root         (0)    12761 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/upnp.py
--rw-rw-rw-   0 root         (0) root         (0)    30493 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/usb.py
--rw-rw-rw-   0 root         (0) root         (0)    12871 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/util.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/blocksatcli/verify_deps_instal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.280509 blocksat-cli-0.4.5/doc/
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/README.md
--rw-rw-rw-   0 root         (0) root         (0)    28571 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/antenna-pointing.md
--rw-rw-rw-   0 root         (0) root         (0)    21151 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/api.md
--rw-rw-rw-   0 root         (0) root         (0)     7192 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/bitcoin.md
--rw-rw-rw-   0 root         (0) root         (0)     5908 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/docker.md
--rw-rw-rw-   0 root         (0) root         (0)     8179 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/dual-satellite.md
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/frequency.md
--rw-rw-rw-   0 root         (0) root         (0)    33395 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/hardware.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:50:25.284509 blocksat-cli-0.4.5/doc/img/
--rw-rw-rw-   0 root         (0) root         (0)   102112 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/api_architecture.png
--rw-rw-rw-   0 root         (0) root         (0)   149401 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/azimuth.png
--rw-rw-rw-   0 root         (0) root         (0)    14581 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/blockstream.png
--rw-rw-rw-   0 root         (0) root         (0)   139354 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/elevation.png
--rw-rw-rw-   0 root         (0) root         (0)   159429 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/gqrx-centered.png
--rw-rw-rw-   0 root         (0) root         (0)   196623 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/gqrx-offset.png
--rw-rw-rw-   0 root         (0) root         (0)    15296 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/leandvb-pls-syms.png
--rw-rw-rw-   0 root         (0) root         (0)    15376 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/leandvb-pre-processed-iq.png
--rw-rw-rw-   0 root         (0) root         (0)    14716 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/leandvb-pre-processed-iq2.png
--rw-rw-rw-   0 root         (0) root         (0)    19167 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/leandvb-spectrum-centered.png
--rw-rw-rw-   0 root         (0) root         (0)    12948 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/leandvb-spectrum-offset.png
--rw-rw-rw-   0 root         (0) root         (0)    89325 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/lnb_polarization.png
--rw-rw-rw-   0 root         (0) root         (0)    97965 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/monitoring-api-authentication.png
--rw-rw-rw-   0 root         (0) root         (0)    13082 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/s400_locked.png
--rw-rw-rw-   0 root         (0) root         (0)    33595 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/s400_rf_status.png
--rw-rw-rw-   0 root         (0) root         (0)    12463 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/s400_searching.png
--rw-rw-rw-   0 root         (0) root         (0)  1196013 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/sat-ip-connections.png
--rw-rw-rw-   0 root         (0) root         (0)   333258 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/sdr_connections.png
--rw-rw-rw-   0 root         (0) root         (0)   141359 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/standalone_connections.png
--rw-rw-rw-   0 root         (0) root         (0)   112570 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/img/usb_connections.png
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/monitoring.md
--rw-rw-rw-   0 root         (0) root         (0)     4909 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/quick-reference.md
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/receiver.md
--rw-rw-rw-   0 root         (0) root         (0)     6412 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/s400.md
--rw-rw-rw-   0 root         (0) root         (0)     7824 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/sat-ip.md
--rw-rw-rw-   0 root         (0) root         (0)     6545 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/sdr.md
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/software.md
--rw-rw-rw-   0 root         (0) root         (0)     5665 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/doc/tbs.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-03 14:50:25.284509 blocksat-cli-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-03-03 14:36:06.000000 blocksat-cli-0.4.5/setup.py
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.521648 blocksat-cli-0.4.6/
+-rw-r--r--   0 igorfreire   (501) staff       (20)    35149 2020-05-04 13:29:52.000000 blocksat-cli-0.4.6/LICENSE
+-rw-r--r--   0 igorfreire   (501) staff       (20)       59 2021-04-29 15:31:48.000000 blocksat-cli-0.4.6/MANIFEST.in
+-rw-r--r--   0 igorfreire   (501) staff       (20)      628 2023-07-12 11:01:38.521512 blocksat-cli-0.4.6/PKG-INFO
+-rw-r--r--   0 igorfreire   (501) staff       (20)     3766 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/README.md
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.489401 blocksat-cli-0.4.6/blocksat_cli.egg-info/
+-rw-r--r--   0 igorfreire   (501) staff       (20)      628 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2759 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)        1 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)       55 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)       69 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/requires.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)       12 2023-07-12 11:01:38.000000 blocksat-cli-0.4.6/blocksat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.499370 blocksat-cli-0.4.6/blocksatcli/
+-rw-r--r--   0 igorfreire   (501) staff       (20)        0 2023-07-07 00:22:16.000000 blocksat-cli-0.4.6/blocksatcli/__init__.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)       31 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/blocksatcli/__main__.py
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.503959 blocksat-cli-0.4.6/blocksatcli/api/
+-rw-r--r--   0 igorfreire   (501) staff       (20)        0 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/api/__init__.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    29740 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/api/api.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2488 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/api/bidding.py
+-rwxr-xr-x   0 igorfreire   (501) staff       (20)    11171 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/demorx.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    14757 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/fec.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     9126 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/gpg.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     8394 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/api/listen.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    24346 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/msg.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4533 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/blocksatcli/api/net.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    16485 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/api/order.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    14070 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/blocksatcli/api/pkt.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2142 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/api/test_bidding.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4540 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/test_fec.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     5224 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/test_gpg.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6879 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/blocksatcli/api/test_listen.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    19124 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/test_msg.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)      953 2023-03-03 11:35:27.000000 blocksat-cli-0.4.6/blocksatcli/api/test_net.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     5470 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/api/test_order.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     8366 2023-06-27 19:39:59.000000 blocksat-cli-0.4.6/blocksatcli/api/test_pkt.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6549 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/bitcoin.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1798 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/cache.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    33185 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/config.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     7628 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/defs.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    29192 2023-07-10 19:11:12.000000 blocksat-cli-0.4.6/blocksatcli/dependencies.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    18074 2023-07-11 20:06:59.000000 blocksat-cli-0.4.6/blocksatcli/firewall.py
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.504209 blocksat-cli-0.4.6/blocksatcli/gpg/
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1704 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/gpg/87D07253F69E4CD8629B0A21A94A007EC9D4458C.gpg
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2771 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/gqrx.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    17729 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/instructions.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    11688 2023-07-12 00:48:51.000000 blocksat-cli-0.4.6/blocksatcli/ip.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     3077 2023-07-07 00:22:16.000000 blocksat-cli-0.4.6/blocksatcli/main.py
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.505974 blocksat-cli-0.4.6/blocksatcli/mib/
+-rw-r--r--   0 igorfreire   (501) staff       (20)      841 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/NOVRA-MIB.mib
+-rw-r--r--   0 igorfreire   (501) staff       (20)    30862 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/NOVRA-s400-MIB.mib
+-rw-r--r--   0 igorfreire   (501) staff       (20)     3067 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/RFC1155-SMI.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)     8263 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-CONF.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)     8924 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-SMI.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)    38034 2021-03-11 20:30:28.000000 blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-TC.txt
+-rw-r--r--   0 igorfreire   (501) staff       (20)    17903 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/monitoring.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    32648 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/monitoring_api.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6102 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/rp.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    31494 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/satip.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    24620 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/sdr.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    28701 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/standalone.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     5098 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/blocksatcli/test_bitcoin.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2957 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/blocksatcli/test_cache.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    30213 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/test_config.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    15327 2023-07-11 20:06:59.000000 blocksat-cli-0.4.6/blocksatcli/test_firewall.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4518 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/blocksatcli/test_gqrx.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4342 2023-04-12 21:21:05.000000 blocksat-cli-0.4.6/blocksatcli/test_helpers.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    15790 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/test_monitoring.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    17964 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/test_monitoring_api.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4470 2023-07-06 14:46:43.000000 blocksat-cli-0.4.6/blocksatcli/test_satip.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1752 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/blocksatcli/test_tsp.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1158 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/test_update.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1986 2023-07-07 20:55:20.000000 blocksat-cli-0.4.6/blocksatcli/test_usb.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4501 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/test_util.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6135 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/tsp.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6190 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/update.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    12761 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/blocksatcli/upnp.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    36040 2023-07-12 00:58:08.000000 blocksat-cli-0.4.6/blocksatcli/usb.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)    12871 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/util.py
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2857 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/blocksatcli/verify_deps_instal.py
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.509529 blocksat-cli-0.4.6/doc/
+-rw-r--r--   0 igorfreire   (501) staff       (20)      618 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/README.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)    28417 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/antenna-pointing.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)    21199 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/api.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     7112 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/bitcoin.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     5842 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/docker.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     8077 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/dual-satellite.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     2133 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/frequency.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)    32815 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/hardware.md
+drwxr-xr-x   0 igorfreire   (501) staff       (20)        0 2023-07-12 11:01:38.520591 blocksat-cli-0.4.6/doc/img/
+-rw-r--r--   0 igorfreire   (501) staff       (20)   102112 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/api_architecture.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   149401 2022-05-30 19:13:44.000000 blocksat-cli-0.4.6/doc/img/azimuth.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    14581 2021-05-17 16:10:20.000000 blocksat-cli-0.4.6/doc/img/blockstream.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   139354 2022-05-30 19:13:44.000000 blocksat-cli-0.4.6/doc/img/elevation.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   159429 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/gqrx-centered.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   196623 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/gqrx-offset.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    15296 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/leandvb-pls-syms.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    15376 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/leandvb-pre-processed-iq.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    14716 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/leandvb-pre-processed-iq2.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    19167 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/leandvb-spectrum-centered.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    12948 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/leandvb-spectrum-offset.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    89325 2022-05-30 19:13:44.000000 blocksat-cli-0.4.6/doc/img/lnb_polarization.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    97965 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/img/monitoring-api-authentication.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    13082 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/s400_locked.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    33595 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/s400_rf_status.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)    12463 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/s400_searching.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)  1196013 2021-05-17 16:10:20.000000 blocksat-cli-0.4.6/doc/img/sat-ip-connections.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   333258 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/sdr_connections.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   141359 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/standalone_connections.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)   112570 2021-04-29 15:31:53.000000 blocksat-cli-0.4.6/doc/img/usb_connections.png
+-rw-r--r--   0 igorfreire   (501) staff       (20)     3715 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/monitoring.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     4869 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/quick-reference.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)      381 2022-01-07 18:50:41.000000 blocksat-cli-0.4.6/doc/receiver.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6326 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/s400.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     7711 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/sat-ip.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     6545 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/sdr.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1257 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/software.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)     5557 2023-07-06 21:32:20.000000 blocksat-cli-0.4.6/doc/tbs.md
+-rw-r--r--   0 igorfreire   (501) staff       (20)       38 2023-07-12 11:01:38.521682 blocksat-cli-0.4.6/setup.cfg
+-rw-r--r--   0 igorfreire   (501) staff       (20)     1335 2023-07-09 18:34:25.000000 blocksat-cli-0.4.6/setup.py
```

### Comparing `blocksat-cli-0.4.5/LICENSE` & `blocksat-cli-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/PKG-INFO` & `blocksat-cli-0.4.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: blocksat-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: Blockstream Satellite CLI
 Home-page: https://github.com/Blockstream/satellite
 Author: Blockstream Corp
 Author-email: satellite@blockstream.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: fec
 License-File: LICENSE
 
 # Blockstream Satellite CLI
 
 A command-line interface for configuring, running and monitoring a Blockstream
 Satellite receiver setup.
```

### Comparing `blocksat-cli-0.4.5/README.md` & `blocksat-cli-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksat_cli.egg-info/PKG-INFO` & `blocksat-cli-0.4.6/blocksat_cli.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: blocksat-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: Blockstream Satellite CLI
 Home-page: https://github.com/Blockstream/satellite
 Author: Blockstream Corp
 Author-email: satellite@blockstream.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: fec
 License-File: LICENSE
 
 # Blockstream Satellite CLI
 
 A command-line interface for configuring, running and monitoring a Blockstream
 Satellite receiver setup.
```

### Comparing `blocksat-cli-0.4.5/blocksat_cli.egg-info/SOURCES.txt` & `blocksat-cli-0.4.6/blocksat_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/api.py` & `blocksat-cli-0.4.6/blocksatcli/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,17 @@
     elif (args.demo):
         interface = "lo"
     else:
         # Infer the interface based on the user's setup
         user_info = blocksatcli_config.read_cfg_file(args.cfg, args.cfg_dir)
         interface = blocksatcli_config.get_net_if(user_info)
     logger.info("Listening on interface: {}".format(interface))
-    logger.info("Downloads will be saved at: {}".format(download_dir))
+
+    if not args.no_save:
+        logger.info("Downloads will be saved at: {}".format(download_dir))
 
     # A passphrase is required for decryption (but not for signature
     # verification)
     if (not args.plaintext and not args.no_password):
         gpg.prompt_passphrase('GPG keyring password for decryption: ')
 
     # Listen continuously
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/bidding.py` & `blocksat-cli-0.4.6/blocksatcli/api/bidding.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/demorx.py` & `blocksat-cli-0.4.6/blocksatcli/api/demorx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 import json
 import logging
 import time
 
 import requests
-import sseclient
 
 from .. import defs
 from . import net
 from .order import ApiOrder, API_CHANNEL_SSE_NAME
 from .pkt import BlocksatPkt, BlocksatPktHandler
 
 logger = logging.getLogger(__name__)
@@ -101,25 +100,22 @@
             if (byte_rate > 0):
                 tx_delay = len(pkt) / byte_rate
                 next_tx += tx_delay
                 sleep = next_tx - time.time()
                 if (sleep > 0):
                     time.sleep(sleep)
 
-    def _handle_event(self, event):
+    def _handle_event(self, event_data):
         """Handle event broadcast by the SSE server
 
         Args:
-            event : Event generated by the sseclient
+            event_data (dict): Event data.
 
         """
-        # Parse the order corresponding to the event
-        order = json.loads(event.data)
-
-        # Debug
+        order = json.loads(event_data)
         logger.debug("Order: " + json.dumps(order, indent=4, sort_keys=True))
 
         # Proceed when the event matches the target Tx trigger event
         if (order["status"] != self.tx_event):
             return
 
         self._handle_order(order)
@@ -204,20 +200,38 @@
 
                 sse_channel = API_CHANNEL_SSE_NAME[self.channel]
                 endpoint = '/admin/subscribe/' if self.admin else '/subscribe/'
                 r = requests.get(self.server + f"{endpoint}{sse_channel}",
                                  stream=True,
                                  cert=(self.tls_cert, self.tls_key))
                 r.raise_for_status()
-                client = sseclient.SSEClient(r)
+
                 logger.info("Connected. Waiting for events...\n")
 
                 # Continuously wait for events
-                for event in client.events():
-                    self._handle_event(event)
+                event_line = 'event:' + sse_channel
+                event_next = False
+                for line in r.iter_lines():
+                    if not line:
+                        continue
+
+                    dec_line = line.decode()
+
+                    if dec_line.startswith(':'):  # comment to be ignored
+                        continue
+
+                    logger.debug(line)
+
+                    if dec_line.startswith(event_line):
+                        event_next = True
+                        continue
+
+                    if event_next and dec_line.startswith('data:'):
+                        self._handle_event(dec_line.replace('data:', ''))
+                        event_next = False
 
             except requests.exceptions.HTTPError as e:
                 logger.error(e)
                 break
 
             except requests.exceptions.ChunkedEncodingError as e:
                 logger.debug(e)
@@ -244,15 +258,15 @@
                              tls_cert=self.tls_cert,
                              tls_key=self.tls_key)
         tx_set = set()
         while (True):
             try:
                 tx_orders = order_mgr.get_orders(['transmitting'],
                                                  self.channel,
-                                                 queue='queued')
+                                                 queue='transmitting')
 
                 # There can only be one order in transmitting state at a time
                 if len(tx_orders) > 1:
                     logger.warning("More than one order in transmitting "
                                    "state on channel {}".format(self.channel))
 
                 # Filter out any repeated orders (already transmitted), except
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/fec.py` & `blocksat-cli-0.4.6/blocksatcli/api/fec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """FEC Encoding/decoding"""
 import logging
 import random
 import struct
 from math import ceil, floor
 
-import zfec
+try:
+    import zfec
+    fec_supported = True
+except ImportError:
+    fec_supported = False
 
 from . import pkt
 
 logger = logging.getLogger(__name__)
 # FEC packet header:
 # Octet 0      : Object id
 # Octet 1      : Number of FEC objects
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/gpg.py` & `blocksat-cli-0.4.6/blocksatcli/api/gpg.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class Gpg():
 
     def __init__(self, gpghome, verbose=False, interactive=False):
         """Create GnuPG instance"""
         if (not os.path.exists(gpghome)):
-            os.mkdir(gpghome)
+            os.makedirs(gpghome)
             # Make sure only the owner has permissions to read, write, and
             # execute the GPG home directory
             os.chmod(gpghome, stat.S_IRWXU)
 
         self.interactive = interactive
         self.gpghome = gpghome
         self.passphrase = None
@@ -58,14 +58,18 @@
         # Password
         if (passphrase is None):
             self.prompt_passphrase('Please enter a passphrase to protect '
                                    'your key: ')
         else:
             self.set_passphrase(passphrase)
 
+        if not self.passphrase:
+            logger.error("Empty passphrase")
+            return
+
         # Generate key
         key_params = self.gpg.gen_key_input(key_type="RSA",
                                             key_length=1024,
                                             name_real=name,
                                             name_comment=comment,
                                             name_email=email,
                                             passphrase=self.passphrase)
@@ -109,32 +113,35 @@
             passphrase=self.passphrase)
         success = res is not None and res != ''
         if not success:
             logger.error("Bad passphrase.")
         return success
 
     def get_default_public_key(self):
-        """Get info corresponding to the first public key on the keyring
+        """Get the default (user) public key from the keyring
 
         Returns:
             Dictionary with key information such as 'fingerprint', 'keyid', and
-            'uids'.
+            'uids'. None if not found.
 
         """
-        return self.gpg.list_keys()[0]
+        for key in self.gpg.list_keys():
+            if key['fingerprint'] != defs.blocksat_pubkey:
+                return key
 
     def get_default_priv_key(self):
-        """Get info corresponding to the first private key on the keyring
+        """Get the default (user) private key from the keyring
 
         Returns:
             Dictionary with key information such as 'fingerprint', 'keyid', and
-            'uids'.
+            'uids'. None if not found.
 
         """
-        return self.gpg.list_keys(True)[0]
+        for key in self.gpg.list_keys(True):
+            return key  # return the first private key found
 
     def get_public_key(self, fingerprint):
         """Find a specific public key on the keyring and return the info dict
 
         Returns:
             Dictionary with key information such as 'fingerprint', 'keyid', and
             'uids'.
@@ -238,17 +245,14 @@
         logger.warning("Failed to import key {}".format(defs.blocksat_pubkey))
         return
 
     logger.info("Imported key {}".format(import_result.fingerprints[0]))
 
     gpg.gpg.trust_keys(defs.blocksat_pubkey, 'TRUST_ULTIMATE')
 
-    if (not is_gpg_keyring_set(gpg.gpghome)):
-        raise RuntimeError("GPG keyring configuration failed")
-
 
 def config_keyring(gpg, log_if_configured=False):
     """Configure the local keyring
 
     Create a keypair and import Blockstream's public key
 
     Args:
@@ -267,12 +271,11 @@
     name = util.string_input("User name represented by the key")
     email = util.string_input("E-mail address")
     comment = util.string_input("Comment to attach to the user ID",
                                 optional=True)
     gpg.create_keys(name, email, comment)
 
     # Import Blockstream's public key
-    #
-    # NOTE: the order is important here. Add Blockstream's public key only
-    # after adding the user key. With that, the user key becomes the first key
-    # on the keyring, which is used by default.
     import_bs_pubkey(gpg)
+
+    if (not is_gpg_keyring_set(gpg.gpghome)):
+        raise RuntimeError("GPG keyring configuration failed")
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/listen.py` & `blocksat-cli-0.4.6/blocksatcli/api/listen.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             # API message is ready to be decoded
             if (channel == ApiChannel.ALL.value):
                 logger.info("-------- API message {:d} (channel {:d})".format(
                     seq_num, pkt.chan_num))
             else:
                 logger.info("-------- API message {:d}".format(seq_num))
             logger.debug("Message source: {}:{}".format(addr[0], addr[1]))
-            logger.info("Fragments: {:d}".format(
+            logger.debug("Fragments: {:d}".format(
                 pkt_handler.get_n_frags(seq_num)))
 
             # Send confirmation of reception to API server
             order = ApiOrder(server_addr,
                              seq_num=seq_num,
                              tls_cert=tls_cert,
                              tls_key=tls_key)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/msg.py` & `blocksat-cli-0.4.6/blocksatcli/api/msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import struct
 import sys
 import time
 import zlib
 
 from .. import defs
-from .fec import Fec
+from .fec import Fec, fec_supported
 
 logger = logging.getLogger(__name__)
 # API message header:
 # Octets 0 - 254   : string with the file name
 # Octet 255        : bool indicating whether the message is text
 # Octets 256 - 259 : CRC32 checksum
 MSG_HEADER_FORMAT = '<255sxI'
@@ -119,16 +119,17 @@
         orig_data = self.data["original"]
         crc32 = zlib.crc32(orig_data)
         header = struct.pack(MSG_HEADER_FORMAT, self.filename.encode(), crc32)
 
         self.data['encapsulated'] = header + orig_data
 
         logger.debug("Checksum: {:d}".format(crc32))
-        logger.debug("Packed in data structure with a total of %d bytes" %
-                     (len(self.data['encapsulated'])))
+        logger.debug(
+            "Packed in data structure with a total of {:d} bytes".format(
+                len(self.data['encapsulated'])))
 
     def decapsulate(self):
         """Decapsulate the data structure
 
         Unpacks the CRC32 checksum and the file name out of the header. Then,
         validates the data integrity using the checksum.
 
@@ -154,20 +155,21 @@
         in_checksum = header[1]
 
         # Check the integrity of the payload
         payload = encap_data[MSG_HEADER_LEN:]
         calc_checksum = zlib.crc32(payload)
 
         if (calc_checksum != in_checksum):
-            logger.error("Checksum (%d) does not match the header value (%d)" %
-                         (calc_checksum, in_checksum))
+            logger.error(
+                "Checksum ({}) does not match the header value ({})".format(
+                    calc_checksum, in_checksum))
             return False
         else:
-            logger.info("File: %s\tChecksum: %d\tSize: %d bytes" %
-                        (self.filename, in_checksum, len(payload)))
+            logger.info("File: {}; Checksum: {}; Size: {:d} bytes".format(
+                self.filename, in_checksum, len(payload)))
 
         self.data['original'] = payload
         return True
 
     def encrypt(self, gpg, recipient, sign, trust):
         """Encrypt the data
 
@@ -183,30 +185,31 @@
             trust      : Skip key validation.
 
 
         """
         data = self.data['encapsulated'] if self.data['encapsulated'] \
             else self.data['original']
 
-        logger.debug("Encrypt for recipient %s" % (recipient))
+        logger.debug("Encrypt for recipient {}".format(recipient))
 
         if (sign and sign is not True):
-            logger.debug("Sign message using key %s" % (sign))
+            logger.debug("Sign message using key {}".format(sign))
 
         encrypted_obj = gpg.encrypt(data,
                                     recipient,
                                     always_trust=trust,
                                     sign=sign)
         if (not encrypted_obj.ok):
             logger.error(encrypted_obj.stderr)
             raise ValueError(encrypted_obj.status)
 
         self.data['encrypted'] = encrypted_obj.data
-        logger.debug("Encrypted version of the data structure has %d bytes" %
-                     (len(self.data['encrypted'])))
+        logger.debug(
+            "Encrypted version of the data structure has {:d} bytes".format(
+                len(self.data['encrypted'])))
 
     def decrypt(self, gpg, signer_filter=None):
         """Decrypt the data
 
         Args:
             gpg           : Gpg object.
             signer_filter : Fingerprint of a target signer. If the message is
@@ -216,39 +219,40 @@
             True if the decryption was successful.
 
         """
 
         decrypted_data = gpg.decrypt(self.data['encrypted'])
 
         if (not decrypted_data.ok):
-            logger.info("Size: %7d bytes\t Decryption: FAILED\t" %
-                        (len(self.data['encrypted'])) +
-                        "Not encrypted for us (%s)" % (decrypted_data.status))
+            logger.info(
+                "Size: {:d} bytes; Decryption: FAILED; ".format(
+                    len(self.data['encrypted'])) +
+                "Not encrypted for us ({})".format(decrypted_data.status))
             return False
 
         # Is the message digitally signed?
         if (decrypted_data.fingerprint is not None):
             signed_by = decrypted_data.fingerprint
             verified = decrypted_data.trust_level is not None
             sign_str_short = "Signed"
 
             if verified:
                 sign_str_long = \
-                    "Signed by %s (verified w/ trust level: %s)" % (
+                    "Signed by {} (verified w/ trust level: {})".format(
                         signed_by, decrypted_data.trust_text)
             else:
-                sign_str_long = "Signed by %s (unverified)" % (signed_by)
+                sign_str_long = "Signed by {} (unverified)".format(signed_by)
         else:
             sign_str_short = "Unsigned"
             sign_str_long = ""
             signed_by = None
             verified = False
 
-        logger.info("Encrypted size: %7d bytes\t Decryption: OK    \t%s" %
-                    (len(self.data['encrypted']), sign_str_short))
+        logger.info("Encrypted size: {:d} bytes; Decryption: OK; {}".format(
+            len(self.data['encrypted']), sign_str_short))
 
         if (len(sign_str_long) > 0):
             logger.info(sign_str_long)
 
         if (signer_filter is not None):
             if (not signed_by):
                 logger.warning("Dropping message - not signed")
@@ -259,15 +263,16 @@
                                "sender")
                 return False
 
             if (decrypted_data.trust_level < decrypted_data.TRUST_FULLY):
                 logger.warning("Dropping message - signature unverified")
                 return False
 
-        logger.info("Decrypted size: %7d bytes" % (len(str(decrypted_data))))
+        logger.info("Decrypted size: {:d} bytes".format(
+            len(str(decrypted_data))))
 
         # We can't know whether decrypted data is encapsulated or not. So, for
         # now, put the data into both fields. If the decrypted data is
         # encapsulated, eventually "decapsulate" will be called and will
         # overwrite the "original" data container.
         self.data['original'] = decrypted_data.data
         self.data['encapsulated'] = decrypted_data.data
@@ -290,20 +295,21 @@
             gpg      : Gpg object.
             sign_key : Fingerprint to use for signing. If set to None, try with
                        the first private key on the keyring.
 
         """
         data = self.data['original']
 
-        logger.debug("Sign message using key %s" % (sign_key))
+        logger.debug("Sign message using key {}".format(sign_key))
 
         signed_obj = gpg.sign(data, sign_key)
 
-        logger.debug("Signed version of the data structure has %d bytes" %
-                     (len(signed_obj.data)))
+        logger.debug(
+            "Signed version of the data structure has {:d} bytes".format(
+                len(signed_obj.data)))
 
         self.data['original'] = signed_obj.data
 
     def verify(self, gpg, signer):
         """Verify signed (but non-encrypted) message from target signer
 
         Detects whether the clearsigned plaintext messages comes from the
@@ -374,14 +380,15 @@
         the last chunk is padded if necessary.
 
         Args:
             overhead : Percentage of the FEC chunks to add as overhead
                        (rounded up).
 
         """
+        assert fec_supported
         fec = Fec(overhead)
         self.data['fec_encoded'] = fec.encode(self.get_data())
 
     def fec_decode(self):
         """Forward error correction (FEC) decoding
 
         Try to decode the FEC-encoded message held in the internal container,
@@ -390,14 +397,15 @@
         Note:
             This function should be called only when the FEC-encoded object is
             decodable. Otherwise, it throws a RuntimeError exception. Use the
             "is_fec_decodable()" method before calling it.
 
         """
         assert (self.data['fec_encoded'] is not None)
+        assert fec_supported
 
         fec = Fec()
         decoded_data = fec.decode(self.data['fec_encoded'])
 
         # The encoded data should be decodable at this point
         if (not decoded_data):
             raise RuntimeError("Failed to decode the FEC-encoded message")
@@ -413,14 +421,16 @@
         """Check if the FEC-encoded data is decodable
 
         Returns:
             (bool) Whether the FEC-encoded data is decodable.
 
         """
         assert (self.data['fec_encoded'] is not None)
+        if not fec_supported:
+            return False
 
         fec = Fec()
         res = fec.decode(self.data['fec_encoded'])
         return res is not False
 
     def save(self, dst_dir, target='original'):
         """Save data into a file
@@ -531,14 +541,18 @@
     Returns:
         Message as an ApiMsg object.
 
     """
     if ((not plaintext or sign) and gpg is None):
         raise ValueError("Gpg object is required for encryption or signing")
 
+    if fec and not fec_supported:
+        raise ValueError(
+            "FEC support disabled. Please install zfec or blocksat-cli[fec].")
+
     msg = ApiMsg(data, filename=filename)
 
     # If transmitting a plaintext message, it could still be clearsigned.
     if (plaintext and sign):
         if (sign_key):
             # Make sure the key exists
             gpg.get_priv_key(sign_key)
@@ -606,14 +620,18 @@
         ApiMsg if the message is succesfully decoded, None otherwise.
 
     """
     if ((not plaintext or sender) and gpg is None):
         raise ValueError("Gpg object is required for decryption/verification")
 
     if (fec):
+        if not fec_supported:
+            raise ValueError("FEC support disabled. "
+                             "Please install zfec or blocksat-cli[fec].")
+
         msg = ApiMsg(data, msg_format="fec_encoded")
         msg.fec_decode()
         data = msg.data['original']
         del msg  # after extracting the data, re-create a new ApiMsg below
 
     if (plaintext):
         if (decapsulate):
@@ -629,15 +647,15 @@
             # from the browser at: https://blockstream.com/satellite-queue/.
             msg = ApiMsg(data, msg_format="original")
 
         # If filtering clearsigned messages, verify
         if (sender and not msg.verify(gpg, sender)):
             return
 
-        logger.info("Message Size: {:d} bytes\tSaving in plaintext".format(
+        logger.info("Size: {:d} bytes".format(
             msg.get_length(target='original')))
 
     else:
         # Cast data into ApiMsg object in encrypted form
         msg = ApiMsg(data, msg_format="encrypted")
 
         # Try to decrypt the data:
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/net.py` & `blocksat-cli-0.4.6/blocksatcli/api/net.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/order.py` & `blocksat-cli-0.4.6/blocksatcli/api/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 }
 SENDABLE_API_CHANNELS = [x for x in API_CHANNELS if x != ApiChannel.ALL.value]
 PAID_API_CHANNELS = [ApiChannel.USER.value]
 ORDER_STATUS = [
     'pending', 'paid', 'transmitting', 'sent', 'received', 'cancelled',
     'expired', 'confirming'
 ]
-ORDER_QUEUES = ['pending', 'queued', 'sent']
+ORDER_QUEUES = [
+    'pending', 'paid', 'transmitting', 'confirming', 'queued', 'sent',
+    'rx-pending', 'received', 'retransmitting'
+]
 
 
 class ApiOrder:
     """API Transmission Order
 
     Handles the payment/bidding for transmission of API messages.
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/pkt.py` & `blocksat-cli-0.4.6/blocksatcli/api/pkt.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_bidding.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_bidding.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_fec.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_fec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 import random
 import string
 import unittest
 from . import fec, pkt
 
 
+@unittest.skipIf(not fec.fec_supported, "FEC support disabled")
 class TestFec(unittest.TestCase):
 
     def _rnd_string(self, n_bytes):
         """Generate a random string with the given number of bytes"""
         return ''.join(
             random.choice(string.ascii_letters + string.digits)
             for _ in range(n_bytes)).encode()
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_listen.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_listen.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_msg.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import math
 import os
 import random
 import string
+from unittest import skipIf
+
 from . import msg, pkt, fec
 from .gpg import Gpg
 
 from ..test_helpers import TestEnv
 
 
 class TestApi(TestEnv):
@@ -269,14 +271,15 @@
         self.assertTrue(rx_msg2.verify(gpg, signer))
         self.assertFalse(rx_msg3.verify(gpg, signer))
 
         # The verifiction step should remove the signature and leave the
         # original data only
         self.assertEqual(rx_msg2.data['original'], data)
 
+    @skipIf(not fec.fec_supported, "FEC support disabled")
     def test_fec_encoding_decoding(self):
         """Test FEC encoding and decoding"""
         fec_overhead = 0.1
 
         # Random data
         n_bytes = 100000
         data = ''.join(
@@ -353,14 +356,15 @@
         # already, but the contents do not match.
         self.assertTrue(os.path.exists(dst_file2))
 
         # Clean up
         os.remove(dst_file)
         os.remove(dst_file2)
 
+    @skipIf(not fec.fec_supported, "FEC support disabled")
     def test_msg_generator_decoder_wrappers(self):
         """Test the message generation and decoding wrappers"""
         data = bytes([0, 1, 2, 3])
         fec_overhead = 0.5
 
         # Set up GPG keyring with two keypairs
         gpg = self._setup_gpg()
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_net.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_net.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/api/test_pkt.py` & `blocksat-cli-0.4.6/blocksatcli/api/test_pkt.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/bitcoin.py` & `blocksat-cli-0.4.6/blocksatcli/bitcoin.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,39 @@
 
     cfg.add_opt("udpmulticast",
                 _udpmulticast(dev=interface, src_addr=src_addr, label=label))
 
     return cfg
 
 
+def create_config_file(abs_path, info, ifname, concat=False, stdout=False):
+    """Generate bitcoin configuration file"""
+    # Generate configuration object
+    cfg = _gen_cfgs(info, ifname)
+
+    # Load and concatenate pre-existing configurations
+    if concat and os.path.exists(abs_path):
+        with open(abs_path, "r") as fd:
+            prev_cfg_text = fd.read()
+            cfg.load_text_cfg(prev_cfg_text)
+
+    # Export configurations to text format
+    cfg_text = cfg.text()
+
+    # Print configurations to stdout and don't save them
+    if stdout:
+        print(cfg_text)
+        return
+
+    with open(abs_path, "w") as fd:
+        fd.write(cfg_text)
+
+    print("Saved")
+
+
 def subparser(subparsers):  # pragma: no cover
     """Argument parser of bitcoin-conf command"""
     p = subparsers.add_parser(
         'bitcoin-conf',
         aliases=['btc'],
         description="Generate Bitcoin configuration file",
         help='Generate Bitcoin configuration file',
@@ -131,54 +156,35 @@
         home = os.path.expanduser("~")
         path = os.path.join(home, ".bitcoin")
     else:
         path = os.path.abspath(args.datadir)
 
     conf_file = "bitcoin.conf"
     abs_path = os.path.join(path, conf_file)
-
-    # Network interface
-    ifname = config.get_net_if(info)
-
-    # Generate configuration object
-    cfg = _gen_cfgs(info, ifname)
-
-    # Load and concatenate pre-existing configurations
-    if args.concat and os.path.exists(abs_path):
-        with open(abs_path, "r") as fd:
-            prev_cfg_text = fd.read()
-            cfg.load_text_cfg(prev_cfg_text)
-
-    # Export configurations to text format
-    cfg_text = cfg.text()
-
-    # Print configurations to stdout and don't save them
-    if (args.stdout):
-        print(cfg_text)
-        return
+    save_file = not args.stdout
 
     # Proceed to saving configurations
-    print("Save {} at {}".format(conf_file, path))
-
-    if (not util.ask_yes_or_no("Proceed?")):
-        print("Aborted")
-        return
-
-    if not os.path.exists(path):
-        os.makedirs(path)
-
-    if os.path.exists(abs_path) and not args.concat:
-        if (not util.ask_yes_or_no("File already exists. Overwrite?")):
+    if save_file:
+        print("Save {} at {}".format(conf_file, path))
+        if not util.ask_yes_or_no("Proceed?"):
             print("Aborted")
             return
 
-    with open(abs_path, "w") as fd:
-        fd.write(cfg_text)
+        if not os.path.exists(path):
+            os.makedirs(path)
 
-    print("Saved")
+        if os.path.exists(abs_path) and not args.concat:
+            if (not util.ask_yes_or_no("File already exists. Overwrite?")):
+                print("Aborted")
+                return
+
+    # Network interface
+    ifname = config.get_net_if(info)
+
+    create_config_file(abs_path, info, ifname, args.concat, args.stdout)
 
     if (info['setup']['type'] == defs.linux_usb_setup_type):
         print()
         util.fill_print(
             "NOTE: {} was configured assuming the dvbnet interface is "
             "named {}. You can check if this is the case after launching the "
             "receiver by running:".format(conf_file, ifname))
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/cache.py` & `blocksat-cli-0.4.6/blocksatcli/cache.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/config.py` & `blocksat-cli-0.4.6/blocksatcli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import textwrap
 from argparse import ArgumentDefaultsHelpFormatter, Namespace
 from decimal import Decimal, getcontext
 from ipaddress import IPv4Address
 from pprint import pprint, pformat
 
-from . import util, defs
+from . import util, defs, gqrx
 
 logger = logging.getLogger(__name__)
 
 
 def _cfg_satellite():
     """Configure satellite covering the user"""
     os.system('clear')
@@ -168,46 +168,90 @@
                 resp = input(
                     "Inform the two extreme frequencies (in MHz) of "
                     "your LNB's frequency range, separated by comma: ")
                 in_range = [float(x) for x in resp.split(",")]
             except ValueError:
                 continue
 
-        if (in_range[1] < in_range[0]):
-            in_range = []
-            print("Please, provide the lowest frequency first, followed by "
-                  "the highest.")
-            continue
-
-        if (in_range[0] < 3000 or in_range[1] < 3000):
-            in_range = []
-            print("Please, provide the frequencies in MHz.")
-            continue
-
-        if not _sat_freq_in_lnb_range(sat, {'in_range': in_range}):
-            print(
-                f"Please, choose a frequency range covering the {sat['name']} "
-                f"downlink frequency of {sat['dl_freq']} MHz")
+        is_valid, msg = _validate_lnb_freq_range(in_range, sat)
+        if not is_valid:
+            print(msg)
             in_range = []
             continue
 
         break
 
     return in_range
 
 
+def _validate_lnb_freq_range(freq_range, sat):
+    """Validate the LNB frequency range
+
+    Args:
+        freq_range (list): Two extreme LNB frequencies.
+        sat (dict): Dictionary with the Satellite information.
+
+    Returns:
+        is_valid (bool): Whether the two frequencies are valid.
+        msg (str): Detailed error message if the frequencies are invalid.
+
+    """
+    assert (isinstance(freq_range, list))
+
+    is_valid = False
+    msg = ""
+
+    if (freq_range[1] < freq_range[0]):
+        msg = ("Please, provide the lowest frequency first, followed by "
+               "the highest.")
+    elif (freq_range[0] < 3000 or freq_range[1] < 3000):
+        msg = "Please, provide the frequencies in MHz."
+    elif not _sat_freq_in_lnb_range(sat, {'in_range': freq_range}):
+        msg = (f"Please, choose a frequency range covering the {sat['name']} "
+               f"downlink frequency of {sat['dl_freq']} MHz")
+    else:
+        is_valid = True
+
+    return is_valid, msg
+
+
+def _validate_lnb_lo_freq(lo_freq, single_lo=False):
+    is_valid = False
+    msg = ""
+
+    if single_lo:
+        assert (isinstance(lo_freq, float))
+        if (lo_freq < 3000):
+            msg = "Please, provide the frequencies in MHz."
+        else:
+            is_valid = True
+
+    else:
+        assert (isinstance(lo_freq, list))
+        if (lo_freq[1] < lo_freq[0]):
+            msg = ("Please, provide the low LO frequency first, followed by "
+                   "the high LO frequency.")
+        elif (lo_freq[0] < 3000 or lo_freq[1] < 3000):
+            msg = "Please, provide the frequencies in MHz."
+        else:
+            is_valid = True
+
+    return is_valid, msg
+
+
 def _ask_lnb_lo(single_lo=True):
     """Prompt the user for the LNB's LO frequencies"""
     if (single_lo):
         while (True):
             lo_freq = util.typed_input("LNB LO frequency in MHz",
                                        in_type=float)
 
-            if (lo_freq < 3000):
-                print("Please, provide the frequencies in MHz.")
+            is_valid, msg = _validate_lnb_lo_freq(lo_freq, single_lo)
+            if (not is_valid):
+                print(msg)
                 continue
 
             break
         return lo_freq
 
     lo_freq = []
     while (True):
@@ -215,23 +259,18 @@
             try:
                 resp = input("Inform the two LO frequencies in MHz, separated "
                              "by comma: ")
                 lo_freq = [float(x) for x in resp.split(",")]
             except ValueError:
                 continue
 
-        if (lo_freq[1] < lo_freq[0]):
+        is_valid, msg = _validate_lnb_lo_freq(lo_freq, single_lo)
+        if (not is_valid):
             lo_freq = []
-            print("Please, provide the low LO frequency first, followed by "
-                  "the high LO frequency.")
-            continue
-
-        if (lo_freq[0] < 3000 or lo_freq[1] < 3000):
-            lo_freq = []
-            print("Please, provide the frequencies in MHz.")
+            print(msg)
             continue
 
         break
 
     return lo_freq
 
 
@@ -431,14 +470,37 @@
     elif (setup['type'] == defs.sdr_setup_type):
         question = ("Are you using one of the LNB power inserters below?")
         lnb["psu_voltage"] = _ask_psu_voltage(question)
 
     return lnb
 
 
+def _calc_if_freq(dl_freq, lo_freq, band):
+    """Calculate the IF frequency for downlink reception with a given LO
+
+    Args:
+        dl_freq : Downlink frequency.
+        lo_freq : LNB LO frequency.
+        band    : Band of the satellite.
+
+    Returns:
+        float: IF frequency.
+
+    """
+    if (band.lower() == "c"):
+        if_freq = float(Decimal(lo_freq) - Decimal(dl_freq))
+    elif (band.lower() == "ku"):
+        if_freq = float(Decimal(dl_freq) - Decimal(lo_freq))
+    else:
+        logging.error("Invalid satellite band: {}".format(band))
+        sys.exit(1)
+
+    return round(if_freq, 2)
+
+
 def _cfg_frequencies(sat, lnb, setup):
     """Print summary of frequencies
 
     Inform the downlink RF frequency, the LNB LO frequency and the L-band
     frequency to be configured in the receiver.
 
     Args:
@@ -450,106 +512,143 @@
 
     if (sat['band'].lower() == "ku"):
         if (lnb['universal']):
             assert (isinstance(lnb['lo_freq'], list)), \
                 "A Universal LNB must have a list with two LO frequencies"
             assert (len(lnb['lo_freq']) == 2), \
                 "A Universal LNB must have two LO frequencies"
-
             if (sat['dl_freq'] > defs.ku_band_thresh):
                 lo_freq = lnb['lo_freq'][1]
             else:
                 lo_freq = lnb['lo_freq'][0]
         else:
             lo_freq = lnb['lo_freq']
-
-        if_freq = float(Decimal(sat['dl_freq']) - Decimal(lo_freq))
-
     elif (sat['band'].lower() == "c"):
         lo_freq = lnb['lo_freq']
-        if_freq = float(Decimal(lo_freq) - Decimal(sat['dl_freq']))
     else:
         raise ValueError("Unknown satellite band")
 
+    if_freq = _calc_if_freq(sat['dl_freq'], lo_freq, sat['band'])
+
     if (if_freq < setup['tun_range'][0] or if_freq > setup['tun_range'][1]):
         logging.error("Your LNB yields an L-band frequency that is out of "
                       "the tuning range of the {} receiver.".format(
                           _get_rx_marketing_name(setup)))
         sys.exit(1)
 
     return {'dl': sat['dl_freq'], 'lo': lo_freq, 'l_band': if_freq}
 
 
-def _cfg_chan_conf(info, chan_file, yes=False):
-    """Generate the channels.conf file"""
+def _gen_chan_conf(info):
+    """Generate the content for the channel configuration file
 
-    util.print_header("Channel Configuration")
+    Returns:
+        dict: Dictionary with the keys and values to be written in the channel
+        configuration file.
+    """
+    chan_conf = {}
+    chan_conf['DELIVERY_SYSTEM'] = 'DVBS2'
+    chan_conf['FREQUENCY'] = str(int(info['sat']['dl_freq'] * 1000))
+    if (info['lnb']['pol'].lower() == "dual" and 'v1_pointed' in info['lnb']
+            and info['lnb']['v1_pointed']):
+        # If a dual-polarization LNB is already pointed for Blocksat v1,
+        # then we must use the polarization that the LNB was pointed to
+        # originally, regardless of the satellite signal's polarization. In
+        # v1, what mattered the most was the power supply voltage, which
+        # determined the polarization of the dual polarization LNBs. If the
+        # power supply provides voltage >= 18 (often the case), then the
+        # LNB necessarily operates currently with horizontal polarization.
+        # Thus, on channels.conf we must use the same polarization in order
+        # for the DVB adapter to supply the 18VDC voltage.
+        if (info['lnb']["v1_psu_voltage"] >= 16):  # 16VDC threshold
+            chan_conf['POLARIZATION'] = 'HORIZONTAL'
+        else:
+            chan_conf['POLARIZATION'] = 'VERTICAL'
+    else:
+        if (info['sat']['pol'] == 'V'):
+            chan_conf['POLARIZATION'] = 'VERTICAL'
+        else:
+            chan_conf['POLARIZATION'] = 'HORIZONTAL'
+    chan_conf['SYMBOL_RATE'] = str(defs.sym_rate[info['sat']['alias']])
+    chan_conf['INVERSION'] = 'AUTO'
+    chan_conf['MODULATION'] = 'QPSK'
+    chan_conf['VIDEO_PID'] = "+".join([str(x) for x in defs.pids])
+    return chan_conf
 
-    print(
-        textwrap.fill("This step will generate the channel configuration "
-                      "file that is required when launching the USB "
-                      "receiver in Linux.") + "\n")
+
+def write_chan_conf(info, chan_file, yes=False, regeneration=False):
+    """Generate the channels.conf file"""
+
+    if not regeneration:
+        util.print_header("Channel Configuration")
+        print(
+            textwrap.fill("This step will generate the channel configuration "
+                          "file that is required when launching the USB "
+                          "receiver in Linux.") + "\n")
+    else:
+        logger.info("Regenerating channel configuration file...")
 
     if (os.path.isfile(chan_file)):
-        print("Found previous %s file:" % (chan_file))
+        if not regeneration:
+            print("Found previous %s file:" % (chan_file))
 
         if (yes or util.ask_yes_or_no("Remove and regenerate file?")):
             os.remove(chan_file)
         else:
             print("Configuration aborted.")
             return
 
     with open(chan_file, 'w') as f:
+        chan_config = _gen_chan_conf(info)
         f.write('[blocksat-ch]\n')
-        f.write('\tDELIVERY_SYSTEM = DVBS2\n')
-        f.write('\tFREQUENCY = %u\n' % (int(info['sat']['dl_freq'] * 1000)))
-        if (info['lnb']['pol'].lower() == "dual"
-                and 'v1_pointed' in info['lnb'] and info['lnb']['v1_pointed']):
-            # If a dual-polarization LNB is already pointed for Blocksat v1,
-            # then we must use the polarization that the LNB was pointed to
-            # originally, regardless of the satellite signal's polarization. In
-            # v1, what mattered the most was the power supply voltage, which
-            # determined the polarization of the dual polarization LNBs. If the
-            # power supply provides voltage >= 18 (often the case), then the
-            # LNB necessarily operates currently with horizontal polarization.
-            # Thus, on channels.conf we must use the same polarization in order
-            # for the DVB adapter to supply the 18VDC voltage.
-            if (info['lnb']["v1_psu_voltage"] >= 16):  # 16VDC threshold
-                f.write('\tPOLARIZATION = HORIZONTAL\n')
-            else:
-                f.write('\tPOLARIZATION = VERTICAL\n')
-        else:
-            if (info['sat']['pol'] == 'V'):
-                f.write('\tPOLARIZATION = VERTICAL\n')
-            else:
-                f.write('\tPOLARIZATION = HORIZONTAL\n')
-        f.write('\tSYMBOL_RATE = {}\n'.format(
-            defs.sym_rate[info['sat']['alias']]))
-        f.write('\tINVERSION = AUTO\n')
-        f.write('\tMODULATION = QPSK\n')
-        pids = "+".join([str(x) for x in defs.pids])
-        f.write('\tVIDEO_PID = {}\n'.format(pids))
+        for k, v in chan_config.items():
+            f.write(f'\t{k} = {v}\n')
 
-    print("File \"%s\" saved." % (chan_file))
+    logger.info("File {} saved.".format(chan_file))
 
     with open(chan_file, 'r') as f:
         logging.debug(f.read())
 
 
 def _parse_chan_conf(chan_file):
-    """Convert channel.conf file contents to dictionary"""
+    """Read channel.conf file and parse contents into a dictionary"""
     chan_conf = {}
     with open(chan_file, 'r') as f:
         lines = f.read().splitlines()
-        for line in lines[1:]:
+        for line in lines[1:]:  # skip the channel name
             key, val = line.split('=')
             chan_conf[key.strip()] = val.strip()
     return chan_conf
 
 
+def get_chan_file_path(cfg_dir, cfg_name):
+    """Get the path to the channels configuration file"""
+    return os.path.join(cfg_dir, cfg_name + '-channel.conf')
+
+
+def verify_chan_conf(info):
+    """Verify if channel.conf file content is up-to-date
+
+    Args:
+        info (dict): User's info.
+
+    Returns:
+        bool: True if the file is up-to-date or false otherwise.
+
+    """
+    if 'channel' not in info['setup'] or not info['setup']['channel']:
+        return False
+
+    chan_file = info['setup']['channel']
+    new_chan_cfg = _gen_chan_conf(info)
+    old_chan_cfg = _parse_chan_conf(chan_file)
+
+    return new_chan_cfg == old_chan_cfg
+
+
 def _cfg_file_name(cfg_name, directory):
     """Get the name of the configuration JSON file"""
     # Remove paths
     basename = os.path.basename(cfg_name)
     # Remove extension
     noext = os.path.splitext(basename)[0]
     # Add JSON extension
@@ -582,25 +681,38 @@
             new_dl_freq = 11452.1
         if info['sat']['alias'] == "T11N EU" and \
                 info['sat']['dl_freq'] == 11484.3:
             new_dl_freq = 11505.4
         if info['sat']['alias'] == "G18" and \
                 info['sat']['dl_freq'] == 12016.4:
             new_dl_freq = 11913.4
+        if info['sat']['alias'] == "T18V C" and \
+                info['sat']['dl_freq'] == 4053.83:
+            new_dl_freq = 4057.4
 
         if new_dl_freq is not None:
             logger.info(
                 "Updating the {} DL frequency from {} MHz to {} MHz".format(
                     info['sat']['alias'], info['sat']['dl_freq'], new_dl_freq))
             info['sat']['dl_freq'] = new_dl_freq
             info['freqs']['dl'] = new_dl_freq
-            info['freqs']['l_band'] = round(new_dl_freq - info['freqs']['lo'],
-                                            2)
+            info['freqs']['l_band'] = _calc_if_freq(new_dl_freq,
+                                                    info['freqs']['lo'],
+                                                    info['sat']['band'])
             updated = True
 
+    if updated and 'setup' in info and info['setup'][
+            'type'] == defs.linux_usb_setup_type:
+        if not verify_chan_conf(info):
+            cfg_dir = os.path.dirname(cfg_file)
+            cfg_name = os.path.basename(cfg_file)
+            cfg_name_no_ext = os.path.splitext(cfg_name)[0]
+            chan_file = get_chan_file_path(cfg_dir, cfg_name_no_ext)
+            write_chan_conf(info, chan_file, yes=True, regeneration=True)
+
     if updated:
         _write_cfg_file(cfg_file, info)
 
 
 def _rst_cfg_file(cfg_file):
     """Reset a previous configuration file in case it exists"""
     info = _read_cfg_file(cfg_file)
@@ -655,14 +767,27 @@
     vendeor-model string.
 
     """
     return (user_info['setup']['vendor'] + " " +
             user_info['setup']['model']).strip()
 
 
+def get_rx_label(user_info):
+    """Return the label of the target receiver"""
+    target_map = {
+        "sdr": defs.sdr_setup_type,
+        "usb": defs.linux_usb_setup_type,
+        "standalone": defs.standalone_setup_type,
+        "sat-ip": defs.sat_ip_setup_type
+    }
+    target = user_info['setup']['type']
+
+    return next(key for key, val in target_map.items() if val == target)
+
+
 def get_satellite_name(sat):
     """Return string with satellite name"""
     return f"{sat['name']} ({sat['alias']})"
 
 
 def get_antenna_model(user_info):
     """Return string with the antenna model"""
@@ -781,17 +906,22 @@
 
     if not os.path.exists(args.cfg_dir):
         os.makedirs(args.cfg_dir)
 
     # Channel configuration file
     if (user_setup['type'] == defs.linux_usb_setup_type):
         chan_file = os.path.join(args.cfg_dir, args.cfg + "-channel.conf")
-        _cfg_chan_conf(user_info, chan_file)
+        write_chan_conf(user_info, chan_file)
         user_info['setup']['channel'] = chan_file
 
+    # Gqrx configuration
+    if (user_setup['type'] == defs.sdr_setup_type):
+        os.system('clear')
+        gqrx._configure(user_info)
+
     # Create the JSON configuration file
     _write_cfg_file(cfg_file, user_info)
 
     os.system('clear')
     util.print_header("JSON configuration file")
     print("Saved configurations on %s" % (cfg_file))
 
@@ -850,36 +980,36 @@
 
     pr_cfgs = get_readable_cfg(info)
 
     if args.json:
         print(json.dumps(pr_cfgs, indent=4))
         return
 
-    box_size = 62
+    box_size = 67
     box_line = "-" * box_size
 
     for category in pr_cfgs:
         print(f"\n{category}")
         print(box_line)
         for key, pr_cfg in pr_cfgs[category].items():
-            print("| {:30s} | {:25s} |".format(key, pr_cfg))
+            print("| {:30s} | {:30s} |".format(key, pr_cfg))
         print(box_line)
 
 
 def channel(args):
     """Configure the channels.conf file directly"""
     user_info = read_cfg_file(args.cfg, args.cfg_dir)
     if (user_info is None):
         return
 
     # Channel configuration file
     if (user_info['setup']['type'] != defs.linux_usb_setup_type):
         raise TypeError("Invalid command for {} receivers".format(
             user_info['setup']['type']))
 
-    chan_file = os.path.join(args.cfg_dir, args.cfg + "-channel.conf")
-    _cfg_chan_conf(user_info, chan_file)
+    chan_file = get_chan_file_path(args.cfg_dir, args.cfg)
+    write_chan_conf(user_info, chan_file)
 
     # Overwrite the channels.conf path in case it is changing from a previous
     # version of the CLI when the conf file name was not bound to the cfg name
     user_info['setup']['channel'] = chan_file
     write_cfg_file(args.cfg, args.cfg_dir, user_info)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/defs.py` & `blocksat-cli-0.4.6/blocksatcli/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     'dl_freq': 11505.4,
     'band': "Ku",
     'pol': "V",
     'ip': "172.16.235.25"
 }, {
     'name': "Telstar 18V C Band",
     'alias': "T18V C",
-    'dl_freq': 4053.83,
+    'dl_freq': 4057.4,
     'band': "C",
     'pol': "H",
     'ip': "172.16.235.41"
 }, {
     'name': "Telstar 18V Ku Band",
     'alias': "T18V Ku",
     'dl_freq': 11506.75,
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/dependencies.py` & `blocksat-cli-0.4.6/blocksatcli/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,27 +678,28 @@
     # ov9650.ko undefined!": disable ov9650 from the build. The problem was
     # observed on kernel versions 5.3.7 and 5.7.7. Apply the workaround for any
     # version < 5.8.
     if (distro_id == "fedora"
             and LooseVersion(linux_release) < LooseVersion('5.8')):
         disable_list.append("VIDEO_OV9650")
 
-    # On Raspbian, disable RC/IR support and disable the MN88436 drivers to
-    # avoid the __aeabi_ldivmod/__aeabi_uldivmod undefined errors. Also,
-    # disable SAA7146 which lead to
-    # saa7146_pgtable_free/saa7146_pgtable_alloc/saa7146_pgtable_build_single
-    # undefined when running on a RPi3 B+ with kernel 5.10.63-v7+.
+    # On Raspbian, disable the MN88436 drivers to avoid the
+    # __aeabi_ldivmod/__aeabi_uldivmod undefined errors.
     if (distro_id == "raspbian"):
+        disable_list.append("DVB_MN88436")
+
+    # Disable RC/IR support
+    if (distro_id == "raspbian"
+            or LooseVersion(linux_release) >= LooseVersion('6.0')):
         runner.run(
             ["sed", "-i", "-r", "s/(^CONFIG.*_RC.*=)./\1n/g", "v4l/.config"],
             cwd=media_build_dir)
         runner.run(
             ["sed", "-i", "-r", "s/(^CONFIG.*_IR.*=)./\1n/g", "v4l/.config"],
             cwd=media_build_dir)
-        disable_list.append("DVB_MN88436")
 
     if args.disable is not None:
         disable_list.extend(args.disable)
 
     for module in disable_list:
         logger.debug("Disabling module {}".format(module))
         runner.run([
@@ -781,14 +782,23 @@
     Args:
         model: USB receiver model.
 
     Returns:
         True if the drivers are installed or False otherwise.
 
     """
+
+    # Bypass the driver verification if the following env var is set. This is
+    # useful in a docker container env, in which case the kernel modules are
+    # installed in the docker host instead of the container.
+    no_check = os.getenv('BLOCKSAT_NO_USB_DRIVERS_CHECK',
+                         'False').lower() in ('true', '1', 't')
+    if no_check:
+        return True
+
     module_map = {
         "5927": "dvb-usb-tbs5927.ko",
         "5520SE": "dvb-usb-tbs5520se.ko"
     }
     if model is None:
         models = list(module_map.keys())
     else:
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/gpg/87D07253F69E4CD8629B0A21A94A007EC9D4458C.gpg` & `blocksat-cli-0.4.6/blocksatcli/gpg/87D07253F69E4CD8629B0A21A94A007EC9D4458C.gpg`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/gqrx.py` & `blocksat-cli-0.4.6/blocksatcli/gqrx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Generate gqrx configurations"""
 import os
+import textwrap
 from argparse import ArgumentDefaultsHelpFormatter
+
 from . import config, util
-import textwrap
 
 
 def subparser(subparsers):  # pragma: no cover
     p = subparsers.add_parser('gqrx-conf',
                               aliases=['gqrx'],
                               description="Generate gqrx configurations",
                               help='Generate gqrx configurations',
@@ -23,32 +24,16 @@
                    to configuration prompts"')
 
     p.set_defaults(func=configure)
 
     return subparser
 
 
-def configure(args):
-    """Configure GQRX"""
-    interactive = not args.yes
-    info = config.read_cfg_file(args.cfg, args.cfg_dir)
-
-    if (info is None):
-        return
-
-    util.print_header("Gqrx Conf Generator")
-
-    if args.path is None:
-        home = os.path.expanduser("~")
-        path = os.path.join(home, ".config", "gqrx")
-    else:
-        path = args.path
-
-    conf_file = "default.conf"
-    abs_path = os.path.join(path, conf_file)
+def gqrx_config(cfg_path, info, interactive=True):
+    """Generate Gqrx configuration file"""
 
     default_gains = r'@Variant(\0\0\0\b\0\0\0\x2\0\0\0\x6\0L\0N\0\x41\0\0' + \
         r'\0\x2\0\0\x1\x92\0\0\0\x4\0I\0\x46\0\0\0\x2\0\0\0\xcc)'
 
     cfg = """
     [General]
     configversion=2
@@ -71,26 +56,52 @@
     demod=0
     """.format(
         int(info['freqs']['dl'] * 1e6),
         default_gains,
         int(info['freqs']['lo'] * 1e6),
     )
 
-    print("Save {} at {}/".format(conf_file, path))
+    cfg_dir = os.path.dirname(cfg_path)
+    if not os.path.exists(cfg_dir):
+        os.makedirs(cfg_dir)
 
-    if (interactive and not util.ask_yes_or_no("Proceed?")):
-        print("Aborted")
-        return
-
-    if not os.path.exists(path):
-        os.makedirs(path)
-
-    if os.path.exists(abs_path):
+    if os.path.exists(cfg_path):
         if (interactive
                 and not util.ask_yes_or_no("File already exists. Overwrite?")):
             print("Aborted")
             return
 
-    with open(abs_path, "w") as file:
+    with open(cfg_path, "w") as file:
         file.write(textwrap.dedent(cfg))
 
     print("Saved")
+
+
+def _configure(info, interactive=True, path=None):
+    """Configure GQRX"""
+
+    util.print_header("Gqrx Conf Generator")
+
+    if path is None:
+        home = os.path.expanduser("~")
+        path = os.path.join(home, ".config", "gqrx")
+
+    conf_file = "default.conf"
+    abs_path = os.path.join(path, conf_file)
+    print("Save {} at {}/".format(conf_file, path))
+
+    if (interactive and not util.ask_yes_or_no("Proceed?")):
+        print("Aborted")
+        return
+
+    gqrx_config(abs_path, info, interactive)
+
+
+def configure(args):
+    """Configure GQRX"""
+    interactive = not args.yes
+    info = config.read_cfg_file(args.cfg, args.cfg_dir)
+
+    if (info is None):
+        return
+
+    _configure(info, interactive, args.path)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/instructions.py` & `blocksat-cli-0.4.6/blocksatcli/firewall.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,459 +1,539 @@
-"""Instructions for the user"""
+"""Configure Firewall Rules"""
 import logging
-import os
-import textwrap
+from abc import ABC, abstractmethod
 from argparse import ArgumentDefaultsHelpFormatter
+from shutil import which
 
-from . import util, defs, config
+from . import config, defs, util
 
+logger = logging.getLogger(__name__)
+runner = util.ProcessRunner(logger)
 
-def _item(text):
-    print(textwrap.fill(text, initial_indent="- ", subsequent_indent="  "))
 
+class BaseFirewall(ABC):
+
+    @abstractmethod
+    def verify(self, ports: list, src_ip: str, igmp: bool) -> bool:
+        pass
+
+    @abstractmethod
+    def configure(self, ports: list, src_ip: str, igmp: bool,
+                  prompt: bool) -> None:
+        pass
+
+
+class Iptables(BaseFirewall):
+
+    def __init__(self, net_if):
+        self.net_if = net_if
+
+    def _get_cmd(self, ports, igmp):
+        """Get command-line options to configure iptables"""
+        cmd = [
+            "iptables",
+            "-I",
+            "INPUT",
+            "-p",
+            "udp",
+            "-i",
+            self.net_if,
+            "--match",
+            "multiport",
+            "--dports",
+            ",".join(ports),
+            "-j",
+            "ACCEPT",
+        ]
+
+        cmd_igmp = [
+            "iptables",
+            "-I",
+            "INPUT",
+            "-p",
+            "igmp",
+            "-i",
+            self.net_if,
+            "-j",
+            "ACCEPT",
+        ]
+
+        return cmd if not igmp else cmd_igmp
+
+    def _get_rules(self):
+        """Get iptables rules specifically applied to a target interface
+
+        Returns:
+            rules (list): List of dictionaries with information of the
+            individual matched rules
+
+        """
+        # Unfortunately, root privileges are required to read the current
+        # firewall rules. Hence, we can't read the current rules without
+        # eventually asking the root password in dry-run mode. As a workaround,
+        # return an empty list as if the rule was not set yet.
+        if (runner.dry):
+            return []
+
+        # Get rules
+        cmd = ["iptables", "-L", "-v", "--line-numbers"]
+        res = runner.run(cmd, root=True, capture_output=True).stdout
+
+        # Parse
+        header1 = ""
+        header2 = ""
+        rules = list()
+        for line in res.splitlines():
+            if ("Chain INPUT" in line.decode()):
+                header1 = line.decode()
+
+            if ("destination" in line.decode()):
+                header2 = line.decode()
+
+            if (self.net_if in line.decode()):
+                rules.append({
+                    'rule': line.decode().split(),
+                    'header1': header1,
+                    'header2': header2
+                })
+
+        return rules
+
+    def _add_rule(self, cmd):
+        """Add iptables rule
+
+        Args:
+            cmd: List with iptables command.
+
+        """
+        assert (cmd[0] != "sudo")
+
+        # Set up the iptables rules
+        runner.run(cmd, root=True)
+
+        for rule in self._get_rules():
+            if (rule['rule'][3] == "ACCEPT" and rule['rule'][6] == cmd[6]
+                    and rule['rule'][4] == cmd[4]):
+                if (cmd[4] == "igmp"):
+                    logger.info(
+                        "Added firewall rule to accept IGMP traffic at the "
+                        "{} interface.".format(cmd[6]))
+                elif (cmd[4] == "udp" and rule['rule'][12] == cmd[10]):
+                    logger.info(
+                        "Added firewall rule to accept UDP traffic at the "
+                        "{} interface with destination ports {}.".format(
+                            cmd[6], cmd[10]))
+
+    def _is_igmp_rule_set(self, cmd):
+        """Check if an iptables rule for IGMP is already configured
+
+        Args:
+            cmd: List with iptables command.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        assert (isinstance(cmd, list))
+        assert (cmd[0] != "sudo")
+
+        interface = cmd[6]
+
+        for rule in self._get_rules():
+            if (rule['rule'][3] == "ACCEPT" and rule['rule'][6] == interface
+                    and rule['rule'][4] == "igmp"):
+                logger.info(
+                    "Firewall rule to accept IGMP traffic at the {} interface "
+                    "is already configured.".format(interface))
+                return True
+
+        return False
+
+    def _is_udp_rule_set(self, cmd):
+        """Check if an iptables rule for UDP is already configured
+
+        Args:
+            net_if : Network interface name.
+            cmd    : List with iptables command.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        assert (isinstance(cmd, list))
+        assert (cmd[0] != "sudo")
+
+        protocol = cmd[4]
+        interface = cmd[6]
+        dest_ports = cmd[10]
+
+        for rule in self._get_rules():
+            if (rule['rule'][3] == "ACCEPT" and rule['rule'][6] == interface
+                    and rule['rule'][4] == protocol
+                    and rule['rule'][12] == dest_ports):
+                logger.info(
+                    "Firewall rule to accept UDP traffic at the {} interface "
+                    "with destination ports {} is already configured.".format(
+                        interface, dest_ports))
+                return True
+        return False
+
+    def verify(self, ports: list, src_ip: str, igmp: bool = False) -> bool:
+        """Verify if iptables rules are set
+
+        Args:
+            ports   : UDP ports used by satellite traffic.
+            src_ip  : Source IP to whitelist (unique to each satellite).
+            igmp    : Whether or not to configure rule to accept IGMP queries.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        # Check UDP rule
+        cmd = self._get_cmd(ports, igmp=False)
+        is_rule_set = self._is_udp_rule_set(cmd)
+
+        if not is_rule_set or not igmp:
+            # Early return if UDP rules are not set. If that is the case,
+            # we need to run the configuration process anyway.
+            return is_rule_set
+
+        # Check IGMP rule
+        cmd = self._get_cmd(ports, igmp=True)
+        is_igmp_rule_set = self._is_igmp_rule_set(cmd)
+
+        return is_igmp_rule_set
+
+    def configure(self,
+                  ports: list,
+                  src_ip: str,
+                  igmp: bool = False,
+                  prompt: bool = True) -> None:
+        """Configure iptables rules on DVB-S2 interface
+
+        Args:
+            ports  : Ports used for blocks traffic and API traffic.
+            igmp   : Whether or not to configure rule to accept IGMP queries.
+            prompt : Ask yes/no before applying any changes.
+
+        """
+
+        cmd = self._get_cmd(ports, igmp=False)
+
+        util.fill_print(
+            "A firewall rule is required to accept Blocksat traffic arriving "
+            + "through interface {} towards UDP ports {}.".format(
+                self.net_if, ",".join(ports)))
+
+        if (runner.dry):
+            util.fill_print("The following command would be executed:")
+
+        if (not self._is_udp_rule_set(cmd)):
+            if (runner.dry or (not prompt) or util.ask_yes_or_no(
+                    "Add the corresponding ACCEPT firewall rule?")):
+                self._add_rule(cmd)
+            else:
+                print("\nFirewall configuration cancelled")
+
+        # We're done, unless we also need to configure an IGMP rule
+        if (not igmp):
+            return
+
+        # IGMP rule supports standalone DVB receivers. The host in this case
+        # will need to periodically send IGMP membership reports in order for
+        # upstream switches between itself and the DVB receiver to continue
+        # delivering the multicast-addressed traffic. This overcomes the
+        # scenario where group membership timeouts are implemented by the
+        # intermediate switches.
+        cmd = self._get_cmd(ports, igmp=True)
+
+        print()
+        util.fill_print(
+            "A firewall rule is required to accept IGMP queries arriving "
+            "from the standalone DVB-S2 receiver on interface {}.".format(
+                self.net_if))
+
+        if (runner.dry):
+            util.fill_print("The following command would be executed:")
+
+        if (not self._is_igmp_rule_set(cmd)):
+            if (runner.dry or (not prompt) or util.ask_yes_or_no(
+                    "Add the corresponding ACCEPT firewall rule?")):
+                self._add_rule(cmd)
+            else:
+                print("\nIGMP firewall rule cancelled")
+
+
+class Firewalld(BaseFirewall):
+
+    def __init__(self, net_if):
+        self.net_if = net_if
+
+    def _get_rich_rule(self, src_ip, mcast_ip, portrange):
+        """Get firewalld rich rule to accept Blocksat traffic"""
+        return ("rule "
+                "family=ipv4 "
+                "source address={} "
+                "destination address={}/32 "
+                "port port={} protocol=udp accept".format(
+                    src_ip, mcast_ip, portrange))
+
+    def _is_udp_rule_set(self, src_ip, mcast_ip, portrange):
+        """Check if firewalld rule for UDP is already configured
+
+        Args:
+            src_ip: Source IP address.
+            mcast_ip: Destination IP address.
+            portrange: Destination port range.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        rich_rule = self._get_rich_rule(src_ip, mcast_ip, portrange)
+        cmd = [
+            'firewall-cmd', '--quiet', '--query-rich-rule',
+            "{}".format(rich_rule)
+        ]
+        res = runner.run(cmd, root=True, nocheck=True)
+        is_rule_set = res is not None and res.returncode == 0
+
+        if is_rule_set:
+            logger.info("Firewall rule to accept UDP traffic from IP address "
+                        "{} to the destination IP address {} in ports {} "
+                        "is already configured.".format(
+                            src_ip, mcast_ip, portrange))
+
+        return is_rule_set
+
+    def _is_igmp_rule_set(self):
+        """Check if firewalld rule for UDP is already configured
+
+        Args:
+            rich_rule: Firewalld rich rule.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        cmd = ['firewall-cmd', '--quiet', '--query-protocol=igmp']
+        res = runner.run(cmd, root=True, nocheck=True)
+        is_rule_set = res is not None and res.returncode == 0
+
+        if is_rule_set:
+            logger.info(
+                "Firewall rule to accept IGMP traffic is already configured.")
+
+        return is_rule_set
+
+    def verify(self, ports: list, src_ip: str, igmp: bool = False) -> bool:
+        """Verify if firewalld rules are set
+
+        Args:
+            ports  : UDP ports used by satellite traffic.
+            src_ip : Source IP to whitelist (unique to each satellite).
+            igmp   : Whether or not to configure rule to accept IGMP queries.
+
+        Returns:
+            True if rule is already set, False otherwise.
+
+        """
+        if len(ports) > 1:
+            portrange = "{}-{}".format(min(ports), max(ports))
+        else:
+            portrange = ports
+
+        # Check UDP rule
+        is_rule_set = self._is_udp_rule_set(src_ip, defs.mcast_ip, portrange)
+        if not is_rule_set or not igmp:
+            # Early return if UDP rules are not set. If that is the case,
+            # we need to run the configuration process anyway.
+            return is_rule_set
+
+        # Check IGMP rule
+        is_igmp_rule_set = self._is_igmp_rule_set()
+        return is_igmp_rule_set
+
+    def configure(self,
+                  ports: list,
+                  src_ip: str,
+                  igmp: bool = False,
+                  prompt: bool = False) -> None:
+        """Configure firewalld for blocksat and IGMP traffic
+
+        Add one rich rule for blocksat traffic coming specifically from the
+        satellite of choice (corresponding to the given source IP) and another
+        rich rule (if necessary) for IGMP traffic.
+
+        NOTE: unlike the iptables configuration, the current firewalld
+        configuration disregards the network interface. The alternative to
+        consider the interface is to use firewalld zones. However, because the
+        network interface may not be dedicated to DVB-S2 traffic (e.g., when
+        using a standalone receiver), it can be undesirable to assign the
+        interface receiving satellite traffic to a dedicated zone just for
+        blocksat. In contrast, the rich rule approach is more generic and works
+        for all types of receivers.
+
+        """
+        if len(ports) > 1:
+            portrange = "{}-{}".format(min(ports), max(ports))
+        else:
+            portrange = ports
+
+        util.fill_print(
+            "- Configure the firewall to accept Blocksat traffic arriving " +
+            "from {} towards address {} on UDP ports {}:\n".format(
+                src_ip, defs.mcast_ip, portrange))
+
+        if (not runner.dry and prompt):
+            if (not util.ask_yes_or_no("Add firewalld rule?")):
+                print("\nFirewall configuration cancelled")
+                return
+
+        if (not self._is_udp_rule_set(src_ip, defs.mcast_ip, portrange)):
+            rich_rule = self._get_rich_rule(src_ip, defs.mcast_ip, portrange)
+            runner.run(
+                ['firewall-cmd', '--add-rich-rule', "{}".format(rich_rule)],
+                root=True)
+            logger.info("Added firewall rule to accept UDP traffic from "
+                        "IP address {} to destination address {} "
+                        "on ports {}.".format(src_ip, defs.mcast_ip,
+                                              portrange))
 
-def _print(text):
-    text = " ".join(text.replace("\n", "").split())
-    print(textwrap.fill(text))
-    print()
-
-
-def _print_s400_instructions(info):
-    """Print instructions for configuration of the Novra S400
-    """
-    util.print_header("Novra S400")
-
-    _print("""
-    The Novra S400 is a standalone receiver, which will receive data from
-    satellite and output IP packets to the host over the network. Hence, you
-    will need to configure both the S400 and the host.
-    """)
-
-    util.print_sub_header("Connections")
-
-    _print("The Novra S400 can be connected as follows:")
-
-    print(("LNB ----> S400 (RF1 Interface) -- "
-           "S400 (LAN 1 Interface) ----> Host / Network\n"))
-
-    _item("Connect the LNB directly to interface RF1 of the S400 using a "
-          "coaxial cable (an RG6 cable is recommended).")
-    _item("Connect the S400's LAN1 interface to your computer or network.")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Network Connection")
-
-    _print("Next, make sure the S400 receiver is reachable by the host.")
-
-    _print("First, configure your host's network interface to the same subnet "
-           "as the S400. By default, the S400 is configured with IP address "
-           "192.168.1.2 on LAN1 and 192.168.2.2 on LAN2. Hence, if you "
-           "connect to LAN1, make sure your host's network interface has IP "
-           "address 192.168.1.x, where \"x\" could be any number higher than "
-           "2. For example, you could configure your host's network interface "
-           "with IP address 192.168.1.3.")
-
-    _print("After that, open the browser and access 192.168.1.2 (or "
-           "192.168.2.2 if connected to LAN 2). The web management console "
-           "should open up successfully.")
-
-    print()
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Software Requirements")
-
-    _print("Next, install all software pre-requisites on your host. Run:")
-
-    print("    blocksat-cli deps install\n")
-
-    _print("""
-    NOTE: this command supports the apt, dnf, and yum package managers.""")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Receiver and Host Configuration")
-
-    print("Now, configure the S400 receiver and the host by running:")
-
-    print("\n    blocksat-cli standalone cfg\n")
-
-    _print("""If you would like to review the changes that will be made to the
-    host before applying them, first run the command in dry-run mode:""")
-
-    print("    blocksat-cli standalone cfg --dry-run\n\n")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Monitoring")
-
-    print("Finally, you can monitor your receiver by running:")
-
-    print("\n    blocksat-cli standalone monitor\n\n")
-
-    util.prompt_for_enter()
-
-
-def _print_usb_rx_instructions(info):
-    """Print instructions for runnning with a Linux USB receiver
-    """
-
-    name = (info['setup']['vendor'] + " " + info['setup']['model']).strip()
-
-    util.print_header(name)
-
-    _print("""
-    The {0} is a USB-based DVB-S2 receiver. It receives the satellite signal
-    fed via a coaxial interface and outputs data to the host over USB. It is
-    also configured directly via USB, and the host is responsible for setting
-    such configurations using specific Linux tools.
-    """.format(name))
-
-    _print("The instructions that follow prepare the host for driving the "
-           "{0} receiver.".format(name))
-
-    util.print_sub_header("Hardware Connections")
-
-    print("The {} should be connected as follows:\n".format(name))
-
-    print(("LNB ----> {0} (LNB Interface) -- "
-           "{0} (USB Interface) ----> Host\n".format(name)))
-
-    _item("Connect the LNB directly to \"LNB IN\" of the {} using a coaxial"
-          " cable (an RG6 cable is recommended).".format(name))
-    _item("Connect the {}'s USB2.0 interface to your computer.".format(name))
-    if (info['setup']['model'] == "5520SE"):
-        power_up_str = "Connect both male connectors of the dual-male " + \
-            "USB Y cable to your host."
+        if (runner.dry):
+            print()
+            util.fill_print(
+                "NOTE: Add \"--permanent\" to make it persistent. In this "
+                "case, remember to reload firewalld afterwards.")
+
+        # We're done, unless we also need to configure an IGMP rule
+        if (not igmp):
+            return
+
+        util.fill_print(
+            "- Allow IGMP packets. This is necessary when using a standalone "
+            "DVB-S2 receiver connected through a switch:\n")
+
+        if (not runner.dry and prompt):
+            if (not util.ask_yes_or_no("Enable IGMP on the firewall?")):
+                print("\nFirewall configuration cancelled")
+                return
+
+        if (not self._is_igmp_rule_set()):
+            runner.run(['firewall-cmd', '--add-protocol=igmp'], root=True)
+            logger.info("Added firewall rule to accept IGMP traffic.")
+
+
+def is_firewalld():
+    """Check if the firewall is based on firewalld"""
+    if (which('firewall-cmd') is None):
+        return False
+
+    if (which('systemctl') is None):
+        # Can't check whether firewalld is running
+        return False
+
+    # Run the following commands even in dry-run mode
+    res1 = runner.run(['systemctl', 'is-active', '--quiet', 'firewalld'],
+                      nodry=True,
+                      nocheck=True)
+    res2 = runner.run(['systemctl', 'is-active', '--quiet', 'iptables'],
+                      nodry=True,
+                      nocheck=True)
+
+    # If running (active), 'is-active' returns 0
+    if (res1.returncode == 0 and res2.returncode == 0):
+        raise ValueError(
+            "Failed to detect firewall system (firewalld or iptables)")
+
+    return (res1.returncode == 0)
+
+
+def get_firewall(net_if) -> BaseFirewall:
+    if is_firewalld():
+        return Firewalld(net_if)
     else:
-        power_up_str = "Connect the 12V DC power supply."
-    _item("Power up the {} device. {} ".format(name, power_up_str))
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Drivers")
-
-    _print("""
-    Next, you will need to install specific device drivers to use the {0}.
-    These are installed by rebuilding and rewriting the Linux Media drivers.
-    Hence, if you are not setting up a dedicated machine to host the {0}, it
-    would be safer and recommended to use a virtual machine (VM) as the
-    receiver host so that the drivers can be installed directly on the VM
-    instead of your main machine.
-    """.format(name))
-
-    _print("Next, install the drivers for the {0} by running:".format(name))
-
-    print("    blocksat-cli deps tbs-drivers\n")
-
-    print("Once the script completes the installation, reboot the machine.")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Host Requirements")
-
-    print("Next, install all the software pre-requisites by running:")
-
-    print("""
-    blocksat-cli deps install
-    """)
-
-    _print("""
-    NOTE: this command supports the apt, dnf, and yum package managers. For
-    other package managers, refer to the instructions at:""")
-    print(defs.user_guide_url + "doc/tbs.html")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Configure the Host")
+        return Iptables(net_if)
 
-    _print("""Next, you need to create and configure the network interface that
-    will output the IP traffic received via the {} device. You can apply all
-    configurations by running the following command:""".format(name))
 
-    print("\n    blocksat-cli usb config\n")
+def verify(net_ifs, ports, src_ip, igmp=False):
+    assert (isinstance(net_ifs, list))
+    firewall_set = list()
 
-    _print("""If you would like to review the changes before applying them,
-    first run the command in dry-run mode:
-    """)
+    for net_if in net_ifs:
+        firewall = get_firewall(net_if)
+        res = firewall.verify(ports, src_ip, igmp)
+        firewall_set.append(res)
 
-    print("\n    blocksat-cli usb config --dry-run\n")
+    return all(firewall_set)
 
-    _print("""
-    Note this command will define an arbitrary IP address to the interface. If
-    you would like to set a specific IP address, for example, to avoid
-    address conflicts, use the option \"--ip\".
-    """)
 
-    _print("""Furthermore, note this configuration is not persistent across
-    reboots. After a reboot, you need to run \"blocksat-cli usb config\"
-    again.""")
+def configure(net_ifs, ports, src_ip, igmp=False, prompt=True, dry=False):
+    """Configure firewall rules to accept blocksat traffic via DVB interface
 
-    util.prompt_for_enter()
+    Args:
+        net_ifs : List of DVB network interface names.
+        ports   : UDP ports used by satellite traffic.
+        src_ip  : Source IP to whitelist (unique to each satellite).
+        igmp    : Whether or not to configure rule to accept IGMP queries.
+        prompt  : Prompt user to accept configurations before executing them.
+        dry     : Dry run mode.
 
-    util.print_sub_header("Launch")
-
-    print("Finally, start the receiver by running:")
-
-    print("\n    blocksat-cli usb launch\n")
-
-    util.prompt_for_enter()
-
-
-def _print_sdr_instructions(info):
-    """Print instruction for configuration of an SDR setup
     """
-    util.print_header("SDR Setup")
-
-    util.print_sub_header("Connections")
-
-    print("The SDR setup is connected as follows:\n")
-
-    print("LNB ----> Power Supply ----> RTL-SDR ----> Host\n")
-
-    _item("Connect the RTL-SDR USB dongle to your host PC.")
-    _item("Connect the **non-powered** port of the power supply (labeled as "
-          "\"Signal to IRD\") to the RTL-SDR using an SMA cable and an "
-          "SMA-to-F adapter.")
-    _item("Connect the **powered** port (labeled \"Signal to SWM\") of the "
-          "power supply to the LNB using a coaxial cable (an RG6 cable is "
-          "recommended).")
-
-    print()
-    _print("IMPORTANT: Do NOT connect the powered port of the power supply "
-           "to the SDR interface. Permanent damage may occur to your SDR "
-           "and/or your computer.")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Software Requirements")
-
-    print("The SDR-based setup relies on the applications listed below:\n")
-
-    _item("leandvb: a software-based DVB-S2 receiver application.")
-    _item("rtl_sdr: reads samples taken by the RTL-SDR and feeds them into "
-          "leandvb.")
-    _item("TSDuck: unpacks the output of leandvb and produces "
-          "IP packets to be fed to Bitcoin Satellite.")
-    _item("Gqrx: useful for spectrum visualization during antenna pointing.")
-
-    print("\nTo install them, run:")
-    print("""
-    blocksat-cli deps install
-    """)
-
-    _print("""
-        NOTE: This command supports the two most recent Ubuntu LTS, Fedora, and
-        CentOS releases. In case you are using another Linux distribution or
-        version, please refer to the manual compilation and installation
-        instructions at:""")
-    print(defs.user_guide_url + "doc/sdr.html")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Configuration")
-
-    _print(
-        "Next, you can generate the configurations that are needed for gqrx "
-        "by running:")
-
-    print("    blocksat-cli gqrx-conf")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Running")
-
-    _print(
-        "You should now be ready to launch the SDR receiver. You can run it "
-        "by executing:")
-
-    print("    blocksat-cli sdr\n")
-    print("Or, in GUI mode:\n")
-    print("    blocksat-cli sdr --gui\n")
-
-    util.prompt_for_enter()
-
-
-def _print_sat_ip_instructions(info):
+    assert (isinstance(net_ifs, list))
+    runner.set_dry(dry)
+    util.print_header("Firewall Rules")
+
+    for i, net_if in enumerate(net_ifs):
+        firewall = get_firewall(net_if)
+        firewall.configure(ports, src_ip, igmp, prompt)
 
-    util.print_header("Sat-IP Setup")
-
-    _print("""The Sat-IP setup relies on the Blockstream Satellite Base
-    Station (available on Blockstream Store), an all-in-one flat-panel antenna
-    with an integrated receiver and LNB. This device receives the satellite
-    signal and outputs IP packets to one or more Sat-IP clients listening to
-    it in the local network.""")
-
-    _print("The following steps explain how you can connect to the base "
-           "station device to receive the Blockstream Satellite traffic.")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Connections")
-
-    _item("Connect the Ethernet cable from your switch or computer's network "
-          "adapter directly to the antenna's Sat>IP port.")
-
-    _item("If your switch/adapter does not support Power over Ethernet (PoE), "
-          "insert a PoE injector in-line between the switch/adapter and the "
-          "antenna's Sat-IP port. Connect the injector's PoE-enabled port to "
-          "the Sat-IP antenna and the non-powered (non-PoE) port to the "
-          "switch/adapter.")
-
-    print()
-    _print("IMPORTANT: If using a PoE injector, make sure you are connecting "
-           "the correct ports. Permanent damage may occur to your switch or "
-           "network adapter otherwise.")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Software Requirements")
-
-    _print("Next, install all software pre-requisites on your host. Run:")
-
-    print("    blocksat-cli deps install\n")
-
-    _print("""
-    NOTE: this command supports the apt, dnf, and yum package managers.""")
-
-    util.prompt_for_enter()
-
-    util.print_sub_header("Running")
-
-    _print("You should now be ready to launch the Sat-IP client. You can run "
-           "it by executing:")
-
-    print("    blocksat-cli sat-ip\n")
-
-    util.prompt_for_enter()
-
-
-def _print_freq_info(info):
-    """Print summary of frequencies of interest"""
-    sat = info['sat']
-    setup = info['setup']
-    lnb = info['lnb']
-    lo_freq = info['freqs']['lo']
-    l_freq = info['freqs']['l_band']
-
-    util.print_header("Frequencies")
-
-    print("For your information, your setup relies on the following "
-          "frequencies:\n")
-    print("| Downlink %2s band frequency            | %8.2f MHz |" %
-          (sat['band'], sat['dl_freq']))
-    print("| LNB local oscillator (LO) frequency   | %8.2f MHz |" % (lo_freq))
-    print("| Receiver L-band frequency             | %7.2f MHz  |" % (l_freq))
-    print()
-
-    if (lnb['universal'] and (setup['type'] == defs.sdr_setup_type)):
-        if (sat['dl_freq'] > defs.ku_band_thresh):
-            print("NOTE regarding Universal LNB:\n")
-
-            print(
-                textwrap.fill(
-                    ("The DL frequency of {} is in Ku high "
-                     "band (> {:.1f} MHz). Hence, you need to use "
-                     "the higher frequency LO ({:.1f} MHz) of your "
-                     "Universal LNB. This requires a 22 kHz tone "
-                     "to be sent to the LNB.").format(sat['alias'],
-                                                      defs.ku_band_thresh,
-                                                      lo_freq)))
-            print()
-            print(
-                textwrap.fill(("With a software-defined setup, you will "
-                               "need to place a 22 kHz tone generator "
-                               "inline between the LNB and the power "
-                               "inserter. Typically the tone generator "
-                               "uses power from the power inserter while "
-                               "delivering the tone directly to the "
-                               "LNB.")))
-
-    util.prompt_for_enter()
-
-
-def _print_lnb_info(info):
-    """Print important waraning based on LNB choice"""
-    lnb = info['lnb']
-    sat = info['sat']
-    setup = info['setup']
-
-    if ((lnb['pol'] != "Dual") and (lnb['pol'] != sat['pol'])):
-        util.print_header("LNB Information")
-        lnb_pol = "Vertical" if lnb['pol'] == "V" else "Horizontal"
-        logging.warning(
-            textwrap.fill(
-                "Your LNB has {} polarization and the signal from {} has the "
-                "opposite polarization.".format(lnb_pol, sat['name'])))
-        util.prompt_for_enter()
-
-    if ((lnb['pol'] == "Dual") and (setup['type'] == defs.sdr_setup_type)):
-        util.print_header("LNB Information")
-        logging.warning(
-            textwrap.fill(
-                "Your LNB has dual polarization. Check the voltage of your "
-                "power supply in order to discover the polarization on which "
-                "your LNB will operate."))
-        util.prompt_for_enter()
-
-
-def _print_next_steps():
-    util.print_header("Next Steps")
-    _print("""
-    At this point, if your dish is already correctly pointed, you should be
-    able to start receiving data on Bitcoin Satellite.
-    """)
-
-    print("You can generate a bitcoin.conf configuration file for Bitcoin "
-          "Satellite using:")
-    print("\n    blocksat-cli btc\n")
-
-    _print("Next, if you are running a supported Linux distribution "
-           "(Ubuntu, Debian, Fedora, CentOS, or Raspberry Pi OS), you can "
-           "install Bitcoin Satellite by running:")
-    print("    blocksat-cli deps install --btc\n")
-
-    _print("Note that Bitcoin Satellite is a fork of Bitcoin Core, and, "
-           "as such, it installs applications with the same name (bitcoind, "
-           "bitcoin-cli, bitcoin-qt, and bitcoin-tx). Hence, the "
-           "Bitcoin Satellite installation will fail if you already have "
-           "Bitcoin Core installed.")
-
-    print("For further information, refer to:\n")
-    print(defs.user_guide_url + "doc/bitcoin.html\n")
-
-    _print("""If your antenna is not pointed yet, please follow the
-    antenna alignment guide at:""")
-    print(defs.user_guide_url + "doc/antenna-pointing.html\n")
+        if (i < len(net_ifs) - 1):
+            print("")
 
 
 def subparser(subparsers):  # pragma: no cover
-    """Argument parser of instructions command"""
-    p = subparsers.add_parser('instructions',
-                              description="Instructions for Blocksat Rx setup",
-                              help='Read instructions for the receiver setup',
+    """Parser for firewall command"""
+    p = subparsers.add_parser('firewall',
+                              description="Set firewall rules",
+                              help='Set firewall rules',
                               formatter_class=ArgumentDefaultsHelpFormatter)
-    p.set_defaults(func=show)
+    p.add_argument('-i',
+                   '--interface',
+                   required=True,
+                   help='Network interface')
+    p.add_argument(
+        '--standalone',
+        default=False,
+        action='store_true',
+        help='Apply configurations for a standalone DVB-S2 receiver')
+    p.add_argument('-y',
+                   '--yes',
+                   default=False,
+                   action='store_true',
+                   help="Default to answering Yes to configuration prompts")
+    p.add_argument("--dry-run",
+                   action='store_true',
+                   default=False,
+                   help="Print all commands but do not execute them")
+    p.set_defaults(func=firewall_subcommand)
     return p
 
 
-def show(args):
-    """Show instructions"""
-    info = config.read_cfg_file(args.cfg, args.cfg_dir)
+def firewall_subcommand(args):
+    """Call function that sets firewall rules
 
-    if (info is None):
-        return
+    Handles the firewall subcommand
 
-    os.system('clear')
-    _print_lnb_info(info)
+    """
+    user_info = config.read_cfg_file(args.cfg, args.cfg_dir)
 
-    if (info['setup']['type'] == defs.standalone_setup_type):
-        _print_s400_instructions(info)
-    elif (info['setup']['type'] == defs.sdr_setup_type):
-        _print_sdr_instructions(info)
-    elif (info['setup']['type'] == defs.linux_usb_setup_type):
-        _print_usb_rx_instructions(info)
-    elif (info['setup']['type'] == defs.sat_ip_setup_type):
-        _print_sat_ip_instructions(info)
+    if (user_info is None):
+        return
 
-    _print_next_steps()
+    configure([args.interface],
+              defs.src_ports,
+              user_info['sat']['ip'],
+              igmp=args.standalone,
+              prompt=(not args.yes),
+              dry=args.dry_run)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/ip.py` & `blocksat-cli-0.4.6/blocksatcli/ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,40 +47,80 @@
 
     if (src_included):
         return
 
     runner.append_to_file("\n" + src_line + "\n", if_file, root=True)
 
 
+def is_network_manager_active():
+    is_nm = runner.run(['systemctl', 'is-active', '--quiet', 'NetworkManager'],
+                       nocheck=True)
+    return is_nm and is_nm.returncode == 0
+
+
 def _add_to_netplan(ifname, addr_with_prefix):
     """Create configuration file at /etc/netplan/"""
     assert ("/" in addr_with_prefix)
     cfg_dir = "/etc/netplan/"
 
+    # Netplan is an abstraction layer for configuring the system network. It
+    # uses NetworkManager or networkd for configuring the network interfaces.
+    # Thus, check which one is being used first.
+    renderer = 'NetworkManager' if is_network_manager_active() else 'networkd'
+
     cfg = ("network:\n"
            "  version: 2\n"
-           "  renderer: networkd\n"
+           "  renderer: {0}\n"
            "  ethernets:\n"
-           "    {0}:\n"
+           "    {1}:\n"
            "      dhcp4: no\n"
            "      optional: true\n"
-           "      addresses: [{1}]\n").format(ifname, addr_with_prefix)
+           "      addresses: [{2}]\n").format(renderer, ifname,
+                                              addr_with_prefix)
 
     fname = "blocksat-" + ifname + ".yaml"
     path = os.path.join(cfg_dir, fname)
 
     if (runner.dry):
         util.fill_print("Create a file named {} at {} and add the "
                         "following to it:".format(fname, cfg_dir))
         print(cfg)
         return
 
     runner.create_file(cfg, path, root=True)
 
 
+def _add_to_network_manager(ifname, addr):
+    """Create connection with network manager CLI
+
+    The network manager CLI (nmcli) automatically creates the configuration
+    file at `/etc/NetworkManager/system-connections/`.
+
+    Args:
+        ifname: Interface name.
+        addr: IP Address.
+
+    """
+    # Delete any existing connection of the chosen interface
+    res = runner.run(["nmcli", "connection", "show", ifname],
+                     nocheck=True,
+                     stdout=subprocess.DEVNULL)
+    if res and res.returncode == 0:
+        runner.run(["nmcli", "connection", "delete", ifname], root=True)
+        logger.info(f"Previous {ifname} connection deleted.")
+
+    # Create new connection
+    logger.info(f"Adding new {ifname} connection.")
+    runner.run([
+        "nmcli", "connection", "add", "type", "ethernet", "ifname", ifname,
+        "con-name", ifname, "ip4", addr
+    ],
+               root=True)
+
+
 def _add_to_interfaces_d(ifname, addr, netmask):
     """Create configuration file at /etc/network/interfaces.d/"""
     if_dir = "/etc/network/interfaces.d/"
     cfg = ("iface {0} inet static\n"
            "    address {1}\n"
            "    netmask {2}\n").format(ifname, addr, netmask)
     fname = ifname + ".conf"
@@ -130,14 +170,16 @@
     addr_with_prefix = ipv4_if.with_prefixlen
     netmask = str(ipv4_if.netmask)
 
     if (which("netplan") is not None):
         _add_to_netplan(ifname, addr_with_prefix)
     elif (os.path.exists("/etc/network/interfaces.d/")):
         _add_to_interfaces_d(ifname, addr, netmask)
+    elif is_network_manager_active():
+        _add_to_network_manager(ifname, addr_with_prefix)
     elif (os.path.exists("/etc/sysconfig/network-scripts")):
         _add_to_sysconfig_net_scripts(ifname, addr, netmask)
     else:
         logger.warning("Falling back to \"ip addr add\" command")
         runner.run(["ip", "addr", "add", addr_with_prefix, "dev", ifname],
                    root=True)
 
@@ -233,14 +275,17 @@
         ifup_required = True
         # Debian approach
         if (dry):
             util.fill_print("Finally, restart the networking service and "
                             "bring up the interfaces:")
             print()
         runner.run(["systemctl", "restart", "networking"], root=True)
+    elif is_network_manager_active():
+        # Bring-up is automatic when creating the interface
+        pass
     elif (os.path.exists("/etc/sysconfig/network-scripts")):
         ifup_required = True
         # CentOS/Fedora/RHEL approach
         if (dry):
             print(textwrap.fill("Finally, bring up the interfaces:") + "\n")
 
     if (ifup_required):
@@ -250,25 +295,27 @@
 
 def check_ips(net_ifs, ip_addrs):
     """Check if IPs of one or multiple DVB network interface(s) are OK
 
     Args:
         net_ifs   : List of DVB network interface names
         ip_addrs  : List of IP addresses for the dvbnet interface's subnet mask
-        verbose   : Controls verbosity
 
     """
     for net_if, ip_addr in zip(net_ifs, ip_addrs):
         has_ip, ip_ok = _check_ip(net_if, ip_addr)
         if (not has_ip):
-            raise ValueError(
+            logger.info(
                 "Interface {} does not have an IP address".format(net_if))
+            return False
         elif (has_ip and not ip_ok):
-            raise ValueError("Interface {} IP is not {}".format(
-                net_if, ip_addr))
+            logger.info("Interface {} IP is not {}".format(net_if, ip_addr))
+            return False
+
+    return True
 
 
 def rm_ip(ifname, dry=False):
     """Remove the static IP configuration of a given interface"""
     runner.set_dry(dry)
 
     # Remove conf file for network interface (next time the interface could
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/main.py` & `blocksat-cli-0.4.6/blocksatcli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 import logging
 import os
 import platform
 import time
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/NOVRA-MIB.mib` & `blocksat-cli-0.4.6/blocksatcli/mib/NOVRA-MIB.mib`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/NOVRA-s400-MIB.mib` & `blocksat-cli-0.4.6/blocksatcli/mib/NOVRA-s400-MIB.mib`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/RFC1155-SMI.txt` & `blocksat-cli-0.4.6/blocksatcli/mib/RFC1155-SMI.txt`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-CONF.txt` & `blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-CONF.txt`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-SMI.txt` & `blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-SMI.txt`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/mib/SNMPv2-TC.txt` & `blocksat-cli-0.4.6/blocksatcli/mib/SNMPv2-TC.txt`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/monitoring.py` & `blocksat-cli-0.4.6/blocksatcli/monitoring.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,22 +52,33 @@
     }
 }
 
 
 def get_report_opts(args):
     """Extract the parser fields needed to construct a Reporter object"""
     return {
-        'cfg': args.cfg,
-        'cfg_dir': args.cfg_dir,
-        'dest_addr': args.report_dest,
-        'hostname': args.report_hostname,
-        'tls_cert': args.report_cert,
-        'tls_key': args.report_key,
-        'gnupghome': args.report_gnupghome,
-        'passphrase': args.report_passphrase
+        'cfg':
+        args.cfg,
+        'cfg_dir':
+        args.cfg_dir,
+        'dest_addr':
+        monitoring_api.DEFAULT_SERVER_URL
+        if args.report_dest is None else args.report_dest,
+        'bs_monitoring':
+        args.report_dest is None or args.report_bs,
+        'hostname':
+        args.report_hostname,
+        'tls_cert':
+        args.report_cert,
+        'tls_key':
+        args.report_key,
+        'gnupghome':
+        args.report_gnupghome,
+        'passphrase':
+        args.report_passphrase
     }
 
 
 class ReportStatus(Enum):
     REGISTRATION_RUNNING = 1
     REGISTRATION_FAILED = 2
 
@@ -79,59 +90,62 @@
 
     """
 
     def __init__(self,
                  cfg,
                  cfg_dir,
                  dest_addr,
+                 bs_monitoring,
                  hostname=None,
                  tls_cert=None,
                  tls_key=None,
                  gnupghome=None,
                  passphrase=None,
-                 reset_api_pwd=False):
+                 address=None,
+                 interactive=True):
         """Reporter Constructor
 
         Args:
             cfg       : User configuration
             cfg_dir   : Configuration directory
             dest_addr : Remote server address
+            bs_monitoring (bool): Whether reporting to the Blockstream
+                Satellite Monitoring API.
             hostname  : Hostname used to identify the reports
             tls_cert  : Optional client side certificate for TLS authentication
             tls_key   : Key associated with the client side certificate
             gnupghome : GnuPG home directory used when reporting to
                         Blockstream's monitoring API
             passphrase : Passphrase to the private key used when reporting to
                          Blockstream's monitoring API. If None, it will be
                          obtained by prompting the user.
-            reset_api_pwd : Reset password for the monitoring API.
+            address : Receiver's address used in non-interactive mode.
+            interactive: Whether to run in interactive mode.
 
         """
         info = config.read_cfg_file(cfg, cfg_dir)
         assert (info is not None)
 
         # Validate the satellite
         satellite = info['sat']['alias']
         assert (satellite is not None), "Reporting satellite undefined"
         assert (satellite in sats), "Invalid satellite"
         self.satellite = satellite
 
-        # Destination address, hostname, and client side cert
-        self.dest_addr = dest_addr
         self.hostname = hostname
         self.tls_cert = tls_cert
         self.tls_key = tls_key
 
-        # If the report destination address corresponds to Blockstream's
-        # Monitoring API (the default), create the object to handle the
-        # interaction with this API (e.g., registration).
-        if (dest_addr == monitoring_api.metric_endpoint):
+        if bs_monitoring:
             self.bs_monitoring = monitoring_api.BsMonitoring(
-                cfg, cfg_dir, gnupghome, passphrase, reset_api_pwd)
+                cfg, cfg_dir, dest_addr, gnupghome, passphrase, address,
+                interactive)
+            self.dest_addr = self.bs_monitoring.get_metric_endpoint()
         else:
+            self.dest_addr = dest_addr
             self.bs_monitoring = None
             logger.info("Reporting Rx status to {} ".format(self.dest_addr))
 
     def send(self, metrics):
         """Save measurement on database
 
         Args:
@@ -190,15 +204,16 @@
                 data['hostname'] = self.hostname
         else:
             self.bs_monitoring.sign_request(data, password_allowed=True)
 
         try:
             r = requests.post(self.dest_addr,
                               json=data,
-                              cert=(self.tls_cert, self.tls_key))
+                              cert=(self.tls_cert, self.tls_key),
+                              timeout=5)
             if (r.status_code != requests.codes.ok):
                 print()
                 logger.error("Report failed: " + r.text)
             post_status = r.status_code
         except requests.exceptions.HTTPError as errh:
             post_status = errh
         except requests.exceptions.ConnectionError as errc:
@@ -469,17 +484,24 @@
     r_p = parser.add_argument_group('receiver reporting options')
     r_p.add_argument('--report',
                      default=False,
                      action='store_true',
                      help='Report receiver metrics to a remote HTTP server')
     r_p.add_argument(
         '--report-dest',
-        default=monitoring_api.metric_endpoint,
-        help='Destination address in http://ip:port format. By default, '
-        'report to the Blockstream Satellite Monitoring API')
+        type=str,
+        default=None,
+        help='Destination address in http://ip:port format. When undefined, '
+        'reports are sent to the Blockstream Satellite Monitoring API')
+    r_p.add_argument(
+        '--report-bs',
+        default=False,
+        action='store_true',
+        help='Force reporting to the Blockstream Satellite Monitoring API '
+        'even if \'--report-dest\' is defined')
     r_p.add_argument('--report-hostname', help='Reporter\'s hostname')
     r_p.add_argument(
         '--report-cert',
         default=None,
         help="Certificate for client-side authentication with the destination")
     r_p.add_argument(
         '--report-key',
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/monitoring_api.py` & `blocksat-cli-0.4.6/blocksatcli/monitoring_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 import requests
 
 from . import util
 from . import defs
 from . import config
 from .cache import Cache
 from .api import api
-from .api.gpg import Gpg
+from .api.gpg import Gpg, is_gpg_keyring_set
 from .api.listen import ApiListener
 from .api.order import ApiChannel
 
 logger = logging.getLogger(__name__)
-base_url = "https://satellite.blockstream.space/monitoring"
-account_endpoint = os.path.join(base_url, 'accounts')
-account_pwd_endpoint = os.path.join(account_endpoint, "password")
-metric_endpoint = os.path.join(base_url, "metrics")
+DEFAULT_SERVER_URL = "https://satellite.blockstream.space/monitoring"
 
 
 def _privacy_explainer():
     util.print_sub_header("Reported Metrics")
 
     util.fill_print("The reported metrics vary according to the receiver type "
                     "and consist of a subset of the following:")
@@ -119,14 +116,37 @@
 
     os.system('clear')
 
     if (print_privacy_info):
         _privacy_explainer()
 
 
+def _ask_address():
+    confirmed = False
+    while (not confirmed):
+        # City (required)
+        city = util.string_input("City")
+
+        # State (optional)
+        state = input("State: ")
+        if (len(state) > 0):
+            address = "{}, {}".format(city, state)
+        else:
+            address = city
+
+        # Country (required)
+        country = util.string_input("Country")
+
+        # Wait until the user confirms the full address
+        address += ", {}".format(country)
+        confirmed = util.ask_yes_or_no("\"{}\"?".format(address))
+
+    return address
+
+
 class BsMonitoring():
     """Blockstream Satellite Monitoring API
 
     This class handles the communication with the Monitoring API used to
     monitor Blockstream Satellite receivers who opt-in to report their receiver
     status metrics.
 
@@ -140,35 +160,48 @@
     will register a new account and obtain a unique UUID.
 
     When the receiver is already registered, as indicated by the local config
     file, this class proceeds with metric reporting right away.
 
     """
 
-    def __init__(self, cfg, cfg_dir, gnupghome, passphrase=None, lazy=False):
+    def __init__(self,
+                 cfg,
+                 cfg_dir,
+                 server_url,
+                 gnupghome,
+                 passphrase=None,
+                 address=None,
+                 interactive=True,
+                 lazy=False):
         """Construct the BsMonitoring object
 
         Args:
             cfg (str): User configuration.
             cfg_dir (str): Configuration directory.
+            server_url (str): Monitoring API server URL.
             gnupghome (str):  GnuPG home directory.
             passphrase (str, optional): GPG private key passphrase for
                 non-interactive mode. When not defined, the user is prompted
                 for the passphrase instead. Defaults to None.
+            address (str, optional) : Receiver's address used in
+                non-interactive mode. Defaults to None.
+            interactive (bool, optional): Whether to run in interactive mode.
             lazy (bool, optional): When True, the constructor returns before
                 running the initial interactive setup. Defaults to False.
-
         """
         self.cfg = cfg
         self.cfg_dir = cfg_dir
+        self.server_url = server_url
         self.gpg = Gpg(os.path.join(cfg_dir, gnupghome))
 
         if (passphrase is not None):
             self.gpg.set_passphrase(passphrase)
 
+        self.interactive = interactive
         self.api_pwd = None
         self.api_cfg_dir = os.path.join(self.cfg_dir, 'monitoring_api')
 
         # Check if this receiver setup is already registered
         self.user_info = config.read_cfg_file(cfg, cfg_dir)
         self.registered = 'monitoring' in self.user_info and \
             self.user_info['monitoring']['registered']
@@ -176,19 +209,19 @@
 
         if lazy:
             return
 
         # Register with the Monitoring API if necessary
         self.rx_lock_event = threading.Event()
         if not self.registered:
-            self._register()
+            self._register(address)
         else:
             self._setup_registered()
 
-    def _has_matching_keys(self):
+    def has_matching_keys(self):
         """Check if the GPG key used for monitoring is available"""
         fingerprint = self.user_info['monitoring']['fingerprint']
         matching_keys = self.gpg.gpg.list_keys(True, keys=fingerprint)
         if (len(matching_keys) == 0):
             logger.error("Could not find key {} in the local "
                          "keyring.".format(fingerprint))
         return len(matching_keys) > 0
@@ -200,21 +233,26 @@
         in the keyring and prompt for the GPG private key passphrase required
         to sign report data. Load also the non-GPG password from the local
         encrypted password file.
 
         """
         logger.info("Loading the Monitoring API reporting credentials")
 
-        if not self._has_matching_keys():
-            try_again = util.ask_yes_or_no(
+        if not self.has_matching_keys():
+            # In non-interactive mode, delete the credentials and try
+            # registering again with no prompt to the user. There is no concern
+            # with losing the credentials here because the Monitoring API
+            # informs when a registering account already exists and is already
+            # verified. Also, the password can be regenerated as needed.
+            try_again = not self.interactive or util.ask_yes_or_no(
                 "Reset the Monitoring API credentials and try registering "
                 "with a new key?",
                 default="n")
             if (try_again):
-                self._delete_credentials()
+                self.delete_credentials()
                 self._register()
             else:
                 print("Aborting")
                 sys.exit(1)
 
             # Return regardless. If the key is not available, don't bother
             # about the password.
@@ -229,22 +267,22 @@
         # else to do. Disable the reporting.
         if not self.gpg.test_passphrase(
                 self.user_info['monitoring']['fingerprint']):
             logger.error("Disabling the Rx status reporting")
             self.disabled = True
             return
 
-        if not self._has_password():
-            self._gen_api_password()
+        if not self.has_password():
+            self.gen_api_password()
         else:
-            self._load_api_password()
+            self.load_api_password()
 
         logger.info("Ready to report the Rx status to the Monitoring API")
 
-    def _delete_credentials(self):
+    def delete_credentials(self):
         """Remove the registration info from the local config file"""
         self.user_info.pop('monitoring')
         config.write_cfg_file(self.cfg, self.cfg_dir, self.user_info)
         self.registered = False
 
     def _save_credentials(self, uuid, fingerprint, has_password=False):
         """Record the successful registration locally on the JSON config"""
@@ -258,15 +296,15 @@
         self.registered = True
 
     def _get_api_password_file_path(self):
         fingerprint = self.user_info['monitoring']['fingerprint']
         return os.path.join(self.api_cfg_dir,
                             f'{fingerprint}_{self.cfg}_pwd.gpg')
 
-    def _has_password(self):
+    def has_password(self):
         return ('monitoring' in self.user_info) and \
             ('has_password' in self.user_info['monitoring']) and \
             (self.user_info['monitoring']['has_password'])
 
     def _save_api_password(self, password):
         """Encrypt and save the monitoring password locally
 
@@ -285,15 +323,15 @@
 
         logger.info(f"Saved the encrypted password at {api_pwd_file}")
 
         # Flag the password availability on the user configuration file
         self.user_info['monitoring']['has_password'] = True
         config.write_cfg_file(self.cfg, self.cfg_dir, self.user_info)
 
-    def _load_api_password(self):
+    def load_api_password(self):
         """Load the password used for non-GPG authentication
 
         When already defined, the password is available locally on an encrypted
         file. This function decrypts it and loads the password.
 
         """
         api_pwd_file = self._get_api_password_file_path()
@@ -316,59 +354,52 @@
 
         # The config file may indicate there is no password (if changing gpg
         # home dirs), but now we know there is a password that can be decrypted
         # with the given fingerprint. So update the info.
         self.user_info['monitoring']['has_password'] = True
         config.write_cfg_file(self.cfg, self.cfg_dir, self.user_info)
 
-    def _gen_api_password(self):
+    def gen_api_password(self):
         """Generate password for non-GPG-authenticated requests
 
         This is the password used as a lightweight authentication mechanism in
         specific endpoints that accept it as an alternative to the main
         authentication approach based on a detached GPG signature.
 
         """
         if self.api_pwd is not None:
             return
 
         request_payload = {}
         self.sign_request(request_payload)
-        rv = requests.post(account_pwd_endpoint, json=request_payload)
+        rv = requests.post(os.path.join(self.server_url, 'accounts',
+                                        "password"),
+                           json=request_payload)
 
         if (rv.status_code != requests.codes.ok):
             logger.error("Password generation failed")
             logger.error("{} ({})".format(rv.reason, rv.status_code))
         else:
             logger.info("Created a new password to authenticate reports")
             self.api_pwd = rv.json()['new_password']
             self._save_api_password(self.api_pwd)
 
-    def _register(self):
-        """Run the registration procedure
-
-        The procedure is divided in two steps:
+    def _register_interactive(self):
+        """Interactive configuration of the user setup
 
-        1) Interaction with the user;
-        2) Interaction with the API.
+        Executes the following steps:
+            1) Shows the registration explainer;
+            2) Ensures a GPG keyring is set up;
+            3) Loads and validates the GPG passphrase for decoding;
+            4) Collects the user address interactively.
 
-        This method implements step 1, where it sets up a GPG keyring, collects
-        the user address, and prepares the request parameters for registering
-        with the monitoring API. In the end, it dispatches step 2 on a thread.
-
-        Note step 2 has to run on a thread because it needs the receiver lock
-        first. By running on a thread, the main (parent) thread can proceed to
-        initializing the receiver.
+        Returns:
+            str: The collected address or None in case of failure.
 
         """
-        self.registration_running = True
-        self.registration_failure = False
-        logger.info("Initiating the registration with the Monitoring API")
-
-        # Save some state on the local cache
         cache = Cache(self.cfg_dir)
 
         # Show the explainer when running the registration for the first time
         # for this configuration
         if (cache.get(self.cfg + '.monitoring.explainer') is None):
             _register_explainer()
 
@@ -394,59 +425,84 @@
             logger.error("Aborting the registration with the Monitoring API")
             self.registration_running = False
             self.registration_failure = True
             return
 
         os.system('clear')
 
-        confirmed = False
+        # In interactive mode, the address is either loaded from the cache or
+        # provided by the user
+        use_cached_address = False
         cached_address = cache.get(self.cfg + '.monitoring.location')
         if cached_address is not None:
-            confirmed = util.ask_yes_or_no(
+            use_cached_address = util.ask_yes_or_no(
                 "Reporting from \"{}\"?".format(cached_address))
 
-        if confirmed:
+        if use_cached_address:
             address = cached_address
         else:
             util.fill_print(
                 "Please inform you city, state (if applicable), and country:")
-
-        while (not confirmed):
-            # City (required)
-            city = util.string_input("City")
-
-            # State (optional)
-            state = input("State: ")
-            if (len(state) > 0):
-                address = "{}, {}".format(city, state)
-            else:
-                address = city
-
-            # Country (required)
-            country = util.string_input("Country")
-
-            # Wait until the user confirms the full address
-            address += ", {}".format(country)
-            confirmed = util.ask_yes_or_no("\"{}\"?".format(address))
+            address = _ask_address()
             cache.set(self.cfg + '.monitoring.location', address)
             cache.save()
 
         os.system('clear')
+        return address
+
+    def _register(self, address=None):
+        """Run the registration procedure
+
+        The procedure is divided in two steps:
+
+        1) Interaction with the user;
+        2) Interaction with the API.
+
+        This method implements step 1 and dispatches step 2 on a thread. Step 2
+        has to run on a thread because it needs the receiver lock first. By
+        running on a thread, the main (parent) thread can proceed to
+        initializing the receiver.
+
+        Args:
+            address (str, optional): Receiver's address used in non-interactive
+                mode. Defaults to None.
+
+        """
+        self.registration_running = True
+        self.registration_failure = False
+        logger.info("Initiating the registration with the Monitoring API")
+
+        if self.interactive:
+            res = self._register_interactive()
+            if res is None:
+                return
+            # Use the address collected interactively, not the one provided by
+            # argument:
+            _address = res
+        else:
+            # In non-interactive mode, the caller must take care of the steps
+            # otherwise implemented by the interactive routine. Also, in this
+            # case, the address must be provided by argument.
+            assert is_gpg_keyring_set(self.gpg.gpghome)
+            assert self.gpg.passphrase is not None
+            assert address is not None
+            _address = address
 
         # Registration parameters
+        fingerprint = self.gpg.get_default_priv_key()['fingerprint']
         pubkey = self.gpg.gpg.export_keys(fingerprint)
         satellite = self.user_info['sat']['alias']
         rx_type = config.get_rx_model(self.user_info)
         antenna = config.get_antenna_model(self.user_info)
         lnb = config.get_lnb_model(self.user_info)
 
         # Run step 2 on a thread
         t1 = threading.Thread(target=self._register_thread,
                               daemon=True,
-                              args=(fingerprint, pubkey, address, satellite,
+                              args=(fingerprint, pubkey, _address, satellite,
                                     rx_type, antenna, lnb))
         t1.start()
 
     def _register_thread(self,
                          fingerprint,
                          pubkey,
                          address,
@@ -500,14 +556,15 @@
                                              'plaintext': False,
                                              'save_raw': True,
                                              'no_save': True
                                          })
         listen_thread.start()
 
         failure = False
+        account_endpoint = os.path.join(self.server_url, 'accounts')
         while (attempts > 0):
             rv = requests.post(account_endpoint,
                                json={
                                    'fingerprint': fingerprint,
                                    'publickey': pubkey,
                                    'city': address,
                                    'satellite': satellite,
@@ -532,16 +589,16 @@
 
             if (verified):
                 logger.info("Receiver already registered and verified")
                 self._save_credentials(uuid, fingerprint)
                 # If we are trying to register an account that already exists,
                 # chances are that the config dir already has its non-GPG
                 # password file. If not, try to redefine the password.
-                self._load_api_password()
-                self._gen_api_password()  # will generate only if necessary
+                self.load_api_password()
+                self.gen_api_password()  # will generate only if necessary
                 break
 
             try:
                 validation_key = recv_queue.get(timeout=10)
                 recv_queue.task_done()
             except queue.Empty:
                 logger.warning("Failed to receive the verification code. "
@@ -565,15 +622,15 @@
             else:
                 logger.info("Functional receiver successfully validated")
                 logger.info(
                     "Ready to report the Rx status to the Monitoring API")
                 self._save_credentials(uuid, fingerprint)
                 # Now that the account is verified, we can generate the
                 # password for non-GPG-authenticated requests
-                self._gen_api_password()
+                self.gen_api_password()
                 break
 
         if (attempts == 0):
             logger.error("Maximum number of registration attempts reached")
             logger.error("Please check if your receiver is running properly "
                          "and restart the application to try again")
             failure = True
@@ -581,14 +638,17 @@
         self.registration_running = False
         self.registration_failure = failure
 
         # Stop the API listener
         listen_loop.stop()
         listen_thread.join()
 
+    def get_metric_endpoint(self):
+        return os.path.join(self.server_url, "metrics")
+
     def sign_request(self, data, password_allowed=False):
         """Sign a dictionary of metrics to be reported to the monitoring API
 
         This function signs a request sent to the monitoring API. Two
         possibilities exist for signing: with a detached GPG signature of the
         payload or the account's password generated by the monitoring API.
 
@@ -645,50 +705,60 @@
         if key == 'uuid':
             key = key.upper()
         else:
             key = key.capitalize()
         print("| {:30s} | {:40s} |".format(key.replace('_', ' '), str(value)))
 
 
-def set_password(args):
+def _load_bs_monitoring(args):
     bs_monitoring = BsMonitoring(args.cfg,
                                  args.cfg_dir,
+                                 args.server,
                                  args.gnupghome,
                                  args.passphrase,
                                  lazy=True)
 
     if not bs_monitoring.registered:
-        return not_registered_error()
+        not_registered_error()
+        return
 
-    if not bs_monitoring._has_matching_keys():
+    if not bs_monitoring.has_matching_keys():
         logger.warning(
             "Please confirm the GPG home (option \'--gnupghome\') is "
             "set correctly")
         return
 
+    return bs_monitoring
+
+
+def set_password(args):
+    bs_monitoring = _load_bs_monitoring(args)
+    if bs_monitoring is None:
+        return
+
     bs_monitoring.gpg.prompt_passphrase('Please enter your GPG passphrase to '
                                         'decrypt/encrypt the password: ')
 
     if not bs_monitoring.gpg.test_passphrase(
             bs_monitoring.user_info['monitoring']['fingerprint']):
         return
 
-    if bs_monitoring._has_password():
-        bs_monitoring._load_api_password()
+    if bs_monitoring.has_password():
+        bs_monitoring.load_api_password()
 
     if bs_monitoring.api_pwd is not None:
         logger.info("Found existing password at {}.".format(
             bs_monitoring._get_api_password_file_path()))
         if not util.ask_yes_or_no("Reset password?", default='n'):
             print("Aborting")
             return
         # Let the password generation function generate a new one
         bs_monitoring.api_pwd = None
 
-    bs_monitoring._gen_api_password()
+    bs_monitoring.gen_api_password()
 
 
 def add_to_parser(parser):
     """Add monitoring API options to parser"""
     p = parser.add_argument_group(
         'Blockstream Monitoring API reporting options')
     p.add_argument(
@@ -707,14 +777,18 @@
 
 def subparser(subparsers):  # pragma: no cover
     p = subparsers.add_parser(
         'reporting',
         description="Manage the reporting to the Monitoring API",
         help='Manage the reporting to the Monitoring API',
         formatter_class=ArgumentDefaultsHelpFormatter)
+    p.add_argument('--server',
+                   type=str,
+                   default=DEFAULT_SERVER_URL,
+                   help="Monitoring API server address")
     p.add_argument(
         '--gnupghome',
         '--gpghome',
         default=".gnupg",
         help="GPG home directory holding the keypair configured for "
         "authentication with the Monitoring API, relative to the "
         "config directory set by option --cfg-dir")
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/rp.py` & `blocksat-cli-0.4.6/blocksatcli/rp.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     safe_ifname = ifname.replace(".", "/")
     cmd = [
         "sysctl", "-w", "net.ipv4.conf." + safe_ifname + ".rp_filter=" + val
     ]
 
     action = "Enabling" if val == "1" else "Disabling"
     if (not runner.dry):
-        print("{} the RP filter on interface \"{}\"".format(action, ifname))
+        logger.info("{} the RP filter on interface \"{}\"".format(
+            action, ifname))
     runner.run(cmd, root=True)
 
 
 def _rm_filter(ifname):
     _write_filter(ifname, "0")
 
 
@@ -64,15 +65,15 @@
     """
     assert (isinstance(dvb_ifs, list))
 
     # If the "all" rule is already disabled, disable only the target DVB-S2
     # interface.
     if (_read_filter("all", nodry=True) == 0):
         if (not runner.dry):
-            print("RP filter for \"all\" interfaces is already disabled")
+            logger.info("RP filter for \"all\" interfaces is already disabled")
 
         for dvb_if in dvb_ifs:
             _rm_filter(dvb_if)
 
     # If the "all" rule is enabled, disable it, and manually enable the RP
     # filtering on all other interfaces.
     else:
@@ -84,63 +85,70 @@
             if (interface == "all" or interface == "lo"
                     or interface in dvb_ifs):
                 continue
 
             # Enable the RP filter if not enabled already.
             if (_read_filter(interface, nodry=True) > 0):
                 if (not runner.dry):
-                    print("RP filter is already enabled on interface %s" %
-                          (interface))
+                    logger.info(
+                        "RP filter is already enabled on interface %s" %
+                        (interface))
             else:
                 _add_filter(interface)
 
         # Disable the overall RP filter
         _rm_filter("all")
 
         # And disable RP filtering on the DVB interface
         for dvb_if in dvb_ifs:
             _rm_filter(dvb_if)
 
 
-def set_filters(dvb_ifs, prompt=True, dry=False):
-    """Disable reverse-path (RP) filtering for the DVB interfaces
+def verify(dvb_ifs):
+    """Check if the RP filters are already configured properly"""
+    rp_filters_set = list()
+    rp_filters_set.append(_read_filter("all", nodry=True) == 0)
+    for dvb_if in dvb_ifs:
+        rp_filters_set.append(_read_filter(dvb_if, nodry=True) == 0)
+
+    all_rp_filters_set = all(rp_filters_set)
+    if all_rp_filters_set:
+        logger.info("RP filtering is already configured on DVB interfaces.")
+
+    return all_rp_filters_set
+
+
+def configure(dvb_ifs, prompt=True, dry=False):
+    """Configure reverse-path (RP) filtering for the DVB interfaces
 
     Args:
         dvb_ifs : list of DVB network interfaces
         prompt  : Whether to prompt user before applying a configuration
         dry     : Dry run mode
 
     """
     assert (isinstance(dvb_ifs, list))
     runner.set_dry(dry)
-    util.print_header("Reverse Path Filters")
 
-    # Check if the RP filters are already configured properly
-    rp_filters_set = list()
-    rp_filters_set.append(_read_filter("all", nodry=True) == 0)
-    for dvb_if in dvb_ifs:
-        rp_filters_set.append(_read_filter(dvb_if, nodry=True) == 0)
-
-    if (all(rp_filters_set)):
-        print("Current RP filtering configurations are already OK")
-        print("Skipping...")
+    if not dry and verify(dvb_ifs):
         return
 
+    util.print_header("Reverse Path Filters")
     util.fill_print("It will be necessary to reconfigure some reverse path \
     (RP) filtering rules applied by the Linux kernel. This is required to \
     prevent the filtering of the one-way Blockstream Satellite traffic.")
 
     if (runner.dry):
         util.fill_print("The following command(s) would be executed to \
         reconfigure the RP filters:")
 
     if (runner.dry or (not prompt) or util.ask_yes_or_no("OK to proceed?")):
         _set_filters(dvb_ifs)
     else:
-        print("RP filtering configuration cancelled")
+        logger.info("RP filtering configuration cancelled")
 
 
 def subparser(subparsers):  # pragma: no cover
     """Parser for rp command"""
     p = subparsers.add_parser('reverse-path',
                               aliases=['rp'],
                               description="Set reverse path filters",
@@ -165,8 +173,8 @@
 
 def run(args):
     """Call function that sets reverse path filters
 
     Handles the reverse-path subcommand
 
     """
-    set_filters([args.interface], prompt=(not args.yes), dry=args.dry_run)
+    configure([args.interface], prompt=(not args.yes), dry=args.dry_run)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/satip.py` & `blocksat-cli-0.4.6/blocksatcli/satip.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,31 +132,46 @@
         except ValueError as e:
             logger.warning("Failed to parse the local Sat-IP client address")
             logger.warning(e)
             return
         logger.debug("Local Sat-IP client address: {}".format(local_addr))
         self.local_addr = local_addr
 
-    def discover(self, interactive=True, src_port=None, interface=None):
-        """Discover the Sat-IP receivers in the local network via UPnP"""
+    def discover(self, src_port, interface):
+        """Discover the Sat-IP receivers in the local network via UPnP
+
+        Args:
+            src_port: Source port.
+            interface: Network interface.
+
+        Retuns:
+            List with the discovered devices
+
+        """
         upnp = UPnP(src_port, interface)
         devices = upnp.discover()
 
         if (len(devices) == 0):
-            return
+            return []
 
         # Filter the Sat-IP devices
         sat_ip_devices = [{
             'host': d.host,
             'base_url': d.base_url
         } for d in devices if d.friendly_name == "SELFSAT-IP"]
         # Note: convert to dictionary so that _ask_multiple_choice can
         # deep-copy the selected element (which would not work for the original
         # SSDPDevice object).
 
+        return sat_ip_devices
+
+    def select_receiver(self, interactive=True, src_port=None, interface=None):
+        """Select Sat-IP receiver discovered in the local network via UPnP"""
+        sat_ip_devices = self.discover(src_port, interface)
+
         if (len(sat_ip_devices) == 0):
             return
 
         if (len(sat_ip_devices) > 1):
             if (not interactive):
                 logger.warning("Found multiple Sat-IP receivers.")
                 logger.warning("Selecting the receiver at {}".format(
@@ -698,14 +713,26 @@
         default=False,
         action='store_true',
         help="Immediately retry the connection if an HTTP error occurs while "
         "reading the MPEG transport stream from the Sat-IP server")
     tsp.add_to_parser(p)
     monitoring.add_to_parser(p)
     p.set_defaults(func=launch)
+
+    subsubparsers = p.add_subparsers(title='subcommands',
+                                     help='Target sub-command')
+
+    p1 = subsubparsers.add_parser(
+        'list',
+        aliases=['ls'],
+        description='List Sat-IP devices discovered in the local network',
+        help='List Sat-IP devices discovered in the local network',
+        formatter_class=ArgumentDefaultsHelpFormatter)
+    p1.set_defaults(func=list_devices)
+
     return p
 
 
 def launch(args, monitor: monitoring.Monitor = None):
     info = config.read_cfg_file(args.cfg, args.cfg_dir)
     if (info is None):
         return
@@ -714,16 +741,16 @@
 
     if (not dependencies.check_dependencies('sat-ip')):
         return
 
     # Discover or define the IP address to communicate with the Sat-IP server
     sat_ip = SatIp()
     if args.addr is None and 'ip_addr' not in info['setup']:
-        sat_ip.discover(src_port=args.ssdp_src_port,
-                        interface=args.ssdp_net_if)
+        sat_ip.select_receiver(src_port=args.ssdp_src_port,
+                               interface=args.ssdp_net_if)
         if (sat_ip.host is None):
             logger.error("Could not find a Sat-IP receiver")
             logger.info("Check your network or specify the receiver address "
                         "through option -a/--addr")
             sys.exit(1)
     else:
         addr = args.addr if args.addr is not None else info['setup']['ip_addr']
@@ -798,7 +825,33 @@
 
     try:
         tsp_handler.proc.communicate()
     except KeyboardInterrupt:
         tsp_handler.proc.kill()
 
     print()
+
+
+def list_devices(args):
+    """List Sat-IP devices"""
+    info = config.read_cfg_file(args.cfg, args.cfg_dir)
+    if (info is None):
+        return
+
+    util.check_configured_setup_type(info, defs.sat_ip_setup_type, logger)
+
+    if (not dependencies.check_dependencies('sat-ip')):
+        return
+
+    # Discover or define the IP address to communicate with the Sat-IP server
+    sat_ip = SatIp()
+    sat_ip_devices = sat_ip.discover(src_port=args.ssdp_src_port,
+                                     interface=args.ssdp_net_if)
+
+    if len(sat_ip_devices) == 0:
+        logger.info("No Sat-IP receiver found.")
+        return
+
+    for device in sat_ip_devices:
+        logger.info(f" - Found receiver at {device['host']}")
+
+    return sat_ip_devices
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/sdr.py` & `blocksat-cli-0.4.6/blocksatcli/sdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,47 @@
 import requests
 
 from . import config, defs, util, dependencies, monitoring, tsp
 
 logger = logging.getLogger(__name__)
 runner = util.ProcessRunner(logger)
 
+MBYTES = 2**20
+
+
+def _verify_max_pipe_size(pipesize):
+    """Verify the maximum size of pipes currently configured
+
+    Returns:
+        tuple (bool, int): The boolean indicates whether the currently
+        configured pipe size is less than required. The integer indicates the
+        currently pipe size.
+
+    """
+    if (not which("sysctl")):
+        logging.error("Couldn't check max-pipe-size. Please check how to tune "
+                      "it in your OS.")
+        return False
+
+    ret = subprocess.check_output(["sysctl", "fs.pipe-max-size"])
+    current_max = int(ret.decode().split()[-1])
+
+    return current_max < pipesize, current_max
+
 
 def _tune_max_pipe_size(pipesize, interactive=True):
     """Tune the maximum size of pipes"""
     if (not which("sysctl")):
         logging.error("Couldn't tune max-pipe-size. Please check how to tune "
                       "it in your OS.")
         return False
 
-    ret = subprocess.check_output(["sysctl", "fs.pipe-max-size"])
-    current_max = int(ret.decode().split()[-1])
+    insufficient_pipe_size, current_max = _verify_max_pipe_size(pipesize)
 
-    if (current_max < pipesize):
+    if insufficient_pipe_size:
         cmd = ["sysctl", "-w", "fs.pipe-max-size=" + str(pipesize)]
         print(
             textwrap.fill("The maximum pipe size that is currently "
                           "configured in your OS is of {} bytes, which is "
                           "not sufficient for the receiver application. "
                           "It will be necessary to run the following command "
                           "as root:".format(current_max),
@@ -309,14 +330,39 @@
     p1 = subprocess.Popen(rtl_cmd)
     try:
         p1.wait()
     except KeyboardInterrupt:
         p1.kill()
 
 
+def verify(args):
+    """Check the host configuration"""
+    if not args.implementation == 'leandvb':
+        return True
+
+    logger.info("Checking SDR host configuration")
+    pipe_size_bytes = int(args.pipe_size * MBYTES)
+    insufficient_pipe_size, _ = _verify_max_pipe_size(pipe_size_bytes)
+
+    return not insufficient_pipe_size
+
+
+def configure(args):
+    """Configure the host"""
+    if not args.implementation == 'leandvb':
+        return True
+
+    if verify(args):
+        return True
+
+    logger.info("Running SDR host configuration")
+    pipe_size_bytes = int(args.pipe_size * MBYTES)
+    return _tune_max_pipe_size(pipe_size_bytes, not args.yes)
+
+
 def subparser(subparsers):  # pragma: no cover
     """Parser for sdr command"""
     default_impl = 'leandvb' if which('dvbs2-rx') is None else 'gr-dvbs2rx'
 
     p = subparsers.add_parser('sdr',
                               description="Launch SDR receiver",
                               help='Launch SDR receiver',
@@ -474,18 +520,18 @@
     info = config.read_cfg_file(args.cfg, args.cfg_dir)
 
     if (info is None):
         return
 
     util.check_configured_setup_type(info, defs.sdr_setup_type, logger)
 
-    if args.implementation == 'leandvb':
-        pipe_size_bytes = int(args.pipe_size * (2**20))
-        if (not _tune_max_pipe_size(pipe_size_bytes, interactive)):
-            return
+    # Configure the host
+    pipe_size_bytes = int(args.pipe_size * MBYTES)
+    if not configure(args):
+        return
 
     # Check if all dependencies are installed
     apps = ["rtl_sdr"]
     if not args.record:
         if args.implementation == 'leandvb':
             apps.extend(["leandvb", "ldpc_tool"])
         else:
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/standalone.py` & `blocksat-cli-0.4.6/blocksatcli/standalone.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,15 +172,16 @@
         """Set variable via SNMP
 
         Args:
             variable : variable to set via SNMP.
             value    : value to set on the given variable.
 
         Returns:
-            bool: Whether the request was successful.
+            bool: Whether the request was successful. Returns true in dry run
+                mode.
 
         """
         if (self.dry):
             # Convert to the corresponding net-snmp command
             for key, val in key_vals:
                 # SNMP OID
                 if (isinstance(key, tuple)):
@@ -369,23 +370,27 @@
                     elif (label == "Standard"):
                         val = cfg[key].upper()
                     else:
                         val = cfg[key]
                     print("- {}: {}".format(label, val))
         return True
 
-    def configure(self, info, freq_corr):
-        """Configure the S400
+    def verify(self, info, freq_corr) -> list:
+        """Check configuration to be updated on the S400
 
         Args:
             info (dict): User info dictionary.
             freq_corr (float): Frequency correction in MHz.
 
+        Returns:
+            list: List of tuples containing the parameters to be
+                applied/updated on the S400.
+
         """
-        logger.info("Configuring the S400 receiver at {} via SNMP".format(
+        logger.info("Checking S400 receiver config at {} via SNMP".format(
             self.address))
 
         l_band_freq = int(round(info['freqs']['l_band'] + freq_corr, 2) * 1e6)
         lo_freq = int(info['freqs']['lo'] * 1e6)
         sym_rate = defs.sym_rate[info['sat']['alias']]
         if (info['lnb']['pol'].lower() == "dual"
                 and 'v1_pointed' in info['lnb'] and info['lnb']['v1_pointed']):
@@ -453,20 +458,17 @@
             no_skip.add(status_oid_str)
 
         target_cfg["LNB power"] = [
             ('s400LNBSupply', 'enabled'),
             ('s400Enable22KHzTone', tone),
         ]
 
+        update_cfg = []
         for section in target_cfg.keys():
-            set_calls = 0
-            if self.dry:
-                logger.info(section)
-            else:
-                logger.info("Configuring {}".format(section))
+            logger.info("Checking {} configuration".format(section))
 
             for config_tuple in target_cfg[section]:
                 key, val = config_tuple
                 if isinstance(key, tuple):
                     key = _tuple_to_dotted_str(key)
                 else:
                     key += '.0'
@@ -482,22 +484,39 @@
                         pass
 
                     if val == current_val and key not in no_skip:
                         logger.debug("Option {} already set to {}".format(
                             key, val))
                         continue  # already set
 
-                set_calls += 1
-                if not self._set(config_tuple):
-                    if (not self.dry):
-                        logger.error("SNMP configuration error")
-                    return
+                update_cfg.append(config_tuple)
+
+        return update_cfg
+
+    def configure(self, info, freq_corr, update_cfg=None):
+        """Configure the S400
 
-            if self.dry and set_calls == 0:
-                logger.info("- Already configured")
+        Args:
+            info (dict): User info dictionary.
+            freq_corr (float): Frequency correction in MHz.
+
+        """
+        if update_cfg is None:
+            update_cfg = self.verify(info, freq_corr)
+
+        if self.dry and len(update_cfg) == 0:
+            logger.info("- Already configured")
+            return
+
+        logger.info("Configuring the S400 receiver at {} via SNMP".format(
+            self.address))
+        for config_tuple in update_cfg:
+            if not self._set(config_tuple):
+                logger.error("SNMP configuration error")
+                sys.exit(1)
 
         if (not self.dry):
             logger.info("Receiver configured successfully")
 
 
 def _parse_address(user_info, arg_addr):
     """Parse the receiver's IP address"""
@@ -551,33 +570,36 @@
                     help='Network interface connected to the standalone \
                     receiver')
     p1.add_argument('-y',
                     '--yes',
                     default=False,
                     action='store_true',
                     help="Default to answering Yes to configuration prompts")
-    p1.add_argument('--host-only',
-                    default=False,
-                    action='store_true',
-                    help="Configure the host only and skip the receiver "
-                    "configuration")
-    p1.add_argument('--rx-only',
-                    default=False,
-                    action='store_true',
-                    help="Configure the receiver only and skip the host "
-                    "configuration")
+    only_opts = p1.add_mutually_exclusive_group()
+    only_opts.add_argument(
+        '--host-only',
+        default=False,
+        action='store_true',
+        help="Configure the host only and skip the receiver "
+        "configuration")
+    only_opts.add_argument(
+        '--rx-only',
+        default=False,
+        action='store_true',
+        help="Configure the receiver only and skip the host "
+        "configuration")
     p1.add_argument("--dry-run",
                     action='store_true',
                     default=False,
                     help="Print all commands but do not execute them")
     p1.add_argument('--freq-corr',
                     default=0,
                     type=float,
                     help='Carrier frequency offset correction in kHz')
-    p1.set_defaults(func=cfg_standalone)
+    p1.set_defaults(func=configure)
 
     # Monitoring
     p2 = subsubparsers.add_parser(
         'monitor',
         description="Monitor the standalone receiver",
         help='Monitor the standalone receiver',
         formatter_class=ArgumentDefaultsHelpFormatter)
@@ -595,67 +617,137 @@
 
     util.check_configured_setup_type(user_info, defs.standalone_setup_type,
                                      logger)
 
     return user_info
 
 
-def cfg_standalone(args):
-    """Configure the standalone receiver and the host
+def verify(args) -> bool:
+    """Verify the configuration of the standalone receiver and host
 
-    Set all parameters required on the standalone receiver: signal, LNB, and
-    MPE parameters. Then, configure the host to communicate with the the
-    standalone DVB-S2 receiver by setting reverse-path filters and firewall
-    configurations.
+    Returns:
+        dict: Dictionary indicating which components (package dependencies, RP
+            filters, firewall, or S400) still need configuration. When the S400
+            needs configuration, the dictionary also contains the list of
+            tuples to be applied to the S400 over SNMP.
 
     """
+    res = {
+        'config': {
+            'deps': args.rx_only,  # assume OK if --rx-only
+            'rp': args.rx_only,
+            'firewall': args.rx_only,
+            's400': args.host_only,  # assume OK if --host-only
+        },
+        'user_info': None,
+        's400': None
+    }
+
+    logger.info("Checking current configuration.")
     user_info = _common(args)
+    res['user_info'] = user_info
     if (user_info is None):
-        return
+        logger.error("Receiver configuration not found.")
+        sys.exit(0)
 
     if (not args.host_only):
         freq_corr_mhz = args.freq_corr / 1e3
         if round(freq_corr_mhz, 2) != freq_corr_mhz:
             logger.error(
                 "Please specify the frequency correction parameter as "
                 "a multiple of 10 kHz")
             sys.exit(1)
 
     # Configure the subprocess runner
     runner.set_dry(args.dry_run)
 
     # IP Address
     rx_ip_addr = _parse_address(user_info, args.address)
+    if rx_ip_addr is None:
+        return False
 
     if (not args.rx_only):
         if 'netdev' not in user_info['setup']:
             assert (args.interface is not None), \
                 ("Please specify the network interface through option "
                  "\"-i/--interface\"")
 
         interface = args.interface if (args.interface is not None) else \
             user_info['setup']['netdev']
 
         # Check if all dependencies are installed
-        if (not dependencies.check_apps(["iptables"])):
-            return
+        res['config']['deps'] = dependencies.check_apps(["iptables"])
+
+        res['config']['rp'] = rp.verify([interface])
+        if not res['config']['rp']:
+            logger.info("Reverse path (RP) filters not configured.")
+
+        res['config']['firewall'] = firewall.verify(
+            net_ifs=[interface],
+            ports=defs.src_ports,
+            src_ip=user_info['sat']['ip'],
+            igmp=True)
+        if not res['config']['firewall']:
+            logger.info("Firewall rules not configured.")
+
+    if (not args.host_only):
+        s400 = S400Client(args.demod, rx_ip_addr, args.port, dry=args.dry_run)
+        s400.check_reachable()
+        missing_snmp_configs = s400.verify(user_info, freq_corr_mhz)
+        res['config']['s400'] = len(missing_snmp_configs) == 0
+        if not res['config']['s400']:
+            res['s400'] = missing_snmp_configs
+
+    return res
+
+
+def configure(args):
+    """Configure the standalone receiver and the host
+
+    Set all parameters required on the standalone receiver: signal, LNB, and
+    MPE parameters. Then, configure the host to communicate with the the
+    standalone DVB-S2 receiver by setting reverse-path filters and firewall
+    configurations.
+
+    """
+    verify_res = verify(args)
+    if all(verify_res['config'].values()):
+        logger.info("Receiver already configured")
+        return
+
+    user_info = verify_res['user_info']
+    assert (user_info is not None)
+
+    # Configure the subprocess runner
+    runner.set_dry(args.dry_run)
+
+    interface = args.interface if (args.interface is not None) else \
+        user_info['setup']['netdev']
 
-        rp.set_filters([interface], prompt=(not args.yes), dry=args.dry_run)
+    if not verify_res['config']['rp']:
+        rp.configure([interface], prompt=(not args.yes), dry=args.dry_run)
+
+    if not verify_res['config']['firewall']:
         firewall.configure([interface],
                            defs.src_ports,
                            user_info['sat']['ip'],
                            igmp=True,
                            prompt=(not args.yes),
                            dry=args.dry_run)
 
-    if (not args.host_only):
-        util.print_header("Receiver Configuration")
+    if not verify_res['config']['s400']:
+        assert verify_res['s400'] is not None
+        assert isinstance(verify_res['s400'], list)
+
+        rx_ip_addr = _parse_address(user_info, args.address)
+        freq_corr_mhz = args.freq_corr / 1e3
+
         s400 = S400Client(args.demod, rx_ip_addr, args.port, dry=args.dry_run)
         s400.check_reachable()
-        s400.configure(user_info, freq_corr_mhz)
+        s400.configure(user_info, freq_corr_mhz, verify_res['s400'])
 
 
 def _get_monitor(args):
     """Create an object of the Monitor class
 
     Args:
         args : Parser arguments.
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_bitcoin.py` & `blocksat-cli-0.4.6/blocksatcli/test_bitcoin.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_cache.py` & `blocksat-cli-0.4.6/blocksatcli/test_cache.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_config.py` & `blocksat-cli-0.4.6/blocksatcli/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,85 +26,83 @@
         user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertEqual(user_info, test_info)
 
     @patch('blocksatcli.util.ask_yes_or_no')
     def test_cfg_patching(self, mock_yes_or_no):
         mock_yes_or_no.return_value = False
 
-        # Configuration based on T11N AFR before the update on May 31st 2022:
-        test_info = {
-            "sat": {
-                "name": "Telstar 11N Africa",
-                "alias": "T11N AFR",
-                "dl_freq": 11480.7,
-                "band": "Ku",
-                "pol": "H",
-                "ip": "172.16.235.17"
-            },
-            "freqs": {
-                "dl": 11480.7,
-                "lo": 9750.0,
-                "l_band": 1730.7
+        change_map = {
+            'T11N AFR': {
+                'old_freq': 11480.7,
+                'new_freq': 11452.1,
+            },  # T11N AFR update on May 31st 2022
+            'T11N EU': {
+                'old_freq': 11484.3,
+                'new_freq': 11505.4
+            },  # T11N EU update on May 31st 2022:
+            'G18': {
+                'old_freq': 12016.4,
+                'new_freq': 11913.4
+            },  # G18 update on March 3, 2023
+            'T18V C': {
+                'old_freq': 4053.83,
+                'new_freq': 4057.4
+            },  # T18V C update on July 12, 2023
+        }
+
+        for satellite in change_map.keys():
+            sat_def = defs.get_satellite_def(satellite)
+            sat_def['dl_freq'] = change_map[satellite]['old_freq']
+            band = sat_def['band']
+            example_lnb = "Titanium C1-PLL" if band == 'C' else \
+                "GEOSATpro UL1PLL"
+            lo_freq = 5150.0 if band == 'C' else (
+                9750.0 if sat_def['dl_freq'] < 11700.0 else 10600.0)
+            old_l_band = config._calc_if_freq(
+                change_map[satellite]['old_freq'], lo_freq, band)
+            new_l_band = config._calc_if_freq(
+                change_map[satellite]['new_freq'], lo_freq, band)
+
+            # Original configuration
+            chan_conf = config.get_chan_file_path(self.cfg_dir, self.cfg_name)
+            old_info = {
+                "sat": sat_def,
+                "freqs": {
+                    "dl": change_map[satellite]['old_freq'],
+                    "lo": lo_freq,
+                    "l_band": old_l_band
+                },
+                "lnb": defs.get_lnb_def(*example_lnb.split()),
+                "setup": {
+                    "type": defs.linux_usb_setup_type,
+                    "channel": chan_conf
+                }
             }
-        }
-        config.write_cfg_file(self.cfg_name, self.cfg_dir, test_info)
-
-        # Check patching
-        user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
-        self.assertEqual(user_info['sat']['dl_freq'], 11452.1)
-        self.assertEqual(user_info['freqs']['dl'], 11452.1)
-        self.assertEqual(user_info['freqs']['l_band'], 1702.1)
-
-        # Configuration based on T11N EU before the update on May 31st 2022:
-        test_info = {
-            "sat": {
-                "name": "Telstar 11N Europe",
-                "alias": "T11N EU",
-                "dl_freq": 11484.3,
-                "band": "Ku",
-                "pol": "V",
-                "ip": "172.16.235.25"
-            },
-            "freqs": {
-                "dl": 11484.3,
-                "lo": 9750.0,
-                "l_band": 1734.3
+            new_info = {
+                "sat": defs.get_satellite_def(satellite),
+                "freqs": {
+                    "dl": change_map[satellite]['new_freq'],
+                    "lo": lo_freq,
+                    "l_band": new_l_band
+                },
+                "lnb": defs.get_lnb_def(*example_lnb.split()),
+                "setup": {
+                    "type": defs.linux_usb_setup_type,
+                    "channel": chan_conf
+                }
             }
-        }
-        config.write_cfg_file(self.cfg_name, self.cfg_dir, test_info)
+            config.write_cfg_file(self.cfg_name, self.cfg_dir, old_info)
+            config.write_chan_conf(old_info, chan_conf)
 
-        # Check patching
-        user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
-        self.assertEqual(user_info['sat']['dl_freq'], 11505.4)
-        self.assertEqual(user_info['freqs']['dl'], 11505.4)
-        self.assertEqual(user_info['freqs']['l_band'], 1755.4)
+            # Before patching, the channel conf file should be inferred invalid
+            config.verify_chan_conf(new_info)
 
-        # Configuration based on G18 before the update on March 3, 2023:
-        test_info = {
-            "sat": {
-                'name': "Galaxy 18",
-                'alias': "G18",
-                'dl_freq': 12016.4,
-                'band': "Ku",
-                'pol': "H",
-                'ip': "172.16.235.1"
-            },
-            "freqs": {
-                "dl": 12016.4,
-                "lo": 10750.0,
-                "l_band": 1266.4
-            }
-        }
-        config.write_cfg_file(self.cfg_name, self.cfg_dir, test_info)
-
-        # Check patching
-        user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
-        self.assertEqual(user_info['sat']['dl_freq'], 11913.4)
-        self.assertEqual(user_info['freqs']['dl'], 11913.4)
-        self.assertEqual(user_info['freqs']['l_band'], 1163.4)
+            # Check patching
+            user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
+            self.assertEqual(user_info, new_info)
 
         # Configuration based on a satellite that is not patched
         test_info = {
             "sat": {
                 "name": "Eutelsat 113",
                 "alias": "E113",
                 "dl_freq": 12066.9,
@@ -136,44 +134,65 @@
         info = {
             'sat': defs.get_satellite_def('G18'),
             'lnb': defs.get_lnb_def('GEOSATpro', 'UL1PLL')
         }
         chan_file = os.path.join(self.cfg_dir, self.cfg_name + "-channel.conf")
 
         # First conf file
-        config._cfg_chan_conf(info, chan_file)
+        config.write_chan_conf(info, chan_file)
         conf = config._parse_chan_conf(chan_file)
         self.assertEqual(int(conf['FREQUENCY']), info['sat']['dl_freq'] * 1e3)
         self.assertEqual(conf['POLARIZATION'], 'HORIZONTAL')
         self.assertEqual(conf['VIDEO_PID'], '32')
 
         # Change PID definitions and try generating the conf file again
         defs.pids = [60, 61]
 
         # Generate a conf file but refuse to overwrite the pre-existing one
         mock_yes_or_no.return_value = False
-        config._cfg_chan_conf(info, chan_file)
+        config.write_chan_conf(info, chan_file)
         conf = config._parse_chan_conf(chan_file)
         # Nothing should be changed
         self.assertEqual(conf['VIDEO_PID'], '32')
 
         # Overwrite the pre-existing conf file
         mock_yes_or_no.return_value = True
-        config._cfg_chan_conf(info, chan_file)
+        config.write_chan_conf(info, chan_file)
         conf = config._parse_chan_conf(chan_file)
         # Now the new PID settings should be in the file
         self.assertEqual(conf['VIDEO_PID'], '60+61')
 
         # Add the v1-pointed flag to change the polarization
         info['lnb']['v1_pointed'] = True
         info['lnb']['v1_psu_voltage'] = 13
-        config._cfg_chan_conf(info, chan_file)
+        config.write_chan_conf(info, chan_file)
         conf = config._parse_chan_conf(chan_file)
         self.assertEqual(conf['POLARIZATION'], 'VERTICAL')
 
+    def test_verify_chan_config(self):
+        chan_file = config.get_chan_file_path(self.cfg_dir, self.cfg_name)
+        info = {
+            'sat': defs.get_satellite_def('G18'),
+            'lnb': defs.get_lnb_def('GEOSATpro', 'UL1PLL'),
+            'setup': {
+                'channel': chan_file
+            }
+        }
+
+        # First, generate the channel config file
+        config.write_chan_conf(info, chan_file)
+
+        # The verify function should check if the channel config file matches
+        # with the configuration expected for the user's satellite and setup
+        self.assertTrue(config.verify_chan_conf(info))
+
+        # Change the satellite to one that is not in the config file
+        info['sat'] = defs.get_satellite_def('T11N EU')
+        self.assertFalse(config.verify_chan_conf(info))
+
     @patch('blocksatcli.util.ask_yes_or_no')
     def test_cfg_reseting(self, mock_yes_or_no):
         # Create the config file
         test_info = {'test': 123}
         config.write_cfg_file(self.cfg_name, self.cfg_dir, test_info)
 
         # Check creation
@@ -281,14 +300,27 @@
         }
         self.assertEqual(config.get_lnb_model(info), 'Custom Universal LNB')
         info['lnb']['universal'] = False
         self.assertEqual(config.get_lnb_model(info), 'Custom Ku-band LNB')
         info['lnb']['band'] = "C"
         self.assertEqual(config.get_lnb_model(info), 'Custom C-band LNB')
 
+    def test_rx_label(self):
+        info = {'setup': {'type': 'Linux USB'}}
+        self.assertEqual(config.get_rx_label(info), 'usb')
+
+        info = {'setup': {'type': 'Software-defined'}}
+        self.assertEqual(config.get_rx_label(info), 'sdr')
+
+        info = {'setup': {'type': 'Standalone'}}
+        self.assertEqual(config.get_rx_label(info), 'standalone')
+
+        info = {'setup': {'type': 'Sat-IP'}}
+        self.assertEqual(config.get_rx_label(info), 'sat-ip')
+
 
 class TestReceiversSetupConfig(TestEnv):
 
     def setUp(self):
         super().setUp()
         self.args = argparse.Namespace(cfg=self.cfg_name, cfg_dir=self.cfg_dir)
 
@@ -461,33 +493,43 @@
         self.expected_config["setup"][
             'channel'] = f"{self.cfg_dir}/{self.cfg_name}-channel.conf"
         config.configure(self.args)
         cfg_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertEqual(cfg_info, self.expected_config)
 
     @patch('builtins.input')
-    def test_sdr_setup(self, mock_user_input):
+    @patch('blocksatcli.gqrx.os.path.expanduser')
+    def test_sdr_setup(self, mock_user_home, mock_user_input):
         """Test Software-defined Radio (SDR) Setup
         """
         # User Input:
         mock_user_input.side_effect = [
             0,  # Satellite: G18
             3,  # DVB-S2 receiver: SDR
             0,  # Antenna: Satellite Dish (45cm / 18in)
             0,  # LNB: GEOSATpro UL1PLL
-            0  # Power Supply: Directv 21 Volt Power
+            0,  # Power Supply: Directv 21 Volt Power
+            'y'  # Generate gqrx config file
         ]
+
+        # Mock the user's home directory so that the gqrx conf is saved on the
+        # temporary test directory
+        mock_user_home.return_value = self.cfg_dir
+        gqrx_path = os.path.join(self.cfg_dir, '.config', 'gqrx')
+        gqrx_conf_file = os.path.join(gqrx_path, 'default.conf')
+
         self.expected_config["setup"] = defs.get_demod_def('', 'RTL-SDR')
         self.expected_config['setup']['antenna'] = defs.get_antenna_def('45cm')
         self.expected_config["lnb"].pop("v1_pointed")
         self.expected_config["lnb"]["psu_voltage"] = 21
 
         config.configure(self.args)
         cfg_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertEqual(cfg_info, self.expected_config)
+        self.assertTrue(os.path.exists(gqrx_conf_file))
 
     @patch('os.listdir')
     @patch('builtins.input')
     def test_setup_with_custom_ku_band_lnb(self, mock_user_input,
                                            mock_eth_interface):
         """Test setup with custom Ku band LNB
         """
@@ -641,17 +683,17 @@
             "in_range": [3400.0, 4800.0],
             "lo_freq": 5150.0,
             "universal": False,
             "band": "C",
             "pol": "V"
         }
         self.expected_config["freqs"] = {
-            "dl": 4053.83,
+            "dl": 4057.4,
             "lo": 5150.0,
-            "l_band": 1096.17
+            "l_band": 1092.6
         }
 
         # Continue with invalid frequency range
         config.configure(self.args)
         cfg_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertEqual(cfg_info, self.expected_config)
 
@@ -685,17 +727,17 @@
             "in_range": [3400.0, 4200.0],
             "lo_freq": 5150.0,
             "universal": False,
             "band": "C",
             "pol": "V"
         }
         self.expected_config["freqs"] = {
-            "dl": 4053.83,
+            "dl": 4057.4,
             "lo": 5150.0,
-            "l_band": 1096.17
+            "l_band": 1092.6
         }
 
         config.configure(self.args)
         cfg_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertEqual(cfg_info, self.expected_config)
 
     @patch('builtins.input')
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_gqrx.py` & `blocksat-cli-0.4.6/blocksatcli/test_gqrx.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_helpers.py` & `blocksat-cli-0.4.6/blocksatcli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_monitoring.py` & `blocksat-cli-0.4.6/blocksatcli/test_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 from unittest.mock import patch, call
 
 from requests.exceptions import ConnectionError
 
 from . import monitoring
-from .monitoring_api import metric_endpoint
 from .test_helpers import create_test_setup, TestEnv
 
 
 class TestReceiverReporter(TestEnv):
 
     def configure_reporter_setup(self,
                                  cfg_name="test_config",
-                                 report_endpoint=metric_endpoint,
+                                 report_endpoint="test_endpoint",
+                                 bs_monitoring=False,
                                  gen_gpg_key=False,
                                  mon_api_registered=False,
-                                 mon_api_gen_pwd=False,
-                                 mon_api_reset_pwd=False):
+                                 mon_api_gen_pwd=False):
         """Configure reporter setup
 
         This function creates a test setup with a complete receiver
         configuration file and the GPG keys. It also instantiates the
         monitoring.Reporter with the correct configuration for testing.
 
         """
@@ -30,18 +29,18 @@
                                       gen_gpg_key=gen_gpg_key,
                                       mon_api_registered=mon_api_registered,
                                       mon_api_gen_password=mon_api_gen_pwd)
 
         reporter = monitoring.Reporter(cfg=cfg_name,
                                        cfg_dir=self.cfg_dir,
                                        dest_addr=report_endpoint,
+                                       bs_monitoring=bs_monitoring,
                                        hostname='hostname-test',
                                        gnupghome=self.gpghome,
-                                       passphrase='test',
-                                       reset_api_pwd=mon_api_reset_pwd)
+                                       passphrase='test')
 
         return test_info, reporter
 
     @patch('blocksatcli.util.prompt_for_enter')
     @patch('blocksatcli.monitoring.requests.post')
     def test_reporter_with_bs_monitoring_api(self, mock_api_post,
                                              mock_prompt_for_enter):
@@ -58,31 +57,34 @@
         """
         # Successfully respond to the password generation request
         mock_api_post.return_value.status_code = 200
         mock_api_post.return_value.json.return_value = {
             'new_password': 'generated-password'
         }
         _, reporter = self.configure_reporter_setup(mon_api_registered=True,
+                                                    bs_monitoring=True,
                                                     gen_gpg_key=True)
 
         reporter.send({'test': 'test'})
 
         # Given that the password was generated successfully, check if the
         # password is used for authentication:
-        mock_api_post.assert_called_with(metric_endpoint,
+        mock_api_post.assert_called_with("test_endpoint/metrics",
                                          json={
                                              'test': 'test',
                                              'uuid': 'test-uuid',
                                              'password': 'generated-password',
                                          },
-                                         cert=(None, None))
+                                         cert=(None, None),
+                                         timeout=5)
 
         # Error in the password generation process
         mock_api_post.return_value.status_code = 502
         _, reporter2 = self.configure_reporter_setup(mon_api_registered=True,
+                                                     bs_monitoring=True,
                                                      gen_gpg_key=True)
 
         reporter2.send({'test': 'test'})
 
         # The reporter should fall back to the GPG signature for authentication
         self.assertTrue('signature' in mock_api_post.call_args[1]['json'])
 
@@ -106,15 +108,16 @@
         mock_api_post.assert_called_with('http://custom.api.test',
                                          json={
                                              'test': 'test',
                                              'satellite':
                                              test_info['sat']['alias'],
                                              'hostname': 'hostname-test',
                                          },
-                                         cert=(None, None))
+                                         cert=(None, None),
+                                         timeout=5)
 
     @patch('blocksatcli.monitoring_api.BsMonitoring')
     @patch('blocksatcli.monitoring.requests.post')
     def test_reporter_with_receiver_not_registered(self, mock_api_post,
                                                    mock_bsmonitoring):
         """Test reporter with receiver not registered with the Monitoring API
 
@@ -127,15 +130,16 @@
         Also, while the receiver is not registered (i.e., while the initial
         registration process is not complete or if it has failed), the reporter
         functionality should remain disabled. In case of registration failure,
         every time reporter.send is called, the reporter prints a warning and
         does not report any metrics to the chosen destination.
 
         """
-        _, reporter = self.configure_reporter_setup(mon_api_registered=False)
+        _, reporter = self.configure_reporter_setup(mon_api_registered=False,
+                                                    bs_monitoring=True)
         self.assertIsNotNone(reporter.bs_monitoring)
 
         mock_bsmonitoring.return_value.registered = False
         mock_bsmonitoring.return_value.registration_failure = False
 
         reporter.send({'test': 'test', 'lock': False})
 
@@ -191,15 +195,17 @@
             'level': -50,
             'snr': 0,
             'ber': 1e-5,
             'quality': 100,
             'pkt_err': 0
         }
 
-    def configure_monitor_setup(self, only_receiver_config=False):
+    def configure_monitor_setup(self,
+                                only_receiver_config=False,
+                                report=False):
         """Configure monitor setup
 
         This function creates a test setup with a complete receiver
         configuration file, the GPG keys, and a monitoring.Monitor instance.
 
         """
         create_test_setup(cfg_name="test_config",
@@ -208,21 +214,22 @@
                           mon_api_registered=True,
                           gen_gpg_key=True)
 
         if only_receiver_config:
             return
 
         monitor = monitoring.Monitor(self.cfg_dir,
-                                     report=True,
+                                     report=report,
                                      echo=True,
                                      min_interval=0,
-                                     report_opts={
+                                     report_opts={} if not report else {
                                          'cfg': 'test_config',
                                          'cfg_dir': self.cfg_dir,
-                                         'dest_addr': metric_endpoint,
+                                         'dest_addr': 'http://test-server/',
+                                         'bs_monitoring': True,
                                          'gnupghome': self.gpghome,
                                          'passphrase': 'test'
                                      })
 
         return monitor
 
     def test_monitor_get_stats(self):
@@ -234,16 +241,18 @@
         self.assertEqual(res_with_units, self.stats)
 
         # Get stats without units
         res_without_units = monitor.get_stats(strip_unit=True)
         self.assertEqual(res_without_units, self.stats_without_units)
 
     @patch('blocksatcli.monitoring.Reporter.send')
-    def test_monitor_update_with_reporting_enabled(self, mock_send_report):
-        monitor = self.configure_monitor_setup()
+    @patch('requests.post')  # used at BsMonitoring.gen_api_password
+    def test_monitor_update_with_reporting_enabled(self, mock_post_req,
+                                                   mock_send_report):
+        monitor = self.configure_monitor_setup(report=True)
 
         monitor.update(self.stats)
         mock_send_report.assert_called_with(self.stats_without_units)
 
     @patch('time.strftime')
     def test_monitor_print_stats(self, mock_time):
         self.configure_monitor_setup(only_receiver_config=True)
@@ -357,11 +366,11 @@
         If reporting to Blockstream's Monitoring API, wait util the
         registration is complete to log the status to the console.
 
         """
         mock_bsmonitoring.return_value.registered = False
         mock_bsmonitoring.return_value.registration_running = True
 
-        monitor = self.configure_monitor_setup()
+        monitor = self.configure_monitor_setup(report=True)
         monitor.update({'lock': (True, None)})
 
         mock_print.assert_called_with()
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_monitoring_api.py` & `blocksat-cli-0.4.6/blocksatcli/test_monitoring_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from . import monitoring_api
 from . import config
 from .test_helpers import create_test_setup, TestEnv
 
 
 class TestMonitoringApi(TestEnv):
 
+    def setUp(self):
+        self.server_url = 'http://test-server'
+        super().setUp()
+
     @patch('blocksatcli.util.prompt_for_enter')
     @patch('blocksatcli.monitoring_api.requests.post')
     def test_request_and_reset_monitoring_api_password(self, mock_api_post,
                                                        mock_prompt_for_enter):
         # Create a configuration file with monitoring.registered=True and
         # monitoring.has_password=False.
         user_info = create_test_setup(self.cfg_name,
@@ -25,27 +29,29 @@
         # request a new password from the Monitoring API.
         mock_api_post.return_value.status_code = 200
         mock_api_post.return_value.json.return_value = {
             'new_password': 'password1'
         }
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase="test")
 
         # Check if the flag that indicates the password availability was set.
         self.assertTrue(monitor_api.user_info['monitoring']['has_password'])
 
         # Make sure the password is available in the monitoring object
         self.assertEqual(monitor_api.api_pwd, 'password1')
 
         # Test if the saved password can be loaded and decrypted correctly when
         # instantiating another BsMonitoring object
         monitor_api2 = monitoring_api.BsMonitoring(self.cfg_name,
                                                    self.cfg_dir,
+                                                   self.server_url,
                                                    self.gpghome,
                                                    passphrase="test")
         self.assertEqual(monitor_api2.api_pwd, 'password1')
 
     @patch('blocksatcli.monitoring_api.BsMonitoring._register')
     def test_save_credentials(self, mock_register):
         """Test saving receiver credentials in the configuration file
@@ -62,14 +68,15 @@
         # receiver is properly registered.
         self.assertFalse('monitoring' in user_info)
 
         # Since the receiver is not registered yet, the BsMonitoring handler
         # should run the registration function.
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase=None)
         self.assertTrue(mock_register.called)
 
         # The receiver credentials should be saved in the cfg file
         monitor_api._save_credentials('test-uuid', 'test-fingerprint')
         user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
@@ -94,20 +101,21 @@
         self.assertTrue('monitoring' in user_info)
 
         # The receiver is registered (i.e., the 'monitoring' key is in the
         # configuration file), so the BsMonitoring handler should run the setup
         # function for registered receivers. Check:
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase=None)
         self.assertTrue(mock_setup_registered.called)
 
         # Delete the receiver credentials from the configuration file
-        monitor_api._delete_credentials()
+        monitor_api.delete_credentials()
         user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertFalse('monitoring' in user_info)
 
     @patch('blocksatcli.monitoring_api.requests.post')
     @patch('blocksatcli.monitoring_api.BsMonitoring._setup_registered')
     def test_sign_request_with_gpg(self, mock_registered, mock_api_post):
         """Test sign requests with GPG
@@ -121,14 +129,15 @@
 
         # Since the non-GPG password is not defined yet, the BsMonitoring
         # constructor will try to configure one. Pretend this step fails so
         # that the subsequent reports are authenticated with the GPG mechanism.
         mock_api_post.return_value.status_code = 400
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase="test")
 
         # Test sign request with GPG method
         report = {"test": "test"}
         monitor_api.sign_request(report, password_allowed=False)
         self.assertTrue("uuid" in report)
@@ -142,14 +151,15 @@
                           self.gpghome,
                           mon_api_registered=True,
                           gen_gpg_key=True,
                           mon_api_gen_password=True)
 
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase="test")
 
         # Test sign request with password method
         report = {"test": "test"}
         monitor_api.sign_request(report, password_allowed=True)
         self.assertTrue("uuid" in report)
@@ -161,27 +171,34 @@
     def test_user_interaction_in_register_procedure(self,
                                                     mock_prompt_for_enter,
                                                     mock_user_input,
                                                     mock_register_thread):
         """Test user interaction in the register procedure
         """
         # Mock user input
-        mock_user_input.side_effect = ['y', 'City', 'State', 'Country', 'y']
+        mock_user_input.side_effect = [
+            'y',  # show explainer
+            'City',
+            'State',
+            'Country',
+            'y'  # confirm address
+        ]
 
         # Create a configuration file with an unregistered receiver
         create_test_setup(self.cfg_name,
                           self.cfg_dir,
                           self.gpghome,
                           mon_api_registered=False,
                           gen_gpg_key=True,
                           mon_api_has_password=False)
 
         # The monitoring api will launch the registration function
         monitoring_api.BsMonitoring(self.cfg_name,
                                     self.cfg_dir,
+                                    self.server_url,
                                     self.gpghome,
                                     passphrase="test")
 
         # Confirm the information sent to the register_thread function
         fingerprint = self.gpg.get_default_priv_key()['fingerprint']
         pubkey = self.gpg.gpg.export_keys(fingerprint)
         mock_register_thread.assert_called_with(
@@ -196,15 +213,15 @@
             # Rx Type
             'Selfsat IP22',
             # Antenna
             'Selfsat>IP22',
             # LNB
             'Selfsat Integrated LNB')
 
-    @patch('blocksatcli.monitoring_api.BsMonitoring._gen_api_password')
+    @patch('blocksatcli.monitoring_api.BsMonitoring.gen_api_password')
     @patch('blocksatcli.monitoring_api.requests.patch')
     @patch('blocksatcli.monitoring_api.queue.Queue')
     @patch('blocksatcli.monitoring_api.ApiListener')
     @patch('blocksatcli.monitoring_api.requests.post')
     @patch('blocksatcli.monitoring_api.BsMonitoring._register')
     def test_api_interaction_in_register_procedure(self, mock_register,
                                                    mock_api_post,
@@ -233,35 +250,36 @@
         mock_queue.return_value.get.return_value = b'validation-key'
         mock_api_patch.return_value.status_code = 200
 
         # For the initial registration, the BsMonitoring object calls the
         # _register_thread function on a thread.
         monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                   self.cfg_dir,
+                                                  self.server_url,
                                                   self.gpghome,
                                                   passphrase="test")
         monitor_api.rx_lock_event.set()
         monitor_api._register_thread(fingerprint, "pubkey", "address",
                                      "satellite", "rx_type", "antenna", "lnb")
 
         # Check the arguments sent to API via post method to sign-up to
         # the monitoring server
-        mock_api_post.assert_called_with(monitoring_api.account_endpoint,
+        mock_api_post.assert_called_with(self.server_url + '/accounts',
                                          json={
                                              'fingerprint': fingerprint,
                                              'publickey': 'pubkey',
                                              'city': 'address',
                                              'satellite': 'satellite',
                                              'receiver_type': 'rx_type',
                                              'antenna': 'antenna',
                                              'lnb': 'lnb'
                                          })
 
         # Check arguments sent to the API via patch method
-        mock_api_patch.assert_called_with(monitoring_api.account_endpoint,
+        mock_api_patch.assert_called_with(self.server_url + '/accounts',
                                           json={
                                               'uuid': 'test-uuid',
                                               'validation_key':
                                               'validation-key'
                                           })
 
         # After the 2FA procedure is done, the _register_thread function
@@ -297,14 +315,15 @@
         self.gpghome = "/tmp/"
 
         # Assert logger error if key is not found in the local keyring
         with self.assertLogs(monitoring_api.logger, level='ERROR'):
             mock_yes_or_no.return_value = 'y'  # Reset credentials
             monitoring_api.BsMonitoring(self.cfg_name,
                                         self.cfg_dir,
+                                        self.server_url,
                                         self.gpghome,
                                         passphrase="test")
 
         # Make sure that the old credentials were deleted and a new
         # registration was initiated by calling the _register function:
         user_info = config.read_cfg_file(self.cfg_name, self.cfg_dir)
         self.assertFalse('monitoring' in user_info)
@@ -331,14 +350,15 @@
         # Set status code different than 200
         mock_api_post.return_value.status_code = 502
 
         # Assert logger error
         with self.assertLogs(monitoring_api.logger, level='ERROR'):
             monitor_api = monitoring_api.BsMonitoring(self.cfg_name,
                                                       self.cfg_dir,
+                                                      self.server_url,
                                                       self.gpghome,
                                                       passphrase="test")
             monitor_api.rx_lock_event.set()
             monitor_api._register_thread(fingerprint, "pubkey", "address",
                                          "satellite", "rx_type", "antenna",
                                          "lnb")
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_satip.py` & `blocksat-cli-0.4.6/blocksatcli/test_satip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,35 @@
+import os
+import zipfile
+from pathlib import Path
 from unittest import TestCase
 from unittest.mock import patch
+from urllib.error import URLError
 
 from .upnp import SSDPDevice
 from . import satip
 
 
 def _gen_ssdp_dev(addr, friendly_name):
     resp = ('HTTP/1.1 200 OK\r\n'
             'LOCATION: http://{}:8000/description.xml\r\n'
             'BOOTID.UPNP.ORG: 24\r\n').format(addr[0])
     ssdp_dev = SSDPDevice(addr, resp)
     ssdp_dev.friendly_name = friendly_name
     return ssdp_dev
 
 
+def _mock_fw_upgrade(url, local_path, progress_callback):
+    # Create a mock upgrade file
+    with zipfile.ZipFile(local_path, 'w') as zip_ref:
+        supg_file = os.path.join(os.path.dirname(local_path), 'upgrade.supg')
+        Path(supg_file).touch()
+        zip_ref.write(supg_file)
+
+
 class MockResponse():
     """Mock requests response"""
 
     def __init__(self, text="", json={}):
         self.text = text
         self._json = json
 
@@ -26,55 +38,61 @@
 
     def json(self):
         return self._json
 
 
 class TestApi(TestCase):
 
+    @patch('urllib.request.urlopen')
     @patch('blocksatcli.util.ask_multiple_choice')
     @patch('blocksatcli.upnp.UPnP.discover')
-    def test_discover(self, mock_upnp_discover, mock_ask_multi_choice):
+    def test_discover(self, mock_upnp_discover, mock_ask_multi_choice,
+                      mock_urllib_urlopen):
         """Test Sat-IP device discovery"""
+        # Raise a mocked URLError instead of trying to open the URL to get the
+        # description from the faked devices.
+        mock_urllib_urlopen.side_effect = URLError('mocked method')
+
         addr1 = ('192.168.9.50', 33783)
         addr2 = ('192.168.9.51', 33781)
         wrong_ssdp_dev = _gen_ssdp_dev(addr1, 'Test-Dev')
         satip_ssdp_dev1 = _gen_ssdp_dev(addr1, 'SELFSAT-IP')
         satip_ssdp_dev2 = _gen_ssdp_dev(addr2, 'SELFSAT-IP')
 
         # UPnP does not discover any device
         mock_upnp_discover.return_value = []
         sat_ip = satip.SatIp()
-        sat_ip.discover()
+        sat_ip.select_receiver()
         self.assertIsNone(sat_ip.host)
 
         # UPnP discovers a device, but not the Sat-IP receiver
         mock_upnp_discover.return_value = [wrong_ssdp_dev]
         sat_ip = satip.SatIp()
-        sat_ip.discover()
+        sat_ip.select_receiver()
         self.assertIsNone(sat_ip.host)
 
         # UPnP discovers the Sat-IP receiver
         mock_upnp_discover.return_value = [satip_ssdp_dev1]
         sat_ip = satip.SatIp()
-        sat_ip.discover()
+        sat_ip.select_receiver()
         self.assertEqual(sat_ip.host, addr1[0])
 
         # UPnP discovers multiple Sat-IP receivers in non-interactive mode
         mock_upnp_discover.return_value = [satip_ssdp_dev1, satip_ssdp_dev2]
         sat_ip = satip.SatIp()
-        sat_ip.discover(interactive=False)
+        sat_ip.select_receiver(interactive=False)
         self.assertEqual(sat_ip.host, addr1[0])
 
         # UPnP discovers multiple Sat-IP receivers in interactive mode
         mock_ask_multi_choice.return_value = {
             'host': satip_ssdp_dev2.host,
             'base_url': satip_ssdp_dev2.base_url
         }
         sat_ip = satip.SatIp()
-        sat_ip.discover(interactive=True)
+        sat_ip.select_receiver(interactive=True)
         self.assertEqual(sat_ip.host, addr2[0])
 
     @patch('requests.get')
     def test_fw_check(self, mock_get):
         """Test Sat-IP firmware validation"""
 
         # Old firmware version that does not satisfy the minimum
@@ -86,25 +104,27 @@
         # Recent firmware version satisfying the minimum
         mock_get.return_value = MockResponse("3.1.18")
         sat_ip = satip.SatIp()
         sat_ip.set_server_addr("192.168.100.2")
         self.assertTrue(sat_ip.check_fw_version())
 
     @patch('requests.post')
-    def test_fw_upgrade(self, mock_post):
+    @patch('blocksatcli.util.urlretrieve')
+    def test_fw_upgrade(self, mock_urlretrieve, mock_post):
         """Test Sat-IP firmware upgrade"""
         mock_post.return_value = MockResponse(
             json={
                 'status': "0",
                 'thisver': {
                     'sw_ver': "2.2.19"
                 },
                 'newver': {
                     'sw_ver': "3.1.18"
                 }
             })
+        mock_urlretrieve.side_effect = _mock_fw_upgrade
         sat_ip = satip.SatIp()
         sat_ip.set_server_addr("192.168.100.2")
         fw_upgrade_ok = sat_ip.upgrade_fw("/tmp/",
                                           interactive=False,
                                           no_wait=True)
         self.assertTrue(fw_upgrade_ok)
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_tsp.py` & `blocksat-cli-0.4.6/blocksatcli/test_tsp.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_update.py` & `blocksat-cli-0.4.6/blocksatcli/test_update.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/test_util.py` & `blocksat-cli-0.4.6/blocksatcli/test_util.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/tsp.py` & `blocksat-cli-0.4.6/blocksatcli/tsp.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/update.py` & `blocksat-cli-0.4.6/blocksatcli/update.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/upnp.py` & `blocksat-cli-0.4.6/blocksatcli/upnp.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/usb.py` & `blocksat-cli-0.4.6/blocksatcli/usb.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,16 +42,24 @@
         if (info['lnb']['pol'].lower() == "dual" and  # user has dual-pol LNB
             (
                 info['sat']['pol'] == "H" or  # and satellite requires H pol
                 (
                     'v1_pointed' in info['lnb'] and info['lnb']['v1_pointed']
                     and info['lnb']['v1_psu_voltage'] >=
                     16  # or LNB already operates with H pol
-                )) and "rangeswitch"
-                not in lnb):  # but LNB candidate is single-pol
+                )) and
+                "rangeswitch" not in lnb  # but LNB candidate is single-pol
+                and info['sat']['band'] != "C"):  # and not C band (see below)
+            # NOTE: the above condition should apply to C band just like it
+            # applies to Ku band. If the LNB needs 18V to operate in H pol, the
+            # v4l LNB definition should have a "rangeswitch" property. However,
+            # the problem is that there are only two C-band LNB definitions in
+            # v4l-utils, and neither of them has a "rangeswitch" property.
+            # Hence, as a temporary workaround, ignore the polarization setting
+            # for the C-band LNB and return the first match.
             continue  # not a validate candidate, skip
 
         if (target_is_universal):
             if (is_universal_option and lnb['lowfreq'] == target_lo_freq[0]
                     and lnb['highfreq'] == target_lo_freq[1]):
                 options.append(lnb)
         else:
@@ -60,23 +68,21 @@
 
     assert (len(options) > 0), "LNB doesn't match a valid option"
     logger.debug("Matching LNB options: {}".format(pformat(options)))
 
     return options[0]
 
 
-def _find_adapter(list_only=False, target_model=None):
+def find_adapters():
     """Find the DVB adapter
 
     Returns:
-        Tuple with (adapter index, frontend index)
+        List of dictionaries with DVB adapter information
 
     """
-    if (target_model is None):
-        util.print_header("Find DVB Adapter")
 
     # Search a range of adapters. There is no command to list all adapters, so
     # we try to list each one individually using `dvbnet -a adapter_no -l`.
     adapters = list()
     for a in range(0, 10):
         cmd = ["dvbnet", "-a", str(a), "-l"]
         logger.debug("> " + " ".join(cmd))
@@ -159,26 +165,42 @@
     dvb_s2_adapters = [a for a in adapters if ("DVB-S/S2" in a["support"])]
     logger.debug(dvb_s2_adapters)
 
     if (len(dvb_s2_adapters) == 0):
         logger.error("No DVB-S2 adapters found")
         sys.exit(1)
 
+    return dvb_s2_adapters
+
+
+def _select_adapter(list_only=False, target_model=None):
+    """Select DVB-S2 adapter
+
+    Returns:
+        Tuple with (adapter index, frontend index)
+
+    """
+
+    if (target_model is None):
+        logger.info("Find DVB adapter")
+
+    dvb_s2_adapters = find_adapters()
+
     chosen_adapter = None
     if (target_model is not None):
         # Search without prompting
         for adapter in dvb_s2_adapters:
             if (adapter["model"] == target_model):
                 chosen_adapter = adapter
                 break
     else:
         # Prompt the user
         for adapter in dvb_s2_adapters:
-            print("Found DVB-S2 adapter: %s %s" %
-                  (adapter["vendor"], adapter["model"]))
+            logger.info("Found DVB-S2 adapter: %s %s" %
+                        (adapter["vendor"], adapter["model"]))
 
             if (not list_only):
                 if (len(dvb_s2_adapters) == 1
                         or util.ask_yes_or_no("Choose adapter?")):
                     chosen_adapter = adapter
                     logger.debug("Chosen adapter:")
                     logger.debug(pformat(adapter))
@@ -193,89 +215,103 @@
         else:
             err_msg = "Please choose a valid DVB-S2 adapter"
         raise ValueError(err_msg)
 
     return chosen_adapter["adapter"], chosen_adapter["frontend"]
 
 
-def _dvbnet_single(adapter, ifname, pid, ule, existing_dvbnet_interfaces):
-    """Start DVB network interface
+def _dvbnet_verify_single(ifname, pid, ule, existing_dvbnet_interfaces):
+    """Check if a single DVB network interface is already created
 
     Args:
-        adapter                    : DVB adapter index
         ifname                     : DVB network interface name
         pid                        : PID to listen to
         ule                        : Whether to use ULE framing
         existing_dvbnet_interfaces : List of dvbnet interfaces already
                                      configured for the adapter
 
-    """
+    Returns:
+        if_exists (bool): Whether the interface exists.
+        is_config (bool): Whether the interface is already configured.
 
-    assert (pid >= 32 and pid <= 8190), "PID not insider range 32 to 8190"
+    """
+    assert (pid >= 32 and pid <= 8190), "PID not inside range 32 to 8190"
 
     if (ule):
         encapsulation = 'ULE'
     else:
         encapsulation = 'MPE'
 
     # Check if the interface already exists
     res = subprocess.call(["ip", "addr", "show", "dev", ifname],
                           stdout=subprocess.DEVNULL,
                           stderr=subprocess.DEVNULL)
     os_interface_exists = (res == 0)
-    matching_dvbnet_if = None
 
     # When the network interface exists in the OS, we also need to check if the
-    # matching dvbnet device is configured according to what we want now
+    # matching dvbnet device is configured according to what we want
+    matching_dvbnet_if = None
     if (os_interface_exists):
-        print("Network interface %s already exists" % (ifname))
+        logger.info(f"Network interface {ifname} already exists.")
 
         for interface in existing_dvbnet_interfaces:
             if (interface['name'] == ifname):
                 matching_dvbnet_if = interface
                 break
 
-    # Our indication that interface exists comes from "ip addr show
-    # dev". However, it is possible that dvbnet does not have any interface
+    # If there is a match, it indicates that the interface exists.
+    if_exists = matching_dvbnet_if is not None
+
+    # Our indication that interface exists comes from "ip addr show dev".
+    # However, it is possible that dvbnet does not have any interface
     # associated to an adapter, so check if we found anything:
-    cfg_interface = False
+    is_config = False
     if (len(existing_dvbnet_interfaces) > 0
             and matching_dvbnet_if is not None):
         # Compare to desired configurations
-        if (matching_dvbnet_if['pid'] != pid
-                or matching_dvbnet_if['encapsulation'] != encapsulation):
-            cfg_interface = True
+        if (matching_dvbnet_if['pid'] == pid
+                and matching_dvbnet_if['encapsulation'] == encapsulation):
+            is_config = True
 
         if (matching_dvbnet_if['pid'] != pid):
             print("Current PID is %d. Set it to %d" %
                   (matching_dvbnet_if['pid'], pid))
 
         if (matching_dvbnet_if['encapsulation'] != encapsulation):
             print("Current encapsulation is %s. Set it to %s" %
                   (matching_dvbnet_if['encapsulation'], encapsulation))
-    else:
-        cfg_interface = True
 
-    # Create interface in case it doesn't exist or needs to be re-created
-    if (cfg_interface):
+    return if_exists, is_config
+
+
+def _dvbnet_single(adapter, ifname, pid, ule, remove=False):
+    """Create DVB network interface
+
+    Args:
+        adapter : DVB adapter index
+        ifname  : DVB network interface name
+        pid     : PID to listen to
+        ule     : Whether to use ULE framing
+        remove  : Whether to remove already created DVB network interface.
+
+    """
+
+    assert (pid >= 32 and pid <= 8190), "PID not insider range 32 to 8190"
+
+    if (remove):
         # If interface exists, but must be re-created, remove the existing one
         # first
-        if (os_interface_exists):
-            _rm_dvbnet_interface(adapter, ifname, verbose=False)
+        _rm_dvbnet_interface(adapter, ifname, verbose=False)
 
-        ule_arg = "-U" if ule else ""
+    ule_arg = "-U" if ule else ""
 
-        if (runner.dry):
-            print("Create interface {}:".format(ifname))
+    if (runner.dry):
+        print("Create interface {}:".format(ifname))
 
-        runner.run(["dvbnet", "-a", adapter, "-p",
-                    str(pid), ule_arg],
-                   root=True)
-    else:
-        print("Network interface %s already configured correctly" % (ifname))
+    runner.run(["dvbnet", "-a", adapter, "-p", str(pid), ule_arg], root=True)
 
 
 def _dvbnet(adapter, ifnames, pids, ule=False):
     """Start DVB network interfaces of a DVB adapter
 
     An adapter can have multiple dvbnet interfaces, one for each PID.
 
@@ -290,18 +326,47 @@
     assert (isinstance(pids, list))
     assert (len(ifnames) == len(pids)), \
         "Interface names and PID number must be vectors of the same length"
 
     # Find the dvbnet interfaces that already exist for the chosen adapter
     existing_dvbnet_iif = _find_dvbnet_interfaces(adapter)
 
-    util.print_header("Network Interface")
+    for ifname, pid in zip(ifnames, pids):
+        if_exists, is_config = _dvbnet_verify_single(ifname, pid, ule,
+                                                     existing_dvbnet_iif)
 
+        if is_config:
+            # If interface is already configured, move to the next.
+            print("Network interface %s already configured correctly" %
+                  (ifname))
+            continue
+
+        _dvbnet_single(adapter, ifname, pid, ule, remove=if_exists)
+
+
+def _verify_dvbnet(adapter, ifnames, pids, ule=False):
+    """Check if all DVB interfaces are configured"""
+    assert (isinstance(ifnames, list))
+    assert (isinstance(pids, list))
+    assert (len(ifnames) == len(pids)), \
+        "Interface names and PID number must be vectors of the same length"
+
+    # Find the dvbnet interfaces that already exist for the chosen adapter
+    existing_dvbnet_iif = _find_dvbnet_interfaces(adapter)
+
+    all_config_iff = []
     for ifname, pid in zip(ifnames, pids):
-        _dvbnet_single(adapter, ifname, pid, ule, existing_dvbnet_iif)
+        _, is_config = _dvbnet_verify_single(ifname, pid, ule,
+                                             existing_dvbnet_iif)
+        all_config_iff.append(is_config)
+
+        if is_config:
+            logger.info(f"DVB interfaces {ifname} already configured.")
+
+    return all(all_config_iff)
 
 
 def _find_dvbnet_interfaces(adapter):
     """Find dvbnet interface(s) of a DVB adapter
 
     An adapter can have multiple dvbnet interfaces, one for each PID.
 
@@ -309,15 +374,14 @@
         adapter: Corresponding DVB adapter
 
     Returns:
         interfaces : List of dvbnet interfaces
 
     """
 
-    util.print_header("Find dvbnet interface(s)")
     cmd = ["dvbnet", "-a", adapter, "-l"]
     logger.debug("> " + " ".join(cmd))
     res = subprocess.check_output(cmd)
 
     interfaces = list()
     for line in res.splitlines():
         if ("Found device" in line.decode()):
@@ -342,22 +406,22 @@
 
     Args:
         adapter   : Corresponding DVB adapter
         interface : dvbnet interface number
         verbose   : Controls verbosity
     """
 
-    if (verbose):
-        util.print_header("Remove dvbnet interface")
-
     runner.run(["ip", "link", "set", ifname, "down"], root=True)
 
     if_number = ifname.split("_")[-1]
     runner.run(["dvbnet", "-a", adapter, "-d", if_number], root=True)
 
+    if (verbose):
+        logger.info(f"DVB interface {ifname} was removed.")
+
     # Remove also the static IP address configuration
     ip.rm_ip(ifname, runner.dry)
 
 
 def zap(adapter,
         frontend,
         ch_conf_file,
@@ -511,14 +575,20 @@
     p1.add_argument('-m',
                     '--monitor',
                     default=False,
                     action='store_true',
                     help='Launch dvbv5-zap in monitor mode to debug MPEG TS '
                     'packet and bit rates')
 
+    p1.add_argument('-y',
+                    '--yes',
+                    default=False,
+                    action='store_true',
+                    help="Defaults to answering Yes to prompts")
+
     monitoring.add_to_parser(p1)
 
     p1.set_defaults(func=launch)
 
     # Initial configurations
     p2 = subsubparsers.add_parser(
         'config',
@@ -563,15 +633,15 @@
                     help="Default to answering Yes to configuration prompts")
 
     p2.add_argument("--dry-run",
                     action='store_true',
                     default=False,
                     help="Print all commands but do not execute them")
 
-    p2.set_defaults(func=usb_config)
+    p2.set_defaults(func=configure)
 
     # Find adapter sub-command
     p3 = subsubparsers.add_parser(
         'list',
         aliases=['ls'],
         description="List DVB-S2 adapters",
         help='List DVB-S2 adapters',
@@ -611,57 +681,81 @@
 
     # Check if dvbnet is available before trying to find the adapter
     if (not dependencies.check_apps(["dvbnet", "dvb-fe-tool"])):
         return
 
     # Find adapter
     if (args.adapter is None):
-        adapter, frontend = _find_adapter()
+        adapter, frontend = _select_adapter()
     else:
         if (args.adapter.isdigit()):
             # Assume argument --adapter has the adapter number. In this case,
             # --frontend is also required.
             if (args.frontend is None):
                 raise ValueError("argument --adapter requires --frontend.")
             adapter = args.adapter
             frontend = args.frontend
         else:
             # Assume argument --adapter has the target model
-            adapter, frontend = _find_adapter(target_model=args.adapter)
+            adapter, frontend = _select_adapter(target_model=args.adapter)
 
     # Cache the adapter number on the local config file so that other modules
     # can read the adapter number directly. Rewrite the info every time, as the
     # adapter number could change between boots.
     user_info['setup']['adapter'] = adapter
     config.write_cfg_file(args.cfg, args.cfg_dir, user_info)
 
     return user_info, adapter, frontend
 
 
-def usb_config(args):
-    """Config the DVB interface(s) and the host"""
+def verify(args) -> dict:
+    """Verify configuration from the DVB interface(s) and the host
+
+    Returns:
+        dict: Dictionary indicating which components (package dependencies,
+            dvbnet interface, RP filters, firewall, or IPs) still need
+            configuration.
+    """
+    res = {
+        'config': {
+            'deps': False,
+            'dvb': False,
+            'rp': args.skip_rp,  # assume OK when skipping
+            'firewall': args.skip_firewall,  # assume OK when skipping
+            'ips': False
+        },
+        'user_info': None,
+        'adapter': None,
+        'frontend': None
+    }
+
+    logger.info("Checking current configuration")
     common_params = _common(args)
     if (common_params is None):
-        return
+        logger.error("Receiver configuration not found.")
+        sys.exit(1)
     user_info, adapter, frontend = common_params
+    res['user_info'] = user_info
+    res['adapter'] = adapter
+    res['frontend'] = frontend
 
     # Check if dependencies other than dvbnet are installed
     apps = ["ip"]
     if not args.skip_firewall:
         apps.append("iptables")
-    if (not dependencies.check_apps(apps)):
-        return
+    res['config']['deps'] = dependencies.check_apps(apps)
 
     # Configure the subprocess runner
     runner.set_dry(args.dry_run)
 
     # Confirm the drivers are installed
     if not args.dry_run and not dependencies.check_drivers(
             user_info['setup']['model']):
-        return
+        logger.error(f"{user_info['setup']['model']} drivers not found.")
+        sys.exit(1)
 
     if args.ip is None:
         ips = ip.compute_rx_ips(user_info['sat']['ip'], len(args.pid))
     else:
         ips = args.ip
 
     assert (all(["/" in x
@@ -676,31 +770,87 @@
     # different IP address.
     net_ifs = list()
     for i_device in range(0, len(args.pid)):
         # Define interface name that is going to be generated by dvbnet
         net_if = "dvb" + adapter + "_" + str(i_device)
         net_ifs.append(net_if)
 
+    # Check the dvbnet interface(s)
+    res['config']['dvb'] = _verify_dvbnet(adapter,
+                                          net_ifs,
+                                          args.pid,
+                                          ule=args.ule)
+
+    # Check RP filters
+    if (not args.skip_rp):
+        res['config']['rp'] = rp.verify(net_ifs)
+        if not res['config']['rp']:
+            logger.info("RP filters not configured.")
+
+    # Check firewall rules
+    if (not args.skip_firewall):
+        res['config']['firewall'] = firewall.verify(net_ifs, defs.src_ports,
+                                                    user_info['sat']['ip'])
+        if not res['config']['firewall']:
+            logger.info("Firewall rules not configured.")
+
+    # Check IP
+    res['config']['ips'] = ip.check_ips(net_ifs, ips)
+
+    return res
+
+
+def configure(args):
+    """Config the DVB interface(s) and the host"""
+
+    verify_res = verify(args)
+    if all(verify_res['config'].values()):
+        logger.info("Receiver already configured")
+        return
+
+    user_info = verify_res['user_info']
+    adapter = verify_res['adapter']
+
+    # Configure the subprocess runner
+    runner.set_dry(args.dry_run)
+
+    if args.ip is None:
+        ips = ip.compute_rx_ips(user_info['sat']['ip'], len(args.pid))
+    else:
+        ips = args.ip
+
+    # dvbnet interfaces of interest
+    #
+    # NOTE: there is one dvbnet interface per PID. Each interface will have a
+    # different IP address.
+    net_ifs = list()
+    for i_device in range(0, len(args.pid)):
+        # Define interface name that is going to be generated by dvbnet
+        net_if = "dvb" + adapter + "_" + str(i_device)
+        net_ifs.append(net_if)
+
     # Create the dvbnet interface(s)
-    _dvbnet(adapter, net_ifs, args.pid, ule=args.ule)
+    if not verify_res['config']['dvb']:
+        _dvbnet(adapter, net_ifs, args.pid, ule=args.ule)
 
     # Set RP filters
-    if (not args.skip_rp):
-        rp.set_filters(net_ifs, prompt=(not args.yes), dry=args.dry_run)
+    if not verify_res['config']['rp']:
+        rp.configure(net_ifs, prompt=(not args.yes), dry=args.dry_run)
 
     # Set firewall rules
-    if (not args.skip_firewall):
+    if not verify_res['config']['firewall']:
         firewall.configure(net_ifs,
                            defs.src_ports,
                            user_info['sat']['ip'],
                            prompt=(not args.yes),
                            dry=args.dry_run)
 
     # Set IP
-    ip.set_ips(net_ifs, ips, dry=runner.dry)
+    if not verify_res['config']['ips']:
+        ip.set_ips(net_ifs, ips, dry=runner.dry)
 
     util.print_header("Next Step")
     print("Run:\n\nblocksat-cli usb launch\n")
 
     return
 
 
@@ -734,14 +884,17 @@
     d['lock'] = ("Lock" in line, None)
     for i, elem in enumerate(elements):
         # Each metric is printed as "name=value"
         if (elem[-1] == "=" and (i + 1) <= n_elem):
             key = elem[:-1]
             raw_value = elements[i + 1]
 
+            if key not in log_key_map:
+                continue  # unexpected key
+
             # Convert key to the nomenclature adopted on monitor.py
             key = log_key_map[key]
 
             # Fix any scientific notation
             if ("^" in raw_value):
                 raw_value = raw_value.replace("x10^", "e")
 
@@ -803,20 +956,27 @@
 
     # Check conflicting logging options
     if ((args.monitor or args.record_file)
             and (args.log_scrolling or args.log_file)):
         raise ValueError("Logging options are disabled when running with "
                          "-m/--monitor or -r/--record-file")
 
+    # Check if the channels.conf file is up-to-date
+    chan_conf = user_info['setup']['channel']
+    if not config.verify_chan_conf(user_info):
+        logger.info('Channel configuration at {} is invalid'.format(chan_conf))
+        config.write_chan_conf(user_info,
+                               chan_conf,
+                               yes=args.yes,
+                               regeneration=True)
+        print()
+
     if monitor is None:
         monitor = _get_monitor(args)
 
-    # Channel configuration file
-    chan_conf = user_info['setup']['channel']
-
     # Zap
     zap_ps = zap(adapter,
                  frontend,
                  chan_conf,
                  user_info,
                  lnb=args.lnb,
                  output=args.record_file,
@@ -854,15 +1014,15 @@
 
     Handles the find-adapter subcommand
 
     """
     if (not dependencies.check_apps(["dvbnet", "dvb-fe-tool"])):
         return
 
-    _find_adapter(list_only=True)
+    _select_adapter(list_only=True)
 
 
 def rm_subcommand(args):
     """Remove DVB interface
 
     """
 
@@ -870,20 +1030,20 @@
         return
 
     # Configure the subprocess runner
     runner.set_dry(args.dry_run)
 
     # Find adapter
     if (args.adapter is None):
-        adapter, _ = _find_adapter()
+        adapter, _ = _select_adapter()
     else:
         # If argument --adapter holds a digit-only string, assume it refers to
         # the adapter number. Otherwise, assume it refers to the target model.
         adapter = args.adapter if args.adapter.isdigit() else \
-            _find_adapter(target_model=args.adapter)[0]
+            _select_adapter(target_model=args.adapter)[0]
 
     interfaces = _find_dvbnet_interfaces(adapter)
     chosen_devices = list()
 
     if (len(interfaces) > 1):
         if (args.all):
             for interface in interfaces:
```

### Comparing `blocksat-cli-0.4.5/blocksatcli/util.py` & `blocksat-cli-0.4.6/blocksatcli/util.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/blocksatcli/verify_deps_instal.py` & `blocksat-cli-0.4.6/blocksatcli/verify_deps_instal.py`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/README.md` & `blocksat-cli-0.4.6/doc/README.md`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/antenna-pointing.md` & `blocksat-cli-0.4.6/doc/antenna-pointing.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 # Antenna Pointing
 
 Aligning a satellite antenna is a precise procedure. Remember that the satellites are over 35,000 km (22,000 mi) away. A tenth of a degree of error will miss the satellite by more than 3500 km. Hence, this is likely the most time-consuming step of the process. This page provides a step-by-step guide for antenna alignment.
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
 **Table of Contents**
 
-- [Antenna Pointing](#antenna-pointing)
-    - [Mount the Antenna](#mount-the-antenna)
-    - [Find the Satellite and Lock the Signal](#find-the-satellite-and-lock-the-signal)
-    - [Optimize the SNR](#optimize-the-snr)
-    - [Next Steps](#next-steps)
-    - [Further Information](#further-information)
-        - [Novra S400's User Interface](#novra-s400s-user-interface)
-        - [Pointing with an SDR-based Receiver](#pointing-with-an-sdr-based-receiver)
-        - [Pointing with a Satellite Finder](#pointing-with-a-satellite-finder)
+- [Mount the Antenna](#mount-the-antenna)
+- [Find the Satellite and Lock the Signal](#find-the-satellite-and-lock-the-signal)
+- [Optimize the SNR](#optimize-the-snr)
+- [Next Steps](#next-steps)
+- [Further Information](#further-information)
+  - [Novra S400's User Interface](#novra-s400s-user-interface)
+  - [Pointing with an SDR-based Receiver](#pointing-with-an-sdr-based-receiver)
+  - [Pointing with a Satellite Finder](#pointing-with-a-satellite-finder)
 
 <!-- markdown-toc end -->
 
 ## Mount the Antenna
 
 First, you should obtain the pointing angles required for your specific location using our [dish alignment tool](https://blockstream.com/satellite/#satellite_network-coverage).
 
@@ -33,17 +32,17 @@
 
 - **Elevation**: the up and down adjustment of your antenna. The antenna aiming tool provides the number of degrees above the horizon to which your antenna must point. 0 degrees represents pointing at the horizon, and 90 degrees is pointing straight up.
 
 - **Polarity**: determines the rotation of the LNB. It is the angle of the LNB within the LNB mounting bracket (or holder). Often this is referred to also as the LNB *polarization angle* or *LNB skew*. A positive angle means a clockwise adjustment when looking at the LNB from behind the dish and facing forwards to the satellite in the sky.
 
 The three angles are illustrated below:
 
-|                    Azimuth                     |                      Elevation                       |                         Polarity                          |
-| :--------------------------------------------: | :--------------------------------------------------: | :-------------------------------------------------------: |
-| ![Azimuth](img/azimuth.png?raw=true "Azimuth") | ![Elevation](img/elevation.png?raw=true "Elevation") | ![Polarity](img/lnb_polarization.png?raw=true "Polarity") |
+|                Azimuth                |                  Elevation                  |                     Polarity                     |
+| :-----------------------------------: | :-----------------------------------------: | :----------------------------------------------: |
+| ![Azimuth](img/azimuth.png "Azimuth") | ![Elevation](img/elevation.png "Elevation") | ![Polarity](img/lnb_polarization.png "Polarity") |
 
 Next, visually inspect the direction to which your antenna must point. Use a compass or smartphone app (e.g., Satellite Pointer for [Android](https://play.google.com/store/apps/details?id=com.tda.satpointer) and [iOS](https://apps.apple.com/br/app/satellite-pointer/id994565490)) to identify it. Ensure that there are no obstacles (like trees or buildings) between your antenna and the target area in the sky. You must have a clear line of sight to that area of the sky.
 
 **IMPORTANT:** If using a compass app on a smartphone, make sure to configure the app to display **true north** instead of the **magnetic north**. The azimuth angle provided by our dish alignment tool refers to true north. Also, if using an ordinary compass or a compass-based satellite finder, make sure to convert the true azimuth obtained from the dish alignment tool into the magnetic azimuth. You can get both the true and magnetic azimuth angles using a tool such as the [Dish Pointer app](https://www.dishpointer.com).
 
 Next, install the satellite antenna according to the directions accompanying it, or have it done professionally. If you install it yourself, proceed with the following steps:
 
@@ -306,15 +305,15 @@
 
 2. If the measured signal level is not 99%, it means the signal received by the finder is not as strong as anticipated. Hence, reduce the attenuation to observe weaker signals. That is, press the right ATT button until you get to a 99% level. Keep the dial on the side at its maximum throughout this process so that you can adjust the attenuation setting first.
 
 3. Once the finder measures 99% signal level, turn the side dial down (reduce the gain) until you get a reasonably low signal level on the finder's display. For example, try achieving a level between 5% and 30%.
 
 At this point, you should be ready to start the antenna alignment process. Make sure to keep an eye on the receiver's lock status (refer to the [lock status instructions](#find-the-satellite-and-lock-the-signal)) throughout the process and continue with the following steps:
 
-1. Adjust the antenna roughly in the right direction based on the azimuth, elevation, and polarity angles obtained from the [website](https://blockstream.com/satellite/#satellite_network-coverage).
+1. Adjust the antenna roughly in the right direction based on the azimuth, elevation, and polarity angles obtained from the [Coverage Map](https://blockstream.com/satellite/#satellite_network-coverage).
 2. Choose a coordinate to optimize (azimuth, elevation, or polarity) and focus on it. For example, start by optimizing the azimuth.
 3. Make subtle adjustments to the chosen coordinate until you can observe an increase in the signal level measured by the finder.
 4. If the level increases too much and reaches 99%, turn the side dial (gain) down slightly such that the measured signal strength comes back to a low value. If the side dial reaches its minimum and the measured level remains at 99%, it means the signal is now too strong to be measured. Increase the attenuation by pressing the left ATT button once and readjust the side dial to get the measured level back at a low value.
 5. Go back to step 3 and repeat the process until you can no longer observe improvements on the measured level for the chosen coordinate.
 6. Go back to step 2 and pick the next coordinate to be optimized.
 
 If the receiver logs `Lock = True` on the console at any point, it means you are in the right direction. Otherwise, if you have optimized all coordinates using the above procedure and the receiver still logs `Lock = False`, you may have pointed to the wrong satellite. In this case, inspect the final alignment and repeat the process if necessary.
```

### Comparing `blocksat-cli-0.4.5/doc/api.md` & `blocksat-cli-0.4.6/doc/api.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,35 @@
 > The API support on the CLI is available starting from version `0.3.0`. Please refer to instructions regarding how to [check and upgrade your CLI version](quick-reference.md#cli-installation-and-upgrade).
 
 For details regarding the RESTful API, please refer to the [Satellite API's repository](https://github.com/Blockstream/satellite-api).
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Satellite API](#satellite-api)
-    - [Encryption Keys](#encryption-keys)
-    - [Satellite API Transmission](#satellite-api-transmission)
-        - [Choosing the Recipient](#choosing-the-recipient)
-        - [Signing the Messages](#signing-the-messages)
-    - [Satellite API Reception](#satellite-api-reception)
-        - [Choosing the Sender](#choosing-the-sender)
-    - [Demo Receiver](#demo-receiver)
-    - [Further Information](#further-information)
-        - [Lightning Wallets](#lightning-wallets)
-        - [Plaintext Mode](#plaintext-mode)
-        - [Receiving Messages Sent from the Browser](#receiving-messages-sent-from-the-browser)
-        - [Reliable Transmissions](#reliable-transmissions)
-        - [Transmission over Selected Regions](#transmission-over-selected-regions)
-        - [Running on Testnet](#running-on-testnet)
-        - [Bump and Delete API orders](#bump-and-delete-api-orders)
-        - [Password-protected GPG keyring](#password-protected-gpg-keyring)
-        - [Automating Lightning Payments](#automating-lightning-payments)
-        - [Executing Commands with Received Files](#executing-commands-with-received-files)
-        - [Satellite API Channels](#satellite-api-channels)
-        - [Lightning Gossip Snapshots](#lightning-gossip-snapshots)
-        - [Bitcoin Source Code Messages](#bitcoin-source-code-messages)
+- [Encryption Keys](#encryption-keys)
+- [Satellite API Transmission](#satellite-api-transmission)
+  - [Choosing the Recipient](#choosing-the-recipient)
+  - [Signing the Messages](#signing-the-messages)
+- [Satellite API Reception](#satellite-api-reception)
+  - [Choosing the Sender](#choosing-the-sender)
+- [Demo Receiver](#demo-receiver)
+- [Further Information](#further-information)
+  - [Lightning Wallets](#lightning-wallets)
+  - [Plaintext Mode](#plaintext-mode)
+  - [Receiving Messages Sent from the Browser](#receiving-messages-sent-from-the-browser)
+  - [Reliable Transmissions](#reliable-transmissions)
+  - [Transmission over Selected Regions](#transmission-over-selected-regions)
+  - [Running on Testnet](#running-on-testnet)
+  - [Bump and Delete API orders](#bump-and-delete-api-orders)
+  - [Password-protected GPG keyring](#password-protected-gpg-keyring)
+  - [Automating Lightning Payments](#automating-lightning-payments)
+  - [Executing Commands with Received Files](#executing-commands-with-received-files)
+  - [Satellite API Channels](#satellite-api-channels)
+  - [Lightning Gossip Snapshots](#lightning-gossip-snapshots)
+  - [Bitcoin Source Code Messages](#bitcoin-source-code-messages)
 
 <!-- markdown-toc end -->
 
 
 
 ## Encryption Keys
 
@@ -220,22 +219,24 @@
 blocksat-cli api send --plaintext --send-raw
 ```
 
 ### Reliable Transmissions
 
 The API messages sent over satellite are not guaranteed to be received by all satellite receivers. Each receiver experiences a unique reception quality, depending primarily on its location, weather conditions, and the adopted receiver hardware. When the signal quality is low, it becomes more likely for the receiver to fail on the reception of packets.
 
-One way to increase the chances of successful reception is to use forward error correction (FEC). In essence, FEC adds redundancy to the transmit data so that receivers can recover the original message even if some parts are missing. This is the mechanism that is used, for instance, in Bitcoin Satellite ([see further details in the project's Wiki](https://github.com/Blockstream/bitcoinsatellite/wiki#forward-error-correction-fec)).
+One way to increase the chances of successful reception is to use forward error correction (FEC). In essence, FEC adds redundancy to the transmitted data so that receivers can recover the original message even if some parts are missing. This is the mechanism that is used, for instance, in Bitcoin Satellite ([see further details in the project's Wiki](https://github.com/Blockstream/bitcoinsatellite/wiki#forward-error-correction-fec)).
 
 To send an API message using FEC encoding, run:
 
 ```
 blocksat-cli api send --fec
 ```
 
+> NOTE: the FEC feature requires the `zfec` dependency. You can enable it by installing the CLI with `sudo pip3 install blocksat-cli[fec]` or by installing the `zfec` package via pip3 directly.
+
 The `api listen` command detects and decodes FEC-encoded messages automatically.
 
 In general, the higher the number of extra (redundant) pieces of data sent over satellite, the better the protection to data loss over the satellite link.  The user can tune this parameter using the command-line argument `--fec-overhead`. By default, this argument is `0.1` (equivalent to 10%), such that, for a message that originally occupies 10 packets, the application sends one extra packet.
 
 
 ### Transmission over Selected Regions
```

### Comparing `blocksat-cli-0.4.5/doc/bitcoin.md` & `blocksat-cli-0.4.6/doc/bitcoin.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 ---
 
 # Bitcoin Satellite
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Bitcoin Satellite](#bitcoin-satellite)
-    - [Overview](#overview)
-    - [Installation](#installation)
-    - [Configuration](#configuration)
-    - [Running](#running)
-    - [Further Information](#further-information)
-        - [UDP Multicast Reception Option](#udp-multicast-reception-option)
-        - [Installation from Binary Packages](#installation-from-binary-packages)
-        - [Compilation from Source](#compilation-from-source)
+- [Overview](#overview)
+- [Installation](#installation)
+- [Configuration](#configuration)
+- [Running](#running)
+- [Further Information](#further-information)
+  - [UDP Multicast Reception Option](#udp-multicast-reception-option)
+  - [Installation from Binary Packages](#installation-from-binary-packages)
+  - [Compilation from Source](#compilation-from-source)
 
 <!-- markdown-toc end -->
 
 ## Overview
 
 [Bitcoin Satellite](https://github.com/Blockstream/bitcoinsatellite) is a fork of [FIBRE (Fast Internet Bitcoin Relay Engine)](https://bitcoinfibre.org) and, consequently, also a fork of [Bitcoin Core](https://bitcoincore.org). It features a version of the bitcoind application with support for the reception of blocks sent over satellite in UDP datagrams with multicast addressing. You can find detailed information regarding how Bitcoin Satellite works on the project's [Wiki page](https://github.com/Blockstream/bitcoinsatellite/wiki).
```

### Comparing `blocksat-cli-0.4.5/doc/docker.md` & `blocksat-cli-0.4.6/doc/docker.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 ---
 
 # Running on Docker
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Running on Docker](#running-on-docker)
-    - [Standalone Receiver](#standalone-receiver)
-    - [USB Receiver](#usb-receiver)
-    - [SDR Receiver](#sdr-receiver)
-    - [Sat-IP Receiver](#sat-ip-receiver)
-    - [Bitcoin Satellite](#bitcoin-satellite)
-    - [Build the Docker Image Locally](#build-the-docker-image-locally)
+- [Standalone Receiver](#standalone-receiver)
+- [USB Receiver](#usb-receiver)
+- [SDR Receiver](#sdr-receiver)
+- [Sat-IP Receiver](#sat-ip-receiver)
+- [Bitcoin Satellite](#bitcoin-satellite)
+- [Build the Docker Image Locally](#build-the-docker-image-locally)
 
 <!-- markdown-toc end -->
 
 
 A Docker image is available to be used as the *Blockstream Satellite host*, that is, the system with everything you need to interface with the supported satellite receivers. All you need to do is run the `blockstream/satellite` Docker image while providing the appropriate resources to the container. This process is explained next.
 
 ## Standalone Receiver
```

### Comparing `blocksat-cli-0.4.5/doc/dual-satellite.md` & `blocksat-cli-0.4.6/doc/dual-satellite.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 ---
 
 # Dual-Satellite Connection
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Dual-Satellite Connection](#dual-satellite-connection)
-    - [Required Hardware](#required-hardware)
-    - [Host Configuration](#host-configuration)
-        - [Novra S400 Standalone Receiver](#novra-s400-standalone-receiver)
-        - [TBS 5927/5520SE USB Receiver](#tbs-usb-receiver)
-        - [Blockstream Base Station Sat-IP Receiver](#blockstream-base-station-sat-ip-receiver)
-        - [SDR Receiver](#sdr-receiver)
+- [Required Hardware](#required-hardware)
+- [Host Configuration](#host-configuration)
+  - [Novra S400 Standalone Receiver](#novra-s400-standalone-receiver)
+  - [TBS USB Receiver](#tbs-usb-receiver)
+  - [Blockstream Base Station Sat-IP Receiver](#blockstream-base-station-sat-ip-receiver)
+  - [SDR Receiver](#sdr-receiver)
 
 <!-- markdown-toc end -->
 
 
 Some regions worldwide are covered by two satellites at the same time. For example, most of the US has coverage from both Galaxy 18 and Eutelsat 113. In Asia, there is extensive overlapping coverage from Telstar 18V C and Telstar 18V Ku. If you are in such a region with overlapping coverage, you can connect to two satellites simultaneously and double the Bitcoin block transfer speed. This page describes the hardware and host configurations required to run such a dual-satellite setup.
 
 Before continuing, however, you should check if your location has overlapping coverage from two satellites using our [Coverage Map](https://blockstream.com/satellite/#satellite_network-coverage). Also, note distinct signal strengths are expected from each satellite, given that the distance and viewing angles from your station to each satellite are different. Hence, we also recommend checking the [Link Analyzer](https://satellite.blockstream.space/link-analyzer/) tool for more specific antenna recommendations for each satellite.
```

### Comparing `blocksat-cli-0.4.5/doc/frequency.md` & `blocksat-cli-0.4.6/doc/frequency.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 ---
 
 # Frequency Guide
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
 **Table of Contents**
 
-- [Frequency Guide](#frequency-guide)
-    - [Signal Bands](#signal-bands)
-    - [Signal Frequencies](#signal-frequencies)
-    - [L-band Frequencies](#l-band-frequencies)
+- [Signal Bands](#signal-bands)
+- [Signal Frequencies](#signal-frequencies)
+- [L-band Frequencies](#l-band-frequencies)
 
 <!-- markdown-toc end -->
 
 This page summarizes several frequencies of interest.
 
 ## Signal Bands
 
@@ -33,22 +32,22 @@
 | Satellite          | Band    | Frequency    |
 | ------------------ | ------- | ------------ |
 | Galaxy 18          | Ku High | 11913.4 MHz  |
 | Eutelsat 113       | Ku High | 12066.9 MHz  |
 | Telstar 11N Africa | Ku Low  | 11452.1 MHz  |
 | Telstar 11N Europe | Ku Low  | 11505.4 MHz  |
 | Telstar 18V Ku     | Ku Low  | 11506.75 MHz |
-| Telstar 18V C      | C       | 4053.83 MHz  |
+| Telstar 18V C      | C       | 4057.4 MHz   |
 
 ## L-band Frequencies
 
 Next, the following table summarizes the L-band frequencies to be used in each region based on the typical LNB local oscillator (LO) frequencies:
 
-| LO Frequency        | 5150 MHz    | 9750 MHz    | 10600 MHz  | 10750 MHz  |
-| ------------------- | ----------- | ----------- | ---------- | ---------- |
-| Galaxy 18           |             |             | 1313.4 MHz | 1163.4 MHz |
-| Eutelsat 113        |             |             | 1466.9 MHz | 1316.9 MHz |
-| Telstar 11N Africa  |             | 1702.1 MHz  |            |            |
-| Telstar 11N Europe  |             | 1755.4 MHz  |            |            |
-| Telstar 18V Ku Band |             | 1756.75 MHz |            |            |
-| Telstar 18V C Band  | 1096.17 MHz |             |            |            |
+| LO Frequency        | 5150 MHz   | 9750 MHz    | 10600 MHz  | 10750 MHz  |
+| ------------------- | ---------- | ----------- | ---------- | ---------- |
+| Galaxy 18           |            |             | 1313.4 MHz | 1163.4 MHz |
+| Eutelsat 113        |            |             | 1466.9 MHz | 1316.9 MHz |
+| Telstar 11N Africa  |            | 1702.1 MHz  |            |            |
+| Telstar 11N Europe  |            | 1755.4 MHz  |            |            |
+| Telstar 18V Ku Band |            | 1756.75 MHz |            |            |
+| Telstar 18V C Band  | 1092.6 MHz |             |            |            |
```

### Comparing `blocksat-cli-0.4.5/doc/hardware.md` & `blocksat-cli-0.4.6/doc/hardware.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,27 @@
 This page explains the hardware components required to assemble a Blockstream Satellite receiver.
 
 There are three alternatives to collect the required hardware. The first and quickest option is to purchase a ready-to-use [Satellite Kit](#satellite-kits). Alternatively, you can buy the [Satellite Kit Components](#satellite-kit-components) on your own. Lastly, you can opt for a completely DIY setup, where you pick a combination of compatible parts on your own. To do so, you will need to understand the [hardware requirements](#diy-hardware-requirements). This page covers the three approaches.
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Hardware Guide](#hardware-guide)
-    - [Satellite Kits](#satellite-kits)
-        - [Satellite Kit Comparison](#satellite-kit-comparison)
-    - [Satellite Kit Components](#satellite-kit-components)
-        - [Blockstream Satellite Basic Kit](#blockstream-satellite-basic-kit)
-        - [Blockstream Satellite Pro Kit](#blockstream-satellite-pro-kit)
-        - [Blockstream Satellite Base Station](#blockstream-satellite-base-station)
-    - [DIY Hardware Requirements](#diy-hardware-requirements)
-        - [Supported Receiver Options](#supported-receiver-options)
-        - [Common Required Components](#common-required-components)
-            - [Satellite Antenna](#satellite-antenna)
-            - [LNB](#lnb)
-            - [LNB Mounting Bracket](#lnb-mounting-bracket)
-            - [Coaxial Cables](#coaxial-cables)
-        - [Setup-Specific Components](#setup-specific-components)
-            - [Software-defined Radio (SDR) Setup](#software-defined-radio-sdr-setup)
-            - [Linux USB Receiver Setup](#linux-usb-receiver-setup)
-            - [Standalone Receiver Setup](#standalone-receiver-setup)
-            - [Sat-IP Receiver Setup](#sat-ip-receiver-setup)
-    - [Further Notes](#further-notes)
-        - [Universal LNB](#universal-lnb)
-        - [LNB vs. LNBF](#lnb-vs-lnbf)
+- [Satellite Kits](#satellite-kits)
+  - [Satellite Kit Comparison](#satellite-kit-comparison)
+- [Satellite Kit Components](#satellite-kit-components)
+  - [Blockstream Satellite Basic Kit](#blockstream-satellite-basic-kit)
+  - [Blockstream Satellite Pro Kit](#blockstream-satellite-pro-kit)
+  - [Blockstream Satellite Base Station](#blockstream-satellite-base-station)
+- [DIY Hardware Requirements](#diy-hardware-requirements)
+  - [Supported Receiver Options](#supported-receiver-options)
+  - [Common Required Components](#common-required-components)
+  - [Setup-Specific Components](#setup-specific-components)
+- [Further Notes](#further-notes)
+  - [Universal LNB](#universal-lnb)
+  - [LNB vs. LNBF](#lnb-vs-lnbf)
 
 <!-- markdown-toc end -->
 
 
 ## Satellite Kits
 
 As mentioned earlier, the quickest alternative to gather the required parts for a Blockstream Satellite setup is by purchasing a satellite kit. Check the kits available on the [Blockstream Store](https://store.blockstream.com/product-category/satellite_kits/).
```

### Comparing `blocksat-cli-0.4.5/doc/img/api_architecture.png` & `blocksat-cli-0.4.6/doc/img/api_architecture.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/azimuth.png` & `blocksat-cli-0.4.6/doc/img/azimuth.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/blockstream.png` & `blocksat-cli-0.4.6/doc/img/blockstream.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/elevation.png` & `blocksat-cli-0.4.6/doc/img/elevation.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/gqrx-centered.png` & `blocksat-cli-0.4.6/doc/img/gqrx-centered.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/gqrx-offset.png` & `blocksat-cli-0.4.6/doc/img/gqrx-offset.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/leandvb-pls-syms.png` & `blocksat-cli-0.4.6/doc/img/leandvb-pls-syms.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/leandvb-pre-processed-iq.png` & `blocksat-cli-0.4.6/doc/img/leandvb-pre-processed-iq.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/leandvb-pre-processed-iq2.png` & `blocksat-cli-0.4.6/doc/img/leandvb-pre-processed-iq2.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/leandvb-spectrum-centered.png` & `blocksat-cli-0.4.6/doc/img/leandvb-spectrum-centered.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/leandvb-spectrum-offset.png` & `blocksat-cli-0.4.6/doc/img/leandvb-spectrum-offset.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/lnb_polarization.png` & `blocksat-cli-0.4.6/doc/img/lnb_polarization.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/monitoring-api-authentication.png` & `blocksat-cli-0.4.6/doc/img/monitoring-api-authentication.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/s400_locked.png` & `blocksat-cli-0.4.6/doc/img/s400_locked.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/s400_rf_status.png` & `blocksat-cli-0.4.6/doc/img/s400_rf_status.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/s400_searching.png` & `blocksat-cli-0.4.6/doc/img/s400_searching.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/sat-ip-connections.png` & `blocksat-cli-0.4.6/doc/img/sat-ip-connections.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/sdr_connections.png` & `blocksat-cli-0.4.6/doc/img/sdr_connections.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/standalone_connections.png` & `blocksat-cli-0.4.6/doc/img/standalone_connections.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/img/usb_connections.png` & `blocksat-cli-0.4.6/doc/img/usb_connections.png`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/monitoring.md` & `blocksat-cli-0.4.6/doc/monitoring.md`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/quick-reference.md` & `blocksat-cli-0.4.6/doc/quick-reference.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 This page contains a quick reference guide for the Blockstream Satellite receiver setup and its general usage. Please refer to the [main guide](../index.md) for detailed explanations on all steps.
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 
 - [CLI Installation and Upgrade](#cli-installation-and-upgrade)
 - [Common Steps](#common-steps)
 - [Receiver-specific Configuration Steps](#receiver-specific-configuration-steps)
-    - [Novra S400 standalone receiver](#novra-s400-standalone-receiver)
-    - [TBS 5927/5520SE USB receiver](#tbs-usb-receiver)
-    - [Sat-IP receiver](#sat-ip-receiver)
-    - [SDR receiver](#sdr-receiver)
+  - [Novra S400 standalone receiver](#novra-s400-standalone-receiver)
+  - [TBS USB receiver](#tbs-usb-receiver)
+  - [Sat-IP receiver](#sat-ip-receiver)
+  - [SDR receiver](#sdr-receiver)
 - [Receiver-specific Antenna Alignment Steps](#receiver-specific-antenna-alignment-steps)
-    - [Novra S400 standalone receiver](#novra-s400-standalone-receiver-1)
-    - [TBS 5927/5520SE USB receiver](#tbs-usb-receiver-1)
-    - [Sat-IP receiver](#sat-ip-receiver-1)
-    - [SDR receiver](#sdr-receiver-1)
+  - [Novra S400 standalone receiver](#novra-s400-standalone-receiver-1)
+  - [TBS USB receiver](#tbs-usb-receiver-1)
+  - [Sat-IP receiver](#sat-ip-receiver-1)
+  - [SDR receiver](#sdr-receiver-1)
 - [Bitcoin-satellite Setup](#bitcoin-satellite-setup)
 - [Satellite API](#satellite-api)
 
 <!-- markdown-toc end -->
 
 
 ## CLI Installation and Upgrade
```

### Comparing `blocksat-cli-0.4.5/doc/s400.md` & `blocksat-cli-0.4.6/doc/s400.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 # Novra S400 Receiver
 
 The Novra S400 is a standalone receiver, which receives a satellite signal and outputs IP packets to one or multiple hosts listening to it in the local network. Hence, you will need to configure both the S400 and the host(s).
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Novra S400 Receiver](#novra-s400-receiver)
-    - [Connections](#connections)
-    - [Network Connection](#network-connection)
-    - [Software Requirements](#software-requirements)
-    - [Receiver and Host Configuration](#receiver-and-host-configuration)
-    - [Monitoring](#monitoring)
-    - [Next Steps](#next-steps)
-    - [Further Information](#further-information)
-        - [Dual-satellite Setup](#dual-satellite-setup)
-        - [S400 configuration via the web UI](#s400-configuration-via-the-web-ui)
+- [Connections](#connections)
+- [Network Connection](#network-connection)
+- [Software Requirements](#software-requirements)
+- [Receiver and Host Configuration](#receiver-and-host-configuration)
+- [Monitoring](#monitoring)
+- [Next Steps](#next-steps)
+- [Further Information](#further-information)
+  - [Dual-satellite Setup](#dual-satellite-setup)
+  - [S400 Configuration via the Web UI](#s400-configuration-via-the-web-ui)
 
 <!-- markdown-toc end -->
 
 ## Connections
 
 The Novra S400 can be connected as follows:
 
@@ -90,15 +89,15 @@
 
 ```
 blocksat-cli --cfg rx2 standalone --demod 2 cfg --rx-only
 ```
 
 Refer to further information on the [dual-satellite setup](dual-satellite.md) guide.
 
-### S400 configuration via the web UI
+### S400 Configuration via the Web UI
 
 1. Open the browser and access the IP address of the S400. By default, the address is `192.168.1.2` if connected to LAN 1 or `192.168.2.2` if connected to LAN 2.
 
 2. Log in as admin on the top right of the page.
 - Default password: "password"
 
 3. Check the signal parameters that apply to your setup. Run the following command and use the results in the next step.
```

### Comparing `blocksat-cli-0.4.5/doc/sat-ip.md` & `blocksat-cli-0.4.6/doc/sat-ip.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 # Selfsat>IP22 Sat-IP Receiver
 
 The Selfsat>IP22 is an all-in-one flat-panel antenna with an integrated DVB-S2 receiver and LNB. It is the basis of the Blockstream Satellite Base Station kit available on the [Blockstream Store](https://store.blockstream.com/product/blockstream-satellite-base-station/). This device receives the satellite signal and outputs IP packets to one or more [Sat-IP clients](https://en.wikipedia.org/wiki/Sat-IP) listening to it in the local network. This page explains how you can connect to the base station device to receive the Blockstream Satellite traffic.
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
 **Table of Contents**
 
-- [Selfsat>IP22 Sat-IP Receiver](#selfsatip22-sat-ip-receiver)
-    - [Connections](#connections)
-    - [Software Requirements](#software-requirements)
-    - [Running](#running)
-    - [Next Steps](#next-steps)
-    - [Further Information](#further-information)
-        - [Software Updates](#software-updates)
-        - [Troubleshooting the Server Discovery](#troubleshooting-the-server-discovery)
-        - [Direct Connection to the Base Station](#direct-connection-to-the-base-station)
-        - [Running on Docker](#running-on-docker)
-        - [Compilation from Source](#compilation-from-source)
+- [Connections](#connections)
+- [Software Requirements](#software-requirements)
+- [Running](#running)
+- [Next Steps](#next-steps)
+- [Further Information](#further-information)
+  - [Software Updates](#software-updates)
+  - [Troubleshooting the Server Discovery](#troubleshooting-the-server-discovery)
+  - [Direct Connection to the Base Station](#direct-connection-to-the-base-station)
+  - [Running on Docker](#running-on-docker)
+  - [Compilation from Source](#compilation-from-source)
 
 <!-- markdown-toc end -->
 
 
 ## Connections
 
 The integrated Sat-IP antenna-receiver can be connected as follows:
```

### Comparing `blocksat-cli-0.4.5/doc/sdr.md` & `blocksat-cli-0.4.6/doc/sdr.md`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/software.md` & `blocksat-cli-0.4.6/doc/software.md`

 * *Files identical despite different names*

### Comparing `blocksat-cli-0.4.5/doc/tbs.md` & `blocksat-cli-0.4.6/doc/tbs.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 The TBS 5927 and TBS 5520SE devices are USB-based DVB-S2 receivers. They receive the satellite signal fed via a coaxial interface and output data to the host over USB. They are also configured directly over USB, and the host is responsible for setting such configurations using specific Linux tools.
 
 The instructions that follow prepare the host for driving the TBS receiver.
 
 <!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
 **Table of Contents**
 
-- [TBS Linux USB Receiver](#tbs-linux-usb-receiver)
-    - [Hardware Connections](#hardware-connections)
-    - [TBS Drivers](#tbs-drivers)
-    - [Setup Configuration Helper](#setup-configuration-helper)
-    - [Software Requirements](#software-requirements)
-    - [Configure the Host](#configure-the-host)
-    - [Launch](#launch)
-    - [Next Steps](#next-steps)
-    - [Further Information](#further-information)
-        - [Docker](#docker)
-        - [Useful Resources](#useful-resources)
-        - [Install Binary Packages Manually](#install-binary-packages-manually)
-        - [Building dvb-apps from source](#building-dvb-apps-from-source)
+- [Hardware Connections](#hardware-connections)
+- [TBS Drivers](#tbs-drivers)
+- [Setup Configuration Helper](#setup-configuration-helper)
+- [Software Requirements](#software-requirements)
+- [Configure the Host](#configure-the-host)
+- [Launch](#launch)
+- [Next Steps](#next-steps)
+- [Further Information](#further-information)
+  - [Docker](#docker)
+  - [Useful Resources](#useful-resources)
+  - [Install Binary Packages Manually](#install-binary-packages-manually)
+  - [Building dvb-apps from Source](#building-dvb-apps-from-source)
 
 <!-- markdown-toc end -->
 
 ## Hardware Connections
 
 The TBS 5927/5520SE should be connected as follows:
 
@@ -136,15 +135,15 @@
 sudo dnf copr enable blockstream/satellite
 sudo dnf install dvb-apps
 ```
 
 > If command `dnf copr enable` is not available in your system, install package `dnf-plugins-core`.
 
 
-### Building dvb-apps from source
+### Building dvb-apps from Source
 
 Alternatively, you can build `dvb-apps` from source by running the following commands:
 
 ```
 git clone https://github.com/Blockstream/dvb-apps
 cd dvb-apps
 make
```

### Comparing `blocksat-cli-0.4.5/setup.py` & `blocksat-cli-0.4.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     description="Blockstream Satellite CLI",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Blockstream Corp",
     author_email="satellite@blockstream.com",
     url="https://github.com/Blockstream/satellite",
     install_requires=[
-        'distro', 'requests', 'python-gnupg>=0.4.7', 'sseclient-py', 'qrcode',
-        'zfec>=1.5.4', 'pysnmp'
+        'distro', 'requests', 'python-gnupg>=0.4.7', 'qrcode', 'pysnmp'
     ],
+    extras_require={"fec": ['zfec>=1.5.4']},
     package_data={'blocksatcli': ['mib/*.mib', 'mib/*.txt', 'gpg/*.gpg']},
     classifiers=[
         'Programming Language :: Python :: 3',
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     python_requires='>=3')
```

