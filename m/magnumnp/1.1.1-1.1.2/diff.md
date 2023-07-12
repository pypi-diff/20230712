# Comparing `tmp/magnumnp-1.1.1.tar.gz` & `tmp/magnumnp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnumnp-1.1.1.tar", last modified: Tue Jun 13 16:00:24 2023, max compression
+gzip compressed data, was "magnumnp-1.1.2.tar", last modified: Wed Jul 12 11:07:30 2023, max compression
```

## Comparing `magnumnp-1.1.1.tar` & `magnumnp-1.1.2.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.279124 magnumnp-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-13 16:00:09.000000 magnumnp-1.1.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35069 2023-06-13 16:00:09.000000 magnumnp-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7495 2023-06-13 16:00:24.278124 magnumnp-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7002 2023-06-13 16:00:09.000000 magnumnp-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.275125 magnumnp-1.1.1/magnumnp/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.276125 magnumnp-1.1.1/magnumnp/common/
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/decorated_tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/material.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/state.py
--rw-rw-rw-   0 root         (0) root         (0)    38962 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/tabulate.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/time_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.277125 magnumnp-1.1.1/magnumnp/field_terms/
--rw-rw-rw-   0 root         (0) root         (0)     1597 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/anisotropy.py
--rw-rw-rw-   0 root         (0) root         (0)     8514 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demag.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demagPBC.py
--rw-rw-rw-   0 root         (0) root         (0)     6734 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demag_nonequidistant.py
--rw-rw-rw-   0 root         (0) root         (0)     8592 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/dmi.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/external.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/field_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     6437 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/oersted.py
--rw-rw-rw-   0 root         (0) root         (0)     4936 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/rkky.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/rux.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/spintorque.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.277125 magnumnp-1.1.1/magnumnp/loggers/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5829 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/scalar_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/solvers/
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/eigensolver.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/llg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/rkf45.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_ode.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_odeint.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/torchdiffeq.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/imaging_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.275125 magnumnp-1.1.1/magnumnp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7495 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1480 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 16:00:24.279124 magnumnp-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-06-13 16:00:19.000000 magnumnp-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.649649 magnumnp-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-12 11:07:15.000000 magnumnp-1.1.2/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35069 2023-07-12 11:07:15.000000 magnumnp-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-07-12 11:07:30.649649 magnumnp-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7002 2023-07-12 11:07:15.000000 magnumnp-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.645982 magnumnp-1.1.2/magnumnp/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.647816 magnumnp-1.1.2/magnumnp/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/decorated_tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/material.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/state.py
+-rw-rw-rw-   0 root         (0) root         (0)    38962 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/tabulate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/time_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/common/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.648732 magnumnp-1.1.2/magnumnp/field_terms/
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/anisotropy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8514 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/demag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/demagPBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6734 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/demag_nonequidistant.py
+-rw-rw-rw-   0 root         (0) root         (0)     8623 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/dmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/external.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/field_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6437 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/oersted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4936 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/rkky.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/rux.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/field_terms/spintorque.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.648732 magnumnp-1.1.2/magnumnp/loggers/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/loggers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5829 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/loggers/field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/loggers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/loggers/scalar_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.649649 magnumnp-1.1.2/magnumnp/solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/LBFGS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/eigensolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/llg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4089 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/minimize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.649649 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/rkf45.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/scipy_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/scipy_odeint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/ode_solvers/torchdiffeq.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/steepest_descent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/solvers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.649649 magnumnp-1.1.2/magnumnp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/utils/imaging_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-12 11:07:15.000000 magnumnp-1.1.2/magnumnp/utils/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:07:30.646899 magnumnp-1.1.2/magnumnp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-07-12 11:07:30.000000 magnumnp-1.1.2/magnumnp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-07-12 11:07:30.000000 magnumnp-1.1.2/magnumnp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 11:07:30.000000 magnumnp-1.1.2/magnumnp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-12 11:07:30.000000 magnumnp-1.1.2/magnumnp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-12 11:07:30.000000 magnumnp-1.1.2/magnumnp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 11:07:30.649649 magnumnp-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-07-12 11:07:25.000000 magnumnp-1.1.2/setup.py
```

### Comparing `magnumnp-1.1.1/LICENSE` & `magnumnp-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/PKG-INFO` & `magnumnp-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.1
+Version: 1.1.2
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 ![magnum.np](logo.png)
 
