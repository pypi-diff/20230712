# Comparing `tmp/clivo-0.3.0.tar.gz` & `tmp/clivo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\clivo-0.3.0.tar", last modified: Sat Mar 26 10:00:49 2022, max compression
+gzip compressed data, was "clivo-0.4.0.tar", last modified: Wed Jul 12 19:56:37 2023, max compression
```

## Comparing `clivo-0.3.0.tar` & `clivo-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-03-26 10:00:49.579451 clivo-0.3.0/
--rw-rw-rw-   0        0        0       75 2022-02-02 13:52:58.000000 clivo-0.3.0/.gitignore
--rw-rw-rw-   0        0        0     6211 2022-02-15 16:13:29.000000 clivo-0.3.0/Example.ipynb
--rw-rw-rw-   0        0        0     1544 2022-02-15 15:22:20.000000 clivo-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       32 2022-02-15 16:24:42.000000 clivo-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1976 2022-03-26 10:00:49.581439 clivo-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      808 2022-02-15 16:16:54.000000 clivo-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-03-26 10:00:49.547723 clivo-0.3.0/clivo/
--rw-rw-rw-   0        0        0      179 2022-02-15 16:13:01.000000 clivo-0.3.0/clivo/__init__.py
--rw-rw-rw-   0        0        0    13302 2022-03-24 20:15:24.000000 clivo-0.3.0/clivo/cli.py
-drwxrwxrwx   0        0        0        0 2022-03-26 10:00:49.575937 clivo-0.3.0/clivo.egg-info/
--rw-rw-rw-   0        0        0     1976 2022-03-26 10:00:48.000000 clivo-0.3.0/clivo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2022-03-26 10:00:48.000000 clivo-0.3.0/clivo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-26 10:00:48.000000 clivo-0.3.0/clivo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-03-26 10:00:48.000000 clivo-0.3.0/clivo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2022-03-26 10:00:49.587961 clivo-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       93 2020-12-30 22:12:42.000000 clivo-0.3.0/setup.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-07-12 19:56:37.147047 clivo-0.4.0/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       69 2023-07-07 09:11:38.000000 clivo-0.4.0/.gitignore
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     6050 2023-07-12 14:20:35.000000 clivo-0.4.0/Example.ipynb
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1515 2023-07-07 09:11:38.000000 clivo-0.4.0/LICENSE
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       31 2023-07-07 09:11:38.000000 clivo-0.4.0/MANIFEST.in
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1459 2023-07-12 19:56:37.147117 clivo-0.4.0/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      745 2023-07-12 08:46:10.000000 clivo-0.4.0/README.md
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-07-12 19:56:37.146363 clivo-0.4.0/clivo/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      208 2023-07-12 08:47:25.000000 clivo-0.4.0/clivo/__init__.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    14025 2023-07-12 14:19:08.000000 clivo-0.4.0/clivo/cli.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-07-12 19:56:37.146950 clivo-0.4.0/clivo.egg-info/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1459 2023-07-12 19:56:36.000000 clivo-0.4.0/clivo.egg-info/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      220 2023-07-12 19:56:37.000000 clivo-0.4.0/clivo.egg-info/SOURCES.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        1 2023-07-12 19:56:36.000000 clivo-0.4.0/clivo.egg-info/dependency_links.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        6 2023-07-12 19:56:36.000000 clivo-0.4.0/clivo.egg-info/top_level.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      782 2023-07-12 19:56:37.147406 clivo-0.4.0/setup.cfg
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       89 2023-07-07 09:11:38.000000 clivo-0.4.0/setup.py
```

### Comparing `clivo-0.3.0/Example.ipynb` & `clivo-0.4.0/Example.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9552330746840478%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'from clivo import CommandLineInterface, "*

 * *            "ControlledProperty, ControlledEvent')], delete: [2]}}, 2: {'source': {insert: [(0, "*

 * *            '"interval = ControlledProperty(attribute=\'timer.interval\',\\n"), (1, '*

 * *            '"                              readable=\'Δt (s)\',\\n"), (2, '*

 * *            '"                              commands=(\'dt\',))\\n"), (4, "averaging = '*

 * *            'ControlledProperty(attribute=\'averaging\',\\n"), (5, "          […]*

