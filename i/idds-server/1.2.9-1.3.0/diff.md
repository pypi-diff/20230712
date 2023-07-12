# Comparing `tmp/idds-server-1.2.9.tar.gz` & `tmp/idds-server-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-server-1.2.9.tar", last modified: Sat Apr 29 19:24:56 2023, max compression
+gzip compressed data, was "idds-server-1.3.0.tar", last modified: Wed Jul 12 16:01:36 2023, max compression
```

## Comparing `idds-server-1.2.9.tar` & `idds-server-1.3.0.tar`

### file list

```diff
@@ -1,263 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.787537 idds-server-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 19:24:44.000000 idds-server-1.2.9/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-29 19:24:56.787537 idds-server-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 19:24:44.000000 idds-server-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.767536 idds-server-1.2.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-04-29 19:24:44.000000 idds-server-1.2.9/bin/idds-daemon
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-29 19:24:56.000000 idds-server-1.2.9/bin/idds.wsgi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-29 19:24:44.000000 idds-server-1.2.9/bin/idds.wsgi.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-29 19:24:44.000000 idds-server-1.2.9/bin/run-idds
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-29 19:24:44.000000 idds-server-1.2.9/bin/run-idds-fake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/config_default/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/gacl
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/httpd-idds-443-py39-cc7.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     3679 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/idds.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/panda.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/rucio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/supervisord_httpd.ini
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/supervisord_idds.ini
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/supervisord_iddsfake.ini
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/supervisord_logrotate.ini
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 19:24:44.000000 idds-server-1.2.9/config_default/supervisord_syslog-ng.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.767536 idds-server-1.2.9/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/alembic.ini.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/auth/auth.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.767536 idds-server-1.2.9/etc/idds/condor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/condor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/condor/client/00personal_condor.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/condor/server/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/condor/server/00personal_condor.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/idds.cfg.client.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     3946 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/idds.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/rest/gacl.template
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-29 19:24:56.000000 idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/rest/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/supervisord.d/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/supervisord.d/idds.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/idds/website/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/website/25-port443.conf
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/idds/website/25-port80.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/etc/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/oracle_11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/oracle_11_test.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/oracle_19.sql
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/oracle_update.sql
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/postgresql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/postgresql_init.sql
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 19:24:44.000000 idds-server-1.2.9/etc/sql/postgresql_update.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.767536 idds-server-1.2.9/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/lib/idds/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.771536 idds-server-1.2.9/lib/idds/agents/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/archive/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/archive/run_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/carrier/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/finisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/poller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    88606 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/carrier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/clerk/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/clerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53880 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/clerk/clerk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/baseagent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/common/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/cache/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/common/eventbus/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/baseeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/dbeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/eventbus.py
--rw-r--r--   0 runner    (1001) docker     (123)    21479 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/eventbus/msgeventbusbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/common/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/plugins/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/timerscheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/common/timertask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/conductor/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/conductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/conductor/conductor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/conductor/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/coordinator/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/coordinator/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/marshaller/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/marshaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/marshaller/marshaller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40926 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/agents/transporter/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/transporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/agents/transporter/transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.775536 idds-server-1.2.9/lib/idds/api/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/api/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/core/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/orm/base/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/orm/base/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/orm/base/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    51533 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    48600 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/orm/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.779537 idds-server-1.2.9/lib/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.783537 idds-server-1.2.9/lib/idds/rest/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/rest/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.787537 idds-server-1.2.9/lib/idds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/activelearning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/auth_test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/cacher_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/core_tests_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/core_tests_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/datacarousel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/doma_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/find_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/fix_content_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/fix_trasnform_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/hyperparameteropt_bayesian_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/hyperparameteropt_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/hyperparameteropt_docker_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/hyperparameteropt_docker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/hyperparameteropt_nevergrad_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/jsonload_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/kill_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/logs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/match_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/message_test1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/migrating_requests_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/panda_iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/panda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/performance_test_with_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/performance_test_with_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/relation_map_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/rest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/retry_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/run_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/scaling_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/split_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_big_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_datacarousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_domapanda.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_domapanda_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_domapanda_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_get_dn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_migrate_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_request_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_running_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_transform_collection_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_transform_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_workflow_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/test_workflow_condition_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-29 19:24:44.000000 idds-server-1.2.9/lib/idds/tests/trigger_release.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-server-1.2.9/lib/idds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.787537 idds-server-1.2.9/lib/idds_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-29 19:24:56.000000 idds-server-1.2.9/lib/idds_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-29 19:24:56.000000 idds-server-1.2.9/lib/idds_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:24:56.000000 idds-server-1.2.9/lib/idds_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-29 19:24:56.000000 idds-server-1.2.9/lib/idds_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:24:56.000000 idds-server-1.2.9/lib/idds_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:56.787537 idds-server-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-29 19:24:44.000000 idds-server-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.767536 idds-server-1.2.9/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:56.787537 idds-server-1.2.9/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/config_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/config_server
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/create_postgres_db.sh
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/destroy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/dump_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-29 19:24:53.000000 idds-server-1.2.9/tools/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/install_env_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/install_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/install_idds_full.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/install_packages.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/merge_configmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/merge_idds_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/setup_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 19:24:44.000000 idds-server-1.2.9/tools/env/setup_panda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.649930 idds-server-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-server-1.3.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 16:01:36.649930 idds-server-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-12 16:01:25.000000 idds-server-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-07-12 16:01:25.000000 idds-server-1.3.0/bin/idds-daemon
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-12 16:01:36.000000 idds-server-1.3.0/bin/idds.wsgi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 16:01:25.000000 idds-server-1.3.0/bin/idds.wsgi.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-07-12 16:01:25.000000 idds-server-1.3.0/bin/run-idds
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 16:01:25.000000 idds-server-1.3.0/bin/run-idds-fake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/gacl
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/httpd-idds-443-py39-cc7.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3679 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/idds.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/logrotate_daemon
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/logrotate_idds
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/panda.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/rucio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/supervisord_httpd.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/supervisord_idds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/supervisord_iddsfake.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/supervisord_logrotate.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-12 16:01:25.000000 idds-server-1.3.0/config_default/supervisord_syslog-ng.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/etc/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/alembic.ini.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/etc/idds/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/auth/auth.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.625929 idds-server-1.3.0/etc/idds/condor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/etc/idds/condor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/condor/client/00personal_condor.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/etc/idds/condor/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/condor/server/00personal_condor.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/idds.cfg.client.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3946 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/idds.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/etc/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/rest/gacl.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-12 16:01:36.000000 idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/rest/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/etc/idds/supervisord.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/supervisord.d/idds.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/etc/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/website/25-port443.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/idds/website/25-port80.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/etc/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/oracle_11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/oracle_11_test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/oracle_19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/oracle_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/postgresql_init.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-12 16:01:25.000000 idds-server-1.3.0/etc/sql/postgresql_update.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/archive/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/archive/run_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/carrier/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94427 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/carrier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/clerk/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/clerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67320 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/clerk/clerk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/baseagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.633930 idds-server-1.3.0/lib/idds/agents/common/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/cache/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/common/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/baseeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/dbeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/eventbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/eventbus/msgeventbusbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/common/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/plugins/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/timerscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/common/timertask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/conductor/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/conductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/conductor/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/conductor/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/coordinator/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/marshaller/marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40926 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/agents/transporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/transporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/agents/transporter/transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/api/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33651 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/core/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.637930 idds-server-1.3.0/lib/idds/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.641930 idds-server-1.3.0/lib/idds/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.641930 idds-server-1.3.0/lib/idds/orm/base/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.641930 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/orm/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.641930 idds-server-1.3.0/lib/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.641930 idds-server-1.3.0/lib/idds/rest/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/rest/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.649930 idds-server-1.3.0/lib/idds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/activelearning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/auth_test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/cacher_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/core_tests_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/core_tests_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/datacarousel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/doma_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/find_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/fix_content_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/fix_trasnform_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/hyperparameteropt_bayesian_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/hyperparameteropt_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/hyperparameteropt_docker_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/hyperparameteropt_docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/hyperparameteropt_nevergrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/jsonload_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/kill_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/logs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/match_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/message_test1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/migrating_requests_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/panda_iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/panda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/performance_test_with_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/performance_test_with_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/relation_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/rest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/retry_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/run_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/scaling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/set_throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/split_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_big_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_datacarousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_domapanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_domapanda_lsst_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_domapanda_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_domapanda_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_get_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_get_request_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_migrate_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_request_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_running_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_transform_collection_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_transform_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_workflow_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/test_workflow_condition_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-12 16:01:25.000000 idds-server-1.3.0/lib/idds/tests/trigger_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-server-1.3.0/lib/idds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.649930 idds-server-1.3.0/lib/idds_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 16:01:36.000000 idds-server-1.3.0/lib/idds_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-12 16:01:36.000000 idds-server-1.3.0/lib/idds_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:36.000000 idds-server-1.3.0/lib/idds_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 16:01:36.000000 idds-server-1.3.0/lib/idds_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:36.000000 idds-server-1.3.0/lib/idds_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:36.649930 idds-server-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-12 16:01:25.000000 idds-server-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.629929 idds-server-1.3.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:36.649930 idds-server-1.3.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/config_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/config_server
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/create_postgres_db.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/destroy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/dump_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 16:01:34.000000 idds-server-1.3.0/tools/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/install_env_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/install_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/install_idds_full.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/install_packages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/merge_configmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/merge_idds_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/setup_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-12 16:01:25.000000 idds-server-1.3.0/tools/env/setup_panda.sh
```

### Comparing `idds-server-1.2.9/LICENSE.rst` & `idds-server-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/PKG-INFO` & `idds-server-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.2.9
+Version: 1.3.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.2.9/bin/idds-daemon` & `idds-server-1.3.0/bin/idds-daemon`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/bin/idds.wsgi` & `idds-server-1.3.0/bin/idds.wsgi`

 * *Files 22% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # - Wen Guan, <wen.guan@cern.ch>, 2019
 
 """----------------------
    Web service startup
 ----------------------"""
 
 import os
-os.environ['IDDS_CONFIG'] = '/opt/hostedtoolcache/Python/3.11.3/x64/etc/idds/idds.cfg'
+os.environ['IDDS_CONFIG'] = '/opt/hostedtoolcache/Python/3.11.4/x64/etc/idds/idds.cfg'
 
 from idds.rest.v1.app import create_app  # noqa: E402
 
 
 application = create_app()
```

### Comparing `idds-server-1.2.9/bin/idds.wsgi.template` & `idds-server-1.3.0/bin/idds.wsgi.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/bin/run-idds` & `idds-server-1.3.0/bin/run-idds`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/alembic.ini` & `idds-server-1.3.0/config_default/alembic.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/gacl` & `idds-server-1.3.0/config_default/gacl`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/httpd-idds-443-py39-cc7.conf` & `idds-server-1.3.0/config_default/httpd-idds-443-py39-cc7.conf`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 <VirtualHost *:8443>
     # ServerName aipanda182.cern.ch:8443
     ServerAdmin wguan@cern.ch
 
     SSLEngine on
     SSLCertificateFile /etc/grid-security/hostcert.pem
     SSLCertificateKeyFile /etc/grid-security/hostkey.pem
+    SSLCertificateChainFile /etc/grid-security/chain.pem
     SSLCACertificatePath /etc/grid-security/certificates
     SSLCARevocationPath /etc/grid-security/certificates
     SSLVerifyClient optional
     SSLVerifyDepth 16
     SSLOptions +StdEnvVars +ExportCertData
 
     # CERN security recommendation to only allow the seven strongest ssl ciphers
```

### Comparing `idds-server-1.2.9/config_default/idds.cfg` & `idds-server-1.3.0/config_default/idds.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/rucio.cfg` & `idds-server-1.3.0/config_default/rucio.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/supervisord_httpd.ini` & `idds-server-1.3.0/config_default/supervisord_httpd.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/supervisord_idds.ini` & `idds-server-1.3.0/config_default/supervisord_idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/supervisord_iddsfake.ini` & `idds-server-1.3.0/config_default/supervisord_iddsfake.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/config_default/supervisord_logrotate.ini` & `idds-server-1.3.0/config_default/supervisord_syslog-ng.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-[program:idds-server]
-environment =
-    RUCIO_HOME=/opt/idds/,
-    RUCIO_ACCOUNT=pilot,
-    RUCIO_AUTH_TYPE=x509_proxy,
-    X509_USER_PROXY=/opt/idds/config/x509up
+[program:syslog-ng]
 ;command=/opt/idds/bin/run-idds
 ;command=bash -c "source /etc/profile.d/conda.sh && conda activate /opt/idds && /opt/idds/bin/run-idds"
 ;command=bash -c "trap 'kill -TERM $PID; wait $PID' TERM && source /etc/profile.d/conda.sh && conda activate /opt/idds && /opt/idds/bin/run-idds && PID=$! && wait $PID"
-command=/usr/sbin/logrotate -d /etc/logrotate.d/idds
+command=/usr/sbin/syslog-ng -F --no-caps --persist-file=/var/log/idds/syslog-ng.persist -p /var/log/idds/syslog-ng.pid
 # process_name=%(process_num)02d
 # user=atlpan
 childlogdir=/var/log/idds
 stdout_logfile=/var/log/idds/%(program_name)s-stdout.log
 stderr_logfile=/var/log/idds/%(program_name)s-stderr.log
+# stdout_logfile=/dev/stdout
+# stderr_logfile=/dev/stderr
 stdout_logfile_maxbytes=2GB
 stderr_logfile_maxbytes=2GB
-stdout_logfile_backups=5
-stderr_logfile_backups=5
-redirect_stderr=false
+stdout_logfile_backups=1
+stderr_logfile_backups=1
+redirect_stderr=true
+redirect_stdout=true
 autorestart=true
 stopsignal=TERM
 stopasgroup=true
 exitcodes=1
```

### Comparing `idds-server-1.2.9/etc/idds/alembic.ini.template` & `idds-server-1.3.0/etc/idds/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/auth/auth.cfg.template` & `idds-server-1.3.0/etc/idds/auth/auth.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/condor/client/00personal_condor.config` & `idds-server-1.3.0/etc/idds/condor/client/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/condor/server/00personal_condor.config` & `idds-server-1.3.0/etc/idds/condor/server/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/idds.cfg.client.template` & `idds-server-1.3.0/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/idds.cfg.template` & `idds-server-1.3.0/etc/idds/idds.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/rest/gacl.template` & `idds-server-1.3.0/etc/idds/rest/gacl.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template` & `idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template` & `idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template` & `idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 # # LoadModule dir_module           /usr/lib64/httpd/modules/mod_dir.so
 # # LoadModule alias_module         /usr/lib64/httpd/modules/mod_alias.so
 # # LoadModule cgi_module           /usr/lib64/httpd/modules/mod_cgi.so
 
 # External modules
 LoadModule gridsite_module /usr/lib64/httpd/modules/mod_gridsite.so
 #LoadModule wsgi_module /usr/lib64/httpd/modules/mod_wsgi.so
-LoadModule wsgi_module /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
+LoadModule wsgi_module /opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
 
-WSGIPythonHome /opt/hostedtoolcache/Python/3.11.3/x64
-WSGIPythonPath /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
+WSGIPythonHome /opt/hostedtoolcache/Python/3.11.4/x64
+WSGIPythonPath /opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages
 
 <IfModule mod_wsgi.c>
-    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.3/x64 python-path=/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
+    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.4/x64 python-path=/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages
     WSGIProcessGroup idds_daemon
     WSGIApplicationGroup %GLOBAL
-    WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.3/x64/bin/idds.wsgi
+    WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.4/x64/bin/idds.wsgi
     # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
     WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
     # WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
     WSGIPassAuthorization On
 </IfModule>
 
 Listen 443
@@ -71,18 +71,18 @@
     SSLHonorCipherOrder on
 
     LogLevel debug
     ErrorLog /var/log/idds/httpd_error_log
     TransferLog /var/log/idds/httpd_access_log
 
     <IfModule mod_wsgi.c>
-        WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.3/x64 python-path=/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
+        WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.4/x64 python-path=/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages
         WSGIProcessGroup idds_daemon
         WSGIApplicationGroup %GLOBAL
-        WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.3/x64/bin/idds.wsgi
+        WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.4/x64/bin/idds.wsgi
         # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
         # WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
         WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
         WSGIPassAuthorization On
     </IfModule>
 
     # Proxy authentication via mod_gridsite
@@ -101,21 +101,21 @@
         GridSiteDNlists /etc/grid-security/dn-lists/
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
         GridSiteACLPath /opt/idds/etc/idds/rest/gacl
         # GridSiteMethods GET
     </LocationMatch>
 
-    <Directory /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages>
+    <Directory /opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages>
         # Order deny,allow
         # Allow from all
         # Require all granted
     </Directory>
 
-    <Directory /opt/hostedtoolcache/Python/3.11.3/x64/bin>
+    <Directory /opt/hostedtoolcache/Python/3.11.4/x64/bin>
         Order deny,allow
         Allow from all
         Require all granted
     </Directory>
 
     <Directory /opt/idds/website/data>
         Order deny,allow
```

### Comparing `idds-server-1.2.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template` & `idds-server-1.3.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/rest/ssl.conf` & `idds-server-1.3.0/etc/idds/rest/ssl.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/supervisord.d/idds.ini` & `idds-server-1.3.0/etc/idds/supervisord.d/idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/idds/website/25-port443.conf` & `idds-server-1.3.0/etc/idds/website/25-port443.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/sql/oracle_11.sql` & `idds-server-1.3.0/etc/sql/oracle_11.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/sql/oracle_11_test.sql` & `idds-server-1.3.0/etc/sql/oracle_11_test.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/sql/oracle_19.sql` & `idds-server-1.3.0/etc/sql/oracle_19.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/sql/oracle_update.sql` & `idds-server-1.3.0/etc/sql/oracle_update.sql`

 * *Files 2% similar despite different names*

```diff
@@ -395,7 +395,50 @@
 alter table HEALTH add (status NUMBER(2));
 alter table contents_update add content_metadata CLOB;
 alter table health modify payload VARCHAR2(2048);
 
 
 --- 2023.03.29
 alter table contents_update add fetch_status NUMBER(2) DEFAULT 0;
+
+
+-- 2023.05.18
+alter table requests add site VARCHAR2(50);
+CREATE INDEX REQUESTS_STATUS_SITE ON requests  (status, site, request_id) COMPRESS 3 LOCAL;
+
+alter table transforms add site VARCHAR2(50);
+CREATE INDEX TRANSFORMS_STATUS_SITE ON transforms  (status, site, request_id, transform_id) COMPRESS 3 LOCAL;
+
+alter table processings add site VARCHAR2(50);
+CREATE INDEX PROCESSINGS_STATUS_SITE ON processings  (status, site, request_id, transform_id, processing_id) COMPRESS 3 LOCAL;
+
+alter table messages add fetching_id NUMBER(12);
+
+
+CREATE SEQUENCE THROTTLER_ID_SEQ MINVALUE 1 INCREMENT BY 1 START WITH 1 NOCACHE ORDER NOCYCLE GLOBAL;
+CREATE TABLE Throttlers
+(
+    throttler_id NUMBER(12) DEFAULT ON NULL THROTTLER_ID_SEQ.NEXTVAL constraint THROTTLER_ID_NN NOT NULL,
+    site VARCHAR2(50),
+    status NUMBER(2),
+    num_requests NUMBER(12),
+    num_transforms NUMBER(12),
+    num_processings NUMBER(12),
+    new_contents NUMBER(12),
+    queue_contents NUMBER(12),
+    created_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    updated_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    others CLOB,
+    CONSTRAINT THROTTLER_PK PRIMARY KEY (throttler_id), -- USING INDEX LOCAL,
+    CONSTRAINT THROTTLER_SITE_UQ UNIQUE (site)
+);
+
+alter table Messages add (poll_period INTERVAL DAY TO SECOND DEFAULT '00 00:05:00');
+
+
+--- 20230626
+alter table contents add (external_coll_id NUMBER(12), external_content_id NUMBER(12), external_event_id NUMBER(12), external_event_status NUMBER(2));
+
+alter table contents add (sub_map_id NUMBER(12) default 0);
+alter table contents add (dep_sub_map_id NUMBER(12) default 0);
+alter table contents drop constraint CONTENT_ID_UQ;
+alter table contents add constraint CONTENT_ID_UQ UNIQUE (transform_id, coll_id, map_id, sub_map_id, dep_sub_map_id, content_relation_type, name, min_id, max_id) USING INDEX LOCAL;
```

### Comparing `idds-server-1.2.9/etc/sql/postgresql.sql` & `idds-server-1.3.0/etc/sql/postgresql.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/etc/sql/postgresql_init.sql` & `idds-server-1.3.0/etc/sql/postgresql_init.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/archive/archiver.py` & `idds-server-1.3.0/lib/idds/agents/archive/archiver.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/archive/run_archive.py` & `idds-server-1.3.0/lib/idds/agents/archive/run_archive.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/finisher.py` & `idds-server-1.3.0/lib/idds/agents/carrier/finisher.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/poller.py` & `idds-server-1.3.0/lib/idds/agents/carrier/poller.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         else:
             self.new_poll_period = int(self.new_poll_period)
         if not hasattr(self, 'update_poll_period') or not self.update_poll_period:
             self.update_poll_period = self.poll_period
         else:
             self.update_poll_period = int(self.update_poll_period)
 
