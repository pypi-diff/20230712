# Comparing `tmp/perun.proxy.utils-1.8.0.tar.gz` & `tmp/perun.proxy.utils-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-1.8.0.tar", last modified: Wed Jul 12 09:12:39 2023, max compression
+gzip compressed data, was "perun.proxy.utils-1.8.1.tar", last modified: Wed Jul 12 11:40:24 2023, max compression
```

## Comparing `perun.proxy.utils-1.8.0.tar` & `perun.proxy.utils-1.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.318135 perun.proxy.utils-1.8.0/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.318135 perun.proxy.utils-1.8.0/perun/proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.370137 perun.proxy.utils-1.8.0/perun/proxy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.402137 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_custom_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_dockers.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_exabgp_propagation.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap_syncrepl.py
--rw-rw-rw-   0 root         (0) root         (0)    72117 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_nginx.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_rpc_status.py
--rwxrwxrwx   0 root         (0) root         (0)    18784 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_saml.py
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_user_logins.py
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/webserver_availability.py
--rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-12 07:46:01.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/run_probes.py
--rw-rw-rw-   0 root         (0) root         (0)     3215 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0 root         (0) root         (0)     2531 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/separate_ssp_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.322136 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.978383 perun.proxy.utils-1.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 11:40:24.978383 perun.proxy.utils-1.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.974383 perun.proxy.utils-1.8.1/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.974383 perun.proxy.utils-1.8.1/perun/proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.974383 perun.proxy.utils-1.8.1/perun/proxy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.978383 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_custom_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_dockers.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_exabgp_propagation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_ldap_syncrepl.py
+-rw-rw-rw-   0 root         (0) root         (0)    72117 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_nginx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_rpc_status.py
+-rwxrwxrwx   0 root         (0) root         (0)    18784 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/webserver_availability.py
+-rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-12 07:46:01.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/run_probes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2531 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.1/perun/proxy/utils/separate_ssp_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:40:24.974383 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 11:40:24.000000 perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-12 11:40:24.978383 perun.proxy.utils-1.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2023-07-12 11:34:42.000000 perun.proxy.utils-1.8.1/setup.py
```

### Comparing `perun.proxy.utils-1.8.0/LICENSE` & `perun.proxy.utils-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/PKG-INFO` & `perun.proxy.utils-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.8.0
+Version: 1.8.1
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.8.0/README.md` & `perun.proxy.utils-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/metadata_expiration.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/metadata_expiration.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_custom_command.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_custom_command.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_dockers.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_dockers.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_exabgp_propagation.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_exabgp_propagation.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_ldap.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_rpc_status.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_rpc_status.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_saml.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_saml.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_user_logins.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/check_user_logins.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/webserver_availability.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/nagios/webserver_availability.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/print_docker_versions.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/run_probes.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/run_probes.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/run_version_script.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/separate_oidc_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-1.8.1/perun/proxy/utils/separate_ssp_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/PKG-INFO` & `perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.8.0
+Version: 1.8.1
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/SOURCES.txt` & `perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/entry_points.txt` & `perun.proxy.utils-1.8.1/perun.proxy.utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.0/setup.py` & `perun.proxy.utils-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "setuptools",
         "pymongo~=4.3",
         "asyncssh~=2.13",
         "docker~=6.0",
         "beautifulsoup4~=4.12",
         "requests~=2.31",
         "ldap3~=2.9.1",
-        "PyYAML~=6.0",
+        "PyYAML>=5.4,<7.0",
         "check_syncrepl_extended~=2020.13",
         "check_nginx_status~=1.0",
     ],
     entry_points={
         "console_scripts": [
             "run_probes=perun.proxy.utils.run_probes:main",
             "check_custom_command=perun.proxy.utils.nagios.check_custom_command:main",
```

