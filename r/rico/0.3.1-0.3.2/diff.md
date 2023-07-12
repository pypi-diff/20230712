# Comparing `tmp/rico-0.3.1.tar.gz` & `tmp/rico-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.3.1.tar", last modified: Sun Jul  2 10:43:10 2023, max compression
+gzip compressed data, was "rico-0.3.2.tar", last modified: Wed Jul 12 16:55:22 2023, max compression
```

## Comparing `rico-0.3.1.tar` & `rico-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-07-02 10:42:37.317854 rico-0.3.1/LICENSE
--rw-r--r--   0        0        0    16506 2023-07-02 10:42:37.317854 rico-0.3.1/README.md
--rw-r--r--   0        0        0     2955 2023-07-02 10:43:10.933957 rico-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      710 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/__init__.py
--rw-r--r--   0        0        0     6399 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_config.py
--rw-r--r--   0        0        0     5509 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_container.py
--rw-r--r--   0        0        0    13794 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_content.py
--rw-r--r--   0        0        0     7951 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-07-02 10:42:37.321854 rico-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__config.py
--rw-r--r--   0        0        0    10250 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__container.py
--rw-r--r--   0        0        0    17254 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__content.py
--rw-r--r--   0        0        0    10803 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__version.py
--rw-r--r--   0        0        0    18162 1970-01-01 00:00:00.000000 rico-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-12 16:54:47.825177 rico-0.3.2/LICENSE
+-rw-r--r--   0        0        0    16832 2023-07-12 16:54:47.825177 rico-0.3.2/README.md
+-rw-r--r--   0        0        0     2993 2023-07-12 16:55:22.505268 rico-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/__init__.py
+-rw-r--r--   0        0        0     7139 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/_config.py
+-rw-r--r--   0        0        0     5280 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/_container.py
+-rw-r--r--   0        0        0    16695 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/_content.py
+-rw-r--r--   0        0        0     7951 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-07-12 16:54:47.829177 rico-0.3.2/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-07-12 16:54:47.829177 rico-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     2803 2023-07-12 16:54:47.829177 rico-0.3.2/tests/test__config.py
+-rw-r--r--   0        0        0    10222 2023-07-12 16:54:47.829177 rico-0.3.2/tests/test__container.py
+-rw-r--r--   0        0        0    25722 2023-07-12 16:54:47.829177 rico-0.3.2/tests/test__content.py
+-rw-r--r--   0        0        0    10803 2023-07-12 16:54:47.829177 rico-0.3.2/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-07-12 16:54:47.829177 rico-0.3.2/tests/test__version.py
+-rw-r--r--   0        0        0    18488 1970-01-01 00:00:00.000000 rico-0.3.2/PKG-INFO
```

### Comparing `rico-0.3.1/LICENSE` & `rico-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.3.1/README.md` & `rico-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,51 +18,29 @@
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
 
 ## Installation
 
-Install the core functionality:
 ```bash
 pip install rico
 ```
 
-The core functionality has no dependencies other than the standard Python packages. Optional additional dependencies are required to support the following content types:
-* Plots. Altair, Matplotlib Pyplot and Seaborn are currently supported.
-* Markdown.
+**rico** has no dependencies other than the standard Python packages.
 
-Install one or several extras to use plots or Markdown in HTML documents.
+### Deprecated
 
