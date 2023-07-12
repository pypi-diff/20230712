# Comparing `tmp/openlrc-0.1.5.tar.gz` & `tmp/openlrc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.1.5.tar", max compression
+gzip compressed data, was "openlrc-0.2.0.tar", max compression
```

## Comparing `openlrc-0.1.5.tar` & `openlrc-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.5/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.5/openlrc/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.1.5/openlrc/chatbot.py
--rw-r--r--   0        0        0     2704 2023-06-27 13:49:50.307093 openlrc-0.1.5/openlrc/context.py
--rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.1.5/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.5/openlrc/logger.py
--rw-r--r--   0        0        0    13967 2023-07-06 16:13:15.634083 openlrc-0.1.5/openlrc/openlrc.py
--rw-r--r--   0        0        0     5204 2023-07-03 18:14:57.916841 openlrc-0.1.5/openlrc/opt.py
--rw-r--r--   0        0        0     7664 2023-06-27 08:09:12.518292 openlrc-0.1.5/openlrc/prompter.py
--rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.1.5/openlrc/subtitle.py
--rw-r--r--   0        0        0    15382 2023-07-06 13:45:34.304340 openlrc-0.1.5/openlrc/transcribe.py
--rw-r--r--   0        0        0     5726 2023-06-27 18:43:39.771392 openlrc-0.1.5/openlrc/translate.py
--rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.1.5/openlrc/utils.py
--rw-r--r--   0        0        0     1718 2023-07-07 02:24:49.837818 openlrc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5606 2023-07-06 14:38:43.653605 openlrc-0.1.5/README.md
--rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 openlrc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.2.0/openlrc/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.2.0/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2761 2023-07-12 18:58:48.074505 openlrc-0.2.0/openlrc/context.py
+-rw-r--r--   0        0        0     1424 2023-07-12 19:00:10.406166 openlrc-0.2.0/openlrc/defaults.py
+-rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.2.0/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.2.0/openlrc/logger.py
+-rw-r--r--   0        0        0    12901 2023-07-12 18:58:48.075680 openlrc-0.2.0/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5165 2023-07-12 18:58:48.076238 openlrc-0.2.0/openlrc/opt.py
+-rw-r--r--   0        0        0     7702 2023-07-12 18:58:48.076743 openlrc-0.2.0/openlrc/prompter.py
+-rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.2.0/openlrc/subtitle.py
+-rw-r--r--   0        0        0     6729 2023-07-12 18:58:48.076743 openlrc-0.2.0/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5735 2023-07-12 18:58:48.077748 openlrc-0.2.0/openlrc/translate.py
+-rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.2.0/openlrc/utils.py
+-rw-r--r--   0        0        0     1654 2023-07-12 19:02:49.168288 openlrc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5572 2023-07-12 19:02:30.593756 openlrc-0.2.0/README.md
+-rw-r--r--   0        0        0     7019 1970-01-01 00:00:00.000000 openlrc-0.2.0/PKG-INFO
```

### Comparing `openlrc-0.1.5/LICENSE` & `openlrc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/openlrc/chatbot.py` & `openlrc-0.2.0/openlrc/chatbot.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/openlrc/context.py` & `openlrc-0.2.0/openlrc/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 import yaml
 
 from openlrc.logger import logger
 
 
 class Context:
-    def __init__(self, background='', synopsis_map=None, audio_type='Anime', config_path=None):
+    def __init__(self, background='', description_map=None, audio_type='Anime', config_path=None):
         """
         Context(optional) for translation.
 
         :param background: Providing background information for establishing context for the translation.
-        :param synopsis_map: {"name(without extension)": "synopsis", ...}
+        :param description_map: {"name(without extension)": "description", ...}
         :param audio_type: Audio type, default to Anime.
         :param config_path: Path to config file.
         """
         self.config_path = None
         self.background = background
         self.audio_type = audio_type
-        self.synopsis_map = synopsis_map if synopsis_map else dict()
+        self.description_map = description_map if description_map else dict()
 
         # if config_path exist, load yaml file
         if config_path:
             config_path = Path(config_path)
             if config_path.exists():
                 self.load_config(config_path)
             else:
