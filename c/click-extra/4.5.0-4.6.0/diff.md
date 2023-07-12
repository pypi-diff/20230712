# Comparing `tmp/click_extra-4.5.0.tar.gz` & `tmp/click_extra-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.5.0.tar", max compression
+gzip compressed data, was "click_extra-4.6.0.tar", max compression
```

## Comparing `click_extra-4.5.0.tar` & `click_extra-4.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6017 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/__init__.py
--rw-r--r--   0        0        0    27922 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/colorize.py
--rw-r--r--   0        0        0    15310 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/commands.py
--rw-r--r--   0        0        0    15776 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/config.py
--rw-r--r--   0        0        0     4014 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6211 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11874 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/logging.py
--rw-r--r--   0        0        0    23477 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/parameters.py
--rw-r--r--   0        0        0    17118 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/py.typed
--rw-r--r--   0        0        0     7685 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     6038 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2542 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11164 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    17922 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    12920 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    16315 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7290 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    14371 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8406 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14478 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     6311 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2613 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/timer.py
--rw-r--r--   0        0        0    10988 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/version.py
--rw-r--r--   0        0        0     7490 2023-07-06 06:50:43.871600 click_extra-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     6631 2023-07-06 06:50:43.871600 click_extra-4.5.0/readme.md
--rw-r--r--   0        0        0     9675 1970-01-01 00:00:00.000000 click_extra-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     6104 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    30238 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    16715 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/commands.py
+-rw-r--r--   0        0        0    16405 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6211 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11805 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/logging.py
+-rw-r--r--   0        0        0    25392 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7676 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5969 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11504 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    18365 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    15075 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    17059 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7354 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    18184 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8396 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14491 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     6359 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2544 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/timer.py
+-rw-r--r--   0        0        0    10995 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/version.py
+-rw-r--r--   0        0        0     7584 2023-07-12 16:24:52.186848 click_extra-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-07-12 16:24:52.186848 click_extra-4.6.0/readme.md
+-rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.0/PKG-INFO
```

### Comparing `click_extra-4.5.0/click_extra/__init__.py` & `click_extra-4.6.0/click_extra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.5.0"
+__version__ = "4.6.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -50,42 +50,42 @@
 
 # Import all click's module-level content to allow for drop-in replacement.
 # XXX Star import is really badly supported by mypy for now and leads to lots of
 # "Module 'XXX' has no attribute 'YYY'". See: https://github.com/python/mypy/issues/4930
 # Overrides click helpers with cloup's.
 from click import *  # noqa: E402, F403
 from click.core import ParameterSource  # noqa: E402
-from cloup import *  # type: ignore[no-redef] # noqa: E402, F403
+from cloup import *  # type: ignore[no-redef, assignment] # noqa: E402, F403
 
 from .colorize import (  # noqa: E402
     ColorOption,
     HelpExtraFormatter,
     HelpExtraTheme,
     HelpOption,
 )
 from .commands import (  # noqa: E402
     ExtraCommand,
     ExtraContext,
     ExtraGroup,
 )
 from .config import ConfigOption  # noqa: E402
-from .decorators import (  # type: ignore[no-redef] # noqa: E402
+from .decorators import (  # type: ignore[no-redef, has-type] # noqa: E402
     color_option,
     command,
     config_option,
     extra_command,
     extra_group,
+    extra_version_option,
     group,
     help_option,
     show_params_option,
     table_format_option,
     telemetry_option,
     timer_option,
     verbosity_option,
-    version_option,
 )
 from .logging import (  # noqa: E402
     ExtraLogFormatter,
     ExtraLogHandler,
     VerbosityOption,
     extra_basic_config,
 )
@@ -95,15 +95,15 @@
     ShowParamsOption,
     search_params,
 )
 from .tabulate import TableFormatOption  # noqa: E402
 from .telemetry import TelemetryOption  # noqa: E402
 from .testing import ExtraCliRunner  # noqa: E402
 from .timer import TimerOption  # noqa: E402
-from .version import VersionOption  # noqa: E402
+from .version import ExtraVersionOption  # noqa: E402
 
 __all__ = [  # noqa: F405
     "Abort",
     "Argument",
     "argument",
     "BadArgumentUsage",
     "BadOptionUsage",
@@ -137,21 +137,23 @@
     "dir_path",
     "echo",
     "echo_via_pager",
     "edit",
     "extra_basic_config",
     "extra_command",
     "extra_group",
+    "extra_version_option",
     "ExtraCliRunner",
     "ExtraCommand",
     "ExtraContext",
     "ExtraGroup",
     "ExtraLogFormatter",
     "ExtraLogHandler",
     "ExtraOption",
+    "ExtraVersionOption",
     "File",
     "file_path",
     "FileError",
     "FLOAT",
     "FloatRange",
     "format_filename",
     "get_app_dir",
```

### Comparing `click_extra-4.5.0/click_extra/colorize.py` & `click_extra-4.6.0/click_extra/colorize.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from cloup.styling import Color, IStyle
 from cloup.typing import MISSING, Possibly
 
 from . import (
     Choice,
     Context,
     HelpFormatter,
+    Option,
     Parameter,
     ParameterSource,
     Style,
     cache,
     echo,
     get_current_context,
 )
@@ -51,14 +52,18 @@
     .. caution::
         We had to redefined all fields and couldn't extend ``cloup.HelpTheme`` as there
         is no way to cleanly do it with MyPy.
 
         See:
         - https://github.com/python/typing/issues/427
         - https://mypy.readthedocs.io/en/stable/runtime_troubles.html#future-annotations-import-pep-563
+
+    .. todo::
+        This is being `discussed upstream at janluke/cloup#159
+        <https://github.com/janluke/cloup/issues/159>`_.
     """
 
     invoked_command: IStyle = identity
     command_help: IStyle = identity
     heading: IStyle = identity
     constraint: IStyle = identity
     section_help: IStyle = identity
@@ -313,62 +318,95 @@
             expose_value=expose_value,
             help=help,
             **kwargs,
         )
 
 
 class HelpOption(ExtraOption):
-    @staticmethod
-    def print_help(ctx: Context, param: Parameter, value: bool) -> None:
-        """Prints help text and exits."""
-        if not value or ctx.resilient_parsing:
-            return
-
-        echo(ctx.get_help(), color=ctx.color)
-
-        # Do not just ctx.exit() as it will prevent callbacks defined on options
-        # to be called.
-        ctx.close()
-        ctx.exit()
+    """Like Click's @help_option but made into a reusable class-based option.
+
+    .. note::
+        Keep implementation in sync with upstream for drop-in replacement
+        compatibility.
+
+    .. todo::
+        Reuse Click's ``HelpOption`` once this PR is merged:
+        https://github.com/pallets/click/pull/2563
+    """
 
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_("Show this message and exit."),
         **kwargs,
     ) -> None:
+        """Same defaults as Click's @help_option but with ``-h`` short option.
+
+        See: https://github.com/pallets/click/blob/d9af5cf/src/click/decorators.py#L563C23-L563C34
+        """
         if not param_decls:
             param_decls = ("--help", "-h")
 
         kwargs.setdefault("callback", self.print_help)
 
         super().__init__(
             param_decls=param_decls,
             is_flag=is_flag,
             expose_value=expose_value,
             is_eager=is_eager,
             help=help,
             **kwargs,
         )
 
+    @staticmethod
+    def print_help(ctx: Context, param: Parameter, value: bool) -> None:
+        """Prints help text and exits.
+
+        Exact same behavior as `Click's original @help_option callback
+        <https://github.com/pallets/click/blob/d9af5cf/src/click/decorators.py#L555-L560>`_,
+        but forces the closing of the context before exiting.
+        """
+        if value and not ctx.resilient_parsing:
+            echo(ctx.get_help(), color=ctx.color)
+            # Do not just ctx.exit() as it will prevent callbacks defined on options
+            # to be called.
+            ctx.close()
+            ctx.exit()
 
-class ExtraHelpColorsMixin:
-    """Adds extra-keywords highlighting to Click commands.
 
-    This mixin for ``click.core.Command``-like classes intercepts the top-level helper-
-    generation method to initialize the formatter with dynamic settings.
+class ExtraHelpColorsMixin:  # (Command)??
+    """Adds extra-keywords highlighting to Click commands.
 
-    This is implemented here to get access to the global context.
+    This mixin for ``click.Command``-like classes intercepts the top-level helper-
+    generation method to initialize the formatter with dynamic settings. This is
+    implemented at this stage so we have access to the global context.
     """
 
-    def collect_keywords(self, ctx):
-        """Parse click context to collect option names, choices and metavar keywords."""
+    def _collect_keywords(
+        self,
+        ctx: Context,
+    ) -> tuple[
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+        set[str],
+    ]:
+        """Parse click context to collect option names, choices and metavar keywords.
+
+        This is Click Extra-specific and is not part of the upstream ``click.Command``
+        API.
+        """
         cli_names: set[str] = set()
         subcommands: set[str] = set()
         command_aliases: set[str] = set()
         options: set[str] = set()
         long_options: set[str] = set()
         short_options: set[str] = set()
         choices: set[str] = set()
@@ -382,15 +420,15 @@
 
         # Will fetch command's metavar (i.e. the "[OPTIONS]" after the CLI name in
         # "Usage:") and dig into subcommands to get subcommand_metavar:
         # ("COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...").
         metavars.update(command.collect_usage_pieces(ctx))
 
         # Get subcommands and their aliases.
-        if hasattr(command, "list_commands"):
+        if isinstance(command, click.MultiCommand):
             subcommands.update(command.list_commands(ctx))
             for sub_id in subcommands:
                 sub_cmd = command.get_command(ctx, sub_id)
                 command_aliases.update(getattr(sub_cmd, "aliases", []))
 
         # Add user defined help options.
         options.update(ctx.help_option_names)
@@ -401,15 +439,19 @@
             options.update(param.secondary_opts)
 
             if isinstance(param.type, Choice):
                 choices.update(param.type.choices)
 
             metavars.add(param.make_metavar())
 
-            envvars.update(param.envvar)
+            if param.envvar:
+                if isinstance(param.envvar, str):
+                    envvars.add(param.envvar)
+                else:
+                    envvars.update(param.envvar)
 
             if isinstance(param, click.Option):
                 default_string = ExtraOption.get_help_default(param, ctx)
                 if default_string:
                     defaults.add(default_string)
 
         # Split between shorts and long options
@@ -437,43 +479,58 @@
             short_options,
             choices,
             metavars,
             envvars,
             defaults,
         )
 
-    def get_help(self, ctx):
+    def get_help_option(self, ctx: Context) -> Option | None:
+        """Returns our custom help option object instead of Click's default one."""
+        # Let Click generate the default help option or not.
+        help_option = super().get_help_option(ctx)  # type: ignore[misc]
+        # If Click decided to not add a default help option, we don't either.
+        if not help_option:
+            return None
+        # Return our own help option.
+        return HelpOption(param_decls=help_option.opts)
+
+    def get_help(self, ctx: Context) -> str:
         """Replace default formatter by our own."""
         ctx.formatter_class = HelpExtraFormatter
-        return super().get_help(ctx)
+        return super().get_help(ctx)  # type: ignore[no-any-return,misc]
 
-    def format_help(self, ctx, formatter):
+    def format_help(self, ctx: Context, formatter: HelpExtraFormatter) -> None:
         """Feed our custom formatter instance with the keywords to highlight."""
         (
             formatter.cli_names,
             formatter.subcommands,
             formatter.command_aliases,
             formatter.long_options,
             formatter.short_options,
             formatter.choices,
             formatter.metavars,
             formatter.envvars,
             formatter.defaults,
-        ) = self.collect_keywords(ctx)
-        return super().format_help(ctx, formatter)
+        ) = self._collect_keywords(ctx)
+        super().format_help(ctx, formatter)  # type: ignore[misc]
 
 
 def escape_for_help_screen(text: str) -> str:
-    """Escape a text to be used in a regular expression to match help screen.
+    """Prepares a string to be used in a regular expression for matches in help screen.
 
-    Like ``re.escape``, but allows any number of optional blank characters (line
-    returns, spaces, tabs) after a dash, to accounts for text wrapping rules and
-    columnar layout.
+    Applies `re.escape <https://docs.python.org/3/library/re.html#re.escape>`_, then
+    accounts for long strings being wrapped on multiple lines and padded with spaces to
+    fit the columnar layout.
+
+    It allows for:
+    - additional number of optional blank characters (line-returns, spaces, tabs, ...)
+      after a dash, as the help renderer is free to wrap strings after a dash.
+    - a space to be replaced by any number of blank characters.
     """
-    return re.escape(text).replace("-", "-\\s*")
+    return re.escape(text).replace("-", "-\\s*").replace("\\ ", "\\s+")
 
 
 class HelpExtraFormatter(HelpFormatter):
     """Extends Cloup's custom HelpFormatter to highlights options, choices, metavars and
     default values.
 
     This is being discussed for upstream integration at:
@@ -503,15 +560,15 @@
     long_options: set[str] = set()
     short_options: set[str] = set()
     choices: set[str] = set()
     metavars: set[str] = set()
     envvars: set[str] = set()
     defaults: set[str] = set()
 
-    # TODO: Hihglight extra keywords <stdout> or <stderr>
+    # TODO: Highlight extra keywords <stdout> or <stderr>
 
     # TODO: add collection of regexps as pre-compiled constants, so we can
     # inspect them and get some performances improvements.
 
     style_aliases = {
         # Layout elements of the square brackets trailing each option.
         "bracket_1": "bracket",
```

### Comparing `click_extra-4.5.0/click_extra/commands.py` & `click_extra-4.6.0/click_extra/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,52 +19,89 @@
 counterparts, but are pre-configured with good and common defaults. You can still
 leverage the mixins in here to build up your own custom variants.
 """
 
 from __future__ import annotations
 
 import logging
-from typing import Any
+from typing import Any, cast
 
 import click
 import cloup
 
 from . import Command, Group
-from .colorize import ColorOption, ExtraHelpColorsMixin, HelpOption
+from .colorize import ColorOption, ExtraHelpColorsMixin, HelpExtraFormatter, HelpOption
 from .config import ConfigOption
 from .logging import VerbosityOption
 from .parameters import (
     ExtraOption,
     ShowParamsOption,
     all_envvars,
     normalize_envvar,
     search_params,
 )
 from .timer import TimerOption
-from .version import VersionOption
+from .version import ExtraVersionOption
 
 
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
     ``meta`` property at instantiation.
+
+    Also inherits ``color`` property from parent context. And sets it to `True` for
+    parentless contexts at instantiatiom, so we can always have colorized output.
+
+    .. todo::
+        Propose addition of ``meta`` keyword upstream to Click.
     """
 
-    _extra_meta: dict[str, Any] = {}
+    formatter_class = HelpExtraFormatter  # type: ignore[assignment]
+    """Use our own formatter to colorize the help screen."""
+
+    def __init__(self, *args, meta: dict[str, Any] | None = None, **kwargs) -> None:
+        """Like parent's context but with an extra ``meta`` keyword-argument.
 
-    def __init__(self, *args, meta: dict[str, Any] = {}, **kwargs) -> None:
-        """Like parent's context but with an extra ``meta`` keyword-argument."""
-        self._extra_meta = meta
+        Also force ``color`` property default to `True` if not provided by user and
+        this context has no parent.
+        """
         super().__init__(*args, **kwargs)
 
+        # Update the context's meta property with the one provided by user.
+        if meta:
+            self._meta.update(meta)
+
+        # Transfer user color setting to our internally managed value.
+        self._color: bool | None = kwargs.get("color", None)
+
+        # A Context created from scratch, i.e. without a parent, and whose color
+        # setting is set to auto-detect (i.e. is None), will defaults to forced
+        # colorized output.
+        if not self.parent and self._color is None:
+            self._color = True
+
     @property
-    def meta(self) -> dict[str, Any]:
-        """Returns context meta augmented with our own."""
-        meta = dict(self._meta)
-        meta.update(self._extra_meta)
-        return meta
+    def color(self) -> bool | None:
+        """Overrides ``Context.color`` to allow inheritance from parent context.
+
+        Returns the color setting of the parent context if it exists and the color is
+        not set on the current context.
+        """
+        if self._color is None and self.parent:
+            return self.parent.color
+        return self._color
+
+    @color.setter
+    def color(self, value: bool | None) -> None:
+        """Set the color value of the current context."""
+        self._color = value
+
+    @color.deleter
+    def color(self) -> None:
+        """Reset the color value so it defaults to inheritance from parent's."""
+        self._color = None
 
 
 def default_extra_params():
     """Default additional options added to ``extra_command`` and ``extra_group``.
 
     .. caution::
         The order of options has been carefully crafted to handle subtle edge-cases and
@@ -102,20 +139,20 @@
     """
     return [
         TimerOption(),
         ColorOption(),
         ConfigOption(),
         ShowParamsOption(),
         VerbosityOption(),
-        VersionOption(),
+        ExtraVersionOption(),
         HelpOption(),
     ]
 
 
-class ExtraCommand(ExtraHelpColorsMixin, Command):
+class ExtraCommand(ExtraHelpColorsMixin, Command):  # type: ignore[misc]
     """Like ``cloup.command``, with sane defaults and extra help screen colorization."""
 
     context_class: type[cloup.Context] = ExtraContext
 
     def __init__(
         self,
         *args,
@@ -123,41 +160,41 @@
         extra_option_at_end: bool = True,
         populate_auto_envvars: bool = True,
         **kwargs: Any,
     ) -> None:
         """List of extra parameters:
 
         :param version: allows a version string to be set directly on the command. Will
-            be passed to the first instance of ``VersionOption`` parameter attached to
-            the command.
+            be passed to the first instance of ``ExtraVersionOption`` parameter
+            attached to the command.
         :param extra_option_at_end: `reorders all parameters attached to the command
             <https://kdeldycke.github.io/click-extra/commands.html#option-order>`_, by
             moving all instances of ``ExtraOption`` at the end of the parameter list.
             The original order of the options is preserved among themselves.
         :param populate_auto_envvars: forces all parameters to have their auto-generated
             environment variables registered. This address the shortcoming of ``click``
             which only evaluates them dynamiccaly. By forcing their registration, the
             auto-generated environment variables gets displayed in the help screen,
             fixing `click#2483 issue <https://github.com/pallets/click/issues/2483>`_.
 
         By default, these `Click context settings
         <https://click.palletsprojects.com/en/8.1.x/api/#click.Context>`_ are applied:
 
-        - ``auto_envvar_prefix = self.name``
+        - ``auto_envvar_prefix = self.name`` (*Click feature*)
 
           Auto-generate environment variables for all options, using the command ID as
           prefix. The prefix is normalized to be uppercased and all non-alphanumerics
           replaced by underscores.
 
-        - ``help_option_names = ("--help", "-h")``
+        - ``help_option_names = ("--help", "-h")`` (*Click feature*)
 
           `Allow help screen to be invoked with either --help or -h options
           <https://click.palletsprojects.com/en/8.1.x/documentation/#help-parameter-customization>`_.
 
-        - ``show_default = True``
+        - ``show_default = True`` (*Click feature*)
 
           `Show all default values
           <https://click.palletsprojects.com/en/8.1.x/api/#click.Context.show_default>`_
           in help screen.
 
         Additionally, these `Cloup context settings
         <https://cloup.readthedocs.io/en/stable/pages/formatting.html#formatting-settings>`_
@@ -259,15 +296,15 @@
         self.context_settings: dict[str, Any] = default_ctx_settings
 
         if populate_auto_envvars:
             for param in self.params:
                 param.envvar = all_envvars(param, self.context_settings)
 
         if version:
-            version_param = search_params(self.params, VersionOption)
+            version_param = search_params(self.params, ExtraVersionOption)
             if version_param:
                 version_param.version = version  # type: ignore[union-attr]
 
         if extra_option_at_end:
             self.params.sort(key=lambda p: isinstance(p, ExtraOption))
 
         # Forces re-identification of grouped and non-grouped options as we re-ordered
@@ -304,25 +341,29 @@
             This workaround is being discussed upstream in `click#1279
             <https://github.com/pallets/click/issues/1279#issuecomment-1493348208>`_.
         """
         # ``args`` needs to be copied: its items are consumed by the parsing process.
         extra.update({"meta": {"click_extra.raw_args": args.copy()}})
         return super().make_context(info_name, args, parent, **extra)
 
-    def invoke(self, ctx):
+    def invoke(self, ctx: click.Context) -> Any:
         """Main execution of the command, just after the context has been instantiated
         in ``main()``.
 
-        If an instance of ``VersionOption`` is found attached to the command, print its
-        output in ``DEBUG`` logs. This facilitates troubleshooting of user's issues.
+        If an instance of ``ExtraVersionOption`` is found attached to the command,
+        print its output in ``DEBUG`` logs. This facilitates troubleshooting of user's
+        issues.
         """
         logger = logging.getLogger("click_extra")
         if logger.getEffectiveLevel() == logging.DEBUG:
             # Look for a ``--version`` parameter.
-            version_opt = search_params(ctx.command.params, VersionOption)
+            version_opt = cast(
+                "ExtraVersionOption | None",
+                search_params(ctx.command.params, ExtraVersionOption),
+            )
             if version_opt:
                 # Environment info is already present in the version string: use it
                 # as-is.
                 if "%(env_info)s" in version_opt.message:
                     msg = version_opt.render_message()
                 # Augments the version string with the environment info.
                 else:
@@ -334,41 +375,35 @@
                 for line in msg.splitlines():
                     # TODO: pretty print JSON output (easier to read in bug reports)?
                     logger.debug(line)
 
         return super().invoke(ctx)
 
 
-class ExtraGroup(ExtraCommand, Group):
+class ExtraGroup(ExtraCommand, Group):  # type: ignore[misc]
     """Same as ``cloup.group``, but with sane defaults and extra help screen
-    colorization.
-    """
+    colorization."""
+
+    command_class = ExtraCommand
+    """Makes commands of an ``ExtraGroup`` be instances of ``ExtraCommand``.
+
+    That way all subcommands created from an ``ExtraGroup`` benefits from the same
+    defaults and extra help screen colorization.
 
-    # XXX This simple override might be enough to replace the command() override below,
-    # but there is a bug in click that prevents this from working:
-    #   https://github.com/pallets/click/issues/2416
-    #   https://github.com/pallets/click/pull/2417
-    #
-    # command_class = ExtraCommand
+    Fixes `click-extra#479 <https://github.com/kdeldycke/click-extra/issues/479>`_.
+    """
 
     def command(self, *args, **kwargs):
-        """Returns a decorator that creates a new subcommand for this ``Group``.
+        """Bypass ``cloup.Group.command()`` to produce an ``ExtraCommand`` decorator.
 
-        This makes a command that is a :class:`~click_extra.command.ExtraCommand`
-        instead of a :class:`~cloup._command.Command` so by default all subcommands of
-        an ``ExtraGroup`` benefits from the same defaults and extra help screen
-        colorization.
+        Starts the seach for the ``command()`` method after the ``cloup.Group`` class
+        in the MRO chain, effectively bypassing ``cloup.Group.command()``, which does
+        not support the ``command_class`` property.
 
-        Fixes `click-extra#479 <https://github.com/kdeldycke/click-extra/issues/479>`_.
+        .. todo::
+            Removes this workaround when `Cloup issue #160 is addressed
+            <https://github.com/janluke/cloup/issues/160>`_.
 
         .. todo::
             Allow this decorator to be called without parenthesis.
         """
-        kwargs.setdefault("cls", ExtraCommand)
-        return super().command(*args, **kwargs)
-
-
-# -0, --zero-exit
-# rospector will exit with a code of 1 (one) if any messages are found. This makes
-# automation easier; if there are any problems at all, the exit code is non-zero.
-# However this behaviour is not always desirable, so if this flag is set, prospector
-# will exit with a code of 0 if it ran successfully, and non-zero if it failed to run.
+        return super(cloup.Group, self).command(*args, **kwargs)
```

### Comparing `click_extra-4.5.0/click_extra/config.py` & `click_extra-4.6.0/click_extra/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import logging
 import os
 import sys
 from configparser import ConfigParser, ExtendedInterpolation
 from enum import Enum
 from gettext import gettext as _
 from pathlib import Path
-from typing import Iterable, Sequence
+from typing import Any, Iterable, Sequence
 from unittest.mock import patch
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib  # type: ignore[import]
 
@@ -195,99 +195,107 @@
         matching pattern."""
         # Pre-compute pretty_path to bypass infinite recursive loop on get_default.
         pretty_path = shrinkuser(Path(self.get_default(ctx)))
         with patch.object(ConfigOption, "get_default") as mock_method:
             mock_method.return_value = pretty_path
             return super().get_help_record(ctx)
 
-    def search_and_read_conf(self, pattern: str) -> Iterable[str]:
+    def search_and_read_conf(self, pattern: str) -> Iterable[tuple[Path | URL, str]]:
         """Search on local file system or remote URL files matching the provided
         pattern.
 
-        ``pattern`` is considered as an URL only if it is parseable as such and starts
+        ``pattern`` is considered an URL only if it is parseable as such and starts
         with ``http://`` or ``https://``.
 
-        Returns an iterator of raw content for each file/URL matching the
-        pattern.
+        Returns an iterator of the normalized configuration location and its textual
+        content, for each file/URL matching the pattern.
         """
         logger = logging.getLogger("click_extra")
 
         # Check if the pattern is an URL.
         location = URL(pattern)
-        if location and location.scheme.lower() in ("http", "https"):
-            logger.debug("Fetch configuration from remote URL.")
+        location.normalize()
+        if location and location.scheme in ("http", "https"):
+            logger.debug(f"Download configuration from URL: {location}")
             with requests.get(location) as response:
                 if response.ok:
-                    yield from (response.text,)
+                    yield location, response.text
                     return
                 logger.warning(f"Can't download {location}: {response.reason}")
-        else:
-            logger.debug("Pattern is not an URL.")
 
-        logger.debug("Search local file system.")
+        logger.debug("Pattern is not an URL: search local file system.")
         # wcmatch expect patterns to be written with Unix-like syntax by default, even
         # on Windows. See more details at:
         # https://facelessuser.github.io/wcmatch/glob/#windows-separators
         # https://github.com/facelessuser/wcmatch/issues/194
         if is_windows():
             pattern = pattern.replace("\\", "/")
         for file in iglob(
             pattern,
             flags=NODIR | GLOBSTAR | DOTGLOB | GLOBTILDE | BRACE | FOLLOW | IGNORECASE,
         ):
-            file_path = Path(file)
+            file_path = Path(file).resolve()
             logger.debug(f"Configuration file found at {file_path}")
-            yield file_path.read_text()
+            yield file_path, file_path.read_text()
 
-    def parse_conf(self, conf_content: str) -> dict | None:
+    def parse_conf(self, conf_text: str) -> dict | None:
         """Try to parse the provided content with each format in the order provided by
         the user.
 
         A successful parsing in any format is supposed to return a ``dict``. Any other
         result, including any raised exception, is considered a failure and the next
         format is tried.
         """
+        logger = logging.getLogger("click_extra")
+
         user_conf = None
         for conf_format in self.formats:
-            logger = logging.getLogger("click_extra")
             logger.debug(f"Parse configuration as {conf_format.name}...")
 
             try:
                 if conf_format == Formats.TOML:
-                    user_conf = tomllib.loads(conf_content)
+                    user_conf = tomllib.loads(conf_text)
 
                 elif conf_format == Formats.YAML:
-                    user_conf = yaml.full_load(conf_content)
+                    user_conf = yaml.full_load(conf_text)
 
                 elif conf_format == Formats.JSON:
-                    user_conf = json.loads(conf_content)
+                    user_conf = json.loads(conf_text)
 
                 elif conf_format == Formats.INI:
-                    user_conf = self.load_ini_config(conf_content)
+                    user_conf = self.load_ini_config(conf_text)
 
                 elif conf_format == Formats.XML:
-                    user_conf = xmltodict.parse(conf_content)
+                    user_conf = xmltodict.parse(conf_text)
 
             except Exception as ex:
                 logger.debug(ex)
                 continue
 
             if isinstance(user_conf, dict):
                 return user_conf
             else:
                 logger.debug(f"{conf_format.name} parsing failed.")
 
         return None
 
-    def read_and_parse_conf(self, pattern: str) -> dict | None:
-        for conf_content in self.search_and_read_conf(pattern):
-            user_conf = self.parse_conf(conf_content)
+    def read_and_parse_conf(
+        self,
+        pattern: str,
+    ) -> tuple[Path | URL, dict[str, Any]] | tuple[None, None]:
+        """Search for a configuration file matching the provided pattern.
+
+        Returns the location and parsed content of the first valid configuration file
+        that is not blank, or `(None, None)` if no file was found.
+        """
+        for conf_path, conf_text in self.search_and_read_conf(pattern):
+            user_conf = self.parse_conf(conf_text)
             if user_conf is not None:
-                return user_conf
-        return None
+                return conf_path, user_conf
+        return None, None
 
     def load_ini_config(self, content):
         """Utility method to parse INI configuration file.
 
         Internal convention is to use a dot (``.``, as set by ``self.SEP``) in
         section IDs as a separator between levels. This is a workaround
         the limitation of ``INI`` format which doesn't allow for sub-sections.
@@ -351,84 +359,86 @@
             elif k in a:
                 a[k] = b[k]
             elif self.strict:
                 msg = f"Parameter {k!r} is not allowed in configuration file."
                 raise ValueError(msg)
         return a
 
-    def merge_conf(self, user_conf):
-        """Try-out configuration formats against file's content and returns a ``dict``.
+    def merge_default_map(self, ctx, user_conf):
+        """Save the user configuration into the context's ``default_map``.
 
-        The returned ``dict`` will only contain options and parameters defined on the
-        CLI. All others will be filtered out.
+        Merge the user configuration into the pre-computed template structure, which
+        will filter out all unrecognized options not supported by the command. Then
+        cleans up blank values and update the context's ``default_map``.
         """
-        # Merge configuration file's content into the template structure, but
-        # ignore all unrecognized options.
-        valid_conf = self.recursive_update(self.params_template, user_conf)
-
-        # Clean-up blank values left-over by the template structure.
+        filtered_conf = self.recursive_update(self.params_template, user_conf)
 
         def visit(path, key, value):
-            """Skip None values and empty dicts."""
+            """Skip `None` values and empty `dict`."""
             if value is None:
                 return False
             if isinstance(value, dict) and not len(value):
                 return False
             return True
 
-        return remap(valid_conf, visit=visit)
+        # Clean-up the conf by removing all blank values left-over by the template
+        # structure.
+        clean_conf = remap(filtered_conf, visit=visit)
+
+        # Update the default_map.
+        if ctx.default_map is None:
+            ctx.default_map = {}
+        ctx.default_map.update(clean_conf.get(ctx.find_root().command.name, {}))
 
     def load_conf(self, ctx, param, path_pattern):
-        """Fetch parameters values from configuration file and merge them with the
-        defaults.
+        """Fetch parameters values from configuration file and sets them as defaults.
 
-        User configuration is
-        `merged to the context default_map as Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
+        User configuration is merged to the `context's default_map
+        <https://click.palletsprojects.com/en/8.1.x/commands/#overriding-defaults>`_,
+        `like Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
 
-        This allow user's config to only overrides defaults. Values sets from direct
-        command line parameters, environment variables or interactive prompts, takes
+        By relying on Click's default_map, we make sure that precedence is respected.
+        And direct CLI parameters, environment variables or interactive prompts takes
         precedence over any values from the config file.
         """
         logger = logging.getLogger("click_extra")
 
         explicit_conf = ctx.get_parameter_source("config") in (
             ParameterSource.COMMANDLINE,
             ParameterSource.ENVIRONMENT,
             ParameterSource.PROMPT,
         )
-        # Always print a message if the user explicitly set the configuration location.
-        # We can't use logger.info because the default have not been loaded yet
-        # and the logger is stuck to its default WARNING level.
+
         message = f"Load configuration matching {path_pattern}"
+        # Force printing of configuration location if the user explicitly set it.
         if explicit_conf:
+            # We have can't simply use logger.info() here as the defaults have not been
+            # loaded yet and the logger is stuck to its default WARNING level.
             echo(message, err=True)
-        # Fallback on default configuration file location.
         else:
             logger.debug(message)
 
         # Read configuration file.
-        conf = {}
-        user_conf = self.read_and_parse_conf(path_pattern)
-        # Exit the CLI if the user-provided config file is bad.
+        conf_path, user_conf = self.read_and_parse_conf(path_pattern)
+        ctx.meta["click_extra.conf_source"] = conf_path
+        ctx.meta["click_extra.conf_full"] = user_conf
+
+        # Exit the CLI if no user-provided config file was found.
         if user_conf is None:
             message = "No configuration file found."
             if explicit_conf:
                 logger.critical(message)
 
                 # Do not just ctx.exit() as it will prevent callbacks defined on options
                 # to be called.
                 ctx.close()
                 ctx.exit(2)
             else:
                 logger.debug(message)
 
         else:
-            conf = self.merge_conf(user_conf)
-            logger.debug(f"Loaded configuration: {conf}")
-
-            # Merge config to the default_map.
-            if ctx.default_map is None:
-                ctx.default_map = {}
-            ctx.default_map.update(conf.get(ctx.find_root().command.name, {}))
+            logger.debug(f"Parsed user configuration: {user_conf}")
+            logger.debug(f"Initial defaults: {ctx.default_map}")
+            self.merge_default_map(ctx, user_conf)
             logger.debug(f"New defaults: {ctx.default_map}")
 
         return path_pattern
```

### Comparing `click_extra-4.5.0/click_extra/decorators.py` & `click_extra-4.6.0/click_extra/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .commands import ExtraCommand, ExtraGroup, default_extra_params
 from .config import ConfigOption
 from .logging import VerbosityOption
 from .parameters import ShowParamsOption
 from .tabulate import TableFormatOption
 from .telemetry import TelemetryOption
 from .timer import TimerOption
-from .version import VersionOption
+from .version import ExtraVersionOption
 
 
 def allow_missing_parenthesis(dec_factory):
     """Allow to use decorators with or without parenthesis.
 
     As proposed in
     `Cloup issue #127 <https://github.com/janluke/cloup/issues/127#issuecomment-1264704896>`_.
@@ -80,30 +80,29 @@
     return decorator
 
 
 # Redefine cloup decorators to allow them to be used with or without parenthesis.
 command = decorator_factory(dec=cloup.command)
 group = decorator_factory(dec=cloup.group)
 
-# Extra command and group decorators with default options.
+# Extra-prefixed decorators augments the default Cloup and Click ones.
 extra_command = decorator_factory(
     dec=cloup.command,
     cls=ExtraCommand,
     params=default_extra_params,
 )
 extra_group = decorator_factory(
     dec=cloup.group,
     cls=ExtraGroup,
     params=default_extra_params,
 )
+extra_version_option = decorator_factory(dec=cloup.option, cls=ExtraVersionOption)
 
-
-# Option decorators.
+# New option decorators provided by Click Extra.
 color_option = decorator_factory(dec=cloup.option, cls=ColorOption)
 config_option = decorator_factory(dec=cloup.option, cls=ConfigOption)
 help_option = decorator_factory(dec=cloup.option, cls=HelpOption)
 show_params_option = decorator_factory(dec=cloup.option, cls=ShowParamsOption)
 table_format_option = decorator_factory(dec=cloup.option, cls=TableFormatOption)
 telemetry_option = decorator_factory(dec=cloup.option, cls=TelemetryOption)
 timer_option = decorator_factory(dec=cloup.option, cls=TimerOption)
 verbosity_option = decorator_factory(dec=cloup.option, cls=VerbosityOption)
-version_option = decorator_factory(dec=cloup.option, cls=VersionOption)
```

### Comparing `click_extra-4.5.0/click_extra/docs_update.py` & `click_extra-4.6.0/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/logging.py` & `click_extra-4.6.0/click_extra/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,16 +255,15 @@
         """Set level of all loggers configured on the option.
 
         Save the verbosity level name in the context.
 
         Also prints the chosen value as a debug message via the internal
         ``click_extra`` logger.
         """
-        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
-        ctx._meta["click_extra.verbosity"] = value
+        ctx.meta["click_extra.verbosity"] = value
 
         for logger in self.all_loggers:
             logger.setLevel(LOG_LEVELS[value])
             logging.getLogger("click_extra").debug(f"Set {logger} to {value}.")
 
         ctx.call_on_close(self.reset_loggers)
```

### Comparing `click_extra-4.5.0/click_extra/parameters.py` & `click_extra-4.6.0/click_extra/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,26 @@
 """
 
 from __future__ import annotations
 
 import inspect
 import logging
 import re
-from collections.abc import MutableMapping
+from collections.abc import Iterable, MutableMapping, Sequence
+from contextlib import nullcontext
 from functools import cached_property, reduce
 from gettext import gettext as _
 from operator import getitem, methodcaller
-from typing import Any, Iterable, Sequence
+from typing import (
+    Any,
+    Callable,
+    ContextManager,
+    cast,
+)
+from unittest.mock import patch
 
 import click
 from boltons.iterutils import unique
 from mergedeep import merge
 from tabulate import tabulate
 
 from . import (
@@ -305,16 +312,15 @@
             self.excluded_params = excluded_params
 
         super().__init__(*args, **kwargs)
 
     @staticmethod
     def init_tree_dict(*path: str, leaf: Any = None):
         """Utility method to recursively create a nested dict structure whose keys are
-        provided by ``path`` list and at the end is populated by a copy of ``leaf``.
-        """
+        provided by ``path`` list and at the end is populated by a copy of ``leaf``."""
 
         def dive(levels):
             if levels:
                 return {levels[0]: dive(levels[1:])}
             return leaf
 
         return dive(path)
@@ -338,18 +344,17 @@
             else:
                 yield new_key, v
 
     def flatten_tree_dict(
         self,
         tree_dict: MutableMapping,
         parent_key: str | None = None,
-    ):
+    ) -> dict[str, Any]:
         """Recursively traverse the tree-like ``dict`` and produce a flat ``dict`` whose
-        keys are path and values are the leaf's content.
-        """
+        keys are path and values are the leaf's content."""
         return dict(self._flatten_tree_dict_gen(tree_dict, parent_key))
 
     def walk_params(self):
         """Generates an unfiltered list of all CLI parameters.
 
         Everything is included, from top-level groups to subcommands, and from options
         to arguments.
@@ -509,16 +514,17 @@
     """
 
     TABLE_HEADERS = (
         "ID",
         "Class",
         "Spec.",
         "Type",
-        "Allowed in conf?",
+        "Hidden",
         "Exposed",
+        "Allowed in conf?",
         "Env. vars.",
         "Default",
         "Value",
         "Source",
     )
     """Hard-coded list of table headers."""
 
@@ -546,38 +552,45 @@
             is_flag=is_flag,
             expose_value=expose_value,
             is_eager=is_eager,
             help=help,
             **kwargs,
         )
 
-    def print_params(self, ctx, param, value):
+    def print_params(
+        self,
+        ctx: click.Context,
+        param: click.Parameter,
+        value: bool,
+    ) -> None:
         """Introspects current CLI and list its parameters and metadata.
 
         .. important::
             Click doesn't keep a list of all parsed arguments and their origin.
             So we need to emulate here what's happening during CLI invocation.
 
             Unfortunately we cannot even do that because the raw, pre-parsed arguments
             are not available anywhere within Click's internals.
 
             Our workaround consist in leveraging our custom
             ``ExtraCommand``/``ExtraGroup`` classes, in which we are attaching
             a ``click_extra.raw_args`` metadata entry to the context.
         """
-        # imported here to avoid circular imports.
+        # Imported here to avoid circular imports.
         from .colorize import KO, OK, default_theme
         from .config import ConfigOption
 
         # Exit early if the callback was processed but the option wasn't set.
         if not value:
             return
 
         logger = logging.getLogger("click_extra")
 
+        get_param_value: Callable[[Any], Any]
+
         if "click_extra.raw_args" in ctx.meta:
             raw_args = ctx.meta.get("click_extra.raw_args", [])
             logger.debug(f"click_extra.raw_args: {raw_args}")
 
             # Mimics click.core.Command.parse_args() so we can produce the list of
             # parsed options values.
             parser = ctx.command.make_parser(ctx)
@@ -593,63 +606,106 @@
         else:
             logger.debug(f"click_extra.raw_args not in {ctx.meta}")
             logger.warning(
                 f"Cannot extract parameters values: "
                 f"{ctx.command} does not inherits from ExtraCommand.",
             )
 
-            def vanilla_getter(param):
+            def vanilla_getter(p):
                 param_value = None
-                source = ctx.get_parameter_source(param.name)
+                source = ctx.get_parameter_source(p.name)
                 return param_value, source
 
             get_param_value = vanilla_getter
 
         # Inspect the CLI to search for any --config option.
-        config_option = search_params(ctx.command.params, ConfigOption)
+        config_option = cast(
+            "ConfigOption",
+            search_params(ctx.command.params, ConfigOption),
+        )
 
-        table = []
+        table: list[
+            tuple[
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+                str | None,
+            ]
+        ] = []
         for path, param_type in self.flatten_tree_dict(self.params_types).items():
             # Get the parameter instance.
             tree_keys = path.split(self.SEP)
-            param = self.get_tree_value(self.params_objects, *tree_keys)
-            assert param.name == tree_keys[-1]
+            par = cast(
+                "click.Parameter",
+                self.get_tree_value(self.params_objects, *tree_keys),
+            )
+            assert par.name == tree_keys[-1]
 
-            param_value, source = get_param_value(param)
+            param_value, source = get_param_value(par)
             param_class = self.get_tree_value(self.params_objects, *tree_keys).__class__
-            param_spec = param.get_help_record(ctx)[0]
+
+            # Collect param's spec and hidden status.
+            hidden = None
+            param_spec = None
+            # Hidden property is only supported by Option, not Argument.
+            # TODO: Allow arguments to produce their spec.
+            if hasattr(par, "hidden"):
+                hidden = OK if par.hidden is True else KO
+
+                # No-op context manager without any effects.
+                hidden_param_bypass: ContextManager = nullcontext()
+                # If the parameter is hidden, we need to temporarily disable this flag
+                # to let Click produce a help record.
+                # See: https://github.com/kdeldycke/click-extra/issues/689
+                # TODO: Submit a PR to Click to separate production of param spec and
+                # help record. That way we can always produce the param spec even if
+                # the parameter is hidden.
+                if par.hidden:
+                    hidden_param_bypass = patch.object(par, "hidden", False)
+                with hidden_param_bypass:
+                    help_record = par.get_help_record(ctx)
+                    if help_record:
+                        param_spec = help_record[0]
 
             # Check if the parameter is allowed in the configuration file.
             allowed_in_conf = None
             if config_option:
                 allowed_in_conf = KO if path in config_option.excluded_params else OK
 
             line = (
                 default_theme.invoked_command(path),
                 f"{param_class.__module__}.{param_class.__qualname__}",
                 param_spec,
                 param_type.__name__,
+                hidden,
+                OK if par.expose_value is True else KO,
                 allowed_in_conf,
-                OK if param.expose_value is True else KO,
-                ", ".join(map(default_theme.envvar, all_envvars(param, ctx))),
-                default_theme.default(param.get_default(ctx)),
+                ", ".join(map(default_theme.envvar, all_envvars(par, ctx))),
+                default_theme.default(str(par.get_default(ctx))),
                 param_value,
                 source._name_ if source else None,
             )
             table.append(line)
 
         def sort_by_depth(line):
             """Sort parameters by depth first, then IDs, so that top-level parameters
             are kept to the top."""
             param_path = line[0]
             tree_keys = param_path.split(self.SEP)
             return len(tree_keys), param_path
 
         header_style = Style(bold=True)
-        header_labels = map(header_style, self.TABLE_HEADERS)
+        header_labels = tuple(map(header_style, self.TABLE_HEADERS))
 
         output = tabulate(
             sorted(table, key=sort_by_depth),
             headers=header_labels,
             tablefmt="rounded_outline",
             disable_numparse=True,
         )
```

### Comparing `click_extra-4.5.0/click_extra/platforms.py` & `click_extra-4.6.0/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/pygments.py` & `click_extra-4.6.0/click_extra/pygments.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 We defaults to ``Generic.Output`` tokens, as this is the token type used by all REPL-
 like and terminal lexers.
 """
 
 
 class AnsiFilter(Filter):
     """Custom filter transforming a particular kind of token (``Generic.Output`` by
-    defaults) into ANSI tokens.
-    """
+    defaults) into ANSI tokens."""
 
     def __init__(self, **options) -> None:
         """Initialize a ``AnsiColorLexer`` and configure the ``token_type`` to be
         colorized.
 
         .. todo::
 
@@ -161,16 +160,15 @@
     locals()[new_name] = new_lexer
     lexer_map[original_lexer] = new_lexer
 
 
 class AnsiHtmlFormatter(ExtendedColorHtmlFormatterMixin, HtmlFormatter):
     """Extend standard Pygments' ``HtmlFormatter``.
 
-    `Adds support for ANSI 256 colors
-    <https://github.com/chriskuehl/pygments-ansi-color#optional-enable-256-color-support>`_.
+    `Adds support for ANSI 256 colors <https://github.com/chriskuehl/pygments-ansi-color#optional-enable-256-color-support>`_.
     """
 
     name = "ANSI HTML"
     aliases = ["ansi-html"]
 
     def __init__(self, **kwargs) -> None:
         """Intercept the ``style`` argument to augment it with ANSI colors support.
```

### Comparing `click_extra-4.5.0/click_extra/sphinx.py` & `click_extra-4.6.0/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tabulate.py` & `click_extra-4.6.0/click_extra/tabulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,15 @@
         """Save table format ID in the context, and adds ``print_table()`` to it.
 
         The ``print_table(tabular_data, headers)`` method added to the context is a
         ready-to-use helper that takes for parameters:
         - ``tabular_data``, a 2-dimensional iterable of iterables for cell values,
         - ``headers``, a list of string to be used as headers.
         """
-        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
-        ctx._meta["click_extra.table_format"] = value
+        ctx.meta["click_extra.table_format"] = value
 
         render_func = None
         if value.startswith("csv"):
             render_func = partial(render_csv, dialect=get_csv_dialect(value))
         elif value == "vertical":
             render_func = render_vertical
         else:
```

### Comparing `click_extra-4.5.0/click_extra/telemetry.py` & `click_extra-4.6.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/testing.py` & `click_extra-4.6.0/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/__init__.py` & `click_extra-4.6.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/conftest.py` & `click_extra-4.6.0/click_extra/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,31 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Fixtures, configuration and helpers for tests."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import click
 import click.testing
 import cloup
 import pytest
 
 from click_extra.decorators import command, extra_command, extra_group, group
 from click_extra.platforms import is_linux, is_macos, is_windows
 from click_extra.testing import ExtraCliRunner
 
 if TYPE_CHECKING:
     from pathlib import Path
 
+    from _pytest.mark import MarkDecorator
+    from _pytest.mark.structures import ParameterSet
+
 skip_linux = pytest.mark.skipif(is_linux(), reason="Skip Linux")
 """Pytest mark to skip a test if run on a Linux system."""
 
 skip_macos = pytest.mark.skipif(is_macos(), reason="Skip macOS")
 """Pytest mark to skip a test if run on a macOS system."""
 
 skip_windows = pytest.mark.skipif(is_windows(), reason="Skip Windows")
@@ -76,111 +79,108 @@
 
 # XXX Support for decorator without parenthesis in Cloup has been reported upstream:
 # https://github.com/janluke/cloup/issues/127
 skip_naked = pytest.mark.skip(reason="Naked decorator not supported yet.")
 
 
 def command_decorators(
-    no_commands=False,
-    no_groups=False,
-    no_click=False,
-    no_cloup=False,
-    no_redefined=False,
-    no_extra=False,
-    with_types=False,
-):
+    no_commands: bool = False,
+    no_groups: bool = False,
+    no_click: bool = False,
+    no_cloup: bool = False,
+    no_redefined: bool = False,
+    no_extra: bool = False,
+    with_parenthesis: bool = True,
+    with_types: bool = False,
+) -> tuple[ParameterSet, ...]:
     """Returns collection of Pytest parameters to test all forms of click/cloup/click-
     extra command-like decorators."""
