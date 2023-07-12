# Comparing `tmp/moftransformer-2.1.1.tar.gz` & `tmp/moftransformer-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-2.1.1.tar", last modified: Thu Jun  8 07:01:28 2023, max compression
+gzip compressed data, was "moftransformer-2.1.2.tar", last modified: Wed Jul 12 11:34:26 2023, max compression
```

## Comparing `moftransformer-2.1.1.tar` & `moftransformer-2.1.2.tar`

### file list

```diff
@@ -1,280 +1,262 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-06-08 07:01:28.724438 moftransformer-2.1.1/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10620 2023-06-07 08:02:27.000000 moftransformer-2.1.1/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      509 2023-06-07 02:32:17.000000 moftransformer-2.1.1/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3088 2023-06-01 07:55:51.000000 moftransformer-2.1.1/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4370 2023-06-01 08:08:34.000000 moftransformer-2.1.1/moftransformer/cli/predict.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5488 2023-06-01 07:50:27.000000 moftransformer-2.1.1/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4141 2023-06-07 07:17:33.000000 moftransformer-2.1.1/moftransformer/cli/test.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3431 2023-05-10 06:19:20.000000 moftransformer-2.1.1/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/dataset/test/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.700438 moftransformer-2.1.1/moftransformer/examples/dataset/total/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.704438 moftransformer-2.1.1/moftransformer/examples/dataset/train/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.704438 moftransformer-2.1.1/moftransformer/examples/dataset/val/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.708438 moftransformer-2.1.1/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.688438 moftransformer-2.1.1/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.708438 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.712438 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.712438 moftransformer-2.1.1/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.688438 moftransformer-2.1.1/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2023-05-11 05:04:23.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2023-05-11 05:04:24.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2023-05-11 05:04:25.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2023-05-11 05:04:26.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2023-05-11 05:04:26.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2023-05-11 05:04:27.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2023-05-11 05:04:27.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2023-05-11 05:04:28.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2023-05-11 05:04:28.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2023-05-11 05:04:29.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2023-05-11 05:04:29.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:33.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2COTA
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2023-05-11 05:04:33.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2props
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:31.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2visit
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2023-05-11 05:04:31.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid_gen
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13191 2023-06-08 05:11:08.000000 moftransformer-2.1.1/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7522 2023-05-11 02:40:22.000000 moftransformer-2.1.1/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8568 2023-06-08 05:11:29.000000 moftransformer-2.1.1/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10433 2023-06-08 05:35:34.000000 moftransformer-2.1.1/moftransformer/predict.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10576 2023-06-07 06:30:29.000000 moftransformer-2.1.1/moftransformer/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8614 2023-06-07 07:19:44.000000 moftransformer-2.1.1/moftransformer/test.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16162 2023-05-25 04:50:04.000000 moftransformer-2.1.1/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3986 2023-06-01 08:08:31.000000 moftransformer-2.1.1/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12879 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-06-08 07:01:28.724438 moftransformer-2.1.1/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.1.1/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-07-12 11:34:26.487928 moftransformer-2.1.2/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10620 2023-07-12 11:18:53.000000 moftransformer-2.1.2/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      509 2023-07-12 08:25:55.000000 moftransformer-2.1.2/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3088 2023-07-12 07:23:56.000000 moftransformer-2.1.2/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4370 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/predict.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5488 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4141 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/test.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3431 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/examples/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer/examples/dataset/test/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/test_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.479928 moftransformer-2.1.2/moftransformer/examples/dataset/total/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-07-12 08:38:25.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-07-12 08:38:25.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:25.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:25.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-07-12 08:38:29.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-07-12 08:38:29.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:29.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:29.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:24.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:30.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:26.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-07-12 08:38:28.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-07-12 08:38:28.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:28.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:28.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-07-12 08:38:27.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-07-12 08:38:27.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:27.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:27.000000 moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.479928 moftransformer-2.1.2/moftransformer/examples/dataset/train/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/train_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.479928 moftransformer-2.1.2/moftransformer/examples/dataset/val/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-07-12 08:38:31.000000 moftransformer-2.1.2/moftransformer/examples/dataset/val_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.483928 moftransformer-2.1.2/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.467928 moftransformer-2.1.2/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.483928 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.467928 moftransformer-2.1.2/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/Vector.hpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13397 2023-07-12 10:53:37.000000 moftransformer-2.1.2/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7522 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8568 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10433 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/predict.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10576 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8614 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/test.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4378 2023-07-12 08:25:33.000000 moftransformer-2.1.2/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16162 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3986 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.487928 moftransformer-2.1.2/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-07-12 07:09:29.000000 moftransformer-2.1.2/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-07-12 11:34:26.471928 moftransformer-2.1.2/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12124 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-07-12 11:34:26.000000 moftransformer-2.1.2/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-07-12 11:34:26.487928 moftransformer-2.1.2/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-07-12 07:09:29.000000 moftransformer-2.1.2/setup.py
```

### Comparing `moftransformer-2.1.1/PKG-INFO` & `moftransformer-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.1.1
+Version: 2.1.2
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.2-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.2-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.1.1 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.2 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
```

### Comparing `moftransformer-2.1.1/README.md` & `moftransformer-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.2-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.2-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

