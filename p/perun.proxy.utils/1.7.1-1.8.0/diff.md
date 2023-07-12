# Comparing `tmp/perun.proxy.utils-1.7.1.tar.gz` & `tmp/perun.proxy.utils-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-1.7.1.tar", last modified: Wed Jun 28 08:30:57 2023, max compression
+gzip compressed data, was "perun.proxy.utils-1.8.0.tar", last modified: Wed Jul 12 09:12:39 2023, max compression
```

## Comparing `perun.proxy.utils-1.7.1.tar` & `perun.proxy.utils-1.8.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:57.036198 perun.proxy.utils-1.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3536 2023-06-28 08:30:57.036198 perun.proxy.utils-1.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-20 12:40:41.000000 perun.proxy.utils-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:56.820193 perun.proxy.utils-1.7.1/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:56.820193 perun.proxy.utils-1.7.1/perun/proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:56.884195 perun.proxy.utils-1.7.1/perun/proxy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:57.036198 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-07 12:28:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_custom_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-07 12:27:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_dockers.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-07 12:27:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_exabgp_propagation.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-07 12:28:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_ldap.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-07 12:27:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_ldap_syncrepl.py
--rw-rw-rw-   0 root         (0) root         (0)    72133 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-12 08:06:47.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_nginx.py
--rw-rw-rw-   0 root         (0) root         (0)     1758 2023-06-07 12:28:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_rpc_status.py
--rwxrwxrwx   0 root         (0) root         (0)    18760 2023-06-15 10:37:02.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_saml.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_user_logins.py
--rwxrwxrwx   0 root         (0) root         (0)      930 2023-06-07 12:27:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/webserver_availability.py
--rwxrwxrwx   0 root         (0) root         (0)     2322 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-06-20 12:40:41.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/run_probes.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0 root         (0) root         (0)     2238 2023-06-05 07:53:45.000000 perun.proxy.utils-1.7.1/perun/proxy/utils/separate_ssp_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:30:56.836194 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3536 2023-06-28 08:30:56.000000 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-06-28 08:30:56.000000 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 08:30:56.000000 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-28 08:30:56.000000 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-28 08:30:56.000000 perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-28 08:30:57.036198 perun.proxy.utils-1.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-28 08:24:25.000000 perun.proxy.utils-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.318135 perun.proxy.utils-1.8.0/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.318135 perun.proxy.utils-1.8.0/perun/proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.370137 perun.proxy.utils-1.8.0/perun/proxy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.402137 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_custom_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_dockers.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_exabgp_propagation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap_syncrepl.py
+-rw-rw-rw-   0 root         (0) root         (0)    72117 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_nginx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_rpc_status.py
+-rwxrwxrwx   0 root         (0) root         (0)    18784 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/webserver_availability.py
+-rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-12 07:46:01.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/run_probes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2531 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.0/perun/proxy/utils/separate_ssp_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:12:39.322136 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 09:12:39.000000 perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-12 09:12:39.406137 perun.proxy.utils-1.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.0/setup.py
```

### Comparing `perun.proxy.utils-1.7.1/LICENSE` & `perun.proxy.utils-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.7.1/PKG-INFO` & `perun.proxy.utils-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.7.1
+Version: 1.8.0
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.7.1/README.md` & `perun.proxy.utils-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_custom_command.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_custom_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
+import re
 import subprocess
 import sys
 
