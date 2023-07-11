# Comparing `tmp/wyoming-0.0.1.tar.gz` & `tmp/wyoming-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming-0.0.1.tar", last modified: Tue Apr 18 03:43:26 2023, max compression
+gzip compressed data, was "wyoming-1.0.0.tar", last modified: Tue Jul 11 22:14:33 2023, max compression
```

## Comparing `wyoming-0.0.1.tar` & `wyoming-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:43:26.824047 wyoming-0.0.1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      635 2023-04-18 03:43:26.824047 wyoming-0.0.1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-18 03:43:26.824047 wyoming-0.0.1/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      879 2023-04-18 03:43:26.000000 wyoming-0.0.1/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:43:26.824047 wyoming-0.0.1/wyoming/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      563 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/asr.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5601 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1938 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/client.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3705 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/event.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1283 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/handle.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2178 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/info.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2692 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/intent.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3341 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/server.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2682 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/snd.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      643 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/tts.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:43:26.824047 wyoming-0.0.1/wyoming/util/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/util/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1890 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/util/dataclasses_json.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1263 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/vad.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1293 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming/wake.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:43:26.824047 wyoming-0.0.1/wyoming.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      635 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      408 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        8 2023-04-18 03:43:26.000000 wyoming-0.0.1/wyoming.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-11 22:14:33.807593 wyoming-1.0.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-11 22:14:33.807593 wyoming-1.0.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      879 2023-07-11 22:14:33.000000 wyoming-1.0.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1586 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/asr.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5718 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1938 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/client.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4104 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/event.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1283 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/handle.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3066 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/info.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2692 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/intent.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4358 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/server.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      428 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/snd.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2038 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/tts.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming/util/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/util/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2192 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/util/dataclasses_json.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1263 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/vad.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1293 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/wake.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      408 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        8 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/top_level.txt
```

### Comparing `wyoming-0.0.1/PKG-INFO` & `wyoming-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: wyoming
-Version: 0.0.1
+Version: 1.0.0
 Summary: Protocol for Rhasspy Voice Assistant
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
+Description: UNKNOWN
 Keywords: voice assistant rhasspy
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `wyoming-0.0.1/setup.py` & `wyoming-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 from setuptools import setup
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming",
-    version="0.0.1",
+    version="1.0.0",
     description="Protocol for Rhasspy Voice Assistant",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=["wyoming", "wyoming.util"],
     classifiers=[
```

### Comparing `wyoming-0.0.1/wyoming/audio.py` & `wyoming-1.0.0/wyoming/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,19 +183,28 @@
                 channels,
                 chunk.rate,
                 self.rate,
                 self._ratecv_state,
             )
             rate = self.rate
 
-        return AudioChunk(rate, width, channels, audio_bytes, timestamp=chunk.timestamp)
+        return AudioChunk(
+            rate,
+            width,
+            channels,
+            audio_bytes,
+            timestamp=chunk.timestamp,
+        )
 
 
 def wav_to_chunks(
-    wav_file: wave.Wave_read, samples_per_chunk: int, timestamp: int = 0
+    wav_file: wave.Wave_read,
+    samples_per_chunk: int,
+    timestamp: int = 0,
+    stream_id: Optional[str] = None,
 ) -> Iterable[AudioChunk]:
     """Splits WAV file into AudioChunks."""
     rate = wav_file.getframerate()
     width = wav_file.getsampwidth()
     channels = wav_file.getnchannels()
     audio_bytes = wav_file.readframes(samples_per_chunk)
     while audio_bytes:
```

### Comparing `wyoming-0.0.1/wyoming/client.py` & `wyoming-1.0.0/wyoming/client.py`

 * *Files identical despite different names*

### Comparing `wyoming-0.0.1/wyoming/event.py` & `wyoming-1.0.0/wyoming/event.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,29 @@
     def is_type(event_type: str) -> bool:
         pass
 
     def to_dict(self) -> Dict[str, Any]:
         return self.event().data
 
 
