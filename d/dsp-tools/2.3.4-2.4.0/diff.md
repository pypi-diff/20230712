# Comparing `tmp/dsp_tools-2.3.4.tar.gz` & `tmp/dsp_tools-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.3.4.tar", max compression
+gzip compressed data, was "dsp_tools-2.4.0.tar", max compression
```

## Comparing `dsp_tools-2.3.4.tar` & `dsp_tools-2.4.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0    35149 2023-06-28 06:11:19.583652 dsp_tools-2.3.4/LICENSE
--rw-r--r--   0        0        0     4373 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/docs/index.md
--rw-r--r--   0        0        0     4845 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    20433 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    89229 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    31627 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14293 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4185 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      929 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     8271 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3325 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8757 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16339 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     8853 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    20424 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      381 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    14778 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2280 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    16628 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1744 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    18683 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1930 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    20694 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    29981 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      401 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0      998 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    25540 2023-06-28 06:11:19.603652 dsp_tools-2.3.4/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    33279 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     1971 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      594 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0     1504 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2172 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8619 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2141 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0        0 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23544 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2526 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15315 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4886 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     8237 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10530 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3189 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0     1134 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/logging.py
--rw-r--r--   0        0        0    42405 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8373 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4694 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18807 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4259 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    13302 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6988 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    51523 2023-06-28 06:11:19.607652 dsp_tools-2.3.4/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 dsp_tools-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-12 09:35:04.011926 dsp_tools-2.4.0/LICENSE
+-rw-r--r--   0        0        0     4602 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/docs/index.md
+-rw-r--r--   0        0        0     5007 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    20863 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    89253 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    31627 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14293 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4185 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0     1059 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     8708 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3325 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8851 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16528 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     8979 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    20524 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      463 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    14896 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2350 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    16761 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1744 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    18840 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1930 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    20694 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    29833 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      496 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0     1040 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    25439 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    33397 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     1971 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      594 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1504 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2172 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8720 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2141 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23544 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     2460 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15142 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4912 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     8237 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10530 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3189 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0     1134 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/logging.py
+-rw-r--r--   0        0        0    42361 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8373 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4694 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18815 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4259 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    13326 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0    13540 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    51547 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 dsp_tools-2.4.0/PKG-INFO
```

### Comparing `dsp_tools-2.3.4/LICENSE` & `dsp_tools-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/docs/index.md` & `dsp_tools-2.4.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 
 # DSP-TOOLS documentation
 
 DSP-TOOLS is a Python package with a command line interface 
 that helps you interact with a DSP server. 
 A DSP server is a remote server or a local machine 
 where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on.
```

### Comparing `dsp_tools-2.3.4/pyproject.toml` & `dsp_tools-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.3.4"
+version = "2.4.0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -30,14 +30,15 @@
 requests = "^2.30.0"
 jsonschema = "^4.17.3"
 openpyxl = "^3.1.2"
 networkx = "^3.1.0"
 pandas = { version = "^2.0.1", extras = ["excel"] }  # extra package that contains xlrd that is necessary for reading old .xls Excel files
 regex = "^2023.5.5"
 docker = "^6.1.2"
+pyyaml = "^6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.11"
 mkdocs-include-markdown-plugin = "*"
@@ -45,23 +46,32 @@
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 types-requests = "^2.30.0.0"
 types-lxml = "^2023.3.28"
 types-jsonschema = "^4.17.0.8"
 types-openpyxl = "^3.1.0.7"
 types-regex = "^2023.5.5.0"
+pre-commit = "^3.3.3"
+types-pyyaml = "^6.0.12.10"
 
 
 [tool.poetry.scripts]
 dsp-tools = "dsp_tools.dsp_tools:main"    # definition of the CLI entry point
 
 
 [tool.poetry-exec-plugin.commands]
-# plugin (https://github.com/keattang/poetry-exec-plugin) to define commands available for the developers, e.g. `poetry exec check-links`
-check-links = "markdown-link-validator ./docs -i \\.\\/assets\\/.+ -i .+github\\.com\\/dasch\\-swiss\\/dsp-tools\\/settings"
+# plugin (https://github.com/keattang/poetry-exec-plugin) to define commands available for the developers,
+# e.g. `poetry exec check-links`
+check-links = """
+    markdown-link-validator \
+    ./docs \
+    -i \\.\\/assets\\/.+ \
+    -i .+github\\.com\\/dasch\\-swiss\\/dsp-tools\\/settings \
+    -i .+github\\.com\\/dasch\\-swiss\\/ops-deploy\\/.+
+"""
 
 
 [build-system]
 # Tells “frontend” build tools (like pip, build, or poetry) what “backend” build tool to use (e.g. setuptools, poetry).
 # The "backend" doesn't need to be installed. It will be installed by the "frontend" in a temporary, isolated
 # environment for use during the build process.
 requires = ["poetry-core"]
@@ -84,15 +94,15 @@
 
 
 [tool.black]
 line-length = 120
 
 
 [tool.pylint.MASTER]
-ignore-paths = ["src/dsp_tools/models/.*$"] # TODO: activate this
+ignore-paths = ["src/dsp_tools/models/resource.py"] # TODO: activate this
 suggestion-mode = true
 
 
 [tool.pylint.format]
 max-line-length = 120
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.4.0/src/dsp_tools/dsp_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.project_create import create_project
 from dsp_tools.utils.project_create_lists import create_lists
 from dsp_tools.utils.project_get import get_project
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.rosetta import upload_rosetta
 from dsp_tools.utils.shared import validate_xml_against_schema
-from dsp_tools.utils.stack_handling import start_stack, stop_stack
+from dsp_tools.utils.stack_handling import StackConfiguration, StackHandler
 from dsp_tools.utils.xml_upload import xml_upload
 
 logger = get_logger(__name__)
 
 
 def make_parser() -> argparse.ArgumentParser:
     """
@@ -239,14 +239,19 @@
         type=int,
         help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)",
     )
     parser_stackup.add_argument("--prune", action="store_true", help="execute 'docker system prune' without asking")
     parser_stackup.add_argument(
         "--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)"
     )
+    parser_stackup.add_argument(
+        "--latest",
+        action="store_true",
+        help="use the latest dev version of DSP-API, from the main branch of the GitHub repository",
+    )
 
     # shutdown DSP-API
     parser_stackdown = subparsers.add_parser(
         name="stop-stack", help="Shut down the local instance of DSP-API and DSP-APP, and delete all data in it"
     )
     parser_stackdown.set_defaults(action="stop-stack")
 
@@ -429,21 +434,26 @@
     elif args.action == "excel2xml":
         success = excel2xml(
             datafile=args.data_source,
             shortcode=args.project_shortcode,
             default_ontology=args.ontology_name,
         )
     elif args.action == "start-stack":
-        success = start_stack(
-            max_file_size=args.max_file_size,
-            enforce_docker_system_prune=args.prune,
-            suppress_docker_system_prune=args.no_prune,
+        stack_handler = StackHandler(
+            StackConfiguration(
+                max_file_size=args.max_file_size,
+                enforce_docker_system_prune=args.prune,
+                suppress_docker_system_prune=args.no_prune,
+                latest_dev_version=args.latest,
+            )
         )
+        success = stack_handler.start_stack()
     elif args.action == "stop-stack":
-        success = stop_stack()
+        stack_handler = StackHandler(StackConfiguration())
+        success = stack_handler.stop_stack()
     elif args.action == "template":
         success = generate_template_repo()
     elif args.action == "rosetta":
         success = upload_rosetta()
     else:
         success = False
         print(f"ERROR: Unknown action '{args.action}'")
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/excel2xml.py` & `dsp_tools-2.4.0/src/dsp_tools/excel2xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#the-root-element-knora
     """
     schema_url = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/data.xsd"
     schema_location_key = str(etree.QName("http://www.w3.org/2001/XMLSchema-instance", "schemaLocation"))
     schema_location_value = f"https://dasch.swiss/schema {schema_url}"
     root = etree.Element(
-        "{%s}knora" % (xml_namespace_map[None]),
+        "{%s}knora" % xml_namespace_map[None],
         attrib={
             schema_location_key: schema_location_value,
             "shortcode": shortcode,
             "default-ontology": default_ontology,
         },
         nsmap=xml_namespace_map,
     )