-
 """
 general script to run non-python checks by a custom-defined command
 """
 
 
 def get_args():
     """
@@ -23,14 +23,20 @@
     )
 
     return parser.parse_args()
 
 
 def main():
     args = get_args()
-    result = subprocess.run(args.command, shell=True, text=True, capture_output=True)
-    print(result.stdout, end="")
+    result = subprocess.run(
+        args.command,
+        shell=True,
+        text=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    )
+    print(re.sub("[ \t\n]+", " ", result.stdout))
     return result.returncode
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_dockers.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_dockers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
 import argparse
+import sys
 
 import docker
 from docker.errors import NotFound, APIError
 
 
 def get_docker_states(req_containers):
     client = docker.from_env()
@@ -49,8 +50,8 @@
         status_info += container_name + ": " + container_status + "; "
 
     print(str(status) + " docker_containers - [" + status_info + "]")
     return status
 
 
 if __name__ == "__main__":
-    exit(main())
+    sys.exit(main())
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_exabgp_propagation.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_exabgp_propagation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+import sys
 from subprocess import run
 
 
 def main():
     result = run(
         ["/usr/bin/docker", "exec", "exabgp", "exabgpcli", "show", "adj-rib", "out"],
         text=True,
@@ -24,8 +24,8 @@
     if len(out) != 0:
         print("-", end=" ")
         print(out)
     return status
 
 
 if __name__ == "__main__":
-    exit(main())
+    sys.exit(main())
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_ldap.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_ldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import argparse
 import sys
 import time
 
 from ldap3 import Server, Connection, SUBTREE
 
-
 """
 check LDAP is available
 """
 
 
 def get_args():
     """
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         return (string, None)
     string = string.rsplit(":", 1)
     host = string[0]  # 1st index is always host
     port = int(string[1])
     return (host, port)
 
 