+async def async_get_stdin(
+    loop: Optional[asyncio.AbstractEventLoop] = None,
+) -> asyncio.StreamReader:
+    """Get StreamReader for stdin."""
+    if loop is None:
+        loop = asyncio.get_running_loop()
+
+    reader = asyncio.StreamReader()
+    await loop.connect_read_pipe(
+        lambda: asyncio.StreamReaderProtocol(reader), sys.stdin
+    )
+
+    return reader
+
+
 async def async_read_event(reader: asyncio.StreamReader) -> Optional[Event]:
     try:
         json_line = await reader.readline()
         if not json_line:
             return None
 
         event_dict = json.loads(json_line)
@@ -51,15 +66,15 @@
         payload: Optional[bytes] = None
         if payload_length is not None:
             payload = await reader.readexactly(payload_length)
 
         return Event(
             type=event_dict[_TYPE], data=event_dict.get(_DATA), payload=payload
         )
-    except KeyboardInterrupt:
+    except (KeyboardInterrupt, ValueError):
         pass
 
     return None
 
 
 async def async_write_event(event: Event, writer: asyncio.StreamWriter):
     event_dict: Dict[str, Any] = event.to_dict()
@@ -116,15 +131,15 @@
         payload: Optional[bytes] = None
         if payload_length is not None:
             payload = reader.read(payload_length)
 
         return Event(
             type=event_dict[_TYPE], data=event_dict.get(_DATA), payload=payload
         )
-    except KeyboardInterrupt:
+    except (KeyboardInterrupt, ValueError):
         pass
 
     return None
 
 
 def write_event(event: Event, writer: Optional[BinaryIO] = None):
     if writer is None:
```

### Comparing `wyoming-0.0.1/wyoming/handle.py` & `wyoming-1.0.0/wyoming/handle.py`

 * *Files identical despite different names*

### Comparing `wyoming-0.0.1/wyoming/info.py` & `wyoming-1.0.0/wyoming/intent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,101 @@
-"""Information about available services/artifacts."""
-from dataclasses import dataclass, field
-from typing import Any, Dict, List
+"""Intent recognition and handling."""
+from dataclasses import asdict, dataclass, field
+from typing import Any, Dict, List, Optional
 
 from .event import Event, Eventable
-from .util.dataclasses_json import DataClassJsonMixin
 
-DOMAIN = "info"
-_DESCRIBE_TYPE = "describe"
-_INFO_TYPE = "info"
+DOMAIN = "intent"
+_RECOGNIZE_TYPE = "recognize"
+_INTENT_TYPE = "intent"
+_NOT_RECOGNIZED_TYPE = "not-recognized"
 
 
 @dataclass
-class Describe(Eventable):
-    @staticmethod
-    def is_type(event_type: str) -> bool:
-        return event_type == _DESCRIBE_TYPE
-
-    def event(self) -> Event:
-        return Event(type=_DESCRIBE_TYPE)
-
-    @staticmethod
-    def from_event(event: Event) -> "Describe":
-        return Describe()
-
-
-@dataclass
-class Attribution(DataClassJsonMixin):
+class Entity:
     name: str
-    url: str
+    value: Optional[Any] = None
 
 
 @dataclass
-class Artifact(DataClassJsonMixin):
-    name: str
-    attribution: Attribution
-    installed: bool
+class Recognize(Eventable):
+    text: str
 
+    @staticmethod
+    def is_type(event_type: str) -> bool:
+        return event_type == _RECOGNIZE_TYPE
 
-@dataclass
-class AsrModel(Artifact):
-    languages: List[str]
-
+    def event(self) -> Event:
+        data: Dict[str, Any] = {"text": self.text}
+        return Event(type=_RECOGNIZE_TYPE, data=data)
 
-@dataclass
-class AsrProgram(Artifact):
-    models: List[AsrModel]
+    @staticmethod
+    def from_event(event: Event) -> "Recognize":
+        assert event.data is not None
+        return Recognize(text=event.data["text"])
 
 
 @dataclass
-class TtsVoice(Artifact):
+class Intent(Eventable):
     name: str
-    languages: List[str]
+    entities: List[Entity] = field(default_factory=list)
 
