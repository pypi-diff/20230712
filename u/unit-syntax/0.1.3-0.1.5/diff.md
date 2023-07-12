# Comparing `tmp/unit_syntax-0.1.3.tar.gz` & `tmp/unit_syntax-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.1.3.tar", max compression
+gzip compressed data, was "unit_syntax-0.1.5.tar", max compression
```

## Comparing `unit_syntax-0.1.3.tar` & `unit_syntax-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5227 2023-05-09 21:09:27.049378 unit_syntax-0.1.3/README.md
--rw-r--r--   0        0        0      641 2023-05-09 21:09:27.053378 unit_syntax-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      689 2023-05-09 21:09:27.053378 unit_syntax-0.1.3/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149332 2023-05-09 21:09:27.053378 unit_syntax-0.1.3/unit_syntax/parser.py
--rw-r--r--   0        0        0     4608 2023-05-09 21:09:27.053378 unit_syntax-0.1.3/unit_syntax/transform.py
--rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 unit_syntax-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5255 2023-07-12 20:16:05.681739 unit_syntax-0.1.5/README.md
+-rw-r--r--   0        0        0      641 2023-07-12 20:16:05.681739 unit_syntax-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2159 2023-07-12 20:16:05.681739 unit_syntax-0.1.5/unit_syntax/__init__.py
+-rw-r--r--   0        0        0   149367 2023-07-12 20:16:05.681739 unit_syntax-0.1.5/unit_syntax/parser.py
+-rw-r--r--   0        0        0     5039 2023-07-12 20:16:05.681739 unit_syntax-0.1.5/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5938 1970-01-01 00:00:00.000000 unit_syntax-0.1.5/PKG-INFO
```

### Comparing `unit_syntax-0.1.3/README.md` & `unit_syntax-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 `unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
 
 ```python
 >>> speed = 5 meters/second
->>> 2 seconds * speed
+>>> (2 seconds) * speed
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
@@ -25,103 +25,124 @@
 
 Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
+Units apply to the immediately preceding value:
 
 ```python
-x * 1.21 gigawatts
+1.21 gigawatts # literal number
+(30 + 7) watts # parenthesized expression
+[5, 7] meters # literal list
+(9, 11) lumens # literal tuple
+# variable reference
+y becquerel
+position.x attoparsec
+velocity[player_id] meters/s
 ```
 
-This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`. The high precedence means units apply to the literal not the whole expression.
+Units are parsed greedily and bind only to the immediately preceding value:
 
-Values can be converted to another measurement system:
+```python
+x * 5 meters # x * (5 meters), not (x*5) meters
+```
+
+Quantities can be converted to another measurement system:
+
+```python
+>>> (88 miles / hour) furlongs / fortnight
+236543.5269120001 furlong / fortnight
+>>> (0 degC) degF
+31.999999999999936 degree_Fahrenheit
+```
+
+It's _highly_ recommended to parenthesize any complex that include units. For example:
 
 ```python
-(88 miles / hour) furlongs / fortnight
+1 meters * sin(degrees)
 ```
 
-Pint transparently [supports numpy](https://pint.readthedocs.io/en/stable/user/numpy.html) when available:
+This is desugared to `Quantity(1, "meters * sin(degrees)")`, when you probably wanted `(1 meters) * sin(degrees)`.
+
+Units _may not_ begin with parentheses (consider the possible
+interpretations of `x (meters)`). Parentheses are allowed anywhere else:
 
 ```python
-velocity = [5, 7] meters/second**2
-location = velocity * 2 seconds
-distance_traveled = numpy.linalg.norm(location)
+x (newton meters)/(second*kg) # parsed as a function call, will result in a runtime error
+x newton meters/(second*kg) # ok
 ```
 
-## The Grammar
+## Syntax Details
 
-The units term follows this grammar:
+The full grammar for units is:
 
 ```
 units:
-    | NAME '/' units_group
-    | NAME '*' units_group
-    | NAME units_group
-    | NAME '**' NUMBER
+    | units '/' units_group
+    | units '*' units_group
+    | units units_group
+    | units '**' NUMBER
     | NAME
 
 units_group:
     | '(' units ')'
     | units
 ```
 
-## Why? How?
+Compound units allow the usual operators multiplication, division, and exponentiation with the usual precedence rules. Adjacent units without an operator are treated as multiplication.
+
+## Help!
+
+If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed python code to the console.
 
-I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
+## Should I use this?
 
-`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
+There are tradeoffs. When using unit-syntax as an interactive calculator the clarity of explicit units improves both readability and correctness. However, the new syntax also introduces _new_ opportunities for error if an expression is parsed in an unexpected way. Usually this is obvious when used interactively, but it's something to be aware of.
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
-The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
+## Why? How?
+
+I like using Python with [Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but its (necessary) verbosity makes it hard to see the underlying calculation that's going. Ultimately I want something that is as readable as what I'd write on paper using normal notation.
+
+`unit-syntax` is an IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
-## Open questions and future work
-
-- Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`. This has the advantage of being unambiguous regardless of parenthesization. In python this would conflcit with `value in [a, b, c]`, but `as` is
-
-- Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
-- Test against various ipython and python versions
-- Support standalone scripts through sys.meta_path
-- Check units at parse time
-- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
-- Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
-- Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
-- Describe parsing ambuguity like `1 meters * sin(45 degrees)`
-- Figure out story around parenthesization
+A [long discussion on the python-ideas mailing list](https://lwn.net/Articles/900739/) about literal units in Python.
 
 ## Development
 
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
- $ poetry install --with dev
- $ poetry run pytest
+
+$ poetry install --with dev
+$ poetry run pytest
+
 ```
 
 ## Future work and open questions
 
-- Parenthisized units expressions
-- Demo colab notebook
-- Move to tree-sitter so there's a chance of getting syntax highlighting
-- Jupyter syntax checks
-- Typography of output
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
-- Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
+- Expand the demo Colab notebook
+- Typography of output
+- Its too easy to get an unexpected parse if you forget parentheses.
+
+```
+
+```
```

### Comparing `unit_syntax-0.1.3/pyproject.toml` & `unit_syntax-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.1.3"
+version = "0.1.5"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{include = "unit_syntax"}]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
-description = "Literal physical units for Jupyter and IPython"
+description = "Physical unit literals for Jupyter and IPython"
 
 [tool.poetry.dependencies]
 python = ">=3.8, < 4"
 Pint = "^0.20"
 ipython = ">=7"
 pegen = "^0.2"
```

### Comparing `unit_syntax-0.1.3/unit_syntax/parser.py` & `unit_syntax-0.1.5/unit_syntax/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2271,51 +2271,51 @@
         if (
             (sum := self.sum())
         ):
             return sum;
         self._reset(mark)
         return None;
 
-    @memoize
+    @memoize_left_rec
     def units(self) -> Optional[Any]:
-        # units: NAME '/' units_group | NAME '*' units_group | NAME units_group | NAME '**' NUMBER | NAME
+        # units: units '/' units_group | units '*' units_group | units units_group | units '**' NUMBER | NAME
         mark = self._mark()
         if (
-            (name := self.name())
+            (units := self.units())
             and
             (literal := self.expect('/'))
             and
             (units_group := self.units_group())
         ):
-            return [name, literal, units_group];
+            return [units, literal, units_group];
         self._reset(mark)
         if (
-            (name := self.name())
+            (units := self.units())
             and
             (literal := self.expect('*'))
             and
             (units_group := self.units_group())
         ):
-            return [name, literal, units_group];
+            return [units, literal, units_group];
         self._reset(mark)
         if (
-            (name := self.name())
+            (units := self.units())
             and
             (units_group := self.units_group())
         ):
-            return [name, units_group];
+            return [units, units_group];
         self._reset(mark)
         if (
-            (name := self.name())
+            (units := self.units())
             and
             (literal := self.expect('**'))
             and
             (number := self.number())
         ):
-            return [name, literal, number];
+            return [units, literal, number];
         self._reset(mark)
         if (
             (name := self.name())
         ):
             return name;
         self._reset(mark)
         return None;
@@ -2455,26 +2455,33 @@
         ):
             return power;
         self._reset(mark)
         return None;
 
     @memoize
     def power(self) -> Optional[Any]:
-        # power: await_primary '**' factor | await_primary
+        # power: await_primary '**' factor | await_primary units | await_primary
         mark = self._mark()
         if (
             (await_primary := self.await_primary())
             and
             (literal := self.expect('**'))
             and
             (factor := self.factor())
         ):
             return [await_primary, literal, factor];
         self._reset(mark)
         if (
+            (a := self.await_primary())
+            and
+            (u := self.units())
+        ):
+            return ( 'value_with_units' , a , u );
+        self._reset(mark)
+        if (
             (await_primary := self.await_primary())
         ):
             return await_primary;
         self._reset(mark)
         return None;
 
     @memoize
@@ -2493,24 +2500,17 @@
         ):
             return primary;
         self._reset(mark)
         return None;
 
     @memoize_left_rec
     def primary(self) -> Optional[Any]:
-        # primary: primary units | primary '.' NAME | primary genexp | primary '(' arguments? ')' | primary '[' slices ']' | atom
+        # primary: primary '.' NAME | primary genexp | primary '(' arguments? ')' | primary '[' slices ']' | atom
         mark = self._mark()
         if (
-            (p := self.primary())
-            and
-            (u := self.units())
-        ):
-            return ( 'primary_with_units' , p , u );
-        self._reset(mark)
-        if (
             (primary := self.primary())
             and
             (literal := self.expect('.'))
             and
             (name := self.name())
         ):
             return [primary, literal, name];
```

### Comparing `unit_syntax-0.1.3/unit_syntax/transform.py` & `unit_syntax-0.1.5/unit_syntax/transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from io import StringIO
 from typing import Iterator, Optional, Generator
 from .parser import GeneratedParser
 from pegen.tokenizer import Tokenizer
 
 Position = tuple[int, int]
 
+
 class SourcePosQuery:
     """Return source ranges between two (line, column) pairs"""
 
     def __init__(self, code: str):
-        self.code_lines = code.splitlines()
+        self.code_lines = code.splitlines(keepends=True)
         # The ENDMARKER token points to one line past the end of the file
         self.code_lines.append("")
 
     def between_pos(self, prev_end: Position, next_start: Position) -> Iterator[str]:
         """returns the text between two tokens, inclusive of prev_end and exclusive of next_start"""
 
         # convert to 0-based indexing because I'm not a maniac
@@ -34,27 +35,26 @@
 class OutputWriter:
     source: SourcePosQuery
     prev_tok_end: Position
     output: list[str]
 
     def __init__(self, source: SourcePosQuery):
         self.source = source
-        self.prev_tok_end = (0, 0)
+        # token lines are 1-indexed
+        self.prev_tok_end = (1, 0)
         self.output = []
 
-    def write_segment(self, lit: str, token: tokenize.TokenInfo, emit_gap=True):
-
+    def write_segment(self, lit: str, token: tokenize.TokenInfo):
         # pegen rules of the form
         #   '<sep>'.rule
         #  match zero or more instances of `rule`` separated by `sep`, and sep is not included
         # in the resulting tree.  Handle this include any un-emitted preceding text when emitting
         # a token, except when we're actually emitting the translated units expressions.
-        if emit_gap:
-            gap = self.source.between_pos(self.prev_tok_end, token.start)
-            self.output.extend(gap)
+        gap = self.source.between_pos(self.prev_tok_end, token.start)
+        self.output.extend(gap)
         if token.end > self.prev_tok_end:
             self.prev_tok_end = token.end
         self.output.append(lit)
 
     def write_bare(self, lit: str):
         self.output.append(lit)
 
@@ -80,37 +80,43 @@
     """Given an AST produced by pegen, rewrite unit expressions into standard python and write the
     whole tree as a string back to `output`"""
     if isinstance(node, list):
         for child in node:
             ast_to_segments(child, output)
     elif isinstance(node, tokenize.TokenInfo):
         output.write_segment(node.string, node)
-    elif isinstance(node, tuple) and node[0] == "primary_with_units":
+    elif isinstance(node, tuple) and node[0] == "value_with_units":
         value_node = node[1]
         units_node = node[2]
 
         # sinc we're emitting text that doesn't appear in the input code, we need to manually grab the
-        # first token of value node to ensure any preceding text is also emitted.  See comment in
-        # write_segment for more details.
+        # first token of value node to ensure any preceding text is also emitted before it.
+        # e.g, for "(1 meters, 2 meters)", this ensures the comma is emitted *before* the Quantity constructor
+        # rather than inside it.
         first = first_token(node)
 
         output.write_segment("unit_syntax.Quantity(", first)
         ast_to_segments(value_node, output)
         output.write_bare(', "')
+        output.prev_tok_end = first_token(units_node).start
+        # no need to escape this because the units grammar rule only allows
+        # identifiers, parens and math operations
         ast_to_segments(units_node, output)
         output.write_bare('")')
     elif node is None:
         # TODO whats this
         pass
     else:
         raise Exception("unknown node: ", node)
 
+
 def generate_tokens(code: str) -> Iterator[tokenize.TokenInfo]:
     return tokenize.generate_tokens(StringIO(code).readline)
 
+
 def parse(tokens: Iterator[tokenize.TokenInfo]):
     VERBOSE = False
     tok = Tokenizer(tokens, verbose=VERBOSE)
     parser = GeneratedParser(tok, verbose=VERBOSE)
     tree = parser.start()
     if not tree:
         raise parser.make_syntax_error("<input>")
@@ -124,8 +130,10 @@
     source_query = SourcePosQuery(code)
     output = OutputWriter(source_query)
     ast_to_segments(tree, output)
     return output.to_string()
 
 
 def transform_lines(lines: list[str]) -> list[str]:
+    """IPython transforms provide a list of strings in the current cell, but to parse correctly we
+    need to parse them as a single string"""
     return transform("".join(lines)).splitlines(keepends=True)