-def main(argv):
+def main():
     p = optparse.OptionParser(
         conflict_handler="resolve",
         description="This Nagios plugin checks the health of mongodb.",
     )
 
     p.add_option(
         "-H",
@@ -2214,8 +2214,8 @@
     return delta
 
 
 #
 # main app
 #
 if __name__ == "__main__":
-    sys.exit(main(sys.argv[1:]))
+    sys.exit(main())
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_rpc_status.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_rpc_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import argparse
 import re
 import sys
 import time
 import requests
 
-
 """
 check RPC API is available
 """
 
 
 def get_args():
     """
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_saml.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,41 +384,41 @@
             )
         if auth_time is None and from_cache is False:
             message = "{}|authtime=;{};{};;".format(
                 message, self.args.warn_time, self.args.critical_time
             )
         if self.args.cache_timeout > 0:
             try:
-                file_path = tempfile.gettempdir() + "/" + args.cache_file
+                file_path = tempfile.gettempdir() + "/" + self.args.cache_file
                 f = open(file_path, "w")
                 f.write("{}_{}_{}".format(cache_time, status, message))
                 f.close()
             except (OSError, ValueError):
                 pass
         if from_cache:
             message = "Cached: " + message
         print("{} - {}".format(status, message))
         sys.exit(STATUS[status])
 
     def check_cache(self):
         try:
             tempdir = tempfile.gettempdir()
-            file_path = tempdir + "/" + args.cache_file
+            file_path = tempdir + "/" + self.args.cache_file
             if os.path.isfile(file_path):
                 with open(file_path, "r") as f:
                     res_b = f.read()
                     if not re.match(CACHE_REGEX, res_b):
                         raise ValueError("Bad cache content!")
                     res = res_b.split("_")
                 cached_time = float(res[0])
                 status = res[1]
                 message = res[2]
                 actual_time = time.time()
                 time_diff = actual_time - float(cached_time)
-                if time_diff < args.cache_timeout:
+                if time_diff < self.args.cache_timeout:
                     self.finish(
                         message=message,
                         status=status,
                         cache_time=cached_time,
                         from_cache=True,
                     )
         except (OSError, ValueError):
@@ -547,11 +547,14 @@
         else:
             self.opener = urllib.request.build_opener(
                 urllib.request.HTTPCookieProcessor(self.cookiejar),
                 ResolvingHTTPRedirectHandler(self.hosts, self.args.verbose),
             )
 
 
-if __name__ == "__main__":
-    args = get_args()
-    checker = SAMLChecker(args)
+def main():
+    checker = SAMLChecker(get_args())
     checker.main()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/check_user_logins.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/check_user_logins.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,13 +106,13 @@
 
 
 def main():
     argv = sys.argv[1:]
     path, regex, datetime_format, logins, seconds = command_line_validate(argv)
     user_dict = parse_log_data(path, regex, datetime_format)
     check_log_data(user_dict, logins, seconds)
-    print("OK", logins, seconds)
-    return 0
+    print("OK - ", logins, seconds)
+    sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/nagios/webserver_availability.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/nagios/webserver_availability.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import argparse
+import sys
 
 import requests
 
 
 def get_args():
     """
     Supports the command-line arguments listed below.
@@ -39,8 +40,8 @@
         pass
 
     print(str(status) + " webserver_availability - " + status_txt)
     return status
 
 
 if __name__ == "__main__":
-    exit(main())
+    sys.exit(main())
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/print_docker_versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 #!/usr/bin/env python3
 
 import multiprocessing
 import os
 import re
 import json
+
 import docker
 import argparse
 import platform
 
-output = {
-    "cpu_count": "",
-    "memory": "",
-    "os_version": "",
-    "kernel_version": "",
-    "docker_version": "",
-    "containerd_version": "",
-    "containers": {},
-}
-
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-e", "--exclude", type=str, help="Space delimited list of containers to exclude"
-)
-args = parser.parse_args()
-exc_containers = args.exclude.split(" ") if args.exclude is not None else []
-output["cpu_count"] = str(multiprocessing.cpu_count())
-mem_bytes = os.sysconf("SC_PAGE_SIZE") * os.sysconf("SC_PHYS_PAGES")
-if mem_bytes > 1:
-    output["memory"] = str(round(mem_bytes / (1024.0**3), 2)) + "GiB"
-name = ""
-maj_version = ""
-with open("/etc/os-release") as file:
-    contents = file.read()
-    match = re.search(r"NAME=\"(.*)\"", contents)
-    if match is not None:
-        name = match.group(1)
-    match = re.search(r"VERSION_ID=\"(.*)\"", contents)
-    if match is not None:
-        maj_version = match.group(1).split(".")[0]
-if name.startswith("Debian"):
-    name = name.split(" ")[0]
-output["os_version"] = name + " " + maj_version
-output["kernel_version"] = platform.release()
-client = docker.from_env()
-if client is not None:
-    version_info = client.version()
-    docker_ver_filter = list(
-        filter(lambda x: x["Name"] == "Engine", version_info["Components"])
-    )
-    output["docker_version"] = (
-        docker_ver_filter[0]["Version"] if len(docker_ver_filter) > 0 else ""
-    )
-    containerd_ver_filter = list(
-        filter(lambda x: x["Name"] == "containerd", version_info["Components"])
-    )
-    containerd_version = (
-        containerd_ver_filter[0]["Version"] if len(containerd_ver_filter) > 0 else ""
+
+def main():
+    output = {
+        "cpu_count": "",
+        "memory": "",
+        "os_version": "",
+        "kernel_version": "",
+        "docker_version": "",
+        "containerd_version": "",
+        "containers": {},
+    }
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-e",
+        "--exclude",
+        type=str,
+        help="Space delimited list of containers to exclude",
     )