+    @staticmethod
+    def is_type(event_type: str) -> bool:
+        return event_type == _INTENT_TYPE
 
-@dataclass
-class TtsProgram(Artifact):
-    voices: List[TtsVoice]
+    def event(self) -> Event:
+        data: Dict[str, Any] = {"name": self.name}
+        if self.entities:
+            data["entities"] = [asdict(entity) for entity in self.entities]
 
+        return Event(type=_INTENT_TYPE, data=data)
 
-@dataclass
-class HandleModel(Artifact):
-    languages: List[str]
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> "Intent":
+        entity_dicts = data.get("entities")
+        if entity_dicts:
+            entities: List[Entity] = [
+                Entity(**entity_dict) for entity_dict in entity_dicts
+            ]
+        else:
+            entities = []
 
+        return Intent(name=data["name"], entities=entities)
 
-@dataclass
-class HandleProgram(Artifact):
-    models: List[HandleModel]
+    @staticmethod
+    def from_event(event: Event) -> "Intent":
+        assert event.data is not None
+        return Intent.from_dict(event.data)
+
+    def to_rhasspy(self) -> Dict[str, Any]:
+        return {
+            "intent": {
+                "name": self.name,
+            },
+            "entities": [
+                {"entity": entity.name, "value": entity.value}
+                for entity in self.entities
+            ],
+            "slots": {entity.name: entity.value for entity in self.entities},
+        }
 
 
 @dataclass
-class Info(Eventable):
-    asr: List[AsrProgram] = field(default_factory=list)
-    tts: List[TtsProgram] = field(default_factory=list)
-    handle: List[HandleProgram] = field(default_factory=list)
+class NotRecognized(Eventable):
+    text: Optional[str] = None
 
     @staticmethod
     def is_type(event_type: str) -> bool:
-        return event_type == _INFO_TYPE
+        return event_type == _NOT_RECOGNIZED_TYPE
 
     def event(self) -> Event:
-        data: Dict[str, Any] = {
-            "asr": [p.to_dict() for p in self.asr],
-            "tts": [p.to_dict() for p in self.tts],
-            "handle": [p.to_dict() for p in self.handle],
-        }
+        data: Dict[str, Any] = {}
+        if self.text is not None:
+            data["text"] = self.text
 
-        return Event(type=_INFO_TYPE, data=data)
+        return Event(type=_NOT_RECOGNIZED_TYPE, data=data)
 
     @staticmethod
-    def from_event(event: Event) -> "Info":
+    def from_event(event: Event) -> "NotRecognized":
         assert event.data is not None
-        return Info(
-            asr=[AsrProgram.from_dict(d) for d in event.data.get("asr", [])],
-            tts=[TtsProgram.from_dict(d) for d in event.data.get("tts", [])],
-            handle=[HandleProgram.from_dict(d) for d in event.data.get("handle", [])],
-        )
+        return NotRecognized(text=event.data.get("text"))
```

### Comparing `wyoming-0.0.1/wyoming/server.py` & `wyoming-1.0.0/wyoming/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
+import sys
 from abc import ABC, abstractmethod
 from functools import partial
 from pathlib import Path
 from typing import Callable, Set, Union
 
