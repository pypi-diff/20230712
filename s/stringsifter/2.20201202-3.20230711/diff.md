# Comparing `tmp/stringsifter-2.20201202.tar.gz` & `tmp/stringsifter-3.20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stringsifter-2.20201202.tar", last modified: Wed Dec  2 17:23:15 2020, max compression
+gzip compressed data, was "stringsifter-3.20230711.tar", max compression
```

## Comparing `stringsifter-2.20201202.tar` & `stringsifter-3.20230711.tar`

### file list

```diff
@@ -1,38 +1,22 @@
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.950141 stringsifter-2.20201202/
--rwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)    11368 2019-11-07 17:56:05.000000 stringsifter-2.20201202/LICENSE
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      434 2019-11-07 17:56:05.000000 stringsifter-2.20201202/MANIFEST.in
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      589 2020-12-02 17:23:15.950141 stringsifter-2.20201202/PKG-INFO
--rwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)     7678 2020-11-24 15:58:57.000000 stringsifter-2.20201202/README.md
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.946140 stringsifter-2.20201202/docker/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      202 2020-12-02 17:21:58.000000 stringsifter-2.20201202/docker/Dockerfile
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.946140 stringsifter-2.20201202/misc/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)    33376 2019-11-07 17:56:05.000000 stringsifter-2.20201202/misc/stringsifter-flat-dark.png
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)       38 2020-12-02 17:23:15.950141 stringsifter-2.20201202/setup.cfg
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)     2622 2020-12-02 17:21:58.000000 stringsifter-2.20201202/setup.py
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.946140 stringsifter-2.20201202/stringsifter/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)     1640 2020-11-24 14:46:06.000000 stringsifter-2.20201202/stringsifter/flarestrings.py
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.950141 stringsifter-2.20201202/stringsifter/lib/
--rwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2019-11-07 17:56:05.000000 stringsifter-2.20201202/stringsifter/lib/__init__.py
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)  1153393 2019-11-07 17:56:05.000000 stringsifter-2.20201202/stringsifter/lib/constants.json
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)   938013 2019-11-07 17:56:05.000000 stringsifter-2.20201202/stringsifter/lib/lid.176.ftz
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)    53353 2020-12-02 17:21:58.000000 stringsifter-2.20201202/stringsifter/lib/markov.pkl
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)     1158 2019-11-07 17:56:05.000000 stringsifter-2.20201202/stringsifter/lib/stats.py
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      431 2019-11-07 17:56:05.000000 stringsifter-2.20201202/stringsifter/lib/util.py
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.950141 stringsifter-2.20201202/stringsifter/model/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)   290829 2020-12-02 17:21:58.000000 stringsifter-2.20201202/stringsifter/model/featurizer.pkl
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)   459050 2020-12-02 17:21:58.000000 stringsifter-2.20201202/stringsifter/model/ranker.pkl
--rwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)    28682 2020-12-02 17:09:02.000000 stringsifter-2.20201202/stringsifter/preprocess.py
--rwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)     5823 2020-12-02 17:09:02.000000 stringsifter-2.20201202/stringsifter/rank_strings.py
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)       27 2020-12-02 17:22:08.000000 stringsifter-2.20201202/stringsifter/version.py
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.946140 stringsifter-2.20201202/stringsifter.egg-info/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      589 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/PKG-INFO
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      741 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/SOURCES.txt
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)        1 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/dependency_links.txt
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)      114 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/entry_points.txt
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)       77 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/requires.txt
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)       30 2020-12-02 17:23:15.000000 stringsifter-2.20201202/stringsifter.egg-info/top_level.txt
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.946140 stringsifter-2.20201202/tests/
-drwxr-xr-x   0 ewalsh    (1000) ewalsh    (1000)        0 2020-12-02 17:23:15.950141 stringsifter-2.20201202/tests/fixtures/
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)     1062 2019-11-07 17:56:05.000000 stringsifter-2.20201202/tests/fixtures/strings_output1
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)    11733 2019-11-07 17:56:05.000000 stringsifter-2.20201202/tests/fixtures/strings_output2
--rw-r--r--   0 ewalsh    (1000) ewalsh    (1000)        0 2019-11-07 17:56:05.000000 stringsifter-2.20201202/tests/fixtures/strings_output3
+-rw-r--r--   0        0        0    11368 2023-07-12 02:17:40.550946 stringsifter-3.20230711/LICENSE
+-rw-r--r--   0        0        0     7531 2023-07-12 02:17:40.550946 stringsifter-3.20230711/README.md
+-rw-r--r--   0        0        0    33376 2023-06-30 21:35:42.871040 stringsifter-3.20230711/misc/stringsifter-flat-dark.png
+-rw-r--r--   0        0        0     1280 2023-07-12 02:17:40.550946 stringsifter-3.20230711/pyproject.toml
+-rw-r--r--   0        0        0     1640 2023-06-30 21:35:42.871040 stringsifter-3.20230711/stringsifter/flarestrings.py
+-rw-r--r--   0        0        0        0 2023-07-12 02:17:40.550946 stringsifter-3.20230711/stringsifter/lib/__init__.py
+-rw-r--r--   0        0        0  1153393 2023-06-30 21:35:42.891042 stringsifter-3.20230711/stringsifter/lib/constants.json
+-rw-r--r--   0        0        0   938013 2023-06-30 21:35:42.903043 stringsifter-3.20230711/stringsifter/lib/lid.176.ftz
+-rw-r--r--   0        0        0    53353 2023-06-30 21:35:42.903043 stringsifter-3.20230711/stringsifter/lib/markov.pkl
+-rw-r--r--   0        0        0     1158 2023-06-30 21:35:42.903043 stringsifter-3.20230711/stringsifter/lib/stats.py
+-rw-r--r--   0        0        0      431 2023-06-30 21:35:42.903043 stringsifter-3.20230711/stringsifter/lib/util.py
+-rw-r--r--   0        0        0   312560 2023-07-12 02:17:40.554946 stringsifter-3.20230711/stringsifter/model/featurizer.pkl
+-rw-r--r--   0        0        0   498381 2023-07-12 02:17:40.554946 stringsifter-3.20230711/stringsifter/model/ranker.pkl
+-rw-r--r--   0        0        0    28682 2023-07-12 02:17:40.558947 stringsifter-3.20230711/stringsifter/preprocess.py
+-rw-r--r--   0        0        0     5823 2023-07-12 02:17:40.558947 stringsifter-3.20230711/stringsifter/rank_strings.py
+-rw-r--r--   0        0        0       27 2023-07-12 02:17:40.558947 stringsifter-3.20230711/stringsifter/version.py
+-rw-r--r--   0        0        0      211 2023-06-30 21:35:42.907044 stringsifter-3.20230711/tests/conftest.py
+-rw-r--r--   0        0        0     1062 2023-06-30 21:35:42.907044 stringsifter-3.20230711/tests/fixtures/strings_output1
+-rw-r--r--   0        0        0    11733 2023-06-30 21:35:42.907044 stringsifter-3.20230711/tests/fixtures/strings_output2
+-rw-r--r--   0        0        0        0 2023-06-30 21:35:42.907044 stringsifter-3.20230711/tests/fixtures/strings_output3
+-rw-r--r--   0        0        0     3067 2023-06-30 21:35:42.907044 stringsifter-3.20230711/tests/test_stringsifter.py
+-rw-r--r--   0        0        0     8432 1970-01-01 00:00:00.000000 stringsifter-3.20230711/PKG-INFO
```

### Comparing `stringsifter-2.20201202/LICENSE` & `stringsifter-3.20230711/LICENSE`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/README.md` & `stringsifter-3.20230711/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,43 +3,42 @@
 </div>
 
 --------------------------------------------------------------------------------
 
 StringSifter is a machine learning tool that automatically ranks strings based on their relevance for malware analysis.
 
 # Quick Links
-* [Technical Blogpost - *Learning to Rank Strings Output for Speedier Malware Analysis*](https://www.fireeye.com/blog/threat-research/2019/05/learning-to-rank-strings-output-for-speedier-malware-analysis.html)
-* [Announcement Blogpost - *Open Sourcing StringSifter*](https://www.fireeye.com/blog/threat-research/2019/09/open-sourcing-stringsifter.html)
+* [Technical Blogpost - *Learning to Rank Strings Output for Speedier Malware Analysis*](https://www.mandiant.com/resources/blog/learning-rank-strings-output-speedier-malware-analysis)
+* [Announcement Blogpost - *Open Sourcing StringSifter*](https://www.mandiant.com/resources/blog/open-sourcing-stringsifter)
 * [DerbyCon Talk - *StringSifter: Learning to Rank Strings Output for Speedier Malware Analysis*](https://youtu.be/pLiaVzOMJSk)
+* [StringSifter releases on PyPi](https://pypi.org/project/stringsifter/)
 
 # Usage
 
-StringSifter requires Python version 3.6 or newer. Run the following commands to get the code, run unit tests, and use the tool:
+StringSifter requires Python version 3.9 or newer. Run the following commands to get the code, run unit tests, and use the tool:
 
 ## Installation
 
-Use `pip` to get running immediately:
 ```sh
 pip install stringsifter
 ```
 
-For development, check out the correct branch for your Python version or stay on master for the latest supported version. Then use `pipenv`:
+For development, use [poetry](https://python-poetry.org/):
 ```sh