```

### Comparing `unit_syntax-0.1.3/PKG-INFO` & `unit_syntax-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.1.3
-Summary: Literal physical units for Jupyter and IPython
+Version: 0.1.5
+Summary: Physical unit literals for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Project-URL: Repository, https://github.com/ahupp/unit-syntax
 Description-Content-Type: text/markdown
 
 `unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
 
 ```python
 >>> speed = 5 meters/second
->>> 2 seconds * speed
+>>> (2 seconds) * speed
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
@@ -44,104 +44,125 @@
 
 Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
+Units apply to the immediately preceding value:
 
 ```python
-x * 1.21 gigawatts
+1.21 gigawatts # literal number
+(30 + 7) watts # parenthesized expression
+[5, 7] meters # literal list
+(9, 11) lumens # literal tuple
+# variable reference
+y becquerel
+position.x attoparsec
+velocity[player_id] meters/s
 ```
 
-This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`. The high precedence means units apply to the literal not the whole expression.
+Units are parsed greedily and bind only to the immediately preceding value:
 
-Values can be converted to another measurement system:
+```python
+x * 5 meters # x * (5 meters), not (x*5) meters
+```
+
+Quantities can be converted to another measurement system:
+
+```python
+>>> (88 miles / hour) furlongs / fortnight
+236543.5269120001 furlong / fortnight
+>>> (0 degC) degF
+31.999999999999936 degree_Fahrenheit
+```
+
+It's _highly_ recommended to parenthesize any complex that include units. For example:
 
 ```python
-(88 miles / hour) furlongs / fortnight
+1 meters * sin(degrees)
 ```
 
-Pint transparently [supports numpy](https://pint.readthedocs.io/en/stable/user/numpy.html) when available:
+This is desugared to `Quantity(1, "meters * sin(degrees)")`, when you probably wanted `(1 meters) * sin(degrees)`.
+
+Units _may not_ begin with parentheses (consider the possible
+interpretations of `x (meters)`). Parentheses are allowed anywhere else:
 
 ```python
-velocity = [5, 7] meters/second**2
-location = velocity * 2 seconds
-distance_traveled = numpy.linalg.norm(location)
+x (newton meters)/(second*kg) # parsed as a function call, will result in a runtime error
+x newton meters/(second*kg) # ok
 ```
 
-## The Grammar
+## Syntax Details
 
-The units term follows this grammar:
+The full grammar for units is:
 
 ```
 units:
-    | NAME '/' units_group
-    | NAME '*' units_group
-    | NAME units_group
-    | NAME '**' NUMBER
+    | units '/' units_group
+    | units '*' units_group
+    | units units_group
+    | units '**' NUMBER
     | NAME
 
 units_group:
     | '(' units ')'
     | units
 ```
 
-## Why? How?
+Compound units allow the usual operators multiplication, division, and exponentiation with the usual precedence rules. Adjacent units without an operator are treated as multiplication.
+
+## Help!
+
+If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed python code to the console.
 
-I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
+## Should I use this?
 
-`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
+There are tradeoffs. When using unit-syntax as an interactive calculator the clarity of explicit units improves both readability and correctness. However, the new syntax also introduces _new_ opportunities for error if an expression is parsed in an unexpected way. Usually this is obvious when used interactively, but it's something to be aware of.
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
-The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
+## Why? How?
+
+I like using Python with [Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but its (necessary) verbosity makes it hard to see the underlying calculation that's going. Ultimately I want something that is as readable as what I'd write on paper using normal notation.
+
+`unit-syntax` is an IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
-## Open questions and future work
-
-- Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`. This has the advantage of being unambiguous regardless of parenthesization. In python this would conflcit with `value in [a, b, c]`, but `as` is
-
-- Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
-- Test against various ipython and python versions
-- Support standalone scripts through sys.meta_path
-- Check units at parse time
-- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
-- Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
-- Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
-- Describe parsing ambuguity like `1 meters * sin(45 degrees)`
-- Figure out story around parenthesization
+A [long discussion on the python-ideas mailing list](https://lwn.net/Articles/900739/) about literal units in Python.
 
 ## Development
 
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
- $ poetry install --with dev
- $ poetry run pytest
+
+$ poetry install --with dev
+$ poetry run pytest
+
 ```
 
 ## Future work and open questions
 
-- Parenthisized units expressions
-- Demo colab notebook
-- Move to tree-sitter so there's a chance of getting syntax highlighting
-- Jupyter syntax checks
-- Typography of output
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
-- Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
+- Expand the demo Colab notebook
+- Typography of output
+- Its too easy to get an unexpected parse if you forget parentheses.
+
+```
+
+```
```