@@ -42,35 +42,35 @@
 
         if config.get('background'):
             self.background = config['background']
 
         if config.get('audio_type'):
             self.audio_type = config['audio_type']
 
-        if config.get('synopsis_map'):
-            self.synopsis_map = config['synopsis_map']
+        if config.get('description_map'):
+            self.description_map = config['description_map']
 
         self.config_path = config_path
 
     def save_config(self):
         with open(self.config_path, 'w') as f:
             yaml.dump({
                 'background': self.background,
                 'audio_type': self.audio_type,
-                'synopsis_map': self.synopsis_map,
+                'description_map': self.description_map,
             }, f)
 
-    def get_synopsis(self, audio_name):
+    def get_description(self, audio_name):
         value = ''
-        if self.synopsis_map:
-            matches = get_close_matches(audio_name, self.synopsis_map.keys())
+        if self.description_map:
+            matches = get_close_matches(audio_name, self.description_map.keys())
             if matches:
                 key = matches[0]
-                value = self.synopsis_map.get(key)
-                logger.info(f'Found synopsis map: {key} -> {value}')
+                value = self.description_map.get(key)
+                logger.info(f'Found description map: {key} -> {value}')
             else:
-                logger.info(f'No synopsis map for {audio_name} found.')
+                logger.info(f'No description map for {audio_name} found.')
 
         return value
 
     def __str__(self):
-        return f'Context(background={self.background}, audio_type={self.audio_type}, synopsis_map={self.synopsis_map})'
+        return f'Context(background={self.background}, audio_type={self.audio_type}, description_map={self.description_map})'
```

### Comparing `openlrc-0.1.5/openlrc/exceptions.py` & `openlrc-0.2.0/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/openlrc/logger.py` & `openlrc-0.2.0/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/openlrc/openlrc.py` & `openlrc-0.2.0/openlrc/openlrc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,93 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
 import concurrent.futures
 import json
-from concurrent.futures import Future
 from pathlib import Path
 from pprint import pformat
 from queue import Queue
 from threading import Lock
 from typing import List
 
+from faster_whisper.transcribe import Segment
+
 from openlrc.context import Context
+from openlrc.defaults import default_asr_options, default_vad_options
 from openlrc.logger import logger
 from openlrc.opt import SubtitleOptimizer
 from openlrc.subtitle import Subtitle
 from openlrc.transcribe import Transcriber
 from openlrc.translate import GPTTranslator
 from openlrc.utils import Timer, extend_filename, get_audio_duration, format_timestamp, extract_audio, \
     get_file_type
 
 
 class LRCer:
+    """
+     :param model_name: Name of whisper model (tiny, tiny.en, base, base.en, small, small.en, medium,
+                    medium.en, large-v1, or large-v2) When a size is configured, the converted model is downloaded
+                    from the Hugging Face Hub.
+                    Default: ``large-v2``
+    :param compute_type: The type of computation to use. Can be ``int8``, ``int8_float16``, ``int16``,
+                    ``float16`` or ``float32``.
+                    Default: ``float16``
+    :param fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
+    :param consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
+    :param asr_options: parameters for whisper model.
+    :param vad_options: parameters for VAD model.
+    """
+
     def __init__(self, model_name='large-v2', compute_type='float16', fee_limit=0.1, consumer_thread=11,
                  asr_options=None, vad_options=None):
-        """
-        :param model_name: Name of whisper model (tiny, tiny.en, base, base.en, small, small.en, medium,
-                        medium.en, large-v1, or large-v2) When a size is configured, the converted model is downloaded
-                        from the Hugging Face Hub.
-                        Default: ``large-v2``
-        :param compute_type: The type of computation to use. Can be ``int8``, ``int8_float16``, ``int16``,
-                        ``float16`` or ``float32``.
-                        Default: ``float16``
-        :param fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
-        :param consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
-        :param asr_options: parameters for whisper model.
-        :param vad_options: parameters for VAD model.
-        """
-
-        self.transcriber = Transcriber(model_name=model_name, compute_type=compute_type)
         self.fee_limit = fee_limit
         self.api_fee = 0  # Can be updated in different thread, operation should be thread-safe
         self.from_video = set()
         self.context: Context = Context()
 
         self._lock = Lock()
         self.exception = None
         self.consumer_thread = consumer_thread
 
         # Default Automatic Speech Recognition (ASR) options
