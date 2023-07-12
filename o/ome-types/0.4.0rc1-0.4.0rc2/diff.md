# Comparing `tmp/ome_types-0.4.0rc1.tar.gz` & `tmp/ome_types-0.4.0rc2.tar.gz`

## Comparing `ome_types-0.4.0rc1.tar` & `ome_types-0.4.0rc2.tar`

### file list

```diff
@@ -1,45 +1,57 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_config.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/main.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/templates/docstrings.numpy.jinja2
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/__init__.py
--rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_conversion.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/py.typed
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/units.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_bin_data.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_pixels.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_structured_annotations.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/hatch_build.py
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/main.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/class.jinja2
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/enum.jinja2
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/__init__.py
+-rw-r--r--   0        0        0    17941 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/units.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_kinded.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_validators.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2003-FC-to-2008-09.xsl
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2007-06-to-2008-09.xsl
+-rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2008-02-to-2008-09.xsl
+-rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2008-09-to-2009-09.xsl
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2009-09-to-2010-04.xsl
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2010-04-to-2010-06.xsl
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2010-06-to-2011-06.xsl
+-rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2011-06-to-2012-06.xsl
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2012-06-to-2013-06.xsl
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2013-06-to-2015-01.xsl
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2015-01-to-2016-06.xsl
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/LICENSE
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/hatch_build.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/PKG-INFO
```

### Comparing `ome_types-0.4.0rc1/CHANGELOG.md` & `ome_types-0.4.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_autogen/_config.py` & `ome_types-0.4.0rc2/src/ome_autogen/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from xsdata.codegen.writer import CodeWriter
 from xsdata.models import config as cfg
 from xsdata.utils import text
 
 from ome_autogen._generator import OmeGenerator
 from ome_autogen._util import camel_to_snake
 