+        if not hasattr(self, 'update_poll_period_for_new_task') or not self.update_poll_period_for_new_task:
+            self.update_poll_period_for_new_task = 180
+        else:
+            self.update_poll_period_for_new_task = int(self.update_poll_period_for_new_task)
+
         if hasattr(self, 'poll_period_increase_rate'):
             self.poll_period_increase_rate = float(self.poll_period_increase_rate)
         else:
             self.poll_period_increase_rate = 2
 
         if hasattr(self, 'max_new_poll_period'):
             self.max_new_poll_period = int(self.max_new_poll_period)
@@ -150,30 +155,33 @@
         work_tag_attribute_value = None
         if work_tag:
             work_tag_attribute = work_tag + "_" + attribute
             if hasattr(self, work_tag_attribute):
                 work_tag_attribute_value = int(getattr(self, work_tag_attribute))
         return work_tag_attribute_value
 
-    def load_poll_period(self, processing, parameters):
+    def load_poll_period(self, processing, parameters, new=False):
         proc = processing['processing_metadata']['processing']
         work = proc.work
         work_tag = work.get_work_tag()
 
         work_tag_new_poll_period = self.get_work_tag_attribute(work_tag, "new_poll_period")
         if work_tag_new_poll_period:
             parameters['new_poll_period'] = work_tag_new_poll_period
         elif self.new_poll_period and processing['new_poll_period'] != self.new_poll_period:
             parameters['new_poll_period'] = self.new_poll_period
 
-        work_tag_update_poll_period = self.get_work_tag_attribute(work_tag, "update_poll_period")
-        if work_tag_update_poll_period:
-            parameters['update_poll_period'] = work_tag_update_poll_period
-        elif self.update_poll_period and processing['update_poll_period'] != self.update_poll_period:
-            parameters['update_poll_period'] = self.update_poll_period
+        if new:
+            parameters['update_poll_period'] = self.update_poll_period_for_new_task
+        else:
+            work_tag_update_poll_period = self.get_work_tag_attribute(work_tag, "update_poll_period")
+            if work_tag_update_poll_period:
+                parameters['update_poll_period'] = work_tag_update_poll_period
+            elif self.update_poll_period and processing['update_poll_period'] != self.update_poll_period:
+                parameters['update_poll_period'] = self.update_poll_period
         return parameters
 
     def get_log_prefix(self, processing):
         return "<request_id=%s,transform_id=%s,processing_id=%s>" % (processing['request_id'],
                                                                      processing['transform_id'],
                                                                      processing['processing_id'])
```

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/receiver.py` & `idds-server-1.3.0/lib/idds/agents/carrier/receiver.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.update_processing_interval = update_processing_interval
         if self.update_processing_interval:
             self.update_processing_interval = int(self.update_processing_interval)
         else:
             self.update_processing_interval = 300
 
         self.mode = mode
+        self.selected = None
         self.selected_receiver = None
 
         self.log_prefix = ''
 
         self._lock = threading.RLock()
 
     def __del__(self):
@@ -75,16 +76,26 @@
 
     def stop_receiver(self):
         if hasattr(self, 'receiver') and self.receiver:
             self.logger.info("Stopping receiver: %s" % self.receiver)
             self.receiver.stop()
             self.receiver = None
 
-    def is_receiver_started(self):
+    def suspend_receiver(self):
         if hasattr(self, 'receiver') and self.receiver:
+            self.logger.info("Stopping receiver: %s" % self.receiver)
+            self.receiver.suspend()
+
+    def resume_receiver(self):
+        if hasattr(self, 'receiver') and self.receiver:
+            self.logger.info("Resuming receiver: %s" % self.receiver)
+            self.receiver.resume()
+
+    def is_receiver_started(self):
+        if hasattr(self, 'receiver') and self.receiver and self.receiver.is_processing():
             return True
         return False
 
     def get_num_queued_messages(self):
         return self.message_queue.qsize()
 
     def get_output_messages(self):
@@ -105,17 +116,23 @@
                 self.logger.error("Failed to get output messages: %s, %s" % (error, traceback.format_exc()))
             if msgs:
                 total_msgs = self.get_num_queued_messages()
                 self.logger.info("process_messages: Get %s messages, left %s messages" % (len(msgs), total_msgs))
             return msgs
 
     def is_selected(self):
+        selected = None
         if not self.selected_receiver:
-            return True
-        return self.is_self(self.selected_receiver)
+            selected = True
+        else:
+            selected = self.is_self(self.selected_receiver)
+        if self.selected is None or self.selected != selected:
+            self.logger.info("is_selected changed from %s to %s" % (self.selected, selected))
+        self.selected = selected
+        return self.selected
 
     def monitor_receiver(self):
         if self.mode == "single":
             self.logger.info("Receiver single mode")
             self.selected_receiver = core_health.select_agent(name='Receiver', newer_than=self.heartbeat_delay * 2)
             self.logger.debug("Selected receiver: %s" % self.selected_receiver)
 
@@ -238,27 +255,29 @@
 
             log_prefix = "<Message>"
             self.log_prefix = log_prefix
 
             # [self.executors.submit(self.worker, log_prefix) for i in range(self.executors.get_max_workers())]
             self.init_event_function_map()
 
+            self.start_receiver()
+
             while not self.graceful_stop.is_set():
                 try:
                     self.execute_schedules()
 
                     time_start = time.time()
 
                     if self.is_selected():
                         if not self.is_receiver_started():
-                            self.start_receiver()
+                            self.resume_receiver()
 
                     if not self.is_selected():
                         if self.is_receiver_started():
-                            self.stop_receiver()
+                            self.suspend_receiver()
 
                     msg = self.get_output_messages()
                     if msg:
                         event = MessageEvent(message=msg)
                         self.event_bus.send(event)
 
                     if not msg:
```

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/submitter.py` & `idds-server-1.3.0/lib/idds/agents/carrier/submitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             if not status:
                 raise exceptions.ProcessSubmitFailed(str(errors))
 
             parameters = {'status': ProcessingStatus.Submitting,
                           'substatus': ProcessingStatus.Submitting,
                           'locking': ProcessingLocking.Idle,
                           'processing_metadata': processing['processing_metadata']}
-            parameters = self.load_poll_period(processing, parameters)
+            parameters = self.load_poll_period(processing, parameters, new=True)
 
             proc = processing['processing_metadata']['processing']
             if proc.submitted_at:
                 if not processing['submitted_at'] or processing['submitted_at'] < proc.submitted_at:
                     parameters['submitted_at'] = proc.submitted_at
 
             # if processing['processing_metadata'] and 'processing' in processing['processing_metadata']:
```

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/trigger.py` & `idds-server-1.3.0/lib/idds/agents/carrier/trigger.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/carrier/utils.py` & `idds-server-1.3.0/lib/idds/agents/carrier/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,18 @@
                'bytes': input_content['bytes'],
                'adler32': input_content['adler32'],
                'content_metadata': input_content['content_metadata']}
     if content['min_id'] is None:
         content['min_id'] = 0
     if content['max_id'] is None:
         content['max_id'] = 0
+    if 'sub_map_id' in input_content:
+        content['sub_map_id'] = input_content['sub_map_id']
+    if 'dep_sub_map_id' in input_content:
+        content['dep_sub_map_id'] = input_content['dep_sub_map_id']
     return content
 
 
 def is_process_terminated(processing_status):
     if processing_status in [ProcessingStatus.Finished, ProcessingStatus.Failed,
                              ProcessingStatus.SubFinished, ProcessingStatus.Cancelled,
                              ProcessingStatus.Suspended, ProcessingStatus.Expired,
@@ -173,48 +177,29 @@
     input_coll_ids = get_collection_ids(input_collections)
     output_coll_ids = get_collection_ids(output_collections)
     log_coll_ids = get_collection_ids(log_collections)
 
     mapped_input_output_maps = core_transforms.get_transform_input_output_maps(transform_id,
                                                                                input_coll_ids=input_coll_ids,
                                                                                output_coll_ids=output_coll_ids,
-                                                                               log_coll_ids=log_coll_ids)
+                                                                               log_coll_ids=log_coll_ids,
+                                                                               with_sub_map_id=work.with_sub_map_id())
 
     # work_name_to_coll_map = core_transforms.get_work_name_to_coll_map(request_id=transform['request_id'])
     # work.set_work_name_to_coll_map(work_name_to_coll_map)
 
     # new_input_output_maps = work.get_new_input_output_maps(mapped_input_output_maps)
     return mapped_input_output_maps
 
 
 def get_ext_contents(transform_id, work):
     contents_ids = core_catalog.get_contents_ext_ids(transform_id=transform_id)
     return contents_ids
 
 
-def resolve_input_dependency_id(request_id, new_input_dep_coll_ids, new_input_dependency_contents, logger=None, log_prefix=''):
-    logger = get_logger(logger)
-
-    logger.info(log_prefix + "resolve_input_dependency_id: new_input_dep_coll_ids: %s" % (str(new_input_dep_coll_ids)))
-    logger.info(log_prefix + "resolve_input_dependency_id: len(new_input_dependency_contents): %s" % len(new_input_dependency_contents))
-
-    if new_input_dep_coll_ids:
-        contents = core_catalog.get_contents_by_coll_id_status(coll_id=new_input_dep_coll_ids)
-        content_name_id_map = {}
-        for content in contents:
-            if content['coll_id'] not in content_name_id_map:
-                content_name_id_map[content['coll_id']] = {}
-            content_name_id_map[content['coll_id']][content['name']] = content['content_id']
-        for content in new_input_dependency_contents:
-            if content['coll_id'] in content_name_id_map and content['name'] in content_name_id_map[content['coll_id']]:
-                content_dep_id = content_name_id_map[content['coll_id']][content['name']]
-                content['content_dep_id'] = content_dep_id
-    return new_input_dependency_contents
-
-
 def get_new_contents(request_id, transform_id, workload_id, new_input_output_maps, logger=None, log_prefix=''):
     logger = get_logger(logger)
 
     logger.debug(log_prefix + "get_new_contents")
     new_input_contents, new_output_contents, new_log_contents = [], [], []
     new_input_dependency_contents = []
     new_input_dep_coll_ids = []
@@ -235,15 +220,14 @@
         for output_content in outputs:
             content = get_new_content(request_id, transform_id, workload_id, map_id, output_content, content_relation_type=ContentRelationType.Output)
             new_output_contents.append(content)
         for log_content in logs:
             content = get_new_content(request_id, transform_id, workload_id, map_id, log_content, content_relation_type=ContentRelationType.Log)
             new_log_contents.append(content)
 
-    # new_input_dependency_contents = resolve_input_dependency_id(request_id, new_input_dep_coll_ids, new_input_dependency_contents, logger=logger, log_prefix=log_prefix)
     return new_input_contents, new_output_contents, new_log_contents, new_input_dependency_contents
 
 
 def get_update_content(content):
     updated_content = {'content_id': content['content_id'],
                        'status': content['substatus'],
                        'substatus': content['substatus']}
@@ -257,42 +241,48 @@
 
     for map_id in input_output_maps:
         inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
         inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
         outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
         # logs = input_output_maps[map_id]['logs'] if 'logs' in input_output_maps[map_id] else []
 
-        content_update_status = None
-        if is_all_contents_available(inputs_dependency):
-            # logger.debug("all input dependency available: %s, inputs: %s" % (str(inputs_dependency), str(inputs)))
-            content_update_status = ContentStatus.Available
-        elif is_all_contents_terminated(inputs_dependency):
-            # logger.debug("all input dependency terminated: %s, inputs: %s, outputs: %s" % (str(inputs_dependency), str(inputs), str(outputs)))
-            content_update_status = ContentStatus.Missing
-
-        if content_update_status:
-            for content in inputs:
-                content['substatus'] = content_update_status
-                if content['status'] != content['substatus']:
-                    updated_content, content = get_update_content(content)
-                    updated_contents.append(updated_content)
-                    updated_input_contents_full.append(content)
-        if content_update_status in [ContentStatus.Missing]:
-            for content in outputs:
-                content['substatus'] = content_update_status
+        input_output_sub_maps = get_input_output_sub_maps(inputs, outputs, inputs_dependency)
+        for sub_map_id in input_output_sub_maps:
+            inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
+            outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
+            inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
+
+            content_update_status = None
+            if is_all_contents_available(inputs_dependency_sub):
+                # logger.debug("all input dependency available: %s, inputs: %s" % (str(inputs_dependency), str(inputs)))
+                content_update_status = ContentStatus.Available
+            elif is_all_contents_terminated(inputs_dependency_sub):
+                # logger.debug("all input dependency terminated: %s, inputs: %s, outputs: %s" % (str(inputs_dependency), str(inputs), str(outputs)))
+                content_update_status = ContentStatus.Missing
+
+            if content_update_status:
+                for content in inputs_sub:
+                    content['substatus'] = content_update_status
+                    if content['status'] != content['substatus']:
+                        updated_content, content = get_update_content(content)
+                        updated_contents.append(updated_content)
+                        updated_input_contents_full.append(content)
+            if content_update_status in [ContentStatus.Missing]:
+                for content in outputs_sub:
+                    content['substatus'] = content_update_status
+                    if content['status'] != content['substatus']:
+                        updated_content, content = get_update_content(content)
+                        updated_contents.append(updated_content)
+                        updated_output_contents_full.append(content)
+
+            for content in outputs_sub:
                 if content['status'] != content['substatus']:
                     updated_content, content = get_update_content(content)
                     updated_contents.append(updated_content)
                     updated_output_contents_full.append(content)
-
-        for content in outputs:
-            if content['status'] != content['substatus']:
-                updated_content, content = get_update_content(content)
-                updated_contents.append(updated_content)
-                updated_output_contents_full.append(content)
         return updated_contents, updated_input_contents_full, updated_output_contents_full
 
 
 def get_message_type(work_type, input_type='file'):
     work_type_value = str(work_type.value)
     if work_type_value not in TransformType2MessageTypeMap:
         return TransformType2MessageTypeMap['0'][input_type]
@@ -311,18 +301,23 @@
     for file in files:
         file_status = file['substatus'].name
         if file['substatus'] == ContentStatus.FakeAvailable:
             file_status = ContentStatus.Available.name
         file_message = {'scope': file['scope'],
                         'name': file['name'],
                         'path': file['path'],
+                        'map_id': file['map_id'],
+                        'content_id': file['content_id'] if 'content_id' in file else None,
+                        'external_coll_id': file['external_coll_id'] if 'external_coll_id' in file else None,
+                        'external_content_id': file['external_content_id'] if 'external_content_id' in file else None,
                         'status': file_status}
         files_message.append(file_message)
     msg_content = {'msg_type': i_msg_type_str.value,
                    'request_id': request_id,
+                   'transform_id': transform_id,
                    'workload_id': workload_id,
                    'relation_type': relation_type,
                    'files': files_message}
     num_msg_content = len(files_message)
     return i_msg_type, msg_content, num_msg_content
 
 
@@ -337,14 +332,15 @@
             # content_map[content['content_id']] = content
             output_contents += outputs
 
     files_message = core_catalog.combine_contents_ext(output_contents, files, with_status_name=True)
     msg_content = {'msg_type': i_msg_type_str.value,
                    'request_id': request_id,
                    'workload_id': workload_id,
+                   'transform_id': transform_id,
                    'relation_type': relation_type,
                    'files': files_message}
     num_msg_content = len(files_message)
     return i_msg_type, msg_content, num_msg_content
 
 
 def generate_collection_messages(request_id, transform_id, workload_id, work, collection, relation_type):
@@ -352,14 +348,15 @@
     if coll_name.endswith(".idds.stagein"):
         coll_name = coll_name.replace(".idds.stagein", "")
 
     i_msg_type, i_msg_type_str = get_message_type(work.get_work_type(), input_type='collection')
     msg_content = {'msg_type': i_msg_type_str.value,
                    'request_id': request_id,
                    'workload_id': workload_id,
+                   'transform_id': transform_id,
                    'relation_type': relation_type,
                    'collections': [{'scope': collection.scope,
                                     'name': coll_name,
                                     'status': collection.status.name}],
                    'output': work.get_output_data(),
                    'error': work.get_terminated_msg()}
     num_msg_content = 1
@@ -367,14 +364,15 @@
 
 
 def generate_work_messages(request_id, transform_id, workload_id, work, relation_type):
     i_msg_type, i_msg_type_str = get_message_type(work.get_work_type(), input_type='work')
     msg_content = {'msg_type': i_msg_type_str.value,
                    'request_id': request_id,
                    'workload_id': workload_id,
+                   'transform_id': transform_id,
                    'relation_type': relation_type,
                    'status': work.get_status().name,
                    'output': work.get_output_data(),
                    'error': work.get_terminated_msg()}
     num_msg_content = 1
     return i_msg_type, msg_content, num_msg_content
 
@@ -530,14 +528,39 @@
                 updated_contents_full_input.append(content)
             elif content['content_relation_type'] == ContentRelationType.InputDependency:
                 updated_contents_full_input_deps.append(content)
     # logger.debug(log_prefix + "get_updated_contents_by_request: updated_contents[:3]: %s" % str(updated_contents[:3]))
     return updated_contents, updated_contents_full_input, updated_contents_full_output, updated_contents_full_input_deps
 
 
+def get_input_output_sub_maps(inputs, outputs, inputs_dependency, logs=[]):
+    input_output_sub_maps = {}
+    for content in inputs:
+        sub_map_id = content['sub_map_id']
+        if sub_map_id not in input_output_sub_maps:
+            input_output_sub_maps[sub_map_id] = {'inputs': [], 'outputs': [], 'logs': [], 'inputs_dependency': []}
+            input_output_sub_maps[sub_map_id]['inputs'].append(content)
+    for content in inputs_dependency:
+        sub_map_id = content['sub_map_id']
+        if sub_map_id not in input_output_sub_maps:
+            input_output_sub_maps[sub_map_id] = {'inputs': [], 'outputs': [], 'logs': [], 'inputs_dependency': []}
+        input_output_sub_maps[sub_map_id]['inputs_dependency'].append(content)
+    for content in outputs:
+        sub_map_id = content['sub_map_id']
+        if sub_map_id not in input_output_sub_maps:
+            input_output_sub_maps[sub_map_id] = {'inputs': [], 'outputs': [], 'logs': [], 'inputs_dependency': []}
+        input_output_sub_maps[sub_map_id]['outputs'].append(content)
+    for content in logs:
+        sub_map_id = content['sub_map_id']
+        if sub_map_id not in input_output_sub_maps:
+            input_output_sub_maps[sub_map_id] = {'inputs': [], 'outputs': [], 'logs': [], 'inputs_dependency': []}
+        input_output_sub_maps[sub_map_id]['logs'].append(content)
+    return input_output_sub_maps
+
+
 def get_updated_contents_by_input_output_maps(input_output_maps=None, logger=None, log_prefix=''):
     updated_contents, updated_contents_full_input, updated_contents_full_output = [], [], []
     updated_contents_full_input_deps = []
     new_update_contents = []
 
     status_to_check = [ContentStatus.Available, ContentStatus.FakeAvailable, ContentStatus.FinalFailed,
                        ContentStatus.Missing, ContentStatus.Failed, ContentStatus.Lost,
@@ -545,14 +568,16 @@
 
     for map_id in input_output_maps:
         inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
         inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
         outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
         # logs = input_output_maps[map_id]['logs'] if 'logs' in input_output_maps[map_id] else []
 
+        input_output_sub_maps = get_input_output_sub_maps(inputs, outputs, inputs_dependency)
+
         for content in inputs:
             if (content['status'] != content['substatus']) and content['substatus'] in status_to_check:
                 u_content = {'content_id': content['content_id'],
                              'status': content['substatus']}
                 updated_contents.append(u_content)
                 u_content_substatus = {'content_id': content['content_id'],
                                        'substatus': content['substatus'],
@@ -578,60 +603,65 @@
         for content in inputs_dependency:
             if (content['status'] != content['substatus']) and content['substatus'] in status_to_check:
                 u_content = {'content_id': content['content_id'],
                              'status': content['substatus']}
                 updated_contents.append(u_content)
                 updated_contents_full_input_deps.append(content)
 
-        input_content_update_status = None
-        if is_all_contents_available(inputs_dependency):
-            input_content_update_status = ContentStatus.Available
-        elif is_all_contents_terminated(inputs_dependency):
-            input_content_update_status = ContentStatus.Missing
-        if input_content_update_status:
-            for content in inputs:
-                if content['substatus'] != input_content_update_status:
-                    u_content = {'content_id': content['content_id'],
-                                 'status': input_content_update_status,
-                                 'substatus': input_content_update_status}
-                    updated_contents.append(u_content)
-                    content['status'] = input_content_update_status
-                    content['substatus'] = input_content_update_status
-                    updated_contents_full_input.append(content)
-                    u_content_substatus = {'content_id': content['content_id'],
-                                           'substatus': content['substatus'],
-                                           'request_id': content['request_id'],
-                                           'transform_id': content['transform_id'],
-                                           'workload_id': content['workload_id'],
-                                           'coll_id': content['coll_id']}
-                    new_update_contents.append(u_content_substatus)
-
-        output_content_update_status = None
-        if is_all_contents_available(inputs):
-            # wait for the job to finish
-            pass
-        elif is_all_contents_terminated_but_not_available(inputs):
-            output_content_update_status = ContentStatus.Missing
-        if output_content_update_status:
-            for content in outputs:
-                if content['substatus'] != output_content_update_status:
-                    u_content = {'content_id': content['content_id'],
-                                 'status': output_content_update_status,
-                                 'substatus': output_content_update_status}
-                    updated_contents.append(u_content)
-                    content['status'] = output_content_update_status
-                    content['substatus'] = output_content_update_status
-                    updated_contents_full_output.append(content)
-                    u_content_substatus = {'content_id': content['content_id'],
-                                           'substatus': content['substatus'],
-                                           'request_id': content['request_id'],
-                                           'transform_id': content['transform_id'],
-                                           'workload_id': content['workload_id'],
-                                           'coll_id': content['coll_id']}
-                    new_update_contents.append(u_content_substatus)
+        for sub_map_id in input_output_sub_maps:
+            inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
+            outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
+            inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
+
+            input_content_update_status = None
+            if is_all_contents_available(inputs_dependency_sub):
+                input_content_update_status = ContentStatus.Available
+            elif is_all_contents_terminated(inputs_dependency_sub):
+                input_content_update_status = ContentStatus.Missing
+            if input_content_update_status:
+                for content in inputs_sub:
+                    if content['substatus'] != input_content_update_status:
+                        u_content = {'content_id': content['content_id'],
+                                     'status': input_content_update_status,
+                                     'substatus': input_content_update_status}
+                        updated_contents.append(u_content)
+                        content['status'] = input_content_update_status
+                        content['substatus'] = input_content_update_status
+                        updated_contents_full_input.append(content)
+                        u_content_substatus = {'content_id': content['content_id'],
+                                               'substatus': content['substatus'],
+                                               'request_id': content['request_id'],
+                                               'transform_id': content['transform_id'],
+                                               'workload_id': content['workload_id'],
+                                               'coll_id': content['coll_id']}
+                        new_update_contents.append(u_content_substatus)
+
+            output_content_update_status = None
+            if is_all_contents_available(inputs_sub):
+                # wait for the job to finish
+                pass
+            elif is_all_contents_terminated_but_not_available(inputs_sub):
+                output_content_update_status = ContentStatus.Missing
+            if output_content_update_status:
+                for content in outputs_sub:
+                    if content['substatus'] != output_content_update_status:
+                        u_content = {'content_id': content['content_id'],
+                                     'status': output_content_update_status,
+                                     'substatus': output_content_update_status}
+                        updated_contents.append(u_content)
+                        content['status'] = output_content_update_status
+                        content['substatus'] = output_content_update_status
+                        updated_contents_full_output.append(content)
+                        u_content_substatus = {'content_id': content['content_id'],
+                                               'substatus': content['substatus'],
+                                               'request_id': content['request_id'],
+                                               'transform_id': content['transform_id'],
+                                               'workload_id': content['workload_id'],
+                                               'coll_id': content['coll_id']}
+                        new_update_contents.append(u_content_substatus)
     return updated_contents, updated_contents_full_input, updated_contents_full_output, updated_contents_full_input_deps, new_update_contents
 
 
 def get_transform_dependency_map(transform_id, logger=None, log_prefix=''):
     cache = get_redis_cache()
     transform_dependcy_map_key = "transform_dependcy_map_%s" % transform_id
     transform_dependcy_map = cache.get(transform_dependcy_map_key, default={})
@@ -790,27 +820,33 @@
     update_contents = []
     update_input_contents_full = {}
     update_input_contents_full[transform_id] = []
 
     for map_id in input_output_maps:
         inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
         inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
-        # outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
+        outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
         # logs = input_output_maps[map_id]['logs'] if 'logs' in input_output_maps[map_id] else []
 
-        if not inputs_dependency:
-            for content in inputs:
-                if content['substatus'] != ContentStatus.Available:
-                    u_content = {'content_id': content['content_id'],
-                                 # 'status': ContentStatus.Available,
-                                 'substatus': ContentStatus.Available}
-                    update_contents.append(u_content)
-                    content['status'] = ContentStatus.Available
-                    content['substatus'] = ContentStatus.Available
-                    update_input_contents_full[transform_id].append(content)
+        input_output_sub_maps = get_input_output_sub_maps(inputs, outputs, inputs_dependency)
+        for sub_map_id in input_output_sub_maps:
+            inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
+            # outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
+            inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
+
+            if not inputs_dependency_sub:
+                for content in inputs_sub:
+                    if content['substatus'] != ContentStatus.Available:
+                        u_content = {'content_id': content['content_id'],
+                                     # 'status': ContentStatus.Available,
+                                     'substatus': ContentStatus.Available}
+                        update_contents.append(u_content)
+                        content['status'] = ContentStatus.Available
+                        content['substatus'] = ContentStatus.Available
+                        update_input_contents_full[transform_id].append(content)
     return update_contents, update_input_contents_full
 
 
 def trigger_release_inputs(request_id, transform_id, workload_id, work, updated_contents_full_output, updated_contents_full_input,
                            updated_contents_full_input_deps, input_output_maps, logger=None, log_prefix=''):
     logger = get_logger(logger)
 
@@ -837,79 +873,129 @@
 
     for map_id in input_output_maps:
         inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
         inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
         outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
         # logs = input_output_maps[map_id]['logs'] if 'logs' in input_output_maps[map_id] else []
 
-        input_content_update_status = None
-        if is_all_contents_available(inputs_dependency):
-            input_content_update_status = ContentStatus.Available
-        elif is_all_contents_terminated(inputs_dependency):
-            input_content_update_status = ContentStatus.Missing
-        if input_content_update_status:
-            for content in inputs_dependency:
-                # u_content = {'content_id': content['content_id'], 'status': content['substatus'])
-                # update_contents.append(u_content)
+        input_output_sub_maps = get_input_output_sub_maps(inputs, outputs, inputs_dependency)
+        for sub_map_id in input_output_sub_maps:
+            inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
+            outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
+            inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
+
+            input_content_update_status = None
+            if is_all_contents_available(inputs_dependency_sub):
+                input_content_update_status = ContentStatus.Available
+            elif is_all_contents_terminated(inputs_dependency_sub):
+                input_content_update_status = ContentStatus.Missing
+            if input_content_update_status:
+                for content in inputs_dependency_sub:
+                    # u_content = {'content_id': content['content_id'], 'status': content['substatus'])
+                    # update_contents.append(u_content)
+                    pass
+                for content in inputs_sub:
+                    u_content = {'content_id': content['content_id'],
+                                 'substatus': input_content_update_status}
+                    update_contents.append(u_content)
+                    content['status'] = input_content_update_status
+                    content['substatus'] = input_content_update_status
+                    update_input_contents_full[transform_id].append(content)
+
+            output_content_update_status = None
+            if is_all_contents_available(inputs_sub):
+                # wait for the job to finish
+                # for content in inputs:
+                #     u_content = {'content_id': content['content_id'], 'status': content['substatus'])
+                #     update_contents.append(u_content)
                 pass
-            for content in inputs:
-                u_content = {'content_id': content['content_id'],
-                             'substatus': input_content_update_status}
-                update_contents.append(u_content)
-                content['status'] = input_content_update_status
-                content['substatus'] = input_content_update_status
-                update_input_contents_full[transform_id].append(content)
-
-        output_content_update_status = None
-        if is_all_contents_available(inputs):
-            # wait for the job to finish
-            # for content in inputs:
-            #     u_content = {'content_id': content['content_id'], 'status': content['substatus'])
-            #     update_contents.append(u_content)
-            pass
-        elif is_all_contents_terminated_but_not_available(inputs):
-            # for content in inputs:
-            #     u_content = {'content_id': content['content_id'], 'status': content['substatus'])
-            #     update_contents.append(u_content)
-            pass
-            output_content_update_status = ContentStatus.Missing
-        if output_content_update_status:
-            for content in outputs:
-                u_content = {'content_id': content['content_id'],
-                             'substatus': output_content_update_status}
-                update_contents.append(u_content)
+            elif is_all_contents_terminated_but_not_available(inputs_sub):
+                # for content in inputs:
+                #     u_content = {'content_id': content['content_id'], 'status': content['substatus'])
+                #     update_contents.append(u_content)
+                pass
+                output_content_update_status = ContentStatus.Missing
+            if output_content_update_status:
+                for content in outputs_sub:
+                    u_content = {'content_id': content['content_id'],
+                                 'substatus': output_content_update_status}
+                    update_contents.append(u_content)
 
     return update_contents, update_input_contents_full, update_contents_status_name, update_contents_status
 
 
 def poll_missing_outputs(input_output_maps):
     content_updates_missing, updated_contents_full_missing = [], []
 
     for map_id in input_output_maps:
         inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
-        # inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
+        inputs_dependency = input_output_maps[map_id]['inputs_dependency'] if 'inputs_dependency' in input_output_maps[map_id] else []
         outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
         # logs = input_output_maps[map_id]['logs'] if 'logs' in input_output_maps[map_id] else []
 
-        content_update_status = None
-        if is_all_contents_terminated_but_not_available(inputs):
-            content_update_status = ContentStatus.Missing
-
-            for content in outputs:
-                content['substatus'] = content_update_status
-                if content['status'] != content['substatus']:
-                    u_content = {'content_id': content['content_id'],
-                                 'substatus': content['substatus']}
+        input_output_sub_maps = get_input_output_sub_maps(inputs, outputs, inputs_dependency)
+        for sub_map_id in input_output_sub_maps:
+            inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
+            outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
+            # inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
+
+            content_update_status = None
+            if is_all_contents_terminated_but_not_available(inputs_sub):
+                content_update_status = ContentStatus.Missing
+
+                for content in outputs_sub:
+                    content['substatus'] = content_update_status
+                    if content['status'] != content['substatus']:
+                        u_content = {'content_id': content['content_id'],
+                                     'substatus': content['substatus']}
 
-                    content_updates_missing.append(u_content)
-                    updated_contents_full_missing.append(content)
+                        content_updates_missing.append(u_content)
+                        updated_contents_full_missing.append(content)
 
     return content_updates_missing, updated_contents_full_missing
 
 
+def has_external_content_id(input_output_maps):
+    for map_id in input_output_maps:
+        inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
+        for content in inputs:
+            if not content['external_content_id']:
+                return False
+    return True
+
+
+def get_update_external_content_ids(input_output_maps, external_content_ids):
+    name_to_id_map = {}
+    update_contents = []
+    for map_id in input_output_maps:
+        inputs = input_output_maps[map_id]['inputs'] if 'inputs' in input_output_maps[map_id] else []
+        outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
+        for content in inputs + outputs:
+            if content['name'] not in name_to_id_map:
+                name_to_id_map[content['name']] = []
+            name_to_id_map[content['name']].append(content['content_id'])
+    for dataset in external_content_ids:
+        dataset_id = dataset['dataset']['id']
+        files = dataset['files']
+        for file_item in files:
+            lfn = file_item['lfn']
+            # remove scope '00000:'
+            pos = lfn.find(":")
+            if pos >= 0:
+                lfn = lfn[pos + 1:]
+            file_id = file_item['id']
+            content_ids = name_to_id_map.get(lfn, [])
+            for content_id in content_ids:
+                update_content = {'content_id': content_id,
+                                  'external_coll_id': dataset_id,
+                                  'external_content_id': file_id}
+                update_contents.append(update_content)
+    return update_contents
+
+
 def handle_update_processing(processing, agent_attributes, logger=None, log_prefix=''):
     logger = get_logger(logger)
 
     ret_msgs = []
     new_contents = []
 
     request_id = processing['request_id']
@@ -920,14 +1006,19 @@
     work = proc.work
     work.set_agent_attributes(agent_attributes, processing)
 
     input_output_maps = get_input_output_maps(transform_id, work)
     logger.debug(log_prefix + "get_input_output_maps: len: %s" % len(input_output_maps))
     logger.debug(log_prefix + "get_input_output_maps.keys[:3]: %s" % str(list(input_output_maps.keys())[:3]))
 
+    if work.has_external_content_id() and not has_external_content_id(input_output_maps):
+        external_content_ids = work.get_external_content_ids(processing, log_prefix=log_prefix)
+        update_external_content_ids = get_update_external_content_ids(input_output_maps, external_content_ids)
+        core_catalog.update_contents(update_external_content_ids)
+
     new_input_output_maps = work.get_new_input_output_maps(input_output_maps)
     logger.debug(log_prefix + "get_new_input_output_maps: len: %s" % len(new_input_output_maps))
     logger.debug(log_prefix + "get_new_input_output_maps.keys[:3]: %s" % str(list(new_input_output_maps.keys())[:3]))
 
     if work.require_ext_contents():
         contents_ext = get_ext_contents(transform_id, work)
         job_info_maps = core_catalog.get_contents_ext_maps()
@@ -1008,15 +1099,15 @@
     workload_id = processing['workload_id']
 
     proc = processing['processing_metadata']['processing']
     work = proc.work
     work.set_agent_attributes(agent_attributes, processing)
 
     if (not work.use_dependency_to_release_jobs()) or workload_id is None:
-        return processing['substatus'], [], [], {}, {}, {}, []
+        return processing['substatus'], [], [], {}, {}, {}, [], []
     else:
         if trigger_new_updates:
             # delete information in the contents_update table, to invoke the trigger.
             # ret_update_transforms = core_catalog.delete_contents_update(request_id=request_id, transform_id=transform_id)
             # logger.debug(log_prefix + "delete_contents_update: %s" % str(ret_update_transforms))
             pass
 
@@ -1081,14 +1172,15 @@
     # return processing['substatus'], content_updates, ret_msgs, {}, update_dep_contents_status_name, update_dep_contents_status, [], ret_update_transforms
     # return processing['substatus'], content_updates, ret_msgs, {}, {}, {}, [], ret_update_transforms
     return processing['substatus'], content_updates, ret_msgs, {}, {}, {}, new_update_contents, ret_update_transforms
 
 
 def get_content_status_from_panda_msg_status(status):
     status_map = {'starting': ContentStatus.New,
+                  'activated': ContentStatus.Activated,
                   'running': ContentStatus.Processing,
                   'finished': ContentStatus.Available,
                   'failed': ContentStatus.Failed}
     if status in status_map:
         return status_map[status]
     return ContentStatus.New
 
@@ -1210,15 +1302,17 @@
     if not input_name_content_id_map:
         content_id_lock.acquire()
 
         contents = core_catalog.get_contents_by_request_transform(request_id=request_id, transform_id=transform_id)
         input_name_content_id_map = {}
         for content in contents:
             if content['content_relation_type'] == ContentRelationType.Output:
-                input_name_content_id_map[content['name']] = content['content_id']
+                if content['name'] not in input_name_content_id_map:
+                    input_name_content_id_map[content['name']] = []
+                input_name_content_id_map[content['name']].append(content['content_id'])
 
         cache.set(input_name_content_id_map_key, input_name_content_id_map)
 
         content_id_lock.release()
     return input_name_content_id_map
 
 
@@ -1233,30 +1327,30 @@
         to_update_jobid = True
         input_name_content_id_map = get_input_name_content_id_map(request_id, workload_id, transform_id)
         for ip in inputs:
             if ':' in ip:
                 pos = ip.find(":")
                 ip = ip[pos + 1:]
             if ip in input_name_content_id_map:
-                content_id = input_name_content_id_map[ip]
-                jobid_content_id_map[job_id] = content_id
+                content_ids = input_name_content_id_map[ip]
+                jobid_content_id_map[job_id] = content_ids
                 break
 
         cache.set(jobid_content_id_map_key, jobid_content_id_map)
     return jobid_content_id_map, to_update_jobid
 
 
 def get_content_id_from_job_id(request_id, workload_id, transform_id, job_id, inputs):
     jobid_content_id_map, to_update_jobid = get_jobid_content_id_map(request_id, workload_id, transform_id, job_id, inputs)
 
     if str(job_id) in jobid_content_id_map:
-        content_id = jobid_content_id_map[str(job_id)]
+        content_ids = jobid_content_id_map[str(job_id)]
     else:
-        content_id = None
-    return content_id, to_update_jobid
+        content_ids = None
+    return content_ids, to_update_jobid
 
 
 pending_lock = threading.Lock()
 
 
 def whether_to_process_pending_workload_id(workload_id, logger=None, log_prefix=''):
     cache = get_redis_cache()
@@ -1366,50 +1460,53 @@
                     logger.debug(log_prefix + "Add to terminated processing: %s" % str(processing_id))
 
         if msg['msg_type'] in ['job_status']:
             workload_id = msg['taskid']
             job_id = msg['jobid']
             status = msg['status']
             inputs = msg['inputs']
-            if inputs and status in ['finished']:
+            # if inputs and status in ['finished']:
+            # add activated
+            if inputs and status in ['finished', 'activated']:
                 logger.debug(log_prefix + "Received message: %s" % str(ori_msg))
 
                 ret_req_tf_pr_id = get_workload_id_transform_id_map(workload_id, logger=logger, log_prefix=log_prefix)
                 if not ret_req_tf_pr_id:
                     # request is submitted by some other instances
                     logger.debug(log_prefix + "No matched workload_id, discard message: %s" % str(ori_msg))
                     continue
 
                 logger.debug(log_prefix + "(request_id, transform_id, processing_id, status, substatus): %s" % str(ret_req_tf_pr_id))
 
                 req_id, tf_id, processing_id, r_status, r_substatus = ret_req_tf_pr_id
-                content_id, to_update_jobid = get_content_id_from_job_id(req_id, workload_id, tf_id, job_id, inputs)
-                if content_id:
-                    if to_update_jobid:
-                        u_content = {'content_id': content_id,
-                                     'request_id': req_id,
-                                     'transform_id': tf_id,
-                                     'workload_id': workload_id,
-                                     # 'status': get_content_status_from_panda_msg_status(status),
-                                     'substatus': get_content_status_from_panda_msg_status(status),
-                                     'content_metadata': {'panda_id': job_id}}
-                    else:
-                        u_content = {'content_id': content_id,
-                                     'request_id': req_id,
-                                     'transform_id': tf_id,
-                                     'workload_id': workload_id,
-                                     'substatus': get_content_status_from_panda_msg_status(status)}
-                        #             # 'status': get_content_status_from_panda_msg_status(status)}
-
-                    update_contents.append(u_content)
-                    # if processing_id not in update_processings:
-                    # if processing_id not in update_processings and whether_to_update_processing(processing_id, update_processing_interval):
-                    if processing_id not in update_processings_by_job:
-                        update_processings_by_job.append(processing_id)
-                        logger.debug(log_prefix + "Add to update processing by job: %s" % str(processing_id))
+                content_ids, to_update_jobid = get_content_id_from_job_id(req_id, workload_id, tf_id, job_id, inputs)
+                if content_ids:
+                    for content_id in content_ids:
+                        if to_update_jobid:
+                            u_content = {'content_id': content_id,
+                                         'request_id': req_id,
+                                         'transform_id': tf_id,
+                                         'workload_id': workload_id,
+                                         # 'status': get_content_status_from_panda_msg_status(status),
+                                         'substatus': get_content_status_from_panda_msg_status(status),
+                                         'content_metadata': {'panda_id': job_id}}
+                        else:
+                            u_content = {'content_id': content_id,
+                                         'request_id': req_id,
+                                         'transform_id': tf_id,
+                                         'workload_id': workload_id,
+                                         'substatus': get_content_status_from_panda_msg_status(status)}
+                            #             # 'status': get_content_status_from_panda_msg_status(status)}
+
+                        update_contents.append(u_content)
+                        # if processing_id not in update_processings:
+                        # if processing_id not in update_processings and whether_to_update_processing(processing_id, update_processing_interval):
+                        if processing_id not in update_processings_by_job:
+                            update_processings_by_job.append(processing_id)
+                            logger.debug(log_prefix + "Add to update processing by job: %s" % str(processing_id))
 
     return update_processings, update_processings_by_job, terminated_processings, update_contents, []
 
 
 def sync_collection_status(request_id, transform_id, workload_id, work, input_output_maps=None,
                            close_collection=False, force_close_collection=False, abort=False, terminate=False):
     if input_output_maps is None:
```