```diff
@@ -4,259 +4,214 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import oclock\n",
                 "from threading import Event\n",
-                "from clivo import CommandLineInterface"
+                "from clivo import CommandLineInterface, ControlledProperty, ControlledEvent"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Info on what object properties will be controlled"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
+                "interval = ControlledProperty(attribute='timer.interval',\n",
+                "                              readable='\u0394t (s)',\n",
+                "                              commands=('dt',))\n",
+                "\n",
+                "averaging = ControlledProperty(attribute='averaging',\n",
+                "                               readable='Averaging',\n",
+                "                               commands=('avg',))\n",
+                "            \n",
+                "value = ControlledProperty(attribute='value',\n",
+                "                           readable='Value',\n",
+                "                           commands=('val',))"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Generate objects to be controlled"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "class TestObjectA:\n",
                 "\n",
                 "    def __init__(self):\n",
                 "        self.timer = oclock.Timer(interval=1, warnings=True)\n",
-                "        self._avg = 10\n",
-                "        \n",
-                "        self.controlled_properties = 'timer.interval', 'averaging'\n",
+                "        self._avg = 10  \n",
+                "        self.controlled_properties = interval, averaging\n",
                 "        \n",
                 "    @property\n",
                 "    def averaging(self):\n",
                 "        return self._avg\n",
                 "\n",
                 "    @averaging.setter\n",
-                "    def averaging(self, value):\n",
-                "        self._avg = value\n",
+                "    def averaging(self, val):\n",
+                "        self._avg = val\n",
                 "        self.timer.reset()  # for immediate effect\n",
                 "\n",
                 "    def on_stop(self):\n",
                 "        self.timer.stop()\n",
                 "        \n",
                 "class TestObjectB:\n",
                 "\n",
-                "    def __init__(self):\n",
-                "        \n",
+                "    def __init__(self):     \n",
                 "        self.averaging = 10\n",
-                "        self.value = 1\n",
-                "        \n",
-                "        self.controlled_properties = 'value', 'averaging'"
+                "        self.value = 1    \n",
+                "        self.controlled_properties = value, averaging"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "obj1 = TestObjectA()\n",
                 "obj2 = TestObjectA()\n",
                 "obj3 = TestObjectB()\n",
                 "\n",
                 "objects = {'A1': obj1, 'A2': obj2, 'objB': obj3}"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "properties = {'timer.interval': {'repr': '\u0394t (s)',  \n",
-                "                                 'commands': ('dt',),     \n",
-                "                                  },  \n",
-                "              'averaging': {'repr': 'Averaging',\n",
-                "                            'commands': ('avg',),\n",
-                "                            },\n",
-                "              'value': {'repr': 'Value',\n",
-                "                        'commands': ('val',),\n",
-                "                     }\n",
-                "              }"
+                "# Indicate what events can be triggered from CLI"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "graph_event = Event()\n",
-                "stop_event = Event()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "events = {'graph': {'event': graph_event,\n",
-                "                    'commands': ('g', 'graph')\n",
-                "                    },\n",
-                "          'stop': {'event': stop_event,\n",
-                "                   'commands': ('q', 'quit')\n",
-                "                   }\n",
-                "          }"
+                "graph_event = ControlledEvent(event=Event(),\n",
+                "                              readable='graph',\n",
+                "                              commands=('g', 'graph'))\n",
+                "                    \n",
+                "events = graph_event,"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "It is possible to not specify the stop event, in this case it is created internally:"
+                "(Note: a stop event is generated internally but can also be passed)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 7,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "events = {'graph': {'event': graph_event,\n",
-                "                    'commands': ('g', 'graph')\n",
-                "                    \n",
-                "                   }\n",
-                "          }"
+                "# Create and start command line interface"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Stop event not passed. Creating one internally.\n"
                     ]
                 }
             ],
             "source": [
-                "cli = CommandLineInterface(objects, properties, events)"
+                "cli = CommandLineInterface(objects=objects, events=events)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Type command (to stop, type q or Q or quit):  dt\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
+                        "OBJECTS ========================================================================\n",
+                        "--- A1 [<__main__.TestObjectA object at 0x108653400>]\n",
+                        "        \u0394t (s)\n",
+                        "        Averaging\n",
+                        "--- A2 [<__main__.TestObjectA object at 0x108653b80>]\n",
+                        "        \u0394t (s)\n",
+                        "        Averaging\n",
+                        "--- objB [<__main__.TestObjectB object at 0x108653d00>]\n",
+                        "        Value\n",
+                        "        Averaging\n",
+                        "COMMANDS =======================================================================\n",
+                        "--- Properties\n",
+                        "        avg -- Averaging [averaging]\n",
+                        "        val -- Value [value]\n",
+                        "        dt -- \u0394t (s) [timer.interval]\n",
+                        "--- Events\n",
+                        "        g, graph -- graph\n",
+                        "--- Exit\n",
+                        "        q, Q, quit\n",
+                        "EXAMPLE ========================================================================\n",
+                        "avg-A2 xx -- change Averaging to xx for A2 only\n",
+                        "avg xx -- change Averaging to xx for all relevant objects\n",
+                        "================================================================================\n",
                         "\u0394t (s)\n",
                         "A1-----1\n",
                         "A2-----1\n",
-                        "objB---N/A\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Type command (to stop, type q or Q or quit):  dt 10\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "New \u0394t (s) for A1: 10\n",
-                        "New \u0394t (s) for A2: 10\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Type command (to stop, type q or Q or quit):  avg\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Averaging\n",
-                        "A1-----10\n",
-                        "A2-----10\n",
-                        "objB---10\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Type command (to stop, type q or Q or quit):  val 3\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "New Value for objB: 3\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Type command (to stop, type q or Q or quit):  dt-A1 10\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "New \u0394t (s) for A1: 10\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Type command (to stop, type q or Q or quit):  q\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
+                        "objB---N/A\n",
+                        "New \u0394t (s) for A1: 3\n",
+                        "Unknown Command. \n",
+                        "\u0394t (s)\n",
+                        "A1-----3\n",
+                        "A2-----1\n",
+                        "objB---N/A\n",
                         "CLI stopped\n"
                     ]
                 }
             ],
             "source": [
                 "cli.run()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "10"
+                            "3"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj1.timer.interval"
             ]
@@ -281,13 +236,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.5"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `clivo-0.3.0/LICENSE` & `clivo-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, Olivier VINCENT
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, Olivier VINCENT
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `clivo-0.3.0/clivo/cli.py` & `clivo-0.4.0/clivo/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,324 +1,367 @@
-"""Interactive command line interface (CLI)."""
-
-
-from threading import Event
-import random
-import os
-
-
-# TODO -- use match statement with python >= 3.10 instead of if/else?
-
-
-# ================================ MAIN CLASS ================================
-
-
-class CommandLineInterface:
-    """Interactive CLI to manage properties of objects and trigger events
-
-    All objects controlled are referred to with a name.
-    Below, we call an arbitrary name X, e.g. X=P for a pressure reading object).
-
-    The CLI can control an arbitrary number of properties for every object
-    (for example time interval, averaging number, etc.). These properties
-    have commands associated with them.
-    Below, we call can arbitrary property command y, e.g. y=dt for time interval.
-
-    It is also possible to trigger events (e.g. request a graph) with some
-    pre-defined commands passed as a dict to the CLI class.
-    Below, we call these commands for event z
-
-    Once the CLI is started (self.run()), the user input options are:
-    - y: inquire current settings (e.g. dt)
-    - y val: change property value of all objects to a value val (e.g. dt 10)
-    - dt-X val: change settings of only object X to value val (e.g. dt-P 5)
-    - z: trigger event (stop event is by default 'Q', 'q' or 'quit', can be changed)
-    """
-
-    def __init__(self, objects, properties, events):
-        """Create interactive command line interface.
-
-        Parameters
-        ----------
-        - objects: dict of {name: object} of objects to control
-                   (name is a str used in the CLI to refer to the object)
-                   objects can define a on_stop() method which indicates
-                   specific things to do when the stop event is set.
-                   objects must define a `controlled_properties` attribute
-                   that lists which ones of its settable properties is
-                   controlled by the CLI. `controlled_properties` is an iterable
-                   of str that must belong to the keys of the `properties`
-                   dict (see below).
-
-        - properties: dict of dict describing the properties of the objects
-                      that the CLI controls.
-                      - The keys are the names of the properties
-                        (can be sub-properties, e.g. a property of an attribute)
-                      - The values are dicts which must contain the entries
-                          - 'repr' (human-readable description for printing)
-                          - 'commands': iterable of command names (str) that
-                                        will trigger modification of the
-                                        property when typed in the CLI
-
-                      Example:
-                      {'timer.interval': {'repr': 'Δt (s)',
-                                          'commands': ('dt',),
-                                          },
-                       'averaging': {'repr': 'Averaging',
-                                     'commands': ('avg',),
-                                     }
-                       }
-
-        - events: dict of dict describing the events that the CLI controls.
-                  The keys are a description (human-readable) of the event,
-                  and the values are dicts which must contain the entries:
-                  - 'event': Event object to control (typically, from threading)
-                  - 'commands': iterable of command names (str) that
-                                will trigger modification of the
-                                property when typed in the CLI
-
-                  Example:
-                  {'graph': {'event': graph_event,
-                             'commands': ('g', 'graph')
-                             },
-                   'stop': {'event': stop_event,
-                            'commands': ('q', 'quit')
-                            }
-                   }
-
-                   Note: the 'stop' event, if provided, gets linked to the
-                   event that triggers exiting of the CLI. If not provided,
-                   the 'stop' event is defined internally
-        """
-        self.objects = objects
-        self.properties = properties
-        self.events = events
-
-        try:
-            self.stop_dict = self.events.pop('stop')
-        except KeyError:
-            print('Stop event not passed. Creating one internally.')
-            self.stop_event = Event()
-            self.stop_commands = 'q', 'Q', 'quit'
-        else:
-            self.stop_event = self.stop_dict['event']
-            self.stop_commands = self.stop_dict['commands']
-
-        # Note: stop_commands is a tuple, event/property_commmands are dicts.
-        self.event_commands = self._get_commands(self.events)
-        self.property_commands = self._get_commands(self.properties)
-
-        # Dict {ppty: [object names that have this ppty controlled]}
-        self.object_properties = self._get_controlled_properties(objects)
-
-        # For CLI printing
-        self.max_name_length = max([len(obj) for obj in self.objects])
-
-    def _get_controlled_properties(self, objects):
-        """Generate dict {ppty: [object names that have this ppty controlled]}."""
-        object_properties = {}
-        for ppty in self.properties:
-            object_properties[ppty] = []
-            for object_name, obj in objects.items():
-                if ppty in obj.controlled_properties:
-                    object_properties[ppty].append(object_name)
-        return object_properties
-
-    @staticmethod
-    def _get_commands(input_data):
-        """Create dict of which command input modifies which property/event.
-
-        Parameters
-        ----------
-        input_data: dict of dict (can be properties dict or event dict)
-
-        Example
-        -------
-        input_data = {'graph': {'event': e_graph,
-                                'commands': ('g', 'graph')},
-                      'stop': {'event': e_stop,
-                               'commands': ('q', 'Q', 'quit')}
-                      }
-        will return {'g': 'graph',
-                     'graph': 'graph',
-                     'q': 'stop',
-                     'Q': 'stop',
-                     'quit': 'stop'}
-        """
-        commands = {}
-        for name, data_dict in input_data.items():
-            for command_name in data_dict['commands']:
-                commands[command_name] = name
-        return commands
-
-    def _set_property_base(self, ppty_cmd, object_name, value, objects):
-        """Base method for _set_property().
-
-        For use in other modules that potentially define other objects.
-        """
-        obj = objects[object_name]
-        ppty = self.property_commands[ppty_cmd]
-
-        if object_name not in self.object_properties[ppty]:
-            return
-
-        ppty_repr = self.properties[ppty]['repr']
-        try:
-            exec(f'obj.{ppty} = {value}')  # avoids having to pass a convert function
-        except Exception:
-            print(f"'{value}' not a valid {ppty_repr} ({ppty})")
-        else:
-            print(f'New {ppty_repr} for {object_name}: {value}')
-
-    def _set_property(self, ppty_cmd, object_name, value):
-        """Manage command from CLI to set a property accordingly."""
-        return self._set_property_base(ppty_cmd, object_name, value, self.objects)
-
-    def _get_property(self, ppty_cmd, object_name):
-        """Get property according to given property command from CLI."""
-        obj = self.objects[object_name]
-        ppty = self.property_commands[ppty_cmd]
-
-        if object_name not in self.object_properties[ppty]:
-            return
-
-        # exec() strategy avoids having to pass a convert function
-        self._value = None  # exec won't work with local references
-        exec(f'self._value = obj.{ppty}')
-        return self._value
-
-    def _print_properties(self, ppty_cmd):
-        """Print current values of properties of all objects"""
-        ppty = self.property_commands[ppty_cmd]
-        ppty_repr = self.properties[ppty]['repr']
-
-        msgs = [ppty_repr]
-
-        for object_name in self.objects:
-
-            if object_name in self.object_properties[ppty]:
-                value = self._get_property(ppty_cmd, object_name)
-            else:
-                value = 'N/A'
-
-            object_name_str = object_name.ljust(self.max_name_length + 3, '-')
-            msg = f'{object_name_str}{value}'
-            msgs.append(msg)
-
-        print('\n'.join(msgs))
-
-    def _print_help(self):
-        """Print help on objects, controlled properties and commands."""
-
-        nmax, _ = os.get_terminal_size()
-
-        print("OBJECTS ".ljust(nmax, '='))
-
-        for name, obj in self.objects.items():
-            print(f'--- {name} [{obj}]')
-            cont_props = obj.controlled_properties
-            cont_reprs = [self.properties[ppty]['repr'] for ppty in cont_props]
-            for cont_repr in cont_reprs:
-                print(f'{" " * 8}{cont_repr}')
-
-        print("COMMANDS ".ljust(nmax, '='))
-
-        print('--- Properties')
-        for ppty, ppty_data in self.properties.items():
-            ppty_repr = ppty_data['repr']
-            ppty_cmds = ppty_data['commands']
-            print(f'{" " * 8}{", ".join(ppty_cmds)} -- {ppty_repr} [{ppty}]')
-
-        print('--- Events')
-        for event_name, event_data in self.events.items():
-            print(f'{" " * 8}{", ".join(event_data["commands"])} -- {event_name}')
-
-        print('--- Exit')
-        print(f'{" " * 8}{", ".join(self.stop_commands)}')
-
-        try:
-            name = random.choice(list(self.objects))
-            ppty = random.choice(list(self.objects[name].controlled_properties))
-        except IndexError:
-            pass
-        else:
-            print("EXAMPLE ".ljust(nmax, '='))
-
-            ppty_repr = self.properties[ppty]['repr']
-            ppty_cmd = random.choice(self.properties[ppty]['commands'])
-
-            print(f'{ppty_cmd}-{name} xx -- change {ppty_repr} to xx for {name} only')
-            print(f'{ppty_cmd} xx -- change {ppty_repr} to xx for all relevant objects')
-
-            print('=' * nmax)
-
-    # ------------------------------------------------------------------------
-    # ========================= MAIN INTERACTIVE CLI =========================
-    # ------------------------------------------------------------------------
-
-    def run(self):
-        """Start the CLI (blocking)."""
-
-        while not self.stop_event.is_set():
-
-            command = input(f'Type command (help: ?): ')
-
-            # Print help -----------------------------------------------------
-
-            if command == '?':
-                self._print_help()
-
-            # Stop all recordings --------------------------------------------
-
-            elif command in self.stop_commands:
-                for obj in self.objects.values():
-                    try:
-                        obj.on_stop()
-                    except AttributeError:
-                        pass
-                self.stop_event.set()
-                print('CLI stopped')
-
-            # Trigger events -------------------------------------------------
-
-            elif command in self.event_commands:
-                event_name = self.event_commands[command]
-                print(f'{event_name.capitalize()} event requested')
-                event = self.events[event_name]['event']
-                event.set()
-
-            # Change properties of objects -----------------------------------
-
-            else:
-
-                for ppty_cmd in self.property_commands:
-
-                    nlett = len(ppty_cmd)
-
-                    # e.g. 'dt' --> inquire about current settings ...........
-                    if command == ppty_cmd:
-                        self._print_properties(ppty_cmd)
-                        break
-
-                    # e.g. 'dt 10' --> change setting for all types at once ..
-                    elif command[:nlett + 1] == ppty_cmd + ' ':
-                        value = command[nlett + 1:]
-                        for object_name in self.objects:
-                            self._set_property(ppty_cmd, object_name, value)
-                        break
-
-                    # e.g. 'dt-P 10' --> change setting only for pressure ....
-                    else:
-                        found = False
-                        for object_name in self.objects:
-                            specific_cmd = f'{ppty_cmd}-{object_name}'  # e.g. 'dt-P'
-                            nspec = len(specific_cmd)
-                            if command[:nspec] == specific_cmd:
-                                value = command[nspec + 1:]
-                                self._set_property(ppty_cmd, object_name, value)
-                                found = True
-                                break
-                        if found:
-                            break
-
-                else:  # at that point, it means nothing else has worked
-                    print('Unknown Command. ')
+"""Interactive command line interface (CLI)."""
+
+
+from threading import Event
+import random
+import os
+
+
+# TODO -- use match statement with python >= 3.10 instead of if/else?
+
+
+class ControlledProperty:
+    """Class to manage object properties controlled by the CLI."""
+
+    def __init__(self, attribute, readable, commands):
+        """Init ControlledProperty object
+
+        Parameters
+        ----------
+
+        - attribute: name of the (settable) object attribute to control
+                    (can be sub-attributes, e.g. a property of an attribute)
+        - readable: human-readable name for the property (for repr purposes)
+        - commands: iterable of command names (str) that will trigger
+                    modification of the property when typed in the CLI
+
+        Example
+        -------
+        interval = ControlledProperty(attribute='timer.interval'
+                                      readable='Δt (s)',
+                                      commands= ('dt',))
+        """
+        self.attribute = attribute
+        self.readable = readable
+        self.commands = commands
+
+    def __repr__(self):
+        msg = f'{self.__class__.__name__} ({self.readable}) '
+        msg += f'[attribute: {self.attribute}] [commands: {self.commands}]'
+        return msg
+
+
+class ControlledEvent:
+    """Class to manage events controlled by the CLI."""
+
+    def __init__(self, event, readable, commands):
+        """Init ControlledProperty object
+
+        Parameters
+        ----------
+
+        - event: Event object to control (typically, from threading)
+        - readable: human-readable name for the property (for repr purposes)
+        - commands: iterable of command names (str) that will trigger
+                    modification of the property when typed in the CLI
+
+        Example
+        -------
+        stop = ControlledEvent(event=stop_event,
+                               readable='stop',
+                               commands=('q', 'quit'))
+        """
+        self.event = event
+        self.readable = readable
+        self.commands = commands
+
+    def __repr__(self):
+        msg = f'{self.__class__.__name__} ({self.readable}) '
+        msg += f'[event: {self.event}] [commands: {self.commands}]'
+        return msg
+
+
+# ================================ MAIN CLASS ================================
+
+
+class CommandLineInterface:
+    """Interactive CLI to manage properties of objects and trigger events
+
+    All objects controlled are referred to with a name.
+    Below, we call an arbitrary name X, e.g. X=P for a pressure reading object).
+
+    The CLI can control an arbitrary number of properties for every object
+    (for example time interval, averaging number, etc.). These properties
+    have commands associated with them. Below, we call can arbitrary property
+    command y, e.g. y=dt for time interval.
+
+    It is also possible to trigger events (e.g. request a graph) with some
+    pre-defined commands. Below, we call these commands for event z.
+
+    Once the CLI is started (self.run()), the user input options are:
+    - y: inquire current settings (e.g. dt)
+    - y val: change property value of all objects to a value val (e.g. dt 10)
+    - dt-X val: change settings of only object X to value val (e.g. dt-P 5)
+    - z: trigger event (stop event is by default 'Q', 'q' or 'quit', can be changed)
+    """
+
+    def __init__(self, objects, events):
+        """Create interactive command line interface.
+
+        Parameters
+        ----------
+        - objects: dict of {name: object} of objects to control
+                   (name is a str used in the CLI to refer to the object)
+                   objects can define a on_stop() method which indicates
+                   specific things to do when the stop event is set.
+                   objects must define a `controlled_properties` attribute
+                   that lists which ones of its settable properties is
+                   controlled by the CLI. `controlled_properties` is an
+                   iterable of ControlledProperty objects.
+
+        - events: iterable of events to control
+                  (of type ControlledEvent or subclass)
+
+                  Note: the 'stop' event, if provided, gets linked to the
+                  event that triggers exiting of the CLI. If not provided,
+                  the 'stop' event is defined internally
+        """
+        self.objects = objects
+        properties = self._get_object_properties()
+        self.properties, self.events = self._create_ppty_and_event_dicts(properties, events)
+
+        try:
+            self.stop_dict = self.events.pop('stop')
+        except KeyError:
+            print('Stop event not passed. Creating one internally.')
+            self.stop_event = Event()
+            self.stop_commands = 'q', 'Q', 'quit'
+        else:
+            self.stop_event = self.stop_dict['event']
+            self.stop_commands = self.stop_dict['commands']
+
+        # Note: stop_commands is a tuple, event/property_commmands are dicts.
+        self.event_commands = self._get_commands(self.events)
+        self.property_commands = self._get_commands(self.properties)
+
+        # Dict {ppty: [object names that have this ppty controlled]}
+        self.object_properties = self._get_controlled_properties(objects)
+
+        # For CLI printing
+        self.max_name_length = max([len(obj) for obj in self.objects])
+
+    def _get_object_properties(self):
+        all_properties = set()
+        for obj in self.objects.values():
+            all_properties.update(obj.controlled_properties)
+        return tuple(all_properties)
+
+    def _create_ppty_and_event_dicts(self, properties, events):
+        """Move from ControlledProperty and ControlledEvent classes to dicts.
+
+        I do this because for now it's too much work to redesign all the
+        code around these new classes.
+        """
+        ppty_dict = {ppty.attribute: {'repr': ppty.readable,
+                                      'commands': ppty.commands}
+                     for ppty in properties}
+        event_dict = {event.readable: {'event': event.event,
+                                       'commands': event.commands}
+                      for event in events}
+        return ppty_dict, event_dict
+
+    def _get_controlled_properties(self, objects):
+        """Generate dict {ppty: [object names that have this ppty controlled]}."""
+        object_properties = {}
+        for ppty in self.properties:
+            object_properties[ppty] = []
+            for object_name, obj in objects.items():
+                ctrl_ppties = [ppty.attribute for ppty in obj.controlled_properties]
+                if ppty in ctrl_ppties:
+                    object_properties[ppty].append(object_name)
+        return object_properties
+
+    @staticmethod
+    def _get_commands(input_data):
+        """Create dict of which command input modifies which property/event.
+
+        Parameters
+        ----------
+        input_data: dict of dict (can be properties dict or event dict)
+
+        Example
+        -------
+        input_data = {'graph': {'event': e_graph,
+                                'commands': ('g', 'graph')},
+                      'stop': {'event': e_stop,
+                               'commands': ('q', 'Q', 'quit')}
+                      }
+        will return {'g': 'graph',
+                     'graph': 'graph',
+                     'q': 'stop',
+                     'Q': 'stop',
+                     'quit': 'stop'}
+        """
+        commands = {}
+        for name, data_dict in input_data.items():
+            for command_name in data_dict['commands']:
+                commands[command_name] = name
+        return commands
+
+    def _set_property(self, ppty_cmd, object_name, value):
+        """Manage command from CLI to set a property accordingly."""
+        obj = self.objects[object_name]
+        ppty = self.property_commands[ppty_cmd]
+
+        if object_name not in self.object_properties[ppty]:
+            return
+
+        ppty_repr = self.properties[ppty]['repr']
+        try:
+            exec(f'obj.{ppty} = {value}')  # avoids having to pass a convert function
+        except Exception:
+            print(f"'{value}' not a valid {ppty_repr} ({ppty})")
+        else:
+            print(f'New {ppty_repr} for {object_name}: {value}')
+
+    def _get_property(self, ppty_cmd, object_name):
+        """Get property according to given property command from CLI."""
+        obj = self.objects[object_name]
+        ppty = self.property_commands[ppty_cmd]
+
+        if object_name not in self.object_properties[ppty]:
+            return
+
+        # exec() strategy avoids having to pass a convert function
+        self._value = None  # exec won't work with local references
+        exec(f'self._value = obj.{ppty}')
+        return self._value
+
+    def _print_properties(self, ppty_cmd):
+        """Print current values of properties of all objects"""
+        ppty = self.property_commands[ppty_cmd]
+        ppty_repr = self.properties[ppty]['repr']
+
+        msgs = [ppty_repr]
+
+        for object_name in self.objects:
+
+            if object_name in self.object_properties[ppty]:
+                value = self._get_property(ppty_cmd, object_name)
+            else:
+                value = 'N/A'
+
+            object_name_str = object_name.ljust(self.max_name_length + 3, '-')
+            msg = f'{object_name_str}{value}'
+            msgs.append(msg)
+
+        print('\n'.join(msgs))
+
+    def _print_help(self):
+        """Print help on objects, controlled properties and commands."""
+
+        try:
+            nmax, _ = os.get_terminal_size()
+        except OSError:  # happens in some cases (e.g. simulated terminals)
+            nmax = 80
+
+        print("OBJECTS ".ljust(nmax, '='))
+
+        for name, obj in self.objects.items():
+            print(f'--- {name} [{obj}]')
+            cont_props = [ppty.attribute for ppty in obj.controlled_properties]
+            cont_reprs = [self.properties[ppty]['repr'] for ppty in cont_props]
+            for cont_repr in cont_reprs:
+                print(f'{" " * 8}{cont_repr}')
+
+        print("COMMANDS ".ljust(nmax, '='))
+
+        print('--- Properties')
+        for ppty, ppty_data in self.properties.items():
+            ppty_repr = ppty_data['repr']
+            ppty_cmds = ppty_data['commands']
+            print(f'{" " * 8}{", ".join(ppty_cmds)} -- {ppty_repr} [{ppty}]')
+
+        print('--- Events')
+        for event_name, event_data in self.events.items():
+            print(f'{" " * 8}{", ".join(event_data["commands"])} -- {event_name}')
+
+        print('--- Exit')
+        print(f'{" " * 8}{", ".join(self.stop_commands)}')
+
+        try:
+            name = random.choice(list(self.objects))
+            ppty = random.choice(list(self.objects[name].controlled_properties))
+        except IndexError:
+            pass
+        else:
+            print("EXAMPLE ".ljust(nmax, '='))
+
+            ppty_repr = ppty.readable
+            ppty_cmd = random.choice(ppty.commands)
+
+            print(f'{ppty_cmd}-{name} xx -- change {ppty_repr} to xx for {name} only')
+            print(f'{ppty_cmd} xx -- change {ppty_repr} to xx for all relevant objects')
+
+            print('=' * nmax)
+
+    # ------------------------------------------------------------------------
+    # ========================= MAIN INTERACTIVE CLI =========================
+    # ------------------------------------------------------------------------
+
+    def run(self):
+        """Start the CLI (blocking)."""
+
+        while not self.stop_event.is_set():
+
+            command = input(f'Type command (help: ?): ')
+
+            # Print help -----------------------------------------------------
+
+            if command == '?':
+                self._print_help()
+
+            # Stop all recordings --------------------------------------------
+
+            elif command in self.stop_commands:
+                for obj in self.objects.values():
+                    try:
+                        obj.on_stop()
+                    except AttributeError:
+                        pass
+                self.stop_event.set()
+                print('CLI stopped')
+
+            # Trigger events -------------------------------------------------
+
+            elif command in self.event_commands:
+                event_name = self.event_commands[command]
+                print(f'{event_name.capitalize()} event requested')
+                event = self.events[event_name]['event']
+                event.set()
+
+            # Change properties of objects -----------------------------------
+
+            else:
+
+                for ppty_cmd in self.property_commands:
+
+                    nlett = len(ppty_cmd)
+
+                    # e.g. 'dt' --> inquire about current settings ...........
+                    if command == ppty_cmd:
+                        self._print_properties(ppty_cmd)
+                        break
+
+                    # e.g. 'dt 10' --> change setting for all types at once ..
+                    elif command[:nlett + 1] == ppty_cmd + ' ':
+                        value = command[nlett + 1:]
+                        for object_name in self.objects:
+                            self._set_property(ppty_cmd, object_name, value)
+                        break
+
+                    # e.g. 'dt-P 10' --> change setting only for pressure ....
+                    else:
+                        found = False
+                        for object_name in self.objects:
+                            specific_cmd = f'{ppty_cmd}-{object_name}'  # e.g. 'dt-P'
+                            nspec = len(specific_cmd)
+                            if command[:nspec] == specific_cmd:
+                                value = command[nspec + 1:]
+                                self._set_property(ppty_cmd, object_name, value)
+                                found = True
+                                break
+                        if found:
+                            break
+
+                else:  # at that point, it means nothing else has worked
+                    print('Unknown Command. ')
```