+KindedTypes = "(Shape|ManufacturerSpec|Annotation)"
+
+
 MIXIN_MODULE = "ome_types._mixins"
 MIXINS: list[tuple[str, str, bool]] = [
     (".*", f"{MIXIN_MODULE}._base_type.OMEType", False),  # base type on every class
     ("OME", f"{MIXIN_MODULE}._ome.OMEMixin", True),
     ("Instrument", f"{MIXIN_MODULE}._instrument.InstrumentMixin", False),
     ("Reference", f"{MIXIN_MODULE}._reference.ReferenceMixin", True),
-    ("BinData", f"{MIXIN_MODULE}._bin_data.BinDataMixin", True),
-    ("Pixels", f"{MIXIN_MODULE}._pixels.PixelsMixin", True),
+    (KindedTypes, f"{MIXIN_MODULE}._kinded.KindMixin", True),
 ]
 
 ALLOW_RESERVED_NAMES = {"type", "Type", "Union"}
 OME_FORMAT = "OME"
 
 
 def get_config(
```

### Comparing `ome_types-0.4.0rc1/src/ome_autogen/_generator.py` & `ome_types-0.4.0rc2/src/ome_autogen/_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sys
 from contextlib import contextmanager
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterator, NamedTuple, cast
+from typing import TYPE_CHECKING, Callable, Iterator, NamedTuple, cast
 
 from xsdata.formats.dataclass.filters import Filters
 from xsdata.formats.dataclass.generator import DataclassGenerator
 
 from ome_autogen import _util
 from xsdata_pydantic_basemodel.generator import PydanticBaseFilters
 
@@ -18,14 +18,41 @@
     from xsdata.models.config import GeneratorConfig
 
 
 # from ome_types._mixins._base_type import AUTO_SEQUENCE
 # avoiding import to avoid build-time dependency on the ome-types package
 AUTO_SEQUENCE = "__auto_sequence__"
 
+# Methods and/or validators to add to generated classes
+# (predicate, method) where predicate returns True if the method should be added
+# to the given class.  Note: imports for these methods are added in
+# IMPORT_PATTERNS below.
+ADDED_METHODS: list[tuple[Callable[[Class], bool], str]] = [
+    (
+        lambda c: c.name == "BinData",
+        "\n\n_v = root_validator(pre=True)(bin_data_root_validator)",
+    ),
+    (
+        lambda c: c.name == "Value",
+        "\n\n_v = validator('any_elements', each_item=True)(any_elements_validator)",
+    ),
+    (
+        lambda c: c.name == "Pixels",
+        "\n\n_v = root_validator(pre=True)(pixels_root_validator)",
+    ),
+    (
+        lambda c: c.name == "XMLAnnotation",
+        "\n\n_v = validator('value', pre=True)(xml_value_validator)",
+    ),
+    (
+        lambda c: c.name == "PixelType",
+        "\n\nnumpy_dtype = property(pixel_type_to_numpy_dtype)",
+    ),
+]
+
 
 class Override(NamedTuple):
     element_name: str  # name of the attribute in the XSD
     class_name: str  # name of our override class
     module_name: str | None  # module where the override class is defined
 
 
@@ -51,14 +78,27 @@
 IMPORT_PATTERNS = {
     o.module_name: {
         o.class_name: [f": {o.class_name} =", f": Optional[{o.class_name}] ="]
     }
     for o in CLASS_OVERRIDES
     if o.module_name
 }
+IMPORT_PATTERNS.update(
+    {
+        "ome_types._mixins._util": {"new_uuid": ["default_factory=new_uuid"]},
+        "datetime": {"datetime": ["datetime"]},
+        "ome_types._mixins._validators": {
+            "any_elements_validator": ["any_elements_validator"],
+            "bin_data_root_validator": ["bin_data_root_validator"],
+            "pixels_root_validator": ["pixels_root_validator"],
+            "xml_value_validator": ["xml_value_validator"],
+            "pixel_type_to_numpy_dtype": ["pixel_type_to_numpy_dtype"],
+        },
+    }
+)
 
 
 class OmeGenerator(DataclassGenerator):
     @classmethod
     def init_filters(cls, config: GeneratorConfig) -> Filters:
         return OmeFilters(config)
 
@@ -95,15 +135,16 @@
 
 
 class OmeFilters(PydanticBaseFilters):
     def register(self, env: Environment) -> None:
         # add our own templates dir to the search path
         tpl_dir = Path(__file__).parent.joinpath("templates")
         cast("FileSystemLoader", env.loader).searchpath.insert(0, str(tpl_dir))
-        return super().register(env)
+        super().register(env)
+        env.filters.update({"methods": self.methods})
 
     def __init__(self, config: GeneratorConfig):
         super().__init__(config)
 
         # TODO: it would be nice to know how to get the schema we're processing from
         # the config.  For now, we just assume it's the OME schema and that's the
         # hardcoded default in _util.get_appinfo
@@ -186,17 +227,21 @@
         type_name = super().field_type(attr, parents)
         # we want to use datetime.datetime instead of XmlDateTime
         return type_name.replace("XmlDateTime", "datetime")
 
     @classmethod
     def build_import_patterns(cls) -> dict[str, dict]:
         patterns = super().build_import_patterns()
+        patterns.setdefault("pydantic", {}).update(
+            {
+                "validator": ["validator("],
+                "root_validator": ["root_validator("],
+            }
+        )
         patterns.update(IMPORT_PATTERNS)
-        patterns["ome_types._mixins._util"] = {"new_uuid": ["default_factory=new_uuid"]}
-        patterns["datetime"] = {"datetime": ["datetime"]}
         return {key: patterns[key] for key in sorted(patterns)}
 
     def field_default_value(self, attr: Attr, ns_map: dict | None = None) -> str:
         if attr.tag == "Attribute" and attr.name == "ID":
             return repr(AUTO_SEQUENCE)
         for override in CLASS_OVERRIDES:
             if attr.name == override.element_name:
@@ -217,7 +262,13 @@
         return super().format_arguments(kwargs, indent)
 
     def constant_name(self, name: str, class_name: str) -> str:
         if class_name in self.appinfo.enums:
             # use the enum names found in appinfo/xsdfu/enum
             return self.appinfo.enums[class_name][name].enum
         return super().constant_name(name, class_name)
+
+    def methods(self, obj: Class) -> list[str]:
+        for predicate, code in ADDED_METHODS:
+            if predicate(obj):
+                return [code]
+        return []
```

### Comparing `ome_types-0.4.0rc1/src/ome_autogen/_transformer.py` & `ome_types-0.4.0rc2/src/ome_autogen/_transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_autogen/_util.py` & `ome_types-0.4.0rc2/src/ome_autogen/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 @lru_cache(maxsize=None)
 def get_appinfo(schema: Path | str = SCHEMA_FILE) -> AppInfo:
     """Gather all the <xsd:appinfo> stuff from the schema.
 
     xsdata doesn't try to do anything with it. But we want to use it to
     provide better enum and plural names
     """
-    tree = ET.parse(schema)  # noqa: S314
+    tree = ET.parse(schema)
     plurals: dict[str, str] = {}
     enums: defaultdict[str, dict[str, EnumInfo]] = defaultdict(dict)
     in_name = ""
     in_value = ""
     abstract = []
     for node in tree.iter():
         if node.tag == "plural":  # <plural>
```

### Comparing `ome_types-0.4.0rc1/src/ome_autogen/main.py` & `ome_types-0.4.0rc2/src/ome_autogen/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from pathlib import Path
 from shutil import rmtree
 
 from ome_autogen import _util
 from ome_autogen._config import get_config
 from ome_autogen._transformer import OMETransformer
 
+BLACK_LINE_LENGTH = 88
+BLACK_TARGET_VERSION = "py37"
+BLACK_SKIP_TRAILING_COMMA = False  # use trailing commas as a reason to split lines?
 OUTPUT_PACKAGE = "ome_types._autogenerated.ome_2016_06"
 DO_MYPY = os.environ.get("OME_AUTOGEN_MYPY", "0") == "1" or "--mypy" in sys.argv
 SRC_PATH = Path(__file__).parent.parent
 SCHEMA_FILE = (SRC_PATH / "ome_types" / "ome-2016-06.xsd").absolute()
 RUFF_IGNORE: list[str] = [
     "D101",  # Missing docstring in public class
     "D106",  # Missing docstring in public nested class
@@ -53,21 +56,29 @@
 
     _print_green(f"OME python model created at {OUTPUT_PACKAGE}")
 
 
 def _fix_formatting(package_dir: str, ruff_ignore: list[str] = RUFF_IGNORE) -> None:
     _print_gray("Running black and ruff ...")
 
-    black = ["black", package_dir, "-q", "--line-length=88"]
-    subprocess.check_call(black)  # noqa S
-
     ruff = ["ruff", "-q", "--fix", package_dir]
     ruff.extend(f"--ignore={ignore}" for ignore in ruff_ignore)
     subprocess.check_call(ruff)  # noqa S
 
+    black = [
+        "black",
+        "-q",
+        f"--line-length={BLACK_LINE_LENGTH}",
+        f"--target-version={BLACK_TARGET_VERSION}",
+    ]
+    if BLACK_SKIP_TRAILING_COMMA:  # pragma: no cover
+        black.append("--skip-magic-trailing-comma")
+    black.extend([str(x) for x in Path(package_dir).rglob("*.py")])
+    subprocess.check_call(black)  # noqa S
+
 
 def _check_mypy(package_dir: str) -> None:
     _print_gray("Running mypy ...")
 
     mypy = ["mypy", package_dir, "--strict"]
     try:
         subprocess.check_output(mypy, stderr=subprocess.STDOUT)  # noqa S
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/__init__.py` & `ome_types-0.4.0rc2/src/ome_types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,22 @@
     from importlib_metadata import PackageNotFoundError, version  # type: ignore
 
 try:
     __version__ = version("ome-types")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from ome_types.units import ureg  # noqa: TCH004
 
 from ome_types import model
-from ome_types._conversion import from_tiff, from_xml, to_dict, to_xml
+from ome_types._conversion import from_tiff, from_xml, to_dict, to_xml, validate_xml
 from ome_types.model import OME
-from ome_types.validation import validate_xml
 
 __all__ = [
     "__version__",
     "from_tiff",
     "from_xml",
     "model",
     "OME",
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0rc2/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/units.py` & `ome_types-0.4.0rc2/src/ome_types/units.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0rc2/src/ome_types/_mixins/_base_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 import warnings
 from datetime import datetime
 from enum import Enum
 from textwrap import indent
-from typing import Any, ClassVar, Dict, Optional, Sequence, Set, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Dict,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    cast,
+)
 
 from pydantic import BaseModel, validator
 
 from ome_types._mixins._ids import validate_id
 
 try:
     from ome_types.units import add_quantity_properties
 except ImportError:
     add_quantity_properties = lambda cls: None  # noqa: E731
 
+if TYPE_CHECKING:
+    from ome_types._conversion import XMLSource
+
+
+T = TypeVar("T", bound="OMEType")
 # Default value to support automatic numbering for id field values.
 AUTO_SEQUENCE = "__auto_sequence__"
 
 
 DEPRECATED_NAMES = {
     "annotation_ref": "annotation_refs",
     "bin_data": "bin_data_blocks",
@@ -72,19 +90,21 @@
 
     # allow use with weakref
     __slots__: ClassVar[Set[str]] = {"__weakref__"}  # type: ignore
 
     _v = validator("id", pre=True, always=True, check_fields=False)(validate_id)
 
     def __init__(self, **data: Any) -> None:
+        warn_extra = data.pop("warn_extra", True)
         field_names = set(self.__fields__.keys())
         _move_deprecated_fields(data, field_names)
         super().__init__(**data)
         kwargs = set(data.keys())
-        if kwargs - field_names:
+        extra = kwargs - field_names
+        if extra and warn_extra:
             warnings.warn(
                 f"Unrecognized fields for type {type(self)}: {kwargs - field_names}",
                 stacklevel=2,
             )
 
     def __init_subclass__(cls) -> None:
         """Add `*_quantity` property for fields that have both a value and a unit.
@@ -131,14 +151,59 @@
                 f"Attribute '{cls_name}.{key}' is deprecated, use {new_key!r} instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
             return getattr(self, new_key)
         raise AttributeError(f"{cls_name} object has no attribute {key!r}")
 
+    def to_xml(self, **kwargs: Any) -> str:
+        """Serialize this object to XML.
+
+        See docstring of [`ome_types.to_xml`][] for kwargs.
+        """
+        from ome_types._conversion import to_xml
+
+        return to_xml(self, **kwargs)
+
+    @classmethod
+    def from_xml(cls: Type[T], xml: "XMLSource", **kwargs: Any) -> T:
+        """Read an ome-types class from XML.
+
+        See docstring of [`ome_types.from_xml`][] for kwargs.
+
+        Note: this will return an instance of whatever the top node is in the XML.
+        so technically, the return type here could be incorrect.  But when used
+        properly (`Image.from_xml()`, `Pixels.from_xml()`, etc.) on an unusual xml
+        document it can provide additional typing information.
+        """
+        from ome_types._conversion import from_xml
+
+        return cast(T, from_xml(xml, **kwargs))
+
+    def _update_set_fields(self) -> None:
+        """Update set fields with populated mutable sequences.
+
+        Because pydantic isn't aware of mutations to sequences, it can't tell when
+        a field has been "set" by mutating a sequence.  This method updates the
+        self.__fields_set__ attribute to reflect that.  We assume that if an attribute
+        is not None, and is not equal to the default value, then it has been set.
+        """
+        for field_name, field in self.__fields__.items():
+            current = getattr(self, field_name)
+            if not current:
+                continue
+            if current != field.get_default():
+                self.__fields_set__.add(field_name)
+            if isinstance(current, OMEType):
+                current._update_set_fields()
+            if isinstance(current, MutableSequence):
+                for item in current:
+                    if isinstance(item, OMEType):
+                        item._update_set_fields()
+
 
 class _RawRepr:
     """Helper class to allow repr to show raw values for fields that are sequences."""
 
     def __init__(self, raw: str) -> None:
         self.raw = raw
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.0rc2/src/ome_types/_mixins/_ids.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0rc2/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0rc2/src/ome_types/_mixins/_ome.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import warnings
 import weakref
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, BinaryIO, Sequence
 
 from ome_types._mixins._base_type import OMEType
 from ome_types._mixins._ids import CONVERTED_IDS
 
 if TYPE_CHECKING:
     from pathlib import Path
 
@@ -32,51 +32,44 @@
 
     def __setstate__(self, state: dict[str, Any]) -> None:
         """Support unpickle of our weakref references."""
         super().__setstate__(state)  # type: ignore
         self._link_refs()
 
     @classmethod
-    def from_xml(cls, xml: Path | str) -> OME:
-        from ome_types._conversion import from_xml
+    def from_tiff(cls, path: Path | str | BinaryIO, **kwargs: Any) -> OME:
+        """Return an OME object from the metadata in a TIFF file.
 
-        return from_xml(xml)
-
-    @classmethod
-    def from_tiff(cls, path: Path | str) -> OME:
+        See docstring of [`ome_types.from_tiff`][] for kwargs.
+        """
         from ome_types._conversion import from_tiff
 
         return from_tiff(path)
 
-    def to_xml(self, **kwargs: Any) -> str:
-        from ome_types._conversion import to_xml
-
-        return to_xml(cast("OME", self), **kwargs)
-
 
 def collect_ids(value: Any) -> dict[str, OMEType]:
     """Return a map of all model objects contained in value, keyed by id.
 
     Recursively walks all dataclass fields and iterates over lists. The base
     case is when value is neither a dataclass nor a list.
     """
     from ome_types.model import Reference
 
     ids: dict[str, OMEType] = {}
-    if isinstance(value, list):
+    if isinstance(value, Sequence) and not isinstance(value, str):
         for v in value:
             ids.update(collect_ids(v))
     elif isinstance(value, OMEType):
-        for f in value.__fields__:
-            if f == "id" and not isinstance(value, Reference):
+        for fname in value.__fields__:
+            if fname == "id" and not isinstance(value, Reference):
                 # We don't need to recurse on the id string, so just record it
                 # and move on.
                 ids[value.id] = value
             else:
-                ids.update(collect_ids(getattr(value, f)))
+                ids.update(collect_ids(getattr(value, fname)))
     # Do nothing for uninteresting types.
     return ids
 
 
 def collect_references(value: Any) -> list[Reference]:
     """Return a list of all References contained in value.
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0rc2/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/__init__.py` & `ome_types-0.4.0rc2/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/_color.py` & `ome_types-0.4.0rc2/src/ome_types/model/_color.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/_converters.py` & `ome_types-0.4.0rc2/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/_shape_union.py` & `ome_types-0.4.0rc2/src/ome_types/model/_shape_union.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             # to create a label rather than a point
             if "kind" in v:
                 kind = v.pop("kind").lower()
                 return _KINDS[kind](**v)
 
             for cls_ in _ShapeCls:
                 with suppress(ValidationError):
-                    return cls_(**v)
+                    return cls_(warn_extra=False, **v)
         raise ValueError(f"Invalid shape: {v}")  # pragma: no cover
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.__root__!r})"
 
     # overriding BaseModel.__iter__ to behave more like a real Sequence
     def __iter__(self) -> Iterator[ShapeType]:  # type: ignore[override]
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/_structured_annotations.py` & `ome_types-0.4.0rc2/src/ome_types/model/_structured_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     CommentAnnotation,
     BooleanAnnotation,
     TimestampAnnotation,
     TagAnnotation,
     TermAnnotation,
     MapAnnotation,
 )