### Comparing `idds-server-1.2.9/lib/idds/agents/clerk/clerk.py` & `idds-server-1.3.0/lib/idds/agents/clerk/clerk.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,52 +12,61 @@
 import random
 import time
 import traceback
 
 from idds.common import exceptions
 from idds.common.constants import (Sections, ReturnCode,
                                    RequestStatus, RequestLocking,
-                                   TransformStatus, CommandType,
-                                   CommandStatus, CommandLocking)
+                                   TransformStatus, ProcessingStatus,
+                                   ContentStatus, ContentRelationType,
+                                   CommandType, CommandStatus, CommandLocking)
 from idds.common.utils import setup_logging, truncate_string
 from idds.core import (requests as core_requests,
                        transforms as core_transforms,
+                       processings as core_processings,
+                       catalog as core_catalog,
+                       throttlers as core_throttlers,
                        commands as core_commands)
 from idds.agents.common.baseagent import BaseAgent
 from idds.agents.common.eventbus.event import (EventType,
                                                NewRequestEvent,
                                                UpdateRequestEvent,
                                                AbortRequestEvent,
                                                ResumeRequestEvent,
                                                NewTransformEvent,
                                                UpdateTransformEvent,
                                                AbortTransformEvent,
                                                ResumeTransformEvent,
                                                ExpireRequestEvent)
 
+from idds.agents.common.cache.redis import get_redis_cache
+
+
 setup_logging(__name__)
 
 
 class Clerk(BaseAgent):
     """
     Clerk works to process requests and converts requests to transforms.
     """
 
-    def __init__(self, num_threads=1, poll_period=10, retrieve_bulk_size=10, pending_time=None, **kwargs):
+    def __init__(self, num_threads=1, poll_period=10, retrieve_bulk_size=10, cache_expire_seconds=300, pending_time=None, **kwargs):
         self.set_max_workers()
         num_threads = self.max_number_workers
         super(Clerk, self).__init__(num_threads=num_threads, name='Clerk', **kwargs)
         self.poll_period = int(poll_period)
         self.retrieve_bulk_size = int(retrieve_bulk_size)
         self.config_section = Sections.Clerk
         if pending_time:
             self.pending_time = float(pending_time)
         else:
             self.pending_time = None
 
+        self.cache_expire_seconds = int(cache_expire_seconds)
+
         if not hasattr(self, 'release_helper') or not self.release_helper:
             self.release_helper = False
         elif str(self.release_helper).lower() == 'true':
             self.release_helper = True
         else:
             self.release_helper = False
 
@@ -65,14 +74,18 @@
             self.new_poll_period = self.poll_period
         else:
             self.new_poll_period = int(self.new_poll_period)
         if not hasattr(self, 'update_poll_period') or not self.update_poll_period:
             self.update_poll_period = self.poll_period
         else:
             self.update_poll_period = int(self.update_poll_period)
+        if not hasattr(self, 'throttle_poll_period') or not self.throttle_poll_period:
+            self.throttle_poll_period = self.poll_period
+        else:
+            self.throttle_poll_period = int(self.new_poll_period)
 
         if hasattr(self, 'poll_period_increase_rate'):
             self.poll_period_increase_rate = float(self.poll_period_increase_rate)
         else:
             self.poll_period_increase_rate = 2
 
         if hasattr(self, 'max_new_poll_period'):
@@ -129,15 +142,15 @@
             # self.logger.info("Main thread get %s TransformingOpen requests to process" % len(reqs_open))
 
             if not self.is_ok_to_run_more_requests():
                 return []
 
             self.show_queue_size()
 
-            req_status = [RequestStatus.New, RequestStatus.Extend, RequestStatus.Built]
+            req_status = [RequestStatus.New, RequestStatus.Extend, RequestStatus.Built, RequestStatus.Throttling]
             reqs_new = core_requests.get_requests_by_status_type(status=req_status, locking=True,
                                                                  not_lock=True,
                                                                  new_poll=True, only_return_id=True,
                                                                  bulk_size=self.retrieve_bulk_size)
 
             # self.logger.debug("Main thread get %s [New+Extend] requests to process" % len(reqs_new))
             if reqs_new:
@@ -267,17 +280,19 @@
                 self.logger.warn("(cx_Oracle.DatabaseError) ORA-00060: deadlock detected while waiting for resource")
             else:
                 # raise ex
                 self.logger.error(ex)
                 self.logger.error(traceback.format_exc())
         return None
 
-    def load_poll_period(self, req, parameters):
+    def load_poll_period(self, req, parameters, throttling=False):
         if self.new_poll_period and req['new_poll_period'] != self.new_poll_period:
             parameters['new_poll_period'] = self.new_poll_period
+        if throttling:
+            parameters['new_poll_period'] = self.throttle_poll_period
         if self.update_poll_period and req['update_poll_period'] != self.update_poll_period:
             parameters['update_poll_period'] = self.update_poll_period
         parameters['max_new_retries'] = req['max_new_retries'] if req['max_new_retries'] is not None else self.max_new_retries
         parameters['max_update_retries'] = req['max_update_retries'] if req['max_update_retries'] is not None else self.max_update_retries
         return parameters
 
     def get_work_tag_attribute(self, work_tag, attribute):
@@ -338,49 +353,244 @@
                                                 'workflow': wf}
                          # 'running_metadata': {'work_data': new_work.get_running_data()}
                          # 'collections': related_collections
                          }
 
         return new_transform
 
+    def get_num_active_requests(self, site_name):
+        cache = get_redis_cache()
+        num_requests = cache.get("num_requests", default={})
+        if num_requests is None:
+            num_requests = {}
+            active_status = [RequestStatus.New, RequestStatus.Ready, RequestStatus.Throttling]
+            active_status1 = [RequestStatus.Transforming, RequestStatus.Terminating]
+            rets = core_requests.get_num_active_requests(active_status + active_status1)
+            for ret in rets:
+                status, site, count = ret
+                if site is None:
+                    site = 'Default'
+                if site not in num_requests:
+                    num_requests[site] = {'new': 0, 'processing': 0}
+                if status in active_status:
+                    num_requests[site]['new'] += count
+                elif status in active_status1:
+                    num_requests[site]['processing'] += count
+            cache.set("num_requests", num_requests, expire_seconds=self.cache_expire_seconds)
+        default_value = {'new': 0, 'processing': 0}
+        return num_requests.get(site_name, default_value)
+
+    def get_num_active_transforms(self, site_name):
+        cache = get_redis_cache()
+        num_transforms = cache.get("num_transforms", default={})
+        if num_transforms is None:
+            num_transforms = {}
+            active_status = [TransformStatus.New, TransformStatus.Ready]
+            active_status1 = [TransformStatus.Transforming, TransformStatus.Terminating]
+            rets = core_transforms.get_num_active_transforms(active_status + active_status1)
+            for ret in rets:
+                status, site, count = ret
+                if site is None:
+                    site = 'Default'
+                if site not in num_transforms:
+                    num_transforms[site] = {'new': 0, 'processing': 0}
+                if status in active_status:
+                    num_transforms[site]['new'] += count
+                elif status in active_status1:
+                    num_transforms[site]['processing'] += count
+            cache.set("num_transforms", num_transforms, expire_seconds=self.cache_expire_seconds)
+        default_value = {'new': 0, 'processing': 0}
+        return num_transforms.get(site_name, default_value)
+
+    def get_num_active_processings(self, site_name):
+        cache = get_redis_cache()
+        num_processings = cache.get("num_processings", default={})
+        active_transforms = cache.get("active_transforms", default={})
+        if num_processings is None:
+            num_processings = {}
+            active_status = [ProcessingStatus.New]
+            active_status1 = [ProcessingStatus.Submitting, ProcessingStatus.Submitted,
+                              ProcessingStatus.Running, ProcessingStatus.Terminating, ProcessingStatus.ToTrigger,
+                              ProcessingStatus.Triggering]
+            rets = core_processings.get_active_processings(active_status + active_status1)
+            for ret in rets:
+                req_id, trf_id, pr_id, site, status = ret
+                if site is None:
+                    site = 'Default'
+                if site not in num_processings:
+                    num_processings[site] = {'new': 0, 'processing': 0}
+                    active_transforms[site] = []
+                if status in active_status:
+                    num_processings[site]['new'] += 1
+                elif status in active_status1:
+                    num_processings[site]['processing'] += 1
+                active_transforms[site].append(trf_id)
+            cache.set("num_processings", num_processings, expire_seconds=self.cache_expire_seconds)
+            cache.set("active_transforms", active_transforms, expire_seconds=self.cache_expire_seconds)
+        default_value = {'new': 0, 'processing': 0}
+        return num_processings.get(site_name, default_value), active_transforms
+
+    def get_num_active_contents(self, site_name, active_transform_ids):
+        cache = get_redis_cache()
+        # 1. input contents not terminated
+        # 2. output contents not terminated
+        tf_id_site_map = {}
+        all_tf_ids = []
+        for site in active_transform_ids:
+            all_tf_ids += active_transform_ids[site]
+            for tf_id in active_transform_ids[site]:
+                tf_id_site_map[tf_id] = site
+
+        num_input_contents = cache.get("num_input_contents", default=None)
+        num_output_contents = cache.get("num_output_contents", default=None)
+        if num_input_contents is None or num_output_contents is None:
+            num_input_contents, num_output_contents = {}, {}
+            if all_tf_ids:
+                ret = core_catalog.get_content_status_statistics_by_relation_type(all_tf_ids)
+                for item in ret:
+                    status, relation_type, transform_id, count = item
+                    site = tf_id_site_map[transform_id]
+                    if site not in num_input_contents:
+                        num_input_contents[site] = {'new': 0, 'activated': 0, 'processed': 0}
+                        num_output_contents[site] = {'new': 0, 'activated': 0, 'processed': 0}
+                    if status in [ContentStatus.New]:
+                        if relation_type == ContentRelationType.Input:
+                            num_input_contents[site]['new'] += count
+                        elif relation_type == ContentRelationType.Output:
+                            num_output_contents[site]['new'] += count
+                    if status in [ContentStatus.Activated]:
+                        if relation_type == ContentRelationType.Input:
+                            num_input_contents[site]['activated'] += count
+                        elif relation_type == ContentRelationType.Output:
+                            num_output_contents[site]['activated'] += count
+                    else:
+                        if relation_type == ContentRelationType.Input:
+                            num_input_contents[site]['processed'] += count
+                        elif relation_type == ContentRelationType.Output:
+                            num_output_contents[site]['processed'] += count
+
+            cache.set("num_input_contents", num_input_contents, expire_seconds=self.cache_expire_seconds)
+            cache.set("num_output_contents", num_output_contents, expire_seconds=self.cache_expire_seconds)
+        default_value = {'new': 0, 'activated': 0, 'processed': 0}
+        return num_input_contents.get(site_name, default_value), num_output_contents.get(site_name, default_value)
+
+    def get_throttlers(self):
+        cache = get_redis_cache()
+        throttlers = cache.get("throttlers", default=None)
+        if throttlers is None:
+            throttler_items = core_throttlers.get_throttlers()
+            throttlers = {}
+            for item in throttler_items:
+                throttlers[item['site']] = {'num_requests': item['num_requests'],
+                                            'num_transforms': item['num_transforms'],
+                                            'num_processings': item['num_processings'],
+                                            'new_contents': item['new_contents'],
+                                            'queue_contents': item['queue_contents'],
+                                            'others': item['others'],
+                                            'status': item['status']}
+            cache.set("throttlers", throttlers, expire_seconds=self.cache_expire_seconds)
+        return throttlers
+
+    def whether_to_throttle(self, request):
+        try:
+            site = request['site']
+            if site is None:
+                site = 'Default'
+            throttlers = self.get_throttlers()
+            num_requests = self.get_num_active_requests(site)
+            num_transforms = self.get_num_active_transforms(site)
+            num_processings, active_transforms = self.get_num_active_processings(site)
+            num_input_contents, num_output_contents = self.get_num_active_contents(site, active_transforms)
+            self.logger.info("throttler(site: %s): active requests(%s), transforms(%s), processings(%s)" % (site, num_requests, num_transforms, num_processings))
+            self.logger.info("throttler(site: %s): active input contents(%s), output contents(%s)" % (site, num_input_contents, num_output_contents))
+
+            throttle_requests = throttlers.get(site, {}).get('num_requests', None)
+            throttle_transforms = throttlers.get(site, {}).get('num_transforms', None)
+            throttle_processings = throttlers.get(site, {}).get('num_processings', None)
+            throttle_new_jobs = throttlers.get(site, {}).get('new_contents', None)
+            throttle_queue_jobs = throttlers.get(site, {}).get('queue_contents', None)
+            self.logger.info("throttler(site: %s): throttle_requests %s, throttle_transforms: %s, throttle_processings: %s" % (site, throttle_requests, throttle_transforms, throttle_processings))
+            if throttle_requests:
+                if num_requests['processing'] >= throttle_requests:
+                    self.logger.info("throttler(site: %s): num of processing requests (%s) is bigger than throttle_requests (%s), set throttling" % (site, num_requests['processing'], throttle_requests))
+                    return True
+            if throttle_transforms:
+                if num_transforms['processing'] >= throttle_transforms:
+                    self.logger.info("throttler(site: %s): num of processing transforms (%s) is bigger than throttle_transforms (%s), set throttling" % (site, num_transforms['processing'], throttle_transforms))
+                    return True
+            if throttle_processings:
+                if num_processings['processing'] >= throttle_processings:
+                    self.logger.info("throttler(site: %s): num of processing processings (%s) is bigger than throttle_processings (%s), set throttling" % (site, num_processings['processing'], throttle_processings))
+                    return True
+
+            new_jobs = num_input_contents['new']
+            released_jobs = num_input_contents['processed']
+            terminated_jobs = num_output_contents['processed']
+            queue_jobs = released_jobs - terminated_jobs
+
+            self.logger.info("throttler(site: %s): throttle_new_jobs: %s, throttle_queue_jobs: %s" % (site, throttle_new_jobs, throttle_queue_jobs))
+            self.logger.info("throttler(site: %s): new_jobs: %s, queue_jobs: %s" % (site, new_jobs, queue_jobs))
+            if throttle_new_jobs:
+                if new_jobs >= throttle_new_jobs:
+                    self.logger.info("throttler(site: %s): num of new jobs(not released) (%s) is bigger than throttle_new_jobs (%s), set throttling" % (site, new_jobs, throttle_new_jobs))
+                    return True
+            if throttle_queue_jobs:
+                if queue_jobs >= throttle_queue_jobs:
+                    self.logger.info("throttler(site: %s): num of queue jobs(released but not terminated) (%s) is bigger than throttle_queue_jobs (%s), set throttling" % (site, queue_jobs, throttle_queue_jobs))
+                    return True
+
+            return False
+        except Exception as ex:
+            self.logger.error("whether_to_throttle: %s" % str(ex))
+            self.logger.error(traceback.format_exc())
+        return False
+
     def get_log_prefix(self, req):
         return "<request_id=%s>" % req['request_id']
 
     def handle_new_request(self, req):
         try:
             log_pre = self.get_log_prefix(req)
             self.logger.info(log_pre + "Handle new request")
-            workflow = req['request_metadata']['workflow']
-
-            # wf = workflow.copy()
-            wf = workflow
-            works = wf.get_new_works()
-            transforms = []
-            for work in works:
-                # new_work = work.copy()
-                new_work = work
-                new_work.add_proxy(wf.get_proxy())
-                # new_work.set_request_id(req['request_id'])
-                # new_work.create_processing()
-
-                transform = self.generate_transform(req, work)
-                transforms.append(transform)
-            self.logger.debug(log_pre + "Processing request(%s): new transforms: %s" % (req['request_id'],
-                                                                                        str(transforms)))
-            # processing_metadata = req['processing_metadata']
-            # processing_metadata = {'workflow_data': wf.get_running_data()}
+            to_throttle = self.whether_to_throttle(req)
+            if to_throttle:
+                ret_req = {'request_id': req['request_id'],
+                           'parameters': {'status': RequestStatus.Throttling,
+                                          'locking': RequestLocking.Idle}}
+                ret_req['parameters'] = self.load_poll_period(req, ret_req['parameters'], throttling=True)
+                self.logger.info(log_pre + "Throttle new request result: %s" % str(ret_req))
+            else:
+                workflow = req['request_metadata']['workflow']
 
-            ret_req = {'request_id': req['request_id'],
-                       'parameters': {'status': RequestStatus.Transforming,
-                                      'locking': RequestLocking.Idle,
-                                      # 'processing_metadata': processing_metadata,
-                                      'request_metadata': req['request_metadata']},
-                       'new_transforms': transforms}
-            ret_req['parameters'] = self.load_poll_period(req, ret_req['parameters'])
-            self.logger.info(log_pre + "Handle new request result: %s" % str(ret_req))
+                # wf = workflow.copy()
+                wf = workflow
+                works = wf.get_new_works()
+                transforms = []
+                for work in works:
+                    # new_work = work.copy()
+                    new_work = work
+                    new_work.add_proxy(wf.get_proxy())
+                    # new_work.set_request_id(req['request_id'])
+                    # new_work.create_processing()
+
+                    transform = self.generate_transform(req, work)
+                    transforms.append(transform)
+                self.logger.debug(log_pre + "Processing request(%s): new transforms: %s" % (req['request_id'],
+                                                                                            str(transforms)))
+                # processing_metadata = req['processing_metadata']
+                # processing_metadata = {'workflow_data': wf.get_running_data()}
+
+                ret_req = {'request_id': req['request_id'],
+                           'parameters': {'status': RequestStatus.Transforming,
+                                          'locking': RequestLocking.Idle,
+                                          # 'processing_metadata': processing_metadata,
+                                          'request_metadata': req['request_metadata']},
+                           'new_transforms': transforms}
+                ret_req['parameters'] = self.load_poll_period(req, ret_req['parameters'])
+                self.logger.info(log_pre + "Handle new request result: %s" % str(ret_req))
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
             retries = req['new_retries'] + 1
             if not req['max_new_retries'] or retries < req['max_new_retries']:
                 req_status = req['status']
             else:
@@ -533,15 +743,16 @@
                 self.logger.error(traceback.format_exc())
         return new_tf_ids, update_tf_ids
 
     def process_new_request(self, event):
         self.number_workers += 1
         try:
             if event:
-                req_status = [RequestStatus.New, RequestStatus.Extend, RequestStatus.Built]
+                # req_status = [RequestStatus.New, RequestStatus.Extend, RequestStatus.Built]
+                req_status = [RequestStatus.New, RequestStatus.Extend, RequestStatus.Built, RequestStatus.Throttling]
                 req = self.get_request(request_id=event._request_id, status=req_status, locking=True)
                 if not req:
                     self.logger.error("Cannot find request for event: %s" % str(event))
                 elif req:
                     log_pre = self.get_log_prefix(req)
                     if self.has_to_build_work(req):
                         ret = self.handle_build_request(req)
@@ -907,22 +1118,29 @@
                         else:
                             if 'workflow' in req['request_metadata']:
                                 wf = req['request_metadata']['workflow']
                             else:
                                 wf = req['request_metadata']['build_workflow']
                         works = wf.get_all_works()
                         if works:
+                            has_abort_work = False
                             for work in works:
                                 if (work.is_started() or work.is_starting()) and not work.is_terminated():
                                     if not to_abort_transform_id or to_abort_transform_id == work.get_work_id():
                                         self.logger.info(log_pre + "AbortTransformEvent(transform_id: %s)" % str(work.get_work_id()))
                                         event = AbortTransformEvent(publisher_id=self.id,
                                                                     transform_id=work.get_work_id(),
                                                                     content=event._content)
                                         self.event_bus.send(event)
+                                        has_abort_work = True
+                            if not has_abort_work:
+                                self.logger.info(log_pre + "not has abort work")
+                                self.logger.info(log_pre + "UpdateRequestEvent(request_id: %s)" % str(req['request_id']))
+                                event = UpdateRequestEvent(publisher_id=self.id, request_id=req['request_id'], content=event._content)
+                                self.event_bus.send(event)
                         else:
                             # no works. should trigger update request
                             self.logger.info(log_pre + "UpdateRequestEvent(request_id: %s)" % str(req['request_id']))
                             event = UpdateRequestEvent(publisher_id=self.id, request_id=req['request_id'], content=event._content)
                             self.event_bus.send(event)
 
                         self.handle_command(event, cmd_status=CommandStatus.Processed, errors=None)