-        self.asr_options = {
-            "beam_size": 5,
-            "best_of": 5,
-            "patience": 1,
-            "length_penalty": 1,
-            "temperatures": [0.0, 0.2, 0.4, 0.6, 0.8, 1.0],
-            "compression_ratio_threshold": 2.4,
-            "log_prob_threshold": -1.0,
-            "no_speech_threshold": 0.6,
-            "condition_on_previous_text": True,
-            "initial_prompt": None,
-            "prefix": None,
-            "suppress_blank": True,
-            "suppress_tokens": [-1],
-            "without_timestamps": True,
-            "max_initial_timestamp": 0.0,
-            "word_timestamps": False,
-            "prepend_punctuations": "\"'“¿([{-",
-            "append_punctuations": "\"'.。,，!！?？:：”)]}、",
-            "suppress_numerals": False,
-        }
+        self.asr_options = default_asr_options
 
-        # Parameters for VAD (see pyannote.audio), reduce them if speech is not being detected
-        self.vad_options = {
-            "vad_onset": 0.500,
-            "vad_offset": 0.363
-        }
+        # Parameters for VAD (see faster_whisper.vad.VadOptions), tune them if speech is not being detected
+        self.vad_options = default_vad_options
 
         if asr_options:
             self.asr_options.update(asr_options)
 
         if vad_options:
             self.vad_options.update(vad_options)
 
+        self.transcriber = Transcriber(model_name=model_name, compute_type=compute_type,
+                                       asr_options=self.asr_options, vad_options=self.vad_options)
+
     def transcription_producer(self, transcription_queue, audio_paths, src_lang):
         """
         Sequential Producer.
         """
         for audio_path in audio_paths:
             transcribed_path = extend_filename(audio_path, '_transcribed').with_suffix('.json')
             if not transcribed_path.exists():
                 with Timer('Transcription process'):
                     logger.info(
                         f'Audio length: {audio_path}: {format_timestamp(get_audio_duration(audio_path), fmt="srt")}')
-                    segments, info = self.transcriber.transcribe(audio_path, batch_size=4, language=src_lang,
-                                                                 asr_options=self.asr_options,
-                                                                 vad_options=self.vad_options)
+                    segments, info = self.transcriber.transcribe(audio_path, language=src_lang)
                     logger.info(f'Detected language: {info.language}')
 
-                    # From generator to list with progress bar shown
-                    seg_list = segments['sentences']  # [{'text': ..., 'start': ..., 'end':...}, ...]
-                    logger.debug(f'Transcribed fast-whisper Segments: {seg_list}')
+                    # [Segment(start, end, text, words=[Word(start, end, word, probability)])]
 
                 # Save the transcribed json
-                self.to_json(seg_list, name=transcribed_path, lang=info.language)  # xxx_transcribed.json
+                self.to_json(segments, name=transcribed_path, lang=info.language)  # xxx_transcribed.json
             else:
                 logger.info(f'Found transcribed json file: {transcribed_path}')
             transcription_queue.put(transcribed_path)