-from .event import Event, async_read_event, async_write_event
+from .event import Event, async_get_stdin, async_read_event, async_write_event
 
 
 class AsyncEventHandler(ABC):
     """Base class for async Wyoming event handler."""
 
     def __init__(
         self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
@@ -20,21 +21,27 @@
     async def handle_event(self, event: Event) -> bool:
         return True
 
     async def write_event(self, event: Event) -> None:
         await async_write_event(event, self.writer)
 
     async def run(self) -> None:
-        while True:
-            event = await async_read_event(self.reader)
-            if event is None:
-                break
+        try:
+            while True:
+                event = await async_read_event(self.reader)
+                if event is None:
+                    break
+
+                if not (await self.handle_event(event)):
+                    break
+        finally:
+            await self.disconnect()
 
-            if not (await self.handle_event(event)):
-                break
+    async def disconnect(self) -> None:
+        pass
 
 
 HandlerFactory = Callable[
     [asyncio.StreamReader, asyncio.StreamWriter], AsyncEventHandler
 ]
 
 
@@ -55,28 +62,55 @@
             return AsyncUnixServer(socket_path)
 
         if uri.startswith("tcp://"):
             host, port_str = uri[len("tcp://") :].split(":")
             port = int(port_str)
             return AsyncTcpServer(host, port)
 
-        raise ValueError("Only unix:// or tcp:// are supported")
+        if uri.startswith("stdio://"):
+            return AsyncStdioServer()
+
+        raise ValueError("Only 'stdio://', 'unix://', or 'tcp://' are supported")
 
     async def _handler_callback(
         self,
         handler_factory: HandlerFactory,
         reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter,
     ):
         handler = handler_factory(reader, writer)
         task = asyncio.create_task(handler.run())
         self._tasks.add(task)
         task.add_done_callback(self._tasks.discard)
 
 
+class AsyncStdioServer(AsyncServer):
+    """Wyoming server over stdin/stdout."""
+
+    async def run(self, handler_factory: HandlerFactory) -> None:
+        reader = await async_get_stdin()
+
+        # Get stdout writer.
+        # NOTE: This will make print() non-blocking.
+        loop = asyncio.get_running_loop()
+        writer_transport, writer_protocol = await loop.connect_write_pipe(
+            asyncio.streams.FlowControlMixin, sys.stdout
+        )
+        writer = asyncio.StreamWriter(writer_transport, writer_protocol, None, loop)
+
+        handler = handler_factory(reader, writer)
+        while True:
+            event = await async_read_event(reader)
+            if event is None:
+                break
+
+            if not (await handler.handle_event(event)):
+                break
+
+
 class AsyncTcpServer(AsyncServer):
     """Wyoming server over TCP."""
 
     def __init__(self, host: str, port: int) -> None:
         super().__init__()
         self.host = host
         self.port = port
@@ -92,15 +126,14 @@
 
 class AsyncUnixServer(AsyncServer):
     """Wyoming server over a Unix domain socket."""
 
     def __init__(self, socket_path: Union[str, Path]) -> None:
         super().__init__()
         self.socket_path = Path(socket_path)
-        self.tasks: Set[asyncio.Task] = set()
 
     async def run(self, handler_factory: HandlerFactory) -> None:
         # Need to unlink socket file if it exists
         self.socket_path.unlink(missing_ok=True)
 
         handler_callback = partial(self._handler_callback, handler_factory)
         server = await asyncio.start_unix_server(
```

### Comparing `wyoming-0.0.1/wyoming/util/dataclasses_json.py` & `wyoming-1.0.0/wyoming/util/dataclasses_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,23 @@
             field = cls_fields[key]
             if is_dataclass(field.type):
                 assert issubclass(field.type, DataClassJsonMixin), field.type
                 kwargs[key] = field.type.from_dict(value)
             else:
                 kwargs[key] = _decode(value, field.type)
 
+        # Fill in optional fields
+        for field in cls_fields.values():
+            if (
+                (field.name not in kwargs)
+                and hasattr(field.type, "__args__")
+                and (type(None) in field.type.__args__)
+            ):
+                kwargs[field.name] = None
+
         return cls(**kwargs)
 
     def to_dict(self) -> Dict[str, Any]:
         """Alias for asdict."""
         return asdict(self)
```

### Comparing `wyoming-0.0.1/wyoming/vad.py` & `wyoming-1.0.0/wyoming/vad.py`

 * *Files identical despite different names*

### Comparing `wyoming-0.0.1/wyoming/wake.py` & `wyoming-1.0.0/wyoming/wake.py`

 * *Files identical despite different names*

### Comparing `wyoming-0.0.1/wyoming.egg-info/PKG-INFO` & `wyoming-1.0.0/wyoming.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: wyoming
-Version: 0.0.1
+Version: 1.0.0
 Summary: Protocol for Rhasspy Voice Assistant
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
+Description: UNKNOWN
 Keywords: voice assistant rhasspy
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