```

### Comparing `idds-server-1.2.9/lib/idds/agents/common/baseagent.py` & `idds-server-1.3.0/lib/idds/agents/common/baseagent.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/cache/redis.py` & `idds-server-1.3.0/lib/idds/agents/common/cache/redis.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/eventbus/baseeventbusbackend.py` & `idds-server-1.3.0/lib/idds/agents/common/eventbus/baseeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py` & `idds-server-1.3.0/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/eventbus/dbeventbusbackend.py` & `idds-server-1.3.0/lib/idds/agents/common/eventbus/dbeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/eventbus/eventbus.py` & `idds-server-1.3.0/lib/idds/agents/common/eventbus/eventbus.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,36 +43,40 @@
             self._id = str(uuid.uuid4())[:8]
             self.setup_logger(logger)
             self.config_section = Sections.EventBus
             attrs = self.load_attributes()
             self.attrs = attrs
             self._backend = None
             self._orig_backend = None
+            self._backup_backend = BaseEventBusBackendOpt(logger=self.logger, **attrs)
             if 'backend' in attrs:
                 if attrs['backend'] == 'message':
                     self.backend = MsgEventBusBackend(logger=self.logger, **attrs)
                 elif attrs['backend'] == "database":
                     if 'to_archive' not in attrs:
                         attrs['to_archive'] = True
                     self.backend = DBEventBusBackend(**attrs)
             if self.backend is None:
                 self.backend = BaseEventBusBackendOpt(logger=self.logger, **attrs)
             self.logger.info("EventBus backend : %s" % self.backend)
+            self._orig_backend = self.backend
             self.backend.start()
 
     @property
     def backend(self):
         if self._backend and isinstance(self._backend, MsgEventBusBackend) and not self._backend.is_ok():
-            self._orig_backend = self._backend
-            self._backend = BaseEventBusBackendOpt(logger=self.logger, **self.attrs)
+            # self._orig_backend = self._backend
+            # self._backend = BaseEventBusBackendOpt(logger=self.logger, **self.attrs)
+            self._backend = self._backup_backend
             self.logger.critical("MsgEventBusBackend failed, switch to use BaseEventBusBackendOpt")
         elif self._orig_backend and isinstance(self._orig_backend, MsgEventBusBackend) and self._orig_backend.is_ok():
-            self.logger.critical("MsgEventBusBackend is ok, switch back to use it")
+            if self._backend != self._orig_backend:
+                self.logger.critical("MsgEventBusBackend is ok, switch back to use it")
             self._backend = self._orig_backend
-            self._orig_backend = None
+            # self._orig_backend = None
         return self._backend
 
     @backend.setter
     def backend(self, value):
         self._backend = value
 
     def setup_logger(self, logger=None):
@@ -121,16 +125,20 @@
         self.backend.clean_event(event)
 
     def fail_event(self, event):
         self.backend.fail_event(event)
 
     def set_manager(self, manager):
         self.backend.set_manager(manager)
+        if self._orig_backend:
+            self._orig_backend.set_manager(manager)
 
     def get_manager(self):
+        if self._orig_backend:
+            return self._orig_backend.get_manager()
         return self.backend.get_manager()
 
     def get_coordinator(self):
         return self.backend.get_coordinator()
 
     def set_coordinator(self, coordinator):
         self.backend.set_coordinator(coordinator)
```

### Comparing `idds-server-1.2.9/lib/idds/agents/common/eventbus/msgeventbusbackend.py` & `idds-server-1.3.0/lib/idds/agents/common/eventbus/msgeventbusbackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,16 @@
 
 class MsgEventBusBackend(BaseEventBusBackend):
     """
     Msg Event Bus Backend
     """
 
     def __init__(self, logger=None, coordinator_port=5556, socket_timeout=10, debug=False,
-                 timeout_threshold=5, failure_threshold=5, **kwargs):
+                 timeout_threshold=5, failure_threshold=5, failure_timeout=180,
+                 num_of_set_failed_at_threshold=10, **kwargs):
         super(MsgEventBusBackend, self).__init__()
         self._id = str(uuid.uuid4())[:8]
         self._state_claim_wait = 60
         self._state_claim = StateClaimEvent(self._id, EventBusState.New, time.time())
 
         self.graceful_stop = threading.Event()
 
@@ -218,14 +219,18 @@
 
         self.max_delay = 180
 
         self._username = 'idds'
         self._password = ''.join(random.choice(string.ascii_uppercase + string.ascii_lowercase + string.digits) for _ in range(20))
 
         self._is_ok = True
+        self._failed_at = None
+        self._failure_timeout = int(failure_timeout)
+        self._num_of_set_failed_at = 0
+        self._num_of_set_failed_at_threshold = int(num_of_set_failed_at_threshold)
         self.num_success = 0
         self.num_failures = 0
         self.num_timeout = 0
         self.cache_events = []
 
         self.setup_logger(logger)
 
@@ -452,16 +457,24 @@
     def clean_event(self, event):
         pass
 
     def fail_event(self, event):
         pass
 
     def is_ok(self):
-        if self.num_failures > self.failure_threshold or self.num_timeout > self.timeout_threshold:
+        if self._num_of_set_failed_at < self._num_of_set_failed_at_threshold and self._failed_at and self._failed_at + self._failure_timeout < time.time():
+            self._is_ok = True
+            self._failed_at = None
+            self.num_failures = 0
+            self.num_timeout = 0
+        elif self.num_failures > self.failure_threshold or self.num_timeout > self.timeout_threshold:
             self._is_ok = False
+            if not self._failed_at:
+                self._failed_at = time.time()
+                self._num_of_set_failed_at += 1
         else:
             self._is_ok = True
         return self._is_ok
 
     def replay_cache_events(self):
         cache_events = self.cache_events
         self.cache_events = []
```

### Comparing `idds-server-1.2.9/lib/idds/agents/common/plugins/messaging.py` & `idds-server-1.3.0/lib/idds/agents/common/plugins/messaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     def __init__(self, name="MessagingSender", logger=None, **kwargs):
         threading.Thread.__init__(self, name=name)
         super(MessagingSender, self).__init__(name=name, logger=logger, **kwargs)
 
         if logger:
             self.logger = logger
         self.graceful_stop = threading.Event()
+        self.graceful_suspend = threading.Event()
+
         self.request_queue = None
         self.output_queue = None
         self.response_queue = None
 
         if not hasattr(self, 'channels'):
             raise Exception('"channels" is required but not defined.')
         self.channels = json_loads(self.channels)
@@ -90,14 +92,23 @@
 
     def get_logger(self):
         return self.logger
 
     def stop(self):
         self.graceful_stop.set()
 
+    def suspend(self):
+        self.graceful_suspend.set()
+
+    def resume(self):
+        self.graceful_suspend.clear()
+
+    def is_processing(self):
+        return (not self.graceful_stop.is_set()) and (not self.graceful_suspend.is_set())
+
     def set_request_queue(self, request_queue):
         self.request_queue = request_queue
 
     def set_output_queue(self, output_queue):
         self.output_queue = output_queue
 
     def set_response_queue(self, response_queue):
@@ -134,28 +145,29 @@
 
                 timeout = broker_timeout
 
                 conns = []
                 for broker, port in broker_addresses:
                     conn = stomp.Connection12(host_and_ports=[(broker, port)],
                                               keepalive=True,
-                                              heartbeats=(60000, 60000),     # one minute
+                                              heartbeats=(60000, 0),     # one minute
                                               timeout=timeout)
                     conns.append(conn)
                 channel_conns[name] = conns
             else:
                 channel_conns[name] = None
         return channel_conns
 
     def disconnect(self, conns):
         for name in conns:
             if conns[name]:
                 for conn in conns[name]:
                     try:
-                        conn.disconnect()
+                        if conn.is_connected():
+                            conn.disconnect()
                     except Exception:
                         pass
 
     def get_connection(self, destination):
         try:
             if destination not in self.conns:
                 destination = 'default'
@@ -256,36 +268,49 @@
 
     def execute_subscribe(self):
         try:
             self.subscribe()
         except Exception as error:
             self.logger.error("Messaging receiver throws an exception: %s, %s" % (error, traceback.format_exc()))
 
+        sleep_count = 0
         while not self.graceful_stop.is_set():
-            has_failed_connection = False
-            try:
-                for name in self.receiver_conns:
-                    for conn in self.receiver_conns[name]:
-                        if not conn.is_connected():
-                            conn.set_listener('message-receiver', self.get_listener(conn.transport._Transport__host_and_ports[0]))
-                            # conn.start()
-                            conn.connect(self.channels[name]['username'], self.channels[name]['password'], wait=True)
-                            conn.subscribe(destination=self.channels[name]['destination'], id='atlas-idds-messaging', ack='auto')
-                time.sleep(0.1)
-            except Exception as error:
-                self.logger.error("Messaging receiver throws an exception: %s, %s" % (error, traceback.format_exc()))
-                has_failed_connection = True
-
-            if has_failed_connection or len(self.receiver_conns) == 0:
+            if self.graceful_suspend.is_set():
                 try:
-                    # re-subscribe
                     self.disconnect(self.receiver_conns)
-                    self.subscribe()
                 except Exception as error:
                     self.logger.error("Messaging receiver throws an exception: %s, %s" % (error, traceback.format_exc()))
+                time.sleep(1)
+                sleep_count += 1
+                if sleep_count > 300:
+                    self.logger.info("graceful_suspend is set. sleeping")
+                    sleep_count = 0
+            else:
+                sleep_count = 0
+                has_failed_connection = False
+                try:
+                    for name in self.receiver_conns:
+                        for conn in self.receiver_conns[name]:
+                            if not conn.is_connected():
+                                conn.set_listener('message-receiver', self.get_listener(conn.transport._Transport__host_and_ports[0]))
+                                # conn.start()
+                                conn.connect(self.channels[name]['username'], self.channels[name]['password'], wait=True)
+                                conn.subscribe(destination=self.channels[name]['destination'], id='atlas-idds-messaging', ack='auto')
+                    time.sleep(0.1)
+                except Exception as error:
+                    self.logger.error("Messaging receiver throws an exception: %s, %s" % (error, traceback.format_exc()))
+                    has_failed_connection = True
+
+                if has_failed_connection or len(self.receiver_conns) == 0:
+                    try:
+                        # re-subscribe
+                        self.disconnect(self.receiver_conns)
+                        self.subscribe()
+                    except Exception as error:
+                        self.logger.error("Messaging receiver throws an exception: %s, %s" % (error, traceback.format_exc()))
 
         self.logger.info('receiver graceful stop requested')
 
         self.disconnect(self.receiver_conns)
 
     def run(self):
         try:
```

### Comparing `idds-server-1.2.9/lib/idds/agents/common/timerscheduler.py` & `idds-server-1.3.0/lib/idds/agents/common/timerscheduler.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/common/timertask.py` & `idds-server-1.3.0/lib/idds/agents/common/timertask.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/conductor/conductor.py` & `idds-server-1.3.0/lib/idds/agents/conductor/conductor.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,40 +4,47 @@
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
 # - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
+import datetime
+import random
 import time
 import traceback
 try:
     # python 3
     from queue import Queue
 except ImportError:
     # Python 2
     from Queue import Queue
 
-from idds.common.constants import (Sections, MessageStatus, MessageDestination, MessageType)
+from idds.common.constants import (Sections, MessageStatus, MessageDestination, MessageType,
+                                   ProcessingStatus, ContentStatus, ContentRelationType)
 from idds.common.exceptions import AgentPluginError, IDDSException
 from idds.common.utils import setup_logging, get_logger
-from idds.core import messages as core_messages
+from idds.core import (messages as core_messages,
+                       catalog as core_catalog,
+                       processings as core_processings,
+                       health as core_health)
 from idds.agents.common.baseagent import BaseAgent
 
 
 setup_logging(__name__)
 
 
 class Conductor(BaseAgent):
     """
     Conductor works to notify workload management that the data is available.
     """
 
-    def __init__(self, num_threads=1, retrieve_bulk_size=1000, threshold_to_release_messages=None,
-                 random_delay=None, delay=60, interval_delay=10, replay_times=3, **kwargs):
+    def __init__(self, num_threads=1, retrieve_bulk_size=200, threshold_to_release_messages=None,
+                 random_delay=None, delay=300, interval_delay=10, max_retry_delay=3600,
+                 max_normal_retries=10, max_retries=30, replay_times=2, mode='single', **kwargs):
         super(Conductor, self).__init__(num_threads=num_threads, name='Conductor', **kwargs)
         self.config_section = Sections.Conductor
         self.retrieve_bulk_size = int(retrieve_bulk_size)
         self.message_queue = Queue()
         self.output_message_queue = Queue()
         if threshold_to_release_messages is None:
             self.threshold_to_release_messages = None
@@ -48,65 +55,107 @@
         else:
             self.random_delay = int(random_delay)
             if self.random_delay < 5:
                 self.random_delay = 5
         if delay is None:
             delay = 60
         self.delay = int(delay)
+        if not max_retry_delay:
+            max_retry_delay = 3600
+        self.max_retry_delay = int(max_retry_delay)
+
+        self.max_normal_retries = int(max_normal_retries)
+        self.max_retries = int(max_retries)
+
         if replay_times is None:
-            replay_times = 3
+            replay_times = 2
         self.replay_times = int(replay_times)
         if not interval_delay:
             interval_delay = 10
         self.interval_delay = int(interval_delay)
         self.logger = get_logger(self.__class__.__name__)
 
+        self.mode = mode
+        self.selected = None
+        self.selected_conductor = None
+
     def __del__(self):
         self.stop_notifier()
 
+    def is_selected(self):
+        selected = None
+        if not self.selected_conductor:
+            selected = True
+        else:
+            selected = self.is_self(self.selected_conductor)
+        if self.selected is None or self.selected != selected:
+            self.logger.info("is_selected changed from %s to %s" % (self.selected, selected))
+        self.selected = selected
+        return self.selected
+
+    def monitor_conductor(self):
+        if self.mode == "single":
+            self.logger.info("Conductor single mode")
+            self.selected_conductor = core_health.select_agent(name='Conductor', newer_than=self.heartbeat_delay * 2)
+            self.logger.debug("Selected conductor: %s" % self.selected_conductor)
+
+    def add_conductor_monitor_task(self):
+        task = self.create_task(task_func=self.monitor_conductor, task_output_queue=None,
+                                task_args=tuple(), task_kwargs={}, delay_time=self.heartbeat_delay,
+                                priority=1)
+        self.add_task(task)
+
     def get_messages(self):
         """
         Get messages
         """
         destination = [MessageDestination.Outside, MessageDestination.ContentExt]
         messages = core_messages.retrieve_messages(status=MessageStatus.New,
                                                    bulk_size=self.retrieve_bulk_size,
                                                    destination=destination)
 
         # self.logger.debug("Main thread get %s new messages" % len(messages))
         if messages:
             self.logger.info("Main thread get %s new messages" % len(messages))
 
-        msg_type = [MessageType.StageInCollection, MessageType.StageInWork,
-                    MessageType.ActiveLearningCollection, MessageType.ActiveLearningWork,
-                    MessageType.HyperParameterOptCollection, MessageType.HyperParameterOptWork,
-                    MessageType.ProcessingCollection, MessageType.ProcessingWork,
-                    MessageType.UnknownCollection, MessageType.UnknownWork]
-        retry_messages = []
-        for retry in range(1, self.replay_times + 1):
-            delay = int(self.delay) * (retry ** 3)
+        # msg_type = [MessageType.StageInCollection, MessageType.StageInWork,
+        #             MessageType.ActiveLearningCollection, MessageType.ActiveLearningWork,
+        #             MessageType.HyperParameterOptCollection, MessageType.HyperParameterOptWork,
+        #             MessageType.ProcessingCollection, MessageType.ProcessingWork,
+        #             MessageType.UnknownCollection, MessageType.UnknownWork]
 
-            messages_d = core_messages.retrieve_messages(status=MessageStatus.Delivered,
-                                                         retries=retry, delay=delay,
-                                                         bulk_size=self.retrieve_bulk_size,
-                                                         destination=destination,
-                                                         msg_type=msg_type)
-            if messages_d:
-                self.logger.info("Main thread get %s retries messages" % len(messages_d))
-                retry_messages += messages_d
+        retry_messages = []
+        messages_d = core_messages.retrieve_messages(status=MessageStatus.Delivered,
+                                                     use_poll_period=True,
+                                                     bulk_size=self.retrieve_bulk_size,
+                                                     destination=destination)    # msg_type=msg_type)
+        if messages_d:
+            self.logger.info("Main thread get %s retries messages" % len(messages_d))
+            retry_messages += messages_d
 
         return messages + retry_messages
 
-    def clean_messages(self, msgs):
+    def clean_messages(self, msgs, confirm=False):
         # core_messages.delete_messages(msgs)
+        msg_status = MessageStatus.Delivered
+        if confirm:
+            msg_status = MessageStatus.ConfirmDelivered
         to_updates = []
         for msg in msgs:
+            retries = msg['retries']
+            if retries < self.max_normal_retries:
+                rand_num = random.randint(1, retries + 1)
+                delay = int(self.delay) * rand_num
+                delay = min(delay, self.max_retry_delay)
+            else:
+                delay = self.max_retry_delay
             to_updates.append({'msg_id': msg['msg_id'],
                                'retries': msg['retries'] + 1,
-                               'status': MessageStatus.Delivered})
+                               'poll_period': datetime.timedelta(seconds=delay),
+                               'status': msg_status})
         core_messages.update_messages(to_updates)
 
     def start_notifier(self):
         if 'notifier' not in self.plugins:
             raise AgentPluginError('Plugin notifier is required')
         self.notifier = self.plugins['notifier']
 
@@ -128,43 +177,114 @@
                 msg = self.output_message_queue.get(False)
                 if msg:
                     msgs.append(msg)
         except Exception as error:
             self.logger.error("Failed to get output messages: %s, %s" % (error, traceback.format_exc()))
         return msgs
 
+    def is_message_processed(self, message):
+        retries = message['retries']
+        try:
+            if retries >= self.max_retries:
+                self.logger.info("message %s has reached max retries %s" % (message['msg_id'], self.max_retries))
+                return True
+            msg_type = message['msg_type']
+            if msg_type not in [MessageType.ProcessingFile]:
+                if retries < self.replay_times:
+                    return False
+                else:
+                    return True
+            else:
+                msg_content = message['msg_content']
+                request_id = message['request_id']
+                transform_id = message['transform_id']
+                if 'files' not in msg_content or not msg_content['files']:
+                    return True
+                if 'relation_type' not in msg_content or msg_content['relation_type'] != 'input':
+                    return True
+
+                files = msg_content['files']
+                one_file = files[0]
+                # only check one file in a message
+                map_id = one_file['map_id']
+                contents = core_catalog.get_contents_by_request_transform(request_id=request_id,
+                                                                          transform_id=transform_id,
+                                                                          map_id=map_id)
+                for content in contents:
+                    if content['content_relation_type'] == ContentRelationType.Output:
+                        if (content['status'] == ContentStatus.Missing):
+                            workload_id = msg_content['workload_id']
+                            processings = core_processings.get_processings_by_transform_id(transform_id=transform_id)
+                            find_processing = None
+                            if processings:
+                                for processing in processings:
+                                    if processing['workload_id'] == workload_id:
+                                        find_processing = processing
+                            if find_processing and find_processing['status'] in [ProcessingStatus.Finished, ProcessingStatus.Failed,
+                                                                                 ProcessingStatus.Lost, ProcessingStatus.SubFinished,
+                                                                                 ProcessingStatus.Cancelled, ProcessingStatus.Expired,
+                                                                                 ProcessingStatus.Suspended, ProcessingStatus.Broken]:
+                                return True
+                            else:
+                                return False
+                        if (content['status'] != ContentStatus.New):
+                            return True
+        except Exception as ex:
+            self.logger.error(ex)
+            self.logger.error(traceback.format_exc())
+
+            if retries < self.replay_times:
+                return False
+        return False
+
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
             self.init_thread_info()
             self.load_plugins()
 
             self.add_default_tasks()
 
+            if self.mode == "single":
+                self.logger.debug("single mode")
+                self.add_conductor_monitor_task()
+
             self.start_notifier()
 
             # self.add_health_message_task()
 
             while not self.graceful_stop.is_set():
                 # execute timer task
                 self.execute_schedules()
 
                 try:
                     num_contents = 0
-                    messages = self.get_messages()
-                    if not messages:
-                        time.sleep(self.interval_delay)
+                    if self.is_selected():
+                        messages = self.get_messages()
+                        if not messages:
+                            time.sleep(self.interval_delay)
+                    else:
+                        messages = []
+
+                    to_discard_messages = []
                     for message in messages:
                         message['destination'] = message['destination'].name
 
                         num_contents += message['num_contents']
-                        self.message_queue.put(message)
+                        if self.is_message_processed(message):
+                            self.logger.debug("message (msg_id: %s) is already processed, not resend it again" % message['msg_id'])
+                            to_discard_messages.append(message)
+                        else:
+                            self.message_queue.put(message)
+                    if to_discard_messages:
+                        self.clean_messages(to_discard_messages, confirm=True)
+
                     while not self.message_queue.empty():
                         time.sleep(1)
                     output_messages = self.get_output_messages()
                     self.clean_messages(output_messages)
                 except IDDSException as error:
                     self.logger.error("Main thread IDDSException: %s" % str(error))
                 except Exception as error:
```

### Comparing `idds-server-1.2.9/lib/idds/agents/conductor/consumer.py` & `idds-server-1.3.0/lib/idds/agents/conductor/consumer.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/coordinator/coordinator.py` & `idds-server-1.3.0/lib/idds/agents/coordinator/coordinator.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/main.py` & `idds-server-1.3.0/lib/idds/agents/main.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/marshaller/marshaller.py` & `idds-server-1.3.0/lib/idds/agents/marshaller/marshaller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/transformer/transformer.py` & `idds-server-1.3.0/lib/idds/agents/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/agents/transporter/transporter.py` & `idds-server-1.3.0/lib/idds/agents/transporter/transporter.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/catalog.py` & `idds-server-1.3.0/lib/idds/api/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/collections.py` & `idds-server-1.3.0/lib/idds/api/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/contents.py` & `idds-server-1.3.0/lib/idds/api/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/processings.py` & `idds-server-1.3.0/lib/idds/api/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/requests.py` & `idds-server-1.3.0/lib/idds/api/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/api/transforms.py` & `idds-server-1.3.0/lib/idds/api/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/core/catalog.py` & `idds-server-1.3.0/lib/idds/core/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,27 +327,27 @@
                                          relation_type=content_relation_type, session=session)
     else:
         rets = []
     return rets
 
 
 @read_session
-def get_contents_by_request_transform(request_id=None, workload_id=None, transform_id=None, status=None, status_updated=False, session=None):
+def get_contents_by_request_transform(request_id=None, workload_id=None, transform_id=None, status=None, map_id=None, status_updated=False, session=None):
     """
     Get contents with request id, workload id and transform id.
 
     :param request_id: the request id.
     :param workload_id: The workload_id of the request.
     :param transform_id: The transform id related to this collection.
     :param session: The database session in use.
 
     :returns: list of contents
     """
     ret = orm_contents.get_contents_by_request_transform(request_id=request_id, transform_id=transform_id,
-                                                         workload_id=workload_id, status=status,
+                                                         workload_id=workload_id, status=status, map_id=map_id,
                                                          status_updated=status_updated, session=session)
     return ret
 
 
 @read_session
 def get_contents_by_content_ids(content_ids, request_id=None, session=None):
     """
@@ -495,24 +495,37 @@
     for row in contents:
         if (not content) or (content['max_id'] - content['min_id'] > row['max_id'] - row['min_id']):
             content = row
     return [content]
 
 
 @read_session
-def get_content_status_statistics(coll_id=None, session=None):
+def get_content_status_statistics(coll_id=None, transform_ids=None, session=None):
     """
     Get statistics group by status
 
     :param coll_id: Collection id.
     :param session: The database session in use.
 
     :returns: statistics group by status, as a dict.
     """
-    return orm_contents.get_content_status_statistics(coll_id=coll_id, session=session)
+    return orm_contents.get_content_status_statistics(coll_id=coll_id, transform_ids=transform_ids, session=session)
+
+
+@read_session
+def get_content_status_statistics_by_relation_type(transform_ids, session=None):
+    """
+    Get statistics group by status
+
+    :param coll_id: Collection id.
+    :param session: The database session in use.
+
+    :returns: statistics group by status, as a dict.
+    """
+    return orm_contents.get_content_status_statistics_by_relation_type(transform_ids, session=session)
 
 
 @transactional_session
 def clean_locking(time_period=3600, session=None):
     """
     Clearn locking which is older than time period.
```

### Comparing `idds-server-1.2.9/lib/idds/core/commands.py` & `idds-server-1.3.0/lib/idds/core/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/core/events.py` & `idds-server-1.3.0/lib/idds/core/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/core/health.py` & `idds-server-1.3.0/lib/idds/core/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/core/messages.py` & `idds-server-1.3.0/lib/idds/core/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 
 """
 operations related to Messages.
 """
 
+import threading
+
 from idds.common.constants import MessageDestination, MessageType, MessageStatus
 from idds.orm.base.session import read_session, transactional_session
 from idds.orm import messages as orm_messages
 
 
 @transactional_session
 def add_message(msg_type, status, source, request_id, workload_id, transform_id,
@@ -42,32 +44,37 @@
 def add_messages(messages, bulk_size=1000, session=None):
     return orm_messages.add_messages(messages, bulk_size=bulk_size, session=session)
 
 
 @read_session
 def retrieve_messages(bulk_size=None, msg_type=None, status=None, destination=None,
                       source=None, request_id=None, workload_id=None, transform_id=None,
-                      processing_id=None, retries=None, delay=None, session=None):
+                      processing_id=None, use_poll_period=False, retries=None, delay=None,
+                      fetching_id=None, session=None):
     """
     Retrieve up to $bulk messages.
 
     :param bulk: Number of messages as an integer.
     :param msg_type: Return only specified msg_type.
     :param status: The status about the message
     :param source: The source where the message is from.
     :param session: The database session.
 
     :returns messages: List of dictionaries
     """
