# Comparing `tmp/pyiron_base-0.6.1.dev0.tar.gz` & `tmp/pyiron_base-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.6.1.dev0.tar", last modified: Wed Jul  5 13:57:58 2023, max compression
+gzip compressed data, was "pyiron_base-0.6.2.tar", last modified: Wed Jul 12 13:55:34 2023, max compression
```

## Comparing `pyiron_base-0.6.1.dev0.tar` & `pyiron_base-0.6.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.943146 pyiron_base-0.6.1.dev0/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.943146 pyiron_base-0.6.1.dev0/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.947146 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.947146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.951146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.951146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.955146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.955146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.963146 pyiron_base-0.6.1.dev0/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.963146 pyiron_base-0.6.1.dev0/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.939146 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/generic/test_filehdfio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.402587 pyiron_base-0.6.2/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57264 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.402587 pyiron_base-0.6.2/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/generic/test_filehdfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/versioneer.py
```

### Comparing `pyiron_base-0.6.1.dev0/LICENSE` & `pyiron_base-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/PKG-INFO` & `pyiron_base-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.6.1.dev0
+Version: 0.6.2
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.1.dev0/README.rst` & `pyiron_base-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/__init__.py` & `pyiron_base-0.6.2/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/_tests.py` & `pyiron_base-0.6.2/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/control.py` & `pyiron_base-0.6.2/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/install.py` & `pyiron_base-0.6.2/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/ls.py` & `pyiron_base-0.6.2/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.6.2/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/rm.py` & `pyiron_base-0.6.2/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/cli/wrapper.py` & `pyiron_base-0.6.2/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/filetable.py` & `pyiron_base-0.6.2/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/generic.py` & `pyiron_base-0.6.2/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/jobtable.py` & `pyiron_base-0.6.2/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/manager.py` & `pyiron_base-0.6.2/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/performance.py` & `pyiron_base-0.6.2/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/database/tables.py` & `pyiron_base-0.6.2/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/factory.py` & `pyiron_base-0.6.2/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.6.2/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.6.2/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/object.py` & `pyiron_base-0.6.2/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.6.2/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/datamining.py` & `pyiron_base-0.6.2/pyiron_base/jobs/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.6.2/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/core.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Server object class which is connected to each job containing the technical details how the job is executed.
 """
 
+from concurrent.futures import Executor, Future
 from collections import OrderedDict
 import numbers
+import socket
+from typing import Union
+
 from pyiron_base.state import state
 from pyiron_base.jobs.job.extension.server.runmode import Runmode
-import socket
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -67,14 +70,22 @@
         .. attribute:: memory_limit
 
             the maximum amount of RAM allocated for the calculation in GB
 
         .. attribute:: new_hdf
 
             defines whether a subjob should be stored in the same HDF5 file or in a new one.
+
+        .. attribute:: executor
+
+            the executor can be used to execute the job object
+
+        .. attribute:: future
+
+            the concurrent.futures.Future object for monitoring the execution of the job object
     """
 
     def __init__(
         self,
         host=None,
         queue=None,
         cores=1,
@@ -87,14 +98,16 @@
         self._threads = threads
         self._active_queue = None
         self._gpus = gpus
         self._run_time = None
         self._memory_limit = None
         self._host = self._init_host(host=host)
         self._run_mode = Runmode()
+        self._executor: Union[Executor, None] = None
+        self._future: Union[Future, None] = None
 
         self.queue = queue
 
         self._user = state.settings.login_user
         self.run_mode = run_mode
 
         self._queue_id = None
@@ -229,26 +242,50 @@
         Args:
             qid (int): queue ID
         """
         self._queue_id = int(qid)
 
     @property
     def threads(self):
+        """
+        The number of threads selected for the current simulation
+
+        Returns:
+            (int): number of threads
+        """
         return self._threads
 
     @threads.setter
     def threads(self, number_of_threads):
+        """
+        The number of threads selected for the current simulation
+
+        Args:
+            number_of_threads (int): number of threads
+        """
         self._threads = number_of_threads
 
     @property
     def gpus(self):
+        """
+        Total number of GPUs to use for this calculation.
+
+        Returns:
+            int: Total number of GPUs to use for this calculation.
+        """
         return self._gpus
 
     @gpus.setter
     def gpus(self, number_of_gpus):
+        """
+        Total number of GPUs to use for this calculation.
+
+        Args:
+            number_of_gpus (int): Total number of GPUs to use for this calculation.
+        """
         self._gpus = number_of_gpus
 
     @property
     def cores(self):
         """
         The number of cores selected for the current simulation
 
@@ -346,25 +383,27 @@
 
     @property
     def run_mode(self):
         """
         Get the run mode of the job
 
         Returns:
-            (str/pyiron_base.server.runmode.Runmode): ['modal', 'non_modal', 'queue', 'manual']
+            (str/pyiron_base.server.runmode.Runmode): ['modal', 'non_modal', 'queue', 'manual', 'thread', 'worker',
+                        'interactive', 'interactive_non_modal', 'srun', 'executor']
         """
         return self._run_mode
 
     @run_mode.setter
     def run_mode(self, new_mode):
         """
         Set the run mode of the job
 
         Args:
-            new_mode (str): ['modal', 'non_modal', 'queue', 'manual']
+            new_mode (str): ['modal', 'non_modal', 'queue', 'manual', 'thread', 'worker', 'interactive',
+                        'interactive_non_modal', 'srun', 'executor']
         """
         self._run_mode.mode = new_mode
         if new_mode == "queue":
             if state.queue_adapter is None:
                 raise TypeError("No queue adapter defined.")
             if self._active_queue is None:
                 self.queue = state.queue_adapter.config["queue_primary"]
@@ -411,14 +450,68 @@
         List the available Job scheduler provided by the system.
 
         Returns:
             (pandas.DataFrame)
         """
         return self.view_queues()
 
+    @property
+    def executor(self) -> Union[Executor, None]:
+        """
+        Executor to execute the job object this server object is attached to in the background.
+
+        Returns:
+            concurrent.futures.Executor:
+        """
+        if not self.run_mode.executor and self._executor is not None:
+            self._executor = None
+        return self._executor
+
+    @executor.setter
+    def executor(self, exe: Union[Executor, None]):
+        """
+        Executor to execute the job object this server object is attached to in the background.
+
+        Args:
+            exe (concurrent.futures.Executor):
+        """
+        if isinstance(exe, Executor):
+            self.run_mode.executor = True
+        elif exe is None and self.run_mode.executor:
+            self.run_mode.modal = True
+        elif exe is not None:
+            raise TypeError(
+                "The executor has to be derived from the concurrent.futures.Executor class."
+            )
+        self._executor = exe
+
+    @property
+    def future(self) -> Union[Future, None]:
+        """
+        Python concurrent.futures.Future object to track the status of the execution of the job this server object is
+        attached to. This is an internal pyiron feature and most users never have to interact with the future object
+        directly.
+
+        Returns:
+             concurrent.futures.Future: future object to track the status of the execution
+        """
+        return self._future
+
+    @future.setter
+    def future(self, future_obj: Future):
+        """
+        Set a python concurrent.futures.Future object to track the status of the execution of the job this server object
+        is attached to. This is an internal pyiron feature and most users never have to interact with the future object
+        directly.
+
+        Args:
+            future_obj (concurrent.futures.Future): future object to track the status of the execution
+        """
+        self._future = future_obj
+
     @staticmethod
     def list_queues():
         """
         List the available Job scheduler provided by the system.
 
         Returns:
             (list)
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Set of functions to interact with the queuing system directly from within pyiron - optimized for the Sun grid engine.
 """
 
+from concurrent.futures import Future
 import pandas
 import time
 import numpy as np
 from pyiron_base.state import state
 from pyiron_base.utils.instance import static_isinstance
 from pyiron_base.jobs.job.extension.jobstatus import job_status_finished_lst
 
@@ -222,15 +223,20 @@
             for _ in range(max_iterations):
                 if state.database.database_is_disabled:
                     job.project.db.update()
                 job.refresh_job_status()
                 if job.status.string in job_status_finished_lst:
                     finished = True
                     break
-                time.sleep(interval_in_s)
+                elif isinstance(job.server.future, Future):
+                    job.server.future.result(timeout=interval_in_s)
+                    finished = job.server.future.done()
+                    break
+                else:
+                    time.sleep(interval_in_s)
             if not finished:
                 raise ValueError(
                     "Maximum iterations reached, but the job was not finished."
                 )
 
 
 def wait_for_jobs(
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,28 +24,35 @@
     "queue",
     "manual",
     "thread",
     "worker",
     "srun",
     "interactive",
     "interactive_non_modal",
+    "executor",
 ]
 
 
 class Runmode(object):
     """
     Run mode describes how the job is going to be executed:
     - modal: the interactive run mode
     - non_modal: sending the job to the background on the same machine
     - queue: submit the job to the queuing system
     - manual: let the user manually execute the job
     - thread: internal job mode, which is selected when the master job is send to the queue.
+    - worker: submit the job to the worker job for execution
     - interactive: the interactive run mode
+    - interactive_non_modal: the combination of the interactive and the non_modal mode
+    - srun: call SLURM to start the subprocess rather than starting it directly
+    - executor: python interface to execute jobs based on the concurrent.futures.Executor
+
     Args:
-        mode (str): ['modal', 'non_modal', 'queue', 'manual', 'thread', 'interactive']
+        mode (str): ['modal', 'non_modal', 'queue', 'manual', 'thread', 'worker', 'interactive',
+                     'interactive_non_modal', 'srun', 'executor']
     """
 
     def __init__(self, mode="modal"):
         super(Runmode, self).__init__()
         self._reset_mode()
         self.mode = mode
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Generic Job class extends the JobCore class with all the functionality to run the job object.
 """
 
+from concurrent.futures import Future
 from datetime import datetime
 import os
 import posixpath
 import signal
 import warnings
 
 from pyiron_base.state import state
@@ -133,20 +134,24 @@
         self._logger = state.logger
         self._executable = None
         if not state.database.database_is_disabled:
             self._status = JobStatus(db=project.db, job_id=self.job_id)
             self.refresh_job_status()
         elif os.path.exists(self.project_hdf5.file_name):
             initial_status = read_hdf5(
-                self.project_hdf5.file_name, self.job_name + "/status"
+                # in most cases self.project_hdf5.h5_path == / + self.job_name but not for child jobs of GenericMasters
+                self.project_hdf5.file_name,
+                self.project_hdf5.h5_path + "/status",
             )
             self._status = JobStatus(initial_status=initial_status)
             if "job_id" in self.list_nodes():
                 self._job_id = read_hdf5(
-                    self.project_hdf5.file_name, self.job_name + "/job_id"
+                    # in most cases self.project_hdf5.h5_path == / + self.job_name but not for child jobs of GenericMasters
+                    self.project_hdf5.file_name,
+                    self.project_hdf5.h5_path + "/job_id",
                 )
         else:
             self._status = JobStatus()
         self._restart_file_list = list()
         self._restart_file_dict = dict()
         self._exclude_nodes_hdf = list()
         self._exclude_groups_hdf = list()
@@ -426,14 +431,23 @@
             )
         elif state.database.database_is_disabled:
             self._status = JobStatus(
                 initial_status=read_hdf5(
                     self.project_hdf5.file_name, self.job_name + "/status"
                 )
             )
