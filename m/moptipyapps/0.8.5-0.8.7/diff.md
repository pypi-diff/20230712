# Comparing `tmp/moptipyapps-0.8.5.tar.gz` & `tmp/moptipyapps-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moptipyapps-0.8.5.tar", last modified: Thu Jun 22 01:51:43 2023, max compression
+gzip compressed data, was "moptipyapps-0.8.7.tar", last modified: Wed Jul 12 08:40:45 2023, max compression
```

## Comparing `moptipyapps-0.8.5.tar` & `moptipyapps-0.8.7.tar`

### file list

```diff
@@ -1,184 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.950831 moptipyapps-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-06-22 01:51:43.950831 moptipyapps-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.898830 moptipyapps-0.8.5/moptipyapps/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.902830 moptipyapps-0.8.5/moptipyapps/binpacking2d/
--rwxr-xr-x   0 runner    (1001) docker     (123)   191757 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/2dpacklib.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/bin_count_and_last_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/ibl_encoding_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22954 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/ibl_encoding_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27747 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/make_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/packing_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/binpacking2d/plot_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.902830 moptipyapps-0.8.5/moptipyapps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tests/on_binpacking2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.902830 moptipyapps-0.8.5/moptipyapps/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/ea1p1_revn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/fea1p1_revn.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/known_optima.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tour_length.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.950831 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/a280.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/a280.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ali535.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/att48.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/att48.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/att532.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bayg29.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bayg29.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bays29.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bays29.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/berlin52.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/berlin52.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bier127.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/br17.atsp
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brazil58.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brg180.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)    98436 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brg180.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/burma14.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch130.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch130.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch150.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch150.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d1291.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    47015 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d1655.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d198.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d493.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d657.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/dantzig42.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil101.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil101.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil51.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil51.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil76.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil76.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl1400.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    44754 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl1577.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl417.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fri26.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fri26.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ft53.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ft70.atsp
--rw-r--r--   0 runner    (1001) docker     (123)   360799 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv170.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv33.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv35.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv38.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv44.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv47.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    38312 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv55.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    51562 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv64.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    60649 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv70.atsp
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gil262.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr120.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)    30909 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr120.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr137.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr17.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr202.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr202.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr21.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr229.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr24.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr24.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr431.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr48.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr48.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr666.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr666.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr96.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr96.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/hk48.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    81561 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kro124p.atsp
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA100.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA150.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA200.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB150.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB200.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroC100.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroC100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroD100.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroD100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroE100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/lin105.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/lin105.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/lin318.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/nrw1379.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/p43.atsp
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/p654.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    33047 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb1173.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb442.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb442.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr1002.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr1002.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr107.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr124.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr136.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr144.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr152.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr226.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr264.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr299.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr439.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr76.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr76.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat195.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat575.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat783.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat99.tsp
--rw-r--r--   0 runner    (1001) docker     (123)   423944 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg323.atsp
--rw-r--r--   0 runner    (1001) docker     (123)   520701 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg358.atsp
--rw-r--r--   0 runner    (1001) docker     (123)   659477 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg403.atsp
--rw-r--r--   0 runner    (1001) docker     (123)   797126 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg443.atsp
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rd100.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rd100.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rd400.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1304.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    37385 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1323.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    53799 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1889.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ry48p.atsp
--rw-r--r--   0 runner    (1001) docker     (123)  2162350 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si1032.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    62351 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si175.tsp
--rw-r--r--   0 runner    (1001) docker     (123)   579782 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si535.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/st70.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/st70.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/swiss42.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ts225.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/tsp225.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/tsp225.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    29768 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1060.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    40548 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1432.tsp
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u159.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    51713 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1817.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u574.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u724.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ulysses16.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ulysses16.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ulysses22.opt.tour
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ulysses22.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/vm1084.tsp
--rw-r--r--   0 runner    (1001) docker     (123)    49714 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/tsp/tsplib/vm1748.tsp
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/moptipyapps/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.902830 moptipyapps-0.8.5/moptipyapps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 01:51:43.000000 moptipyapps-0.8.5/moptipyapps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 01:51:43.950831 moptipyapps-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:51:43.950831 moptipyapps-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/tests/test_examples_in_examples_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-06-22 01:42:20.000000 moptipyapps-0.8.5/tests/test_links_in_documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.779011 moptipyapps-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    23875 2023-07-12 08:40:45.779011 moptipyapps-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.739009 moptipyapps-0.8.7/moptipyapps/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.743009 moptipyapps-0.8.7/moptipyapps/binpacking2d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   191757 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/2dpacklib.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/bin_count_and_last_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/bin_count_and_last_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/ibl_encoding_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22954 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/ibl_encoding_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27904 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/make_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/packing_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/binpacking2d/plot_packing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.743009 moptipyapps-0.8.7/moptipyapps/dynamic_control/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.747009 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/cubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/min_ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/partially_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/controllers/quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/objective_le.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/results_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/results_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/starting_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.747009 moptipyapps-0.8.7/moptipyapps/dynamic_control/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/systems/lorenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/dynamic_control/systems/stuart_landau.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.747009 moptipyapps-0.8.7/moptipyapps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tests/on_binpacking2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.747009 moptipyapps-0.8.7/moptipyapps/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/ea1p1_revn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/fea1p1_revn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/known_optima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tour_length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.775011 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/a280.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/a280.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ali535.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/att48.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/att48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/att532.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bayg29.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bayg29.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bays29.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bays29.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/berlin52.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/berlin52.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bier127.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/br17.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brazil58.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brg180.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    98436 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brg180.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/burma14.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch130.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch130.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch150.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d1291.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    47015 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d1655.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d198.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d493.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d657.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/dantzig42.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil101.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil101.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil51.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil51.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil76.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil76.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl1400.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    44754 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl1577.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl417.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fri26.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fri26.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ft53.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ft70.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   360799 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv170.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv33.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv35.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv38.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv44.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv47.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    38312 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv55.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    51562 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv64.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    60649 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv70.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gil262.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr120.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    30909 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr120.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr137.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr17.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr202.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr202.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr21.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr229.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr24.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr24.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr431.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr48.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr666.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr666.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr96.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr96.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/hk48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    81561 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kro124p.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA200.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB200.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroC100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroC100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroD100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroD100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroE100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/lin105.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/lin105.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/lin318.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/nrw1379.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/p43.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/p654.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    33047 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb1173.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb442.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb442.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr1002.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr1002.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr107.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr124.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr136.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr144.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr152.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr226.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr264.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr299.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr439.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr76.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr76.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat195.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat575.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat783.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat99.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)   423944 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg323.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   520701 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg358.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   659477 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg403.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   797126 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg443.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rd100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rd100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rd400.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1304.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    37385 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1323.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    53799 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1889.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ry48p.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)  2162350 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si1032.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    62351 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si175.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)   579782 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si535.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/st70.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/st70.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/swiss42.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ts225.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/tsp225.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/tsp225.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    29768 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1060.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    40548 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1432.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u159.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    51713 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1817.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u574.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u724.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ulysses16.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ulysses16.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ulysses22.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ulysses22.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/vm1084.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    49714 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/tsp/tsplib/vm1748.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/moptipyapps/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.739009 moptipyapps-0.8.7/moptipyapps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23875 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 08:40:45.000000 moptipyapps-0.8.7/moptipyapps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-12 08:40:45.779011 moptipyapps-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:40:45.779011 moptipyapps-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/tests/test_examples_in_examples_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-07-12 08:31:05.000000 moptipyapps-0.8.7/tests/test_links_in_documentation.py
```

### Comparing `moptipyapps-0.8.5/PKG-INFO` & `moptipyapps-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moptipyapps
-Version: 0.8.5
+Version: 0.8.7
 Summary: Applications of Metaheuristic Optimization in Python.
 Home-page: https://thomasweise.github.io/moptipy
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -148,14 +148,41 @@
 *Examples:*
 
 - [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
 
 Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
+### 3.3. Dynamic Controller Synthesis
+
+Another interesting example for optimization is the synthesis of [active controllers for dynamic systems](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.html).
+Dynamic systems have a state that changes over time based on some laws.
+These laws may be expressed as ordinary differential equations, for example.
+The classical [Stuart-Landau system](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.systems.html#module-moptipyapps.dynamic_control.systems.stuart_landau), for instance, represents an object whose coordinates on a two-dimensional plane change as follows:
+
+```
+sigma = 0.1 - x² - y²
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x
+```
+
+Regardless on which `(x, y)` the object initially starts, it tends to move to a circular rotation path centered around the origin with radius `sqrt(0.1)`.
+Now we try to create a controller `ctrl` for such a system that moves the object from this periodic circular path into a fixed and stable location.
+The controller `ctrl` receives the current state, i.e., the object location, as input and can influence the system as follows:
+
+```
+sigma = 0.1 - x² - y²
+c = ctrl(x, y)
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x + c
+```
+
+What we try to find is the controller which can bring move object to the origin `(0, 0)` as quickly as possible while expending the least amount of force, i.e., having the smallest aggregated `c` values over time.
+
+
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
 In other words, detecting bugs is very hard.
 Unfortunately, this holds also for the components of the algorithms, such as the search operators, especially if they are randomized as well.
```

### Comparing `moptipyapps-0.8.5/README.md` & `moptipyapps-0.8.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,41 @@
 *Examples:*
 
 - [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
 
 Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
+### 3.3. Dynamic Controller Synthesis
+
+Another interesting example for optimization is the synthesis of [active controllers for dynamic systems](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.html).
+Dynamic systems have a state that changes over time based on some laws.
+These laws may be expressed as ordinary differential equations, for example.
+The classical [Stuart-Landau system](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.systems.html#module-moptipyapps.dynamic_control.systems.stuart_landau), for instance, represents an object whose coordinates on a two-dimensional plane change as follows:
+
+```
+sigma = 0.1 - x² - y²
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x
+```
+
+Regardless on which `(x, y)` the object initially starts, it tends to move to a circular rotation path centered around the origin with radius `sqrt(0.1)`.
+Now we try to create a controller `ctrl` for such a system that moves the object from this periodic circular path into a fixed and stable location.
+The controller `ctrl` receives the current state, i.e., the object location, as input and can influence the system as follows:
+
+```
+sigma = 0.1 - x² - y²
+c = ctrl(x, y)
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x + c
+```
+
+What we try to find is the controller which can bring move object to the origin `(0, 0)` as quickly as possible while expending the least amount of force, i.e., having the smallest aggregated `c` values over time.
+
+
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
 In other words, detecting bugs is very hard.
 Unfortunately, this holds also for the components of the algorithms, such as the search operators, especially if they are randomized as well.
```

### Comparing `moptipyapps-0.8.5/moptipyapps/__init__.py` & `moptipyapps-0.8.7/moptipyapps/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/2dpacklib.txt` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/2dpacklib.txt`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/__init__.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/bin_count_and_last_empty.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/bin_count_and_last_empty.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 An objective function for minimizing the number of bins of packings.
 
 This objective function first computes the number of bins used. Let's call it
 `n_bins`. We know the total number of items,
 :attr:`~moptipyapps.binpacking2d.instance.Instance.n_items`, as
 well (because this is also the number of rows in the packing).
 Now we return `(n_items * (n_bins - 1)) + number_of_items_in_last_bin`,
-wher `number_of_items_in_last_bin` is, well, the number of items in the
+where `number_of_items_in_last_bin` is, well, the number of items in the
 very last bin.
 
 The idea behind this is: If one of two packings has the smaller number of
 bins, then this one will always have the smaller objective value. If two
 packings have the same number of bins, but one has fewer items in the very
 last bin, then that one is better. With this mechanism, we drive the search
 towards "emptying" the last bin. If the number of items in the last bin would
@@ -23,15 +23,15 @@
 from moptipy.api.objective import Objective
 from moptipy.utils.types import type_error
 
 from moptipyapps.binpacking2d.instance import Instance
 from moptipyapps.binpacking2d.packing import IDX_BIN
 
 
-@numba.njit(cache=True, inline="always")
+@numba.njit(cache=True, inline="always", fastmath=True, boundscheck=False)
 def bin_count_and_last_empty(y: np.ndarray) -> int:
     """
     Compute the number of bins and the emptiness of the last bin.
 
     We compute the total number of bins minus 1 and multiply it with the
     number of items. We then add the number of items in the last bin.
```

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/ibl_encoding_1.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/ibl_encoding_1.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/ibl_encoding_2.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/ibl_encoding_2.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/instance.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,16 @@
 
     #: the name of the instance
     name: str
     #: the total number of items (including repetitions)
     n_items: int
     #: the number of different items
     n_different_items: int
+    #: the total area occupied by all items
+    total_item_area: int
     #: the bin width
     bin_width: int
     #: the bin height
     bin_height: int
     #: the minimum number of bins that this instance requires
     lower_bound_bins: int
 
@@ -341,16 +343,18 @@
         #: the total number of items, i.e., the number of different items
         #: multiplied with their repetition counts
         obj.n_items = n_items
         #: the height of the bins
         obj.bin_height = bin_height
         #: the width of the bins
         obj.bin_width = bin_width
+        #: the total area occupied by all items
+        obj.total_item_area = item_area
 
-# We need as least as many bins such that their area is big enough
+# We need at least as many bins such that their area is big enough
 # for the total area of the items.
         bin_area: int = bin_height * bin_width
         min_size: int = item_area // bin_area
         if (min_size * bin_area) < item_area:
             min_size += 1
         #: the lower bound for the number of bins needed
         obj.lower_bound_bins = check_int_range(
```

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/make_instances.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/make_instances.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/packing.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/packing.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/packing_space.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/packing_space.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/binpacking2d/plot_packing.py` & `moptipyapps-0.8.7/moptipyapps/binpacking2d/plot_packing.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tests/on_binpacking2d.py` & `moptipyapps-0.8.7/moptipyapps/tests/on_binpacking2d.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/__init__.py` & `moptipyapps-0.8.7/moptipyapps/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/ea1p1_revn.py` & `moptipyapps-0.8.7/moptipyapps/tsp/ea1p1_revn.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/fea1p1_revn.py` & `moptipyapps-0.8.7/moptipyapps/tsp/fea1p1_revn.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/instance.py` & `moptipyapps-0.8.7/moptipyapps/tsp/instance.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/known_optima.py` & `moptipyapps-0.8.7/moptipyapps/tsp/known_optima.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tour_length.py` & `moptipyapps-0.8.7/moptipyapps/tsp/tour_length.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/__init__.py` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/a280.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/a280.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/a280.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/a280.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ali535.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ali535.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/att48.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/att48.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/att532.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/att532.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bayg29.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bayg29.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bays29.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bays29.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/berlin52.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/berlin52.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/bier127.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/bier127.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/br17.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/br17.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brazil58.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brazil58.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brg180.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brg180.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/brg180.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/brg180.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/burma14.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/burma14.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch130.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch130.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch150.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch150.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ch150.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ch150.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d1291.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d1291.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d1655.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d1655.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d198.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d198.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d493.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d493.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/d657.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/d657.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/dantzig42.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/dantzig42.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil101.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil101.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil51.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil51.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/eil76.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/eil76.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl1400.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl1400.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl1577.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl1577.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fl417.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fl417.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/fri26.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/fri26.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ft53.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ft53.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ft70.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ft70.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv170.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv170.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv33.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv33.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv35.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv35.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv38.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv38.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv44.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv44.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv47.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv47.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv55.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv55.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv64.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv64.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ftv70.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ftv70.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gil262.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gil262.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr120.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr120.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr137.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr137.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr17.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr17.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr202.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr202.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr202.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr202.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr21.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr21.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr229.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr229.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr24.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr24.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr431.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr431.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr48.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr48.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr666.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr666.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr666.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr666.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/gr96.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/gr96.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/hk48.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/hk48.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kro124p.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kro124p.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA150.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA150.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroA200.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroA200.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB150.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB150.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroB200.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroB200.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroC100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroC100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroD100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroD100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/kroE100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/kroE100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/lin105.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/lin105.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/lin318.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/lin318.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/nrw1379.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/nrw1379.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/p43.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/p43.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/p654.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/p654.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb1173.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb1173.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb442.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb442.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pcb442.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pcb442.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr1002.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr1002.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr1002.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr1002.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr107.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr107.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr124.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr124.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr136.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr136.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr144.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr144.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr152.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr152.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr226.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr226.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr264.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr264.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr299.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr299.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr439.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr439.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/pr76.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/pr76.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat195.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat195.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat575.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat575.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat783.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat783.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rat99.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rat99.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg323.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg323.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg358.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg358.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg403.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg403.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rbg443.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rbg443.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rd100.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rd100.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rd400.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rd400.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1304.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1304.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1323.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1323.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/rl1889.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/rl1889.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ry48p.atsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ry48p.atsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si1032.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si1032.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si175.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si175.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/si535.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/si535.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/st70.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/st70.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/swiss42.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/swiss42.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ts225.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ts225.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/tsp225.opt.tour` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/tsp225.opt.tour`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/tsp225.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/tsp225.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1060.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1060.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1432.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1432.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u159.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u159.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u1817.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u1817.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u574.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u574.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/u724.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/u724.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/ulysses22.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/ulysses22.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/vm1084.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/vm1084.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps/tsp/tsplib/vm1748.tsp` & `moptipyapps-0.8.7/moptipyapps/tsp/tsplib/vm1748.tsp`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/moptipyapps.egg-info/PKG-INFO` & `moptipyapps-0.8.7/moptipyapps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moptipyapps
-Version: 0.8.5
+Version: 0.8.7
 Summary: Applications of Metaheuristic Optimization in Python.
 Home-page: https://thomasweise.github.io/moptipy
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -148,14 +148,41 @@
 *Examples:*
 
 - [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
 
 Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
+### 3.3. Dynamic Controller Synthesis
+
+Another interesting example for optimization is the synthesis of [active controllers for dynamic systems](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.html).
+Dynamic systems have a state that changes over time based on some laws.
+These laws may be expressed as ordinary differential equations, for example.
+The classical [Stuart-Landau system](https://thomasweise.github.io/moptipyapps/moptipyapps.dynamic_control.systems.html#module-moptipyapps.dynamic_control.systems.stuart_landau), for instance, represents an object whose coordinates on a two-dimensional plane change as follows:
+
+```
+sigma = 0.1 - x² - y²
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x
+```
+
+Regardless on which `(x, y)` the object initially starts, it tends to move to a circular rotation path centered around the origin with radius `sqrt(0.1)`.
+Now we try to create a controller `ctrl` for such a system that moves the object from this periodic circular path into a fixed and stable location.
+The controller `ctrl` receives the current state, i.e., the object location, as input and can influence the system as follows:
+
+```
+sigma = 0.1 - x² - y²
+c = ctrl(x, y)
+dx/dt = sigma * x - y
+dy/dt = sigma * y + x + c
+```
+
+What we try to find is the controller which can bring move object to the origin `(0, 0)` as quickly as possible while expending the least amount of force, i.e., having the smallest aggregated `c` values over time.
+
+
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
 In other words, detecting bugs is very hard.
 Unfortunately, this holds also for the components of the algorithms, such as the search operators, especially if they are randomized as well.
```

### Comparing `moptipyapps-0.8.5/setup.cfg` & `moptipyapps-0.8.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 	Source = https://github.com/thomasWeise/moptipyapps/
 	Tracker = https://github.com/thomasWeise/moptipyapps/issues
 
 [options]
 include_package_data = True
 install_requires = 
 	certifi >= 2023.5.7
-	moptipy >= 0.9.77
+	moptipy >= 0.9.84
 	numpy >= 1.24.3
-	numba >= 0.57.0
+	numba >= 0.57.1
 	matplotlib >= 3.7.1
+	scikit-learn >= 1.2.2
 	urllib3 >= 1.26.16
 packages = find:
 python_requires = >= 3.10
 zip_safe = False
 
 [options.package_data]
 moptipyapps = py.typed
```

### Comparing `moptipyapps-0.8.5/setup.py` & `moptipyapps-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/tests/test_examples_in_examples_directory.py` & `moptipyapps-0.8.7/tests/test_examples_in_examples_directory.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.5/tests/test_links_in_documentation.py` & `moptipyapps-0.8.7/tests/test_links_in_documentation.py`

 * *Files identical despite different names*