+_KINDS = {cls.__name__.lower(): cls for cls in AnnotationTypes}
 
 
 class StructuredAnnotationList(OMEType, UserSequence[Annotation]):  # type: ignore[misc]
     """A mutable sequence of [`ome_types.model.Annotation`][].
 
     Members of this sequence must be one of the following types:
 
@@ -66,14 +67,16 @@
     )
 
     @validator("__root__", each_item=True)
     def _validate_root(cls, v: Annotation) -> Annotation:
         if isinstance(v, AnnotationTypes):
             return v
         if isinstance(v, dict):
+            if "kind" in v:
+                return _KINDS[v.pop("kind")](**v)
             for cls_ in AnnotationTypes:
                 with suppress(ValidationError):
                     return cls_(**v)
         raise ValueError(f"Invalid Annotation: {v} of type {type(v)}")
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.__root__!r})"
```

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.0rc2/src/ome_types/model/_user_sequence.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/ome_types/model/simple_types.py` & `ome_types-0.4.0rc2/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/compat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+try:
+    from lxml import etree as ET
+except ImportError:
+    import xml.etree.ElementTree as ET  # type: ignore
+
 from dataclasses import MISSING, field
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     cast,
 )
-from xml.etree.ElementTree import QName
 
 from pydantic import BaseModel, validators
 from pydantic.fields import Field, ModelField, Undefined
 from xsdata.formats.dataclass.compat import Dataclasses, class_types
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.datatype import XmlDate, XmlDateTime, XmlDuration, XmlPeriod, XmlTime
 
@@ -31,24 +35,32 @@
     :param children: The element's list of child elements.
     :param attributes: The element's key-value attribute mappings.
     """
 
     qname: Optional[str] = Field(default=None)
     text: Optional[str] = Field(default=None)
     tail: Optional[str] = Field(default=None)