-[Altair](https://altair-viz.github.io/):
-```bash
-pip install rico[altair]
-```
+Optional additional dependencies were required to support the following content types:
+* Plots (`rico[altair]`, `rico[pyplot]`, `rico[seaborn]`).
+* Markdown (`rico[markdown]`).
 
-[Markdown](https://python-markdown.github.io/):
-```bash
-pip install rico[markdown]
-```
+The `rico[complete]` extra incudes all the dependencies above.
 
-[Matplotlib Pyplot](https://matplotlib.org/):
-```bash
-pip install rico[pyplot]
-```
-
-[Seaborn](https://seaborn.pydata.org/):
-```bash
-pip install rico[seaborn]
-```
-
-Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old Seaborn plotting functions return Matplotlib Pyplot Axes objects.
-
-All extras:
-```bash
-pip install rico[complete]
-```
+They are no longer needed and will be removed in version 0.4.0.
 
 ## User guide
 
 ### Basic usage
 
 **rico** provides both declarative and imperative style interfaces.
 
@@ -143,16 +121,16 @@
 * `indent_space = "  "`,
 * `strip_html = False`.
 
 ### Rich content types
 
 **rico** automatically recognizes the following content types:
 * `rico` content classes (subclasses of `rico.ContentBase`).
-* Plots (Altair, Matplotlib Pyplot, Seaborn).
-* Dataframes and other types with `_repr_html_` method.
+* Matplotlib Pyplot Plots.
+* Dataframes and other types with [IPython rich representation methods](https://ipython.readthedocs.io/en/stable/config/integrating.html).
 * Text.
 
 Use specific classes for plots and texts to change the default behavior:
 ```python
 doc = rico.Doc(
     rico.Text("Hello world!", mono=True),  # The default value is False.
     df,
@@ -174,18 +152,20 @@
 with rico.config_context(text_mono=True, image_format="png"):
     doc = rico.Doc("Hello world!", df, plot, title="My doc")
 ```
 
 Use specific classes and methods for other content types:
 * Images: `Image` or `Doc.append_image`.
 * Code: `Code` or `Doc.append_code`.
-* Markdown: `Markdown` or `Doc.append_markdown`.
+* Markdown*: `Markdown` or `Doc.append_markdown`.
 * HTML tag: `Tag` or `Doc.append_tag`.
 * Raw HTML: `HTML` or `Doc.append_html`.
 
+*Install [markdown-it-py](https://github.com/executablebooks/markdown-it-py) or [markdown](https://github.com/Python-Markdown/markdown/), or define a custom Markdown renderer with the `markdown_renderer` global option to use `Markdown` or `Doc.append_markdown`.
+
 For example:
 ```python
 doc = rico.Doc(
     rico.Markdown("## Dataframe"),
     df,
     rico.Tag("h2", "Plot"),  # An alternative way to add a header.
     plot,
@@ -375,14 +355,15 @@
 ```
 
 ### Global configuration
 
 Use global configuration to:
 * Get or set default parameter values.
 * Get or set document properties.
+* Get or set a markdown renderer method.
 
 The following global options define the default parameter values:
 
 | Global option    | Parameter | Classes, methods, functions       |
 |:-----------------|:----------|:----------------------------------|
 | `indent_html`    | `indent`  | `obj.serialize`, `serialize_html` |
 | `indent_space`   | `space`   | `obj.serialize`, `serialize_html` |
@@ -396,14 +377,19 @@
 The following global options define document properties:
 * `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata. Set it to `""` to disable.
 * `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata. Set it to `""` to disable.
 * `bootstrap_css` defines a link to the Bootstrap CSS file.
 * `bootstrap_js` defines a link to the Bootstrap JS file.
 * `dataframe_style` defines a dataframe style. Set it to `""` to disable.
 
+The `markdown_renderer` global option defines a callable that converts Markdown to HTML. It should accept a Markdown string as the first argument and return HTML as a string. The default value is defined as follows:
+* If the `markdown_it` module can be imported, then the default value is `markdown_it.MarkdownIt().render`.
+* Otherwise, if the `markdown` module can be imported, then the default value is `markdown.markdown`.
+* Otherwise, the default value is `None`. In this case, calling `rico.Markdown` or `obj.append_markdown` will throw an error.
+
 Get a dictionary with global options using `get_config` without parameters:
 ```python
 global_config = rico.get_config()
 print(global_config["indent_html"])
 # False
 ```
```

### Comparing `rico-0.3.1/pyproject.toml` & `rico-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.3.1"
+version = "0.3.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
@@ -61,14 +61,16 @@
 lint = [
     "ruff",
     "pyright",
 ]
 test = [
     "pytest",
     "coverage[toml]",
+    "markdown-it-py",
+    "markdown",
 ]
 
 [tool.pdm.scripts]
 test = "coverage run -m pytest"
 lint = "ruff check ."
 type = "pyright"
```

### Comparing `rico-0.3.1/src/rico/__init__.py` & `rico-0.3.2/src/rico/__init__.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.1/src/rico/_config.py` & `rico-0.3.2/src/rico/_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 
 import contextlib
 import textwrap
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
-    from collections.abc import Generator
+    from collections.abc import Callable, Generator
     from typing import Any, Literal
 
 
+try:
+    import markdown_it
+    md_renderer = markdown_it.MarkdownIt().render
+except ImportError:
+    try:
+        import markdown
+        md_renderer = markdown.markdown
+    except ImportError:
+        md_renderer = None
+
+
 BOOTSTRAP_VER = "5"
 BOOTSTRAP_CSS= f"https://cdn.jsdelivr.net/npm/bootstrap@{BOOTSTRAP_VER}/dist/css/bootstrap.min.css"
 BOOTSTRAP_JS = f"https://cdn.jsdelivr.net/npm/bootstrap@{BOOTSTRAP_VER}/dist/js/bootstrap.min.js"
 
 DATAFRAME_STYLE = textwrap.dedent("""\
     .dataframe table {
         border: none;
@@ -55,14 +66,15 @@
     "bootstrap_js": BOOTSTRAP_JS,
     "dataframe_style": DATAFRAME_STYLE,
     "image_format": "svg",
     "indent_html": False,
     "indent_space": "  ",
     "inline_scripts": False,
     "inline_styles": False,
+    "markdown_renderer": md_renderer,
     "meta_charset": "utf-8",
     "meta_viewport": "width=device-width, initial-scale=1",
     "strip_html": False,
     "text_mono": False,
     "text_wrap": False,
 }
 
@@ -87,14 +99,15 @@
     bootstrap_js: str | None = None,
     dataframe_style: str | None = None,
     image_format: Literal["svg", "png"] | None = None,
     indent_html: bool | None = None,
     indent_space: str | None = None,
     inline_scripts: bool | None = None,
     inline_styles: bool | None = None,
+    markdown_renderer: Callable[..., str] | None = None,
     meta_charset: str | None = None,
     meta_viewport: str | None = None,
     strip_html: bool | None = None,
     text_mono: bool | None = None,
     text_wrap: bool | None = None,
 ) -> None:
     """Set global configuration.
@@ -110,14 +123,17 @@
             If True, indent the elements.
         indent_space: Default value of the `space` parameter for serialization methods.
             Whitespace for indentation.
         inline_scripts: Default value of the `inline` parameter of the Script class.
             If True, load script inline, downdload it from source link.
         inline_styles: Default value of the `inline` parameter of the Style class.
             If True, load stylesheet inline, downdload it from source link.
+        markdown_renderer: A callable that converts Markdown to HTML.
+            Should accept a Markdown string as the first argument and
+            return HTML as a string.
         meta_charset: HTML document charset. If empty, then it's not used.
         meta_viewport: HTML document viewport property. If empty, then it's not used.
         strip_html: Default value of the `strip` parameter for serialization methods.
             If True, strip unnecessary whitespace.
         text_mono: Default value of the `mono` parameter of the Text class.
             If True, set the text font to monospaced.
         text_wrap: Default value of the `wrap` parameter of the Text class.
@@ -134,14 +150,15 @@
     bootstrap_js: str | None = None,
     dataframe_style: str | None = None,
     image_format: Literal["svg", "png"] | None = None,
     indent_html: bool | None = None,
     indent_space: str | None = None,
     inline_scripts: bool | None = None,
     inline_styles: bool | None = None,
+    markdown_renderer: Callable[..., str] | None = None,
     meta_charset: str | None = None,
     meta_viewport: str | None = None,
     strip_html: bool | None = None,
     text_mono: bool | None = None,
     text_wrap: bool | None = None,
 ) -> Generator[None, Any, None]:
     """Context manager for configuration.
@@ -157,14 +174,17 @@
             If True, indent the elements.
         indent_space: Default value of the `space` parameter for serialization methods.
             Whitespace for indentation.
         inline_scripts: Default value of the `inline` parameter of the Script class.
             If True, load script inline, downdload it from source link.
         inline_styles: Default value of the `inline` parameter of the Style class.
             If True, load stylesheet inline, downdload it from source link.
+        markdown_renderer: A callable that converts Markdown to HTML.
+            Should accept a Markdown string as the first argument and
+            return HTML as a string.
         meta_charset: HTML document charset. If empty, then it's not used.
         meta_viewport: HTML document viewport property. If empty, then it's not used.
         strip_html: Default value of the `strip` parameter for serialization methods.
             If True, strip unnecessary whitespace.
         text_mono: Default value of the `mono` parameter of the Text class.
             If True, set the text font to monospaced.
         text_wrap: Default value of the `wrap` parameter of the Text class.
```

### Comparing `rico-0.3.1/src/rico/_container.py` & `rico-0.3.2/src/rico/_container.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,25 @@
         **kwargs: P.kwargs,
     ) -> None:
         content = content_type(*args, **kwargs)
         self.container.append(content.container)
 
     return method
 
-
-class Div(rico._content.ContentBase):
+class Div(rico._content.Obj):
     def __init__(self, *objects: Any, class_: str | None = None):
         """Create a <div> container, create HTML elements and add them to the container.
 
         Each HTML element is also wrapped in a separate <div> container.
 
         Args:
             *objects: Objects that are used to create HTML elements.
             class_: The container class attribute.
         """
-        super().__init__(class_=class_)
-        for obj in objects:
-            if isinstance(obj, rico._content.ContentBase):
-                self.container.append(obj.container)
-            else:
-                self.container.append(rico._content.Obj(obj).container)
+        super().__init__(*objects, class_=class_)
 
     append_tag = _append(rico._content.Tag, rico._content.Tag.__init__)
     append_text = _append(rico._content.Text, rico._content.Text.__init__)
     append_code = _append(rico._content.Code, rico._content.Code.__init__)
     append_html = _append(rico._content.HTML, rico._content.HTML.__init__)
     append_markdown = _append(rico._content.Markdown, rico._content.Markdown.__init__)
     append_image = _append(rico._content.Image, rico._content.Image.__init__)
```

### Comparing `rico-0.3.1/src/rico/_content.py` & `rico-0.3.2/src/rico/_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,34 @@
 
 from __future__ import annotations
 
 import base64
 import io
 from typing import TYPE_CHECKING
 import urllib.request
+import warnings
 import xml.etree.ElementTree as ET
 
 import rico._config
 import rico._html
 
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
+    _ReprResult = str | bytes | dict[str, str | bytes]
+
 
 try:
     import altair as alt
     import vl_convert as vlc
 except ImportError:
     alt = None
 
 try:
-    import markdown
-except ImportError:
-    markdown = None
-
-try:
     import matplotlib.pyplot as plt
 except ImportError:
     plt = None
 
 try:
     import seaborn.objects as so
 except ImportError:
@@ -200,20 +198,21 @@
 
         Args:
             text: The Markdown text.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to the `markdown.markdown` function.
 
         Raises:
-            ImportError: The markdown package is not installed.
+            RuntimeError: The markdown renderer is not defined.
         """
-        if markdown is None:
-            raise ImportError("The markdown package is not installed.")
+        md_renderer = rico._config.get_config("markdown_renderer")
+        if md_renderer is None:
+            raise RuntimeError("The markdown renderer is not defined.")
 
-        content = HTML(markdown.markdown(text, **kwargs), class_=class_)
+        content = HTML(md_renderer(text, **kwargs), class_=class_)
         self.container = content.container
 
 
 class Image(ContentBase):
     def __init__(
         self,
         data: bytes | str,
@@ -249,17 +248,22 @@
         format: Literal["svg", "png"] | None = None,  # noqa: A002
         class_: str | None = None,
         **kwargs: Any,
     ):
         """Create an HTML element from a plot object and wrap it in a <div> container.
 
         The supported plot types are the following:
-        - Altair Chart,
-        - Pyplot Axes and Figure,
-        - Seaborn Plot (seaborn.objects interface).
+        - Matplotlib Pyplot Axes and Figure,
+        - [Deprecated] Altair Chart,
+        - [Deprecated] Seaborn Plot (seaborn.objects interface).
+
+        Deprecated:
+            Support of the Seaborn plots in this class/method is deprecated
+            and will be removed in version 0.4.0.
+            Use the rico.Obj or obj.append indstead.
 
         Args:
             obj: The plot object.
             format: Image format.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to the function
                 which converts the object to an image.
@@ -275,18 +279,32 @@
             obj = obj.figure
 
         if plt is not None and isinstance(obj, plt.Figure):  # type: ignore
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.savefig(stream, format=format, **kwargs)
             image = stream.getvalue()
         elif so is not None and isinstance(obj, so.Plot):
+            warnings.warn(
+                "Support of the Seaborn plots in this class/method is deprecated "
+                    "and will be removed in version 0.4.0. "
+                    "Use the rico.Obj or obj.append indstead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.save(stream, format=format, **kwargs)
             image = stream.getvalue()
         elif alt is not None and isinstance(obj, alt.TopLevelMixin):
+            warnings.warn(
+                "Support of the Altair plots in this class/method is deprecated "
+                    "and will be removed in version 0.4.0. "
+                    "Use the rico.Obj or obj.append indstead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
             convert = vlc.vegalite_to_svg if format == "svg" else vlc.vegalite_to_png  # type: ignore  # noqa: E501
             image = convert(  # type: ignore
                 obj.to_json(),  # type: ignore
                 vl_version="_".join(alt.SCHEMA_VERSION.split(".")[:2]),
                 **kwargs,
             )
         else:
@@ -299,51 +317,14 @@
         mime_subtype = "svg+xml" if format == "svg" else format
         content = Image(data=image, mime_subtype=mime_subtype, class_=class_)  # type: ignore  # noqa: E501
         self.container = content.container
 
 Chart = Plot
 
 
-class Obj(ContentBase):
-    def __init__(self, *objects: Any, class_: str | None = None):
-        """Create HTML elements from objects and wrap them in a <div> container.
-
-        Automatically determines the content type in the following order:
-        1. `rico` content classes (subclasses of `ContentBase`).
-        2. Plots.
-        3. Dataframes and other types with `_repr_html_` method.
-        4. Text.
-        All other types are converted to text.
-
-        Args:
-            *objects: The objects.
-            class_: The container class attribute.
-        """
-        super().__init__(class_=class_)
-        for obj in objects:
-            if isinstance(obj, ContentBase):
-                elements = (obj.container,)
-            elif (
-                alt is not None and isinstance(obj, alt.TopLevelMixin) or
-                plt is not None and isinstance(obj, plt.Axes | plt.Figure) or  # type: ignore  # noqa: E501
-                so is not None and isinstance(obj, so.Plot)
-            ):
-                elements = Plot(obj).container
-            elif hasattr(obj, "_repr_html_") and callable(obj._repr_html_):
-                elements = HTML(
-                    obj._repr_html_(),
-                    strip_dataframe_borders=True,
-                ).container
-            else:
-                elements = Text(obj).container
-
-            for element in elements:
-                self.container.append(element)
-
-
 class Script(ContentBase):
     footer: bool = False
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
@@ -441,7 +422,89 @@
             if "rel" not in attrib:
                 attrib = {**attrib, "rel": "stylesheet"}
         else:
             tag = "style"
 
         self.container = ET.Element(tag, {**attrib, **extra})
         self.container.text = text
+
+
+def _call_repr(
+    obj: Any,
+    repr_name: str,
+    mime_type: str = "text/plain",
+) -> dict[str, str | bytes]:
+    if hasattr(obj, repr_name):
+        repr_fn = getattr(obj, repr_name)
+        if callable(repr_fn):
+            data : _ReprResult | tuple[_ReprResult, _ReprResult] | None = repr_fn()
+            if isinstance(data, tuple):
+                data = data[0]
+            if data is None:
+                return {}
+            if not isinstance(data, dict):
+                return {mime_type: data}
+            return data
+    return {}
+
+def _decode(data: str | bytes) -> str:
+    return data.decode() if isinstance(data, bytes) else data
+
+def _get_repr(obj: Any) -> ET.Element:  # noqa: C901, PLR0911, PLR0912
+    data = _call_repr(obj, "_repr_mimebundle_")
+    if data == {}:
+        data = _call_repr(obj, "_repr_javascript_", "application/javascript")
+    if data == {}:
+        data = _call_repr(obj, "_repr_html_", "text/html")
+    if data == {}:
+        data = _call_repr(obj, "_repr_markdown_", "text/markdown")
+    if data == {}:
+        data = _call_repr(obj, "_repr_svg_", "image/svg+xml")
+    if data == {}:
+        data = _call_repr(obj, "_repr_png_", "image/png")
+    if data == {}:
+        data = _call_repr(obj, "_repr_jpeg_", "image/jpeg")
+
+    if "application/javascript" in data and data["application/javascript"]:
+        return Script(_decode(data["application/javascript"])).container
+    if "text/html" in data and data["text/html"]:
+        return HTML(_decode(data["text/html"]), strip_dataframe_borders=True).container
+    if "text/markdown" in data and data["text/markdown"]:
+        return Markdown(_decode(data["text/markdown"])).container
+    if "image/svg+xml" in data and data["image/svg+xml"]:
+        return Image(data["image/svg+xml"], "svg+xml").container
+    if "image/png" in data and data["image/png"]:
+        return Image(data["image/png"], "png").container
+    if "image/jpeg" in data and data["image/jpeg"]:
+        return Image(data["image/jpeg"], "jpeg").container
+    if "image/gif" in data and data["image/gif"]:
+        return Image(data["image/gif"], "gif").container
+    if "text/plain" in data and data["text/plain"]:
+        return Text(data["text/plain"]).container
+    return Text(str(obj)).container
+
+class Obj(ContentBase):
+    def __init__(self, *objects: Any, class_: str | None = None):
+        """Create HTML elements from objects and wrap them in a <div> container.
+
+        Automatically determines the content type in the following order:
+        1. `rico` content classes (subclasses of `ContentBase`).
+        2. Matplotlib Pyplot.
+        3. Dataframes and other types IPython rich replresentation methods.
+        All other types are converted to text.
+
+        More about IPython rich representation methods:
+        https://ipython.readthedocs.io/en/stable/config/integrating.html
+
+        Args:
+            *objects: The objects.
+            class_: The container class attribute.
+        """
+        super().__init__(class_=class_)
+        for obj in objects:
+            if isinstance(obj, ContentBase):
+                container = obj.container
+            elif plt is not None and isinstance(obj, plt.Axes | plt.Figure):  # type: ignore  # noqa: E501
+                container = Plot(obj).container
+            else:
+                container = _get_repr(obj)
+            self.container.append(container)
```

### Comparing `rico-0.3.1/src/rico/_html.py` & `rico-0.3.2/src/rico/_html.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.1/tests/test__container.py` & `rico-0.3.2/tests/test__container.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
 def test_div_append_plot(div_container: rico._container.Div):
     div_container.append_plot(altair_chart)
     content = rico._content.Plot(altair_chart)
     assert str(div_container) == f"<div>{content}</div>"
 
 
 def test_div_append(div_container: rico._container.Div):
-    div_container.append("Hello world", altair_chart)
-    content = rico._content.Obj("Hello world", altair_chart)
+    div_container.append("Hello world")
+    content = rico._content.Obj("Hello world")
     assert str(div_container) == f"<div>{content}</div>"
 
 
 def test_doc_init_default():  # noqa: PLR0915
     doc = rico._container.Doc("Hello world")
 
     html = doc.html
```

### Comparing `rico-0.3.1/tests/test__html.py` & `rico-0.3.2/tests/test__html.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.1/tests/test__version.py` & `rico-0.3.2/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.1/PKG-INFO` & `rico-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package for creating HTML documents from rich content: dataframes, plots, images, markdown etc. It provides a high-level, easy-to-use API with reasonable defaults, as well as low-level access for better control.
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -54,51 +54,29 @@
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
 
 ## Installation
 
-Install the core functionality:
 ```bash
 pip install rico
 ```
 
-The core functionality has no dependencies other than the standard Python packages. Optional additional dependencies are required to support the following content types:
-* Plots. Altair, Matplotlib Pyplot and Seaborn are currently supported.
-* Markdown.
+**rico** has no dependencies other than the standard Python packages.
 
-Install one or several extras to use plots or Markdown in HTML documents.
+### Deprecated
 
-[Altair](https://altair-viz.github.io/):
-```bash
-pip install rico[altair]
-```
+Optional additional dependencies were required to support the following content types:
+* Plots (`rico[altair]`, `rico[pyplot]`, `rico[seaborn]`).
+* Markdown (`rico[markdown]`).
 
-[Markdown](https://python-markdown.github.io/):
-```bash
-pip install rico[markdown]
-```
+The `rico[complete]` extra incudes all the dependencies above.
 
-[Matplotlib Pyplot](https://matplotlib.org/):
-```bash
-pip install rico[pyplot]
-```
-
-[Seaborn](https://seaborn.pydata.org/):
-```bash
-pip install rico[seaborn]
-```
-
-Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old Seaborn plotting functions return Matplotlib Pyplot Axes objects.
-
-All extras:
-```bash
-pip install rico[complete]
-```
+They are no longer needed and will be removed in version 0.4.0.
 
 ## User guide
 
 ### Basic usage
 
 **rico** provides both declarative and imperative style interfaces.
 
@@ -179,16 +157,16 @@
 * `indent_space = "  "`,
 * `strip_html = False`.
 
 ### Rich content types
 
 **rico** automatically recognizes the following content types:
 * `rico` content classes (subclasses of `rico.ContentBase`).
-* Plots (Altair, Matplotlib Pyplot, Seaborn).
-* Dataframes and other types with `_repr_html_` method.
+* Matplotlib Pyplot Plots.
+* Dataframes and other types with [IPython rich representation methods](https://ipython.readthedocs.io/en/stable/config/integrating.html).
 * Text.
 
 Use specific classes for plots and texts to change the default behavior:
 ```python
 doc = rico.Doc(
     rico.Text("Hello world!", mono=True),  # The default value is False.
     df,
@@ -210,18 +188,20 @@
 with rico.config_context(text_mono=True, image_format="png"):
     doc = rico.Doc("Hello world!", df, plot, title="My doc")
 ```
 
 Use specific classes and methods for other content types:
 * Images: `Image` or `Doc.append_image`.
 * Code: `Code` or `Doc.append_code`.
-* Markdown: `Markdown` or `Doc.append_markdown`.
+* Markdown*: `Markdown` or `Doc.append_markdown`.
 * HTML tag: `Tag` or `Doc.append_tag`.
 * Raw HTML: `HTML` or `Doc.append_html`.
 
+*Install [markdown-it-py](https://github.com/executablebooks/markdown-it-py) or [markdown](https://github.com/Python-Markdown/markdown/), or define a custom Markdown renderer with the `markdown_renderer` global option to use `Markdown` or `Doc.append_markdown`.
+
 For example:
 ```python
 doc = rico.Doc(
     rico.Markdown("## Dataframe"),
     df,
     rico.Tag("h2", "Plot"),  # An alternative way to add a header.
     plot,
@@ -411,14 +391,15 @@
 ```
 
 ### Global configuration
 
 Use global configuration to:
 * Get or set default parameter values.
 * Get or set document properties.
+* Get or set a markdown renderer method.
 
 The following global options define the default parameter values:
 
 | Global option    | Parameter | Classes, methods, functions       |
 |:-----------------|:----------|:----------------------------------|
 | `indent_html`    | `indent`  | `obj.serialize`, `serialize_html` |
 | `indent_space`   | `space`   | `obj.serialize`, `serialize_html` |
@@ -432,14 +413,19 @@
 The following global options define document properties:
 * `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata. Set it to `""` to disable.
 * `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata. Set it to `""` to disable.
 * `bootstrap_css` defines a link to the Bootstrap CSS file.
 * `bootstrap_js` defines a link to the Bootstrap JS file.
 * `dataframe_style` defines a dataframe style. Set it to `""` to disable.
 
+The `markdown_renderer` global option defines a callable that converts Markdown to HTML. It should accept a Markdown string as the first argument and return HTML as a string. The default value is defined as follows:
+* If the `markdown_it` module can be imported, then the default value is `markdown_it.MarkdownIt().render`.
+* Otherwise, if the `markdown` module can be imported, then the default value is `markdown.markdown`.
+* Otherwise, the default value is `None`. In this case, calling `rico.Markdown` or `obj.append_markdown` will throw an error.
+
 Get a dictionary with global options using `get_config` without parameters:
 ```python
 global_config = rico.get_config()
 print(global_config["indent_html"])
 # False
 ```
```