### Comparing `clivo-0.3.0/setup.cfg` & `clivo-0.4.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2063 6c69 766f 0d0a 6175 7468 6f72   = clivo..author
-00000020: 203d 204f 6c69 7669 6572 2056 696e 6365   = Olivier Vince
-00000030: 6e74 0d0a 6175 7468 6f72 5f65 6d61 696c  nt..author_email
-00000040: 203d 206f 7669 6e63 2e70 7940 676d 6169   = ovinc.py@gmai
-00000050: 6c2e 636f 6d0d 0a75 726c 203d 2068 7474  l.com..url = htt
-00000060: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000070: 6f76 696e 632f 636c 6976 6f0d 0a64 6573  ovinc/clivo..des
-00000080: 6372 6970 7469 6f6e 203d 2047 656e 6572  cription = Gener
-00000090: 616c 2063 6f6d 6d61 6e64 206c 696e 6520  al command line 
-000000a0: 696e 7465 7266 6163 6520 746f 2063 6f6e  interface to con
-000000b0: 7472 6f6c 206f 626a 6563 7420 7072 6f70  trol object prop
-000000c0: 6572 7469 6573 2069 6e20 7265 616c 2074  erties in real t
-000000d0: 696d 6520 616e 6420 7472 6967 6765 7220  ime and trigger 
-000000e0: 6576 656e 7473 0d0a 6c6f 6e67 5f64 6573  events..long_des
-000000f0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000100: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-00000110: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-00000120: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000130: 2f6d 6172 6b64 6f77 6e0d 0a6b 6579 776f  /markdown..keywo
-00000140: 7264 7320 3d20 636f 6d6d 616e 642c 206c  rds = command, l
-00000150: 696e 652c 2069 6e74 6572 6661 6365 0d0a  ine, interface..
-00000160: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000170: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000180: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000190: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001b0: 7974 686f 6e20 3a3a 2033 2e36 0d0a 0950  ython :: 3.6...P
-000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001e0: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
-000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000200: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000210: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000220: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000230: 2033 2e39 0d0a 094c 6963 656e 7365 203a   3.9...License :
-00000240: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000250: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
-00000260: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000270: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000280: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000290: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-000002a0: 5f64 6174 6120 3d20 5472 7565 0d0a 7061  _data = True..pa
-000002b0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-000002c0: 7365 7475 705f 7265 7175 6972 6573 203d  setup_requires =
-000002d0: 200d 0a09 7365 7475 7074 6f6f 6c73 5f73   ...setuptools_s
-000002e0: 636d 0d0a 7079 7468 6f6e 5f72 6571 7569  cm..python_requi
-000002f0: 7265 7320 3d20 0d0a 093e 3d33 2e36 0d0a  res = ...>=3.6..
-00000300: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000310: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000320: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 636c 6976 6f0a 6175 7468 6f72 203d  = clivo.author =
+00000020: 204f 6c69 7669 6572 2056 696e 6365 6e74   Olivier Vincent
+00000030: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000040: 6f76 696e 632e 7079 4067 6d61 696c 2e63  ovinc.py@gmail.c
+00000050: 6f6d 0a75 726c 203d 2068 7474 7073 3a2f  om.url = https:/
+00000060: 2f67 6974 6875 622e 636f 6d2f 6f76 696e  /github.com/ovin
+00000070: 632f 636c 6976 6f0a 6465 7363 7269 7074  c/clivo.descript
+00000080: 696f 6e20 3d20 4765 6e65 7261 6c20 636f  ion = General co
+00000090: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
+000000a0: 6661 6365 2074 6f20 636f 6e74 726f 6c20  face to control 
+000000b0: 6f62 6a65 6374 2070 726f 7065 7274 6965  object propertie
+000000c0: 7320 696e 2072 6561 6c20 7469 6d65 2061  s in real time a
+000000d0: 6e64 2074 7269 6767 6572 2065 7665 6e74  nd trigger event
+000000e0: 730a 6c6f 6e67 5f64 6573 6372 6970 7469  s.long_descripti
+000000f0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000100: 452e 6d64 0a6c 6f6e 675f 6465 7363 7269  E.md.long_descri
+00000110: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000120: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000130: 776e 0a6b 6579 776f 7264 7320 3d20 636f  wn.keywords = co
+00000140: 6d6d 616e 642c 206c 696e 652c 2069 6e74  mmand, line, int
+00000150: 6572 6661 6365 0a63 6c61 7373 6966 6965  erface.classifie
+00000160: 7273 203d 200a 0950 726f 6772 616d 6d69  rs = ..Programmi
+00000170: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000180: 7974 686f 6e20 3a3a 2033 0a09 5072 6f67  ython :: 3..Prog
+00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001b0: 360a 0950 726f 6772 616d 6d69 6e67 204c  6..Programming L
+000001c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001d0: 6e20 3a3a 2033 2e37 0a09 5072 6f67 7261  n :: 3.7..Progra
+000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000200: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000210: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000220: 3a3a 2033 2e39 0a09 4c69 6365 6e73 6520  :: 3.9..License 
+00000230: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000240: 3a3a 2042 5344 204c 6963 656e 7365 0a09  :: BSD License..
+00000250: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000260: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000270: 6e74 0a0a 5b6f 7074 696f 6e73 5d0a 696e  nt..[options].in
+00000280: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000290: 7461 203d 2054 7275 650a 7061 636b 6167  ta = True.packag
+000002a0: 6573 203d 2066 696e 643a 0a73 6574 7570  es = find:.setup
+000002b0: 5f72 6571 7569 7265 7320 3d20 0a09 7365  _requires = ..se
+000002c0: 7475 7074 6f6f 6c73 5f73 636d 0a70 7974  tuptools_scm.pyt
+000002d0: 686f 6e5f 7265 7175 6972 6573 203d 200a  hon_requires = .
+000002e0: 093e 3d33 2e36 0a0a 5b65 6767 5f69 6e66  .>=3.6..[egg_inf
+000002f0: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
+00000300: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
```