-git clone https://github.com/fireeye/stringsifter.git
+git clone https://github.com/mandiant/stringsifter.git
 cd stringsifter
-git checkout python3.7 #Optional
-pipenv install --dev
+poetry install --with dev
 ```
 
 ## Running Unit Tests
 
 To run unit tests from the StringSifter installation directory:
 
 ```sh
-pipenv run tests
+poetry run tests -v
 ```
 
 ## Running from the Command Line
 
 The `pip install` command installs two runnable scripts `flarestrings` and `rank_strings` into your python environment. When developing from source, use `pipenv run flarestrings` and `pipenv run rank_strings`.
 
 `flarestrings` mimics features of GNU binutils' `strings`, and `rank_strings` accepts piped input, for example:
@@ -132,8 +131,8 @@
 ## Issues
 We use [GitHub Issues](https://github.com/fireeye/stringsifter/issues) for posting bugs and feature requests.
 
 ## Acknowledgements
 - Thanks to the FireEye Data Science (FDS) and FireEye Labs Reverse Engineering (FLARE) teams for review and feedback.
 - StringSifter was designed and developed by Philip Tully (FDS), Matthew Haigh (FLARE), Jay Gibble (FLARE), and Michael Sikorski (FLARE).
 - The StringSifter logo was designed by Josh Langner (FLARE).
-- `flarestrings` is derived from the excellent tool [FLOSS](https://github.com/fireeye/flare-floss/blob/master/floss/strings.py#L7-L9).
+- `flarestrings` is derived from the excellent tool [FLOSS](https://github.com/mandiant/flare-floss).
```

### Comparing `stringsifter-2.20201202/misc/stringsifter-flat-dark.png` & `stringsifter-3.20230711/misc/stringsifter-flat-dark.png`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/flarestrings.py` & `stringsifter-3.20230711/stringsifter/flarestrings.py`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/lib/constants.json` & `stringsifter-3.20230711/stringsifter/lib/constants.json`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/lib/lid.176.ftz` & `stringsifter-3.20230711/stringsifter/lib/lid.176.ftz`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/lib/markov.pkl` & `stringsifter-3.20230711/stringsifter/lib/markov.pkl`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/lib/stats.py` & `stringsifter-3.20230711/stringsifter/lib/stats.py`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/preprocess.py` & `stringsifter-3.20230711/stringsifter/preprocess.py`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/stringsifter/rank_strings.py` & `stringsifter-3.20230711/stringsifter/rank_strings.py`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/tests/fixtures/strings_output1` & `stringsifter-3.20230711/tests/fixtures/strings_output1`

 * *Files identical despite different names*

### Comparing `stringsifter-2.20201202/tests/fixtures/strings_output2` & `stringsifter-3.20230711/tests/fixtures/strings_output2`

 * *Files identical despite different names*