### Comparing `moftransformer-2.1.1/moftransformer/assets/bbs.json` & `moftransformer-2.1.2/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/assets/colors.py` & `moftransformer-2.1.2/moftransformer/assets/colors.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/assets/topology.json` & `moftransformer-2.1.2/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/cli/download.py` & `moftransformer-2.1.2/moftransformer/cli/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/cli/main.py` & `moftransformer-2.1.2/moftransformer/cli/main.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/cli/predict.py` & `moftransformer-2.1.2/moftransformer/cli/predict.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/cli/run.py` & `moftransformer-2.1.2/moftransformer/cli/run.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/cli/test.py` & `moftransformer-2.1.2/moftransformer/cli/test.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/config.py` & `moftransformer-2.1.2/moftransformer/config.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/config_ex.py` & `moftransformer-2.1.2/moftransformer/config_ex.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/database/__init__.py` & `moftransformer-2.1.2/moftransformer/database/__init__.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/datamodules/datamodule.py` & `moftransformer-2.1.2/moftransformer/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/datamodules/dataset.py` & `moftransformer-2.1.2/moftransformer/datamodules/dataset.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.cif` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.graphdata` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.griddata16` & `moftransformer-2.1.2/moftransformer/examples/dataset/val/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/smm+N577+E166.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/ukg+N387+E203.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-2.1.2/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-2.1.2/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/gadgets/my_metrics.py` & `moftransformer-2.1.2/moftransformer/gadgets/my_metrics.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-2.1.2/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/modules/cgcnn.py` & `moftransformer-2.1.2/moftransformer/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/modules/heads.py` & `moftransformer-2.1.2/moftransformer/modules/heads.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/modules/module.py` & `moftransformer-2.1.2/moftransformer/modules/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,18 +326,21 @@
     def on_predict_start(self):
         self.write_log = False
         module_utils.set_task(self)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         output = self(batch)
         
-        softmax = torch.nn.Softmax(dim=1)
         if 'classification_logits' in output:
-            output['classification_logits'] = softmax(output['classification_logits'])
-            output['classification_logits_index'] = torch.argmax(output['classification_logits'], dim=1)
+            if self.hparams.config['n_classes'] == 2:
+                output['classification_logits_index'] = torch.round(output['classification_logits']).to(torch.int)
+            else:
+                softmax = torch.nn.Softmax(dim=1)
+                output['classification_logits'] = softmax(output['classification_logits'])
+                output['classification_logits_index'] = torch.argmax(output['classification_logits'], dim=1)
 
         output = {
             k: (v.cpu().tolist() if torch.is_tensor(v) else v)
             for k, v in output.items()
             if ('logits' in k) or ('labels' in k) or 'cif_id' == k
         }
```

### Comparing `moftransformer-2.1.1/moftransformer/modules/module_utils.py` & `moftransformer-2.1.2/moftransformer/modules/module_utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/modules/objectives.py` & `moftransformer-2.1.2/moftransformer/modules/objectives.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-2.1.2/moftransformer/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/predict.py` & `moftransformer-2.1.2/moftransformer/predict.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/run.py` & `moftransformer-2.1.2/moftransformer/run.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/test.py` & `moftransformer-2.1.2/moftransformer/test.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/utils/download.py` & `moftransformer-2.1.2/moftransformer/utils/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/utils/install_griday.py` & `moftransformer-2.1.2/moftransformer/utils/install_griday.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,18 +61,26 @@
         raise InstallationError(ps.stderr)
     ps = subprocess.run(["make"], cwd=dir_griday / "scripts")
     if ps.returncode:
         raise InstallationError(ps.stderr)
     print(
         "=== Successfully download ======================================================="
     )
