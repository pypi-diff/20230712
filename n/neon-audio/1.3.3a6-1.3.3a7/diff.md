# Comparing `tmp/neon-audio-1.3.3a6.tar.gz` & `tmp/neon-audio-1.3.3a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-audio-1.3.3a6.tar", last modified: Tue Jun 27 20:24:39 2023, max compression
+gzip compressed data, was "neon-audio-1.3.3a7.tar", last modified: Wed Jul 12 01:51:55 2023, max compression
```

## Comparing `neon-audio-1.3.3a6.tar` & `neon-audio-1.3.3a7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.965032 neon-audio-1.3.3a6/neon_audio/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/neon_audio/tts/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/tts/neon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/neon_audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.965032 neon-audio-1.3.3a6/neon_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:24:39.000000 neon-audio-1.3.3a6/neon_audio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/tests/api_method_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:24:39.969032 neon-audio-1.3.3a6/tests/test_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/tests/test_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-27 20:24:34.000000 neon-audio-1.3.3a6/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/tts/neon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/api_method_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/tests/test_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/test_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/unit_tests.py
```

### Comparing `neon-audio-1.3.3a6/LICENSE.md` & `neon-audio-1.3.3a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/PKG-INFO` & `neon-audio-1.3.3a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.3.3a6
+Version: 1.3.3a7
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.3.3a6/README.md` & `neon-audio-1.3.3a7/README.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/__init__.py` & `neon-audio-1.3.3a7/neon_audio/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/__main__.py` & `neon-audio-1.3.3a7/neon_audio/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/cli.py` & `neon-audio-1.3.3a7/neon_audio/cli.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/service.py` & `neon-audio-1.3.3a7/neon_audio/service.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/tts/__init__.py` & `neon-audio-1.3.3a7/neon_audio/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio/tts/neon.py` & `neon-audio-1.3.3a7/neon_audio/tts/neon.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 from ovos_plugin_manager.language import OVOSLangDetectionFactory,\
     OVOSLangTranslationFactory
 from ovos_plugin_manager.templates.tts import TTS, PlaybackThread
 from ovos_utils.enclosure.api import EnclosureAPI
 
 from neon_utils.file_utils import encode_file_to_base64_string
 from neon_utils.message_utils import resolve_message
