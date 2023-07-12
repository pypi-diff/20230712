# Comparing `tmp/fogLedger-3.0.0b0.tar.gz` & `tmp/fogLedger-3.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fogLedger-3.0.0b0.tar", last modified: Sat Jul  8 02:07:38 2023, max compression
+gzip compressed data, was "fogLedger-3.0.1b0.tar", last modified: Wed Jul 12 03:10:07 2023, max compression
```

## Comparing `fogLedger-3.0.0b0.tar` & `fogLedger-3.0.1b0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogLedger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/indy/
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/indy/IndyBasic.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/indy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/iota/
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/iota/IotaBasic.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/iota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/test-iota-distributed-network.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/test-iota-local-network.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.703019 fogLedger-3.0.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-12 03:10:07.703019 fogLedger-3.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.699019 fogLedger-3.0.1b0/fogLedger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 03:10:07.000000 fogLedger-3.0.1b0/fogLedger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.699019 fogLedger-3.0.1b0/fogledger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.699019 fogLedger-3.0.1b0/fogledger/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/data/config-coo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/data/config-node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/data/config-spammer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3544 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/data/private-tangle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/data/utils.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.699019 fogLedger-3.0.1b0/fogledger/indy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/indy/IndyBasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/indy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:10:07.703019 fogLedger-3.0.1b0/fogledger/iota/
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/iota/IotaBasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/iota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/test-iota-distributed-network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/fogledger/test-iota-local-network.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:10:07.703019 fogLedger-3.0.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-12 03:09:56.000000 fogLedger-3.0.1b0/setup.py
```

### Comparing `fogLedger-3.0.0b0/LICENSE.txt` & `fogLedger-3.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fogLedger-3.0.0b0/PKG-INFO` & `fogLedger-3.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 3.0.0b0
+Version: 3.0.1b0
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-3.0.0b0/README.md` & `fogLedger-3.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `fogLedger-3.0.0b0/fogLedger.egg-info/PKG-INFO` & `fogLedger-3.0.1b0/fogLedger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 3.0.0b0
+Version: 3.0.1b0
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-3.0.0b0/fogledger/indy/IndyBasic.py` & `fogLedger-3.0.1b0/fogledger/indy/IndyBasic.py`

 * *Files identical despite different names*

### Comparing `fogLedger-3.0.0b0/fogledger/iota/IotaBasic.py` & `fogLedger-3.0.1b0/fogledger/iota/IotaBasic.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 )
 from typing import List
 from typing import Dict
 import os
 import json
 import time
 import subprocess