+        if (
+            isinstance(self.server.future, Future)
+            and not self.status.finished
+            and self.server.future.done()
+        ):
+            if self.server.future.cancelled():
+                self.status.aborted = True
+            else:
+                self.status.finished = True
 
     def clear_job(self):
         """
         Convenience function to clear job info after suspend. Mimics deletion of all the job info after suspend in a
         local test environment.
         """
         del self.__name__
@@ -462,14 +476,22 @@
         )
         copied_self.reset_job_id()
 
         # Reload object from HDF5 file
         _job_reload_after_copy(
             job=copied_self, delete_file_after_copy=delete_file_after_copy
         )
+
+        # Copy executor - it cannot be copied and is just linked instead
+        if self.server.executor is not None:
+            copied_self.server.executor = self.server.executor
+        if self.server.future is not None and not self.server.future.done():
+            raise RuntimeError(
+                "Jobs whose server has executor and future attributes cannot be copied unless the future is `done()`"
+            )
         return copied_self
 
     def _internal_copy_to(
         self,
         project=None,
         new_job_name=None,
         new_database_entry=True,
@@ -597,14 +619,26 @@
         return self.copy_to(
             project=project,
             new_job_name=new_job_name,
             input_only=True,
             new_database_entry=False,
         )
 
+    def remove(self, _protect_childs=True):
+        """
+        Remove the job - this removes the HDF5 file, all data stored in the HDF5 file an the corresponding database entry.
+
+        Args:
+            _protect_childs (bool): [True/False] by default child jobs can not be deleted, to maintain the consistency
+                                    - default=True
+        """
+        if isinstance(self.server.future, Future) and not self.server.future.done():
+            self.server.future.cancel()
+        super().remove(_protect_childs=_protect_childs)
+
     def remove_child(self):
         """
         internal function to remove command that removes also child jobs.
         Do never use this command, since it will destroy the integrity of your project.
         """
         _kill_child(job=self)
         super(GenericJob, self).remove_child()
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/path.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/runfunction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
+from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime
 import multiprocessing
 import os
 import posixpath
 import subprocess
 
+from jinja2 import Template
+
 from pyiron_base.utils.deprecate import deprecate
 from pyiron_base.jobs.job.wrapper import JobWrapper
 from pyiron_base.state import state
+from pyiron_base.utils.instance import static_isinstance
+
+
+try:
+    import flux.job
 
+    flux_available = True
+except ImportError:
+    flux_available = False
 
 """
 The function job.run() inside pyiron is executed differently depending on the status of the job object. This module 
 introduces the most general run functions and how they are selected. 
 
 If an additional parameter is provided, then a specific run function is executed: 
     repair: run_job_with_parameter_repair
@@ -35,14 +46,15 @@
     manual: run_job_with_runmode_manually
     modal: run_job_with_runmode_modal
     non_modal: run_job_with_runmode_non_modal
     interactive: run_job_with_runmode_interactive
     interactive_non_modal: run_job_with_runmode_interactive_non_modal
     queue: run_job_with_runmode_queue
     srun: run_job_with_runmode_srun
+    executor: run_job_with_runmode_executor
     thread: only affects children of a GenericMaster 
     worker: only affects children of a GenericMaster 
     
 Finally for jobs which call an external executable the execution is implemented in an function as well: 
     execute_job_with_external_executable
 """
 
@@ -98,14 +110,28 @@
         run_job_with_runmode_manually(job=job, _manually_print=True)
     elif job.server.run_mode.worker:
         run_job_with_runmode_manually(job=job, _manually_print=True)
     elif job.server.run_mode.modal:
         job.run_static()
     elif job.server.run_mode.srun:
         run_job_with_runmode_srun(job=job)
+    elif job.server.run_mode.executor:
+        if job.server.gpus is not None:
+            gpus_per_slot = int(job.server.gpus / job.server.cores)
+            if gpus_per_slot < 0:
+                raise ValueError(
+                    "Both job.server.gpus and job.server.cores have to be greater than zero."
+                )
+        else:
+            gpus_per_slot = None
+        run_job_with_runmode_executor(
+            job=job,
+            executor=job.server.executor,
+            gpus_per_slot=gpus_per_slot,
+        )
     elif (
         job.server.run_mode.non_modal
         or job.server.run_mode.thread
         or job.server.run_mode.worker
     ):
         run_job_with_runmode_non_modal(job=job)
     elif job.server.run_mode.queue:
@@ -427,14 +453,177 @@
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         universal_newlines=True,
     )
 
 