-    if len(containerd_version) > 0 and containerd_version[0] == "v":
-        containerd_version = containerd_version[1:]
-    output["containerd_version"] = containerd_version
-    containers = client.containers.list()
-    containers = list(filter(lambda x: x.name not in exc_containers, containers))
-    for container in containers:
-        container_image = container.image.tags[0] if container.image.tags else ""
-        output["containers"][container.name] = container_image.split(":")[-1]
-print(json.dumps(output))
+    args = parser.parse_args()
+    exc_containers = args.exclude.split(" ") if args.exclude is not None else []
+    output["cpu_count"] = str(multiprocessing.cpu_count())
+    mem_bytes = os.sysconf("SC_PAGE_SIZE") * os.sysconf("SC_PHYS_PAGES")
+    if mem_bytes > 1:
+        output["memory"] = str(round(mem_bytes / (1024.0**3), 2)) + "GiB"
+    name = ""
+    maj_version = ""
+    with open("/etc/os-release") as file:
+        contents = file.read()
+        match = re.search(r"NAME=\"(.*)\"", contents)
+        if match is not None:
+            name = match.group(1)
+        match = re.search(r"VERSION_ID=\"(.*)\"", contents)
+        if match is not None:
+            maj_version = match.group(1).split(".")[0]
+    if name.startswith("Debian"):
+        name = name.split(" ")[0]
+    output["os_version"] = name + " " + maj_version
+    output["kernel_version"] = platform.release()
+    client = docker.from_env()
+    if client is not None:
+        version_info = client.version()
+        docker_ver_filter = list(
+            filter(lambda x: x["Name"] == "Engine", version_info["Components"])
+        )
+        output["docker_version"] = (
+            docker_ver_filter[0]["Version"] if len(docker_ver_filter) > 0 else ""
+        )
+        containerd_ver_filter = list(
+            filter(lambda x: x["Name"] == "containerd", version_info["Components"])
+        )
+        containerd_version = (
+            containerd_ver_filter[0]["Version"]
+            if len(containerd_ver_filter) > 0
+            else ""
+        )
+        if len(containerd_version) > 0 and containerd_version[0] == "v":
+            containerd_version = containerd_version[1:]
+        output["containerd_version"] = containerd_version
+        containers = client.containers.list()
+        containers = list(filter(lambda x: x.name not in exc_containers, containers))
+        for container in containers:
+            container_image = container.image.tags[0] if container.image.tags else ""
+            output["containers"][container.name] = container_image.split(":")[-1]
+    print(json.dumps(output))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/run_probes.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/run_probes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,46 +12,50 @@
         with open(filepath) as f:
             return f.read()
     except OSError as e:
         print(
             f"Cannot open config with path: {filepath}, error: {e.strerror}",
             file=sys.stderr,
         )
-        exit(2)
+        sys.exit(2)
 
 
 def run_probe(probe_name, command):
-    result = subprocess.run(command, text=True, capture_output=True)
-    search = re.search(r" - .*", result.stdout)
+    result = subprocess.run(
+        command, text=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
+    )
+    output = re.sub("[ \t\n]+", " ", result.stdout)
+    search = re.search(r" - .*", output)
     if search:
         print(f"{result.returncode} {probe_name} {search.group()}")
     else:
-        print(f"{result.returncode} {probe_name} - {result.stdout}")
+        print(f"{result.returncode} {probe_name} - {output}")
     return result.returncode
 
 
-def main(config_filepath):
+def main():
+    config_filepath = "/etc/run_probes_cfg.yaml"
     config = yaml.safe_load(open_file(config_filepath))
     if not config:
         return
 
     for _, options in config.items():
         module = options["module"]
         for name, args in options.get("runs").items():
-            command = ["python", "-m", module]
+            command = ["python3", "-m", module]
             for arg_name, arg_val in args.items():
                 if len(arg_name) == 1:
                     arg_name = "-" + arg_name
                 else:
                     arg_name = "--" + arg_name
                 if arg_val is True:
                     arg_val = "true"
                 elif arg_val is False:
                     arg_val = "false"
                 command.append(arg_name)
-                command.append(str(arg_val))
+                if arg_val is not None:
+                    command.append(str(arg_val))
             Thread(target=run_probe, args=[name, command]).start()
 
 
 if __name__ == "__main__":
-    config_filepath = "/etc/run_probes_cfg.yaml"
-    main(config_filepath)
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/run_version_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,30 +46,30 @@
             + " | ".join(
                 [f"{str(value[i]):<{length}}" for length, value in zip(lengths, values)]
             )
             + " |"
         )
 
 
-async def run_script(user, host):
+async def run_script(user, host, exc_containers):
     try:
         async with asyncssh.connect(host, username=user) as conn:
             await asyncssh.scp("print_docker_versions.py", (conn, "/tmp/"))
             return (
                 await conn.run(
                     'python3 /tmp/print_docker_versions.py -e "' + exc_containers + '"',
                 ),
                 host,
             )
     except Exception as e:
         return e, host
 
 
