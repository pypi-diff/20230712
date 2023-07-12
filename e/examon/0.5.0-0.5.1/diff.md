# Comparing `tmp/examon-0.5.0.tar.gz` & `tmp/examon-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon-0.5.0.tar", max compression
+gzip compressed data, was "examon-0.5.1.tar", max compression
```

## Comparing `examon-0.5.0.tar` & `examon-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.0/examon/__init__.py
--rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.0/examon/lib/__init__.py
--rwxr-xr-x   0        0        0      468 2023-02-04 14:18:10.434445 examon-0.5.0/examon/lib/calc_stats.py
--rw-r--r--   0        0        0     1736 2023-07-07 15:08:43.883637 examon-0.5.0/examon/lib/quiz_engine.py
--rw-r--r--   0        0        0     1262 2023-07-09 20:52:59.296815 examon-0.5.0/examon/lib/quiz_engine_factory.py
--rw-r--r--   0        0        0     2389 2023-07-09 19:37:47.112886 examon-0.5.0/examon/lib/repo_manager.py
--rw-r--r--   0        0        0      366 2023-05-09 19:07:23.705779 examon-0.5.0/examon/lib/streak_tracker.py
--rwxr-xr-x   0        0        0      118 2023-07-09 20:03:47.840793 examon-0.5.0/examon/main.py
--rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.0/examon/view/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.0/examon/view/cli/__init__.py
--rwxr-xr-x   0        0        0     1711 2023-07-09 20:21:28.227289 examon-0.5.0/examon/view/cli/examon_arg_parse.py
--rwxr-xr-x   0        0        0      663 2023-07-12 17:14:39.575934 examon-0.5.0/examon/view/cli/main.py
--rw-r--r--   0        0        0      312 2023-07-12 17:16:53.877238 examon-0.5.0/examon/view/cli/overview.py
--rw-r--r--   0        0        0     1134 2023-07-11 10:42:41.187587 examon-0.5.0/examon/view/cli/repo.py
--rw-r--r--   0        0        0      488 2023-07-12 17:16:20.529570 examon-0.5.0/examon/view/cli/runner.py
--rwxr-xr-x   0        0        0      861 2023-04-12 17:42:31.225766 examon-0.5.0/examon/view/formatter_options.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.0/examon/view/input/__init__.py
--rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.0/examon/view/input/answer_question.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.0/examon/view/output/__init__.py
--rwxr-xr-x   0        0        0      187 2023-04-12 17:29:51.001345 examon-0.5.0/examon/view/output/display_stats.py
--rwxr-xr-x   0        0        0      335 2023-01-28 12:55:33.777034 examon-0.5.0/examon/view/output/functions.py
--rwxr-xr-x   0        0        0     1771 2023-06-03 10:59:00.541458 examon-0.5.0/examon/view/output/question.py
--rwxr-xr-x   0        0        0      509 2023-07-12 17:33:46.129266 examon-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 examon-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      837 2023-07-11 11:00:43.648041 examon-0.5.1/README.md
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.1/examon/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.1/examon/lib/__init__.py
+-rwxr-xr-x   0        0        0      468 2023-02-04 14:18:10.434445 examon-0.5.1/examon/lib/calc_stats.py
+-rw-r--r--   0        0        0     1738 2023-07-12 20:04:21.589727 examon-0.5.1/examon/lib/quiz_engine.py
+-rw-r--r--   0        0        0     1242 2023-07-12 20:04:21.584847 examon-0.5.1/examon/lib/quiz_engine_factory.py
+-rw-r--r--   0        0        0     2389 2023-07-09 19:37:47.112886 examon-0.5.1/examon/lib/repo_manager.py
+-rw-r--r--   0        0        0      366 2023-05-09 19:07:23.705779 examon-0.5.1/examon/lib/streak_tracker.py
+-rwxr-xr-x   0        0        0       99 2023-07-12 20:13:15.318911 examon-0.5.1/examon/main.py
+-rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.1/examon/view/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.1/examon/view/cli/__init__.py
+-rwxr-xr-x   0        0        0     1711 2023-07-09 20:21:28.227289 examon-0.5.1/examon/view/cli/examon_arg_parse.py
+-rwxr-xr-x   0        0        0      663 2023-07-12 17:14:39.575934 examon-0.5.1/examon/view/cli/main.py
+-rw-r--r--   0        0        0      312 2023-07-12 17:16:53.877238 examon-0.5.1/examon/view/cli/overview.py
+-rw-r--r--   0        0        0     1134 2023-07-11 10:42:41.187587 examon-0.5.1/examon/view/cli/repo.py
+-rw-r--r--   0        0        0      488 2023-07-12 17:16:20.529570 examon-0.5.1/examon/view/cli/runner.py
+-rwxr-xr-x   0        0        0      861 2023-04-12 17:42:31.225766 examon-0.5.1/examon/view/formatter_options.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.1/examon/view/input/__init__.py
+-rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.1/examon/view/input/answer_question.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.1/examon/view/output/__init__.py
+-rwxr-xr-x   0        0        0      187 2023-04-12 17:29:51.001345 examon-0.5.1/examon/view/output/display_stats.py
+-rwxr-xr-x   0        0        0      335 2023-01-28 12:55:33.777034 examon-0.5.1/examon/view/output/functions.py
+-rwxr-xr-x   0        0        0     1771 2023-06-03 10:59:00.541458 examon-0.5.1/examon/view/output/question.py
+-rwxr-xr-x   0        0        0      532 2023-07-12 20:21:35.984248 examon-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 examon-0.5.1/PKG-INFO
```

### Comparing `examon-0.5.0/examon/lib/quiz_engine.py` & `examon-0.5.1/examon/lib/quiz_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from examon_core.question_response import QuestionResponse
 from examon.lib.streak_tracker import StreakTracker
+
+
 class QuizEngine:
     def __init__(self, questions=None,
                  stats_outputter=None,
                  view_mappings=None):
         self.questions = questions
         self.correct_answers = 0
         self.responses = []
```

### Comparing `examon-0.5.0/examon/lib/quiz_engine_factory.py` & `examon-0.5.1/examon/lib/quiz_engine_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from examon_core.question import *
 from examon_core.examon_item_registry import *
 
-from examon.view.input.answer_question import AutoAnswerInputter, AnswerInputter, FreeTextAnswerInputter
+from examon.view.input.answer_question import AnswerInputter, FreeTextAnswerInputter
 from examon.view.output.question import *
 from .calc_stats import calc_stats
 from .quiz_engine import QuizEngine
 
 
 class QuizEngineFactory:
     @staticmethod
```

### Comparing `examon-0.5.0/examon/lib/repo_manager.py` & `examon-0.5.1/examon/lib/repo_manager.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/cli/examon_arg_parse.py` & `examon-0.5.1/examon/view/cli/examon_arg_parse.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/cli/main.py` & `examon-0.5.1/examon/view/cli/main.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/cli/repo.py` & `examon-0.5.1/examon/view/cli/repo.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/formatter_options.py` & `examon-0.5.1/examon/view/formatter_options.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/input/answer_question.py` & `examon-0.5.1/examon/view/input/answer_question.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.0/examon/view/output/question.py` & `examon-0.5.1/examon/view/output/question.py`

 * *Files identical despite different names*