-            logger.info(f'Put transcription: {transcribed_path}')
+            # logger.info(f'Put transcription: {transcribed_path}')
 
         transcription_queue.put(None)
         logger.info('Transcription producer finished.')
 
     def transcription_consumer(self, transcription_queue, target_lang, prompter, skip_trans):
         """
         Parallel Consumer.
@@ -155,30 +132,30 @@
 
             final_subtitle.to_lrc()
             if audio_name in self.from_video:
                 final_subtitle.to_srt()
             logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
     def _translate(self, audio_name, prompter, target_lang, transcribed_opt_sub, translated_path):
-        json_filename = Path(translated_path.parent / audio_name).with_suffix('.json')
+        json_filename = Path(translated_path.parent / (audio_name + '.json'))
         compare_path = Path(translated_path.parent, f'{audio_name}_compare.json')
         if not translated_path.exists():
             if not compare_path.exists():
                 # Translate the transcribed json
                 translator = GPTTranslator(prompter=prompter, fee_limit=self.fee_limit)
                 context = self.context
 
                 target_texts = translator.translate(
                     transcribed_opt_sub.texts,
                     src_lang=transcribed_opt_sub.lang,
                     target_lang=target_lang,
                     title=audio_name,
                     audio_type=context.audio_type,
                     background=context.background,
-                    synopsis=context.get_synopsis(audio_name),
+                    description=context.get_description(audio_name),
                     compare_path=compare_path
                 )
 
                 with self._lock:
                     self.api_fee += translator.api_fee  # Ensure thread-safe
             else:
                 logger.info(f'Found compare json file: {compare_path}')
@@ -240,39 +217,39 @@
                 logger.info(f'Default context config not found: {self.context}, using default context.')
 
         transcription_queue = Queue()
 
         with Timer('Transcription (Producer) and Translation (Consumer) process'):
             consumer = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Consumer') \
                 .submit(self.transcription_consumer, transcription_queue, target_lang, prompter, skip_trans)
-            producer: Future = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Producer') \
+            producer = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Producer') \
                 .submit(self.transcription_producer, transcription_queue, audio_paths, src_lang)
 
             producer.result()
             consumer.result()
 
             if self.exception:
                 # traceback.print_exception(type(self.exception), self.exception, self.exception.__traceback__)
                 raise self.exception
 
         logger.info(f'Totally used API fee: {self.api_fee:.4f} USD')
 
     @staticmethod
-    def to_json(segments, name, lang):
+    def to_json(segments: List[Segment], name, lang):
         result = {
             'generator': 'LRC generated by https://github.com/zh-plus/Open-Lyrics',
             'language': lang,
             'segments': []
         }
 
         for segment in segments:
             result['segments'].append({
-                'start': segment["start"],
-                'end': segment["end"],
-                'text': segment["text"]
+                'start': segment.start,
+                'end': segment.end,
+                'text': segment.text
             })
 
         with open(name, 'w', encoding='utf-8') as f:
             json.dump(result, f, ensure_ascii=False, indent=4)
 
         logger.info(f'File saved to {name}')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openlrc-0.1.5/openlrc/opt.py` & `openlrc-0.2.0/openlrc/opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,31 +54,31 @@
         for i, element, in enumerate(self.subtitle.segments):
             if i == 0 or element.duration >= threshold:
                 if merged_element:
                     if merged_element.duration < 1:
                         # If the merged elements is still too small, find the smaller element nearby and merge it
                         if new_elements[-1].duration > element.duration:
                             # merge to the next
-                            element.text = merged_element.text + ' ' + element.text
+                            element.text = merged_element.text + element.text
                             element.start = merged_element.start
                         else:
                             # merge to the last
-                            new_elements[-1].text += ' ' + merged_element.text
+                            new_elements[-1].text += merged_element.text
                             new_elements[-1].end = merged_element.end
                     else:
                         new_elements.append(merged_element)
                     new_elements.append(element)
                     merged_element = None
                 else:
                     new_elements.append(element)
             else:
                 if not merged_element:
                     merged_element = element
                 else:
-                    merged_element.text += ' ' + element.text
+                    merged_element.text += element.text
                     merged_element.end = element.end
 
         self.subtitle.segments = new_elements
 
     def merge_repeat(self):
         """
         Merge the same pattern in one lyric.
@@ -103,15 +103,15 @@
 
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
             if len(element.text) > threshold and len(element.text) / len(set(element.text)) > 3.0:
                 # text length larger than threshold and text density is larger than 3.0
                 logger.warning(f'Cut long text: {element.text}\nInto: {element.text[:keep]}...')
-                new_elements[i].text = element.text[:keep] + f'(Cut to {keep})'
+                new_elements[i].text = element.text[:keep]
 
         self.subtitle.segments = new_elements
 
     def traditional2mandarin(self):
         new_elements = self.subtitle.segments
 
         for i, element in enumerate(new_elements):