-magnum.np 1.1.1
+magnum.np 1.1.2
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -38,21 +38,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1SIdiiz8plOI0SG3HhxNJYOxbknG178Qo))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HazB7ydSYZKbtrQoPc9xE3U0d7uc-1Ir))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1OWMH0_qqxM73rB5gK5pi7nFRtO4nO_N8))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1kYudJgbuhGBrhTTFs_HzT68LxFcVkJPu))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1RXlrHUtB39aHtyp2btk3GNEBS0f5ZDFk))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1LgIX3o4e_6bww-RtIzJLX38QabUC5QMB))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/1mN56sxjhgPuLA5yB7z3skmZ2cy733BbS))
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
```

### Comparing `magnumnp-1.1.1/README.md` & `magnumnp-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![magnum.np](logo.png)
 
-magnum.np 1.1.1
+magnum.np 1.1.2
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -25,21 +25,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1SIdiiz8plOI0SG3HhxNJYOxbknG178Qo))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HazB7ydSYZKbtrQoPc9xE3U0d7uc-1Ir))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1OWMH0_qqxM73rB5gK5pi7nFRtO4nO_N8))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1kYudJgbuhGBrhTTFs_HzT68LxFcVkJPu))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1RXlrHUtB39aHtyp2btk3GNEBS0f5ZDFk))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1LgIX3o4e_6bww-RtIzJLX38QabUC5QMB))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/1mN56sxjhgPuLA5yB7z3skmZ2cy733BbS))
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
```

### Comparing `magnumnp-1.1.1/magnumnp/__init__.py` & `magnumnp-1.1.2/magnumnp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """magnum.np main module"""
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 import magnumnp.common.logging as logging
 import torch
 torch.set_default_dtype(torch.float64)
 
 # monkey patch torch versions < 2.0 or on Windows
 try:
```

### Comparing `magnumnp-1.1.1/magnumnp/common/__init__.py` & `magnumnp-1.1.2/magnumnp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/constants.py` & `magnumnp-1.1.2/magnumnp/common/constants.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/decorated_tensor.py` & `magnumnp-1.1.2/magnumnp/common/decorated_tensor.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/io.py` & `magnumnp-1.1.2/magnumnp/common/io.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/logging.py` & `magnumnp-1.1.2/magnumnp/common/logging.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/material.py` & `magnumnp-1.1.2/magnumnp/common/material.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/mesh.py` & `magnumnp-1.1.2/magnumnp/common/mesh.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/state.py` & `magnumnp-1.1.2/magnumnp/common/state.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/tabulate.py` & `magnumnp-1.1.2/magnumnp/common/tabulate.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/time_interpolator.py` & `magnumnp-1.1.2/magnumnp/common/time_interpolator.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/common/timer.py` & `magnumnp-1.1.2/magnumnp/common/timer.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/__init__.py` & `magnumnp-1.1.2/magnumnp/field_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/anisotropy.py` & `magnumnp-1.1.2/magnumnp/field_terms/anisotropy.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/demag.py` & `magnumnp-1.1.2/magnumnp/field_terms/demag.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/demagPBC.py` & `magnumnp-1.1.2/magnumnp/field_terms/demagPBC.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/demag_nonequidistant.py` & `magnumnp-1.1.2/magnumnp/field_terms/demag_nonequidistant.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/exchange.py` & `magnumnp-1.1.2/magnumnp/field_terms/exchange.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/external.py` & `magnumnp-1.1.2/magnumnp/field_terms/external.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/field_terms.py` & `magnumnp-1.1.2/magnumnp/field_terms/field_terms.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/oersted.py` & `magnumnp-1.1.2/magnumnp/field_terms/oersted.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/rkky.py` & `magnumnp-1.1.2/magnumnp/field_terms/rkky.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/rux.py` & `magnumnp-1.1.2/magnumnp/field_terms/rux.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 from magnumnp.common import timedmethod, constants
 import torch
 from .field_terms import LinearFieldTerm
 
 __all__ = ["AtomisticRuXExchangeField"]
 
 class AtomisticRuXExchangeField(LinearFieldTerm):
+    r"""
+    Noncollinear coupling caused by Ru-X Spacer Layers:
+    see: https://www.science.org/doi/full/10.1126/sciadv.abd8861
+         https://journals.aps.org/prb/abstract/10.1103/PhysRevB.106.054401
+
+    :param Jij: List of Coupling Constants
+    :type Jij: list, optional
+    """
     parameters = ["J"]
 
     def __init__(self, Jij, hom = None, **kwargs):
         self._hom = hom
         self._Jij = Jij
         super().__init__(**kwargs)
```

### Comparing `magnumnp-1.1.1/magnumnp/field_terms/spintorque.py` & `magnumnp-1.1.2/magnumnp/field_terms/spintorque.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/loggers/__init__.py` & `magnumnp-1.1.2/magnumnp/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/loggers/field_logger.py` & `magnumnp-1.1.2/magnumnp/loggers/field_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/loggers/logger.py` & `magnumnp-1.1.2/magnumnp/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/loggers/scalar_logger.py` & `magnumnp-1.1.2/magnumnp/loggers/scalar_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/__init__.py` & `magnumnp-1.1.2/magnumnp/solvers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,12 +16,18 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.solvers.eigensolver import *
 from magnumnp.solvers.llg import *
 from magnumnp.solvers.ode_solvers import *
 from magnumnp.solvers.string import *
