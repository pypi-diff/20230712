# Comparing `tmp/gridappsd_field_bus-2023.6.1a2.tar.gz` & `tmp/gridappsd_field_bus-2023.7.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_field_bus-2023.6.1a2.tar", max compression
+gzip compressed data, was "gridappsd_field_bus-2023.7.1a0.tar", max compression
```

## Comparing `gridappsd_field_bus-2023.6.1a2.tar` & `gridappsd_field_bus-2023.7.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/README.md
--rw-r--r--   0        0        0        0 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/__no_init__here
--rw-r--r--   0        0        0      227 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    15260 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     1987 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0     1840 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7538 2023-06-08 19:47:57.084977 gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0      892 2023-06-08 19:49:00.221149 gridappsd_field_bus-2023.6.1a2/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.6.1a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 20:31:44.478587 gridappsd_field_bus-2023.7.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 20:31:44.478587 gridappsd_field_bus-2023.7.1a0/gridappsd/__no_init__here
+-rw-r--r--   0        0        0      227 2023-07-12 20:31:44.478587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-12 20:31:44.482587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    15023 2023-07-12 20:31:44.482587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     2034 2023-07-12 20:31:44.482587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0     1856 2023-07-12 20:31:44.482587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7538 2023-07-12 20:31:44.482587 gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0      892 2023-07-12 20:32:51.349778 gridappsd_field_bus-2023.7.1a0/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 gridappsd_field_bus-2023.7.1a0/PKG-INFO
```

### Comparing `gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/agents/agents.py` & `gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/agents/agents.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,19 @@
         self.params = ConnectionParameters()
         self.connection = GridappsdConnection(self.params)
 
         self.app_id = agent_config['app_id']
         self.description = agent_config['description']
         dt = datetime.now()
         ts = datetime.timestamp(dt)
-        self.agent_id = "da_" + self.app_id + "_" + str(int(ts))
+        if ('context_manager' not in self.app_id):
+            self.agent_id = "da_" + self.app_id + "_" + str(int(ts))
+        else:
+            self.agent_id = downstream_message_bus_def.id+'.context_manager'
+
         self.agent_area_dict = agent_area_dict
 
         if upstream_message_bus_def is not None:
             if upstream_message_bus_def.is_ot_bus:
                 self.upstream_message_bus = GridAPPSDMessageBus(
                     upstream_message_bus_def)
         #            else:
@@ -83,15 +87,15 @@
 
         # self.context = ContextManager.get(self.feeder_id, self.area_id)
 
         #if agent_dict is not None:
         #    self.addressable_equipments = agent_dict['addressable_equipment']
         #    self.unaddressable_equipments = agent_dict['unaddressable_equipment']
 
-    def connect(self):
+    def _connect(self):
 
         if self.upstream_message_bus is not None:
             self.upstream_message_bus.connect()
         if self.downstream_message_bus is not None:
             self.downstream_message_bus.connect()
         if self.downstream_message_bus is None and self.upstream_message_bus is None:
             raise ValueError(
@@ -105,14 +109,21 @@
         self.subscribe_to_measurement()
         self.subscribe_to_messages()
         self.subscribe_to_requests()
 
         if ('context_manager' not in self.app_id):
             LocalContext.register_agent(self.downstream_message_bus,
                                         self.upstream_message_bus, self)
+            
+    def disconnect(self):
+
+        if self.upstream_message_bus is not None:
+            self.upstream_message_bus.disconnect()
+        if self.downstream_message_bus is not None:
+            self.downstream_message_bus.disconnect()
 
     def subscribe_to_measurement(self):
         if self.simulation_id is None:
             self.downstream_message_bus.subscribe(
                 t.field_output_topic(self.downstream_message_bus.id),
                 self.on_measurement)
         else:
@@ -140,26 +151,28 @@
                                           self.app_id),
             self.on_downstream_message)
         self.downstream_message_bus.subscribe(
             t.field_message_bus_app_topic(self.upstream_message_bus.id,
                                           self.app_id),
             self.on_upstream_message)
 