+def run_job_with_runmode_executor(job, executor, gpus_per_slot=None):
+    """
+    Introduced in Python 3.2 the concurrent.futures interface enables the asynchronous execution of python programs.
+    A function is submitted to the executor and a future object is returned. The future object is updated in the
+    background once the executor finished executing the function. The job.server.run_mode.executor implements the same
+    functionality for pyiron jobs. An executor is set as an attribute to the server object:
+
+    >>> job.server.executor = concurrent.futures.Executor()
+    >>> job.run()
+    >>> job.server.future.done()
+    False
+    >>> job.server.future.result()
+    >>> job.server.future.done()
+    True
+
+    When the job is executed by calling the run() function a future object is returned. The job is then executed in the
+    background and the user can use the future object to check the status of the job.
+
+    Args:
+        job (GenericJob): pyiron job object
+        executor (concurrent.futures.Executor): executor class which implements the executor interface defined in the
+                                                python concurrent.futures.Executor class.
+        gpus_per_slot (int): number of GPUs per MPI rank, typically 1
+    """
+
+    if static_isinstance(
+        obj=job,
+        obj_type="pyiron_base.jobs.master.generic.GenericMaster"
+        # The static check is used to avoid a circular import:
+        # runfunction -> GenericJob -> GenericMaster -> runfunction
+        # This smells a bit, so if a better architecture is found in the future, use it
+        # to avoid string-based specifications
+    ):
+        raise NotImplementedError(
+            "Currently job.server.run_mode.executor does not support GenericMaster jobs."
+        )
+    if flux_available and isinstance(executor, flux.job.FluxExecutor):
+        return run_job_with_runmode_executor_flux(
+            job=job, executor=executor, gpus_per_slot=gpus_per_slot
+        )
+    elif isinstance(executor, ProcessPoolExecutor):
+        return run_job_with_runmode_executor_futures(job=job, executor=executor)
+    else:
+        raise NotImplementedError(
+            "Currently only flux.job.FluxExecutor and concurrent.futures.ProcessPoolExecutor are supported."
+        )
+
+
+def run_job_with_runmode_executor_futures(job, executor):
+    """
+    Interface for the ProcessPoolExecutor implemented in the python standard library as part of the concurrent.futures
+    module. The ProcessPoolExecutor does not provide any resource management, so the user is responsible to keep track of
+    the number of compute cores in use, as over-subscription can lead to low performance.
+
+    The [ProcessPoolExecutor docs](https://docs.python.org/3/library/concurrent.futures.html#processpoolexecutor) state: "The __main__ module must be importable by worker subprocesses. This means that ProcessPoolExecutor will not work in the interactive interpreter." (i.e. Jupyter notebooks). For standard usage this is a non-issue, but for the edge case of job classes defined in-notebook (e.g. children of `PythonTemplateJob`), the using the ProcessPoolExecutor will result in errors. To resolve this, relocate such classes to an importable .py file.
+
+    >>> from concurrent.futures import ProcessPoolExecutor
+    >>> job.server.executor = ProcessPoolExecutor()
+    >>> job.server.future.done()
+    False
+    >>> job.server.future.result()
+    >>> job.server.future.done()
+    True
+
+    Args:
+        job (GenericJob): pyiron job object
+        executor (concurrent.futures.Executor): executor class which implements the executor interface defined in the
+                                                python concurrent.futures.Executor class.
+    """
+    if state.database.database_is_disabled:
+        file_path = job.project_hdf5.file_name + job.project_hdf5.h5_path
+        connection_string = None
+    else:
+        file_path = None
+        if state.database.using_local_database:
+            connection_string = str(job.project.db.conn.engine.url)
+        else:
+            connection_string = None
+
+    job.server.future = executor.submit(
+        multiprocess_wrapper,
+        working_directory=job.project_hdf5.working_directory,
+        job_id=job.job_id,
+        file_path=file_path,
+        debug=False,
+        connection_string=connection_string,
+    )
+
+
+def run_job_with_runmode_executor_flux(job, executor, gpus_per_slot=None):
+    """
+    Interface for the flux.job.FluxExecutor executor. Flux is a hierarchical resource management. It can either be used to
+    replace queuing systems like SLURM or be used as a user specific queuing system within an existing allocation.
+    pyiron provides two interfaces to flux, this executor interface as well as a traditional queuing system interface
+    via pysqa. This executor interface is designed for the development of asynchronous simulation protocols, while the
+    traditional queuing system interface simplifies the transition from other queuing systems like SLURM. The usuage
+    is analog to the concurrent.futures.Executor interface:
+
+    >>> from flux.job import FluxExecutor
+    >>> job.server.executor = FluxExecutor()
+    >>> job.run()
+    >>> job.server.future.done()
+    False
+    >>> job.server.future.result()
+    >>> job.server.future.done()
+    True
+
+    A word of caution - flux is currently only available on Linux, for all other operation systems the ProcessPoolExecutor
+    from the python standard library concurrent.futures is recommended. The advantage of flux over the ProcessPoolExecutor
+    is that flux takes over the resource management, like monitoring how many cores are available while with the
+    ProcessPoolExecutor this is left to the user.
+
+    Args:
+        job (GenericJob): pyiron job object
+        executor (flux.job.FluxExecutor): flux executor class which implements the executor interface defined in the
+                                      python concurrent.futures.Executor class.
+        gpus_per_slot (int): number of GPUs per MPI rank, typically 1
+
+     Returns:
+         concurrent.futures.Future: future object to develop asynchronous simulation protocols
+    """
+    if not flux_available:
+        raise ModuleNotFoundError(
+            "No module named 'flux'. Running in flux mode is only available on Linux;"
+            "For CPU jobs, please use `conda install -c conda-forge flux-core`; for "
+            "GPU support you will additionally need "
+            "`conda install -c conda-forge flux-sched libhwloc=*=cuda*`"
+        )
+    if not state.database.database_is_disabled:
+        executable_template = Template(
+            "#!/bin/bash\n",
+            "python -m pyiron_base.cli wrapper -p {{working_directory}} -j {{job_id}}",
+        )
+        exeuctable_str = executable_template.render(
+            working_directory=job.working_directory,
+            job_id=str(job.job_id),
+        )
+        job_name = "pi_" + str(job.job_id)
+    else:
+        executable_template = Template(
+            "#!/bin/bash\n",
+            "python -m pyiron_base.cli wrapper -p {{working_directory}} -f {{file_name}}{{h5_path}}",
+        )
+        exeuctable_str = executable_template.render(
+            working_directory=job.working_directory,
+            file_name=job.project_hdf5.file_name,
+            h5_path=job.project_hdf5.h5_path,
+        )
+        job_name = "pi_" + job.job_name
+
+    jobspec = flux.job.JobspecV1.from_batch_command(
+        jobname=job_name,
+        script=exeuctable_str,
+        num_nodes=1,
+        cores_per_slot=1,
+        gpus_per_slot=gpus_per_slot,
+        num_slots=job.server.cores,
+    )
+    jobspec.cwd = job.project_hdf5.working_directory
+    jobspec.environment = dict(os.environ)
+    return executor.submit(jobspec)
+
+
 def run_time_decorator(func):
     def wrapper(job):
         if not state.database.database_is_disabled and job.job_id is not None:
             job.project.db.item_update({"timestart": datetime.now()}, job.job_id)
             func(job)
             job.project.db.item_update(job._runtime(), job.job_id)
         else:
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/template.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/util.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.6.2/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/list.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,16 @@
         Args:
             convert_to_object (bool): load the full GenericJob object (default) or just the HDF5 / JobCore object
 
         Returns:
             yield: Yield of GenericJob or JobCore
         """
         project_working_directory = self.project.open(self.job_name + "_hdf5")
+        if state.database.database_is_disabled:
+            project_working_directory.db.update()
         for job_id in self._get_jobs_sorted():
             yield project_working_directory.load(
                 job_id, convert_to_object=convert_to_object
             )
 
     def _get_jobs_sorted(self):
         job_names = self.child_names.values()
@@ -524,15 +526,17 @@
         The run_static function is executed within the GenericJob class and depending on the run_mode of the
         Parallelmaster and its child jobs a more specific run function is selected.
         """
         self._logger.info("{} run parallel master (modal)".format(self.job_info_str))
         self.status.running = True
         self.submission_status.total_jobs = len(self._job_generator)
         self.submission_status.submitted_jobs = 0