@@ -312,15 +312,15 @@
     """
 
     PERMISSIONS = E.permissions
     ALLOW = E.allow
     # lxml.builder.E is a more sophisticated element factory than etree.Element.
     # E.tag is equivalent to E("tag") and results in <tag>
 
-    res_default = etree.Element("{%s}permissions" % (xml_namespace_map[None]), id="res-default")
+    res_default = etree.Element("{%s}permissions" % xml_namespace_map[None], id="res-default")
     res_default.append(ALLOW("V", group="UnknownUser"))
     res_default.append(ALLOW("V", group="KnownUser"))
     res_default.append(ALLOW("D", group="ProjectMember"))
     res_default.append(ALLOW("CR", group="ProjectAdmin"))
     res_default.append(ALLOW("CR", group="Creator"))
     root_element.append(res_default)
 
@@ -397,15 +397,15 @@
         except BaseError:
             raise BaseError(
                 f"The resource '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
                 f"Did you perhaps forget the timezone?"
             ) from None
         kwargs["creation_date"] = creation_date
 
-    resource_ = etree.Element("{%s}resource" % (xml_namespace_map[None]), **kwargs)  # type: ignore
+    resource_ = etree.Element("{%s}resource" % xml_namespace_map[None], **kwargs)  # type: ignore[arg-type]
     return resource_
 
 
 def make_bitstream_prop(
     path: Union[str, os.PathLike[Any]],
     permissions: str = "prop-default",
     calling_resource: str = "",
@@ -435,24 +435,24 @@
     if not os.path.isfile(path):
         warnings.warn(
             f"Failed validation in bitstream tag of resource '{calling_resource}': "
             f"The following path doesn't point to a file: {path}",
             stacklevel=2,
         )
     prop_ = etree.Element(
-        "{%s}bitstream" % (xml_namespace_map[None]),
+        "{%s}bitstream" % xml_namespace_map[None],
         permissions=permissions,
         nsmap=xml_namespace_map,
     )
     prop_.text = str(path)
     return prop_
 
 
 def _format_bool(
-    unformatted: Union[bool, str, int],
+    unformatted: Union[bool, str, int, float],
     name: str,
     calling_resource: str,
 ) -> str:
     """
     This method takes an unformatted boolean-like value, and transforms it into the string values "true" or "false".
 
     Args:
@@ -464,17 +464,17 @@
         BaseError: if the input cannot be transformed into "true"/"false"
 
     Returns:
         "true" if the input is in (True, "true", "1", 1, "yes"); "false" if input is in (False, "false", "0", 0, "no")
     """
     if isinstance(unformatted, str):
         unformatted = unformatted.lower()
-    if unformatted in (False, "false", "0", 0, "no"):
+    if unformatted in (False, "false", "0", 0, 0.0, "no"):
         return "false"
-    elif unformatted in (True, "true", "1", 1, "yes"):
+    elif unformatted in (True, "true", "1", 1, 1.0, "yes"):
         return "true"
     else:
         raise BaseError(
             f"Failed validation in resource '{calling_resource}', property '{name}': "
             f"'{unformatted}' is not a valid boolean."
         )
 
@@ -514,37 +514,37 @@
                 </boolean-prop>
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#boolean-prop
     """
 
     # validate input
     if isinstance(value, PropertyElement):
-        value_new = dataclasses.replace(value, value=_format_bool(value.value, name, calling_resource))  # type: ignore
+        value_new = dataclasses.replace(value, value=_format_bool(value.value, name, calling_resource))
     elif isinstance(value, (str, bool, int)):
         value_new = PropertyElement(_format_bool(value, name, calling_resource))
     else:
         raise BaseError(
             f"Failed validation in resource '{calling_resource}', property '{name}': '{value}' is not a valid boolean."
         )
 
     # make xml structure of the value
     prop_ = etree.Element(
-        "{%s}boolean-prop" % (xml_namespace_map[None]),
+        "{%s}boolean-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     kwargs = {"permissions": value_new.permissions}
-    if check_notna(value_new.comment):
-        kwargs["comment"] = value_new.comment  # type: ignore
+    if value_new.comment and check_notna(value_new.comment):
+        kwargs["comment"] = value_new.comment
     value_ = etree.Element(
-        "{%s}boolean" % (xml_namespace_map[None]),
-        **kwargs,  # type: ignore
+        "{%s}boolean" % xml_namespace_map[None],
+        **kwargs,  # type: ignore[arg-type]
         nsmap=xml_namespace_map,
     )
-    value_.text = value_new.value  # type: ignore
+    value_.text = str(value_new.value)
     prop_.append(value_)
 
     return prop_
 
 
 def make_color_prop(
     name: str,
@@ -593,25 +593,25 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid color."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}color-prop" % (xml_namespace_map[None]),
+        "{%s}color-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}color" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}color" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(val.value).strip()
         prop_.append(value_)
 
     return prop_
 
@@ -674,25 +674,25 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid DSP date."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}date-prop" % (xml_namespace_map[None]),
+        "{%s}date-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}date" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}date" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(val.value).strip()
         prop_.append(value_)
 
     return prop_
 
@@ -747,25 +747,25 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid decimal number."
             ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}decimal-prop" % (xml_namespace_map[None]),
+        "{%s}decimal-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}decimal" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}decimal" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(float(val.value))
         prop_.append(value_)
 
     return prop_
 
@@ -810,36 +810,36 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         try:
-            value_as_dict = json.loads(val.value)  # type: ignore
+            value_as_dict = json.loads(str(val.value))
             assert value_as_dict["type"] in ["rectangle", "circle", "polygon"]
             assert isinstance(value_as_dict["points"], list)
         except (json.JSONDecodeError, TypeError, IndexError, KeyError, AssertionError):
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid JSON geometry object."
             ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}geometry-prop" % (xml_namespace_map[None]),
+        "{%s}geometry-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}geometry" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}geometry" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(val.value)
         prop_.append(value_)
     return prop_
 
 
@@ -891,25 +891,25 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a geonames.org identifier."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}geoname-prop" % (xml_namespace_map[None]),
+        "{%s}geoname-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}geoname" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}geoname" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
@@ -964,25 +964,25 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid integer."
             ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}integer-prop" % (xml_namespace_map[None]),