-from neon_utils.signal_utils import create_signal
+from neon_utils.signal_utils import create_signal, check_for_signal,\
+    init_signal_bus
 from ovos_utils.log import LOG
 
 from ovos_config.config import Configuration
 
 
 def get_requested_tts_languages(msg) -> list:
     """
@@ -129,16 +130,32 @@
     return tts_reqs
 
 
 class NeonPlaybackThread(PlaybackThread):
     def __init__(self, queue):
         PlaybackThread.__init__(self, queue)
 
+    def begin_audio(self, message=None):
+        # TODO: Mark signals for deprecation
+        check_for_signal("isSpeaking")
+        create_signal("isSpeaking")
+        PlaybackThread.begin_audio(self, message)
+
+    def end_audio(self, listen, message=None):
+        PlaybackThread.end_audio(self, listen, message)
+        # TODO: Mark signals for deprecation
+        check_for_signal("isSpeaking")
+
     def _play(self):
         ident = self._now_playing[3]
+        if not ident and len(self._now_playing) >= 5 and \
+                isinstance(self._now_playing[4], Message):
+            LOG.debug("Handling new style playback")
+            ident = self._now_playing[4].context.get('session',
+                                                     {}).get('session_id')
         super()._play()
         LOG.info(f"Played {ident}")
         self.bus.emit(Message(ident))
 
 
 class WrappedTTS(TTS):
     def __new__(cls, base_engine, *args, **kwargs):
@@ -181,14 +198,15 @@
         return base_engine
 
     def _init_playback(self):
         # shutdown any previous thread
         if TTS.playback:
             TTS.playback.shutdown()
 
+        init_signal_bus(self.bus)
         TTS.playback = NeonPlaybackThread(TTS.queue)
         TTS.playback.set_bus(self.bus)
         TTS.playback.attach_tts(self)
         if not TTS.playback.enclosure:
             TTS.playback.enclosure = EnclosureAPI(self.bus)
         TTS.playback.start()
 
@@ -315,8 +333,9 @@
                         # queue for playback
                         self.queue.put((self.audio_ext, wav_file, vis, ident,
                                         listen))
                         self.handle_metric({"metric_type": "tts.queued"})
         else:
             LOG.warning(f'no Message associated with TTS request: {ident}')
             assert isinstance(self, TTS)
+            create_signal("isSpeaking")
             TTS.execute(self, sentence, ident, listen, **kwargs)
```

### Comparing `neon-audio-1.3.3a6/neon_audio/utils.py` & `neon-audio-1.3.3a7/neon_audio/utils.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/neon_audio.egg-info/PKG-INFO` & `neon-audio-1.3.3a7/neon_audio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.3.3a6
+Version: 1.3.3a7
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.3.3a6/neon_audio.egg-info/SOURCES.txt` & `neon-audio-1.3.3a7/neon_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/setup.py` & `neon-audio-1.3.3a7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,12 +80,13 @@
     zip_safe=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
     ],
     entry_points={
         'console_scripts': [
+            # TODO: Deprecate neon_audio_client entrypoint
             'neon_audio_client=neon_audio.__main__:main',
             'neon-audio=neon_audio.cli:neon_audio_cli'
         ]
     }
 )
```

### Comparing `neon-audio-1.3.3a6/tests/__init__.py` & `neon-audio-1.3.3a7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/tests/api_method_tests.py` & `neon-audio-1.3.3a7/tests/api_method_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,92 +26,85 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import sys
 import unittest
 
+from unittest.mock import Mock, patch
 from threading import Event
 from time import time
-from mock.mock import Mock
 from ovos_bus_client import Message
 from ovos_utils.messagebus import FakeBus
-from neon_utils.configuration_utils import init_config_dir
-from ovos_config.config import Configuration
 from neon_utils.message_utils import dig_for_message
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 from neon_audio.service import NeonPlaybackService
-from neon_audio.utils import use_neon_audio
+
+
+_TEST_CONFIG = {
+    "g2p": {"module": "dummy"},
+    "Audio": {},
+    "tts": {"module": "neon-tts-plugin-larynx-server",
+            "neon-tts-plugin-larynx-server": {"host": "https://larynx.2022.us/"}
+            }
+}
 
 
 class TestAPIMethods(unittest.TestCase):
+    bus = FakeBus()
+    bus.connected_event = Event()
+    bus.connected_event.set()
+    test_config_dir = os.path.join(os.path.dirname(__file__), "config")
+    os.environ["XDG_CONFIG_HOME"] = test_config_dir
+
     @classmethod
-    def setUpClass(cls) -> None:
-        test_config_dir = os.path.join(os.path.dirname(__file__), "config")
-        os.makedirs(test_config_dir, exist_ok=True)
-        os.environ["XDG_CONFIG_HOME"] = test_config_dir
-        use_neon_audio(init_config_dir)()
-
-        test_config = Configuration()
-        test_config["tts"]["module"] = "neon-tts-plugin-larynx-server"
-        test_config["tts"]["neon-tts-plugin-larynx-server"] = \
-            {"host": os.environ.get("TTS_URL") or "https://larynx.2022.us/"}
-        assert test_config["tts"]["module"] == "neon-tts-plugin-larynx-server"
-
-        # cls.messagebus = NeonBusService(debug=True, daemonic=True)
-        # cls.messagebus.start()
-        cls.bus = FakeBus()
-        cls.bus.connected_event = Event()
-        cls.bus.connected_event.set()
-        cls.audio_service = NeonPlaybackService(audio_config=test_config,
-                                                daemonic=True, bus=cls.bus)
+    @patch("ovos_audio.service.Configuration")
+    def setUpClass(cls, config) -> None:
+        config.return_value = _TEST_CONFIG
+        ready_event = Event()
+
+        def on_ready():
+            ready_event.set()
+
+        cls.audio_service = NeonPlaybackService(daemonic=True, bus=cls.bus,
+                                                ready_hook=on_ready)
+        assert cls.audio_service.config == _TEST_CONFIG
         cls.audio_service.start()
-        # cls.bus = MessageBusClient()
-        # cls.bus.run_in_thread()
-        # if not cls.bus.connected_event.wait(30):
-        #     raise TimeoutError("Bus not connected after 60 seconds")
-        alive = False
-        timeout = time() + 120
-        while not alive and time() < timeout:
-            message = cls.bus.wait_for_response(Message("mycroft.audio.is_ready"))
-            if message:
-                alive = message.data.get("status")
-        if not alive:
-            raise TimeoutError("Speech module not ready after 120 seconds")
+        if not ready_event.wait(30):
+            raise TimeoutError("Audio service not ready")
 
     @classmethod
     def tearDownClass(cls) -> None:
-        super(TestAPIMethods, cls).tearDownClass()
-        # try:
-        #     cls.messagebus.shutdown()
-        # except Exception as e:
-        #     print(e)
         try:
             cls.audio_service.shutdown()
         except Exception as e:
             print(e)
 
     def test_get_tts_no_sentence(self):
         context = {"client": "tester",
                    "ident": "123",
                    "user": "TestRunner"}
-        tts_resp = self.bus.wait_for_response(Message("neon.get_tts", {}, context), context["ident"])
+        tts_resp = self.bus.wait_for_response(Message("neon.get_tts", {},
+                                                      context),
+                                              context["ident"])
         self.assertEqual(tts_resp.context, context)
         self.assertIsInstance(tts_resp.data.get("error"), str)
         self.assertEqual(tts_resp.data["error"], "No text provided.")
 
     def test_get_tts_invalid_type(self):
         context = {"client": "tester",
                    "ident": "1234",
                    "user": "TestRunner"}
-        tts_resp = self.bus.wait_for_response(Message("neon.get_tts", {"text": 123}, context),
+        tts_resp = self.bus.wait_for_response(Message("neon.get_tts",
+                                                      {"text": 123}, context),
                                               context["ident"], timeout=60)
         self.assertEqual(tts_resp.context, context)
-        self.assertTrue(tts_resp.data.get("error").startswith("text is not a str:"))
+        self.assertTrue(tts_resp.data.get("error")
+                        .startswith("text is not a str:"))
 
     def test_get_tts_valid_default(self):
         text = "This is a test"
         context = {"client": "tester",
                    "ident": str(time()),
                    "user": "TestRunner"}
         tts_resp = self.bus.wait_for_response(Message("neon.get_tts",
@@ -168,15 +161,15 @@
                                          {"utterance": "test3"},
                                          {"ident": "test4"})
         self.audio_service.handle_speak(message_no_destination)
         mock_tts.assert_called_with("test3", "test4", False)
 
         # Setup bus API handling
         self.audio_service._playback_timeout = 60
-        msg: Message = None
+        msg = None
 
         def handle_tts(*args, **kwargs):
             nonlocal msg
             msg = dig_for_message()
             ident = msg.data.get('speak_ident') or msg.data.get('ident')
             if ident:
                 self.bus.emit(Message(ident))
```

### Comparing `neon-audio-1.3.3a6/tests/test_objects/__init__.py` & `neon-audio-1.3.3a7/tests/test_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a6/tests/unit_tests.py` & `neon-audio-1.3.3a7/tests/unit_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,37 +36,39 @@
 from threading import Event
 from unittest.mock import Mock, patch
 from click.testing import CliRunner
 from ovos_bus_client import Message
 from ovos_plugin_manager.templates.tts import PlaybackThread
 from ovos_utils.messagebus import FakeBus
 
-from neon_utils.signal_utils import check_for_signal
-
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 from neon_audio.tts import WrappedTTS
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 from test_objects import DummyTTS, DummyTTSValidator
 
 
 class TTSBaseClassTests(unittest.TestCase):
+    lang = "en-us"
+    config = {"key": "val"}
+    test_cache_dir = join(dirname(__file__), "test_cache")
+    test_conf_dir = join(dirname(__file__), "config")
+    bus = FakeBus()
+    bus.connected_event = Event()
+    bus.connected_event.set()
+
     @classmethod
-    def setUpClass(cls) -> None:
-        cls.test_cache_dir = join(dirname(__file__), "test_cache")
-        cls.test_conf_dir = join(dirname(__file__), "config")
+    @patch("ovos_plugin_manager.templates.tts.Configuration")
+    def setUpClass(cls, config) -> None:
+        config.return_value = cls.config  # Explicitly no g2p
         os.makedirs(cls.test_conf_dir, exist_ok=True)
         os.environ["XDG_CACHE_HOME"] = cls.test_cache_dir
-        cls.config = {"key": "val"}
-        cls.lang = "en-us"
+
         cls.tts = WrappedTTS(DummyTTS, cls.lang, cls.config)
-        bus = FakeBus()
-        bus.connected_event = Event()
-        bus.connected_event.set()
-        cls.tts.init(bus)
+        cls.tts.init(cls.bus)
 
     @classmethod
     def tearDownClass(cls) -> None:
         cls.tts.shutdown()
         if os.path.exists(cls.test_cache_dir):
             shutil.rmtree(cls.test_cache_dir)
         if os.path.exists(cls.test_conf_dir):
@@ -115,14 +117,16 @@
 
     def test_preprocess_sentence(self):
         # TODO: Legacy
         sentence = "this is a test"
         self.assertEqual(self.tts._preprocess_sentence(sentence), [sentence])
 
     def test_execute(self):
+        from neon_utils.signal_utils import check_for_signal, init_signal_bus
+        init_signal_bus(self.bus)
         sentence = "testing"
         ident = time()
         default_execute = self.tts._execute
         self.tts._execute = Mock()
         self.tts.execute(sentence, ident)
         self.assertTrue(check_for_signal("isSpeaking"))
         self.tts._execute.assert_called_once_with(sentence, ident, False)
@@ -158,15 +162,17 @@
         self.assertIsNone(self.tts.viseme(""))
 
     def test_validator_valid(self):
         self.assertTrue(self.tts.validator.validate_lang())
         self.assertTrue(self.tts.validator.validate_dependencies())
         self.assertTrue(self.tts.validator.validate_connection())
 
-    def test_validator_invalid(self):
+    @patch("ovos_plugin_manager.templates.tts.Configuration")
+    def test_validator_invalid(self, config):
+        config.return_value = self.config  # Explicitly no g2p
         tts = DummyTTS("es", {})
 
         with self.assertRaises(Exception):
             tts.validator.validate()
 
         tts.shutdown()
```