-    params = []
+    params: list[tuple[Any, set[str], str, tuple | MarkDecorator]] = []
 
     if no_commands is False:
         if not no_click:
-            params.extend(
-                [
-                    (click.command, {"click", "command"}, "click.command", ()),
+            params.append((click.command, {"click", "command"}, "click.command", ()))
+            if with_parenthesis:
+                params.append(
                     (click.command(), {"click", "command"}, "click.command()", ()),
-                ],
-            )
+                )
 
         if not no_cloup:
-            params.extend(
-                [
-                    (cloup.command, {"cloup", "command"}, "cloup.command", skip_naked),
-                    (cloup.command(), {"cloup", "command"}, "cloup.command()", ()),
-                ],
+            params.append(
+                (cloup.command, {"cloup", "command"}, "cloup.command", skip_naked),
             )
+            if with_parenthesis:
+                params.append(
+                    (cloup.command(), {"cloup", "command"}, "cloup.command()", ()),
+                )
 
         if not no_redefined:
-            params.extend(
-                [
-                    (command, {"redefined", "command"}, "click_extra.command", ()),
-                    (command(), {"redefined", "command"}, "click_extra.command()", ()),
-                ],
+            params.append(
+                (command, {"redefined", "command"}, "click_extra.command", ()),
             )
+            if with_parenthesis:
+                params.append(
+                    (command(), {"redefined", "command"}, "click_extra.command()", ()),
+                )
 
         if not no_extra:
-            params.extend(
-                [
-                    (
-                        extra_command,
-                        {"extra", "command"},
-                        "click_extra.extra_command",
-                        (),
-                    ),
+            params.append(
+                (
+                    extra_command,
+                    {"extra", "command"},
+                    "click_extra.extra_command",
+                    (),
+                ),
+            )
+            if with_parenthesis:
+                params.append(
                     (
                         extra_command(),
                         {"extra", "command"},
                         "click_extra.extra_command()",
                         (),
                     ),
-                ],
-            )
+                )
 
     if not no_groups:
         if not no_click:
-            params.extend(
-                [
-                    (click.group, {"click", "group"}, "click.group", ()),
-                    (click.group(), {"click", "group"}, "click.group()", ()),
-                ],
-            )
+            params.append((click.group, {"click", "group"}, "click.group", ()))
+            if with_parenthesis:
+                params.append((click.group(), {"click", "group"}, "click.group()", ()))
 
         if not no_cloup:
-            params.extend(
-                [
-                    (cloup.group, {"cloup", "group"}, "cloup.group", skip_naked),
-                    (cloup.group(), {"cloup", "group"}, "cloup.group()", ()),
-                ],
-            )
+            params.append((cloup.group, {"cloup", "group"}, "cloup.group", skip_naked))
+            if with_parenthesis:
+                params.append((cloup.group(), {"cloup", "group"}, "cloup.group()", ()))
 
         if not no_redefined:
-            params.extend(
-                [
-                    (group, {"redefined", "group"}, "click_extra.group", ()),
+            params.append((group, {"redefined", "group"}, "click_extra.group", ()))
+            if with_parenthesis:
+                params.append(
                     (group(), {"redefined", "group"}, "click_extra.group()", ()),
-                ],
-            )
+                )
 
         if not no_extra:
-            params.extend(
-                [
-                    (
-                        extra_group,
-                        {"extra", "group"},
-                        "click_extra.extra_group",
-                        (),
-                    ),
+            params.append(
+                (
+                    extra_group,
+                    {"extra", "group"},
+                    "click_extra.extra_group",
+                    (),
+                ),
+            )
+            if with_parenthesis:
+                params.append(
                     (
                         extra_group(),
                         {"extra", "group"},
                         "click_extra.extra_group()",
                         (),
                     ),
-                ],
-            )
+                )
 
     decorator_params = []
     for deco, deco_type, label, marks in params:
         args = [deco]
         if with_types:
             args.append(deco_type)
         decorator_params.append(pytest.param(*args, id=label, marks=marks))
@@ -190,14 +190,15 @@
 
 @pytest.fixture()
 def create_config(tmp_path):
     """A generic fixture to produce a temporary configuration file."""
 
     def _create_config(filename: str | Path, content: str) -> Path:
         """Create a fake configuration file."""
+        config_path: Path
         if isinstance(filename, str):
             config_path = tmp_path.joinpath(filename)
         else:
             config_path = filename.resolve()
 
         # Create the missing folder structure, like "mkdir -p" does.
         config_path.parent.mkdir(parents=True, exist_ok=True)
@@ -265,16 +266,15 @@
 )
 
 
 default_debug_uncolored_log_start = (
     r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
     r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
     r"debug: Load configuration matching .+\*\.{toml,yaml,yml,json,ini,xml}\n"
-    r"debug: Pattern is not an URL.\n"
-    r"debug: Search local file system.\n"
+    r"debug: Pattern is not an URL: search local file system.\n"
     r"debug: No configuration file found.\n"
     r"debug: \S+, version \S+\n"
     r"debug: {.*}\n"
 )
 
 default_debug_uncolored_log_end = (
     r"debug: Reset <RootLogger root \(DEBUG\)> to WARNING.\n"
@@ -283,16 +283,15 @@
 
 
 default_debug_colored_log_start = (
     r"\x1b\[34mdebug\x1b\[0m: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
     r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
     r"\x1b\[34mdebug\x1b\[0m: Load configuration"
     r" matching .+\*\.{toml,yaml,yml,json,ini,xml}\n"
-    r"\x1b\[34mdebug\x1b\[0m: Pattern is not an URL.\n"
-    r"\x1b\[34mdebug\x1b\[0m: Search local file system.\n"
+    r"\x1b\[34mdebug\x1b\[0m: Pattern is not an URL: search local file system.\n"
     r"\x1b\[34mdebug\x1b\[0m: No configuration file found.\n"
     r"\x1b\[34mdebug\x1b\[0m: \x1b\[97m\S+\x1b\[0m,"
     r" version \x1b\[32m\S+\x1b\[0m\n"
     r"\x1b\[34mdebug\x1b\[0m: \x1b\[90m{.*}\x1b\[0m\n"
 )
 
 default_debug_colored_log_end = (
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_colorize.py` & `click_extra-4.6.0/click_extra/tests/test_colorize.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from click_extra import (
     HelpTheme,
     Style,
     argument,
     echo,
     option,
     option_group,
+    pass_context,
     secho,
     style,
 )
 from click_extra.colorize import (
     HelpExtraFormatter,
     HelpExtraTheme,
     default_theme,
@@ -401,33 +402,44 @@
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
 )
 def test_integrated_color_option(invoke, param, expecting_colors):
+    """Check effect of color option on all things colored, including verbosity option.
+
+    Also checks the color option in subcommands is inherited from parent context.
+    """
+
     @extra_group
-    def color_cli8():
+    @pass_context
+    def color_cli8(ctx):
+        echo(f"ctx.color={ctx.color}")
         echo(Style(fg="yellow")("It works!"))
         echo("\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m")
 
     @color_cli8.command()
-    def command1():
+    @pass_context
+    def command1(ctx):
+        echo(f"ctx.color={ctx.color}")
         echo(style("Run command #1.", fg="magenta"))
         logging.getLogger("click_extra").warning("Processing...")
         print(style("print() bypass Click.", fg="blue"))
         secho("Done.", fg="green")
 
     result = invoke(color_cli8, param, "--verbosity", "DEBUG", "command1", color=True)
 
     assert result.exit_code == 0
     if expecting_colors:
         assert result.stdout == (
+            "ctx.color=True\n"
             "\x1b[33mIt works!\x1b[0m\n"
             "\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m\n"
+            "ctx.color=True\n"
             "\x1b[35mRun command #1.\x1b[0m\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "\x1b[32mDone.\x1b[0m\n"
         )
         assert re.fullmatch(
             (
                 rf"{default_debug_colored_log_start}"
@@ -435,16 +447,18 @@
                 rf"{default_debug_colored_log_end}"
             ),
             result.stderr,
         )
 
     else:
         assert result.stdout == (
+            "ctx.color=False\n"
             "It works!\n"
             "Art\n"
+            "ctx.color=False\n"
             "Run command #1.\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "Done.\n"
         )
         assert re.fullmatch(
             (
                 rf"{default_debug_uncolored_log_start}"
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_commands.py` & `click_extra-4.6.0/click_extra/tests/test_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 import re
 from pathlib import Path
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
-from pytest_cases import fixture
+from pytest_cases import fixture, parametrize
 
-from click_extra import echo, option, option_group
+from click_extra import echo, option, option_group, pass_context
 from click_extra.decorators import extra_command, extra_group
 
 from .conftest import (
+    command_decorators,
     default_debug_uncolored_log_end,
     default_debug_uncolored_log_start,
     default_options_colored_help,
     default_options_uncolored_help,
     skip_windows_colors,
 )
 
@@ -180,15 +181,15 @@
     "params",
     ("--version", "blah", ("--verbosity", "DEBUG"), ("--config", "random.toml")),
 )
 def test_help_eagerness(invoke, all_command_cli, params):
     """See: https://click.palletsprojects.com/en/8.0.x/advanced/#callback-evaluation-
     order.
     """
-    result = invoke(all_command_cli, "--help", params)
+    result = invoke(all_command_cli, "--help", params, color=False)
     assert result.exit_code == 0
     assert re.fullmatch(help_screen, result.stdout)
     assert "It works!" not in result.stdout
     assert not result.stderr
 
 
 @skip_windows_colors
@@ -256,14 +257,47 @@
 def test_integrated_version_value(invoke, all_command_cli):
     result = invoke(all_command_cli, "--version", color=False)
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "command-cli1, version 2021.10.08\n"
 
 
+@skip_windows_colors
+@parametrize(
+    "cmd_decorator",
+    command_decorators(
+        no_click=True,
+        no_cloup=True,
+        no_redefined=True,
+        with_parenthesis=False,
+    ),
+)
+@pytest.mark.parametrize("param", ("-h", "--help"))
+def test_colored_bare_help(invoke, cmd_decorator, param):
+    """Extra decorators are always colored.
+
+    Even when stripped of their default parameters, as reported in:
+    https://github.com/kdeldycke/click-extra/issues/534
+    https://github.com/kdeldycke/click-extra/pull/543
+    """
+
+    @cmd_decorator(params=None)
+    def bare_cli():
+        pass
+
+    result = invoke(bare_cli, param)
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert (
+        "\n"
+        "\x1b[94m\x1b[1m\x1b[4mOptions:\x1b[0m\n"
+        "  \x1b[36m-h\x1b[0m, \x1b[36m--help\x1b[0m  Show this message and exit.\n"
+    ) in result.stdout
+
+
 def test_no_option_leaks_between_subcommands(invoke):
     """As reported in https://github.com/kdeldycke/click-extra/issues/489."""
 
     @click.group
     def cli():
         echo("Run cli...")
 
@@ -340,14 +374,15 @@
     def command_cli2(opt1, opt2, opt3, opt4):
         echo("It works!")
 
     @command_cli2.command()
     def default_command():
         echo("Run command...")
 
+    # Remove colors to simplify output comparison.
     result = invoke(command_cli2, "--help", color=False)
     assert result.exit_code == 0
     assert re.fullmatch(
         (
             r"Usage: command-cli2 \[OPTIONS\] COMMAND \[ARGS\]...\n"
             r"\n"
             r"Group 1:\n"
@@ -413,11 +448,46 @@
     @cmd_decorator(context_settings=ctx_settings)
     @option("--flag1", is_flag=True, envvar=["custom1"])
     @option("--flag2", is_flag=True, envvar=["custom2"], show_envvar=True)
     @option("--flag3", is_flag=True, envvar=["custom3"], show_envvar=False)
     def cli():
         pass
 
-    result = invoke(cli, "--help")
+    # Remove colors to simplify output comparison.
+    result = invoke(cli, "--help", color=False)
     assert result.exit_code == 0
     assert not result.stderr
     assert expected_help in result.stdout
+
+
+def test_raw_args(invoke):
+    """Raw args are expected to be scoped in subcommands."""
+
+    @extra_group
+    @option("--dummy-flag/--no-flag")
+    @pass_context
+    def my_cli(ctx, dummy_flag):
+        echo("-- Group output --")
+        echo(f"dummy_flag is {dummy_flag!r}")
+        echo(f"Raw parameters: {ctx.meta.get('click_extra.raw_args', [])}")
+
+    @my_cli.command()
+    @pass_context
+    @option("--int-param", type=int, default=10)
+    def subcommand(ctx, int_param):
+        echo("-- Subcommand output --")
+        echo(f"int_parameter is {int_param!r}")
+        echo(f"Raw parameters: {ctx.meta.get('click_extra.raw_args', [])}")
+
+    result = invoke(my_cli, "--dummy-flag", "subcommand", "--int-param", "33")
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert result.stdout == dedent(
+        """\
+        -- Group output --
+        dummy_flag is True
+        Raw parameters: ['--dummy-flag', 'subcommand', '--int-param', '33']
+        -- Subcommand output --
+        int_parameter is 33
+        Raw parameters: ['--int-param', '33']
+        """,
+    )
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_config.py` & `click_extra-4.6.0/click_extra/tests/test_parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import re
+from os.path import sep
 from pathlib import Path
 from textwrap import dedent
 
 import click
 import pytest
-from boltons.pathutils import shrinkuser
-from pytest_cases import fixture, parametrize
+from pytest_cases import parametrize
+from tabulate import tabulate
 
 from click_extra import (
     BOOL,
     FLOAT,
     INT,
     STRING,
     UNPROCESSED,
@@ -35,277 +36,223 @@
     Choice,
     DateTime,
     File,
     FloatRange,
     IntRange,
     Tuple,
     argument,
+    command,
     echo,
     get_app_dir,
     option,
+    search_params,
 )
-from click_extra.colorize import escape_for_help_screen
-from click_extra.config import ConfigOption
-from click_extra.decorators import config_option, extra_group
-from click_extra.parameters import search_params
-
-from .conftest import (
-    default_debug_uncolored_log_end,
-    default_debug_uncolored_log_start,
-)
-
-DUMMY_TOML_FILE = dedent(
-    """
-    # Comment
-
-    top_level_param             = "to_ignore"
-
-    [config-cli1]
-    verbosity = "DEBUG"
-    blahblah = 234
-    dummy_flag = true
-    my_list = ["pip", "npm", "gem"]
-
-    [garbage]
-    # An empty random section that will be skipped
-
-    [config-cli1.default-command]
-    int_param = 3
-    random_stuff = "will be ignored"
-    """,
-)
-
-DUMMY_YAML_FILE = dedent(
-    """
-    # Comment
-
-    top_level_param: to_ignore
-
-    config-cli1:
-        verbosity : DEBUG
-        blahblah: 234
-        dummy_flag: True
-        my_list:
-          - pip
-          - "npm"
-          - gem
-        default-command:
-            int_param: 3
-            random_stuff : will be ignored
-
-    garbage:
-        # An empty random section that will be skipped
-
-    """,
-)
-
-DUMMY_JSON_FILE = dedent(
-    """
-    {
-        "top_level_param": "to_ignore",
-        "config-cli1": {
-            "blahblah": 234,
-            "dummy_flag": true,
-            "my_list": [
-                "pip",
-                "npm",
-                "gem"
-            ],
-            "verbosity": "DEBUG",   // log level
-
-            # Subcommand config
-            "default-command": {
-                "int_param": 3,
-                "random_stuff": "will be ignored"
-            }
-        },
+from click_extra.decorators import extra_command, show_params_option
+from click_extra.parameters import ShowParamsOption, extend_envvars, normalize_envvar
+from click_extra.platforms import is_windows
 
-        // Section to ignore
-        "garbage": {}
-    }
-    """,
-)
+from .conftest import command_decorators
 
-DUMMY_INI_FILE = dedent(
-    """
-    ; Comment
-    # Another kind of comment
 
-    [to_ignore]
-    key=value
-    spaces in keys=allowed
-    spaces in values=allowed as well
-    spaces around the delimiter = obviously
-    you can also use : to delimit keys from values
-
-    [config-cli1.default-command]
-    int_param = 3
-    random_stuff = will be ignored
-
-    [garbage]
-    # An empty random section that will be skipped
-
-    [config-cli1]
-    verbosity : DEBUG
-    blahblah: 234
-    dummy_flag = true
-    my_list = ["pip", "npm", "gem"]
-    """,
+@pytest.mark.parametrize(
+    ("envvars_1", "envvars_2", "result"),
+    (
+        ("MY_VAR", "MY_VAR", ("MY_VAR",)),
+        (None, "MY_VAR", ("MY_VAR",)),
+        ("MY_VAR", None, ("MY_VAR",)),
+        (["MY_VAR"], "MY_VAR", ("MY_VAR",)),
+        (["MY_VAR"], None, ("MY_VAR",)),
+        ("MY_VAR", ["MY_VAR"], ("MY_VAR",)),
+        (None, ["MY_VAR"], ("MY_VAR",)),
+        (["MY_VAR"], ["MY_VAR"], ("MY_VAR",)),
+        (["MY_VAR1"], ["MY_VAR2"], ("MY_VAR1", "MY_VAR2")),
+        (["MY_VAR1", "MY_VAR2"], ["MY_VAR2"], ("MY_VAR1", "MY_VAR2")),
+        (["MY_VAR1"], ["MY_VAR1", "MY_VAR2"], ("MY_VAR1", "MY_VAR2")),
+        (["MY_VAR1"], ["MY_VAR2", "MY_VAR2"], ("MY_VAR1", "MY_VAR2")),
+        (["MY_VAR1", "MY_VAR1"], ["MY_VAR2"], ("MY_VAR1", "MY_VAR2")),
+    ),
 )
+def test_extend_envvars(envvars_1, envvars_2, result):
+    assert extend_envvars(envvars_1, envvars_2) == result
 
-DUMMY_XML_FILE = dedent(
-    """
-    <!-- Comment -->
-
-    <config-cli1 has="an attribute">
-
-        <to_ignore>
-            <key>value</key>
-            <spaces >    </spaces>
-            <text_as_value>
-                Ratione omnis sit rerum dolor.
-                Quas omnis dolores quod sint aspernatur.
-                Veniam deleniti est totam pariatur temporibus qui
-                        accusantium eaque.
-            </text_as_value>
-
-        </to_ignore>
-
-        <verbosity>debug</verbosity>
-        <blahblah>234</blahblah>
-        <dummy_flag>true</dummy_flag>
-
-        <my_list>pip</my_list>
-        <my_list>npm</my_list>
-        <my_list>gem</my_list>
-
-        <garbage>
-            <!-- An empty random section that will be skipped -->
-        </garbage>
-
-        <default-command>
-            <int_param>3</int_param>
-            <random_stuff>will be ignored</random_stuff>
-        </default-command>
 
-    </config-cli1>
-    """,
+@pytest.mark.parametrize(
+    ("env_name", "normalized_env"),
+    (
+        ("show-params-cli_VERSION", "SHOW_PARAMS_CLI_VERSION"),
+        ("show---params-cli___VERSION", "SHOW_PARAMS_CLI_VERSION"),
+        ("__show-__params-_-_-", "SHOW_PARAMS"),
+    ),
 )
+def test_normalize_envvar(env_name, normalized_env):
+    assert normalize_envvar(env_name) == normalized_env
 
 
-all_config_formats = pytest.mark.parametrize(
-    "conf_name, conf_content",
+@pytest.mark.parametrize(
+    ("cmd_decorator", "option_help"),
     (
-        pytest.param(f"configuration.{ext}", content, id=ext)
-        for ext, content in (
-            ("toml", DUMMY_TOML_FILE),
-            ("yaml", DUMMY_YAML_FILE),
-            ("json", DUMMY_JSON_FILE),
-            ("ini", DUMMY_INI_FILE),
-            ("xml", DUMMY_XML_FILE),
-        )
+        # Click does not show the auto-generated envvar in the help screen.
+        (click.command, "  --flag / --no-flag  [env var: custom]\n"),
+        # Click Extra always adds the auto-generated envvar to the help screen
+        # (and show the defaults).
+        (
+            extra_command,
+            "  --flag / --no-flag        "
+            "[env var: custom, yo_FLAG; default: no-flag]\n",
+        ),
     ),
 )
+def test_show_auto_envvar_help(invoke, cmd_decorator, option_help):
+    """Check that the auto-generated envvar appears in the help screen with the extra
+    variants.
 
+    Checks that https://github.com/pallets/click/issues/2483 is addressed.
+    """
 
-@fixture
-def simple_config_cli():
-    @extra_group
-    @option("--dummy-flag/--no-flag")
-    @option("--my-list", multiple=True)
-    def config_cli1(dummy_flag, my_list):
-        echo(f"dummy_flag = {dummy_flag!r}")
-        echo(f"my_list = {my_list!r}")
-
-    @config_cli1.command()
-    @option("--int-param", type=int, default=10)
-    def default_command(int_param):
-        echo(f"int_parameter = {int_param!r}")
-
-    return config_cli1
-
+    @cmd_decorator(context_settings={"auto_envvar_prefix": "yo"})
+    @option("--flag/--no-flag", envvar=["custom"], show_envvar=True)
+    def envvar_help():
+        pass
 
-def test_unset_conf_no_message(invoke, simple_config_cli):
-    result = invoke(simple_config_cli, "default-command")
+    # Remove colors to simplify output comparison.
+    result = invoke(envvar_help, "--help", color=False)
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
-
-
-def test_unset_conf_debug_message(invoke, simple_config_cli):
-    result = invoke(
-        simple_config_cli,
-        "--verbosity",
-        "DEBUG",
-        "default-command",
-        color=False,
-    )
-    assert result.exit_code == 0
-    assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
-    assert re.fullmatch(
-        default_debug_uncolored_log_start + default_debug_uncolored_log_end,
-        result.stderr,
-    )
-
+    assert option_help in result.stdout
 
-def test_conf_default_path(invoke, simple_config_cli):
-    result = invoke(simple_config_cli, "--help", color=False)
-    assert result.exit_code == 0
-    assert not result.stderr
 
-    # OS-specific path.
-    default_path = shrinkuser(
-        Path(get_app_dir("config-cli1")) / "*.{toml,yaml,yml,json,ini,xml}",
-    )
+def envvars_test_cases():
+    params = []
 
-    # Make path string compatible with regexp.
-    assert re.search(
-        rf"\[default:\s+{escape_for_help_screen(str(default_path))}\]",
-        result.stdout,
-    )
+    matrix = {
+        (command, "command"): {
+            "working_envvar": (
+                # User-defined envvars are recognized as-is.
+                "Magic",
+                "sUper",
+                # XXX Uppercased auto-generated envvar is recognized but should not be.
+                "YO_FLAG",
+            ),
+            "unknown_envvar": (
+                # Uppercased user-defined envvar is not recognized.
+                "MAGIC",
+                # XXX Literal auto-generated is not recognized but should be.
+                "yo_FLAG",
+                # Mixed-cased auto-generated envvat is not recognized.
+                "yo_FlAg",
+            ),
+        },
+        (extra_command, "extra_command"): {
+            "working_envvar": (
+                # User-defined envvars are recognized as-is.
+                "Magic",
+                "sUper",
+                # Literal auto-generated is properly recognized but is not in vanilla
+                # Click (see above).
+                "yo_FLAG",
+                # XXX Uppercased auto-generated envvar is recognized but should not be.
+                "YO_FLAG",
+            ),
+            "unknown_envvar": (
+                # Uppercased user-defined envvar is not recognized.
+                "MAGIC",
+                # Mixed-cased auto-generated envvat is not recognized.
+                "yo_FlAg",
+            ),
+        },
+    }
 
+    # Windows is automaticcaly normalizing any env var to upper-case, see:
+    # https://github.com/python/cpython/blob/e715da6/Lib/os.py#L748-L749
+    # https://docs.python.org/3/library/os.html?highlight=environ#os.environ
+    # So Windows needs its own test case.
+    if is_windows():
+        all_envvars = (
+            "Magic",
+            "MAGIC",
+            "sUper",
+            "yo_FLAG",
+            "YO_FLAG",
+            "yo_FlAg",
+        )
+        matrix = {
+            (command, "command"): {
+                "working_envvar": all_envvars,
+                "unknown_envvar": (),
+            },
+            (extra_command, "extra_command"): {
+                "working_envvar": all_envvars,
+                "unknown_envvar": (),
+            },
+        }
+
+    # If properly recognized, these envvar values should be passed to the flag.
+    working_value_map = {
+        "True": True,
+        "true": True,
+        "tRuE": True,
+        "1": True,
+        "": False,  # XXX: Should be True?
+        "False": False,
+        "false": False,
+        "fAlsE": False,
+        "0": False,
+    }
+    # No envvar value will have an effect on the flag if the envvar is not recognized.
+    broken_value_map = {k: False for k in working_value_map}
 
-def test_conf_not_exist(invoke, simple_config_cli):
-    conf_path = Path("dummy.toml")
-    result = invoke(
-        simple_config_cli,
-        "--config",
-        str(conf_path),
-        "default-command",
-        color=False,
-    )
-    assert result.exit_code == 2
-    assert not result.stdout
-    assert f"Load configuration matching {conf_path}\n" in result.stderr
-    assert "critical: No configuration file found.\n" in result.stderr
+    for (cmd_decorator, decorator_name), envvar_cases in matrix.items():
+        for case_name, envvar_names in envvar_cases.items():
+            value_map = (
+                working_value_map if case_name == "working_envvar" else broken_value_map
+            )
 
+            for envvar_name in envvar_names:
+                for envar_value, expected_flag in value_map.items():
+                    envvar = {envvar_name: envar_value}
+                    params.append(
+                        pytest.param(
+                            cmd_decorator,
+                            envvar,
+                            expected_flag,
+                            id=f"{decorator_name}|{case_name}={envvar}|expected_flag={expected_flag}",
+                        ),
+                    )
+
+    return params
+
+
+@parametrize("cmd_decorator, envvars, expected_flag", envvars_test_cases())
+def test_auto_envvar_parsing(invoke, cmd_decorator, envvars, expected_flag):
+    """This test highlights the way Click recognize and parse envvars.
 
-def test_conf_not_file(invoke, simple_config_cli):
-    conf_path = Path().parent
-    result = invoke(
-        simple_config_cli,
-        "--config",
-        str(conf_path),
-        "default-command",
-        color=False,
-    )
-    assert result.exit_code == 2
-    assert not result.stdout
+    It shows that the default behavior is not ideal, and covers how ``extra_command``
+    improves the situation by normalizing the envvar name.
+    """
 
-    assert f"Load configuration matching {conf_path}\n" in result.stderr
-    assert "critical: No configuration file found.\n" in result.stderr
+    @cmd_decorator(context_settings={"auto_envvar_prefix": "yo"})
+    @option("--flag/--no-flag", envvar=["Magic", "sUper"])
+    def my_cli(flag):
+        echo(f"Flag value: {flag}")
+
+    registered_envvars = ["Magic", "sUper"]
+    # @extra_command forces registration of auto-generated envvar.
+    if cmd_decorator == extra_command:
+        registered_envvars = (*registered_envvars, "yo_FLAG")
+    assert my_cli.params[0].envvar == registered_envvars
 
+    result = invoke(my_cli, env=envvars)
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert result.stdout == f"Flag value: {expected_flag}\n"
 
-@parametrize("option_decorator", (config_option, config_option()))
-def test_conf_auto_types(invoke, create_config, option_decorator):
-    """Check the conf type and structure is properly derived from CLI options.
 
-    Also covers the tests of the standalone ``@config_option`` decorator in all its
-    flavors.
-    """
+@parametrize("option_decorator", (show_params_option, show_params_option()))
+def test_params_auto_types(invoke, option_decorator):
+    """Check parameters types and structure are properly derived from CLI."""
 
     @click.command
     @option("--flag1/--no-flag1")
     @option("--flag2", is_flag=True)
     @option("--str-param1", type=str)
     @option("--str-param2", type=STRING)
     @option("--int-param1", type=int)
@@ -321,18 +268,19 @@
     @option("--choice-param", type=Choice(("a", "b", "c")))
     @option("--int-range-param", type=IntRange())
     @option("--count-param", count=True)  # See issue #170.
     @option("--float-range-param", type=FloatRange())
     @option("--datetime-param", type=DateTime())
     @option("--tuple1", nargs=2, type=Tuple([str, int]))
     @option("--list1", multiple=True)
+    @option("--hidden-param", hidden=True)  # See issue #689.
     @argument("file_arg1", type=File("w"))
     @argument("file_arg2", type=File("w"), nargs=-1)
     @option_decorator
-    def config_cli2(
+    def params_introspection(
         flag1,
         flag2,
         str_param1,
         str_param2,
         int_param1,
         int_param2,
         float_param1,
@@ -346,243 +294,301 @@
         choice_param,
         int_range_param,
         count_param,
         float_range_param,
         datetime_param,
         tuple1,
         list1,
+        hidden_param,
         file_arg1,
         file_arg2,
     ):
         echo("Works!")
 
-    conf_path = create_config("dummy.toml", DUMMY_TOML_FILE)
+    # Invoke the --show-params option to trigger the introspection.
     result = invoke(
-        config_cli2,
-        "--config",
-        str(conf_path),
+        params_introspection,
+        "--show-params",
         "random_file1",
         "random_file2",
         color=False,
     )
 
     assert result.exit_code == 0
-    assert result.stdout == "Works!\n"
+    assert result.stdout != "Works!\n"
 
-    cli_config_option = search_params(config_cli2.params, ConfigOption)
-    assert cli_config_option.params_template == {
-        "config-cli2": {
+    show_param_option = search_params(params_introspection.params, ShowParamsOption)
+    assert show_param_option.params_template == {
+        "params-introspection": {
             "flag1": None,
             "flag2": None,
             "str_param1": None,
             "str_param2": None,
             "int_param1": None,
             "int_param2": None,
             "float_param1": None,
             "float_param2": None,
             "bool_param1": None,
             "bool_param2": None,
             "uuid_param": None,
             "unprocessed_param": None,
             "file_param": None,
             "path_param": None,
+            "show_params": None,
             "choice_param": None,
             "int_range_param": None,
             "count_param": None,
             "float_range_param": None,
             "datetime_param": None,
             "tuple1": None,
             "list1": None,
+            "hidden_param": None,
             "file_arg1": None,
             "file_arg2": None,
         },
     }
-    assert cli_config_option.params_types == {
-        "config-cli2": {
+    assert show_param_option.params_types == {
+        "params-introspection": {
             "flag1": bool,
             "flag2": bool,
             "str_param1": str,
             "str_param2": str,
             "int_param1": int,
             "int_param2": int,
             "float_param1": float,
             "float_param2": float,
             "bool_param1": bool,
             "bool_param2": bool,
             "uuid_param": str,
             "unprocessed_param": str,
             "file_param": str,
             "path_param": str,
+            "show_params": bool,
             "choice_param": str,
             "int_range_param": int,
             "count_param": int,
             "float_range_param": float,
             "datetime_param": str,
             "tuple1": list,
             "list1": list,
+            "hidden_param": str,
             "file_arg1": str,
             "file_arg2": list,
         },
     }
 
 
-def test_strict_conf(invoke, create_config):
-    """Same test as the one shown in the readme, but in strict validation mode."""
-
-    @click.group
-    @option("--dummy-flag/--no-flag")
-    @option("--my-list", multiple=True)
-    @config_option(strict=True)
-    def config_cli3(dummy_flag, my_list):
-        echo(f"dummy_flag    is {dummy_flag!r}")
-        echo(f"my_list       is {my_list!r}")
-
-    @config_cli3.command
-    @option("--int-param", type=int, default=10)
-    def subcommand(int_param):
-        echo(f"int_parameter is {int_param!r}")
+# Skip click extra's commands, as show_params option is already part of the default.
+@parametrize("cmd_decorator", command_decorators(no_extra=True))
+@parametrize("option_decorator", (show_params_option, show_params_option()))
+def test_standalone_show_params_option(invoke, cmd_decorator, option_decorator):
+    @cmd_decorator
+    @option_decorator
+    def show_params():
+        echo("It works!")
 
-    conf_file = dedent(
-        """
-        # My default configuration file.
+    result = invoke(show_params, "--show-params")
+    assert result.exit_code == 0
 
-        [config-cli3]
-        dummy_flag = true   # New boolean default.
-        my_list = ["item 1", "item #2", "Very Last Item!"]
-
-        [config-cli3.subcommand]
-        int_param = 3
-        random_stuff = "will be ignored"
-        """,
+    table = [
+        (
+            "show-params.show_params",
+            "click_extra.parameters.ShowParamsOption",
+            "--show-params",
+            "bool",
+            "✘",
+            "✘",
+            "",
+            "",
+            False,
+            "",
+            "COMMANDLINE",
+        ),
+    ]
+    output = tabulate(
+        table,
+        headers=ShowParamsOption.TABLE_HEADERS,
+        tablefmt="rounded_outline",
+        disable_numparse=True,
     )
+    assert result.stdout == f"{output}\n"
 
-    conf_path = create_config("messy.toml", conf_file)
-
-    result = invoke(config_cli3, "--config", str(conf_path), "subcommand", color=False)
-
-    assert result.exception
-    assert type(result.exception) == ValueError
-    assert (
-        str(result.exception)
-        == "Parameter 'random_stuff' is not allowed in configuration file."
+    assert re.fullmatch(
+        r"warning: Cannot extract parameters values: "
+        r"<(Group|Command) show-params> does not inherits from ExtraCommand\.\n",
+        result.stderr,
     )
 
-    assert result.exit_code == 1
-    assert f"Load configuration matching {conf_path}\n" in result.stderr
-    assert not result.stdout
-
-
-@all_config_formats
-def test_conf_file_overrides_defaults(
-    invoke,
-    simple_config_cli,
-    create_config,
-    httpserver,
-    conf_name,
-    conf_content,
-):
-    # Create a local file and remote config.
-    conf_filepath = create_config(conf_name, conf_content)
-    httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
-    conf_url = httpserver.url_for(f"/{conf_name}")
-
-    for conf_path, is_url in (conf_filepath, False), (conf_url, True):
-        result = invoke(
-            simple_config_cli,
-            "--config",
-            str(conf_path),
-            "default-command",
-            color=False,
-        )
-        assert result.exit_code == 0
-        assert result.stdout == (
-            "dummy_flag = True\nmy_list = ('pip', 'npm', 'gem')\nint_parameter = 3\n"
-        )
 
-        # Debug level has been activated by configuration file.
-        debug_log = rf"Load configuration matching {re.escape(str(conf_path))}\n"
-        if is_url:
-            debug_log += (
-                r"info: 127\.0\.0\.1 - - \[\S+ \S+\] "
-                rf'"GET /{re.escape(conf_name)} HTTP/1\.1" 200 -\n'
-            )
-        debug_log += (
-            r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
-            r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
-            r"debug: \S+, version \S+\n"
-            r"debug: {.*}\n"
-            rf"{default_debug_uncolored_log_end}"
-        )
-        assert re.fullmatch(debug_log, result.stderr)
+def test_integrated_show_params_option(invoke, create_config):
+    @extra_command
+    @option("--int-param1", type=int, default=10)
+    @option("--int-param2", type=int, default=555)
+    @option("--hidden-param", hidden=True)  # See issue #689.
+    def show_params_cli(int_param1, int_param2, hidden_param):
+        echo(f"int_param1 is {int_param1!r}")
+        echo(f"int_param2 is {int_param2!r}")
+        echo(f"hidden_param is {hidden_param!r}")
 
+    conf_file = dedent(
+        """
+        [show-params-cli]
+        int_param1 = 3
+        extra_value = "unallowed"
+        """,
+    )
+    conf_path = create_config("show-params-cli.toml", conf_file)
 
-@all_config_formats
-def test_auto_env_var_conf(
-    invoke,
-    simple_config_cli,
-    create_config,
-    httpserver,
-    conf_name,
-    conf_content,
-):
-    # Create a local config.
-    conf_filepath = create_config(conf_name, conf_content)
-
-    # Create a remote config.
-    httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
-    conf_url = httpserver.url_for(f"/{conf_name}")
-
-    for conf_path in conf_filepath, conf_url:
-        conf_path = create_config(conf_name, conf_content)
-        result = invoke(
-            simple_config_cli,
-            "default-command",
-            color=False,
-            env={"CONFIG_TEST_CLI_CONFIG": str(conf_path)},
-        )
-        assert result.exit_code == 0
-        assert result.stdout == (
-            "dummy_flag = True\nmy_list = ('pip', 'npm', 'gem')\nint_parameter = 3\n"
-        )
-        # Debug level has been activated by configuration file.
-        assert result.stderr == (
-            f"Load configuration matching {conf_path.resolve()}\n"
-            "debug: Verbosity set to DEBUG.\n"
-        )
+    raw_args = [
+        "--verbosity",
+        "DeBuG",
+        "--config",
+        str(conf_path),
+        "--int-param1",
+        "9999",
+        "--show-params",
+        "--help",
+    ]
+    result = invoke(show_params_cli, *raw_args, color=False)
 
+    assert result.exit_code == 0
+    assert f"debug: click_extra.raw_args: {raw_args!r}\n" in result.stderr
 
-@all_config_formats
-def test_conf_file_overridden_by_cli_param(
-    invoke,
-    simple_config_cli,
-    create_config,
-    httpserver,
-    conf_name,
-    conf_content,
-):
-    # Create a local file and remote config.
-    conf_filepath = create_config(conf_name, conf_content)
-    httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
-    conf_url = httpserver.url_for(f"/{conf_name}")
-
-    for conf_path in conf_filepath, conf_url:
-        conf_path = create_config(conf_name, conf_content)
-        result = invoke(
-            simple_config_cli,
-            "--my-list",
-            "super",
-            "--config",
+    table = [
+        (
+            "show-params-cli.color",
+            "click_extra.colorize.ColorOption",
+            "--color, --ansi / --no-color, --no-ansi",
+            "bool",
+            "✘",
+            "✘",
+            "✓",
+            "SHOW_PARAMS_CLI_COLOR",
+            True,
+            True,
+            "DEFAULT",
+        ),
+        (
+            "show-params-cli.config",
+            "click_extra.config.ConfigOption",
+            "-C, --config CONFIG_PATH",
+            "str",
+            "✘",
+            "✘",
+            "✘",
+            "SHOW_PARAMS_CLI_CONFIG",
+            f"{Path(get_app_dir('show-params-cli')).resolve()}{sep}*.{{toml,yaml,yml,json,ini,xml}}",
             str(conf_path),
-            "--verbosity",
-            "CRITICAL",
-            "--no-flag",
-            "--my-list",
-            "wow",
-            "default-command",
-            "--int-param",
-            "15",
-        )
-        assert result.exit_code == 0
-        assert result.stdout == (
-            "dummy_flag = False\nmy_list = ('super', 'wow')\nint_parameter = 15\n"
-        )
-        assert result.stderr == f"Load configuration matching {conf_path.resolve()}\n"
+            "COMMANDLINE",
+        ),
+        (
+            "show-params-cli.help",
+            "click_extra.colorize.HelpOption",
+            "-h, --help",
+            "bool",
+            "✘",
+            "✘",
+            "✘",
+            "SHOW_PARAMS_CLI_HELP",
+            False,
+            True,
+            "COMMANDLINE",
+        ),
+        (
+            "show-params-cli.hidden_param",
+            "cloup._params.Option",
+            "--hidden-param TEXT",
+            "str",
+            "✓",
+            "✓",
+            "✓",
+            "SHOW_PARAMS_CLI_HIDDEN_PARAM",
+            "None",
+            None,
+            "DEFAULT",
+        ),
+        (
+            "show-params-cli.int_param1",
+            "cloup._params.Option",
+            "--int-param1 INTEGER",
+            "int",
+            "✘",
+            "✓",
+            "✓",
+            "SHOW_PARAMS_CLI_INT_PARAM1",
+            3,
+            9999,
+            "COMMANDLINE",
+        ),
+        (
+            "show-params-cli.int_param2",
+            "cloup._params.Option",
+            "--int-param2 INTEGER",
+            "int",
+            "✘",
+            "✓",
+            "✓",
+            "SHOW_PARAMS_CLI_INT_PARAM2",
+            555,
+            555,
+            "DEFAULT",
+        ),
+        (
+            "show-params-cli.show_params",
+            "click_extra.parameters.ShowParamsOption",
+            "--show-params",
+            "bool",
+            "✘",
+            "✘",
+            "✘",
+            "SHOW_PARAMS_CLI_SHOW_PARAMS",
+            False,
+            True,
+            "COMMANDLINE",
+        ),
+        (
+            "show-params-cli.time",
+            "click_extra.timer.TimerOption",
+            "--time / --no-time",
+            "bool",
+            "✘",
+            "✘",
+            "✓",
+            "SHOW_PARAMS_CLI_TIME",
+            False,
+            False,
+            "DEFAULT",
+        ),
+        (
+            "show-params-cli.verbosity",
+            "click_extra.logging.VerbosityOption",
+            "-v, --verbosity LEVEL",
+            "str",
+            "✘",
+            "✘",
+            "✓",
+            "SHOW_PARAMS_CLI_VERBOSITY",
+            "WARNING",
+            "DeBuG",
+            "COMMANDLINE",
+        ),
+        (
+            "show-params-cli.version",
+            "click_extra.version.ExtraVersionOption",
+            "--version",
+            "bool",
+            "✘",
+            "✘",
+            "✘",
+            "SHOW_PARAMS_CLI_VERSION",
+            False,
+            False,
+            "DEFAULT",
+        ),
+    ]
+    output = tabulate(
+        table,
+        headers=ShowParamsOption.TABLE_HEADERS,
+        tablefmt="rounded_outline",
+        disable_numparse=True,
+    )
+    assert result.stdout == f"{output}\n"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_logging.py` & `click_extra-4.6.0/click_extra/tests/test_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 )
 def test_unrecognized_verbosity(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
     @verbosity_option
     def logging_cli1():
         echo("It works!")
 
-    result = invoke(logging_cli1, "--verbosity", "random")
+    # Remove colors to simplify output comparison.
+    result = invoke(logging_cli1, "--verbosity", "random", color=False)
     assert result.exit_code == 2
     assert not result.stdout
 
     group_help = " COMMAND [ARGS]..." if "group" in cmd_type else ""
     extra_suggest = (
         "Try 'logging-cli1 --help' for help.\n" if "extra" not in cmd_type else ""
     )
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_platforms.py` & `click_extra-4.6.0/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/test_pygments.py` & `click_extra-4.6.0/click_extra/tests/test_pygments.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,28 +142,26 @@
     lexer_classes = {find_lexer_class_by_name(alias) for alias in lexer_candidates}
     # We cannot test for strict equality yet, as some ANSI-ready lexers do not
     # have any test artifacts producing ``Generic.Output`` tokens.
     assert lexer_classes.issubset(collect_session_lexers())
 
 
 def collect_classes(klass, prefix="Ansi"):
-    """Returns all classes defined in ``click_extra.pygments`` that are a
-    subclass of ``klass``, and whose name starts with the provided ``prefix``.
-    """
+    """Returns all classes defined in ``click_extra.pygments`` that are a subclass of
+    ``klass``, and whose name starts with the provided ``prefix``."""
     klasses = {}
     for name, var in extra_pygments.__dict__.items():
         if issubclass(var, klass) and name.startswith(prefix):
             klasses[name] = var
     return klasses
 
 
 def get_pyproject_section(*section_path: str) -> dict[str, str]:
     """Descends into the TOML tree of ``pyproject.toml`` to reach the value specified by
-    ``section_path``.
-    """
+    ``section_path``."""
     toml_path = PROJECT_ROOT.joinpath("pyproject.toml").resolve()
     section: dict = tomllib.loads(toml_path.read_text(encoding="utf-8"))
     for section_id in section_path:
         section = section[section_id]
     return section
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_tabulate.py` & `click_extra-4.6.0/click_extra/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 )
 def test_unrecognized_format(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
     @table_format_option
     def tabulate_cli1():
         echo("It works!")
 
-    result = invoke(tabulate_cli1, "--table-format", "random")
+    result = invoke(tabulate_cli1, "--table-format", "random", color=False)
     assert result.exit_code == 2
     assert not result.stdout
 
     group_help = " COMMAND [ARGS]..." if "group" in cmd_type else ""
     extra_suggest = (
         "Try 'tabulate-cli1 --help' for help.\n" if "extra" not in cmd_type else ""
     )
```

### Comparing `click_extra-4.5.0/click_extra/tests/test_telemetry.py` & `click_extra-4.6.0/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/test_testing.py` & `click_extra-4.6.0/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/test_timer.py` & `click_extra-4.6.0/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/click_extra/tests/test_version.py` & `click_extra-4.6.0/click_extra/tests/test_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
 import click
 import pytest
 from boltons.strutils import strip_ansi
 from pytest_cases import parametrize
 
 from click_extra import Style, __version__, echo, pass_context
-from click_extra.decorators import color_option, extra_group, version_option
+from click_extra.decorators import color_option, extra_group, extra_version_option
 
 from .conftest import command_decorators, skip_windows_colors
 
 
 @skip_windows_colors
 @parametrize("cmd_decorator", command_decorators())
-@parametrize("option_decorator", (version_option, version_option()))
+@parametrize("option_decorator", (extra_version_option, extra_version_option()))
 def test_standalone_version_option(invoke, cmd_decorator, option_decorator):
     @cmd_decorator
     @option_decorator
     def standalone_option():
         echo("It works!")
 
     result = invoke(standalone_option, "--version", color=True)
@@ -47,15 +47,15 @@
         "\x1b[0m\n"
     )
 
 
 @skip_windows_colors
 def test_set_version(invoke):
     @click.group
-    @version_option(version="1.2.3.4")
+    @extra_version_option(version="1.2.3.4")
     def color_cli2():
         echo("It works!")
 
     # Test default coloring.
     result = invoke(color_cli2, "--version", color=True)
     assert result.exit_code == 0
     assert not result.stderr
@@ -91,28 +91,28 @@
             r"\x1b\[97mclick_extra"
             r"\x1b\[0m\n",
         ),
     ),
 )
 def test_custom_message(invoke, cmd_decorator, message, regex_stdout):
     @cmd_decorator
-    @version_option(message=message)
+    @extra_version_option(message=message)
     def color_cli3():
         echo("It works!")
 
     result = invoke(color_cli3, "--version", color=True)
     assert result.exit_code == 0
     assert not result.stderr
     assert re.fullmatch(regex_stdout, result.output)
 
 
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
 def test_style_reset(invoke, cmd_decorator):
     @cmd_decorator
-    @version_option(
+    @extra_version_option(
         version_style=None,
         package_name_style=None,
         prog_name_style=None,
         env_info_style=None,
         message_style=None,
     )
     def color_reset():
@@ -123,15 +123,15 @@
     assert not result.stderr
     assert result.output == strip_ansi(result.output)
 
 
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
 def test_context_meta(invoke, cmd_decorator):
     @cmd_decorator
-    @version_option
+    @extra_version_option
     @pass_context
     def version_metadata(ctx):
         for var in ("version", "package_name", "prog_name", "env_info"):
             value = ctx.meta[f"click_extra.{var}"]
             echo(f"{var} = {value}")
 
     result = invoke(version_metadata, color=True)
@@ -180,15 +180,15 @@
         Maybe have the possibility to tweak CLI callback evaluation order so we can
         let the user to have the NO_COLOR env set to allow for color-less ``--version``
         output.
     """
 
     @click.command
     @color_option
-    @version_option(version="2.1.9")
+    @extra_version_option(version="2.1.9")
     def color_cli6():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli6, "--no-color", "--version", "command1", color=True)
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "color-cli6, version 2.1.9\n"
```

### Comparing `click_extra-4.5.0/click_extra/timer.py` & `click_extra-4.6.0/click_extra/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 
         Computes and print the execution time at the end of the CLI, if option has been
         activated.
         """
         # Take timestamp snapshot.
         self.start_time = perf_counter()
 
-        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
-        ctx._meta["click_extra.start_time"] = self.start_time
+        ctx.meta["click_extra.start_time"] = self.start_time
 
         # Skip timekeeping if option is not active.
         if value:
             # Register printing at the end of execution.
             ctx.call_on_close(self.print_timer)
 
     def __init__(
```

### Comparing `click_extra-4.5.0/click_extra/version.py` & `click_extra-4.6.0/click_extra/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from cloup.styling import IStyle
 
 
-class VersionOption(ExtraOption):
+class ExtraVersionOption(ExtraOption):
     """Gather CLI metadata and prints a colored version string.
 
     .. warning::
         This started as a `copy of the standard @click.version_option() decorator
         <https://github.com/pallets/click/blob/dc918b4/src/click/decorators.py#L399-L466>`_,
-        but is **no longer a drop-in replacement**.
+        but is **no longer a drop-in replacement**. Hence the ``Extra`` prefix.
 
-        Still, keep an eye on the original implementation to backport fixes and
+        Still, we'll keep an eye on the original implementation to backport fixes and
         improvements.
 
     .. important::
         This option has been made into a class here, to allow its use with the
         declarative ``params=`` argument. Which `fixes Click #2324 issue
         <https://github.com/pallets/click/issues/2324>`_.
     """
@@ -59,16 +59,17 @@
         param_decls: Sequence[str] | None = None,
         version: str | None = None,
         package_name: str | None = None,
         prog_name: str | None = None,
         message: str | None = None,
         env_info: dict[str, str] | None = None,
         version_style: IStyle | None = Style(fg="green"),
-        package_name_style: IStyle | None = default_theme.invoked_command,
-        prog_name_style: IStyle | None = default_theme.invoked_command,
+        package_name_style: IStyle
+        | None = default_theme.invoked_command,  # type: ignore
+        prog_name_style: IStyle | None = default_theme.invoked_command,  # type: ignore
         env_info_style: IStyle | None = Style(fg="bright_black"),
         message_style: IStyle | None = None,
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_("Show the version and exit."),
         **kwargs,
@@ -275,20 +276,19 @@
         param: Parameter,
         value: bool,
     ) -> None:
         """Print the version string and exits.
 
         Also stores all version string elements in the Context's ``meta`` `dict`.
         """
-        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
-        ctx._meta["click_extra.package_name"] = self.package_name
+        ctx.meta["click_extra.package_name"] = self.package_name
         # Trigger the version after package_name as it depends on it.
-        ctx._meta["click_extra.version"] = self.version
-        ctx._meta["click_extra.prog_name"] = self.prog_name
-        ctx._meta["click_extra.env_info"] = self.env_info
+        ctx.meta["click_extra.version"] = self.version
+        ctx.meta["click_extra.prog_name"] = self.prog_name
+        ctx.meta["click_extra.env_info"] = self.env_info
 
         if not value or ctx.resilient_parsing:
             return
 
         echo(self.render_message(), color=ctx.color)
 
         # Do not just ctx.exit() as it will prevent callbacks defined on options
```

### Comparing `click_extra-4.5.0/pyproject.toml` & `click_extra-4.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.5.0"
+version = "4.6.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -68,16 +68,18 @@
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
 python = "^3.8"
 # XXX boltons.ecoutils 23.0.0 breaks PDB interactive sessions in pytest.
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
 boltons = "^23.0.0"
-# Click 8.1 is the first version to support ``params=`` in ``@command``.
-click = "^8.1"
+# Click 8.1.4 fix @group.command calls with a custom command_class. See:
+# https://github.com/pallets/click/issues/2416
+# https://github.com/pallets/click/pull/2417
+click = "^8.1.4"
 # Cloup 2.1.1 fix heading colorization.
 cloup = "^2.1.1"
 commentjson = "^0.9.0"
 mergedeep = "^1.3.4"
 # Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
 Pallets-Sphinx-Themes = "^2.1.1"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
@@ -180,15 +182,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.5.0"
+current_version = "4.6.0"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./click_extra/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "./pyproject.toml"
```

### Comparing `click_extra-4.5.0/readme.md` & `click_extra-4.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.5.0/PKG-INFO` & `click_extra-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.5.0
+Version: 4.6.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -37,15 +37,15 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
-Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: cloup (>=2.1.1,<3.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.5.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.6.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -21,18 +21,18 @@
 Classifier: Topic :: System :: Shells Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing :: Filters Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
 Markdown Classifier: Topic :: Text Processing :: Markup :: XML Classifier:
 Topic :: Text Processing :: Markup :: reStructuredText Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Dist: Pallets-Sphinx-Themes
 (>=2.1.1,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
-(>=8.1,<9.0) Requires-Dist: cloup (>=2.1.1,<3.0.0) Requires-Dist: commentjson
-(>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
-pygments (>=2.14,<3.0) Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
-Requires-Dist: pyyaml (>=6.0.0,<7.0.0) Requires-Dist: regex
+(>=8.1.4,<9.0.0) Requires-Dist: cloup (>=2.1.1,<3.0.0) Requires-Dist:
+commentjson (>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
+Requires-Dist: pygments (>=2.14,<3.0) Requires-Dist: pygments-ansi-color
+(>=0.3.0,<0.4.0) Requires-Dist: pyyaml (>=6.0.0,<7.0.0) Requires-Dist: regex
 (>=2023.3.22,<2024.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
 Dist: sphinx (>=6,<7) Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist:
 wcmatch (>=8.4.1,<9.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
 URL: Changelog, https://kdeldycke.github.io/click-extra/changelog.html Project-
 URL: Documentation, https://kdeldycke.github.io/click-extra Project-URL:
 Funding, https://github.com/sponsors/kdeldycke Project-URL: Issues, https://
```

