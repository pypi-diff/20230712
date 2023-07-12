# Comparing `tmp/Akatosh-2.1.1.tar.gz` & `tmp/Akatosh-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.1.tar", last modified: Tue Jul 11 12:53:33 2023, max compression
+gzip compressed data, was "Akatosh-2.1.2.tar", last modified: Wed Jul 12 07:58:50 2023, max compression
```

## Comparing `Akatosh-2.1.1.tar` & `Akatosh-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.871408 Akatosh-2.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.856414 Akatosh-2.1.1/Akatosh/
--rw-rw-rw-   0        0        0      181 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/__init__.py
--rw-rw-rw-   0        0        0     5122 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/entity.py
--rw-rw-rw-   0        0        0    11587 2023-07-11 12:50:46.000000 Akatosh-2.1.1/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/states.py
--rw-rw-rw-   0        0        0     5467 2023-07-11 12:42:40.000000 Akatosh-2.1.1/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:53:33.867410 Akatosh-2.1.1/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 12:53:33.000000 Akatosh-2.1.1/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-11 12:53:33.869408 Akatosh-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.1/README.md
--rw-rw-rw-   0        0        0      635 2023-07-11 12:52:28.000000 Akatosh-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 12:53:33.871408 Akatosh-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.888119 Akatosh-2.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.824120 Akatosh-2.1.2/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.2/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    12961 2023-07-12 07:56:31.000000 Akatosh-2.1.2/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.2/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/states.py
+-rw-rw-rw-   0        0        0     5356 2023-07-12 07:48:11.000000 Akatosh-2.1.2/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.877124 Akatosh-2.1.2/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-12 07:58:50.885120 Akatosh-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.2/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-12 07:20:32.000000 Akatosh-2.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:58:50.891145 Akatosh-2.1.2/setup.cfg
```

### Comparing `Akatosh-2.1.1/Akatosh/event.py` & `Akatosh-2.1.2/Akatosh/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,20 @@
         if callable(priority):
             self._priority = priority()
         else:
             self._priority = priority
         # assign label
         self._label = label
         # add to the universe
-        Mundus.future_events.append(self)
+        if Mundus.now<self.at:
+            Mundus.future_events.append(self)
+        elif Mundus.now>self.at:
+            raise RuntimeError(f"Event {self.label} tries to later the past.")
+        else:
+            Mundus.current_events.append(self)
 
     def end(self):
         """End the event and activate the follower events if there is any."""
         self.state = State.ENDED
         for event in self.follower:
             try:
                 event.activate()
@@ -100,15 +105,21 @@
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
         self.state = State.CANCELED
-
+        if self in Mundus.future_events:
+            Mundus.future_events.remove(self)
+        if self in Mundus.current_events:
+            Mundus.current_events.remove(self)
+        Mundus.past_events.append(self)
+        logger.debug(f"Event {self.label} is cancelled.")
+        
     @abstractmethod
     async def _perform(self):
         """Abstract method for the event to perform its action."""
         pass
 
     def __eq__(self, _o: Event) -> bool:
         """Determine if two events are the same."""
@@ -213,15 +224,15 @@
                     self.action()
             Mundus.current_events.remove(self)
             Mundus.past_events.append(self)
             self.end()
             logger.debug(f"Event {self.label} is ended.")
 
 