-        _log.debug(
-            f"Subscribing to message on agents topics: \n {t.field_message_bus_agent_topic(self.downstream_message_bus.id, self.agent_id)} \
-                                                            \n {t.field_message_bus_agent_topic(self.upstream_message_bus.id, self.agent_id)}"
-        )
-        self.downstream_message_bus.subscribe(
-            t.field_message_bus_agent_topic(self.downstream_message_bus.id,
-                                            self.agent_id),
-            self.on_downstream_message)
-        self.downstream_message_bus.subscribe(
-            t.field_message_bus_agent_topic(self.upstream_message_bus.id,
-                                            self.agent_id),
-            self.on_upstream_message)
+
+        if ('context_manager' not in self.app_id):
+            _log.debug(
+                f"Subscribing to message on agents topics: \n {t.field_message_bus_agent_topic(self.downstream_message_bus.id, self.agent_id)} \
+                                                                \n {t.field_message_bus_agent_topic(self.upstream_message_bus.id, self.agent_id)}"
+            )
+            self.downstream_message_bus.subscribe(
+                t.field_message_bus_agent_topic(self.downstream_message_bus.id,
+                                                self.agent_id),
+                self.on_downstream_message)
+            self.upstream_message_bus.subscribe(
+                t.field_message_bus_agent_topic(self.upstream_message_bus.id,
+                                                self.agent_id),
+                self.on_upstream_message)
 
     def subscribe_to_requests(self):
 
         _log.debug(
             f"Subscribing to requests on agents queue: \n {t.field_agent_request_queue(self.downstream_message_bus.id, self.agent_id)} \
                                                             \n {t.field_agent_request_queue(self.upstream_message_bus.id, self.agent_id)}"
         )
@@ -227,30 +240,23 @@
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  feeder_dict=None,
                  simulation_id=None):
-        super(FeederAgent,
-              self).__init__(upstream_message_bus_def,
+        super().__init__(upstream_message_bus_def,
                              downstream_message_bus_def, agent_config,
                              feeder_dict, simulation_id)
         self.feeder_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
-        if self.agent_area_dict is not None:
-            feeder = cim.Feeder(mRID=self.downstream_message_bus_def.id)
-            self.feeder_area = DistributedModel(connection=self.connection,
-                                                feeder=feeder,
-                                                topology=self.agent_area_dict)
-    
 
-    def connect(self):
-        super().connect()
-        if self.feeder_area is None:
+        self._connect()
+
+        if self.agent_area_dict is not None:
             feeder = cim.Feeder(mRID=self.downstream_message_bus_def.id)
             self.feeder_area = DistributedModel(connection=self.connection,
                                                 feeder=feeder,
                                                 topology=self.agent_area_dict)
 
 
 class SwitchAreaAgent(DistributedAgent):
@@ -261,23 +267,18 @@
                  agent_config: Dict,
                  switch_area_dict=None,
                  simulation_id=None):
         super().__init__(upstream_message_bus_def, downstream_message_bus_def,
                          agent_config, switch_area_dict, simulation_id)
         self.switch_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
-        if self.agent_area_dict is not None:
-            self.switch_area = SwitchArea(self.downstream_message_bus_def.id,
-                                          self.connection)
-            self.switch_area.initialize_switch_area(self.agent_area_dict)
-    
 
-    def connect(self):
-        super().connect()
-        if self.switch_area is None:
+        self._connect()
+
+        if self.agent_area_dict is not None:
             self.switch_area = SwitchArea(self.downstream_message_bus_def.id,
                                           self.connection)
             self.switch_area.initialize_switch_area(self.agent_area_dict)
 
 
 class SecondaryAreaAgent(DistributedAgent):
 
@@ -287,26 +288,25 @@
                  agent_config: Dict,
                  secondary_area_dict=None,
                  simulation_id=None):
         super().__init__(upstream_message_bus_def, downstream_message_bus_def,
                          agent_config, secondary_area_dict, simulation_id)
         self.secondary_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
-        if self.agent_area_dict is not None:
-            self.secondary_area = SecondaryArea(self.downstream_message_bus_def.id,
-                                                self.connection)
-            self.secondary_area.initialize_secondary_area(self.agent_area_dict)
-    
 
-    def connect(self):
-        super().connect()
-        if self.secondary_area is None:
+        self._connect()
+
+        if self.agent_area_dict is not None:
+            if len(self.agent_area_dict['addressable_equipment']) == 0:
+                _log.warn(f"No addressable equipment in the secondary area with down stream message bus id: {self.downstream_message_bus.id}.")
+            
             self.secondary_area = SecondaryArea(self.downstream_message_bus_def.id,
                                                 self.connection)
             self.secondary_area.initialize_secondary_area(self.agent_area_dict)
