# Comparing `tmp/aocd_example_parser-0.0.1.tar.gz` & `tmp/aocd_example_parser-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aocd_example_parser-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aocd_example_parser-2023.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aocd_example_parser-0.0.1.tar` & `aocd_example_parser-2023.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-07-12 02:44:04.456415 aocd_example_parser-0.0.1/LICENSE
--rw-r--r--   0        0        0     6774 2023-07-12 05:52:27.350796 aocd_example_parser-0.0.1/README.md
--rw-r--r--   0        0        0     1356 2023-07-12 04:52:26.740386 aocd_example_parser-0.0.1/aocd_example_parser.py
--rw-r--r--   0        0        0      872 2023-07-12 03:09:07.854443 aocd_example_parser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7351 1970-01-01 00:00:00.000000 aocd_example_parser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-12 05:57:39.031185 aocd_example_parser-2023.1/LICENSE
+-rw-r--r--   0        0        0     7231 2023-07-12 08:50:01.616493 aocd_example_parser-2023.1/README.md
+-rw-r--r--   0        0        0     1411 2023-07-12 08:50:01.616737 aocd_example_parser-2023.1/aocd_example_parser/__init__.py
+-rw-r--r--   0        0        0    55308 2023-07-12 08:50:01.617107 aocd_example_parser-2023.1/aocd_example_parser/examples.json
+-rw-r--r--   0        0        0     1788 2023-07-12 08:50:01.617332 aocd_example_parser-2023.1/aocd_example_parser/extraction.py
+-rw-r--r--   0        0        0      377 2023-07-12 08:50:01.617510 aocd_example_parser-2023.1/aocd_example_parser/util.py
+-rw-r--r--   0        0        0      873 2023-07-12 08:50:01.617725 aocd_example_parser-2023.1/pyproject.toml
+-rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 aocd_example_parser-2023.1/PKG-INFO
```

### Comparing `aocd_example_parser-0.0.1/README.md` & `aocd_example_parser-2023.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Advent-of-Code-Data Example Parser
 ==================================
 
 The annual programming challenge [Advent of Code](https://adventofcode.com/) frequently provides some example data (and solutions) for you to test your code against, which are usually scaled-down versions of the real input data you're supposed to be solving with each day.
 
 Although the real puzzle inputs and answers differ by user, the example data is written directly in the puzzle prose and is available to unauthenticated users too.
 
-To illustrate what this means, the first puzzle of 2022 was [--- Day 1: Calorie Counting ---
-](https://adventofcode.com/2022/day/1) and it has an example data of 54 bytes:
+To illustrate what this means, the first puzzle of 2022 was [`--- Day 1: Calorie Counting ---`
+](https://adventofcode.com/2022/day/1) and it has the following example data (54 bytes):
 
 ```
 1000
 2000
 3000
 
 4000
@@ -23,23 +23,23 @@
 9000
 
 10000
 ```
 
 The correct answers corresponding to this sample data were `24000` for part a, and `45000` for part b. The example data text was found in the first `<pre>` tag, and the answers were found in the last `<code>` blocks from each of the two `<article>` sections in the puzzle page HTML. Note that the first half of the puzzle must be solved before the second `<article>` tag shows up, so the second article is not visible to unauthenticated users.
 
-In 2022, this same pattern of example data locations in the HTML was repeated for four more days consecutively, before varying on [--- Day 6: Tuning Trouble ---](https://adventofcode.com/2022/day/6).
+In 2022, this same pattern of example data locations in the HTML was repeated for four more days, consecutively, before varying on [`--- Day 6: Tuning Trouble ---`](https://adventofcode.com/2022/day/6).
 
 
 What is this package?
 ---------------------
 
-This package provides an implementation of an [aocd example parser](https://github.com/wimglenn/advent-of-code-data/blob/main/aocd/examples.py) plugin, which attempts to parse the sample data and solutions automatically from the puzzle prose.
+This package provides an implementation of an [aocd example parser](https://github.com/wimglenn/advent-of-code-data/blob/main/aocd/examples.py) plugin, which attempts to parse the sample data and corresponding answers automatically from the puzzle prose.
 
-An aocd example parser plugin is an [entry-point](https://packaging.python.org/en/latest/specifications/entry-points/) in the `"adventofcode.examples"` group. It should be a callable accepting two arguments, like this:
+An aocd example parser plugin is an [entry-point](https://packaging.python.org/en/latest/specifications/entry-points/) in the `"adventofcode.examples"` group. It must be a callable accepting two arguments, like this:
 
 ```python
 from aocd.examples import Example
 from aocd.examples import Page
 
 def my_plugin(page: Page, datas: list[str]) -> list[Example]:
     """my example parser implementation"""
@@ -47,16 +47,17 @@
     # given the puzzle html found in "page", and a list of real user inputs found in
     # "datas" for potential comparison, the plugin function should scrape and return
     # a list of Example instances. Note that "datas" might be an empty list, if aocd
     # doesn't have any real user inputs cached locally.
     return result
 ```
 
-Such a package should register an entry point in the `"adventofcode.examples"` group within the package metadata, by adding something like this in your `pyproject.toml` file:
+This callable must return a list of `Example` instances. If no examples can be parsed, you should return an empty list `[]`, rather than `None`.
 
+Any package providing an example parser should register an entry point in the `"adventofcode.examples"` group within the package metadata, by adding something like this in your `pyproject.toml` file:
 ```toml
 [project.entry-points."adventofcode.examples"]
 my_example_parser = "my_module:my_plugin"
 ```
 
 See the [Entry points](https://peps.python.org/pep-0621/#entry-points) section in [_PEP 621 – Storing project metadata in pyproject.toml_](https://peps.python.org/pep-0621) for more information.
 
@@ -76,40 +77,40 @@
 
 And it should be selectable for use/verification with
 
 ```bash
 $ aoce --plugin=my_example_parser
 ```
 
+
 Why a plugin? Wouldn't it be simpler to write a parser in aocd directly?
 ------------------------------------------------------------------------
 
-Most of the logic for my parser _is_ written in `aocd` directly.
-
 I've created this package, and the corresponding tester `aoce` in `advent-of-code-data`, to open it up to the community to try and come up with a better parser.
-This package exemplifies the interface that a parser should work with, so to speak.
+This package exemplifies the interface that a parser should work with, so to speak, and `aocd` uses this plugin for [dogfooding](https://en.wikipedia.org/wiki/Eating_your_own_dog_food). As an added benifit, it means the example parsing can be frequently updated to ensure correct results are returned for previous puzzles, without requiring a new release of `aocd` itself.
 
 There are so many creative and smart people hacking on AoC that I'm sure several of you can come up with something much better than I was able to!
 The default implementation from `aocd` fails more than 40% of the time, so you don't have a very high bar to beat.
 If someone comes up with a better-performing parser than "_take the first pre as input data, take answers from the last codeblocks in each article_", I will make their implementation the new default in a future version of `aocd`.
 
-Please note that you probably shouldn't try to get to 100% success, that will be super-difficult if not _impossible_.
+If you're considering writing an example parser, it's not advisable to try to get to 100% success rate, that will be super-difficult if not _impossible_.
 Some of the puzzles have [many examples](https://adventofcode.com/2022/day/6), some are [really tricky to parse](https://adventofcode.com/2018/day/15), and some offer [no example at all](https://adventofcode.com/2018/day/21).
 But difficulty aside, the main reason is that you needn't "overfit" to previous puzzles.
 This is because `advent-of-code-data` always intends to return correct example data _for past puzzles_ by hardcoding the code-block locations.
 
 **The only thing that matters for a parser plugin is how well it can perform for a never-before seen puzzle**.
 That is, the goal is to maximize the _probability_ that your parser will somehow find the right result at the instant a new puzzle unlocks.
 
+
 How well does the default implementation perform?
 -------------------------------------------------
 
 It depends on the year.
 The locations got a lot more consistent in recent years, so it has performed better more recently.
-The last thing the `aoce` script points out is a rough percentage the parser got right.
+The final line that `aoce` script prints out is a rough percentage the parser got right.
 
 ```bash
 $ for YEAR in {2015..2022};
 do echo -n "$YEAR " && aoce -p aocd_examples_default -y $YEAR | tail -1;
 done
 2015 plugin 'aocd_examples_default' scored 78/336 (23.2%)
 2016 plugin 'aocd_examples_default' scored 53/159 (33.3%)
```

### Comparing `aocd_example_parser-0.0.1/aocd_example_parser.py` & `aocd_example_parser-2023.1/aocd_example_parser/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from aocd.examples import extract_examples
 from aocd.examples import Example
 from aocd.examples import Page
 
+from .extraction import extract_examples
+from .util import real_datas_unused
 
+
+@real_datas_unused
 def plugin(page: Page, datas: list[str]) -> list[Example]:
     """
     Example parser implementation which always uses the aocd default locators.
     These are currently:
 
       "default_locators": {
         "input_data": "a_pre[0]",
@@ -16,19 +19,20 @@
       },
 
     The text of the first <pre> tag, if any, is the input data.
     The last <code> block of the first <article> contains the part a answer.
     The last <code> block of the second <article> contains the part b answer.
     The extra context is nothing.
     """
-    return extract_examples(page.raw_html, use_default_locators=True)
+    return extract_examples(page, use_default_locators=True)
 
 
+@real_datas_unused
 def hardcoded_locations(page: Page, datas: list[str]) -> list[Example]:
     """
     Example parser implementation which always uses the pre-calculated locators.
     This implementation will always return correct results for puzzles which are
     published in the past. It can be used as a reference to compare the results of
     other example parser implementations against. For puzzles that hadn't been released
     yet, the results are the same as the "default locators" plugin defined above.
     """
-    return extract_examples(page.raw_html)
+    return extract_examples(page)
```

### Comparing `aocd_example_parser-0.0.1/pyproject.toml` & `aocd_example_parser-2023.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
-name = "aocd_example_parser"
-version = "0.0.1"
+name = "aocd-example-parser"
+version = "2023.1"
 description = "Default implementation of an example parser plugin for advent-of-code-data"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `aocd_example_parser-0.0.1/PKG-INFO` & `aocd_example_parser-2023.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aocd_example_parser
-Version: 0.0.1
+Name: aocd-example-parser
+Version: 2023.1
 Summary: Default implementation of an example parser plugin for advent-of-code-data
 Author-email: Wim Glenn <hey@wimglenn.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,16 +15,16 @@
 Advent-of-Code-Data Example Parser
 ==================================
 
 The annual programming challenge [Advent of Code](https://adventofcode.com/) frequently provides some example data (and solutions) for you to test your code against, which are usually scaled-down versions of the real input data you're supposed to be solving with each day.
 
 Although the real puzzle inputs and answers differ by user, the example data is written directly in the puzzle prose and is available to unauthenticated users too.
 
-To illustrate what this means, the first puzzle of 2022 was [--- Day 1: Calorie Counting ---
-](https://adventofcode.com/2022/day/1) and it has an example data of 54 bytes:
+To illustrate what this means, the first puzzle of 2022 was [`--- Day 1: Calorie Counting ---`
+](https://adventofcode.com/2022/day/1) and it has the following example data (54 bytes):
 
 ```
 1000
 2000
 3000
 
 4000
@@ -37,23 +37,23 @@
 9000
 
 10000
 ```
 
 The correct answers corresponding to this sample data were `24000` for part a, and `45000` for part b. The example data text was found in the first `<pre>` tag, and the answers were found in the last `<code>` blocks from each of the two `<article>` sections in the puzzle page HTML. Note that the first half of the puzzle must be solved before the second `<article>` tag shows up, so the second article is not visible to unauthenticated users.
 
-In 2022, this same pattern of example data locations in the HTML was repeated for four more days consecutively, before varying on [--- Day 6: Tuning Trouble ---](https://adventofcode.com/2022/day/6).
+In 2022, this same pattern of example data locations in the HTML was repeated for four more days, consecutively, before varying on [`--- Day 6: Tuning Trouble ---`](https://adventofcode.com/2022/day/6).
 
 
 What is this package?
 ---------------------
 
-This package provides an implementation of an [aocd example parser](https://github.com/wimglenn/advent-of-code-data/blob/main/aocd/examples.py) plugin, which attempts to parse the sample data and solutions automatically from the puzzle prose.
+This package provides an implementation of an [aocd example parser](https://github.com/wimglenn/advent-of-code-data/blob/main/aocd/examples.py) plugin, which attempts to parse the sample data and corresponding answers automatically from the puzzle prose.
 
-An aocd example parser plugin is an [entry-point](https://packaging.python.org/en/latest/specifications/entry-points/) in the `"adventofcode.examples"` group. It should be a callable accepting two arguments, like this:
+An aocd example parser plugin is an [entry-point](https://packaging.python.org/en/latest/specifications/entry-points/) in the `"adventofcode.examples"` group. It must be a callable accepting two arguments, like this:
 
 ```python
 from aocd.examples import Example
 from aocd.examples import Page
 
 def my_plugin(page: Page, datas: list[str]) -> list[Example]:
     """my example parser implementation"""
@@ -61,16 +61,17 @@
     # given the puzzle html found in "page", and a list of real user inputs found in
     # "datas" for potential comparison, the plugin function should scrape and return
     # a list of Example instances. Note that "datas" might be an empty list, if aocd
     # doesn't have any real user inputs cached locally.
     return result
 ```
 
-Such a package should register an entry point in the `"adventofcode.examples"` group within the package metadata, by adding something like this in your `pyproject.toml` file:
+This callable must return a list of `Example` instances. If no examples can be parsed, you should return an empty list `[]`, rather than `None`.
 
+Any package providing an example parser should register an entry point in the `"adventofcode.examples"` group within the package metadata, by adding something like this in your `pyproject.toml` file:
 ```toml
 [project.entry-points."adventofcode.examples"]
 my_example_parser = "my_module:my_plugin"
 ```
 
 See the [Entry points](https://peps.python.org/pep-0621/#entry-points) section in [_PEP 621 – Storing project metadata in pyproject.toml_](https://peps.python.org/pep-0621) for more information.
 
@@ -90,40 +91,40 @@
 
 And it should be selectable for use/verification with
 
 ```bash
 $ aoce --plugin=my_example_parser
 ```
 
+
 Why a plugin? Wouldn't it be simpler to write a parser in aocd directly?
 ------------------------------------------------------------------------
 
-Most of the logic for my parser _is_ written in `aocd` directly.
-
 I've created this package, and the corresponding tester `aoce` in `advent-of-code-data`, to open it up to the community to try and come up with a better parser.
-This package exemplifies the interface that a parser should work with, so to speak.
+This package exemplifies the interface that a parser should work with, so to speak, and `aocd` uses this plugin for [dogfooding](https://en.wikipedia.org/wiki/Eating_your_own_dog_food). As an added benifit, it means the example parsing can be frequently updated to ensure correct results are returned for previous puzzles, without requiring a new release of `aocd` itself.
 
 There are so many creative and smart people hacking on AoC that I'm sure several of you can come up with something much better than I was able to!
 The default implementation from `aocd` fails more than 40% of the time, so you don't have a very high bar to beat.
 If someone comes up with a better-performing parser than "_take the first pre as input data, take answers from the last codeblocks in each article_", I will make their implementation the new default in a future version of `aocd`.
 
-Please note that you probably shouldn't try to get to 100% success, that will be super-difficult if not _impossible_.
+If you're considering writing an example parser, it's not advisable to try to get to 100% success rate, that will be super-difficult if not _impossible_.
 Some of the puzzles have [many examples](https://adventofcode.com/2022/day/6), some are [really tricky to parse](https://adventofcode.com/2018/day/15), and some offer [no example at all](https://adventofcode.com/2018/day/21).
 But difficulty aside, the main reason is that you needn't "overfit" to previous puzzles.
 This is because `advent-of-code-data` always intends to return correct example data _for past puzzles_ by hardcoding the code-block locations.
 
 **The only thing that matters for a parser plugin is how well it can perform for a never-before seen puzzle**.
 That is, the goal is to maximize the _probability_ that your parser will somehow find the right result at the instant a new puzzle unlocks.
 
+
 How well does the default implementation perform?
 -------------------------------------------------
 
 It depends on the year.
 The locations got a lot more consistent in recent years, so it has performed better more recently.
-The last thing the `aoce` script points out is a rough percentage the parser got right.
+The final line that `aoce` script prints out is a rough percentage the parser got right.
 
 ```bash
 $ for YEAR in {2015..2022};
 do echo -n "$YEAR " && aoce -p aocd_examples_default -y $YEAR | tail -1;
 done
 2015 plugin 'aocd_examples_default' scored 78/336 (23.2%)
 2016 plugin 'aocd_examples_default' scored 53/159 (33.3%)
```