-    if Path(GRIDAY_PATH).exists():
+    if not Path(GRIDAY_PATH).exists():
+        raise InstallationError(f"GRIDAY is not installed. Please try again.")
+    
+    print(
+        "=== Check GIRDAY ================================================================"
+    )    
+    ps = subprocess.run([str(GRIDAY_PATH)], cwd=dir_griday, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    if ps.stderr == b'./make_egrid spacing atom_type force_field input_cssr egrid_stem\n':
         print(f"GRIDAY is installed to {dir_griday}")
     else:
-        raise InstallationError(f"GRIDAY is not installed. Please try again.")
+        print (ps.stdout, ps.stderr)
+        print(f'GRIDAY does not installed correctly. Please uninstall griday and re-install.')    
 
 
 def install_griday(install_make=False):
     """
     Installation a GRIDAY which calculates the energy grid for prepare-data.py
     Original code : https://github.com/Sangwon91/GRIDAY.git
```

### Comparing `moftransformer-2.1.1/moftransformer/utils/prepare_data.py` & `moftransformer-2.1.2/moftransformer/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/utils/validation.py` & `moftransformer-2.1.2/moftransformer/utils/validation.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/visualize/drawer.py` & `moftransformer-2.1.2/moftransformer/visualize/drawer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/visualize/setting.py` & `moftransformer-2.1.2/moftransformer/visualize/setting.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/visualize/utils.py` & `moftransformer-2.1.2/moftransformer/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer/visualize/visualizer.py` & `moftransformer-2.1.2/moftransformer/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.1/moftransformer.egg-info/PKG-INFO` & `moftransformer-2.1.2/moftransformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.1.1
+Version: 2.1.2
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.2-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.2-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.1.1 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.2 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
```

### Comparing `moftransformer-2.1.1/moftransformer.egg-info/SOURCES.txt` & `moftransformer-2.1.2/moftransformer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -166,75 +166,57 @@
 moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
 moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
 moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
 moftransformer/gadgets/__init__.py
 moftransformer/gadgets/my_metrics.py
 moftransformer/libs/GRIDAY/AtomTypeMap.cpp
 moftransformer/libs/GRIDAY/AtomTypeMap.hpp
-moftransformer/libs/GRIDAY/AtomTypeMap.o
 moftransformer/libs/GRIDAY/Cell.hpp
 moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
 moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
-moftransformer/libs/GRIDAY/ChannelAnalyzer.o
 moftransformer/libs/GRIDAY/EnergyGrid.cpp
 moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
 moftransformer/libs/GRIDAY/EnergyGrid.hpp
-moftransformer/libs/GRIDAY/EnergyGrid.o
 moftransformer/libs/GRIDAY/ForceField.cpp
 moftransformer/libs/GRIDAY/ForceField.hpp
-moftransformer/libs/GRIDAY/ForceField.o
 moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
 moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
-moftransformer/libs/GRIDAY/FourierAnalyzer.o
 moftransformer/libs/GRIDAY/Framework.cpp
 moftransformer/libs/GRIDAY/Framework.hpp
-moftransformer/libs/GRIDAY/Framework.o
 moftransformer/libs/GRIDAY/Gaussian.cpp
 moftransformer/libs/GRIDAY/Gaussian.hpp
-moftransformer/libs/GRIDAY/Gaussian.o
 moftransformer/libs/GRIDAY/GridMaker.cpp
 moftransformer/libs/GRIDAY/GridMaker.hpp
-moftransformer/libs/GRIDAY/GridMaker.o
 moftransformer/libs/GRIDAY/Griday.hpp
 moftransformer/libs/GRIDAY/GridayException.cpp
 moftransformer/libs/GRIDAY/GridayException.hpp
-moftransformer/libs/GRIDAY/GridayException.o
 moftransformer/libs/GRIDAY/GridayTypes.hpp
 moftransformer/libs/GRIDAY/LennardJones.cpp
 moftransformer/libs/GRIDAY/LennardJones.hpp
-moftransformer/libs/GRIDAY/LennardJones.o
 moftransformer/libs/GRIDAY/Makefile
 moftransformer/libs/GRIDAY/MaterialGrid.cpp
 moftransformer/libs/GRIDAY/MaterialGrid.hpp
-moftransformer/libs/GRIDAY/MaterialGrid.o
 moftransformer/libs/GRIDAY/NlistMaker.cpp
 moftransformer/libs/GRIDAY/NlistMaker.hpp
-moftransformer/libs/GRIDAY/NlistMaker.o
 moftransformer/libs/GRIDAY/PairEnergy.hpp
 moftransformer/libs/GRIDAY/Random.hpp
 moftransformer/libs/GRIDAY/ShiftedLJ.cpp
 moftransformer/libs/GRIDAY/ShiftedLJ.hpp
-moftransformer/libs/GRIDAY/ShiftedLJ.o
 moftransformer/libs/GRIDAY/Timer.hpp
 moftransformer/libs/GRIDAY/Vector.hpp
-moftransformer/libs/GRIDAY/libgriday.a
 moftransformer/libs/GRIDAY/FF/UFF_FF.def
 moftransformer/libs/GRIDAY/FF/UFF_Type.def
 moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
 moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
 moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
 moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
 moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
 moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
 moftransformer/libs/GRIDAY/scripts/Makefile
 moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
-moftransformer/libs/GRIDAY/scripts/grid2COTA
-moftransformer/libs/GRIDAY/scripts/grid2props
-moftransformer/libs/GRIDAY/scripts/grid2visit
-moftransformer/libs/GRIDAY/scripts/grid_gen
 moftransformer/libs/GRIDAY/scripts/main_cota.cpp
 moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
 moftransformer/libs/GRIDAY/scripts/main_visit.cpp
 moftransformer/modules/__init__.py
 moftransformer/modules/cgcnn.py
 moftransformer/modules/heads.py
 moftransformer/modules/module.py
```

### Comparing `moftransformer-2.1.1/setup.py` & `moftransformer-2.1.2/setup.py`

 * *Files identical despite different names*