-async def collect_info(hosts):
-    tasks = (run_script(host[0], host[1]) for host in hosts)
+async def collect_info(hosts, exc_containers):
+    tasks = (run_script(host[0], host[1], exc_containers) for host in hosts)
     results = await asyncio.gather(*tasks, return_exceptions=True)
     stdouts = []
     hosts = []
     for result, host in results:
         if isinstance(result, Exception):
             print("Connecting to host %s failed: %s" % (host, str(result)))
         elif result.exit_status != 0:
@@ -81,17 +81,25 @@
         else:
             stdouts.append(result.stdout)
             hosts.append(host)
     if len(stdouts) > 0 and len(hosts) > 0:
         dict_to_md_table(jsons_to_dictionary(stdouts, hosts))
 
 
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-e", "--exclude", type=str, help="Space delimited list of containers to exclude"
-)
-parser.add_argument("machines", nargs="+", help="Machines to collect the info from")
-
-args = parser.parse_args()
-exc_containers = args.exclude if args.exclude is not None else ""
-machines = list(map(lambda x: x.split("@"), args.machines))
-asyncio.run(collect_info(machines))
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-e",
+        "--exclude",
+        type=str,
+        help="Space delimited list of containers to exclude",
+    )
+    parser.add_argument("machines", nargs="+", help="Machines to collect the info from")
+
+    args = parser.parse_args()
+    exc_containers = args.exclude if args.exclude is not None else ""
+    machines = list(map(lambda x: x.split("@"), args.machines))
+    asyncio.run(collect_info(machines, exc_containers))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/separate_oidc_logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,70 +2,76 @@
 
 import gzip
 import shutil
 import re
 import sys
 from os import mkdir, path, rename, remove, system
 
-if len(sys.argv) <= 1:
-    print("One argument is expected!")
-    exit(-1)
 
-absolute_file_name = sys.argv[1]
+def main():
+    if len(sys.argv) <= 1:
+        print("One argument is expected!")
+        sys.exit(-1)
 
-if not path.exists(absolute_file_name):
-    print("File with name " + absolute_file_name + " doesn't exists!")
-    exit(-1)
+    absolute_file_name = sys.argv[1]
 
-file_name = path.basename(absolute_file_name)
-dir_name = path.dirname(absolute_file_name)
+    if not path.exists(absolute_file_name):
+        print("File with name " + absolute_file_name + " doesn't exists!")
+        sys.exit(-1)
 
-if len(dir_name) != 0:
-    dir_name += "/"
+    file_name = path.basename(absolute_file_name)
+    dir_name = path.dirname(absolute_file_name)
 
-full_log_dir_name = dir_name + "full_logs/"
-full_log_file_name = "full_" + file_name
-full_log_absolute_name = full_log_dir_name + full_log_file_name
+    if len(dir_name) != 0:
+        dir_name += "/"
 
-if not path.exists(full_log_dir_name):
-    mkdir(full_log_dir_name)
+    full_log_dir_name = dir_name + "full_logs/"
+    full_log_file_name = "full_" + file_name
+    full_log_absolute_name = full_log_dir_name + full_log_file_name
 
-rename(absolute_file_name, full_log_absolute_name)
+    if not path.exists(full_log_dir_name):
+        mkdir(full_log_dir_name)
 
-session_ids = set()
-regex_session_id = r"(?<=\s\[)\w+(?=\]\s+\S+\s+:)"
+    rename(absolute_file_name, full_log_absolute_name)
 
-file = open(full_log_absolute_name, "r")
-for line in file:
-    res = re.search("proxyidptester@cesnet.cz|9006464@muni.cz", line)
-    if res is not None:
+    session_ids = set()
+    regex_session_id = r"(?<=\s\[)\w+(?=\]\s+\S+\s+:)"
+
+    file = open(full_log_absolute_name, "r")
+    for line in file:
+        res = re.search("proxyidptester@cesnet.cz|9006464@muni.cz", line)
+        if res is not None:
+            session_id = re.search(regex_session_id, line)
+            if session_id is not None:
+                session_ids.add(session_id.group(0))
+    file.close()
+
+    file = open(full_log_absolute_name, "r")
+
+    final_log_file = open(absolute_file_name, "w")
+    last_session_id = ""
+    for line in file:
         session_id = re.search(regex_session_id, line)
         if session_id is not None:
-            session_ids.add(session_id.group(0))
-file.close()
+            last_session_id = session_id.group(0)
+        if session_id is None or session_id.group(0) not in session_ids:
+            if last_session_id not in session_ids:
+                final_log_file.write(line)
+
+    file.close()
+    final_log_file.close()
+
+    # Zip old log file
+    with open(full_log_absolute_name, "rb") as f_in, gzip.open(
+        full_log_absolute_name + ".gz", "wb"
+    ) as f_out:
+        shutil.copyfileobj(f_in, f_out)
 
-file = open(full_log_absolute_name, "r")
+    # Remove unzip file
+    remove(full_log_absolute_name)
 
-final_log_file = open(absolute_file_name, "w")
-last_session_id = ""
-for line in file:
-    session_id = re.search(regex_session_id, line)
-    if session_id is not None:
-        last_session_id = session_id.group(0)
-    if session_id is None or session_id.group(0) not in session_ids:
-        if last_session_id not in session_ids:
-            final_log_file.write(line)
-
-file.close()
-final_log_file.close()
-
-# Zip old log file
-with open(full_log_absolute_name, "rb") as f_in, gzip.open(
-    full_log_absolute_name + ".gz", "wb"
-) as f_out:
-    shutil.copyfileobj(f_in, f_out)
+    # Remove old files
+    system("find " + full_log_dir_name + " -mtime +7 -delete")
 
-# Remove unzip file
-remove(full_log_absolute_name)
 
-# Remove old files
-system("find " + full_log_dir_name + " -mtime +7 -delete")
+if __name__ == "__main__":
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-1.8.0/perun/proxy/utils/separate_ssp_logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,80 +2,86 @@
 
 import gzip
 import shutil
 import re
 import sys
 from os import mkdir, path, rename, remove, system
 
-if len(sys.argv) <= 1:
-    print("One argument is expected!")
-    exit(-1)
 
-absolute_file_name = sys.argv[1]
-
-if not path.exists(absolute_file_name):
-    print("File with name " + absolute_file_name + " doesn't exists!")
-    exit(-1)
-
-file_name = path.basename(absolute_file_name)
-dir_name = path.dirname(absolute_file_name)
-
-if len(dir_name) != 0:
-    dir_name += "/"
-
-full_log_dir_name = dir_name + "full_logs/"
-full_log_file_name = "full_" + file_name
-full_log_absolute_name = full_log_dir_name + full_log_file_name
-
-if not path.exists(full_log_dir_name):
-    mkdir(full_log_dir_name)
-
-rename(absolute_file_name, full_log_absolute_name)
-
-session_ids = set()
-thread_ids = set()
-regex_session_id = r"^.*]:\s\d\s\[(.*?)\].*$"
-regex_thread_id = r"^.*\[(.*?)\]:.*$"
-
-file = open(full_log_absolute_name, "r")
-for line in file:
-    res = re.search("proxyidptester@cesnet.cz|9006464@muni.cz", line)
-    if res is not None:
+def main():
+    if len(sys.argv) <= 1:
+        print("One argument is expected!")
+        sys.exit(-1)
+
+    absolute_file_name = sys.argv[1]
+
+    if not path.exists(absolute_file_name):
+        print("File with name " + absolute_file_name + " doesn't exists!")
+        sys.exit(-1)
+
+    file_name = path.basename(absolute_file_name)
+    dir_name = path.dirname(absolute_file_name)
+
+    if len(dir_name) != 0:
+        dir_name += "/"
+
+    full_log_dir_name = dir_name + "full_logs/"
+    full_log_file_name = "full_" + file_name
+    full_log_absolute_name = full_log_dir_name + full_log_file_name
+
+    if not path.exists(full_log_dir_name):
+        mkdir(full_log_dir_name)
+
+    rename(absolute_file_name, full_log_absolute_name)
+
+    session_ids = set()
+    thread_ids = set()
+    regex_session_id = r"^.*]:\s\d\s\[(.*?)\].*$"
+    regex_thread_id = r"^.*\[(.*?)\]:.*$"
+
+    file = open(full_log_absolute_name, "r")
+    for line in file:
+        res = re.search("proxyidptester@cesnet.cz|9006464@muni.cz", line)
+        if res is not None:
+            session_id = re.search(regex_session_id, line)
+            if session_id is not None:
+                session_ids.add(session_id.group(1))
+            thread_id = re.search(regex_thread_id, line)
+            if thread_id is not None:
+                thread_ids.add(thread_id.group(1))
+    file.close()
+
+    file = open(full_log_absolute_name, "r")
+
+    final_log_file = open(absolute_file_name, "w")
+    last_session_id = ""
+    for line in file:
         session_id = re.search(regex_session_id, line)
         if session_id is not None:
-            session_ids.add(session_id.group(1))
-        thread_id = re.search(regex_thread_id, line)
-        if thread_id is not None:
-            thread_ids.add(thread_id.group(1))
-file.close()
-
-file = open(full_log_absolute_name, "r")
-
-final_log_file = open(absolute_file_name, "w")
-last_session_id = ""
-for line in file:
-    session_id = re.search(regex_session_id, line)
-    if session_id is not None:
-        last_session_id = session_id.group(1)
-    if session_id is None or session_id.group(1) not in session_ids:
-        thread_id = re.search(regex_thread_id, line)
-        if (
-            thread_id is None
-            or thread_id.group(1) not in thread_ids
-            or last_session_id not in session_ids
-        ):
-            final_log_file.write(line)
-
-file.close()
-final_log_file.close()
-
-# Zip old log file
-with open(full_log_absolute_name, "rb") as f_in, gzip.open(
-    full_log_absolute_name + ".gz", "wb"
-) as f_out:
-    shutil.copyfileobj(f_in, f_out)
+            last_session_id = session_id.group(1)
+        if session_id is None or session_id.group(1) not in session_ids:
+            thread_id = re.search(regex_thread_id, line)
+            if (
+                thread_id is None
+                or thread_id.group(1) not in thread_ids
+                or last_session_id not in session_ids
+            ):
+                final_log_file.write(line)
+
+    file.close()
+    final_log_file.close()
+
+    # Zip old log file
+    with open(full_log_absolute_name, "rb") as f_in, gzip.open(
+        full_log_absolute_name + ".gz", "wb"
+    ) as f_out:
+        shutil.copyfileobj(f_in, f_out)
+
+    # Remove unzip file
+    remove(full_log_absolute_name)
+
+    # Remove old files
+    system("find " + full_log_dir_name + " -mtime +7 -delete")
 
-# Remove unzip file
-remove(full_log_absolute_name)
 
-# Remove old files
-system("find " + full_log_dir_name + " -mtime +7 -delete")
+if __name__ == "__main__":
+    main()
```

### Comparing `perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/PKG-INFO` & `perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.7.1
+Version: 1.8.0
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.7.1/perun.proxy.utils.egg-info/SOURCES.txt` & `perun.proxy.utils-1.8.0/perun.proxy.utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 perun.proxy.utils.egg-info/PKG-INFO
 perun.proxy.utils.egg-info/SOURCES.txt
 perun.proxy.utils.egg-info/dependency_links.txt
+perun.proxy.utils.egg-info/entry_points.txt
 perun.proxy.utils.egg-info/requires.txt
 perun.proxy.utils.egg-info/top_level.txt
 perun/proxy/utils/__init__.py
 perun/proxy/utils/metadata_expiration.py
 perun/proxy/utils/print_docker_versions.py
 perun/proxy/utils/run_probes.py
 perun/proxy/utils/run_version_script.py
```