```

### Comparing `openlrc-0.1.5/openlrc/prompter.py` & `openlrc-0.2.0/openlrc/prompter.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from openlrc.logger import logger
 
 # instruction prompt modified from https://github.com/machinewrapped/gpt-subtrans
 base_instruction = f'''You are a translator, your task is to accurately revise and translate subtitles into a target language.
 The input are transcribed from audio, so there may be errors in the transcription. Please correct any errors you find in the sentences first, based on their context. Then translate them to target language according to the revised sentences.
 The user will provide a chunk of lines, you should respond with an accurate, concise, and natural-sounding translation for the dialogue. 
-The user may provide additional context, such as background, synopsis or title of the film, a summary of the current scene, or a list of character names. Use this information to improve the quality of your translation.
+The user may provide additional context, such as background, description or title of the source material, a summary of the current scene, or a list of character names. Use this information to improve the quality of your translation.
 Your response will be processed by an automated system, so it is imperative that you adhere to the required output format.
 
 Example input (Japanese to Chinese):
 
 #200
 Original>
 変わりゆく時代において、
@@ -69,15 +69,15 @@
 
 Please ensure that each line of dialogue remains distinct in the  translation. Merging lines together can lead to timing problems during playback.
 
 At the end of each set of translations, include a one or two line synopsis of the input text in a <summary/> tag, for example:
 <summary>John and Sarah discuss their plan to locate a suspect, deducing that he is likely in the uptown area.</summary>
 Remember to end this tag with ``</summary>``.
 
-Use the available information to add a short synopsis of the current scene in a <scene/> tag, for example:
+Use the available information to add a short description of the current scene in a <scene/> tag, for example:
 <scene>John and Sarah are in their office analyzing data and planning their next steps. They deduce that the suspect is probably in the uptown area and decide to start their search there.</scene>
 Remember to end this tag with ``</scene>``.
 
 Use the target language when writing content for the <summary/> and <scene/> tags. 
 Ensure that the summary and scene are concise, containing less than 100 words.
 You need to update your summary and scene with the new information you have.
 Do not guess or improvise if the context is unclear, just summarise the dialogue.
@@ -103,29 +103,29 @@
         raise NotImplementedError()
 
     def check_format(self, messages, output_str):
         raise NotImplementedError()
 
 
 class BaseTranslatePrompter(TranslatePrompter):
-    def __init__(self, src_lang, target_lang, audio_type=None, title='', background='', synopsis=''):
+    def __init__(self, src_lang, target_lang, audio_type=None, title='', background='', description=''):
         self.src_lang = src_lang
         self.target_lang = target_lang
         self.src_lang_display = Language.get(src_lang).display_name('en')
         self.target_lang_display = Language.get(target_lang).display_name('en')
         self.lan_detector = LanguageDetectorBuilder.from_all_languages().build()
 
         self.audio_type = audio_type
         self.title = title
         self.background = background
-        self.synopsis = synopsis
+        self.description = description
         self.user_prompt = f'''
 {f"<title>{self.title}</title>" if self.title else ""}
 {f"<background>{self.background}</background>" if self.background else ""}
-{f"<synopsis>{self.synopsis}</synopsis>" if self.synopsis else ""}
+{f"<description>{self.description}</description>" if self.description else ""}
 <context>
 <scene>{{scene}}</scene>
 <chunk> {{summaries_str}} </chunk>
 </context>
 <chunk_id> Scene 1 Chunk {{chunk_num}} <chunk_id>
 
 Please translate these subtitles for {self.audio_type}{f" named {self.title}" if self.title else ""} from {self.src_lang_display} to {self.target_lang_display}.\n
```

### Comparing `openlrc-0.1.5/openlrc/subtitle.py` & `openlrc-0.2.0/openlrc/subtitle.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/openlrc/translate.py` & `openlrc-0.2.0/openlrc/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
 
             return summary.strip(), scene.strip(), [t.strip() for t in translation]
 
         except Exception as e:
             logger.error(f'Failed to extract contents from response: {content}')
             raise e
 
-    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', background='', synopsis='',
+    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', background='', description='',
                   compare_path='test_intermediate.json'):
         prompter: BaseTranslatePrompter = prompter_map[self.prompter](
-            src_lang, target_lang, audio_type, title=title, background=background, synopsis=synopsis)
+            src_lang, target_lang, audio_type, title=title, background=background, description=description)
         translate_bot = GPTBot(fee_limit=self.fee_limit)
         translate_bot.update(temperature=0.7)
 
         chunks = self.make_chunks(texts, chunk_size=self.chunk_size)
         logger.info(f'Translating {title}: {len(chunks)} chunks, {len(texts)} lines in total.')
 
         # Start chunk-by-chunk translation