+from magnumnp.solvers.minimize import *
+from magnumnp.solvers.steepest_descent import *
+from magnumnp.solvers.LBFGS import *
 
 __all__ = (eigensolver.__all__ +
            llg.__all__ +
            ode_solvers.__all__ +
-           string.__all__)
+           string.__all__ +
+           minimize.__all__ +
+           steepest_descent.__all__ +
+           LBFGS.__all__)
```

### Comparing `magnumnp-1.1.1/magnumnp/solvers/eigensolver.py` & `magnumnp-1.1.2/magnumnp/solvers/eigensolver.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/llg.py` & `magnumnp-1.1.2/magnumnp/solvers/llg.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/__init__.py` & `magnumnp-1.1.2/magnumnp/solvers/ode_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/rkf45.py` & `magnumnp-1.1.2/magnumnp/solvers/ode_solvers/rkf45.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_ode.py` & `magnumnp-1.1.2/magnumnp/solvers/ode_solvers/scipy_ode.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_odeint.py` & `magnumnp-1.1.2/magnumnp/solvers/ode_solvers/scipy_odeint.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/torchdiffeq.py` & `magnumnp-1.1.2/magnumnp/solvers/ode_solvers/torchdiffeq.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/solvers/string.py` & `magnumnp-1.1.2/magnumnp/solvers/string.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/utils/__init__.py` & `magnumnp-1.1.2/magnumnp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/utils/imaging_tools.py` & `magnumnp-1.1.2/magnumnp/utils/imaging_tools.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp/utils/misc.py` & `magnumnp-1.1.2/magnumnp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.1/magnumnp.egg-info/PKG-INFO` & `magnumnp-1.1.2/magnumnp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.1
+Version: 1.1.2
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 ![magnum.np](logo.png)
 
-magnum.np 1.1.1
+magnum.np 1.1.2
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -38,21 +38,21 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
-   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
-   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
-   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
-   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
-   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
-   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+   * [RKKY](demos/rkky/run.ipynb) ([Colab](https://colab.research.google.com/drive/1SIdiiz8plOI0SG3HhxNJYOxbknG178Qo))
+   * [Softmagnetic Composite](demos/softmagnetic_composite/run.ipynb) ([Colab](https://colab.research.google.com/drive/1HazB7ydSYZKbtrQoPc9xE3U0d7uc-1Ir))
+   * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1OWMH0_qqxM73rB5gK5pi7nFRtO4nO_N8))
+   * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1kYudJgbuhGBrhTTFs_HzT68LxFcVkJPu))
+   * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1RXlrHUtB39aHtyp2btk3GNEBS0f5ZDFk))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1LgIX3o4e_6bww-RtIzJLX38QabUC5QMB))
+   * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/1mN56sxjhgPuLA5yB7z3skmZ2cy733BbS))
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
```

### Comparing `magnumnp-1.1.1/magnumnp.egg-info/SOURCES.txt` & `magnumnp-1.1.2/magnumnp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,20 @@
 magnumnp/field_terms/rkky.py
 magnumnp/field_terms/rux.py
 magnumnp/field_terms/spintorque.py
 magnumnp/loggers/__init__.py
 magnumnp/loggers/field_logger.py
 magnumnp/loggers/logger.py
 magnumnp/loggers/scalar_logger.py
+magnumnp/solvers/LBFGS.py
 magnumnp/solvers/__init__.py
 magnumnp/solvers/eigensolver.py
 magnumnp/solvers/llg.py
+magnumnp/solvers/minimize.py
+magnumnp/solvers/steepest_descent.py
 magnumnp/solvers/string.py
 magnumnp/solvers/ode_solvers/__init__.py
 magnumnp/solvers/ode_solvers/rkf45.py
 magnumnp/solvers/ode_solvers/scipy_ode.py
 magnumnp/solvers/ode_solvers/scipy_odeint.py
 magnumnp/solvers/ode_solvers/torchdiffeq.py
 magnumnp/utils/__init__.py
```

### Comparing `magnumnp-1.1.1/setup.py` & `magnumnp-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='magnumnp',
-      version='v1.1.1',
+      version='v1.1.2',
       description='magnum.np finite-difference package for the solution of micromagnetic problems',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Florian Bruckner',
       author_email='florian.bruckner@univie.ac.at',
       url='http://gitlab.com/magnum.np/magnum.np',
       project_urls = {'Documentation': 'https://magnum.np.gitlab.io/magnum.np/',
```