-        if self.job_id and not self.is_finished():
+        if (
+            self.job_id or state.database.database_is_disabled
+        ) and not self.is_finished():
             self._logger.debug(
                 "{} child project {}".format(self.job_name, self.project.__str__())
             )
             job = next(self._job_generator, None)
             if job is not None:
                 if (
                     self.server.run_mode.non_modal
@@ -548,14 +552,18 @@
                     self._run_if_master_non_modal_child_non_modal(job)
                 elif (self.server.run_mode.modal and job.server.run_mode.modal) or (
                     self.server.run_mode.interactive and job.server.run_mode.interactive
                 ):
                     self._run_if_master_modal_child_modal(job)
                 elif self.server.run_mode.modal and job.server.run_mode.non_modal:
                     self._run_if_master_modal_child_non_modal(job)
+                elif job.server.run_mode.executor:
+                    raise NotImplementedError(
+                        "Currently ParallelMaster jobs do not support child jobs with job.server.run_mode.executor."
+                    )
                 else:
                     raise TypeError()
         else:
             self.status.collect = True
             self.run()
 
     def run_if_interactive(self):
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/serial.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,18 @@
                 self._run_if_master_queue(job)
             elif self.server.run_mode.non_modal and job.server.run_mode.non_modal:
                 self._run_if_master_non_modal_child_non_modal(job)
             elif self.server.run_mode.modal and job.server.run_mode.modal:
                 self._run_if_master_modal_child_modal(job)
             elif self.server.run_mode.modal and job.server.run_mode.non_modal:
                 self._run_if_master_modal_child_non_modal(job)
+            elif job.server.run_mode.executor:
+                raise NotImplementedError(
+                    "Currently SerialMasterBase jobs do not support child jobs with job.server.run_mode.executor."
+                )
             else:
                 raise TypeError()
         else:
             self.status.collect = True
             self.run()
 
     def set_goal(self, convergence_goal, **qwargs):
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.6.2/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/script.py` & `pyiron_base-0.6.2/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/jobs/worker.py` & `pyiron_base-0.6.2/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.6.2/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.6.2/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/data.py` & `pyiron_base-0.6.2/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/external.py` & `pyiron_base-0.6.2/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/generic.py` & `pyiron_base-0.6.2/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/gui.py` & `pyiron_base-0.6.2/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/maintenance.py` & `pyiron_base-0.6.2/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/path.py` & `pyiron_base-0.6.2/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.6.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/__init__.py` & `pyiron_base-0.6.2/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/install.py` & `pyiron_base-0.6.2/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/logger.py` & `pyiron_base-0.6.2/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/publications.py` & `pyiron_base-0.6.2/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.6.2/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/settings.py` & `pyiron_base-0.6.2/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/signal.py` & `pyiron_base-0.6.2/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/state/update.py` & `pyiron_base-0.6.2/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.6.2/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/filedata.py` & `pyiron_base-0.6.2/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/fileio.py` & `pyiron_base-0.6.2/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.6.2/pyiron_base/storage/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.6.2/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfio.py` & `pyiron_base-0.6.2/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.6.2/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.6.2/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/storage/parameters.py` & `pyiron_base-0.6.2/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/deprecate.py` & `pyiron_base-0.6.2/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/error.py` & `pyiron_base-0.6.2/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/instance.py` & `pyiron_base-0.6.2/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/jedi.py` & `pyiron_base-0.6.2/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/parser.py` & `pyiron_base-0.6.2/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/safetar.py` & `pyiron_base-0.6.2/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base/utils/units.py` & `pyiron_base-0.6.2/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.6.2/pyiron_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.6.1.dev0
+Version: 0.6.2
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.1.dev0/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.6.2/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/setup.py` & `pyiron_base-0.6.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,24 @@
                 ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'dill>=0.3.6',
         'gitpython>=3.1.31',
-        'h5io>=0.1.7',
+        'h5io>=0.1.8',
         'h5py>=3.9.0',
+        'jinja2>=3.1.2',
         'numpy>=1.24.3',
         'pandas>=2.0.3',
         'pint>=0.22',
         'psutil>=5.9.5',
         'pyfileindex>=0.0.11',
         'pysqa>=0.0.25',
-        'sqlalchemy>=2.0.17',
+        'sqlalchemy>=2.0.18',
         'tables>=3.8.0',
         'tqdm>=4.65.0',
         'traitlets>=5.9.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     entry_points={
```

### Comparing `pyiron_base-0.6.1.dev0/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.6.2/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/tests/test_testwithproject.py` & `pyiron_base-0.6.2/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/tests/test_toolkit.py` & `pyiron_base-0.6.2/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1.dev0/versioneer.py` & `pyiron_base-0.6.2/versioneer.py`

 * *Files identical despite different names*