+        "{%s}integer-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}integer" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}integer" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
         value_.text = str(int(val.value))
         prop_.append(value_)
 
     return prop_
 
@@ -1034,28 +1034,28 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid DSP interval."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}interval-prop" % (xml_namespace_map[None]),
+        "{%s}interval-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}interval" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}interval" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
-        value_.text = val.value  # type: ignore
+        value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_list_prop(
     list_name: str,
@@ -1106,29 +1106,29 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid name of a list node."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}list-prop" % (xml_namespace_map[None]),
+        "{%s}list-prop" % xml_namespace_map[None],
         list=list_name,
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}list" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}list" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
-        value_.text = val.value  # type: ignore
+        value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_resptr_prop(
     name: str,
@@ -1177,28 +1177,28 @@
             raise BaseError(
                 f"Validation Error in resource '{calling_resource}', property '{name}': "
                 f"The following doesn't seem to be a valid ID of a target resource: '{val.value}'"
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}resptr-prop" % (xml_namespace_map[None]),
+        "{%s}resptr-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}resptr" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}resptr" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
-        value_.text = val.value  # type: ignore
+        value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_text_prop(
     name: str,
@@ -1256,28 +1256,28 @@
                 f"Warning for resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is probably not a usable string.",
                 stacklevel=2,
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}text-prop" % (xml_namespace_map[None]),
+        "{%s}text-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         if check_notna(val.encoding):
             kwargs["encoding"] = val.encoding  # type: ignore
         else:
             kwargs["encoding"] = "utf8"
         value_ = etree.Element(
-            "{%s}text" % (xml_namespace_map[None]),
+            "{%s}text" % xml_namespace_map[None],
             **kwargs,  # type: ignore
             nsmap=xml_namespace_map,
         )
         if kwargs["encoding"] == "utf8":
             # write the text into the tag, without validation
             value_.text = str(val.value)
         else:
@@ -1356,28 +1356,28 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid DSP time."
             )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}time-prop" % (xml_namespace_map[None]),
