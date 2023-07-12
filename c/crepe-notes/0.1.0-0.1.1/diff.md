# Comparing `tmp/crepe_notes-0.1.0-py2.py3-none-any.whl.zip` & `tmp/crepe_notes-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21489 bytes, number of entries: 10
+Zip file size: 22249 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      131 b- defN 22-Sep-07 08:07 crepe_notes/__init__.py
--rw-r--r--  2.0 unx     2300 b- defN 23-Jul-12 07:52 crepe_notes/cli.py
--rw-r--r--  2.0 unx    13921 b- defN 23-Jul-12 07:52 crepe_notes/crepe_notes.py
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4908 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      840 b- defN 23-Jul-12 08:15 crepe_notes-0.1.0.dist-info/RECORD
-10 files, 57582 bytes uncompressed, 20049 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx     2468 b- defN 23-Jul-12 08:55 crepe_notes/cli.py
+-rw-r--r--  2.0 unx    13946 b- defN 23-Jul-12 09:35 crepe_notes/crepe_notes.py
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6474 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      840 b- defN 23-Jul-12 09:53 crepe_notes-0.1.1.dist-info/RECORD
+10 files, 59341 bytes uncompressed, 20809 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: crepe_notes/cli.py
 Comment: 
 
 Filename: crepe_notes/crepe_notes.py
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/AUTHORS.rst
+Filename: crepe_notes-0.1.1.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/LICENSE
+Filename: crepe_notes-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/METADATA
+Filename: crepe_notes-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/WHEEL
+Filename: crepe_notes-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/entry_points.txt
+Filename: crepe_notes-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/top_level.txt
+Filename: crepe_notes-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: crepe_notes-0.1.0.dist-info/RECORD
+Filename: crepe_notes-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## crepe_notes/cli.py

```diff
@@ -15,16 +15,19 @@
 @click.option('--use-smoothing', is_flag=True, default=False, help='Enable smoothing of confidence')
 @click.option('--use-cwd', is_flag=True, default=False, help='If True, write to the cwd of the current command, else write to the parent folder of the f0_path')
 @click.option('--f0', type=click.Path(exists=True))
 @click.option('--save-analysis-files', is_flag=True, default=False, help='Save f0, madmom onsets and amp envelope as files')
 @click.argument('audio_path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.help_option()
 def main(f0, audio_path, output_label, sensitivity, min_duration, min_velocity, disable_splitting, tuning_offset, use_smoothing, use_cwd, save_analysis_files):
-    if f0 is None:
+    default_f0_path = audio_path.with_suffix('.f0.csv')
+    if not default_f0_path.exists() and f0 is None:
         frequency, confidence = run_crepe(audio_path)
+    elif f0 is None:
+        frequency, confidence = parse_f0(default_f0_path)
     else:
         frequency, confidence = parse_f0(f0)
 
         
     """CREPE notes - get midi or discrete notes from the CREPE pitch tracker"""
     click.echo(click.format_filename(audio_path))
     process(frequency, confidence, audio_path, output_label=output_label, sensitivity=sensitivity, use_smoothing=use_smoothing,
```

## crepe_notes/crepe_notes.py

```diff
@@ -85,15 +85,15 @@
             tuning_offset=False,
             detect_amplitude=True,
             save_amp_envelope=False,
             default_sample_rate=44100,
             save_analysis_files=False,):
     
     cached_amp_envelope_path = audio_path.with_suffix(".amp_envelope.npz")
-    sr, y, filtered_amp_envelope, detect_amplitude = load_audio(audio_path, cached_amp_envelope_path, default_sample_rate, detect_amplitude, save_amp_envelope)
+    sr, y, filtered_amp_envelope, detect_amplitude = load_audio(audio_path, cached_amp_envelope_path, default_sample_rate, detect_amplitude, (save_analysis_files or save_amp_envelope))
 
     if use_cwd:
         # write to location that the bin was run from
         output_filename = audio_path.stem
     else:
         # write to same folder as the orignal audio file
         output_filename = str(audio_path.parent) + "/" + audio_path.stem
```

## Comparing `crepe_notes-0.1.0.dist-info/LICENSE` & `crepe_notes-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `crepe_notes-0.1.0.dist-info/METADATA` & `crepe_notes-0.1.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepe-notes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Post-processing for CREPE to turn f0 pitch estimates into discrete notes e.g. MIDI
 Home-page: https://github.com/xavriley/crepe_notes
 Author: Xavier Riley
 Author-email: xavriley@hotmail.com
 License: GNU General Public License v3.0 license
 Keywords: crepe_notes
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: Click (>=7.0)
 Requires-Dist: librosa (>=0.7.2)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: madmom
 Requires-Dist: pretty-midi
+Requires-Dist: crepe
 
 CREPE notes
 ===========
 
 
 <!-- .. image:: https://img.shields.io/pypi/v/crepe_notes.svg -->
 <!--         :target: https://pypi.python.org/pypi/crepe_notes -->
@@ -39,43 +40,66 @@
 <!--         :target: https://crepe-notes.readthedocs.io/en/latest/?version=latest -->
 <!--         :alt: Documentation Status -->
 
 Post-processing for CREPE to turn f0 pitch estimates into discrete notes (MIDI)
 
 https://github.com/xavriley/crepe_notes/assets/369527/4cc895f5-9bfe-47af-809d-0152933dc4c9
 