-def event(
+def instant_event(
     at: int | float | Callable,
     precursor: Event | List[Event] | None = None,
     priority: int | float | Callable = 0,
     label: str | None = None,
     **kwargs,
 ):
     """Decorator for creating instant event.
@@ -229,25 +240,25 @@
     Args:
         at (int | float | Callable): When the event happens.
         precursor (Event | List[Event] | None, optional): The precursor events. Defaults to None.
         priority (int | float | Callable, optional): The priority of the event. Defaults to 0.
         label (str | None, optional): Short description of the event. Defaults to None.
     """
 
-    def _event(func: Callable):
+    def _instant_event(func: Callable):
         return InstantEvent(
             at=at,
             precursor=precursor,
             action=func,
             priority=priority,
             label=label,
             **kwargs,
         )
 
-    return _event
+    return _instant_event
 
 
 class ContinuousEvent(Event):
     def __init__(
         self,
         at: int | float | Callable[..., Any],
         interval: int | float | Callable[..., Any],
@@ -273,14 +284,15 @@
             at=at,
             precursor=precursor,
             action=action,
             priority=priority,
             label=label,
             **kwargs,
         )
+
         self._interval = interval
         if callable(duration):
             self._duration = round(duration(), Mundus.resolution)
         else:
             self._duration = round(duration, Mundus.resolution)
         self._till = self.at + self.duration
         self._sub_events: List[InstantEvent] = list()
@@ -317,7 +329,42 @@
         """Return the time when the event ends."""
         return self._till
 
     @property
     def sub_events(self) -> List[InstantEvent]:
         """Return the sub events of the continous event."""
         return self._sub_events
+
+
+def continuous_event(
+    at: int | float | Callable,
+    interval: int | float | Callable,
+    duration: int | float | Callable,
+    precursor: Event | List[Event] | None = None,
+    priority: int | float | Callable = 0,
+    label: str | None = None,
+    **kwargs,
+):
+    """A decorator for creating continous event.
+
+    Args:
+        at (int | float | Callable): when the continuous event starts.
+        interval (int | float | Callable): how frequent the event happens.
+        duration (int | float | Callable): the duration of the event.
+        precursor (Event | List[Event] | None, optional): the precursors for this event. Defaults to None.
+        priority (int | float | Callable, optional): the priority for this event. Defaults to 0.
+        label (str | None, optional): short description of the event. Defaults to None.
+    """
+
+    def _continous_event(func: Callable):
+        return ContinuousEvent(
+            at=at,
+            interval=interval,
+            duration=duration,
+            precursor=precursor,
+            action=func,
+            priority=priority,
+            label=label,
+            **kwargs,
+        )
+
+    return _continous_event
```

### Comparing `Akatosh-2.1.1/Akatosh/resource.py` & `Akatosh-2.1.2/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.1/Akatosh/universe.py` & `Akatosh-2.1.2/Akatosh/universe.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class Universe:
     def __init__(self) -> None:
         """The Simulation Universe."""
         self._resolution = (
             1  # the resolution of the time. 1 means minimum time unit is 0.1 second.
         )
-        self._now: int | float = 0  # the current time of the simulated universe.
+        self._now: int | float = -1  # the current time of the simulated universe.
         self._future_events: List[Event] = list()  # the future events queue.
         self._current_events: List[Event] = list()  # the current events queue.
         self._past_events: List[Event] = list()  # the past events queue.
         self._alduin: bool = False  # trigger to stop the simulation.
         self.set_logger(logging.ERROR)  # set the default logger level to ERROR.
 
     async def akatosh(self, till: int | float | None = None):
@@ -34,51 +34,48 @@
         Raises:
             RuntimeError: raise if the event is in unknown state or being placed in wrong event queue.
         """
         while len(self.future_events) != 0:
             if self.alduin:
                 return
 
-            if self.now < min(event.at for event in self.future_events):
-                active_event = [
-                    event for event in self.future_events if event.state == State.ACTIVE
-                ]
-                if len(active_event) == 0:
-                    return
-                else:
-                    self._now = min(event.at for event in active_event)
+            active_future_event = [
+                event for event in self.future_events if event.state == State.ACTIVE
+            ]
+            if len(active_future_event) == 0:
+                return
+            _time = min(event.at for event in active_future_event)
+            if self.now < _time:
+                self._now = _time
                 if till is not None:
                     if self.now > till:
                         return
             logger.debug(f"Time: {self.now}")
 
             logger.debug(
-                f"Future events: {[(event.at, event.label) for event in self.future_events]}"
+                f"Future active events: {[(event.at, event.label) for event in self.future_events]}"
             )
 
             for event in self.future_events[:]:
-                if event.at == self.now:
+                if event.at <= self.now:
                     if event.state == State.ACTIVE or event.state == State.INACTIVE:
                         logger.debug(f"Event {event.label} is triggered.")
                         self.future_events.remove(event)
                         self.current_events.append(event)
                     elif event.state == State.CANCELED:
-                        logger.debug(f"Event {event.label} is canceled.")
-                        self.future_events.remove(event)
-                        self.past_events.append(event)
-                        event.state = State.ENDED
+                        raise RuntimeError(f"Event {event.label} is canceled but inside future events queue.")
                     elif event.state == State.ENDED:
                         raise RuntimeError(
                             f"Event {event.label} is ended but inside future events queue."
                         )
                     else:
                         raise RuntimeError(f"Event {event.label} is in unknown state.")
 
             logger.debug(
-                f"Current events: {[event.label for event in self.current_events]}"
+                f"Current events: {[(event.priority, event.label) for event in self.current_events]}"
             )
 
             while (
                 len(
                     [
                         event
                         for event in self.current_events
@@ -89,15 +86,15 @@
             ):
                 priority = min(
                     event.priority
                     for event in self.current_events
                     if event.state == State.ACTIVE
                 )
                 logger.debug(
-                    f"Current Priority: {priority}, {[(event.label, event.priority) for event in self.current_events]}"
+                    f"Current Priority: {priority}, Executing events: {[event.label for event in self.current_events if event.priority == priority]}"
                 )
                 await asyncio.gather(
                     *[
                         event._perform()
                         for event in self.current_events
                         if event.priority == priority
                     ]
```

### Comparing `Akatosh-2.1.1/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.2/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.1
+Version: 2.1.2
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.1/PKG-INFO` & `Akatosh-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.1
+Version: 2.1.2
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.1/README.md` & `Akatosh-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.1/pyproject.toml` & `Akatosh-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.1"
+version = "2.1.2"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