+        "{%s}time-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}time" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}time" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
-        value_.text = val.value  # type: ignore
+        value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_uri_prop(
     name: str,
@@ -1428,28 +1428,28 @@
             raise BaseError(
                 f"Failed validation in resource '{calling_resource}', property '{name}': "
                 f"'{val.value}' is not a valid URI."
             ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
-        "{%s}uri-prop" % (xml_namespace_map[None]),
+        "{%s}uri-prop" % xml_namespace_map[None],
         name=name,
         nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
-        if check_notna(val.comment):
-            kwargs["comment"] = val.comment  # type: ignore
+        if val.comment and check_notna(val.comment):
+            kwargs["comment"] = val.comment
         value_ = etree.Element(
-            "{%s}uri" % (xml_namespace_map[None]),
-            **kwargs,  # type: ignore
+            "{%s}uri" % xml_namespace_map[None],
+            **kwargs,  # type: ignore[arg-type]
             nsmap=xml_namespace_map,
         )
-        value_.text = val.value  # type: ignore
+        value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_region(
     label: str,
@@ -1501,16 +1501,16 @@
             raise BaseError(
                 f"The region '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
                 f"Did you perhaps forget the timezone?"
             ) from None
         kwargs["creation_date"] = creation_date
 
     region_ = etree.Element(
-        "{%s}region" % (xml_namespace_map[None]),
-        **kwargs,  # type: ignore
+        "{%s}region" % xml_namespace_map[None],
+        **kwargs,  # type: ignore[arg-type]
     )
     return region_
 
 
 def make_annotation(
     label: str,
     id: str,  # pylint: disable=redefined-builtin
@@ -1559,16 +1559,16 @@
             raise BaseError(
                 f"The annotation '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
                 f"Did you perhaps forget the timezone?"
             ) from None
         kwargs["creation_date"] = creation_date
 
     annotation_ = etree.Element(
-        "{%s}annotation" % (xml_namespace_map[None]),
-        **kwargs,  # type: ignore
+        "{%s}annotation" % xml_namespace_map[None],
+        **kwargs,  # type: ignore[arg-type]
     )
     return annotation_
 
 
 def make_link(
     label: str,
     id: str,  # pylint: disable=redefined-builtin
@@ -1617,16 +1617,16 @@
             raise BaseError(
                 f"The link '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
                 f"Did you perhaps forget the timezone?"
             ) from None
         kwargs["creation_date"] = creation_date
 
     link_ = etree.Element(
-        "{%s}link" % (xml_namespace_map[None]),
-        **kwargs,  # type: ignore
+        "{%s}link" % xml_namespace_map[None],
+        **kwargs,  # type: ignore[arg-type]
     )
     return link_
 
 
 def create_json_excel_list_mapping(
     path_to_json: str,
     list_name: str,
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
     Raises:
         BaseError: if a referenced file doesn't exist in the file system
 
     Returns:
         list of all paths in the <bitstream> tags
     """
-    tree: etree._ElementTree = etree.parse(xml_file)  # type: ignore
+    tree: etree._ElementTree[etree._Element] = etree.parse(xml_file)
     bitstream_paths: set[Path] = set()
     for x in tree.iter():
         if x.text and etree.QName(x).localname.endswith("bitstream"):
             path = Path(x.text)
             if path.is_file():
                 bitstream_paths.add(path)
             else:
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.4.0/src/dsp_tools/models/bitstream.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 
     def __init__(self, value: str, permissions: Optional[Permissions] = None):
         self._value = value
         self._permissions = permissions
 
     @property
     def value(self) -> str:
+        """File path of the bitstream"""
         return self._value
 
     @property
     def permissions(self) -> Optional[Permissions]:
+        """Permissions of the bitstream"""
         return self._permissions
 
-    def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
+    def toJsonLdObj(self, action: Actions) -> dict[str, Any]:  # pylint: disable=missing-function-docstring
         tmp = {}
         if action == Actions.Create:
             tmp["knora-api:fileValueHasFilename"] = self._value
             if self._permissions:
                 tmp["knora-api:hasPermissions"] = self.permissions.toJsonLdObj()
         return tmp
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/connection.py` & `dsp_tools-2.4.0/src/dsp_tools/models/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,20 +80,23 @@
         :return: token string
         """
 
         return self._token
 
     @property
     def token(self) -> str:
+        """Get the token of this connection"""
         return self._token
 
     def start_logging(self) -> None:
+        """Start writing every API call to a file"""
         self._log = True
 
     def stop_logging(self):
+        """Stop writing every API call to a file"""
         self._log = False
 
     def logout(self) -> None:
         """
         Performs a logout
         :return: None
         """
@@ -115,43 +118,48 @@
         """
         Post Json data to a given server using a HTTP POST request
         :param path: Path of RESTful route
         :param jsondata: Valid JSON as string
         :return: Response from server
         """
 
+        # timeout must be None,
+        # otherwise the client can get a timeout error while the API is still processing the request
+        # in that case, the client's retry will fail, and the response of the original API call is lost
+        timeout = None
+
         if path[0] != "/":
             path = "/" + path
         headers = None
         if jsondata is None:
             if self._token is not None:
                 headers = {"Authorization": "Bearer " + self._token}
                 response = requests.post(
                     self._server + path,
                     headers=headers,
-                    timeout=5,
+                    timeout=timeout,
                 )
             else:
-                response = requests.post(self._server + path, timeout=5)
+                response = requests.post(self._server + path, timeout=timeout)
         else:
             if self._token is not None:
                 headers = {"Content-Type": "application/json; charset=UTF-8", "Authorization": "Bearer " + self._token}
                 response = requests.post(
                     self._server + path,
                     headers=headers,
                     data=jsondata,
-                    timeout=5,
+                    timeout=timeout,
                 )
             else:
                 headers = {"Content-Type": "application/json; charset=UTF-8"}
                 response = requests.post(
                     self._server + path,
                     headers=headers,
                     data=jsondata,
-                    timeout=5,
+                    timeout=timeout,
                 )
         if self._log:
             if jsondata:
                 jsonobj = json.loads(jsondata)
             else:
                 jsonobj = None
             logobj = {
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.4.0/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/group.py` & `dsp_tools-2.4.0/src/dsp_tools/models/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-function-docstring
+
 """
 This module implements the handling (CRUD) of DSP groups.
 
 CREATE:
     * Instantiate a new object of the class Group with all required parameters
     * Call the ``create``-method on the instance
 
@@ -31,15 +33,15 @@
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Actions
 from dsp_tools.models.langstring import LangString
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 
 
-class Group(Model):
+class Group(Model):  # pylint: disable=too-many-instance-attributes
     """
     This class represents a DSP group
 
     Attributes
     ----------
 
     con : Connection
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/helpers.py` & `dsp_tools-2.4.0/src/dsp_tools/models/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 import re
 from dataclasses import dataclass
 from enum import Enum, unique
 from typing import Any, Optional, Pattern, Union
 
 from dsp_tools.models.exceptions import BaseError
 
@@ -23,15 +25,15 @@
     iri: str
     hashtag: bool
 
 
 ContextType = dict[str, OntoIri]
 
 
-class IriTest:
+class IriTest:  # pylint: disable=too-few-public-methods
     __iri_regexp = re.compile("^(http)s?://([\\w\\.\\-~]+)?(:\\d{,6})?(/[\\w\\-~]+)*(#[\\w\\-~]*)?")
 
     @classmethod
     def test(cls, val: str) -> bool:
         m = cls.__iri_regexp.match(val)
         return m.span()[1] == len(val) if m else False
 
@@ -48,22 +50,22 @@
 class Cardinality(Enum):
     C_1 = "1"
     C_0_1 = "0-1"
     C_1_n = "1-n"
     C_0_n = "0-n"
 
 
-class ContextIterator:
+class ContextIterator:  # pylint: disable=too-few-public-methods
     _context: "Context"
     _prefixes: list[str]
     _index: int
 
     def __init__(self, context: "Context"):
         self._context = context
-        self._prefixes = [x for x in self._context.context]
+        self._prefixes = list(self._context.context)
         self._index = 0
 
     def __next__(self) -> tuple[Optional[str], Optional[OntoIri]]:
         if len(self._context.context) == 0 and self._index == 0:
             return None, None
         elif self._index < len(self._context.context):
             tmp = self._prefixes[self._index]
@@ -441,15 +443,15 @@
     def __str__(self: "DateTimeStamp") -> Union[None, str]:
         return self._dateTimeStamp
 
     def toJsonObj(self):
         return {"@type": "xsd:dateTimeStamp", "@value": self._dateTimeStamp}
 
 
-class WithId:
+class WithId:  # pylint: disable=too-few-public-methods
     """
     Class helper to get json-ld "@id" thingies
     """
 
     _tmp: str = None
 
     def __init__(self, obj: Optional[dict[str, str]]):
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/langstring.py` & `dsp_tools-2.4.0/src/dsp_tools/models/langstring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+# pylint: disable=missing-function-docstring
+
 from enum import Enum, unique
 from typing import Any, Optional, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 
 @unique
 class Languages(Enum):
+    """Languages supported by DSP"""
+
     EN = "en"
     DE = "de"
     FR = "fr"
     IT = "it"
     RM = "rm"
 
 
 LangStringParam = Optional[Union[dict[Union[Languages, str], str], str]]
 
 
-class LangStringIterator:
+class LangStringIterator:  # pylint: disable=too-few-public-methods
     """Iterator class for LangString class."""
 
     _langstring: "LangString"
     _index: int
 
     def __init__(self, langstring: "LangString"):
         self._langstring = langstring
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/listnode.py` & `dsp_tools-2.4.0/src/dsp_tools/models/listnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-function-docstring
+
 """
 This module implements the handling (CRUD) of list nodes and adds some function to read whole lists.
 
 CREATE:
     * Instantiate a new object of the class ListNode
     * Call the ``create`` method on the instance
 
@@ -33,33 +35,33 @@
 from dsp_tools.models.project import Project
 from dsp_tools.models.set_encoder import SetEncoder
 
 
 def list_creator(con: Connection, project: Project, parent_node: "ListNode", nodes: list[dict]) -> list["ListNode"]:
     nodelist: list[ListNode] = []
 
-    for node in nodes:
+    for n in nodes:
         new_node = ListNode(
             con=con,
             project=project,
-            label=node["labels"],
-            comments=node.get("comments"),
-            name=node["name"],
+            label=n["labels"],
+            comments=n.get("comments"),
+            name=n["name"],
             parent=parent_node,
         )
 
-        if node.get("nodes"):
-            new_node.children = list_creator(con, project, new_node, node["nodes"])
+        if n.get("nodes"):
+            new_node.children = list_creator(con, project, new_node, n["nodes"])
 
         nodelist.append(new_node)
 
     return nodelist
 
 
-class ListNode(Model):
+class ListNode(Model):  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     """
     This class represents a list node
 
     Attributes
     ----------
 
     con : Connection
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/ontology.py` & `dsp_tools-2.4.0/src/dsp_tools/models/ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 """
 This model implements the handling of ontologies. It is to note that ResourceClasses, PropertyClasses
 as well as the assignment of PropertyCLasses to the ResourceClasses (with a given cardinality)
 is handled in "cooperation" with the propertyclass.py (PropertyClass) and resourceclass.py (ResourceClass
 and HasProperty) modules.
 
 CREATE:
@@ -37,15 +39,15 @@
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 from dsp_tools.models.propertyclass import PropertyClass
 from dsp_tools.models.resourceclass import ResourceClass
 from dsp_tools.models.set_encoder import SetEncoder
 
 
-class Ontology(Model):
+class Ontology(Model):  # pylint: disable=too-many-instance-attributes
     ROUTE: str = "/v2/ontologies"
     METADATA: str = "/metadata/"
     ALL_LANGUAGES: str = "?allLanguages=true"
 
     _iri: str
     _project: str
     _name: str
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/permission.py` & `dsp_tools-2.4.0/src/dsp_tools/models/permission.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 import re
 from enum import Enum, unique
 from typing import Optional, Union
 
 
 @unique
 class PermissionValue(Enum):
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/project.py` & `dsp_tools-2.4.0/src/dsp_tools/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 """
 This module implements the handling (CRUD) of DSP projects.
 
 CREATE:
     * Instantiate a new object of the class Project with all required parameters
     * Call the ``create``-method on the instance
 
@@ -32,15 +34,15 @@
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Actions
 from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.set_encoder import SetEncoder
 
 
-class Project(Model):
+class Project(Model):  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     """
     This class represents a project in DSP.
 
     Attributes
     ----------
 
     con : Connection
@@ -412,15 +414,15 @@
 
     def createDefinitionFileObj(self) -> dict[str, Any]:
         return {
             "shortcode": self._shortcode,
             "shortname": self._shortname,
             "longname": self._longname,
             "descriptions": self._description.createDefinitionFileObj(),
-            "keywords": [kw for kw in self._keywords],
+            "keywords": list(self._keywords),
         }
 
     def create(self) -> Project:
         """
         Create a new project in DSP
 
         :return: JSON-object from DSP
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.4.0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.4.0/src/dsp_tools/models/propertyclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring,duplicate-code
+
 import json
 import re
 from typing import Any, Optional, Sequence, Union
 from urllib.parse import quote_plus
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
 from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.model import Model
 from dsp_tools.models.set_encoder import SetEncoder
 
 
-class PropertyClass(Model):
+class PropertyClass(Model):  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     ROUTE: str = "/v2/ontologies/properties"
 
     _context: Context
     _iri: str
     _name: str
     _ontology_id: str
     _superproperties: list[str]
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.4.0/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/resource.py` & `dsp_tools-2.4.0/src/dsp_tools/models/resource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.4.0/src/dsp_tools/models/resourceclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 This model implements the handling of resource classes. It contains two classes that work closely together:
     * "HasProperty" deals with the association of Property-instances with the Resource-instances. This association
       is done using the "cardinality"-clause
     * "ResourceClass" is the main class representing a DSP resource class.
 """
 
+# pylint: disable=missing-class-docstring,missing-function-docstring,too-many-instance-attributes,duplicate-code
+
 import json
 import re
 from enum import Enum
 from typing import Any, Optional, Sequence, Union
 from urllib.parse import quote_plus
 
 from dsp_tools.models.connection import Connection
@@ -40,15 +42,14 @@
         con: Connection,
         context: Context,
         ontology_id: Optional[str] = None,
         property_id: Optional[str] = None,
         resclass_id: Optional[str] = None,
         cardinality: Optional[Cardinality] = None,
         gui_order: Optional[int] = None,
-        is_inherited: Optional[bool] = None,
         ptype: Optional[Ptype] = None,
     ):
         super().__init__(con)
         if not isinstance(context, Context):
             raise BaseError('"context"-parameter must be an instance of Context')
         self._context = context
         if ontology_id is not None:
@@ -124,20 +125,14 @@
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
         salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
 
         if jsonld_obj.get("@type") is None or jsonld_obj.get("@type") != owl + ":Restriction":
             raise BaseError("Expected restriction type")
 
         #
-        # let's get the inherited field...
-        #
-        tmp = jsonld_obj.get(knora_api + ":isInherited")
-        is_inherited = tmp if tmp is not None else False
-
-        #
         # let's get the cardinality
         #
         cardinality: Cardinality
         if jsonld_obj.get(owl + ":cardinality") is not None:
             cardinality = Cardinality.C_1
         elif jsonld_obj.get(owl + ":maxCardinality") is not None:
             cardinality = Cardinality.C_0_1
@@ -178,15 +173,14 @@
         return property_id, cls(
             con=con,
             context=context,
             ontology_id=ontology_id,
             property_id=property_id,
             cardinality=cardinality,
             gui_order=gui_order,
-            is_inherited=is_inherited,
             ptype=ptype,
         )
 
     def toJsonObj(self, lastModificationDate: DateTimeStamp, action: Actions) -> Any:
         if self._cardinality is None:
             raise BaseError("There must be a cardinality given!")
         tmp = {}
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/sipi.py` & `dsp_tools-2.4.0/src/dsp_tools/models/sipi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=too-few-public-methods
+
 import os
 from typing import Any
 
 import requests
 
 from dsp_tools.models.connection import check_for_api_error
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/user.py` & `dsp_tools-2.4.0/src/dsp_tools/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from dsp_tools.models.group import Group
 from dsp_tools.models.helpers import Actions
 from dsp_tools.models.langstring import Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 
 
-class User(Model):
+class User(Model):  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     """
     This class represents a user in DSP.
 
     Attributes
     ----------
 
     iri : str
@@ -213,77 +213,68 @@
         self._rm_from_project = {}
         self._change_admin = {}
         self._add_to_group = set()
         self._rm_from_group = set()
 
     @property
     def iri(self) -> Optional[str]:
+        """IRI of this user"""
         return self._iri
 
-    @iri.setter
-    def iri(self, value: str) -> None:
-        raise BaseError("User iri cannot be modified!")
-
     @property
     def username(self) -> Optional[str]:
+        """Username of this user"""
         return self._username
 
     @username.setter
     def username(self, value: Optional[str]):
         if value is None:
             return
         self._username = str(value)
         self._changed.add("username")
 
     @property
     def email(self) -> Optional[str]:
+        """Email address of this user"""
         return self._email
 
     @email.setter
     def email(self, value: Optional[str]):
         if value is None:
             return
         self._email = str(value)
         self._changed.add("email")
 
     @property
     def givenName(self) -> Optional[str]:
+        """Given name (firstname) of this user"""
         return self._givenName
 
     @givenName.setter
     def givenName(self, value: Optional[str]):
         if value is None:
             return
         self._givenName = str(value)
         self._changed.add("givenName")
 
     @property
     def familyName(self) -> Optional[str]:
+        """Family name (lastname) of this user"""
         return self._familyName
 
     @familyName.setter
     def familyName(self, value: Optional[str]):
         if value is None:
             return
         self._familyName = str(value)
         self._changed.add("familyName")
 
     @property
-    def password(self) -> Optional[str]:
-        return None
-
-    @password.setter
-    def password(self, value: Optional[str]):
-        if value is None:
-            return
-        self._password = str(value)
-        self._changed.add("password")
-
-    @property
     def lang(self) -> Optional[Languages]:
+        """Language of this user"""
         return self._lang
 
     @lang.setter
     def lang(self, value: Optional[Union[str, Languages]]):
         if value is None:
             return
         if isinstance(value, Languages):
@@ -294,40 +285,39 @@
             if lmap.get(value) is None:
                 raise BaseError('Invalid language string "' + value + '"!')
             self._lang = lmap[value]
             self._changed.add("lang")
 
     @property
     def status(self) -> bool:
+        """Status of this user (True=active, False=inactive)"""
         return self._status
 
     @status.setter
     def status(self, value: Optional[bool]) -> None:
         self._status = None if value is None else bool(value)
         if value is not None:
             self._changed.add("status")
 
     @property
     def sysadmin(self) -> bool:
+        """True if the user is sysadmin"""
         return self._sysadmin
 
     @sysadmin.setter
     def sysadmin(self, value: bool):
         self._sysadmin = None if value is None else bool(value)
         if value is not None:
             self._changed.add("sysadmin")
 
     @property
     def in_groups(self) -> set[str]:
+        """Set of group IRI's the user is member of"""
         return self._in_groups
 
-    @in_groups.setter
-    def in_groups(self, value: Any):
-        raise BaseError('Group membership cannot be modified directly! Use methods "addToGroup" and "rmFromGroup"')
-
     def addToGroup(self, value: str):
         """
         Add the user to the given group (executed at next update)
 
         :param value: IRI of the group
         :return: None
         """
@@ -354,22 +344,17 @@
             self._rm_from_group.add(value)
             self._changed.add("in_groups")
         else:
             raise BaseError("User is not in groups!")
 
     @property
     def in_projects(self) -> dict[str, bool]:
+        """dict with project-IRI as key, boolean(True=project admin) as value"""
         return self._in_projects
 
-    @in_projects.setter
-    def in_projects(self, value: Any):
-        raise BaseError(
-            'Project membership cannot be modified directly! Use methods "addToProject" and "rmFromProject"'
-        )
-
     def addToProject(self, value: str, padmin: bool = False):
         """
         Add the user to the given project (executed at next update)
 
         :param value: project IRI
         :param padmin: True, if user should be project admin, False otherwise
         :return: None
@@ -588,29 +573,29 @@
         :param requesterPassword: Old password if a user wants to change it's own password
         :return: JSON-object from DSP
         """
 
         jsonobj = self.toJsonObj(Actions.Update)
         if jsonobj:
             jsondata = json.dumps(jsonobj)
-            self._con.put(User.IRI + quote_plus(self.iri) + "/BasicUserInformation", jsondata)
+            self._con.put(User.IRI + quote_plus(self._iri) + "/BasicUserInformation", jsondata)
         if "status" in self._changed:
             jsonobj = {"status": self._status}
             jsondata = json.dumps(jsonobj)
-            self._con.put(User.IRI + quote_plus(self.iri) + "/Status", jsondata)
+            self._con.put(User.IRI + quote_plus(self._iri) + "/Status", jsondata)
         if "password" in self._changed:
             if requesterPassword is None:
                 raise BaseError("Requester's password is missing!")
             jsonobj = {"requesterPassword": requesterPassword, "newPassword": self._password}
             jsondata = json.dumps(jsonobj)
-            self._con.put(User.IRI + quote_plus(self.iri) + "/Password", jsondata)
+            self._con.put(User.IRI + quote_plus(self._iri) + "/Password", jsondata)
         if "sysadmin" in self._changed:
             jsonobj = {"systemAdmin": self._sysadmin}
             jsondata = json.dumps(jsonobj)
-            self._con.put(User.IRI + quote_plus(self.iri) + "/SystemAdmin", jsondata)
+            self._con.put(User.IRI + quote_plus(self._iri) + "/SystemAdmin", jsondata)
         for p in self._add_to_project.items():
             self._con.post(User.IRI + quote_plus(self._iri) + User.PROJECT_MEMBERSHIPS + quote_plus(p[0]))
             if p[1]:
                 self._con.post(User.IRI + quote_plus(self._iri) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0]))
 
         for p in self._rm_from_project:
             if self._in_projects.get(p) is not None and self._in_projects[p]:
@@ -672,34 +657,35 @@
 
     def createDefinitionFileObj(
         self,
         con: Connection,
         proj_shortname: str,
         proj_iri: str,
     ) -> dict[str, Union[str, list[str], None]]:
+        """Create a JSON object that can be used to create a project definition file"""
         user: dict[str, Union[str, list[str], bool, None]] = {
             "username": self.username,
-            "email": self.email,
-            "givenName": self.givenName,
-            "familyName": self.familyName,
+            "email": self._email,
+            "givenName": self._givenName,
+            "familyName": self._familyName,
             "password": "",
         }
-        if self.lang:
-            user["lang"] = self.lang.value
+        if self._lang:
+            user["lang"] = self._lang.value
         groups = list()
         for group_iri in self._in_groups:
             group_info = con.get(f"/admin/groups/{urllib.parse.quote_plus(group_iri)}")
             if "group" in group_info and "name" in group_info["group"]:
                 groupname = group_info["group"]["name"]
                 groups.append(f"{proj_shortname}:{groupname}")
-        if self.sysadmin:
+        if self._sysadmin:
             groups.append("SystemAdmin")
         user["groups"] = groups
         user["projects"] = list()
         for proj, is_admin in self._in_projects.items():
             if proj == proj_iri:
                 if is_admin:
                     user["projects"].append(f"{proj_shortname}:admin")
                 else:
                     user["projects"].append(f"{proj_shortname}:member")
-        user["status"] = self.status
+        user["status"] = self._status
         return user
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/value.py` & `dsp_tools-2.4.0/src/dsp_tools/models/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 import re
 from typing import Any, Optional, Union
 
 import regex
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Actions, IriTest
@@ -250,15 +252,15 @@
             tmp["knora-api:colorValueAsColor"] = self._value
         return tmp
 
     def __str__(self) -> str:
         return self._value + " " + super().__str__()
 
 
-class DateValue(Value):
+class DateValue(Value):  # pylint: disable=too-many-instance-attributes
     _calendar: str
     _e1: str
     _y1: int
     _m1: int
     _d1: int
     _e2: str
     _y2: int
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlresource.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dsp_tools.models.helpers import DateTimeStamp
 from dsp_tools.models.permission import Permissions
 from dsp_tools.models.value import KnoraStandoffXml
 from dsp_tools.models.xmlbitstream import XMLBitstream
 from dsp_tools.models.xmlproperty import XMLProperty
 
 
-class XMLResource:
+class XMLResource:  # pylint: disable=too-many-instance-attributes
     """Represents a resource in the XML used for data import"""
 
     _id: str
     _iri: Optional[str]
     _ark: Optional[str]
     _label: str
     _restype: str
@@ -102,14 +102,15 @@
     @property
     def bitstream(self) -> Optional[XMLBitstream]:
         """The bitstream object belonging to the resource"""
         return self._bitstream
 
     @property
     def properties(self) -> list[XMLProperty]:
+        """The list of properties of the resource"""
         return self._properties
 
     @properties.setter
     def properties(self, new_properties: list[XMLProperty]) -> None:
         self._properties = new_properties
 
     def get_props_with_links(self) -> list[XMLProperty]:
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.4.0/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.4.0/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.4.0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.4.0/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.4.0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.4.0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 ---
 
 version: '3.7'
 
 services:
 
   app:
-    image: daschswiss/dsp-app:v10.21.0  # on the verge of every deployment (fortnightly), update this from the "app" value of
-                                        # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    # on the verge of every deployment (fortnightly), update the "image" value from the "app" value of
+    # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    image: daschswiss/dsp-app:v10.22.0
     ports:
       - "4200:4200"
     networks:
       - knora-net
 
   db:
-    image: daschswiss/apache-jena-fuseki:2.0.11  # on the verge of every deployment (fortnightly), update this from the "db" value of
-                                                 # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    # on the verge of every deployment (fortnightly), update the "image" value from the "db" value of
+    # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    image: daschswiss/apache-jena-fuseki:2.0.11
     ports:
       - "3030:3030"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
-    image: daschswiss/knora-sipi:29.0.1  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    image: daschswiss/knora-sipi:29.1.0
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -40,16 +43,17 @@
       - SIPI_WEBAPI_HOSTNAME=api
       - SIPI_WEBAPI_PORT=3333
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
-    image: daschswiss/knora-api:29.0.1  # on the verge of every deployment (fortnightly), update this from the "api" value of
-                                        # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    # on the verge of every deployment (fortnightly), update the "image" value from the "api" value of
+    # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
+    image: daschswiss/knora-api:29.1.0
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,56 +22,57 @@
 """Module level variable used to ensure that there are no duplicate node names"""
 
 
 def expand_lists_from_excel(
     lists_section: list[dict[str, Union[str, dict[str, Any]]]],
 ) -> list[dict[str, Any]]:
     """
-    Checks if the "lists" section of a JSON project file contains references to Excel files. Expands all Excel files to
-    JSON, and returns the expanded "lists" section. If there are no references to Excel files, the "lists" section is
-    returned as is.
-    Returns a tuple consisting of the expanded "lists" section and a boolean value: True if everything went smoothly,
-    False if one of the lists couldn't be expanded correctly.
+    Checks if the "lists" section of a JSON project file contains references to Excel files.
+    Expands all Excel files to JSON,
+    and returns the expanded "lists" section.
+    If there are no references to Excel files,
+    the "lists" section is returned as is.
 
     Args:
         lists_section: the "lists" section of a parsed JSON project file.
             If this is an empty list, an empty list will be returned.
 
     Raises:
         BaseError: if a problem occurred while trying to expand the Excel files
 
     Returns:
         the same "lists" section, but without references to Excel files
     """
     new_lists = []
     for _list in lists_section:
+        # case 1: this list is a JSON list: return it as it is
         if "folder" not in _list["nodes"]:
-            # this list is a JSON list: return it as it is
             new_lists.append(_list)
-        else:
-            # this is a reference to a folder with Excel files
-            foldername = _list["nodes"]["folder"]  # type: ignore
-            excel_file_paths = _extract_excel_file_paths(foldername)
-            try:
-                returned_lists_section = _make_json_lists_from_excel(excel_file_paths, verbose=False)
-                # we only need the "nodes" section of the first element of the returned "lists" section. This "nodes"
-                # section needs to replace the Excel folder reference. But the rest of the user-defined list element
-                # needs to stay intact, e.g. the labels and comments.
-                _list["nodes"] = returned_lists_section[0]["nodes"]
-                new_lists.append(_list)
-                print(
-                    f"\tThe list '{_list['name']}' contains a reference to the folder '{foldername}'. The Excel "
-                    f"files therein have been temporarily expanded into the 'lists' section of your project."
-                )
-            except BaseError as err:
-                raise BaseError(
-                    f"\tWARNING: The list '{_list['name']}' contains a reference to the folder '{foldername}', but a "
-                    f"problem occurred while trying to expand the Excel files therein into the 'lists' section of "
-                    f"your project: {err.message}"
-                ) from None
+            continue
+
+        # case 2: this is a reference to a folder with Excel files
+        foldername = _list["nodes"]["folder"]  # type: ignore[index]  # types are too complex to annotate them correctly
+        excel_file_paths = _extract_excel_file_paths(foldername)
+        try:
+            returned_lists_section = _make_json_lists_from_excel(excel_file_paths, verbose=False)
+            # we only need the "nodes" section of the first element of the returned "lists" section. This "nodes"
+            # section needs to replace the Excel folder reference. But the rest of the user-defined list element
+            # needs to stay intact, e.g. the labels and comments.
+            _list["nodes"] = returned_lists_section[0]["nodes"]
+            new_lists.append(_list)
+            print(
+                f"\tThe list '{_list['name']}' contains a reference to the folder '{foldername}'. The Excel "
+                f"files therein have been temporarily expanded into the 'lists' section of your project."
+            )
+        except BaseError as err:
+            raise BaseError(
+                f"\tWARNING: The list '{_list['name']}' contains a reference to the folder '{foldername}', but a "
+                f"problem occurred while trying to expand the Excel files therein into the 'lists' section of "
+                f"your project: {err.message}"
+            ) from None
 
     return new_lists
 
 
 def _get_values_from_excel(
     excelfiles: dict[str, Worksheet],
     base_file: dict[str, Worksheet],
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # validate input
     # --------------
     if not os.path.isdir(data_model_files):
         raise BaseError(f"ERROR: {data_model_files} is not a directory.")
     folder = [x for x in os.scandir(data_model_files) if not re.search(r"^(\.|~\$).+", x.name)]
 
     processed_files = []
-    onto_folders = [x for x in folder if os.path.isdir(x) and re.search(r"([\w.-]+) (\([\w.\- ]+\))", x.name)]
+    onto_folders = [x for x in folder if os.path.isdir(x) and re.search(r"([\w.-]+) \(([\w.\- ]+)\)", x.name)]
     if len(onto_folders) == 0:
         raise BaseError(
             f"'{data_model_files}' must contain at least one subfolder named after the pattern 'onto_name (onto_label)'"
         )
     for onto_folder in onto_folders:
         contents = sorted([x.name for x in os.scandir(onto_folder) if not re.search(r"^(\.|~\$).+", x.name)])
         if contents != ["properties.xlsx", "resources.xlsx"]:
@@ -84,15 +84,15 @@
     # -------------
     lists, success = excel2lists(excelfolder=f"{data_model_files}/lists") if listfolder else (None, True)
     if not success:
         overall_success = False
 
     ontologies = []
     for onto_folder in onto_folders:
-        name, label = re.search(r"([\w.-]+) \(([\w.\- ]+)\)", onto_folder.name).groups()  # type: ignore
+        name, label = re.search(r"([\w.-]+) \(([\w.\- ]+)\)", onto_folder.name).groups()  # type: ignore[union-attr]
         resources, success1 = excel2resources(f"{data_model_files}/{onto_folder.name}/resources.xlsx")
         properties, success2 = excel2properties(f"{data_model_files}/{onto_folder.name}/properties.xlsx")
         if not success1 or not success2:
             overall_success = False
         ontologies.append(
             {
                 "name": name,
@@ -111,16 +111,16 @@
             "shortname": "",
             "longname": "",
             "descriptions": {"en": ""},
             "keywords": [""],
         },
     }
     if lists:
-        project["project"]["lists"] = lists  # type: ignore
-    project["project"]["ontologies"] = ontologies  # type: ignore
+        project["project"]["lists"] = lists  # type: ignore[index]
+    project["project"]["ontologies"] = ontologies  # type: ignore[index]
 
     with open(path_to_output_file, "w", encoding="utf-8") as f:
         json.dump(project, f, indent=4, ensure_ascii=False)
 
     print(f"JSON project file successfully saved at {path_to_output_file}")
 
     return overall_success
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/id_to_iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/logging.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/project_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         for all groups that have successfully been created (or already exist).
         The dict is empty if no group was created.
     """
     overall_success = True
     current_project_groups: dict[str, Group] = {}
     try:
         remote_groups: list[Group] = try_network_action(
-            lambda: Group.getAllGroupsForProject(con=con, proj_iri=project.iri)  # type: ignore
+            lambda: Group.getAllGroupsForProject(con=con, proj_iri=str(project.iri))
         )
     except BaseError:
         err_msg = (
             "Unable to check if group names are already existing on DSP server, because it is "
             "not possible to retrieve the remote groups from the DSP server."
         )
         print(f"WARNING: {err_msg}")
@@ -189,15 +189,15 @@
             group_remote: Group = try_network_action(group_local.create)
         except BaseError:
             print(f"\tWARNING: Unable to create group '{group_name}'.")
             logger.warning(f"Unable to create group '{group_name}'.", exc_info=True)
             overall_success = False
             continue
 
-        current_project_groups[group_remote.name] = group_remote  # type: ignore
+        current_project_groups[str(group_remote.name)] = group_remote
         print(f"\tCreated group '{group_name}'.")
 
     return current_project_groups, overall_success
 
 
 def _get_group_iris_for_user(
     json_user_definition: dict[str, str],
@@ -334,15 +334,15 @@
                 print(
                     f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. Skipping..."
                 )
                 success = False
                 continue
             in_project = in_project_list[0]
 
-        project_info[in_project.iri] = bool(project_role == "admin")  # type: ignore
+        project_info[str(in_project.iri)] = bool(project_role == "admin")
         if verbose:
             print(f"\tAdded user '{username}' as {project_role} to project '{in_project.shortname}'.")
 
     return project_info, success
 
 
 def _create_users(
@@ -596,15 +596,15 @@
     """
 
     overall_success = True
 
     print("Create ontologies...")
     try:
         project_ontologies: list[Ontology] = try_network_action(
-            lambda: Ontology.getProjectOntologies(con=con, project_id=project_remote.iri)  # type: ignore
+            lambda: Ontology.getProjectOntologies(con=con, project_id=str(project_remote.iri))
         )
     except BaseError:
         err_msg = "Unable to retrieve remote ontologies. Cannot check if your ontology already exists."
         print("WARNING: {err_msg}")
         logger.warning(err_msg, exc_info=True)
         project_ontologies = []
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/project_get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/project_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             # filter out DSP base properties
             cardnames = [card for card in cardnames if ":" in card]
             # extend short form
             cardnames = [regex.sub(r"^:", f"{ontoname}:", card) for card in cardnames]
             # filter out other ontos
             cardnames = [card for card in cardnames if regex.search(f"^{ontoname}:", card)]
             # convert to short form
-            cardnames = [regex.sub(ontoname, "", card) for card in cardnames]
+            cardnames = [regex.sub(f"^{ontoname}:", ":", card) for card in cardnames]
 
             invalid_cardnames = [card for card in cardnames if regex.sub(":", "", card) not in propnames]
             if invalid_cardnames:
                 errors[f"Ontology '{ontoname}', resource '{res['name']}'"] = invalid_cardnames
 
     if errors:
         err_msg = "Your data model contains cardinalities with invalid propnames:\n"
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/shared.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,16 +192,16 @@
     for text in doc_without_namespace.findall(path="resource/text-prop/text"):
         if text.attrib["encoding"] == "utf8":
             if (
                 regex.search(r'<([a-zA-Z/"]+|[^\s0-9].*[^\s0-9])>', str(text.text))
                 or len(list(text.iterchildren())) > 0
             ):
                 sourceline = f" line {text.sourceline}: " if text.sourceline else " "
-                propname = text.getparent().attrib["name"]  # type: ignore
-                resname = text.getparent().getparent().attrib["id"]  # type: ignore
+                propname = text.getparent().attrib["name"]  # type: ignore[union-attr]
+                resname = text.getparent().getparent().attrib["id"]  # type: ignore[union-attr]
                 resources_with_illegal_xml_tags.append(f" -{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
         err_msg = (
             "XML-tags are not allowed in text properties with encoding=utf8. "
             "The following resources of your XML file violate this rule:\n"
         )
         err_msg += "\n".join(resources_with_illegal_xml_tags)
```

### Comparing `dsp_tools-2.3.4/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.4.0/src/dsp_tools/utils/xml_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,15 +400,15 @@
     if not any(x.startswith(ontoname) for x in resclass_name_2_type.keys()):
         err_msg = (
             f"The <knora> tag of your XML file references the ontology '{ontoname}', "
             f"but the project {shortcode} on the DSP server doesn't contain an ontology with this name."
         )
         logger.error(err_msg)
         raise UserError(err_msg)
-    knora_properties = resclass_name_2_type[resources[0].restype].knora_properties  # type: ignore
+    knora_properties = resclass_name_2_type[resources[0].restype].knora_properties  # type: ignore[attr-defined]
 
     for resource in resources:
         # check that the resource type is consistent with the ontology
         if resource.restype not in resclass_name_2_type:
             res_syntaxes = [
                 'DSP-API internals: <resource restype="restype">',
                 'current ontology:  <resource restype=":restype">',
@@ -427,15 +427,15 @@
             )
             for res_syntax, res_explanation in zip(res_syntaxes, res_explanations):
                 err_msg += f" - {res_syntax:<55} ({res_explanation})\n"
             logger.error(err_msg)
             raise UserError(err_msg)
 
         # check that the property types are consistent with the ontology
-        resource_properties = resclass_name_2_type[resource.restype].properties.keys()  # type: ignore
+        resource_properties = resclass_name_2_type[resource.restype].properties.keys()  # type: ignore[attr-defined]
         for propname in [prop.name for prop in resource.properties]:
             if propname not in knora_properties and propname not in resource_properties:
                 prop_syntaxes = [
                     'DSP-API internals: <text-prop name="propname">',
                     'current ontology:  <text-prop name=":propname">',
                     'other ontology:    <text-prop name="other:propname">',
                 ]
@@ -710,26 +710,26 @@
                 logger.warning(msg, exc_info=True)
                 failed_uploads.append(resource.id)
                 continue
             bitstream_size_uploaded_mb += bitstream_all_sizes_mb[i]
             msg = f"Uploaded file '{pth}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)"
             print(msg)
             logger.info(msg)
-            internal_file_name_bitstream = img["uploadedFiles"][0]["internalFilename"]  # type: ignore
+            internal_file_name_bitstream = img["uploadedFiles"][0]["internalFilename"]  # type: ignore[index]
             resource_bitstream = resource.get_bitstream(internal_file_name_bitstream, permissions_lookup)
 
         # create the resource in DSP
         resclass_type = resclass_name_2_type[resource.restype]
         properties = resource.get_propvals(id2iri_mapping, permissions_lookup)
         try:
             resource_instance: ResourceInstance = resclass_type(
                 con=con,
                 label=resource.label,
                 iri=resource_iri,
-                permissions=permissions_lookup.get(resource.permissions),  # type: ignore
+                permissions=permissions_lookup.get(str(resource.permissions)),
                 creation_date=resource.creation_date,
                 bitstream=resource_bitstream,
                 values=properties,
             )
             resource_creation_start = datetime.now()
             created_resource: ResourceInstance = try_network_action(resource_instance.create)
             resource_creation_duration = datetime.now() - resource_creation_start
```

### Comparing `dsp_tools-2.3.4/PKG-INFO` & `dsp_tools-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.3.4
+Version: 2.4.0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,21 +17,24 @@
 Requires-Dist: docker (>=6.1.2,<7.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: networkx (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas[excel] (>=2.0.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: regex (>=2023.5.5,<2024.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Documentation, https://docs.dasch.swiss/latest/DSP-TOOLS/
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 
 # DSP-TOOLS documentation
 
 DSP-TOOLS is a Python package with a command line interface 
 that helps you interact with a DSP server. 
 A DSP server is a remote server or a local machine 
 where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on.
```