-    children: List[object] = Field(
+    children: List["AnyElement"] = Field(
         default_factory=list, metadata={"type": XmlType.WILDCARD}
     )
     attributes: Dict[str, str] = Field(
         default_factory=dict, metadata={"type": XmlType.ATTRIBUTES}
     )
 
     class Config:
         arbitrary_types_allowed = True
 
+    def to_etree_element(self) -> "ET._Element":
+        elem = ET.Element(self.qname or "", self.attributes)
+        elem.text = self.text
+        elem.tail = self.tail
+        for child in self.children:
+            elem.append(child.to_etree_element())
+        return elem
+
 
 class DerivedElement(BaseModel, Generic[T]):
     """Generic model wrapper for type substituted elements.
 
     Example: eg. <b xsi:type="a">...</b>
 
     :param qname: The element's qualified name
@@ -132,15 +144,15 @@
     validators._VALIDATORS.extend(
         [
             (XmlDate, make_validators(XmlDate, XmlDate.from_string)),
             (XmlDateTime, make_validators(XmlDateTime, XmlDateTime.from_string)),
             (XmlTime, make_validators(XmlTime, XmlTime.from_string)),
             (XmlDuration, make_validators(XmlDuration, XmlDuration)),
             (XmlPeriod, make_validators(XmlPeriod, XmlPeriod)),
-            (QName, make_validators(QName, QName)),
+            (ET.QName, make_validators(ET.QName, ET.QName)),
         ]
     )
 else:
     import warnings
 
     warnings.warn(
         "Could not find pydantic.validators._VALIDATORS."
```

### Comparing `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/.gitignore` & `ome_types-0.4.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/LICENSE` & `ome_types-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc1/README.md` & `ome_types-0.4.0rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/ome-types.svg)](https://python.org)
 [![Tests](https://github.com/tlambert03/ome-types/workflows/tests/badge.svg)](https://github.com/tlambert03/ome-types/actions)
 [![Docs](https://readthedocs.org/projects/ome-types/badge/?version=latest)](https://ome-types.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/tlambert03/ome-types/branch/main/graph/badge.svg?token=GocY9y8A32)](https://codecov.io/gh/tlambert03/ome-types)
+[![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/tlambert03/ome-types)
 
 ## A pure-python implementation of the OME data model
 
 `ome_types` provides a set of python dataclasses and utility functions for
 parsing the [OME-XML
 format](https://docs.openmicroscopy.org/ome-model/latest/ome-xml/) into
 fully-typed python objects for interactive or programmatic access in python. It
@@ -32,16 +33,21 @@
 ```shell
 pip install ome-types
 ```
 
 With all optional dependencies:
 
 ```shell
-# lxml => if you want to use lxml as the XML parser
-# pint => if you want to use object.<field>_quantity properties
+# lxml => if you ...
+#           - want to use lxml as the XML parser
+#           - want to validate XML against the ome.xsd schema
+#           - want to use XML documents older than the 2016-06 schema
+# pint      => if you want to use object.<field>_quantity properties
+# xmlschema => if you want to validate XML but DON'T want lxml
+
 pip install ome-types[lxml,pint]
 ```
 
 ### from conda
 
 ```shell
 conda install -c conda-forge ome-types
@@ -231,28 +237,27 @@
 python code. To run the code generation script in a development environment,
 clone this repository and run:
 
 ```sh
 python -m src.ome_autogen
 ```
 
-
 The documentation and types for the full model can be in the [API Reference](https://ome-types.readthedocs.io/en/latest/ome_types.model.html)
 
 ## Contributing
 
 To clone and install this repository locally:
 
 ```shell
 git clone https://github.com/tlambert03/ome-types.git
 cd ome-types
 pip install -e .[test,dev]
 ```
 
-We use `pre-commit` to run various code-quality checks  during continuous
+We use `pre-commit` to run various code-quality checks during continuous
 integration. If you'd like to make sure that your code will pass these checks
 before you commit your code, you should install `pre-commit` after cloning this
 repository:
 
 ```shell
 pre-commit install
 ```
```

### Comparing `ome_types-0.4.0rc1/pyproject.toml` & `ome_types-0.4.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,22 @@
   "xsdata[cli]>=23.6",
   "mypy",
   "pre-commit",
   "types-lxml; python_version >= '3.8'",
 ]
 docs = ["mkdocs-material", "mkdocstrings-python"]
 test = [
-  "pint",
   "lxml",
-  "pytest",
+  "numpy",
+  "pint",
+  "pytest-codspeed",
   "pytest-cov",
-  "xmlschema",
   "pytest-mypy-plugins",
+  "pytest",
+  "xmlschema",
 ]
 
 # https://hatch.pypa.io/latest/plugins/build-hook/custom/
 [tool.hatch.build.targets.wheel.hooks.custom]
 # requirements to run the autogen script in hatch_build.py
 require-runtime-dependencies = true
 dependencies = ["black", "ruff", "xsdata[cli]>=23.6"]
@@ -117,14 +119,15 @@
   "D213",   # Multi-line docstring summary should start at the second line
   "D400",   # First line should end with a period
   "D404",   # First word of the docstring should not be This
   "D413",   # Missing blank line after last section
   "D416",   # Section name should end with a colon
   "C901",   # Function is too complex
   "RUF009", # Do not perform function calls in default arguments
+  "S3",     # xml security
 ]
 exclude = ['src/_ome_autogen.py']
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all" # Disallow all relative imports.
 
 [tool.ruff.per-file-ignores]
@@ -144,20 +147,14 @@
   "mkdocs.yml",
   "docs/**/*",
   "tests/**/*",
   "typesafety/**/*",
 ]
 
 
-[tool.isort]
-profile = "black"
-line_length = 88
-float_to_top = true
-skip_glob = ["*examples/*", "*vendored*"]
-
 [tool.black]
 target-version = ['py38']
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
@@ -206,14 +203,13 @@
   "raise NotImplementedError()",
 ]
 
 [tool.coverage.run]
 source = ["ome_types", "ome_autogen"]
 omit = ["src/ome_types/_autogenerated/*", "/private/var/folders/*"]
 
-
 # Entry points -- REMOVE ONCE XSDATA-PYDANTIC-BASEMODEL IS SEPARATE
 [project.entry-points."xsdata.plugins.class_types"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.class_type"
 
 [project.entry-points."xsdata.plugins.cli"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.cli"
```

### Comparing `ome_types-0.4.0rc1/PKG-INFO` & `ome_types-0.4.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -38,16 +38,18 @@
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: lxml
 Requires-Dist: lxml>=4.8.0; extra == 'lxml'
 Provides-Extra: pint
 Requires-Dist: pint>=0.15; extra == 'pint'
 Provides-Extra: test
 Requires-Dist: lxml; extra == 'test'
+Requires-Dist: numpy; extra == 'test'
 Requires-Dist: pint; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-codspeed; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mypy-plugins; extra == 'test'
 Requires-Dist: xmlschema; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ome-types
 
@@ -55,14 +57,15 @@
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/ome-types.svg)](https://python.org)
 [![Tests](https://github.com/tlambert03/ome-types/workflows/tests/badge.svg)](https://github.com/tlambert03/ome-types/actions)
 [![Docs](https://readthedocs.org/projects/ome-types/badge/?version=latest)](https://ome-types.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/tlambert03/ome-types/branch/main/graph/badge.svg?token=GocY9y8A32)](https://codecov.io/gh/tlambert03/ome-types)
+[![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/tlambert03/ome-types)
 
 ## A pure-python implementation of the OME data model
 
 `ome_types` provides a set of python dataclasses and utility functions for
 parsing the [OME-XML
 format](https://docs.openmicroscopy.org/ome-model/latest/ome-xml/) into
 fully-typed python objects for interactive or programmatic access in python. It
@@ -83,16 +86,21 @@
 ```shell
 pip install ome-types
 ```
 
 With all optional dependencies:
 
 ```shell
-# lxml => if you want to use lxml as the XML parser
-# pint => if you want to use object.<field>_quantity properties
+# lxml => if you ...
+#           - want to use lxml as the XML parser
+#           - want to validate XML against the ome.xsd schema
+#           - want to use XML documents older than the 2016-06 schema
+# pint      => if you want to use object.<field>_quantity properties
+# xmlschema => if you want to validate XML but DON'T want lxml
+
 pip install ome-types[lxml,pint]
 ```
 
 ### from conda
 
 ```shell
 conda install -c conda-forge ome-types
@@ -282,28 +290,27 @@
 python code. To run the code generation script in a development environment,
 clone this repository and run:
 
 ```sh
 python -m src.ome_autogen
 ```
 
-
 The documentation and types for the full model can be in the [API Reference](https://ome-types.readthedocs.io/en/latest/ome_types.model.html)
 
 ## Contributing
 
 To clone and install this repository locally:
 
 ```shell
 git clone https://github.com/tlambert03/ome-types.git
 cd ome-types
 pip install -e .[test,dev]
 ```
 
-We use `pre-commit` to run various code-quality checks  during continuous
+We use `pre-commit` to run various code-quality checks during continuous
 integration. If you'd like to make sure that your code will pass these checks
 before you commit your code, you should install `pre-commit` after cloning this
 repository:
 
 ```shell
 pre-commit install
 ```
```

