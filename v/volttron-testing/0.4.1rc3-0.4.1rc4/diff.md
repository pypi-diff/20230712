# Comparing `tmp/volttron_testing-0.4.1rc3.tar.gz` & `tmp/volttron_testing-0.4.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_testing-0.4.1rc3.tar", max compression
+gzip compressed data, was "volttron_testing-0.4.1rc4.tar", max compression
```

## Comparing `volttron_testing-0.4.1rc3.tar` & `volttron_testing-0.4.1rc4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11928 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/LICENSE
--rw-r--r--   0        0        0     3607 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/README.md
--rw-r--r--   0        0        0     1806 2023-05-11 17:23:25.650281 volttron_testing-0.4.1rc3/pyproject.toml
--rw-r--r--   0        0        0     1166 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/src/volttrontesting/__init__.py
--rw-r--r--   0        0        0     5184 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/src/volttrontesting/agent_additions.py
--rw-r--r--   0        0        0     9155 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/src/volttrontesting/certs_utils.py
--rw-r--r--   0        0        0      979 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/src/volttrontesting/client_mock.py
--rw-r--r--   0        0        0        0 2023-05-11 17:22:41.469209 volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/__init__.py
--rw-r--r--   0        0        0     4696 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/cert_fixtures.py
--rw-r--r--   0        0        0     4686 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/docker_wrapper.py
--rw-r--r--   0        0        0     8103 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/rmq_test_setup.py
--rw-r--r--   0        0        0    29475 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/volttron_platform_fixtures.py
--rw-r--r--   0        0        0     3422 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/memory_pubsub.py
--rw-r--r--   0        0        0    62220 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/platformwrapper.py
--rw-r--r--   0        0        0    12618 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/server_mock.py
--rw-r--r--   0        0        0     7115 2023-05-11 17:22:41.473209 volttron_testing-0.4.1rc3/src/volttrontesting/utils.py
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 volttron_testing-0.4.1rc3/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/LICENSE
+-rw-r--r--   0        0        0     3607 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/README.md
+-rw-r--r--   0        0        0     1806 2023-07-12 00:14:38.386248 volttron_testing-0.4.1rc4/pyproject.toml
+-rw-r--r--   0        0        0     1166 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/__init__.py
+-rw-r--r--   0        0        0     5184 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/agent_additions.py
+-rw-r--r--   0        0        0     9155 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/certs_utils.py
+-rw-r--r--   0        0        0      979 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/client_mock.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/__init__.py
+-rw-r--r--   0        0        0     4696 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/cert_fixtures.py
+-rw-r--r--   0        0        0     4686 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/docker_wrapper.py
+-rw-r--r--   0        0        0     8103 2023-07-12 00:13:44.198061 volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/rmq_test_setup.py
+-rw-r--r--   0        0        0    29475 2023-07-12 00:13:44.202061 volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/volttron_platform_fixtures.py
+-rw-r--r--   0        0        0     3422 2023-07-12 00:13:44.202061 volttron_testing-0.4.1rc4/src/volttrontesting/memory_pubsub.py
+-rw-r--r--   0        0        0    62703 2023-07-12 00:13:44.202061 volttron_testing-0.4.1rc4/src/volttrontesting/platformwrapper.py
+-rw-r--r--   0        0        0    12618 2023-07-12 00:13:44.202061 volttron_testing-0.4.1rc4/src/volttrontesting/server_mock.py
+-rw-r--r--   0        0        0     7115 2023-07-12 00:13:44.202061 volttron_testing-0.4.1rc4/src/volttrontesting/utils.py
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 volttron_testing-0.4.1rc4/PKG-INFO
```

### Comparing `volttron_testing-0.4.1rc3/LICENSE` & `volttron_testing-0.4.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/README.md` & `volttron_testing-0.4.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/pyproject.toml` & `volttron_testing-0.4.1rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-testing"
-version = "0.4.1rc3"
+version = "0.4.1rc4"
 description = "The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-testing"
 homepage = "https://github.com/eclipse-volttron/volttron-testing"
 keywords = []
```

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/__init__.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/agent_additions.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/agent_additions.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/certs_utils.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/certs_utils.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/client_mock.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/client_mock.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/cert_fixtures.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/cert_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/docker_wrapper.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/rmq_test_setup.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/rmq_test_setup.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/fixtures/volttron_platform_fixtures.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/fixtures/volttron_platform_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/memory_pubsub.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/memory_pubsub.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/platformwrapper.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/platformwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1064,15 +1064,20 @@
         :return:
         """
         with with_os_environ(self.env):
             self.logit("Waiting for control_connection to exit")
             disconnected = False
             timer_start = time.time()
             while not disconnected:
-                peers = self.dynamic_agent.vip.peerlist().get(timeout=20)
+                try:
+                    peers = self.dynamic_agent.vip.peerlist().get(timeout=10)
+                except gevent.Timeout:
+                    self.logit("peerlist call timed out. Exiting loop. "
+                               "Not waiting for control connection to exit.")
+                    break
                 disconnected = CONTROL_CONNECTION not in peers
                 if disconnected:
                     break
                 if time.time() - timer_start > timeout:
                     # raise PlatformWrapperError(f"Failed for {CONTROL_CONNECTION} to exit in a timely manner.")
                     # See https://githb.com/VOLTTRON/volttron/issues/2938
                     self.logit("Control connection did not exit")
@@ -1347,15 +1352,15 @@
         with with_os_environ(self.env):
             # Handle cascading calls from multiple levels of fixtures.
             if self._instance_shutdown:
                 self.logit(f"Instance already shutdown {self._instance_shutdown}")
                 return
 
             if not self.is_running():
-                self.logit(f"Instance not running {self.is_running()} and skip cleanup: {self.skip_cleanup}")
+                self.logit(f"Instance running {self.is_running()} and skip cleanup: {self.skip_cleanup}")
                 if not self.skip_cleanup:
                     self.__remove_home_directory__()
                 return
 
             running_pids = []
             if self.dynamic_agent:  # because we are not creating dynamic agent in setupmode
                 try:
@@ -1363,14 +1368,18 @@
                         pid = self.agent_pid(agnt['uuid'])
                         if pid is not None and int(pid) > 0:
                             running_pids.append(int(pid))
                     if not self.skip_cleanup:
                         self.remove_all_agents()
                 except gevent.Timeout:
                     self.logit("Timeout getting list of agents")
+                except RuntimeError as e:
+                    if not self.is_running():
+                        self.logit("Unable to shutdown agent. instance is already shutdown")
+                    self.logit(f"Error shutting down agent {e}")
 
                 try:
                     # don't wait indefinitely as shutdown will not throw an error if RMQ is down/has cert errors
                     self.dynamic_agent.vip.rpc(CONTROL, 'shutdown').get(timeout=10)
                     self.dynamic_agent.core.stop(timeout=10)
                 except gevent.Timeout:
                     self.logit("Timeout shutting down platform")
```

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/server_mock.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/server_mock.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/src/volttrontesting/utils.py` & `volttron_testing-0.4.1rc4/src/volttrontesting/utils.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc3/PKG-INFO` & `volttron_testing-0.4.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-testing
-Version: 0.4.1rc3
+Version: 0.4.1rc4
 Summary: The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.
 Home-page: https://github.com/eclipse-volttron/volttron-testing
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