+    if fetching_id is None:
+        hb_thread = threading.current_thread()
+        fetching_id = hb_thread.ident
+
     return orm_messages.retrieve_messages(bulk_size=bulk_size, msg_type=msg_type,
                                           status=status, source=source, destination=destination,
                                           request_id=request_id, workload_id=workload_id,
                                           transform_id=transform_id, processing_id=processing_id,
-                                          retries=retries, delay=delay,
-                                          session=session)
+                                          retries=retries, delay=delay, fetching_id=fetching_id,
+                                          use_poll_period=use_poll_period, session=session)
 
 
 @read_session
 def retrieve_request_messages(request_id, bulk_size=1, session=None):
     return retrieve_messages(request_id=request_id,
                              msg_type=MessageType.IDDSCommunication,
                              status=MessageStatus.New,
```

### Comparing `idds-server-1.2.9/lib/idds/core/processings.py` & `idds-server-1.3.0/lib/idds/core/processings.py`

 * *Files 6% similar despite different names*

```diff
@@ -290,17 +290,28 @@
         if content['coll_id'] not in coll_ids:
             coll_ids.append(content['coll_id'])
     contents = orm_contents.get_contents(coll_id=coll_ids, relation_type=ContentRelationType.Output, session=session)
     content_name_id_map = {}
     for content in contents:
         if content['coll_id'] not in content_name_id_map:
             content_name_id_map[content['coll_id']] = {}
-        content_name_id_map[content['coll_id']][content['name']] = content['content_id']
+        if content['name'] not in content_name_id_map[content['coll_id']]:
+            content_name_id_map[content['coll_id']][content['name']] = {}
+        # if content['map_id'] not in content_name_id_map[content['coll_id']][content['name']]:
+        #     content_name_id_map[content['coll_id']][content['name']][content['map_id']] = {}
+        content_name_id_map[content['coll_id']][content['name']][content['sub_map_id']] = content['content_id']
+        # content_name_id_map[content['coll_id']][content['name']] = content['content_id']
+
     for content in new_input_dependency_contents:
-        content_dep_id = content_name_id_map[content['coll_id']][content['name']]
+        if 'sub_map_id' not in content or content['sub_map_id'] is None:
+            content['sub_map_id'] = 0
+        dep_sub_map_id = content.get("dep_sub_map_id", 0)
+        if dep_sub_map_id is None:
+            dep_sub_map_id = 0
+        content_dep_id = content_name_id_map[content['coll_id']][content['name']][dep_sub_map_id]
         content['content_dep_id'] = content_dep_id
     return new_input_dependency_contents
 
 
 @transactional_session
 def update_processing_contents(update_processing, update_contents, update_messages=None, new_contents=None,
                                update_dep_contents=None, update_collections=None, messages=None,
@@ -365,7 +376,17 @@
 def clean_next_poll_at(status, session=None):
     """
     Clearn next_poll_at.
 
     :param status: status of the processing
     """
     orm_processings.clean_next_poll_at(status=status, session=session)
+
+
+@read_session
+def get_num_active_processings(active_status=None, session=None):
+    return orm_processings.get_num_active_processings(active_status=active_status, session=session)
+
+
+@read_session
+def get_active_processings(active_status=None, session=None):
+    return orm_processings.get_active_processings(active_status=active_status, session=session)
```

### Comparing `idds-server-1.2.9/lib/idds/core/requests.py` & `idds-server-1.3.0/lib/idds/core/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,7 +463,17 @@
 
     :param status: status of the request.
     :param older_than: days older than current timestamp.
 
     :returns request_id
     """
     return orm_requests.get_last_request_id(status=status, older_than=older_than, session=session)
+
+
+@read_session
+def get_num_active_requests(active_status=None, session=None):
+    return orm_requests.get_num_active_requests(active_status=active_status, session=session)
+
+
+@read_session
+def get_active_requests(active_status=None, session=None):
+    return orm_requests.get_active_requests(active_status=active_status, session=session)
```

### Comparing `idds-server-1.2.9/lib/idds/core/transforms.py` & `idds-server-1.3.0/lib/idds/core/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -377,47 +377,65 @@
 
     :param status: status of the transform
     """
     orm_transforms.clean_next_poll_at(status=status, session=session)
 
 
 @read_session
-def get_transform_input_output_maps(transform_id, input_coll_ids, output_coll_ids, log_coll_ids=[], session=None):
+def get_transform_input_output_maps(transform_id, input_coll_ids, output_coll_ids, log_coll_ids=[], with_sub_map_id=False, session=None):
     """
     Get transform input output maps.
 
     :param transform_id: transform id.
     """
     contents = orm_contents.get_contents_by_request_transform(transform_id=transform_id, session=session)
     ret = {}
     for content in contents:
         map_id = content['map_id']
-        if map_id not in ret:
-            ret[map_id] = {'inputs_dependency': [], 'inputs': [], 'outputs': [], 'logs': [], 'others': []}
-
+        if not with_sub_map_id:
+            if map_id not in ret:
+                ret[map_id] = {'inputs_dependency': [], 'inputs': [], 'outputs': [], 'logs': [], 'others': []}
+        else:
+            sub_map_id = content['sub_map_id']
+            if map_id not in ret:
+                ret[map_id] = {}
+            if sub_map_id not in ret[map_id]:
+                ret[map_id][sub_map_id] = {'inputs_dependency': [], 'inputs': [], 'outputs': [], 'logs': [], 'others': []}
         """
         if content['coll_id'] in input_coll_ids:
             ret[map_id]['inputs'].append(content)
         elif content['coll_id'] in output_coll_ids:
             ret[map_id]['outputs'].append(content)
         elif content['coll_id'] in log_coll_ids:
             ret[map_id]['logs'].append(content)
         else:
             ret[map_id]['others'].append(content)
         """
-        if content['content_relation_type'] == ContentRelationType.Input:
-            ret[map_id]['inputs'].append(content)
-        elif content['content_relation_type'] == ContentRelationType.InputDependency:
-            ret[map_id]['inputs_dependency'].append(content)
-        elif content['content_relation_type'] == ContentRelationType.Output:
-            ret[map_id]['outputs'].append(content)
-        elif content['content_relation_type'] == ContentRelationType.Log:
-            ret[map_id]['logs'].append(content)
+        if not with_sub_map_id:
+            if content['content_relation_type'] == ContentRelationType.Input:
+                ret[map_id]['inputs'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.InputDependency:
+                ret[map_id]['inputs_dependency'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.Output:
+                ret[map_id]['outputs'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.Log:
+                ret[map_id]['logs'].append(content)
+            else:
+                ret[map_id]['others'].append(content)
         else:
-            ret[map_id]['others'].append(content)
+            if content['content_relation_type'] == ContentRelationType.Input:
+                ret[map_id][sub_map_id]['inputs'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.InputDependency:
+                ret[map_id][sub_map_id]['inputs_dependency'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.Output:
+                ret[map_id][sub_map_id]['outputs'].append(content)
+            elif content['content_relation_type'] == ContentRelationType.Log:
+                ret[map_id][sub_map_id]['logs'].append(content)
+            else:
+                ret[map_id][sub_map_id]['others'].append(content)
     return ret
 
 
 def release_inputs(to_release_inputs):
     update_contents = []
     for to_release in to_release_inputs:
         contents = orm_contents.get_input_contents(request_id=to_release['request_id'],
@@ -623,7 +641,17 @@
                                                                            'workload_id': coll['workload_id'],
                                                                            'scope': coll['scope'], 'name': coll['name']})
                     elif coll['relation_type'] == CollectionRelationType.Output:
                         work_name_to_coll_map[work_name]['outputs'].append({'coll_id': coll['coll_id'], 'transform_id': coll['transform_id'],
                                                                             'workload_id': coll['workload_id'],
                                                                             'scope': coll['scope'], 'name': coll['name']})
     return work_name_to_coll_map
+
+
+@read_session
+def get_num_active_transforms(active_status=None, session=None):
+    return orm_transforms.get_num_active_transforms(active_status=active_status, session=session)
+
+
+@read_session
+def get_active_transforms(active_status=None, session=None):
+    return orm_transforms.get_active_transforms(active_status=active_status, session=session)
```

### Comparing `idds-server-1.2.9/lib/idds/core/workprogress.py` & `idds-server-1.3.0/lib/idds/core/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/alembic/env.py` & `idds-server-1.3.0/lib/idds/orm/base/alembic/env.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py` & `idds-server-1.3.0/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py` & `idds-server-1.3.0/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/enum.py` & `idds-server-1.3.0/lib/idds/orm/base/enum.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/models.py` & `idds-server-1.3.0/lib/idds/orm/base/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                                    WorkprogressStatus, WorkprogressLocking,
                                    TransformType, TransformStatus, TransformLocking,
                                    ProcessingStatus, ProcessingLocking,
                                    CollectionStatus, CollectionLocking, CollectionType,
                                    CollectionRelationType, ContentType, ContentRelationType,
                                    ContentStatus, ContentFetchStatus, ContentLocking, GranularityType,
                                    MessageType, MessageStatus, MessageLocking,
-                                   MessageSource, MessageDestination,
+                                   MessageSource, MessageDestination, ThrottlerStatus,
                                    CommandType, CommandStatus, CommandLocking,
                                    CommandLocation, HealthStatus)
 from idds.common.event import (EventType, EventStatus)
 from idds.common.utils import date_to_str
 from idds.orm.base.enum import EnumSymbol
 from idds.orm.base.types import JSON, JSONString, EnumWithValue
 from idds.orm.base.session import BASE, DEFAULT_SCHEMA_NAME
@@ -154,14 +154,15 @@
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
     max_new_retries = Column(Integer(), default=3)
     max_update_retries = Column(Integer(), default=0)
     new_poll_period = Column(Interval(), default=datetime.timedelta(seconds=1))
     update_poll_period = Column(Interval(), default=datetime.timedelta(seconds=10))
+    site = Column(String(50))
     errors = Column(JSONString(1024))
     _request_metadata = Column('request_metadata', JSON())
     _processing_metadata = Column('processing_metadata', JSON())
 
     @property
     def request_metadata(self):
         if self._request_metadata:
@@ -238,14 +239,15 @@
             del values['processing_metadata']
         super(Request, self).update(values, flush, session)
 
     __table_args__ = (PrimaryKeyConstraint('request_id', name='REQUESTS_PK'),
                       CheckConstraint('status IS NOT NULL', name='REQUESTS_STATUS_ID_NN'),
                       # UniqueConstraint('name', 'scope', 'requester', 'request_type', 'transform_tag', 'workload_id', name='REQUESTS_NAME_SCOPE_UQ '),
                       Index('REQUESTS_SCOPE_NAME_IDX', 'name', 'scope', 'workload_id'),
+                      Index('REQUESTS_STATUS_SITE', 'status', 'site', 'request_id'),
                       Index('REQUESTS_STATUS_PRIO_IDX', 'status', 'priority', 'request_id', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
                       Index('REQUESTS_STATUS_POLL_IDX', 'status', 'priority', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at', 'request_id'))
 
 
 class Workprogress(BASE, ModelBase):
     """Represents a workprogress which monitors the progress of a workflow"""
     __tablename__ = 'workprogresses'
@@ -302,14 +304,15 @@
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
     max_new_retries = Column(Integer(), default=3)
     max_update_retries = Column(Integer(), default=0)
     new_poll_period = Column(Interval(), default=datetime.timedelta(seconds=1))
     update_poll_period = Column(Interval(), default=datetime.timedelta(seconds=10))
+    site = Column(String(50))
     name = Column(String(NAME_LENGTH))
     errors = Column(JSONString(1024))
     _transform_metadata = Column('transform_metadata', JSON())
     _running_metadata = Column('running_metadata', JSON())
 
     @property
     def transform_metadata(self):
@@ -365,14 +368,15 @@
         super(Transform, self).update(values, flush, session)
 
     __table_args__ = (PrimaryKeyConstraint('transform_id', name='TRANSFORMS_PK'),
                       CheckConstraint('status IS NOT NULL', name='TRANSFORMS_STATUS_ID_NN'),
                       Index('TRANSFORMS_TYPE_TAG_IDX', 'transform_type', 'transform_tag', 'transform_id'),
                       Index('TRANSFORMS_STATUS_UPDATED_AT_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
                       Index('TRANSFORMS_REQ_IDX', 'request_id', 'transform_id'),
+                      Index('TRANSFORMS_STATUS_SITE', 'status', 'site', 'request_id', 'transform_id'),
                       Index('TRANSFORMS_STATUS_POLL_IDX', 'status', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at', 'transform_id'))
 
 
 class Workprogress2transform(BASE, ModelBase):
     """Represents a workprogress to transform"""
     __tablename__ = 'wp2transforms'
     workprogress_id = Column(BigInteger().with_variant(Integer, "sqlite"), primary_key=True)
@@ -407,14 +411,15 @@
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
     max_new_retries = Column(Integer(), default=3)
     max_update_retries = Column(Integer(), default=0)
     new_poll_period = Column(Interval(), default=datetime.timedelta(seconds=1))
     update_poll_period = Column(Interval(), default=datetime.timedelta(seconds=10))
+    site = Column(String(50))
     errors = Column(JSONString(1024))
     _processing_metadata = Column('processing_metadata', JSON())
     _running_metadata = Column('running_metadata', JSON())
     output_metadata = Column(JSON())
 
     @property
     def processing_metadata(self):
@@ -469,14 +474,15 @@
             del values['running_metadata']
         super(Transform, self).update(values, flush, session)
 
     __table_args__ = (PrimaryKeyConstraint('processing_id', name='PROCESSINGS_PK'),
                       ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='PROCESSINGS_TRANSFORM_ID_FK'),
                       CheckConstraint('status IS NOT NULL', name='PROCESSINGS_STATUS_ID_NN'),
                       CheckConstraint('transform_id IS NOT NULL', name='PROCESSINGS_TRANSFORM_ID_NN'),
+                      Index('PROCESSINGS_STATUS_SITE', 'status', 'site', 'request_id', 'transform_id', 'processing_id'),
                       Index('PROCESSINGS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
                       Index('PROCESSINGS_STATUS_POLL_IDX', 'status', 'processing_id', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at'))
 
 
 class Collection(BASE, ModelBase):
     """Represents a collection"""
     __tablename__ = 'collections'
@@ -528,14 +534,16 @@
     __tablename__ = 'contents'
     content_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('CONTENT_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
     transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     coll_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
     map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0, nullable=False)
+    sub_map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0)
+    dep_sub_map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0)
     content_dep_id = Column(BigInteger())
     scope = Column(String(SCOPE_LENGTH))
     name = Column(String(LONG_NAME_LENGTH))
     min_id = Column(Integer(), default=0)
     max_id = Column(Integer(), default=0)
     content_type = Column(EnumWithValue(ContentType), nullable=False)
     content_relation_type = Column(EnumWithValue(ContentRelationType), default=0, nullable=False)
@@ -544,26 +552,31 @@
     locking = Column(EnumWithValue(ContentLocking), nullable=False)
     bytes = Column(Integer())
     md5 = Column(String(32))
     adler32 = Column(String(8))
     processing_id = Column(Integer())
     storage_id = Column(Integer())
     retries = Column(Integer(), default=0)
+    external_coll_id = Column(BigInteger())
+    external_content_id = Column(BigInteger())
+    external_event_id = Column(BigInteger())
+    external_event_status = Column(EnumWithValue(ContentStatus))
     path = Column(String(4000))
     created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
     updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
     accessed_at = Column("accessed_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
     expired_at = Column("expired_at", DateTime)
     content_metadata = Column(JSONString(100))
 
     __table_args__ = (PrimaryKeyConstraint('content_id', name='CONTENTS_PK'),
                       # UniqueConstraint('name', 'scope', 'coll_id', 'content_type', 'min_id', 'max_id', name='CONTENT_SCOPE_NAME_UQ'),
                       # UniqueConstraint('name', 'scope', 'coll_id', 'min_id', 'max_id', name='CONTENT_SCOPE_NAME_UQ'),
                       # UniqueConstraint('content_id', 'coll_id', name='CONTENTS_UQ'),
-                      UniqueConstraint('transform_id', 'coll_id', 'map_id', 'name', 'min_id', 'max_id', name='CONTENT_ID_UQ'),
+                      # UniqueConstraint('transform_id', 'coll_id', 'map_id', 'name', 'min_id', 'max_id', name='CONTENT_ID_UQ'),
+                      UniqueConstraint('transform_id', 'coll_id', 'map_id', 'sub_map_id', 'dep_sub_map_id', 'content_relation_type', 'name', 'min_id', 'max_id', name='CONTENT_ID_UQ'),
                       ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='CONTENTS_TRANSFORM_ID_FK'),
                       ForeignKeyConstraint(['coll_id'], ['collections.coll_id'], name='CONTENTS_COLL_ID_FK'),
                       CheckConstraint('status IS NOT NULL', name='CONTENTS_STATUS_ID_NN'),
                       CheckConstraint('coll_id IS NOT NULL', name='CONTENTS_COLL_ID_NN'),
                       Index('CONTENTS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'created_at'),
                       Index('CONTENTS_ID_NAME_IDX', 'coll_id', 'scope', 'name', 'status'),
                       Index('CONTENTS_DEP_IDX', 'request_id', 'transform_id', 'content_dep_id'),
@@ -707,16 +720,18 @@
     destination = Column(EnumWithValue(MessageDestination), nullable=False)
     request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
     workload_id = Column(Integer())
     transform_id = Column(Integer())
     processing_id = Column(Integer())
     num_contents = Column(Integer())
     retries = Column(Integer(), default=0)
+    fetching_id = Column(Integer())
     created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
     updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
+    poll_period = Column(Interval(), default=datetime.timedelta(seconds=300), nullable=False)
     msg_content = Column(JSON())
 
     __table_args__ = (PrimaryKeyConstraint('msg_id', name='MESSAGES_PK'),
                       Index('MESSAGES_TYPE_ST_IDX', 'msg_type', 'status', 'destination', 'request_id'),
                       Index('MESSAGES_TYPE_ST_TF_IDX', 'msg_type', 'status', 'destination', 'transform_id'),
                       Index('MESSAGES_TYPE_ST_PR_IDX', 'msg_type', 'status', 'destination', 'processing_id'),
                       Index('MESSAGES_ST_IDX', 'status', 'destination', 'created_at'),
@@ -879,14 +894,33 @@
     processing_at = Column("processing_at", DateTime, default=None)
     processed_at = Column("processed_at", DateTime, default=None)
     content = Column(JSON())
 
     __table_args__ = (PrimaryKeyConstraint('event_id', name='EVENTS_AR_PK'),)
 
 
+class Throttler(BASE, ModelBase):
+    """Represents the operations events"""
+    __tablename__ = 'throttlers'
+    throttler_id = Column(BigInteger(), primary_key=True)
+    site = Column(String(50), nullable=False)
+    status = Column(EnumWithValue(ThrottlerStatus), nullable=False)
+    num_requests = Column(Integer())
+    num_transforms = Column(Integer())
+    num_processings = Column(Integer())
+    new_contents = Column(Integer())
+    queue_contents = Column(Integer())
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
+    others = Column(JSON())
+
+    __table_args__ = (PrimaryKeyConstraint('throttler_id', name='THROTTLER_PK'),
+                      UniqueConstraint('site', name='THROTTLER_SITE_UQ'))
+
+
 def create_trigger():
     func = DDL("""
         SET search_path TO %s;
         CREATE OR REPLACE FUNCTION update_dep_contents_status()
         RETURNS TRIGGER AS $$
         BEGIN
             UPDATE %s.contents set substatus = old.substatus where %s.contents.content_dep_id = old.content_id;
@@ -1015,28 +1049,28 @@
 
 def register_models(engine):
     """
     Creates database tables for all models with the given engine
     """
 
     # models = (Request, Workprogress, Transform, Workprogress2transform, Processing, Collection, Content, Health, Message)
-    models = (Request, Transform, Processing, Collection, Content, Content_update, Content_ext, Health, Message, Command)
+    models = (Request, Transform, Processing, Collection, Content, Content_update, Content_ext, Health, Message, Command, Throttler)
 
     create_proc_to_update_contents()
 
     for model in models:
         # if not engine.has_table(model.__tablename__, model.metadata.schema):
         model.metadata.create_all(engine)   # pylint: disable=maybe-no-member
 
 
 def unregister_models(engine):
     """
     Drops database tables for all models with the given engine
     """
 
     # models = (Request, Workprogress, Transform, Workprogress2transform, Processing, Collection, Content, Health, Message)
-    models = (Request, Transform, Processing, Collection, Content, Content_update, Content_ext, Health, Message, Command)
+    models = (Request, Transform, Processing, Collection, Content, Content_update, Content_ext, Health, Message, Command, Throttler)
 
     drop_proc_to_update_contents()
 
     for model in models:
         model.metadata.drop_all(engine)   # pylint: disable=maybe-no-member
```

### Comparing `idds-server-1.2.9/lib/idds/orm/base/session.py` & `idds-server-1.3.0/lib/idds/orm/base/session.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/types.py` & `idds-server-1.3.0/lib/idds/orm/base/types.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/base/utils.py` & `idds-server-1.3.0/lib/idds/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/collections.py` & `idds-server-1.3.0/lib/idds/orm/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/commands.py` & `idds-server-1.3.0/lib/idds/orm/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/contents.py` & `idds-server-1.3.0/lib/idds/orm/contents.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         raise exceptions.NoObject('No record can be found with (coll_id=%s, name=%s): %s' %
                                   (coll_id, name, error))
     except Exception as error:
         raise error
 
 
 @read_session
-def get_contents_by_request_transform(request_id=None, transform_id=None, workload_id=None, status=None, status_updated=False, session=None):
+def get_contents_by_request_transform(request_id=None, transform_id=None, workload_id=None, status=None, map_id=None, status_updated=False, session=None):
     """
     Get content or raise a NoObject exception.
 
     :param request_id: request id.
     :param transform_id: transform id.
     :param workload_id: workload id.
 
@@ -360,14 +360,16 @@
             query = query.filter(models.Content.request_id == request_id)
         if transform_id:
             query = query.filter(models.Content.transform_id == transform_id)
         if workload_id:
             query = query.filter(models.Content.workload_id == workload_id)
         if status is not None:
             query = query.filter(models.Content.substatus.in_(status))
+        if map_id:
+            query = query.filter(models.Content.map_id == map_id)
         if status_updated:
             query = query.filter(models.Content.status != models.Content.substatus)
         query = query.order_by(asc(models.Content.request_id), asc(models.Content.transform_id), asc(models.Content.map_id))
 
         tmp = query.all()
         rets = []
         if tmp:
@@ -378,38 +380,73 @@
         raise exceptions.NoObject('No record can be found with (transform_id=%s): %s' %
                                   (transform_id, error))
     except Exception as error:
         raise error
 
 
 @read_session
-def get_content_status_statistics(coll_id=None, session=None):
+def get_content_status_statistics(coll_id=None, transform_ids=None, session=None):
     """
     Get statistics group by status
 
     :param coll_id: Collection id.
     :param session: The database session in use.
 
     :returns: statistics group by status, as a dict.
     """
     try:
+        if transform_ids and not isinstance(transform_ids, (list, tuple)):
+            transform_ids = [transform_ids]
+        if transform_ids and len(transform_ids) == 1:
+            transform_ids = [transform_ids[0], transform_ids[0]]
+
         query = session.query(models.Content.status, func.count(models.Content.content_id))
         if coll_id:
             query = query.filter(models.Content.coll_id == coll_id)
+        if transform_ids:
+            query = query.filter(models.Content.transform_id.in_(transform_ids))
+
         query = query.group_by(models.Content.status)
         tmp = query.all()
         rets = {}
         if tmp:
             for status, count in tmp:
                 rets[status] = count
         return rets
     except Exception as error:
         raise error
 
 
+@read_session
+def get_content_status_statistics_by_relation_type(transform_ids=None, session=None):
+    """
+    Get statistics group by status
+
+    :param coll_id: Collection id.
+    :param session: The database session in use.
+
+    :returns: statistics group by status, as a dict.
+    """
+    try:
+        if transform_ids and not isinstance(transform_ids, (list, tuple)):
+            transform_ids = [transform_ids]
+        if transform_ids and len(transform_ids) == 1:
+            transform_ids = [transform_ids[0], transform_ids[0]]
+
+        query = session.query(models.Content.status, models.Content.content_relation_type, models.Content.transform_id, func.count(models.Content.content_id))
+        if transform_ids:
+            query = query.filter(models.Content.transform_id.in_(transform_ids))
+
+        query = query.group_by(models.Content.status, models.Content.content_relation_type, models.Content.transform_id)
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
+
+
 @transactional_session
 def update_content(content_id, parameters, session=None):
     """
     update a content.
 
     :param content_id: the content id.
     :param parameters: A dictionary of parameters.
```

### Comparing `idds-server-1.2.9/lib/idds/orm/events.py` & `idds-server-1.3.0/lib/idds/orm/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/health.py` & `idds-server-1.3.0/lib/idds/orm/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/orm/messages.py` & `idds-server-1.3.0/lib/idds/orm/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 operations related to Messages.
 """
 
 import datetime
 import re
 import copy
 
-from sqlalchemy import or_
+from sqlalchemy import or_, asc
 from sqlalchemy.exc import DatabaseError, IntegrityError
 
 from idds.common import exceptions
 from idds.common.constants import MessageDestination
 from idds.orm.base import models
 from idds.orm.base.session import read_session, transactional_session
 
@@ -113,16 +113,16 @@
         else:
             raise exceptions.DatabaseException('Could not persist message: %s' % str(e))
 
 
 @read_session
 def retrieve_messages(bulk_size=1000, msg_type=None, status=None, source=None,
                       destination=None, request_id=None, workload_id=None,
-                      transform_id=None, processing_id=None,
-                      retries=None, delay=None, session=None):
+                      transform_id=None, processing_id=None, fetching_id=None,
+                      use_poll_period=False, retries=None, delay=None, session=None):
     """
     Retrieve up to $bulk messages.
 
     :param bulk: Number of messages as an integer.
     :param msg_type: Return only specified msg_type.
     :param status: The status about the message
     :param source: The source where the message is from.
@@ -161,23 +161,28 @@
             query = query.filter_by(transform_id=transform_id)
         if processing_id is not None:
             query = query.filter_by(processing_id=processing_id)
         if retries:
             query = query.filter_by(retries=retries)
         if delay:
             query = query.filter(models.Message.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=delay))
+        elif use_poll_period:
+            query = query.filter(models.Message.updated_at + models.Message.poll_period <= datetime.datetime.utcnow())
+
+        query = query.order_by(asc(models.Message.updated_at))
 
         if bulk_size:
             query = query.order_by(models.Message.created_at).limit(bulk_size)
         # query = query.with_for_update(nowait=True)
 
         tmp = query.all()
         if tmp:
             for t in tmp:
-                messages.append(t.to_dict())
+                message = t.to_dict()
+                messages.append(message)
         return messages
     except IntegrityError as e:
         raise exceptions.DatabaseException(e.args)
 
 
 @transactional_session
 def delete_messages(messages, session=None):
```

### Comparing `idds-server-1.2.9/lib/idds/orm/processings.py` & `idds-server-1.3.0/lib/idds/orm/processings.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 operations related to Processings.
 """
 
 import datetime
 
 import sqlalchemy
+from sqlalchemy import func
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.sql.expression import asc
 
 from idds.common import exceptions
 from idds.common.constants import ProcessingStatus, ProcessingLocking, GranularityType
 from idds.orm.base.session import read_session, transactional_session
 from idds.orm.base import models
@@ -420,7 +421,46 @@
         status = [status]
     if len(status) == 1:
         status = [status[0], status[0]]
 
     params = {'next_poll_at': datetime.datetime.utcnow()}
     session.query(models.Processing).filter(models.Processing.status.in_(status))\
            .update(params, synchronize_session=False)
+
+
+@read_session
+def get_num_active_processings(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Processing.status, models.Processing.site, func.count(models.Processing.processing_id))
+        if active_status:
+            query = query.filter(models.Processing.status.in_(active_status))
+        query = query.group_by(models.Processing.status, models.Processing.site)
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
+
+
+@read_session
+def get_active_processings(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Processing.request_id,
+                              models.Processing.transform_id,
+                              models.Processing.processing_id,
+                              models.Processing.site,
+                              models.Processing.status)
+        if active_status:
+            query = query.filter(models.Processing.status.in_(active_status))
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
```

### Comparing `idds-server-1.2.9/lib/idds/orm/requests.py` & `idds-server-1.3.0/lib/idds/orm/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 operations related to Requests.
 """
 
 import datetime
 import random
 
 import sqlalchemy
-from sqlalchemy import and_
+from sqlalchemy import and_, func
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.sql.expression import asc, desc
 
 from idds.common import exceptions
 from idds.common.constants import RequestType, RequestStatus, RequestLocking
 from idds.orm.base.session import read_session, transactional_session
 from idds.orm.base import models
@@ -825,16 +825,18 @@
             query = query.filter(models.Request.request_id.in_(request_ids))
         if locking:
             query = query.filter(models.Request.locking == RequestLocking.Idle)
 
         if locking_for_update:
             query = query.with_for_update(skip_locked=True)
         else:
-            query = query.order_by(asc(models.Request.updated_at))\
-                         .order_by(desc(models.Request.priority))
+            # query = query.order_by(asc(models.Request.updated_at))\
+            #              .order_by(desc(models.Request.priority))
+            query = query.order_by(desc(models.Request.priority))\
+                         .order_by(asc(models.Request.updated_at))
 
         if bulk_size:
             query = query.limit(bulk_size)
 
         tmp = query.all()
         rets = []
         if tmp:
@@ -977,7 +979,42 @@
         query = query.filter(models.Request.status.in_(status))
     query = query.filter(models.Request.updated_at <= datetime.datetime.utcnow() - datetime.timedelta(days=older_than))
     query = query.order_by(desc(models.Request.request_id))
     ret = query.first()
     if ret:
         return ret[0]
     return ret
+
+
+@read_session
+def get_num_active_requests(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Request.status, models.Request.site, func.count(models.Request.request_id))
+        if active_status:
+            query = query.filter(models.Request.status.in_(active_status))
+        query = query.group_by(models.Request.status, models.Request.site)
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
+
+
+@read_session
+def get_active_requests(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Request.request_id, models.Request.status, models.Request.site)
+        if active_status:
+            query = query.filter(models.Request.status.in_(active_status))
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
```

### Comparing `idds-server-1.2.9/lib/idds/orm/transforms.py` & `idds-server-1.3.0/lib/idds/orm/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 operations related to Transform.
 """
 
 import datetime
 
 import sqlalchemy
-from sqlalchemy import and_
+from sqlalchemy import and_, func
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.sql.expression import asc, desc
 
 from idds.common import exceptions
 from idds.common.constants import TransformStatus, TransformLocking, CollectionRelationType
 from idds.orm.base.session import read_session, transactional_session
 from idds.orm.base import models
@@ -505,7 +505,45 @@
         status = [status]
     if len(status) == 1:
         status = [status[0], status[0]]
 
     params = {'next_poll_at': datetime.datetime.utcnow()}
     session.query(models.Transform).filter(models.Transform.status.in_(status))\
            .update(params, synchronize_session=False)
+
+
+@read_session
+def get_num_active_transforms(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Transform.status, models.Transform.site, func.count(models.Transform.transform_id))
+        if active_status:
+            query = query.filter(models.Transform.status.in_(active_status))
+        query = query.group_by(models.Transform.status, models.Transform.site)
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
+
+
+@read_session
+def get_active_transforms(active_status=None, session=None):
+    if active_status and not isinstance(active_status, (list, tuple)):
+        active_status = [active_status]
+    if active_status and len(active_status) == 1:
+        active_status = [active_status[0], active_status[0]]
+
+    try:
+        query = session.query(models.Transform.request_id,
+                              models.Transform.transform_id,
+                              models.Transform.site,
+                              models.Transform.status)
+        if active_status:
+            query = query.filter(models.Transform.status.in_(active_status))
+        tmp = query.all()
+        return tmp
+    except Exception as error:
+        raise error
```

### Comparing `idds-server-1.2.9/lib/idds/orm/workprogress.py` & `idds-server-1.3.0/lib/idds/orm/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/app.py` & `idds-server-1.3.0/lib/idds/rest/v1/app.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/auth.py` & `idds-server-1.3.0/lib/idds/rest/v1/auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/cacher.py` & `idds-server-1.3.0/lib/idds/rest/v1/cacher.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/catalog.py` & `idds-server-1.3.0/lib/idds/rest/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/controller.py` & `idds-server-1.3.0/lib/idds/rest/v1/controller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/hyperparameteropt.py` & `idds-server-1.3.0/lib/idds/rest/v1/hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/logs.py` & `idds-server-1.3.0/lib/idds/rest/v1/logs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/messages.py` & `idds-server-1.3.0/lib/idds/rest/v1/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/monitor.py` & `idds-server-1.3.0/lib/idds/rest/v1/monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/ping.py` & `idds-server-1.3.0/lib/idds/rest/v1/ping.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/requests.py` & `idds-server-1.3.0/lib/idds/rest/v1/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/rest/v1/utils.py` & `idds-server-1.3.0/lib/idds/rest/v1/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/activelearning_test.py` & `idds-server-1.3.0/lib/idds/tests/activelearning_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/auth_test_script.py` & `idds-server-1.3.0/lib/idds/tests/auth_test_script.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/cacher_test.py` & `idds-server-1.3.0/lib/idds/tests/cacher_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/catalog_test.py` & `idds-server-1.3.0/lib/idds/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/client_test.py` & `idds-server-1.3.0/lib/idds/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/common.py` & `idds-server-1.3.0/lib/idds/tests/common.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/core_tests.py` & `idds-server-1.3.0/lib/idds/tests/core_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,21 @@
 # reqs = get_requests(request_id=373602, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=376086, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=380474, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=381520, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=28182323, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=385554, with_request=True, with_detail=False, with_metadata=True)
 reqs = get_requests(request_id=479187, with_request=True, with_detail=False, with_metadata=True)
+reqs = get_requests(request_id=4498, with_request=True, with_detail=False, with_metadata=True)
+reqs = get_requests(request_id=4615, with_request=True, with_detail=False, with_metadata=True)
 for req in reqs:
     # print(req['request_id'])
     # print(req)
     # print(rets)
-    # print(json_dumps(req, sort_keys=True, indent=4))
+    print(json_dumps(req, sort_keys=True, indent=4))
     # show_works(req)
     pass
     if 'build_workflow' in req['request_metadata']:
         workflow = req['request_metadata']['build_workflow']
         # workflow.get_new_works()
         print(workflow.runs.keys())
         # print(workflow.runs["1"])
@@ -218,21 +220,24 @@
     print_workflow_template(workflow)
 
     # workflow.sync_works()
 
     print("workflow template")
     print(json_dumps(workflow.template, sort_keys=True, indent=4))
 
+
+"""
 sys.exit(0)
 
 reqs = get_requests(request_id=28182323, with_request=False, with_detail=True, with_metadata=False)
 for req in reqs:
     print(json_dumps(req, sort_keys=True, indent=4))
 
 # sys.exit(0)
+"""
 
 """
 # reqs = get_requests()
 # print(len(reqs))
 for req in reqs:
     if req['request_id'] == 113:
         # print(req)
@@ -240,15 +245,15 @@
         # print(json_dumps(req, sort_keys=True, indent=4))
         pass
 
 sys.exit(0)
 
 """
 
-
+"""
 tfs = get_transforms(request_id=470)
 # tfs = get_transforms(transform_id=350723)
 for tf in tfs:
     # print(tf)
     # print(tf['transform_metadata']['work'].to_dict())
     # print(tf)
     print(json_dumps(tf, sort_keys=True, indent=4))
@@ -256,15 +261,15 @@
     print(tf['transform_metadata']['work_name'])
     print(tf['transform_metadata']['work'].num_run)
     print(tf['transform_metadata']['work'].task_name)
     print(tf['transform_metadata']['work'].output_data)
     pass
 
 sys.exit(0)
-
+"""
 
 """
 msgs = retrieve_messages(workload_id=25972557)
 number_contents = 0
 for msg in msgs:
     # if msg['msg_id'] in [323720]:
     # if True:
@@ -277,15 +282,15 @@
                 number_contents += 1
     pass
 print(number_contents)
 
 sys.exit(0)
 """
 
-prs = get_processings(request_id=373602)
+prs = get_processings(request_id=4615)
 # prs = get_processings(transform_id=350723)
 i = 0
 for pr in prs:
     # if pr['request_id'] == 91:
     print("processing_number: %s" % i)
     i += 1
     print(json_dumps(pr, sort_keys=True, indent=4))
```

### Comparing `idds-server-1.2.9/lib/idds/tests/core_tests_dep_id.py` & `idds-server-1.3.0/lib/idds/tests/core_tests_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/core_tests_stat.py` & `idds-server-1.3.0/lib/idds/tests/core_tests_stat.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/datacarousel_test.py` & `idds-server-1.3.0/lib/idds/tests/datacarousel_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/doma_build_test.py` & `idds-server-1.3.0/lib/idds/tests/doma_build_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/find_dependencies.py` & `idds-server-1.3.0/lib/idds/tests/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/fix_content_dep_id.py` & `idds-server-1.3.0/lib/idds/tests/fix_content_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/fix_trasnform_name.py` & `idds-server-1.3.0/lib/idds/tests/fix_trasnform_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/hyperparameteropt_bayesian_test.py` & `idds-server-1.3.0/lib/idds/tests/hyperparameteropt_bayesian_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/hyperparameteropt_client_test.py` & `idds-server-1.3.0/lib/idds/tests/hyperparameteropt_client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/hyperparameteropt_docker_local_test.py` & `idds-server-1.3.0/lib/idds/tests/hyperparameteropt_docker_local_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/hyperparameteropt_docker_test.py` & `idds-server-1.3.0/lib/idds/tests/hyperparameteropt_docker_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/hyperparameteropt_nevergrad_test.py` & `idds-server-1.3.0/lib/idds/tests/hyperparameteropt_nevergrad_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/jsonload_test.py` & `idds-server-1.3.0/lib/idds/tests/jsonload_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/kill_workflow_task.py` & `idds-server-1.3.0/lib/idds/tests/kill_workflow_task.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/logs_test.py` & `idds-server-1.3.0/lib/idds/tests/logs_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/match_test.py` & `idds-server-1.3.0/lib/idds/tests/match_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/message_test.py` & `idds-server-1.3.0/lib/idds/tests/message_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/message_test1.py` & `idds-server-1.3.0/lib/idds/tests/message_test1.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/migrating_requests_v1_to_v2.py` & `idds-server-1.3.0/lib/idds/tests/migrating_requests_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/panda_iam_test.py` & `idds-server-1.3.0/lib/idds/tests/panda_iam_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/panda_test.py` & `idds-server-1.3.0/lib/idds/tests/panda_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,32 @@
 import os   # noqa E402
 import sys
 import datetime
 
 os.environ['PANDA_URL'] = 'http://pandaserver-doma.cern.ch:25080/server/panda'
 os.environ['PANDA_URL_SSL'] = 'https://pandaserver-doma.cern.ch:25443/server/panda'
 
-os.environ['PANDA_URL'] = 'http://rubin-panda-server-dev.slac.stanford.edu:80/server/panda'
-os.environ['PANDA_URL_SSL'] = 'https://rubin-panda-server-dev.slac.stanford.edu:8443/server/panda'
+os.environ['PANDA_BEHIND_REAL_LB'] = "1"
+# os.environ['PANDA_URL'] = 'http://rubin-panda-server-dev.slac.stanford.edu:80/server/panda'
+# os.environ['PANDA_URL_SSL'] = 'https://rubin-panda-server-dev.slac.stanford.edu:8443/server/panda'
 
 from pandaclient import Client  # noqa E402
 
+
+task_ids = [i for i in range(157023, 157050)]
+task_ids = []
+for task_id in task_ids:
+    print("Killing %s" % task_id)
+    ret = Client.killTask(task_id)
+    print(ret)
+
+# jobids = [52690679]
+jobids = [9]
 """
-jobids = [1408118]
-jobs_list_status = Client.getJobStatus(jobids, verbose=0)
+jobs_list_status = Client.getJobStatus(jobids, verbose=1)
 print(jobs_list_status)
 jobs_list = jobs_list_status[1]
 print(jobs_list)
 for job_info in jobs_list:
     if job_info is not None:
         # if job_info.Files and len(job_info.Files) > 0:
         print(job_info)
@@ -26,15 +36,32 @@
         print(job_info.Files)
         print(job_info.Files[0])
         for f in job_info.Files:
             # print(dir(f))
             print(f._attributes)
             print(f.values())
             print(f.type)
+"""
+
+# ret = Client.getFullJobStatus(ids=jobids, verbose=False)
+# print(ret)
+
+jediTaskID = 156668
+ret = Client.get_files_in_datasets(jediTaskID, verbose=False)
+print(ret)
+
+print("get events")
+panda_ids = [{'task_id': 157016, 'panda_id': 53943290}]
+panda_ids = [{'task_id': 157076, 'panda_id': 53943504}]
+ret = Client.get_events_status(panda_ids, verbose=True)
+print(ret)
+
+# sys.exit(0)
 
+"""
 jediTaskID = 10517    # 10607
 jediTaskID = 146329
 ret = Client.getJediTaskDetails({'jediTaskID': jediTaskID}, True, True, verbose=False)
 print(ret)
 # ret = Client.getTaskStatus(jediTaskID, verbose=False)
 # print(ret)
 
@@ -63,30 +90,37 @@
         print(len(ret[1]))
     ret_jobs = ret_jobs + ret[1]
     print(len(ret_jobs))
 """
 
 # sys.exit(0)
 
-"""
-jediTaskID = 998
+
+jediTaskID = 152096
+# jediTaskID = 154357
+print(jediTaskID)
+
+ret = Client.getTaskStatus(jediTaskID)
+print(ret)
+
 ret = Client.getPandaIDsWithTaskID(jediTaskID, verbose=False)
-# print(ret)
+print(ret)
 jobids = ret[1]
-# print(jobids)
+print(jobids)
 
 ret = Client.getJobStatus(ids=jobids, verbose=False)
 print(ret)
 
 ret = Client.getFullJobStatus(ids=jobids, verbose=False)
-# print(ret)
+print(ret)
 
 ret = Client.getJediTaskDetails({'jediTaskID': jediTaskID}, True, True, verbose=False)
 print(ret)
-"""
+
+# sys.exit(0)
 
 task_ids = []
 # task_ids = [1565, 1566, 1567, 1568, 1570, 1572, 1575, 1576, 1579, 1580, 1581, 1582, 1584, 1585, 1586, 1587, 1588, 1589, 1590, 1591, 1592, 1593, 1597, 1598, 1599, 1601, 1602, 1603, 1604, 1607, 1608, 1609, 1610, 1611, 1612, 1613, 1617]
 # task_ids = [i for i in range(1091, 1104)] + [i for i in range(1274, 1392)]
 # task_ids = [812]
 # task_ids += [i for i in range(815, 822)]
 # task_ids = [827, 830, 913, 914, 916, 917, 1030, 1031, 1033, 1034, 1036, 1048, 1090, 1392]
@@ -107,14 +141,16 @@
 # task_ids = [i for i in range(150050, 150065)]
 # task_ids = [150607, 150619, 150649, 150637, 150110, 150111]
 # task_ids = [150864, 150897, 150910]
 # task_ids = [151114, 151115]
 # task_ids = [i for i in range(151444, 151453)]
 task_ids = [i for i in range(45, 53)]
 # task_ids = []
+task_ids = [i for i in range(156974, 156981)]
+task_ids = [i for i in range(157023, 157050)]
 for task_id in task_ids:
     print("Killing %s" % task_id)
     Client.killTask(task_id)
 
 """
 jobids = []
 Client.getJobStatus(ids=jobids, verbose=False)
```

### Comparing `idds-server-1.2.9/lib/idds/tests/performance_test_with_cx_oracle.py` & `idds-server-1.3.0/lib/idds/tests/performance_test_with_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/performance_test_with_sqlalchemy.py` & `idds-server-1.3.0/lib/idds/tests/performance_test_with_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/relation_map_test.py` & `idds-server-1.3.0/lib/idds/tests/relation_map_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/rest_test.py` & `idds-server-1.3.0/lib/idds/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/run_sql.py` & `idds-server-1.3.0/lib/idds/tests/run_sql.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/scaling_checks.py` & `idds-server-1.3.0/lib/idds/tests/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/split_messages.py` & `idds-server-1.3.0/lib/idds/tests/split_messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_activelearning.py` & `idds-server-1.3.0/lib/idds/tests/test_activelearning.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_atlaspandawork.py` & `idds-server-1.3.0/lib/idds/tests/test_atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_auth.py` & `idds-server-1.3.0/lib/idds/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_big_request.py` & `idds-server-1.3.0/lib/idds/tests/test_big_request.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_catalog.py` & `idds-server-1.3.0/lib/idds/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_client.py` & `idds-server-1.3.0/lib/idds/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_datacarousel.py` & `idds-server-1.3.0/lib/idds/tests/test_datacarousel.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_domapanda.py` & `idds-server-1.3.0/lib/idds/tests/test_domapanda.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 task_cloud = 'US'
 
 task_queue = 'DOMA_LSST_GOOGLE_TEST'
 # task_queue = 'DOMA_LSST_GOOGLE_MERGE'
 # task_queue = 'SLAC_TEST'
 # task_queue = 'DOMA_LSST_SLAC_TEST'
 task_queue = 'SLAC_Rubin'
+# task_queue = 'SLAC_Rubin_Extra_Himem_32Cores'
 
 # task_cloud = 'EU'
 # task_queue = 'CC-IN2P3_TEST'
 
 # task_cloud = 'EU'
 # task_queue = 'LANCS_TEST'
 
@@ -133,42 +134,45 @@
 
     work1 = DomaPanDAWork(executable='echo',
                           primary_input_collection={'scope': 'pseudo_dataset', 'name': 'pseudo_input_collection#1'},
                           output_collections=[{'scope': 'pseudo_dataset', 'name': 'pseudo_output_collection#1'}],
                           log_collections=[], dependency_map=taskN1.dependencies,
                           task_name=taskN1.name, task_queue=task_queue,
                           encode_command_line=True,
+                          task_priority=981,
                           prodSourceLabel='managed',
                           task_log={"dataset": "PandaJob_#{pandaid}/",
                                     "destination": "local",
                                     "param_type": "log",
                                     "token": "local",
                                     "type": "template",
                                     "value": "log.tgz"},
                           task_cloud=task_cloud)
     work2 = DomaPanDAWork(executable='echo',
                           primary_input_collection={'scope': 'pseudo_dataset', 'name': 'pseudo_input_collection#2'},
                           output_collections=[{'scope': 'pseudo_dataset', 'name': 'pseudo_output_collection#2'}],
                           log_collections=[], dependency_map=taskN2.dependencies,
                           task_name=taskN2.name, task_queue=task_queue,
                           encode_command_line=True,
+                          task_priority=881,
                           prodSourceLabel='managed',
                           task_log={"dataset": "PandaJob_#{pandaid}/",
                                     "destination": "local",
                                     "param_type": "log",
                                     "token": "local",
                                     "type": "template",
                                     "value": "log.tgz"},
                           task_cloud=task_cloud)
     work3 = DomaPanDAWork(executable='echo',
                           primary_input_collection={'scope': 'pseudo_dataset', 'name': 'pseudo_input_collection#3'},
                           output_collections=[{'scope': 'pseudo_dataset', 'name': 'pseudo_output_collection#3'}],
                           log_collections=[], dependency_map=taskN3.dependencies,
                           task_name=taskN3.name, task_queue=task_queue,
                           encode_command_line=True,
+                          task_priority=781,
                           prodSourceLabel='managed',
                           task_log={"dataset": "PandaJob_#{pandaid}/",
                                     "destination": "local",
                                     "param_type": "log",
                                     "token": "local",
                                     "type": "template",
                                     "value": "log.tgz"},
```

### Comparing `idds-server-1.2.9/lib/idds/tests/test_domapanda_pandaclient.py` & `idds-server-1.3.0/lib/idds/tests/test_domapanda_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_domapanda_workflow.py` & `idds-server-1.3.0/lib/idds/tests/test_domapanda_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_get_dn.py` & `idds-server-1.3.0/lib/idds/tests/test_get_dn.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_hyperparameteropt.py` & `idds-server-1.3.0/lib/idds/tests/test_hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_logger.py` & `idds-server-1.3.0/lib/idds/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_merge_dict.py` & `idds-server-1.3.0/lib/idds/tests/test_merge_dict.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_migrate_requests.py` & `idds-server-1.3.0/lib/idds/tests/test_migrate_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,25 +55,28 @@
     old_request_id = 2816       # big tasks
     # old_request_id = 3178     # 125 tasks
     old_request_id = 3578
     old_request_id = 3612
     old_request_id = 3628
 
     old_request_ids = [3628]
+
+    # old_request_ids = [21]
+
     # old_request_id = 1
     # for old_request_id in [152]:
     # for old_request_id in [60]:    # noqa E115
     # for old_request_id in [200]:    # noqa E115
     for old_request_id in old_request_ids:    # noqa E115  # doma 183
         reqs = cm1.get_requests(request_id=old_request_id, with_metadata=True)
 
-        # cm2 = ClientManager(host=dev_host)
+        cm2 = ClientManager(host=dev_host)
         # cm2 = ClientManager(host=doma_host)
         # cm2 = ClientManager(host=atlas_host)
-        cm2 = ClientManager(host=slac_k8s_dev_host)
+        # cm2 = ClientManager(host=slac_k8s_dev_host)
         # cm2 = ClientManager(host=cern_k8s_dev_host)
         # print(reqs)
 
         print("num requests: %s" % len(reqs))
         for req in reqs[:1]:
             # print(req)
             # workflow = req['request_metadata']['workflow']
```

### Comparing `idds-server-1.2.9/lib/idds/tests/test_request_transform.py` & `idds-server-1.3.0/lib/idds/tests/test_request_transform.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_requests.py` & `idds-server-1.3.0/lib/idds/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_running_data.py` & `idds-server-1.3.0/lib/idds/tests/test_running_data.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_scaling.py` & `idds-server-1.3.0/lib/idds/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_transform_collection_content.py` & `idds-server-1.3.0/lib/idds/tests/test_transform_collection_content.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_transform_processing.py` & `idds-server-1.3.0/lib/idds/tests/test_transform_processing.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_workflow.py` & `idds-server-1.3.0/lib/idds/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_workflow_condition.py` & `idds-server-1.3.0/lib/idds/tests/test_workflow_condition.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/test_workflow_condition_v2.py` & `idds-server-1.3.0/lib/idds/tests/test_workflow_condition_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds/tests/trigger_release.py` & `idds-server-1.3.0/lib/idds/tests/trigger_release.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/lib/idds_server.egg-info/PKG-INFO` & `idds-server-1.3.0/lib/idds_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.2.9
+Version: 1.3.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.2.9/lib/idds_server.egg-info/SOURCES.txt` & `idds-server-1.3.0/lib/idds_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 bin/run-idds
 bin/run-idds-fake
 config_default/alembic.ini
 config_default/auth.cfg
 config_default/gacl
 config_default/httpd-idds-443-py39-cc7.conf
 config_default/idds.cfg
+config_default/logrotate_daemon
+config_default/logrotate_idds
 config_default/panda.cfg
 config_default/rucio.cfg
 config_default/supervisord_httpd.ini
 config_default/supervisord_idds.ini
 config_default/supervisord_iddsfake.ini
 config_default/supervisord_logrotate.ini
 config_default/supervisord_syslog-ng.ini
@@ -94,38 +96,44 @@
 lib/idds/core/catalog.py
 lib/idds/core/commands.py
 lib/idds/core/events.py
 lib/idds/core/health.py
 lib/idds/core/messages.py
 lib/idds/core/processings.py
 lib/idds/core/requests.py
+lib/idds/core/throttlers.py
 lib/idds/core/transforms.py
 lib/idds/core/workprogress.py
 lib/idds/orm/__init__.py
 lib/idds/orm/collections.py
 lib/idds/orm/commands.py
 lib/idds/orm/contents.py
 lib/idds/orm/events.py
 lib/idds/orm/health.py
 lib/idds/orm/messages.py
 lib/idds/orm/processings.py
 lib/idds/orm/requests.py
+lib/idds/orm/throttlers.py
 lib/idds/orm/transforms.py
 lib/idds/orm/workprogress.py
 lib/idds/orm/base/__init__.py
 lib/idds/orm/base/enum.py
 lib/idds/orm/base/models.py
 lib/idds/orm/base/session.py
 lib/idds/orm/base/types.py
 lib/idds/orm/base/utils.py
 lib/idds/orm/base/alembic/__init__.py
 lib/idds/orm/base/alembic/env.py
+lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
+lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
 lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
 lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
 lib/idds/orm/base/alembic/versions/__init__.py
+lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
+lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
 lib/idds/rest/__init__.py
 lib/idds/rest/v1/__init__.py
 lib/idds/rest/v1/app.py
 lib/idds/rest/v1/auth.py
 lib/idds/rest/v1/cacher.py
 lib/idds/rest/v1/catalog.py
 lib/idds/rest/v1/controller.py
@@ -168,26 +176,29 @@
 lib/idds/tests/performance_test_with_cx_oracle.py
 lib/idds/tests/performance_test_with_sqlalchemy.py
 lib/idds/tests/relation_map_test.py
 lib/idds/tests/rest_test.py
 lib/idds/tests/retry_processing.py
 lib/idds/tests/run_sql.py
 lib/idds/tests/scaling_checks.py
+lib/idds/tests/set_throttlers.py
 lib/idds/tests/split_messages.py
 lib/idds/tests/test_activelearning.py
 lib/idds/tests/test_atlaspandawork.py
 lib/idds/tests/test_auth.py
 lib/idds/tests/test_big_request.py
 lib/idds/tests/test_catalog.py
 lib/idds/tests/test_client.py
 lib/idds/tests/test_datacarousel.py
 lib/idds/tests/test_domapanda.py
+lib/idds/tests/test_domapanda_lsst_workflow.py
 lib/idds/tests/test_domapanda_pandaclient.py
 lib/idds/tests/test_domapanda_workflow.py
 lib/idds/tests/test_get_dn.py
+lib/idds/tests/test_get_request_info.py
 lib/idds/tests/test_hyperparameteropt.py
 lib/idds/tests/test_logger.py
 lib/idds/tests/test_merge_dict.py
 lib/idds/tests/test_migrate_requests.py
 lib/idds/tests/test_property.py
 lib/idds/tests/test_request_transform.py
 lib/idds/tests/test_requests.py
```

### Comparing `idds-server-1.2.9/setup.py` & `idds-server-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/config_monitor.py` & `idds-server-1.3.0/tools/env/config_monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/create_database.py` & `idds-server-1.3.0/tools/env/create_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/destroy_database.py` & `idds-server-1.3.0/tools/env/destroy_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/dump_database.py` & `idds-server-1.3.0/tools/env/dump_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/environment.yml` & `idds-server-1.3.0/tools/env/environment.yml`

 * *Files 5% similar despite different names*

```diff
@@ -26,10 +26,12 @@
   - psycopg2-binary
   - pyjwt
   - cryptography
   - redis
   - alembic
   - deepdiff
   - pyzmq
-  - idds-common==1.2.9
-  - idds-workflow==1.2.9
-  - idds-client==1.2.9
+  - oic
+  - lsst-ctrl-bps
+  - idds-common==1.3.0
+  - idds-workflow==1.3.0
+  - idds-client==1.3.0
```

### Comparing `idds-server-1.2.9/tools/env/install_env_conda.sh` & `idds-server-1.3.0/tools/env/install_env_conda.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/install_idds_full.sh` & `idds-server-1.3.0/tools/env/install_idds_full.sh`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #  rm -fr *; cp -r /afs/cern.ch/user/w/wguan/workdisk/iDDS/* .;python setup.py install --old-and-unmanageable
 git clone @github_idds@ /opt/idds_source
 conda env create --prefix=/opt/idds -f main/tools/env/environment.yml
 # source /etc/profile.d/conda.sh
 conda activate /opt/idds
 conda install -c conda-forge python-gfal2
 
-pip install rucio-clients-atlas rucio-clients panda-client
+pip install rucio-clients-atlas rucio-clients panda-client-light
 # root ca.crt to  /opt/idds/etc/ca.crt
 
 pip install requests SQLAlchemy urllib3 retrying mod_wsgi flask futures stomp.py cx-Oracle  unittest2 pep8 flake8 pytest nose sphinx recommonmark sphinx-rtd-theme nevergrad
  pip install psycopg2-binary
 
 # add "auth_type = x509_proxy" to /opt/idds/etc/rucio.cfg
```

### Comparing `idds-server-1.2.9/tools/env/merge_configmap.py` & `idds-server-1.3.0/tools/env/merge_configmap.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/merge_idds_configs.py` & `idds-server-1.3.0/tools/env/merge_idds_configs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/setup_dev.sh` & `idds-server-1.3.0/tools/env/setup_dev.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.2.9/tools/env/setup_panda.sh` & `idds-server-1.3.0/tools/env/setup_panda.sh`

 * *Files identical despite different names*