+            
 
 
 class CoordinatingAgent:
     """
     A CoordinatingAgent performs following functions:
         1. Spawns distributed agents
         2. Publishes compiled output to centralized OT bus
@@ -333,20 +333,19 @@
         # print(self.context)
         # self.addressable_equipments = self.context['data']['addressable_equipment']
         # self.unaddressable_equipments = self.context['data']['unaddressable_equipment']
         # self.switch_areas = self.context['data']['switch_areas']
 
         # self.subscribe_to_feeder_bus()
 
-    def spawn_distributed_agent(self, distributed_agent: DistributedAgent):
+
+''' def spawn_distributed_agent(self, distributed_agent: DistributedAgent):
         distributed_agent.connect()
         self.distributed_agents.append(distributed_agent)
 
-
-'''    
     def on_control(self, control):
         device_id = control.get('device')
         command = control.get('command')
         self.control_device(device_id, command)
 
     def publish_to_distribution_bus(self,message):
         self.publish_to_downstream_bus(message)
```

### Comparing `gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/context.py` & `gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from gridappsd.field_interface.interfaces import FieldMessageBus
+from gridappsd_field_interface.interfaces import FieldMessageBus
 import dataclasses
 import gridappsd.topics as t
 import json
 
 
 
 class LocalContext:
     
     @classmethod
     def get_context_by_feeder(cls, downstream_message_bus: FieldMessageBus, feeder_mrid, area_id=None):
         
         request = {'request_type' : 'get_context',
                     'modelId': feeder_mrid,
                    'areaId': area_id}
+        print(t.context_request_queue(downstream_message_bus.id))
         response = downstream_message_bus.get_response(t.context_request_queue(downstream_message_bus.id), request, timeout=10)
         return response
 
     @classmethod
     def get_context_by_message_bus(cls, downstream_message_bus: FieldMessageBus):
         """
         return agents/devices based on downstream message bus as input
 
         """
         request = {'request_type' : 'get_context',
-                   'downstream_message_bus_id': downstream_message_bus.id
+                   'areaId': downstream_message_bus.id
                    }
         return downstream_message_bus.get_response(t.context_request_queue(downstream_message_bus.id), request)
     
     @classmethod
     def register_agent(cls, downstream_message_bus: FieldMessageBus, upstream_message_bus: FieldMessageBus, agent):
         """
         Sends the newly created distributed agent's info to OT bus
```

### Comparing `gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/gridappsd_field_bus.py` & `gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/gridappsd_field_bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,10 +49,10 @@
         Sends a message on a specific concrete queue, waits and returns the response
         """
         if self.gridappsd_obj is not None:
             return self.gridappsd_obj.get_response(topic, message, timeout)
         
     def disconnect(self):
         """
-        Disconnect the device from the concrete message bus.
+        Disconnect from the concrete message bus.
         """
-        pass
+        self.gridappsd_obj.disconnect()
```

### Comparing `gridappsd_field_bus-2023.6.1a2/gridappsd/field_interface/interfaces.py` & `gridappsd_field_bus-2023.7.1a0/gridappsd/field_interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2023.6.1a2/pyproject.toml` & `gridappsd_field_bus-2023.7.1a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-field-bus"
-version = "2023.6.1a2"
+version = "2023.7.1a0"
 description = "GridAPPS-D Field Bus Implementation"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -20,15 +20,15 @@
 packages = [
     { include = 'gridappsd'}
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7.9,<4.0"
-gridappsd-python = "^2023.6.1a2"
+gridappsd-python = "^2023.7.1a0"
 cim-graph = "^2023.5.1a3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
```

### Comparing `gridappsd_field_bus-2023.6.1a2/PKG-INFO` & `gridappsd_field_bus-2023.7.1a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gridappsd-field-bus
-Version: 2023.6.1a2
+Version: 2023.7.1a0
 Summary: GridAPPS-D Field Bus Implementation
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cim-graph (>=2023.5.1a3,<2024.0.0)
-Requires-Dist: gridappsd-python (>=2023.6.1a2,<2024.0.0)
+Requires-Dist: gridappsd-python (>=2023.7.1a0,<2024.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
```