-
-* Free software: mainly MIT licensed, some dependencies (madmom) have restrictions on commercial use
-* Documentation: https://crepe-notes.readthedocs.io.
+[Demo video for pypi users also available here](https://www.youtube.com/watch?v=vFvbedBgLKg)
   
+Features
+--------
+
+* outputs midi notes for monophonic audio
+* include MIDI velocity information
+* includes options to filter notes that are too quiet or too short
+
 Installation
 ------------
 
 ```
-pip install crepe_notes
+pip install crepe-notes
 ```
 
+> **Warning**
+> Python 3.10 and above will fail to run, due to [this long running issue](https://github.com/CPJKU/madmom/issues/509) with madmom.
+>
+> As a workaround, please run `!pip install -e git+https://github.com/CPJKU/madmom#egg=madmom` after installation
+
 Basic Usage
 -----------
 
 ```
 crepe_notes [path_to_original_audio]
 ```
 
 A '.mid' file will be created in the location of the audio file with the name `[audio_file_stem].transcription.mid`.
 
 For additional options check out `crepe_notes --help`.
 
-Features
---------
+## Min duration, min velocity and sensitivity
 
-* outputs midi notes for monophonic audio
-* include MIDI velocity information
-* includes options to filter notes that are too quiet or too short
+These are the three params you may need to tweak to get optimal results.
+
+* `--min-duration` is specified in seconds (e.g. `0.03` is `30ms`). For fast, virtuosic music this is a reasonable default but for things like vocals and double bass lines a longer min duration (`50ms` or higher) may reduce the number of errors in your transcription.
+
+* `--min-velocity` is expressed as in MIDI e.g. `0 - 127`. The default is `6` which removes any notes with velocities at or below that value, but you may find recordings with a higher noise floor benefit from a higher threshold.
+
+* `--sensitivity` relates to the peak picking threshold used on the combined signal (see paper for details) and defaults to `0.001`. If the source material has an unstable pitch profile which results in a lot of short notes either side of a longer target note, increasing the sensitivity to `0.002` may help. 
+
+
+## Caching data files
+
+If you are running `crepe_notes` over an entire dataset, we recommend using the `--save-analysis-files` flag. This will write the following results:
+
+* crepe to `[audio_file_stem].f0.csv`.
+* madmom onset activations to `[audio_file_stem].onsets.npz`
+* amplitude envelope calculations to `[audio_file_stem].amp_envelope.npz`
 
+This will speed up run times at the expense of some disk space.
 
 About
 -----
 
 This repo is the code to accompany the following paper:
 
 > X. Riley and S. Dixon, “CREPE Notes: A new method for segmenting pitch contours into discrete notes,” in Proceedings of the 20th Sound and Music Computing Conference, Stockholm, Sweden, 2023, pp. 1–5.
```

## Comparing `crepe_notes-0.1.0.dist-info/RECORD` & `crepe_notes-0.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 crepe_notes/__init__.py,sha256=OwyCKpDg-oS8m3s6zEtJbkZMhNJsyZ2kiR1LLXm76zY,131
-crepe_notes/cli.py,sha256=ALHs9rzkgpxRiVM_nAv-vsA6dBT_FFd2-fF32AATa2U,2300
-crepe_notes/crepe_notes.py,sha256=juRVK7xV2Ew9oA2DLoqGTbQW5K9hrgf4BiqYnmj6t3Y,13921
-crepe_notes-0.1.0.dist-info/AUTHORS.rst,sha256=g6Ze1dzuTB01AJuUPwpwqgysGxhHP78ohHVA4OElhjY,158
-crepe_notes-0.1.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-crepe_notes-0.1.0.dist-info/METADATA,sha256=e_hIW9czvAne-ibt3chetctHv36fiLdSA5EdTuiSJSc,4908
-crepe_notes-0.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-crepe_notes-0.1.0.dist-info/entry_points.txt,sha256=iKgAXksnyz0yJN7n6Csp0UvSQmYNWb-FPIGrJNP-LYY,53
-crepe_notes-0.1.0.dist-info/top_level.txt,sha256=NdjHi-isyyfnSPur473qW-3ZGPbrL8m7o2FZVNHLyoc,12
-crepe_notes-0.1.0.dist-info/RECORD,,
+crepe_notes/cli.py,sha256=Y3uXMkMp0CdZ-yVqdIWphGqGPz7zXsIoYMwOlbNEdgg,2468
+crepe_notes/crepe_notes.py,sha256=htiO5c7nSxikSgBZgvGQkBEzdcnV-H-mAEOm4J7foGE,13946
+crepe_notes-0.1.1.dist-info/AUTHORS.rst,sha256=g6Ze1dzuTB01AJuUPwpwqgysGxhHP78ohHVA4OElhjY,158
+crepe_notes-0.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+crepe_notes-0.1.1.dist-info/METADATA,sha256=BtKFerm_NOmrbHwNVr2GsAY07codDuIaPKA1RnUr58Q,6474
+crepe_notes-0.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+crepe_notes-0.1.1.dist-info/entry_points.txt,sha256=iKgAXksnyz0yJN7n6Csp0UvSQmYNWb-FPIGrJNP-LYY,53
+crepe_notes-0.1.1.dist-info/top_level.txt,sha256=NdjHi-isyyfnSPur473qW-3ZGPbrL8m7o2FZVNHLyoc,12
+crepe_notes-0.1.1.dist-info/RECORD,,
```