```

### Comparing `openlrc-0.1.5/openlrc/utils.py` & `openlrc-0.2.0/openlrc/utils.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.5/README.md` & `openlrc-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. Install [PyTorch](https://pytorch.org/get-started/locally/):
    ```shell
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
    ```
 
-4. Install [whisperx](https://github.com/m-bain/whisperX) and (Recommended) the
-   latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
+4. Install latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
    ```shell
    pip install git+https://github.com/guillaumekln/faster-whisper
-   pip install git+https://github.com/m-bain/whisperx.git
    ```
 
 5. (Optional) If you want to process videos, install [ffmpeg](https://ffmpeg.org/download.html) and add `bin` directory
    to your `PATH`.
 
 6. This project can be installed from PyPI:
 
@@ -65,39 +63,43 @@
 # Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
 
 # To skip translation process
 lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
+
+# Change asr_options or vad_options, check openlrc.defaults for details
+vad_options = {"threshold": 0.1}
+lrcer = LRCer(vad_options=vad_options)
+lrcer.run('./data/test.mp3', target_lang='zh-cn')
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
 
 ```yaml
 background: "This is a multi-line background.
 This is a basic example."
 audio_type: Movie
-synopsis_map: {
+description_map: {
   movie_name1 (without extension): "This
-  is a multi-line synopsis for movie1.",
+  is a multi-line description for movie1.",
   movie_name2 (without extension): "This
-  is a multi-line synopsis for movie2.",
-  movie_name3 (without extension): "This is a single-line synopsis for movie 3.",
+  is a multi-line description for movie2.",
+  movie_name3 (without extension): "This is a single-line description for movie 3.",
 }
 ```
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
-- [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
 - [x] [Feature] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
 - [x] [Quality] Improve batched translation/polish prompt according
   to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
 - [x] [Feature] Input video support.
 - [X] [Feature] Multiple output format support.
```

### Comparing `openlrc-0.1.5/PKG-INFO` & `openlrc-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.1.5
+Version: 0.2.0
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -56,19 +56,17 @@
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. Install [PyTorch](https://pytorch.org/get-started/locally/):
    ```shell
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
    ```
 
-4. Install [whisperx](https://github.com/m-bain/whisperX) and (Recommended) the
-   latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
+4. Install latest [fast-whisper](https://github.com/guillaumekln/faster-whisper)
    ```shell
    pip install git+https://github.com/guillaumekln/faster-whisper
-   pip install git+https://github.com/m-bain/whisperx.git
    ```
 
 5. (Optional) If you want to process videos, install [ffmpeg](https://ffmpeg.org/download.html) and add `bin` directory
    to your `PATH`.
 
 6. This project can be installed from PyPI:
 
@@ -104,39 +102,43 @@
 # Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
 
 # To skip translation process
 lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
+
+# Change asr_options or vad_options, check openlrc.defaults for details
+vad_options = {"threshold": 0.1}
+lrcer = LRCer(vad_options=vad_options)
+lrcer.run('./data/test.mp3', target_lang='zh-cn')
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
 
 ```yaml
 background: "This is a multi-line background.
 This is a basic example."
 audio_type: Movie
-synopsis_map: {
+description_map: {
   movie_name1 (without extension): "This
-  is a multi-line synopsis for movie1.",
+  is a multi-line description for movie1.",
   movie_name2 (without extension): "This
-  is a multi-line synopsis for movie2.",
-  movie_name3 (without extension): "This is a single-line synopsis for movie 3.",
+  is a multi-line description for movie2.",
+  movie_name3 (without extension): "This is a single-line description for movie 3.",
 }
 ```
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
-- [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
 - [x] [Feature] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
 - [x] [Quality] Improve batched translation/polish prompt according
   to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
 - [x] [Feature] Input video support.
 - [X] [Feature] Multiple output format support.
```