+import pkg_resources
+
 
 class IotaBasic:
     def __init__(
         self,
         exp: FogbedExperiment,
         prefix: str = 'cloud',
         nodes: List[Dict[str, str]] = []
@@ -41,15 +43,15 @@
         with open(file_path, 'r') as file:
             return file.read()
 
     def startScript(self, nodes: List[Dict[str, str]]):
         print("starting script...")
         node_names = [node['name'] for node in nodes]
         concatenated_string = ":".join(node_names)
-        path_script = os.path.abspath('images/iota/scripts/')
+        path_script = pkg_resources.resource_filename('fogledger', 'data')
         path_private_tangle = os.path.join(path_script, "private-tangle.sh")
         subprocess.run(["chmod", "+x", path_private_tangle])
         subprocess.run(["/bin/bash", path_private_tangle, "install",
                        concatenated_string], check=True, cwd=path_script)
         print("finished script...")
 
     def createContainers(self, nodes: List[str]):
@@ -60,34 +62,34 @@
             
             ip = nodeLabel['ip'] if ("ip" in nodeLabel) else None
             
             port_bindings = nodeLabel['port_bindings'] if ("port_bindings" in nodeLabel) else {}
             
             node = Container(
                 name=name,
-                dimage='larsid/iota-node:v3.0.0-beta',
+                dimage='larsid/fogbed-iota-node:v3.0.0-beta',
                 ip=ip,
                 port_bindings=port_bindings,
                 ports=['14265', '8081', '1883', '15600', '14626/udp']
             )
             self.add_ledger(f'ledger-{node.name}', [node])
 
         ### COO ###
         coo = Container(
             name='coo',
-            dimage='larsid/iota-node:v3.0.0-beta',
+            dimage='larsid/fogbed-iota-node:v3.0.0-beta',
             environment={'COO_PRV_KEYS': ''},
             ports=['15600']
         )
         self.add_ledger(f'ledger-{coo.name}', [coo])
 
         ### spammer ###
         spammer = Container(
             name="spammer",
-            dimage='larsid/iota-node:v3.0.0-beta',
+            dimage='larsid/fogbed-iota-node:v3.0.0-beta',
             ports=['15600', '14626/udp']
         )
         self.add_ledger(f'ledger-{spammer.name}', [spammer])
 
     def searchNode(self, node_name: str):
         for node in self.nodes.values():
             if node.name == node_name:
@@ -124,35 +126,38 @@
             coo.cmd('mkdir -p /app/coo-state')
             coo.cmd(f'./hornet tool ed25519-key > {coo_key_pair_file}')
             COO_PRV_KEYS = coo.cmd(
                 f'cat {coo_key_pair_file} | awk -F : \'{{if ($1 ~ /private key/) print $2}}\' | sed "s/ \+//g" | tr -d "\n" | tr -d "\r"').strip("> >")
             coo.cmd(f'export COO_PRV_KEYS={COO_PRV_KEYS}')
             coo_public_key = coo.cmd(
                 f'cat {coo_key_pair_file} | awk -F : \'{{if ($1 ~ /public key/) print $2}}\' | sed "s/ \+//g" | tr -d "\n" | tr -d "\r"').strip("> >")
-            os.system(
-                f'echo {coo_public_key} > {os.path.abspath("iota/coo-milestones-public-key.txt")}'.format(coo_public_key))
+            
+            file_path = os.path.join("/tmp", "iota")
+            command = f'echo {coo_public_key} > {file_path}/coo-milestones-public-key.txt'
+            os.system(command)
             for node in self.nodes.values():
-                json_data = IotaBasic.read_file(os.path.abspath(f"iota/config/config-{node.name}.json"))
+                json_data = IotaBasic.read_file(f"{file_path}/config/config-{node.name}.json")
                 json_data = json.loads(json_data)
                 json_data["protocol"]["publicKeyRanges"][0]["key"] = coo_public_key
                 updated_data = json.dumps(json_data)
                 node.cmd(f"echo \'{updated_data}\' | jq . > /app/config.json")
             print("Coordinator set up! ✅")
         else:
             print("Coordinator not found! ❌")
 
     def copySnapshotToNodes(self):
         print("\nCopying snapshot to each node")
         # Executar o comando base64 no arquivo full_snapshot.bin e capturar a saída
-        command = f"base64 {os.path.abspath('iota/snapshots/private-tangle/full_snapshot.bin')}"
+        file_path = os.path.join("/tmp", "iota", "snapshots", "private-tangle","full_snapshot.bin")
+        command = f"base64 {file_path}"
         output = subprocess.run(command, capture_output=True, text=True, shell=True).stdout
-
+        print(output)
         # Salvar a saída em uma variável
         output_b64 = output.strip()
-
+        print("veio")
         for node in self.nodes.values():
             node.cmd("mkdir -p /app/snapshots/private-tangle")
             node.cmd(f"echo '{output_b64}' | base64 -d > /app/snapshots/private-tangle/full_snapshot.bin")
 
         print("Snapshot copied! ✅")
 
     # Bootstraps the coordinator
```

### Comparing `fogLedger-3.0.0b0/fogledger/test-iota-distributed-network.py` & `fogLedger-3.0.1b0/fogledger/test-iota-distributed-network.py`

 * *Files identical despite different names*

### Comparing `fogLedger-3.0.0b0/fogledger/test-iota-local-network.py` & `fogLedger-3.0.1b0/fogledger/test-iota-local-network.py`

 * *Files identical despite different names*

### Comparing `fogLedger-3.0.0b0/setup.py` & `fogLedger-3.0.1b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="fogLedger",
-    version="3.0.0-beta",
+    version="3.0.1-beta",
     description='Plugin to build DLTs in Fogbed.',
     long_description='Plugin to build DLT in Fogbed. Suport Hyperledger Indy. \
         The FogLedger is a plugin for [Fogbed](https://github.com/larsid/fogbed). It allows you to emulate a fog network with distributed ledgers. \
         Currently, FogLedger has suport for Hyperledger Indy. It is a distributed ledger, purpose-built for decentralized identity. \
         It provides tools, libraries, and reusable components for creating and using independent digital identities rooted on blockchains or other distributed ledgers so that they are interoperable across administrative domains, applications, and any other silo. \
         Indy is interoperable with other blockchains or can be used standalone powering the decentralization of identity. \
         With FogLedger you can create a network of nodes running Hyperledger Indy. A emulation can have multiple networks of nodes running different distributed ledgers. \
@@ -25,9 +25,10 @@
 
     ],
     install_requires = [
         'numpy>=1.24.2',
     ],
     packages=find_packages(),
     include_package_data=True,
-    zip_safe=False
+    zip_safe=False,
+    package_data={'fogledger': ['data/*.sh', 'data/*.json']}
 )
```

