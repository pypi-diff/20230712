# Comparing `tmp/hoppr-1.8.8.tar.gz` & `tmp/hoppr-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.8.tar", max compression
+gzip compressed data, was "hoppr-1.9.0.tar", max compression
```

## Comparing `hoppr-1.8.8.tar` & `hoppr-1.9.0.tar`

### file list

```diff
@@ -1,61 +1,70 @@
--rw-r--r--   0        0        0     1084 2023-07-11 18:05:35.000000 hoppr-1.8.8/LICENSE
--rw-r--r--   0        0        0     1214 2023-07-11 18:05:35.000000 hoppr-1.8.8/README.md
--rw-r--r--   0        0        0     1035 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11010 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10697 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10932 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     4305 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4113 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6368 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7961 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4833 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5673 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4606 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/in_toto.py
--rw-r--r--   0        0        0     3357 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17448 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/py.typed
--rw-r--r--   0        0        0     4018 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5023 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    27309 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-07-11 18:05:35.000000 hoppr-1.8.8/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-07-11 18:05:35.000000 hoppr-1.8.8/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-12 18:05:34.000000 hoppr-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1215 2023-07-12 18:05:34.000000 hoppr-1.9.0/README.md
+-rw-r--r--   0        0        0      994 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11546 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10563 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0     2843 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     2875 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/bundle.py
+-rw-r--r--   0        0        0     2252 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/generate.py
+-rw-r--r--   0        0        0     4025 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/layout.py
+-rw-r--r--   0        0        0     7383 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/merge.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/py.typed
+-rw-r--r--   0        0        0      563 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12806 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0     2330 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_cargo_plugin.py
+-rw-r--r--   0        0        0    10738 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4327 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4637 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     2330 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_golang_plugin.py
+-rw-r--r--   0        0        0     4109 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6284 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7946 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     2390 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_npm_plugin.py
+-rw-r--r--   0        0        0     2788 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_nuget_plugin.py
+-rw-r--r--   0        0        0     4819 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3033 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3608 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5511 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5248 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4635 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6782 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3378 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1627 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1546 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    12363 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/py.typed
+-rw-r--r--   0        0        0    20656 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/sbom.py
+-rw-r--r--   0        0        0     4556 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5667 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/net.py
+-rw-r--r--   0        0        0     4251 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    27443 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0    19725 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/resources/hoppr-hippo.ascii
+-rw-r--r--   0        0        0     4036 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/result.py
+-rw-r--r--   0        0        0     7785 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/utils.py
+-rw-r--r--   0        0        0     5100 2023-07-12 18:05:34.000000 hoppr-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 hoppr-1.9.0/PKG-INFO
```

### Comparing `hoppr-1.8.8/LICENSE` & `hoppr-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/README.md` & `hoppr-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 - **Documentation**: <https://hoppr.dev>
 - **Source Code**: <https://gitlab.com/hoppr/hoppr>
 
 # Getting Started
 
 ## Basic Install [from PyPI](https://pypi.org/project/hoppr/)
+
 ```
 pip install hoppr
 ```
 
 ## Quickstart Tutorial
 
 Once you have Hoppr installed, we recommend the ["Your First Bundle" tutorial](https://hoppr.dev/docs/using-hoppr/tutorials/your-first-bundle) to understand the basics.
 
-# Join Us!
+# Join Us
 
-We're completely open source, [MIT licensed](LICENSE), and community friendly. Built with a plugin architecture, Hoppr enables users to extend its SBOM-processing capabilities through their own plugins and algorithms.  
-[Learn more about how to contribute](https://hoppr.dev/docs/category/contribute-to-hoppr), it's easy and we've got
-a welcoming community!
+We're completely open source, [MIT licensed](LICENSE), and community friendly. Built with a plugin architecture, Hoppr enables users to extend its SBOM-processing capabilities through their own plugins and algorithms.
+[Learn more about how to contribute](https://hoppr.dev/docs/development/contributing/guide), it's easy and we've got
+a welcoming community!
```

### Comparing `hoppr-1.8.8/hoppr/__init__.py` & `hoppr-1.9.0/hoppr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """
 Tool for manipulating bundles for airgapped transfers.
 """
 from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprCredentialsError, HopprError, HopprLoadDataError, HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService, Credentials
-from hoppr.models.manifest import Component, ExternalReference, Manifest, Property, Sbom
+from hoppr.models.manifest import Manifest
+from hoppr.models.sbom import Component, Sbom
 from hoppr.models.transfer import ComponentCoverage, Transfer
 from hoppr.models.types import BomAccess, PurlType
 from hoppr.result import Result
 
 __all__ = [
     "BomAccess",
     "Component",
     "ComponentCoverage",
     "CredentialRequiredService",
     "Credentials",
-    "ExternalReference",
     "hoppr_process",
     "hoppr_rerunner",
     "HopprContext",
     "HopprCredentialsError",
     "HopprError",
     "HopprLoadDataError",
     "HopprPlugin",
     "HopprPluginError",
     "Manifest",
-    "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.8"
+__version__ = "1.9.0"
```

### Comparing `hoppr-1.8.8/hoppr/base_plugins/collector.py` & `hoppr-1.9.0/hoppr/base_plugins/collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 """
 Base class for all collector plugins
 """
 from __future__ import annotations
 
 import json
+import os
 import socket
 
 from abc import abstractmethod
 from datetime import datetime, timezone
+from fnmatch import fnmatch
 from pathlib import Path
-from typing import Any, Union, final
+from typing import TYPE_CHECKING, Any, final
 from urllib.parse import urlparse
+from urllib.request import getproxies
 
-from packageurl import PackageURL  # type: ignore[import]
+import hoppr.utils
 
 from hoppr import __version__, constants, plugin_utils
 from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_ignore_excluded, hoppr_process, hoppr_rerunner
 from hoppr.models.credentials import CredentialRequiredService, Credentials
-from hoppr.models.manifest import Component, Property, SearchSequence
+from hoppr.models.manifest import SearchSequence
+from hoppr.models.sbom import Component, Property
 from hoppr.models.transfer import ComponentCoverage
-from hoppr.models.types import BomAccess, PurlType
+from hoppr.models.types import BomAccess, PurlType, RepositoryUrl
 from hoppr.result import Result
-from hoppr.utils import dedup_list, remove_empty
+
+if TYPE_CHECKING:
+    from packageurl import PackageURL
 
 
 class BaseCollectorPlugin(HopprPlugin):
     """
     Base class for collector plugins
     """
 
     default_component_coverage = ComponentCoverage.EXACTLY_ONCE
     bom_access = BomAccess.COMPONENT_ACCESS
     system_repositories: list[str] = []
 
     @staticmethod
+    def _get_proxies_for(url: str) -> dict[str, str] | None:
+        no_proxy_domains = filter(None, set(f"{os.getenv('no_proxy', '')},{os.getenv('NO_PROXY', '')}".split(",")))
+
+        hostname = RepositoryUrl(url=url).hostname or ""
+
+        try:
+            next(pattern for pattern in no_proxy_domains if pattern in hostname or fnmatch(name=hostname, pat=pattern))
+            return None
+        except StopIteration:
+            return getproxies()
+
+    @staticmethod
     def _get_repo_search_list(comp: Component) -> list[str]:
         repo_list: list[str] = []
         for prop in comp.properties or []:
             if prop.name == constants.BomProps.COMPONENT_SEARCH_SEQUENCE:
                 search_sequence_str = json.loads(prop.value or '{"version": "v1", "repositories": []}')
                 search_sequence = SearchSequence.parse_obj(search_sequence_str)
                 repo_list.extend(map(str, search_sequence.repositories))
 
         return repo_list
 
     def _get_repos(self, comp: Component) -> list[str]:
         """
         Returns all repos listed in all BOM_PROPS_COMPONENT_SEARCH_SEQUENCE properties for this component
         """
-
-        purl_url = PackageURL.from_string(comp.purl).qualifiers.get("repository_url")
+        purl = hoppr.utils.get_package_url(comp.purl)
+        purl_url = purl.qualifiers.get("repository_url")
 
         if purl_url is not None and not self.context.strict_repos:
             return [purl_url]
 
         repo_list = self._get_repo_search_list(comp)
 
         if purl_url is not None:
@@ -68,22 +86,22 @@
                     return [purl_url]
 
             return []
 
         if not self.context.strict_repos:
             repo_list.extend(self.system_repositories)
 
-        return dedup_list(repo_list)
+        return hoppr.utils.dedup_list(repo_list)
 
     def empty_repo_list_reason(self, comp: Component) -> str:
         """
         _get_repos may return an empty list, this method returns a string
         giving a reasonable explanation as to why.
         """
-        purl = PackageURL.from_string(comp.purl)
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         if not self.context.strict_repos:
             return f"No repositories specified for purl type {purl.type}, and no repository_url specified in purl"
 
         if len(self._get_repo_search_list(comp)) == 0:
             return (
                 f"No repositories specified in manifest for purl type {purl.type}. "
@@ -97,17 +115,17 @@
                 "line option"
             )
 
         return "Reason for empty repo list undetermined"
 
     def directory_for(
         self,
-        purl_type: Union[str, PurlType],
+        purl_type: str | PurlType,
         repo_url: str,
-        subdir: Union[str, None] = None,
+        subdir: str | None = None,
     ) -> Path:
         """
         Identify the directory into which the artifact should be copied
         """
 
         repo_dir = plugin_utils.dir_name_from_repo_url(repo_url)
         directory = Path(self.context.collect_root_dir, str(purl_type), repo_dir)
@@ -123,15 +141,15 @@
     def _parse_url_for_comparison(url: str) -> tuple[str, str, str]:
         """
         Resulting tuple is (host, port, path)
         """
         if url.startswith("file:") or "//" in url:
             initial_parse = urlparse(url)
         else:
-            initial_parse = urlparse("//" + url)
+            initial_parse = urlparse(f"//{url}")
 
         host_data = initial_parse.netloc.split(":")
 
         host = host_data[0]
 
         if len(host_data) > 1:
             port = host_data[1]
@@ -166,31 +184,28 @@
             and (not parsed_purl_url[1] or parsed_repo_url[1] == parsed_purl_url[1])  # Compare port if present
             and parsed_repo_url[2].startswith(parsed_purl_url[2])  # Compare initial path
         ):
             return Result.success()
 
         return Result.fail(f"Purl-specified repository url ({purl_url}) does not match current repo ({repo_url}).")
 
-    def set_collection_params(self, comp: Component, repository: str, directory: Union[Path, str]) -> None:
+    def set_collection_params(self, comp: Component, repository: str, directory: Path | str) -> None:
         """
         Set collection parameters on sbom component
         """
 
         rel_dir = str(Path(directory).relative_to(self.context.collect_root_dir))
 
         collect_props: dict[str, str] = {
             constants.BomProps.COLLECTION_REPOSITORY: repository,
             constants.BomProps.COLLECTION_DIRECTORY: rel_dir,
             constants.BomProps.COLLECTION_PLUGIN: f"{type(self).__name__}:{self.get_version()}",
             constants.BomProps.COLLECTION_TIMETAG: str(datetime.now(timezone.utc)),
         }
 
-        if comp.properties is None:
-            comp.properties = []
-
         for prop in comp.properties:
             if prop.name in collect_props:
                 prop.value = collect_props.pop(prop.name)
 
         for key, value in collect_props.items():
             if value is not None:
                 comp.properties.append(Property(name=key, value=value))
@@ -269,15 +284,15 @@
 
     @hoppr_process
     def post_stage_process(self):
         for purl_type in self.supported_purl_types:
             directory = Path(self.context.collect_root_dir, purl_type)
 
             if directory.is_dir():
-                remove_empty(directory)
+                hoppr.utils.remove_empty(directory)
 
         return Result.success()
 
 
 class BatchCollectorPlugin(BaseCollectorPlugin):
     """
     Base class for single-process collector plugins
```

### Comparing `hoppr-1.8.8/hoppr/base_plugins/hoppr.py` & `hoppr-1.9.0/hoppr/base_plugins/hoppr.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 import time
 import traceback
 
 from abc import ABC, abstractmethod
 from os import PathLike
 from typing import Any, Callable, Dict, List, Optional
 
-from hoppr import plugin_utils
+import hoppr.plugin_utils
+import hoppr.utils
+
 from hoppr.mem_logger import MemoryLogger
 from hoppr.models import HopprContext
 from hoppr.models.transfer import ComponentCoverage
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import get_package_url, obscure_passwords
 
 
 def _get_component(*args, **kwargs) -> Optional[Any]:
     # TODO: This will only utilize the first Component found in 1) args, 2) kwargs  # pylint: disable=fixme
     # and assumes all plugins operate this way
     comp = next((arg for arg in args if type(arg).__name__ == "Component"), None)
 
@@ -55,29 +56,29 @@
 
         result = None
         if comp is not None:
             if comp.purl is None:
                 result = Result.fail("No purl supplied for component")
 
             else:
-                purl_type = get_package_url(comp.purl).type
+                purl_type = hoppr.utils.get_package_url(comp.purl).type
 
                 if not self.supports_purl_type(purl_type):
                     return Result.skip(f"Class {self.__class__.__name__} does not support purl type {purl_type}")
 
                 component_header = f"{comp.name}" + (f"@{comp.version}" if comp.version is not None else "")
 
                 self.get_logger().info(
                     msg=f"{'-' * 4} Component: {component_header} {'-' * 50}",
                 )
 
         if result is None:
             # Only check for missing commands if func has been overridden
             if func.__module__ != HopprPlugin.__module__:
-                command_result = plugin_utils.check_for_missing_commands(self.required_commands)
+                command_result = hoppr.plugin_utils.check_for_missing_commands(self.required_commands)
                 if command_result.is_fail():
                     self.get_logger().error(command_result.message)
                     return command_result
 
             try:
                 result = func(self, *args, **kwargs)
             except Exception as error:  # pylint: disable=broad-except
@@ -178,15 +179,15 @@
     """
     Product: the result of carrying out a step. Products are usually persistent (e.g,.
     files), and are often meant to be used as materials on subsequent steps. Products are
     recorded as part of link metadata.
 
     This is a list of strings where each element is a relative path file or wildcard.
 
-    See in-toto specificaion:
+    See in-toto specification:
     - https://github.com/in-toto/docs/blob/master/in-toto-spec.md
     """
     products: List[str] = []
 
     default_component_coverage = ComponentCoverage.OPTIONAL
     bom_access = BomAccess.NO_ACCESS
     process_timeout = 60
@@ -197,17 +198,15 @@
         config: Optional[Dict] = None,
     ) -> None:
         self._logger: MemoryLogger
         self._start_time: float = 0.0
         self.context = context
         self.config = config
 
-        if self.config is not None:
-            if "process_timeout" in self.config:
-                self.process_timeout = self.config["process_timeout"]
+        self.process_timeout = (self.config or {}).get("process_timeout", self.process_timeout)
 
     @abstractmethod
     def get_version(self) -> str:
         """
         Returns the version of this plug-in
         """
 
@@ -278,15 +277,15 @@
 
     def run_command(
         self, command: list[str], password_list: list[str] | None = None, cwd: str | PathLike[str] | None = None
     ) -> subprocess.CompletedProcess[bytes]:
         """
         Run a command and log any errors
         """
-        obscured_command = obscure_passwords(command, password_list)
+        obscured_command = hoppr.utils.obscure_passwords(command, password_list)
         self.get_logger().debug(msg=f"Running command: '{obscured_command}'", indent_level=2)
 
         try:
             result = subprocess.run(
                 command, check=False, shell=False, capture_output=True, cwd=cwd, timeout=self.process_timeout
             )
         except subprocess.TimeoutExpired as timeout_expired:
@@ -294,18 +293,17 @@
                 f"Command \"{command[0]}\" timed out after {timeout_expired.timeout} seconds", indent_level=2
             )
             result = subprocess.CompletedProcess(
                 command, returncode=124, stdout=timeout_expired.stdout or b'', stderr=timeout_expired.stderr or b''
             )
 
         if result.returncode != 0:
-            # Prefix each line of the command's stdout with 4 spaces
-            stdout_indented = "\n".join(["    " + line for line in result.stdout.decode("utf-8").split("\n")])
+            # Prefix each line of the command's stdout and stderr with 4 spaces
+            stdout_indented, stderr_indented = map(
+                lambda output: "\n".join([f"    {line}" for line in output.decode("utf-8").split("\n")]),
+                [result.stdout, result.stderr],
+            )
 
             self.get_logger().debug(msg=f"{command[0]} command stdout content:\n{stdout_indented}", indent_level=2)
-
-            # Prefix each line of the command's stderr with 4 spaces
-            stderr_indented = "\n".join(["    " + line for line in result.stderr.decode("utf-8").split("\n")])
-
             self.get_logger().error(msg=f"{command[0]} command failed with error:\n{stderr_indented}", indent_level=2)
 
         return result
```

### Comparing `hoppr-1.8.8/hoppr/constants.py` & `hoppr-1.9.0/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.9.0/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,35 @@
 import os
 import shutil
 
 from configparser import ConfigParser
 from os import PathLike
 from pathlib import Path
 from subprocess import CalledProcessError
-from typing import Mapping
+from typing import TYPE_CHECKING, Mapping
 from urllib.parse import urlparse
 
 import jc
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import BatchCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
-from hoppr.models.manifest import Component, Repository
+from hoppr.models.manifest import Repository
+from hoppr.models.sbom import Component
 from hoppr.models.types import PurlType
 from hoppr.result import Result
 
+if TYPE_CHECKING:
+    from packageurl import PackageURL
+
 
 class CollectAptPlugin(BatchCollectorPlugin):
     """
     Collector plugin for apt packages
     """
 
     required_commands: list[str] = ["apt", "apt-cache"]
@@ -73,22 +77,16 @@
             self.required_commands[0],
             f"--option=Dir={self.config_dir}",
             f"--option=Dir::State::status={self.config_dir / 'var' / 'lib' / 'dpkg' / 'status'}",
             *proxy_args,
         ]
 
     def _artifact_string(self, purl: PackageURL) -> str:
-        artifact_string = purl.name
-
-        if purl.qualifiers.get("arch") is not None:
-            artifact_string = ":".join([artifact_string, purl.qualifiers.get("arch")])
-        if purl.version is not None:
-            artifact_string = "=".join([artifact_string, purl.version])
-
-        return artifact_string
+        arch = purl.qualifiers.get("arch")
+        return f"{purl.name}{f':{arch}' if arch else ''}{f'={purl.version}' if purl.version else ''}"
 
     def _download_component(self, purl: PackageURL) -> None:
         artifact = self._artifact_string(purl)
 
         try:
             # Download the component
             download_result = self.run_command(
@@ -304,15 +302,15 @@
 
     @hoppr_rerunner
     def collect(self, comp: Component) -> Result:
         """
         Copy a component to the local collection directory structure
         """
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         try:
             found_url, download_filename = self._get_component_download_info(purl=purl)
         except (CalledProcessError, HopprPluginError) as ex:
             return Result.retry(message=str(ex))
 
         download_url_path = Path(self._get_download_url_path(purl=purl))
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,60 +2,57 @@
 Collector plugin for DNF packages
 """
 from __future__ import annotations
 
 import fnmatch
 import os
 import shutil
+import time
 
 from configparser import ConfigParser
 from os import PathLike
 from pathlib import Path
-from time import sleep
+from typing import TYPE_CHECKING
 from urllib.parse import quote_plus, urlparse
 
 import requests
 
-from packageurl import PackageURL
 from requests.auth import HTTPBasicAuth
 
 import hoppr.net
 import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import BatchCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
-from hoppr.models.manifest import Component
+from hoppr.models.sbom import Component
 from hoppr.models.types import PurlType, RepositoryUrl
 from hoppr.result import Result
 
+if TYPE_CHECKING:
+    from packageurl import PackageURL
 
-def _artifact_string(purl: PackageURL) -> str:
-    artifact_string = purl.name
-
-    if purl.version is not None:
-        artifact_string = "-".join([artifact_string, purl.version])
-    if purl.qualifiers.get("arch") is not None:
-        artifact_string = ".".join([artifact_string, purl.qualifiers.get("arch")])
 
-    return artifact_string
+def _artifact_string(purl: PackageURL) -> str:
+    arch = purl.qualifiers.get("arch")
+    return f"{purl.name}{f'-{purl.version}' if purl.version else ''}{f'.{arch}' if arch else ''}"
 
 
 def _is_rpm_repo(repo_url: str) -> bool:
     url = RepositoryUrl(url=repo_url) / "repodata/repomd.xml"
     basic_auth = None
     creds = Credentials.find(repo_url)
     if creds is not None:
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
     for attempt in range(3):
         if attempt > 0:
-            sleep(5)
+            time.sleep(5)
 
         resp = requests.get(f"{url}", auth=basic_auth, allow_redirects=False, stream=True, verify=True, timeout=60)
         if resp.status_code < 300:
             return True
         if resp.status_code < 500:
             return False
 
@@ -143,15 +140,15 @@
 
     def get_version(self) -> str:
         return __version__
 
     @hoppr_process
     def pre_stage_process(self) -> Result:
         repo_config = ConfigParser()
-        repo_config["main"] = dict(cachedir=f"{self.config_file.parent / 'cache'}")
+        repo_config["main"] = {"cachedir": f"{self.config_file.parent / 'cache'}"}
 
         # Clear out cache before starting the pre_stage_process
         search_root = self.config_file.parent / "cache"
         _clear_cache(search_root)
 
         for idx, repo in enumerate(self.context.repositories[PurlType.RPM]):
             temp_repo = f"hoppr-tmp-{idx}"
@@ -216,33 +213,33 @@
 
     @hoppr_rerunner
     def collect(self, comp: Component) -> Result:
         """
         Copy a component to the local collection directory structure
         """
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         self.get_logger().info(msg=f"Copying DNF package from {purl}", indent_level=2)
 
         # Try getting RPM URL
         try:
-            found_url = self._get_component_download_url(purl)  # type: ignore
+            found_url = self._get_component_download_url(purl)
         except HopprPluginError as ex:
             return Result.retry(message=str(ex))
 
         repo = self._get_found_repo(found_url)
         # Return failure if found RPM URL is not from a repo defined in the manifest
         if repo is None:
             return Result.fail(
                 "Successfully found RPM file but URL does not match any repository in manifest."
                 f" (Found URL: '{found_url}')"
             )
 
-        result = self.check_purl_specified_url(purl, repo)  # type: ignore
+        result = self.check_purl_specified_url(purl, repo)
         if not result.is_success():
             return result
 
         found_url_path = Path(found_url)
         subdir = found_url_path.relative_to(repo).parent
         target_dir = self.directory_for(purl.type, repo, subdir=str(subdir))
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 
 # pylint: disable=too-many-locals
 
 from __future__ import annotations
 
 import re
 import urllib.parse
-
-from typing import Any
 from packageurl import PackageURL
 
 import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
+from hoppr.models.sbom import Component
 from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectDockerPlugin(SerialCollectorPlugin):
     """
     Collector plugin for docker images
@@ -55,15 +54,15 @@
         """
         source_image = RepositoryUrl(url=url) / (purl.namespace or "") / urllib.parse.quote_plus(image_name)
         if source_image.scheme != "docker":
             source_image = RepositoryUrl(url="docker://" + re.sub(r"^(.*://)", "", str(source_image)))
         return source_image
 
     @hoppr_rerunner
-    def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
+    def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Copy a component to the local collection directory structure
         """
         purl = hoppr.utils.get_package_url(comp.purl)
         version_path = purl.version
 
         # Determine if purl version contains SHA string, determine proper formatting for skopeo command
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_git_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Collector plugin for git repositories
 """
 from __future__ import annotations
 
-import os
 import re
 
 from pathlib import Path
 
-from packageurl import PackageURL  # type: ignore[import]
+import hoppr
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
-from hoppr.models.manifest import Component
+from hoppr.models.sbom import Component
+from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectGitPlugin(SerialCollectorPlugin):
     """
     Class to copy git repositories
 
@@ -42,24 +43,23 @@
             self.required_commands = [self.config["git_command"]]
 
     @hoppr_rerunner
     def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None) -> Result:
         """
         Collect git repository
         """
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
-
-        source_url = os.path.join(repo_url, purl.namespace, purl.name)
+        purl = hoppr.utils.get_package_url(comp.purl)
+        source_url = RepositoryUrl(url=repo_url) / (purl.namespace or "") / purl.name
 
         self.get_logger().info(msg=f"Cloning {source_url}", indent_level=2)
 
         # Only reference the namespace.  The actual clone creates the named directory
         target_dir = self.directory_for(purl.type, repo_url, subdir=purl.namespace)
 
-        git_result = self.git_clone(tmp_dir=target_dir, source_url=source_url, source_creds=creds, comp=comp)
+        git_result = self.git_clone(tmp_dir=target_dir, source_url=f"{source_url}", source_creds=creds, comp=comp)
         if not git_result.is_success():
             return git_result
 
         git_result = self.git_update(target_dir, purl.name)
         if not git_result.is_success():
             return git_result
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
-from hoppr.models.manifest import Component
+from hoppr.models.sbom import Component
 from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectHelmPlugin(SerialCollectorPlugin):
     """
     Class to copy helm charts
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from subprocess import CalledProcessError
 from tempfile import NamedTemporaryFile
 from typing import Any, OrderedDict
 
 import jmespath
 import xmltodict
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
-from hoppr.models.manifest import Component
+from hoppr.models.sbom import Component
 from hoppr.result import Result
 
 _MAVEN_DEP_PLUGIN = "org.apache.maven.plugins:maven-dependency-plugin:3.5.0"
 
 
 class CollectMavenPlugin(SerialCollectorPlugin):
     """
@@ -67,17 +67,15 @@
 
                     for repo in repo_urls:
                         if repo not in self.system_repositories:
                             self.system_repositories.append(repo)
 
     def _get_maven_component(self, command: list[str], password_list: list[str], **kwargs):
         full_command = command.copy()
-        for key, value in kwargs.items():
-            full_command.append(f"-D{key}={value}")
-
+        full_command.extend(f"-D{key}={value}" for key, value in kwargs.items())
         result = self.run_command(full_command, password_list)
 
         # The maven plugin does not recognize the 'destFileName' argument, so rename the file
         if result.returncode == 0:
             _, name, version, extension = kwargs.get("artifact", "::::").split(":")
             directory = kwargs.get("outputDirectory", ".")
             old_name = f"{name}-{version}.{extension}"
@@ -90,15 +88,15 @@
     @hoppr_rerunner
     def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None) -> Result:
         """
         Copy a component to the local collection directory structure
         """
         # pylint: disable=too-many-locals
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
         artifact = f"{purl.namespace}:{purl.name}:{purl.version}"
 
         extension = purl.qualifiers.get("type", "tar.gz")
         target_dir = self.directory_for(purl.type, repo_url, subdir=f"{purl.namespace}")
 
         self.get_logger().info(msg="Copying maven artifact:", indent_level=2)
         self.get_logger().info(msg=f"source: {repo_url}", indent_level=3)
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_nexus_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """
 Collector plugin to copy artifacts using the Nexus API
 """
 from __future__ import annotations
 
 import json
 import re
+import time
 
 from pathlib import Path
-from time import sleep
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 import requests
 
-from packageurl import PackageURL  # type: ignore
 from requests.auth import HTTPBasicAuth
 
+import hoppr.utils
+
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
 from hoppr.models.types import PurlType, RepositoryUrl
 from hoppr.net import download_file
 from hoppr.result import Result
 
+if TYPE_CHECKING:
+    from packageurl import PackageURL
+
 
 class CollectNexusSearch(SerialCollectorPlugin):
     """
     Class to copy artifacts using the Nexus API
     """
 
     def get_version(self) -> str:  # pylint: disable=duplicate-code
@@ -65,15 +69,15 @@
             auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
 
         nexus_url = self._parse_nexus_url(repo_url)[0]
 
         if not CollectNexusSearch.is_nexus_instance(nexus_url, auth):
             return Result.fail(f"{nexus_url} is not a Nexus instance")
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         source_urls = CollectNexusSearch.get_download_urls(purl, repo_url, auth)
         if len(source_urls) == 0:
             msg = f"No artifacts found in Nexus instance {repo_url} for purl {comp.purl}"
             self.get_logger().error(msg, indent_level=2)
             return Result.fail(msg)
 
@@ -131,15 +135,15 @@
         """
         Checks whether or not the repo_url refers to a Nexus instance
         """
         test_url = RepositoryUrl(url=repo_url) / "service" / "rest" / "v1" / "status"
 
         for attempt in range(3):
             if attempt > 0:
-                sleep(5)
+                time.sleep(5)
 
             response = requests.get(
                 f"{test_url}",
                 auth=auth,
                 allow_redirects=True,
                 stream=True,
                 verify=True,
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 import importlib.util
 import re
 import sys
 
 from subprocess import CalledProcessError
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
-from hoppr.models.manifest import Component
+from hoppr.models.sbom import Component
 from hoppr.models.types import RepositoryUrl
 from hoppr.result import Result
 
 
 class CollectPypiPlugin(SerialCollectorPlugin):
     """
     Collector plugin for pypi images
@@ -76,15 +76,15 @@
     def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None) -> Result:
         """
         Copy a component to the local collection directory structure
         """
         if importlib.util.find_spec(name="pip") is None:
             return Result.fail(message="The pip package was not found. Please install and try again.")
 
-        purl = PackageURL.from_string(comp.purl)
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         source_url = RepositoryUrl(url=repo_url)
         if not re.match(pattern="^.*simple/?$", string=f"{source_url}"):
             source_url /= "simple"
 
         password_list = []
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import shutil
 
 from pathlib import Path
 from typing import Any, List
 from urllib.parse import unquote
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models.credentials import CredentialRequiredService
 from hoppr.models.types import RepositoryUrl
 from hoppr.net import download_file
@@ -33,15 +33,15 @@
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Copy a component to the local collection directory structure
         """
         source_url = RepositoryUrl(url=repo_url)
 
-        purl = PackageURL.from_string(comp.purl)
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         subdir = None
         if purl.namespace is not None:
             source_url /= f"{purl.namespace}"
             subdir = unquote(purl.namespace)
 
         target_dir = self.directory_for(purl.type, repo_url, subdir=subdir)
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.9.0/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Collector plugin for Yum packages
 """
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
 from hoppr.result import Result
 
@@ -38,25 +38,23 @@
     products: list[str] = ["rpm/*"]
 
     def get_version(self) -> str:
         return __version__
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
-        if self.config is not None:
-            if "yumdownloader_command" in self.config:
-                self.required_commands = [self.config["yumdownloader_command"]]
+        self.required_commands = (self.config or {}).get("yumdownloader_command", self.required_commands)
 
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds=None):
         """
         Copy a component to the local collection directory structure
         """
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
         artifact = _artifact_string(purl)
 
         self.get_logger().info(msg=f"Copying yum package from {comp.purl}", indent_level=2)
 
         command = [
             self.required_commands[0],
             "-q",
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/composite_collector.py` & `hoppr-1.9.0/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.9.0/hoppr/core_plugins/delta_sbom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """
 Plugin to remove SBOM components that are specified by a "previous" SBOM
 """
+from __future__ import annotations
+
+import contextlib
 import io
 import tarfile
 
-from copy import deepcopy
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-from packageurl import PackageURL
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process
 from hoppr.exceptions import HopprError
-from hoppr.models.manifest import Component, Manifest, Sbom
+from hoppr.models.manifest import Manifest
+from hoppr.models.sbom import Component, Sbom
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import dedup_list, get_package_url, load_string
+
+if TYPE_CHECKING:
+    from packageurl import PackageURL
 
 
 class DeltaSbom(HopprPlugin):
     """
     Plugin to remove SBOM components that are specified by a "previous" SBOM
     """
 
@@ -41,28 +47,28 @@
             return Result.success(
                 "No previously delivered bundle specified for delta bundle. All components will be delivered"
             )
         else:
             previous_source = self.config.get("previous")
 
         if not Path(previous_source).exists():  # pyright: ignore[reportGeneralTypeIssues]
-            return Result.fail(f"Previous source file \"{previous_source}\" not found.")
+            return Result.fail(f'Previous source file "{previous_source}" not found.')
 
         self.get_logger().info(f"Creating delta/update SBOM, previous SBOM being retrieved from {previous_source}")
 
         previous_sbom = self._get_previous_bom(previous_source)  # pyright: ignore[reportGeneralTypeIssues]
 
         target_dir = self.context.collect_root_dir / "generic" / "_metadata_"
         target_dir.mkdir(parents=True, exist_ok=True)
 
         with (target_dir / "_previous_bom.json").open(mode="w", encoding="utf-8") as bom_data:
             bom_data.write(previous_sbom.json(exclude_none=True, by_alias=True, indent=2))
 
-        delta_sbom = deepcopy(self.context.delivered_sbom)
-        delta_sbom.components = []
+        delta_sbom = self.context.delivered_sbom.copy(deep=True)
+        delta_sbom.components.clear()
 
         for new_comp in self.context.delivered_sbom.components or []:
             include_component = True
             for prev_comp in previous_sbom.components or []:
                 if DeltaSbom._component_match(new_comp, prev_comp):
                     include_component = False
                     break
@@ -82,73 +88,61 @@
             f"Delivering updates for {len(delta_sbom.components)} of "
             f"{len(self.context.delivered_sbom.components)} components.",
             return_obj=delta_sbom,
         )
 
     @staticmethod
     def _get_previous_bom(source: str) -> Sbom:
-        try:
-            Manifest.load(Path(source))
-            return Sbom.consolidated_sbom
-        except (TypeError, UnicodeDecodeError):
-            pass
+        with contextlib.suppress(TypeError, UnicodeDecodeError):
+            Sbom.loaded_sboms.clear()
+            return Manifest.load(Path(source)).consolidated_sbom
 
         with tarfile.open(source) as tar:
             buffer = tar.extractfile("./generic/_metadata_/_consolidated_bom.json")
 
             if buffer is None:
                 raise HopprError("Unable to extract BOM file from tar")
 
             with io.TextIOWrapper(buffer) as bom_file:
                 content: str = bom_file.read()
-                bom_dict = load_string(content)
+                bom_dict = hoppr.utils.load_string(content)
                 if not isinstance(bom_dict, dict):
                     raise HopprError("Invalid BOM file retrieved from tar")
                 return Sbom(**bom_dict)
 
     @staticmethod
     def _purl_match(new_purl: PackageURL, prev_purl: PackageURL) -> bool:
-
-        if (
-            new_purl.name != prev_purl.name
-            or new_purl.type != prev_purl.type
-            or (new_purl.namespace or "") != (prev_purl.namespace or "")
-            or (new_purl.version or "") != (prev_purl.version or "")
-            or (new_purl.subpath or "") != (prev_purl.subpath or "")
+        if any(
+            getattr(new_purl, attr) != getattr(prev_purl, attr)
+            for attr in ["name", "type", "namespace", "version", "subpath"]
         ):
             return False
 
-        qual_keys = list(new_purl.qualifiers.keys()) or []
-        qual_keys.extend(list(prev_purl.qualifiers.keys()) or [])
-
-        for key in dedup_list(qual_keys):
-            if new_purl.qualifiers.get(key) != prev_purl.qualifiers.get(key):
-                return False
+        qual_keys = list(new_purl.qualifiers.keys())
+        qual_keys.extend(list(prev_purl.qualifiers.keys()))
 
-        return True
+        return all(
+            new_purl.qualifiers.get(key) == prev_purl.qualifiers.get(key) for key in hoppr.utils.dedup_list(qual_keys)
+        )
 
     @staticmethod
     def _component_match(new_comp: Component, prev_comp: Component) -> bool:
-
-        new_purl: PackageURL = get_package_url(new_comp.purl)
-        prev_purl: PackageURL = get_package_url(prev_comp.purl)
+        new_purl = hoppr.utils.get_package_url(new_comp.purl)
+        prev_purl = hoppr.utils.get_package_url(prev_comp.purl)
 
         if not DeltaSbom._purl_match(new_purl, prev_purl):
             return False
 
         hash_matches = 0
 
-        for new_hash in new_comp.hashes or []:
-            for prev_hash in prev_comp.hashes or []:
-                if new_hash.alg.value != prev_hash.alg.value:
+        for new_hash in new_comp.hashes:
+            for prev_hash in prev_comp.hashes:
+                if new_hash.alg != prev_hash.alg:
                     continue
                 if new_hash.content != prev_hash.content:
                     return False
                 hash_matches += 1
 
         if hash_matches > 0:
             return True
 
-        if new_purl.version is None or new_purl.version == "latest":
-            return False
-
-        return True
+        return new_purl.version is not None and new_purl.version != "latest"
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.9.0/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/oras_registry.py` & `hoppr-1.9.0/hoppr/core_plugins/oras_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import json
 import os
 import platform
 
 from datetime import datetime
 from http import cookiejar
 
-import jsonschema  # type: ignore
-import oras.defaults  # type: ignore
-import oras.oci  # type: ignore
-import oras.provider  # type: ignore
+import jsonschema  # type: ignore[import]
+import oras.defaults
+import oras.oci
+import oras.provider
+import oras.schemas
 import requests
 
-from oras.container import Container  # type: ignore
-from oras.decorator import ensure_container  # type: ignore
+from oras.container import Container
+from oras.decorator import ensure_container
 
 import hoppr
 
 
 class Registry(oras.provider.Registry):
     """Override the default Oras Registry Class"""
 
@@ -70,15 +71,14 @@
         Args:
             container (Container): oras container
             archives (list): list of layers to upload
             logger (_type_): hoppr logger
         """
         # Upload files as blobs
         for item in archives:
-
             blob = item.get("path")
             media_type = item.get("media_type")
             annots = item.get("annotations") or {}
 
             if not blob or not os.path.exists(blob):
                 logger.info(f"Path {blob} does not exist or is not defined.")
                 continue
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 import typer
 
 from jinja2 import Environment, FileSystemLoader
 
 from hoppr import __version__
 from hoppr.base_plugins.hoppr import HopprPlugin
-from hoppr.models.manifest import Component, SearchSequence
+from hoppr.models.sbom import Component
+from hoppr.models.manifest import SearchSequence
 from hoppr.result import ResultStatus
 
 
 class Report:  # pylint: disable=too-few-public-methods
     """
     A report of a plugin's execution stage result.
     """
```

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/in_toto.py` & `hoppr-1.9.0/hoppr/in_toto.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 This module includes a function for creating in-toto layout files, and
 wrapping other processing with "start" and "stop" functions.
 """
 from __future__ import annotations
 
 from pathlib import Path
 
-from in_toto.models.layout import Layout, Step  # type: ignore
-from in_toto.models.metadata import Metablock  # type: ignore
-from in_toto.runlib import in_toto_record_start, in_toto_record_stop  # type: ignore
-from securesystemslib import interface  # type: ignore
+from in_toto.models.layout import Layout, Step
+from in_toto.models.metadata import Metablock
+from in_toto.runlib import in_toto_record_start, in_toto_record_stop
+from securesystemslib import interface
 
 from hoppr.models.transfer import Transfer
 from hoppr.utils import plugin_class
 
 
 def _get_products(transfer: Transfer) -> tuple[dict[str, list[str]], list[str]]:
     """
@@ -28,15 +28,14 @@
     products = {}
     stages = []
 
     stages.append("_collect_metadata")
     products["_collect_metadata"] = ["generic/_metadata_/*"]
 
     for stage_ref in transfer.stages:
-
         stages.append(stage_ref.name)
 
         products[stage_ref.name] = []
         for plugin_ref in stage_ref.plugins:
             plugin_cls = plugin_class(plugin_ref.name)
             products[stage_ref.name] += plugin_cls.get_attestation_products(plugin_ref.config)
```

### Comparing `hoppr-1.8.8/hoppr/main.py` & `hoppr-1.9.0/hoppr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 from hoppr.models.manifest import Manifest
 from hoppr.models.transfer import Transfer
 from hoppr.processor import HopprProcessor
 
 
 def bundle(  # pylint: disable=too-many-arguments,too-many-locals
     manifest_file: Path,
-    credentials_file: Path,
+    credentials_file: Optional[Path],
     transfer_file: Path,
-    log_file: Path,
+    log_file: Optional[Path],
     verbose: bool = False,
     strict_repos: bool = True,
     create_attestations: bool = False,
     functionary_key_path: Optional[Path] = None,
     functionary_key_prompt: bool = False,
     functionary_key_password: Optional[str] = None,
     previous_delivery: Optional[Path] = None,
 ):
     """
     Run the stages specified in the transfer config
     file on the content specified in the manifest
     """
     echo(
-        f"Loading {str(manifest_file).rsplit(str(sep), maxsplit=1)[-1]} and"
+        f"Loading {str(manifest_file).rsplit(str(sep), maxsplit=1)[-1]} and "
         f"{str(transfer_file).rsplit(str(sep), maxsplit=1)[-1]} files..."
     )
     metadata_files = [manifest_file, transfer_file]
 
     if credentials_file is not None:
         echo(f"Loading {str(credentials_file).rsplit(str(sep), maxsplit=1)[-1]} file...")
         metadata_files.append(credentials_file)
```

### Comparing `hoppr-1.8.8/hoppr/mem_logger.py` & `hoppr-1.9.0/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/models/__init__.py` & `hoppr-1.9.0/hoppr/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """
 Base model for Hoppr config files
 """
 from __future__ import annotations
 
 import logging
 
-from copy import deepcopy
 from multiprocessing.managers import BaseProxy
 from pathlib import Path
 from threading import _RLock as RLock
-from typing import TYPE_CHECKING, ClassVar
 
-from pydantic import Field, root_validator
+from pydantic import Field
 
 from hoppr.models.base import HopprBaseModel
 from hoppr.models.credentials import CredentialRequiredService, Credentials, CredentialsFile
-from hoppr.models.manifest import Manifest, ManifestFile, Repositories, Sbom
+from hoppr.models.manifest import Manifest, ManifestFile, Repositories
+from hoppr.models.sbom import Sbom
 from hoppr.models.transfer import StageRef, Transfer, TransferFile
 
 __all__ = [
     "Credentials",
     "CredentialsFile",
     "HopprBaseModel",
     "Manifest",
     "ManifestFile",
     "Transfer",
     "TransferFile",
 ]
 
-if TYPE_CHECKING:
-    from pydantic.typing import DictStrAny
-
 
 class HopprSchemaModel(HopprBaseModel):
     """
     Consolidated Hoppr config file schema definition
     """
 
     __root__: CredentialsFile | ManifestFile | TransferFile = Field(..., discriminator="kind")
@@ -56,7 +52,10 @@
     max_processes: int
     previous_delivery: Path | str | None = None
     repositories: Repositories
     retry_wait_seconds: float = 5
     sboms: list[Sbom]
     stages: list[StageRef]
     strict_repos: bool = True
+
+
+HopprContext.update_forward_refs()
```

### Comparing `hoppr-1.8.8/hoppr/models/__main__.py` & `hoppr-1.9.0/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/models/base.py` & `hoppr-1.9.0/hoppr/models/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Base model for Hoppr config files
 """
 from __future__ import annotations
 
 from typing import Literal
 
-from pydantic import Extra, Field, validator
+from pydantic import BaseConfig, Extra, Field, validator
 from pydantic_yaml import YamlModel
 
 
 class Metadata(YamlModel):
     """
     Metadata data model
     """
@@ -20,22 +20,27 @@
 
 
 class HopprBaseModel(YamlModel):
     """
     Base Hoppr data model
     """
 
-    class Config:  # pylint: disable=too-few-public-methods
-        """Config for HopprBaseModel"""
+    class Config(BaseConfig):  # pylint: disable=too-few-public-methods
+        """
+        Config options for HopprBaseModel
+        """
 
         allow_population_by_field_name = True
         arbitrary_types_allowed = True
         extra = Extra.forbid
         use_enum_values = True
 
+    def __eq__(self, other: object) -> bool:
+        return hash(self) == hash(other)
+
     def __hash__(self) -> int:
         """
         Define to test equality or uniqueness between objects
         """
         return hash(repr(self))
```

### Comparing `hoppr-1.8.8/hoppr/models/credentials.py` & `hoppr-1.9.0/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/models/manifest.py` & `hoppr-1.9.0/hoppr/models/manifest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 """
 Manifest file data model
 """
 from __future__ import annotations
 
-import uuid
-
 from copy import deepcopy
 from pathlib import Path
 from typing import TYPE_CHECKING, Annotated, ClassVar, Literal, MutableMapping
 
-from hoppr_cyclonedx_models.cyclonedx_1_4 import Component as ComponentSpecVersion14
-from hoppr_cyclonedx_models.cyclonedx_1_4 import CyclonedxSoftwareBillOfMaterialsStandard as SbomSpecVersion14
-from hoppr_cyclonedx_models.cyclonedx_1_4 import ExternalReference as ExternalReferenceSpecVersion14
-from hoppr_cyclonedx_models.cyclonedx_1_4 import Property as PropertySpecVersion14
-from packageurl import PackageURL
-from pydantic import AnyUrl, Extra, Field, FileUrl, HttpUrl, NoneStr, create_model, validator
+from pydantic import Field, NoneStr, create_model, validator
 from pydantic.main import ModelMetaclass
 from requests import HTTPError
 from typer import secho
 
 import hoppr.net
 import hoppr.oci_artifacts
 import hoppr.utils
 
 from hoppr.constants import BomProps
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models.base import HopprBaseModel, HopprBaseSchemaModel
-from hoppr.models.types import PurlType, RepositoryUrl
+from hoppr.models.sbom import Component, ExternalReference, Property, Sbom, SbomRef
+from hoppr.models.types import LocalFile, OciFile, PurlType, RepositoryUrl, UrlFile
 
 if TYPE_CHECKING:
     from pydantic.typing import DictStrAny
 
 
 class Repository(HopprBaseModel):
     """
@@ -73,150 +67,37 @@
         setattr(self, str(item), value)
 
     def __iter__(self):
         for purl_type in PurlType:
             yield (purl_type, self[purl_type])
 
 
-class LocalFile(HopprBaseModel):
-    """
-    LocalFile data model
-    """
-
-    local: Path
-
-
-class OciFile(HopprBaseModel):
-    """
-    OciFile data model
-    """
-
-    oci: AnyUrl | str
-
-
-class UrlFile(HopprBaseModel):
-    """
-    UrlFile data model
-    """
-
-    url: HttpUrl | FileUrl | AnyUrl | str
-
-
 class SearchSequence(HopprBaseModel):
     """
     SearchSequence data model
     """
 
     version: Literal["v1"]
     repositories: list[RepositoryUrl | str] = []
 
 
 IncludeRef = Annotated[LocalFile | UrlFile, Field(..., description="Reference to a local or remote manifest file")]
 Includes = Annotated[list[IncludeRef], Field(..., description="List of manifest files to load")]
-SbomRef = Annotated[LocalFile | OciFile | UrlFile, Field(..., description="Reference to a local or remote SBOM file")]
-Sboms = Annotated[list[SbomRef], Field(..., description="List of SBOMs to process")]
-SbomRefMap = Annotated[MutableMapping[SbomRef, "Sbom"], Field(...)]
-ComponentPurlMap = Annotated[MutableMapping[str, "Component"], Field(...)]
-
-
-class ExternalReference(HopprBaseModel, ExternalReferenceSpecVersion14):
-    """
-    ExternalReference data model derived from HopprBaseModel
-    """
-
-    class Config(HopprBaseModel.Config):  # pylint: disable=too-few-public-methods
-        "Config for ExternalReference model"
-        extra = Extra.allow
-
-
-class Property(HopprBaseModel, PropertySpecVersion14):
-    """
-    Property data model derived from HopprBaseModel
-    """
-
-
-class Component(HopprBaseModel, ComponentSpecVersion14):
-    """
-    Component data model derived from HopprBaseModel
-    """
-
-    class Config(HopprBaseModel.Config):  # pylint: disable=too-few-public-methods
-        "Config for Component model"
-        extra = Extra.allow
-
-    components: list[Component] | None = Field(None)  # type: ignore[assignment]
-    externalReferences: list[ExternalReference] | None = Field(None)  # type: ignore[assignment]
-    properties: list[Property] | None = Field(None)  # type: ignore[assignment]
-
-    # Attributes not included in schema
-    component_lookup: ClassVar[ComponentPurlMap] = {}
-
-    @classmethod
-    def find(cls, purl_string: str) -> Component | None:
-        """
-        Look up Component object by package URL string
-
-        Args:
-            purl_string (str): Package URL string to look up
-
-        Returns:
-            Component | None: Component object if found, otherwise None
-        """
-        return cls.component_lookup.get(purl_string)
-
-
-class Sbom(HopprBaseModel, SbomSpecVersion14):
-    """
-    Sbom data model derived from HopprBaseModel
-    """
-
-    class Config(HopprBaseModel.Config):  # pylint: disable=too-few-public-methods
-        "Config for generic Sbom model"
-
-        extra = Extra.allow
-
-    components: list[Component] = Field(...)  # type: ignore[assignment]
-    externalReferences: list[ExternalReference] | None = Field(None)  # type: ignore[assignment]
-
-    # Attributes not included in schema
-    loaded_sboms: ClassVar[SbomRefMap] = {}
-    consolidated_sbom: ClassVar[Sbom]
-
-    @classmethod
-    def find(cls, ref_type: Literal["local", "oci", "url"], location: str | Path) -> Sbom | None:
-        """
-        Look up SBOM object by reference
-
-        Args:
-            ref_type (Literal["local", "oci", "url"]): Type of SBOM reference
-            location (str | Path): Location of SBOM reference
-
-        Returns:
-            Sbom | None: SBOM object if found, otherwise None
-        """
-        match ref_type:
-            case "local":
-                return cls.loaded_sboms.get(LocalFile(local=Path(location)), None)
-            case "oci":
-                return cls.loaded_sboms.get(OciFile(oci=str(location)), None)
-            case "url":
-                return cls.loaded_sboms.get(UrlFile(url=str(location)), None)
-            case _:
-                return None
+IncludeRefMap = Annotated[MutableMapping[IncludeRef, "ManifestFile"], Field(...)]
 
 
 class ManifestFile(HopprBaseSchemaModel):
     """
     Data model to describe a single manifest file
     """
 
     kind: Literal["Manifest"]
     repositories: Repositories = Field(..., description="Maps supported PURL types to package repositories/registries")
     includes: Includes = []
-    sboms: Sboms = []
+    sboms: list[SbomRef] = []
 
     @classmethod
     def parse_file(cls, path: str | Path, *args, **kwargs) -> ManifestFile:  # pylint: disable=unused-argument
         """
         Override to resolve local file paths relative to manifest file
         """
         path = Path(path).resolve()
@@ -250,22 +131,21 @@
             if "local" in sbom and not Path(sbom["local"]).is_absolute():
                 secho(f"Skipping local SBOM: relative path '{sbom['local']}' cannot be resolved", fg="yellow")
                 obj["sboms"].remove(sbom)
 
         return cls(**obj)
 
 
-IncludeRefMap = Annotated[MutableMapping[IncludeRef, ManifestFile], Field(...)]
-
-
 class Manifest(ManifestFile):
     """
     Manifest data model that generates lookups for `includes` and `sboms` references
     """
 
+    consolidated_sbom: Sbom = Field(default=Sbom(), exclude=True)  # pyright: ignore
+
     # Attributes not included in schema
     loaded_manifests: ClassVar[IncludeRefMap] = {}
 
     @validator("includes", allow_reuse=True, always=True)
     @classmethod
     def populate_loaded_manifests(cls, includes: Includes, values: DictStrAny) -> Includes:
         """
@@ -305,138 +185,99 @@
 
                 cls.loaded_manifests[include_ref] = loaded
 
         return includes
 
     @validator("sboms", allow_reuse=True, always=True)
     @classmethod
-    def populate_loaded_sboms(cls, sboms: Sboms, values: DictStrAny) -> Sboms:
+    def populate_loaded_sboms(cls, sboms: list[SbomRef], values: DictStrAny) -> list[SbomRef]:
         """
         Validator that automatically loads SBOM from local file or URL into lookup dictionary
         """
-        if not hasattr(Sbom, "consolidated_sbom"):
-            Sbom.consolidated_sbom = Sbom(
-                specVersion="1.4",
-                version=1,
-                bomFormat="CycloneDX",  # type: ignore[arg-type]
-                serialNumber=uuid.uuid4().urn,
-                components=[],
-                externalReferences=[],
-            )
-
         for sbom_ref in sboms:
             if sbom_ref not in Sbom.loaded_sboms:
-                loaded = cls._load_sbom(sbom_ref)
-                ref_url = cls._get_ref_url(sbom_ref)
-
-                if loaded is None or ref_url is None:
+                if (loaded_sbom := cls._load_sbom(sbom_ref)) is None:
                     continue
 
-                loaded_sn = getattr(loaded, "serialNumber")
-
                 # Merge current SBOM metadata into consolidated SBOM
-                Sbom.consolidated_sbom.externalReferences.append(  # type: ignore[union-attr]
-                    ExternalReference(
-                        url=ref_url,
-                        type="bom",  # type: ignore[arg-type]
-                        comment=loaded_sn,
-                        hashes=None,
-                    )
-                )
-
-                for component in loaded.components or []:
-                    purl_str = getattr(component, "purl", None)
-                    if purl_str is None:
+                for component in loaded_sbom.components or []:
+                    if not (purl_str := getattr(component, "purl", None)):
                         continue
 
                     purl_type = hoppr.utils.get_package_url(purl_str).type
 
-                    if component.properties is None:
-                        component.properties = []
-
                     # Generate the repository search sequence
                     search_sequence = SearchSequence(
                         version="v1", repositories=[str(repo.url) for repo in values["repositories"][purl_type]]
                     )
 
                     # Add repository search sequence as component property
                     component.properties.append(
                         Property(name=BomProps.COMPONENT_SEARCH_SEQUENCE, value=search_sequence.json())
                     )
 
                     # Add external reference to SBOM file that includes this component
-                    if component.externalReferences is None:
-                        component.externalReferences = []
-
                     component.externalReferences.append(
                         ExternalReference(
-                            url=ref_url, comment=loaded_sn, type="bom", hashes=None  # type: ignore[arg-type]
+                            url=str(sbom_ref),
+                            type="bom",  # type: ignore[arg-type]
+                            comment=loaded_sbom.serialNumber,
+                            hashes=None,
                         )
                     )
 
                     # Merge component into consolidated SBOM
                     cls._add_component(component)
 
-                Sbom.loaded_sboms[sbom_ref] = loaded
-
         return sboms
 
+    @validator("consolidated_sbom", allow_reuse=True, always=True)
     @classmethod
-    def _add_component(cls, component: Component) -> None:
-        # Remove purl qualifiers for later comparison
-        purl: PackageURL = hoppr.utils.get_package_url(component.purl)
-        purl.qualifiers.clear()
-        purl_str = purl.to_string()
-
-        loaded = Component.find(purl_str)
-        # Merge component into previously loaded component
-        if loaded is not None:
-            loaded.externalReferences = hoppr.utils.dedup_list(
-                [*(loaded.externalReferences or []), *(component.externalReferences or [])]
+    def populate_consolidated_sbom(cls, consolidated_sbom: Sbom) -> Sbom:
+        """
+        Populate `consolidated_sbom` with previously loaded `components` and `externalReferences`
+        """
+        for sbom_ref, sbom in Sbom.loaded_sboms.items():
+            external_ref = ExternalReference(
+                url=str(sbom_ref),
+                type="bom",  # type: ignore[arg-type]
+                comment=sbom.serialNumber,
+                hashes=None,
             )
 
-            if loaded.properties is None:
-                loaded.properties = []  # pragma: no cover
+            sbom.externalReferences = hoppr.utils.dedup_list([*sbom.externalReferences, external_ref])
 
-            for prop in component.properties or []:
-                if prop.name not in [loaded_prop.name for loaded_prop in loaded.properties]:
-                    loaded.properties.append(prop)
-        else:
-            Sbom.consolidated_sbom.components.append(component)
-            Component.component_lookup[purl_str] = component
+            for component in sbom.components:
+                component.externalReferences = hoppr.utils.dedup_list([*component.externalReferences, external_ref])
+
+            consolidated_sbom.merge(sbom)
+
+        return consolidated_sbom
 
     @classmethod
-    def _get_ref_url(cls, sbom_ref: SbomRef) -> str | None:
-        match sbom_ref:
-            case LocalFile():
-                return sbom_ref.local.as_uri()
-            case OciFile():
-                return sbom_ref.oci
-            case UrlFile():
-                return sbom_ref.url
-            case _:
-                return None
+    def _add_component(cls, component: Component) -> None:
+        # Merge component into previously loaded component
+        if loaded := Component.find(component.bom_ref):
+            loaded.merge(component)
+        else:
+            Component.unique_id_map[component.bom_ref] = component
 
     @classmethod
     def _load_sbom(cls, sbom_ref: SbomRef) -> Sbom | None:
         match sbom_ref:
             case LocalFile():
-                return Sbom.parse_file(sbom_ref.local)
+                return Sbom.load(sbom_ref.local)
             case OciFile():
                 data = hoppr.oci_artifacts.pull_artifact(sbom_ref.oci)
                 if not isinstance(data, dict):
                     raise TypeError("OCI URL SBOM file was not loaded as dictionary")
 
-                return Sbom.parse_obj(data)
+                return Sbom.load(data)
             case UrlFile():
-                data = hoppr.net.load_url(sbom_ref.url)
-                if not isinstance(data, dict):
-                    raise TypeError("URL SBOM file was not loaded as dictionary")
-
-                return Sbom.parse_obj(data)
+                return Sbom.load(sbom_ref.url)
             case _:
                 return None
 
     @classmethod
     def find(cls, ref_type: Literal["local", "url"], location: str | Path) -> ManifestFile | None:
         """
         Lookup manifest object by include reference
```

### Comparing `hoppr-1.8.8/hoppr/models/transfer.py` & `hoppr-1.9.0/hoppr/models/transfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import math
 import re
 
 from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, Annotated, Any, Literal, Pattern
 
-from pydantic import ConstrainedStr, Field, validator
+from importlib.metadata import entry_points
+from pydantic import ConstrainedStr, Field, validator, root_validator
 
 from hoppr.models.base import HopprBaseModel, HopprBaseSchemaModel
 
 if TYPE_CHECKING:
     from pydantic.typing import DictStrAny
 else:
     DictStrAny = dict[str, Any]
@@ -34,14 +35,30 @@
     """
     Plugin data model
     """
 
     name: str = Field(..., description="Name of plugin")
     config: DictStrAny | None = Field(None, description="Mapping of additional plugin configuration settings to values")
 
+    @root_validator(pre=True)
+    @classmethod
+    def validate_model(cls, values: DictStrAny):
+        """
+        Validate Plugin model
+        """
+        name = values.get("name")
+        plugin_eps = entry_points(group='hoppr.plugin')
+
+        for plugin in plugin_eps:
+            if str(name) in plugin.value:
+                values["name"] = plugin.value.split(":")[0]
+                break
+
+        return values
+
 
 Plugin.update_forward_refs()
 
 
 class ComponentCoverage(Enum):
     """
     Enumeration to indicate how often each component should be processed
@@ -116,14 +133,15 @@
         add_delta = True
 
         for stage_name, stage in stages.items():
             stage["name"] = stage_name
             stage_refs.append(StageRef.parse_obj(stage))
 
             for plugin in stage["plugins"]:
+                plugin = Plugin.validate_model(plugin)
                 if plugin["name"] == "hoppr.core_plugins.delta_sbom":
                     add_delta = False
 
         if add_delta:
             stage_refs.insert(
                 0,
                 StageRef(
```

### Comparing `hoppr-1.8.8/hoppr/models/types.py` & `hoppr-1.9.0/hoppr/models/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,61 @@
 """
 Enumeration to indicate how a plugin may change a BOM
 """
 from __future__ import annotations
 
 import re
 
+from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from hoppr_cyclonedx_models.cyclonedx_1_4 import Component
 from hoppr_cyclonedx_models.cyclonedx_1_4 import CyclonedxSoftwareBillOfMaterialsStandard as Bom
-from pydantic import Field, SecretStr, root_validator
+from pydantic import AnyUrl, Field, FileUrl, HttpUrl, SecretStr, root_validator
 from pydantic_yaml import YamlIntEnum, YamlStrEnum
 
 from hoppr.models.base import HopprBaseModel
 
 if TYPE_CHECKING:
     from pydantic.typing import DictStrAny
 
 
+class LocalFile(HopprBaseModel):
+    """
+    LocalFile data model
+    """
+
+    local: Path
+
+    def __str__(self) -> str:
+        return self.local.as_uri()
+
+
+class OciFile(HopprBaseModel):
+    """
+    OciFile data model
+    """
+
+    oci: AnyUrl | str
+
+    def __str__(self) -> str:
+        return str(self.oci)
+
+
+class UrlFile(HopprBaseModel):
+    """
+    UrlFile data model
+    """
+
+    url: HttpUrl | FileUrl | AnyUrl | str
+
+    def __str__(self) -> str:
+        return str(self.url)
+
+
 class BomAccess(YamlIntEnum):
     """
     Enumeration to indicate how a plugin may change a BOM
     """
 
     # pylint: disable=duplicate-code
     NO_ACCESS = 0
@@ -43,24 +77,26 @@
 
 class PurlType(YamlStrEnum):
     """
     Enumeration of supported purl types
     """
 
     # pylint: disable=duplicate-code
+    CARGO = "cargo"
     DEB = "deb"
     DOCKER = "docker"
     GENERIC = "generic"
     GIT = "git"
     GITHUB = "github"
     GITLAB = "gitlab"
     GOLANG = "golang"
     HELM = "helm"
     MAVEN = "maven"
     NPM = "npm"
+    NUGET = "nuget"
     PYPI = "pypi"
     RAW = "raw"
     REPO = "repo"
     RPM = "rpm"
 
 
 class RepositoryUrl(HopprBaseModel):
@@ -92,14 +128,17 @@
         """
         if not (url := values.get("url")):
             raise ValueError("Input parameter `url` must be a non-empty string")
 
         if url.endswith(":"):
             url = f"{url}//"
 
+        if "://" not in url:
+            url = f"http://{url}"
+
         if not (
             match := re.search(
                 pattern=(
                     r"^((?P<scheme>[^:/?#]+):(?=//))?(//)?((("
                     r"?P<username>[^:]+)(?::("
                     r"?P<password>[^@]+)?)?@)?("
                     r"?P<hostname>[^@/?#:]*)(?::("
```

### Comparing `hoppr-1.8.8/hoppr/net.py` & `hoppr-1.9.0/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/oci_artifacts.py` & `hoppr-1.9.0/hoppr/oci_artifacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Functions to faciliate interaction with non-image OCI Artifacts"""
 import re
 
 from pathlib import Path
 from typing import Dict, Tuple
 
-from oras.client import OrasClient  # type: ignore[import]
-from oras.container import Container  # type: ignore[import]
-from oras.provider import Registry  # type: ignore[import]
+from oras.client import OrasClient
+from oras.container import Container
+from oras.provider import Registry
 
 from hoppr import utils
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models.credentials import Credentials
 
 # Regex per: https://semver.org/#is-there-a-suggested-regular-expression-regex-to-check-a-semver-string
 SEM_VER_CORE_REGEX = r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$"
```

### Comparing `hoppr-1.8.8/hoppr/plugin_utils.py` & `hoppr-1.9.0/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/processor.py` & `hoppr-1.9.0/hoppr/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,39 @@
 import socket
 import sys
 import tempfile
 import time
 import uuid
 
 from concurrent.futures import Future, ThreadPoolExecutor, as_completed
-from copy import deepcopy
 from datetime import datetime
 from multiprocessing import cpu_count
 from os import PathLike
 from pathlib import Path
 from threading import _RLock as RLock
 from typing import Any, MutableMapping
 from urllib.parse import quote_plus
 
 import jmespath
 
 from packageurl import PackageURL
 from typer import colors, echo, secho
 
+import hoppr.utils
+
 from hoppr import __version__
 from hoppr.base_plugins.hoppr import HopprPlugin
 from hoppr.core_plugins.report_generator import Report, ReportGenerator
 from hoppr.exceptions import HopprPluginError
 from hoppr.in_toto import HopprInTotoLinks
 from hoppr.mem_logger import MemoryLogger
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
-from hoppr.models.manifest import Component, Manifest, ManifestFile, Sbom
+from hoppr.models.manifest import Manifest, ManifestFile
+from hoppr.models.sbom import Component, Sbom
 from hoppr.models.transfer import ComponentCoverage, Plugin, StageRef, Transfer
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
 from hoppr.utils import plugin_class, plugin_instance
 
 # Import on Unix systems only
 if os.name == "posix":
@@ -53,32 +55,31 @@
     config: dict[str, Any] | None,
     method_name: str,
     component: Component | None,
 ) -> Result:
     """
     Runs a single method for a single component (if supplied) on a single plugin
     """
-    plugin = plugin_instance(plugin_name, context, config)
+    plugin = hoppr.utils.plugin_instance(plugin_name, context, config)
 
     match method_name:
         case HopprPlugin.pre_stage_process.__name__:
             result = plugin.pre_stage_process()
         case HopprPlugin.process_component.__name__:
             result = plugin.process_component(component)
         case HopprPlugin.post_stage_process.__name__:
             result = plugin.post_stage_process()
         case _:
             result = Result.fail(f"Invalid method: {method_name}")
 
-    if result.return_obj is not None:
-        if not plugin.bom_access.has_access_to(result.return_obj):
-            result = Result.fail(
-                f"Plugin {type(plugin).__name__} has BOM access level {plugin.bom_access.name}, "
-                f"but returned an object of type {type(result.return_obj).__name__}"
-            )
+    if result.return_obj is not None and not plugin.bom_access.has_access_to(result.return_obj):
+        result = Result.fail(
+            f"Plugin {type(plugin).__name__} has BOM access level {plugin.bom_access.name}, "
+            f"but returned an object of type {type(result.return_obj).__name__}"
+        )
 
     return result
 
 
 class StageProcessor:  # pylint: disable=too-few-public-methods
     """
     Class to handle all processing within a single Hoppr stage
@@ -86,27 +87,32 @@
 
     component_based_methods = [HopprPlugin.process_component.__name__]
 
     def __init__(self, stage_ref: StageRef, context: HopprContext):
         self.stage_id = stage_ref.name
         self.context = context
         self.plugin_ref_list = stage_ref.plugins
+
         self.config_component_coverage = None
         if stage_ref.component_coverage is not None:
             self.config_component_coverage = ComponentCoverage[str(stage_ref.component_coverage)]
+
         self.required_coverage = ComponentCoverage.OPTIONAL
         self.results: dict[str, list[tuple[str, str | None, Result]]] = {}
 
     def run(self) -> Result:
         """
         Run all processes for this stage
         """
         try:
             self.plugin_ref_list = self._get_stage_plugins()
             self.required_coverage = self._get_required_coverage()
+
+            if not self.plugin_ref_list and str(self.required_coverage) in {"EXACTLY_ONCE", "AT_LEAST_ONCE"}:
+                raise HopprPluginError(f"No plugins were loaded, but required coverage is {self.required_coverage}")
         except (ModuleNotFoundError, HopprPluginError) as err:
             return Result.fail(str(err))
 
         result = self._check_bom_access()
         if not result.is_success():
             return result
 
@@ -240,31 +246,32 @@
     def _get_required_coverage(self) -> ComponentCoverage:
         if self.config_component_coverage is not None:
             return self.config_component_coverage
 
         if len(self.plugin_ref_list) == 0:
             return ComponentCoverage.OPTIONAL
 
-        plugin = plugin_class(self.plugin_ref_list[0].name)
+        plugin = hoppr.utils.plugin_class(self.plugin_ref_list[0].name)
         coverage = plugin.default_component_coverage
 
         for plugin_ref in self.plugin_ref_list:
-            plugin = plugin_class(plugin_ref.name)
+            plugin = hoppr.utils.plugin_class(plugin_ref.name)
             if plugin.default_component_coverage != coverage:
                 raise HopprPluginError(
                     f"Plugins for stage {self.stage_id} do not have consistent default "
                     "component coverage values. The value may be overridden in transfer file."
                 )
 
         return coverage
 
     def _check_component_coverage(self, method_name: str) -> int:
         result_count: dict[str | None, int] = {}
-        for _, purl, _ in self.results.get(method_name, []):
-            result_count[purl] = result_count.get(purl, 0) + 1
+
+        for _, bom_ref, _ in self.results.get(method_name, []):
+            result_count[bom_ref] = result_count.get(bom_ref, 0) + 1
 
         additional_failures = 0
         for component in self.context.delivered_sbom.components or []:
             count = result_count.get(component.purl, 0)
             if not self.required_coverage.accepts_count(count) and str(component.scope) not in {
                 'excluded',
                 'Scope.excluded',
@@ -275,20 +282,18 @@
                 self._save_result(method_name, f"Stage {self.stage_id}", bad_comp_result, component)
                 self._report_result(f"Stage {self.stage_id}", component, bad_comp_result)
                 additional_failures += 1
 
         return additional_failures
 
     def _check_bom_access(self) -> Result:
-        access_counts: dict[BomAccess, list[str]] = {}
-        for access in BomAccess:
-            access_counts[access] = []
+        access_counts: dict[BomAccess, list[str]] = {access: [] for access in BomAccess}
 
         for plugin_ref in self.plugin_ref_list:
-            plugin_cls = plugin_class(plugin_ref.name)
+            plugin_cls = hoppr.utils.plugin_class(plugin_ref.name)
             access_counts[plugin_cls.bom_access].append(plugin_cls.__name__)
 
         if len(access_counts[BomAccess.FULL_ACCESS]) > 0 and len(self.plugin_ref_list) > 1:
             msg = (
                 f"Stage {self.stage_id} has one or more plugins with {BomAccess.FULL_ACCESS.name}: "
                 f"{', '.join(access_counts[BomAccess.FULL_ACCESS])}"
                 ", and multiple plugins defined for the stage."
@@ -320,38 +325,35 @@
         elif isinstance(return_obj, Sbom):
             self.context.delivered_sbom = return_obj
 
     @staticmethod
     def _report_result(plugin: str, comp: Component | None, result: Result):
         desc = f"      {plugin} {result.status.name}"
         if comp is not None:
-            desc = desc + f" for {comp.purl}"
+            desc = f"{desc} for {comp.purl}"
 
         if result.is_success():
             color = colors.GREEN
         elif result.is_excluded():
             color = colors.YELLOW
         else:
             color = colors.RED
         if result.message:
-            desc = desc + f": {result.message}"
+            desc = f"{desc}: {result.message}"
         secho(desc, fg=color)
 
     def _save_result(self, method_name: str, plugin: str, result: Result, comp: Component | None):
         """
         Store the results for later use
         """
-        comp_string = None
-        if comp is not None and PackageURL.from_string(comp.purl) is not None:
-            comp_string = comp.purl
+        comp_string = comp.bom_ref if comp is not None else None
 
         # If needed, create a new list for this method
         # Might need to expand this definition in the future to separate by plug-in
-
-        if not method_name in self.results:
+        if method_name not in self.results:
             self.results[method_name] = []
 
         self.results[method_name].append((plugin, comp_string, result))
 
     def _get_stage_plugins(self) -> list[Plugin]:
         """
         Determine list of plugin references used in this stage
@@ -360,21 +362,21 @@
 
         # Get list of all component PURLs that are not None
         results = jmespath.search(
             expression="components[*].purl | not_null(@)",
             data=self.context.delivered_sbom.dict(by_alias=True),
         )
 
-        used_purl_types.update(PackageURL.from_string(purl).type for purl in results)
+        used_purl_types.update(hoppr.utils.get_package_url(purl).type for purl in results)
 
         plugin_list: list[Plugin] = []
 
         # Loop over copy of transfer plugin references
         for plugin_ref in set(self.plugin_ref_list):
-            plugin_cls = plugin_class(plugin_ref.name)
+            plugin_cls = hoppr.utils.plugin_class(plugin_ref.name)
 
             # Determine if plugin's `supported_purl_types` are in the set of PURL types defined in SBOM components
             plugin_needed: bool = len(used_purl_types.intersection(plugin_cls.supported_purl_types)) > 0
 
             if len(plugin_cls.supported_purl_types) == 0 or plugin_needed:
                 plugin_list.append(plugin_ref)
 
@@ -595,17 +597,17 @@
         result = Result.success()
 
         with tempfile.TemporaryDirectory() as collection_root, multiprocessing.Manager() as manager:
             logfile_lock = manager.RLock()
 
             self.context = HopprContext(
                 collect_root_dir=Path(collection_root).resolve(),
-                consolidated_sbom=deepcopy(Sbom.consolidated_sbom),
+                consolidated_sbom=self.manifest.consolidated_sbom.copy(deep=True),
                 credential_required_services=getattr(self.credentials, "credential_required_services", None),
-                delivered_sbom=deepcopy(Sbom.consolidated_sbom),
+                delivered_sbom=self.manifest.consolidated_sbom.copy(deep=True),
                 log_level=self.log_level,
                 logfile_location=self.log_file,
                 logfile_lock=logfile_lock,
                 max_processes=self.transfer.max_processes or cpu_count(),
                 repositories=self.manifest.repositories,
                 sboms=list(Sbom.loaded_sboms.values()),
                 stages=self.transfer.stages,
@@ -630,18 +632,16 @@
             self._collect_consolidated_bom()
             self.in_toto_links.record_stage_stop("_collect_metadata")
 
             # Reset some class variables (we should refactor to use instance variables, see issue
             # https://gitlab.com/hoppr/hoppr/-/issues/230) so that:
             #   1: The consolidated bom cannot be modified
             #   2: Plug-ins may choose to load other manifests.
-            del Sbom.consolidated_sbom
-            Component.component_lookup = {}
-            Component.components = []
-            Component.properties = []
+            Sbom.unique_id_map = {}
+            Component.unique_id_map = {}
             Manifest.loaded_manifests = {}
 
             msg = f"Beginning Hoppr Process execution, max_processes={self.context.max_processes}"
             self.logger.info(msg=msg)
             echo(message=msg)
 
             for stage_ref in self.transfer.stages:
```

### Comparing `hoppr-1.8.8/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.9.0/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/result.py` & `hoppr-1.9.0/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.8/hoppr/utils.py` & `hoppr-1.9.0/hoppr/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,114 @@
 """
 Hoppr utility functions
 """
 from __future__ import annotations
 
 import importlib
 import inspect
+import pyclbr
 
-from abc import ABCMeta
 from functools import cache
+from importlib.metadata import entry_points
 from pathlib import Path
 from types import ModuleType
-from typing import TYPE_CHECKING, Any, Type
+from typing import TYPE_CHECKING, Any, Iterable, Type
+from urllib.parse import unquote
 
 from packageurl import PackageURL
 from ruamel.yaml import YAML
 from ruamel.yaml.parser import ParserError as YAMLParserError
 from ruamel.yaml.scanner import ScannerError as YAMLScannerError
 
 from hoppr.exceptions import HopprLoadDataError, HopprPluginError
 
 if TYPE_CHECKING:
     from hoppr.base_plugins.hoppr import HopprPlugin
     from hoppr.models import HopprContext
 
 
-def _class_in_module(cls_type: ABCMeta, plugin_module: ModuleType):
+def _class_in_module(plugin_module: ModuleType) -> Type[HopprPlugin]:
     """
-    Determines if the specified object is a class
-    defined in the module
-    """
-    return inspect.isclass(cls_type) and cls_type.__module__ == plugin_module.__name__
+    Find the appropriate class in given module
 
+    Args:
+        plugin_module (ModuleType): Previously loaded module to search for specified plugin class
 
-def plugin_class(plugin_name: str) -> Type[HopprPlugin]:
+    Raises:
+        HopprPluginError: No class definition or more than one class definition found in module
+
+    Returns:
+        Type[HopprPlugin]: Class type of plugin
     """
-    return a concrete class of an object defined by a plugin name
+    # Prevent circular import
+    base_cls = getattr(importlib.import_module(name="hoppr.base_plugins.hoppr"), "HopprPlugin")
 
-    Assumes the specified plugin will define exactly one concrete class, which
-    will be instaniated using a default constructor (i.e., one with no parameters).
+    # Get classes defined in plugin_module
+    module_members = pyclbr.readmodule(module=plugin_module.__name__)
+
+    def is_hoppr_plugin(obj: ModuleType):
+        return inspect.isclass(obj) and issubclass(obj, base_cls) and obj.__name__ in module_members
+
+    module_classes = dict(inspect.getmembers(object=plugin_module, predicate=is_hoppr_plugin))
+
+    match list(module_classes.keys()):
+        case []:
+            raise HopprPluginError(f"No class definition found in '{plugin_module.__name__}'.")
+        case [multiple_cls, *extra] if extra:
+            cls_names = ", ".join(f"'{cls_name}'" for cls_name in [multiple_cls, *extra])
+            raise HopprPluginError(f"Multiple candidate classes defined in '{plugin_module.__name__}': {cls_names}")
+
+    return list(module_classes.values())[0]
+
+
+def plugin_class(plugin_name: str) -> Type[HopprPlugin]:
     """
-    try:
-        plugin_module = importlib.import_module(name=plugin_name)
-    except ModuleNotFoundError as mnfe:
-        raise ModuleNotFoundError(f"Unable to locate plug-in {plugin_name}: {mnfe}") from mnfe
+    Get plugin class type from module path or class name
 
-    plugin_cls = None
+    If the plugin name references a module, it is assumed the module defines
+    exactly one subclass of `HopprPlugin`, which will be instantiated using
+    a default constructor (i.e., one with no parameters).
 
-    for cls_name, cls_type in inspect.getmembers(plugin_module, inspect.isclass):
-        if _class_in_module(cls_type, plugin_module):
-            if plugin_cls is not None:
-                raise HopprPluginError(
-                    f"Multiple candidate classes defined in {plugin_name}: {plugin_cls.__name__}, {cls_name}"
-                )
+    Args:
+        plugin_name (str): Name of the plugin module or class defined in transfer file
 
-            plugin_cls = cls_type
+    Raises:
+        ModuleNotFoundError: Import of specified module failed
+        HopprPluginError: No class definition or more than one class definition found in module
 
-    if plugin_cls is None:
-        raise HopprPluginError(f"No class definition found in in {plugin_name}.")
+    Returns:
+        Type[HopprPlugin]: Class type of plugin
+    """
+    discovered_plugins = entry_points(group="hoppr.plugin")
 
-    return plugin_cls
+    try:
+        if found_plugin := [
+            *discovered_plugins.select(name=plugin_name),
+            *discovered_plugins.select(module=plugin_name),
+            *discovered_plugins.select(attr=plugin_name),
+        ]:
+            match found_plugin:
+                case [found_one]:
+                    loaded = found_one.load()
+
+                    # Return directly if provided plugin name was loaded as a plugin class
+                    # Otherwise, search the loaded plugin module for appropriate class
+                    return loaded if inspect.isclass(loaded) else _class_in_module(loaded)
+                case [found_multiple, *extra]:
+                    matches = ", ".join(f"'{found.name}'" for found in [found_multiple, *extra])
+                    raise HopprPluginError(f"Multiple entry points matched '{plugin_name}': {matches}")
+
+        # Provided plugin name not found in entry points
+        # Attempt to load using fully qualified module path
+        loaded = importlib.import_module(name=plugin_name)
+        return _class_in_module(loaded)
+    except ModuleNotFoundError as mnfe:
+        raise ModuleNotFoundError(f"Unable to locate plug-in '{plugin_name}': {mnfe}") from mnfe
+    except HopprPluginError as ex:
+        raise ex
 
 
 def plugin_instance(plugin_name: str, context: HopprContext, config: Any = None):
     """
     Create an instance of an object defined by a plugin name
 
     Assumes the specified plugin will define exactly one concrete class, which
@@ -83,24 +129,23 @@
     # Replace tab characters with spaces to prevent parsing errors
     contents = contents.replace("\t", "  ")
     loaded_contents: dict | list | None = None
 
     try:
         # Applicable to both YAML and JSON formats since valid JSON data is also valid YAML
         yaml = YAML(typ="safe", pure=True)
-        contents = contents.replace("\t", "  ")
         loaded_contents = yaml.load(contents)
 
         # yaml.safe_load will sometimes return a single string rather than the required structure
         if isinstance(loaded_contents, str):
             raise HopprLoadDataError("Expected dictionary or list, but contents were loaded and returned as string")
     except (YAMLParserError, YAMLScannerError) as ex:
         raise HopprLoadDataError("Unable to recognize data as either json or yaml") from ex
     except HopprLoadDataError as ex:
-        raise HopprLoadDataError from ex
+        raise ex
 
     return loaded_contents
 
 
 def load_file(input_file_path: Path) -> dict | list | None:
     """
     Load file content (either JSON or YAML) into a dict
@@ -113,19 +158,19 @@
         content: str = input_file.read()
         if not content.strip():
             raise HopprLoadDataError(f"File {input_file_path} is empty.")
 
     return load_string(content)
 
 
-def dedup_list(list_in: list[Any]) -> list[Any]:
+def dedup_list(list_in: Iterable[Any]) -> list[Any]:
     """
     De-duplicate a list
     """
-    return list(dict.fromkeys(list_in)) if list_in is not None else []
+    return list(dict.fromkeys(list_in or []))
 
 
 def obscure_passwords(command_list: list[str], sensitive_args: list[str] | None = None) -> str:
     """
     Returns an input string with any specified passwords hidden
     """
 
@@ -175,8 +220,8 @@
     Args:
         purl_string (str): The string representation of a Package URL
 
     Returns:
         PackageURL: The object representation of a PackageURL
 
     """
-    return PackageURL.from_string(purl_string)  # pyright: ignore[reportGeneralTypeIssues]
+    return PackageURL.from_string(unquote(purl_string))
```

### Comparing `hoppr-1.8.8/PKG-INFO` & `hoppr-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.8
+Version: 1.9.0
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
@@ -15,24 +15,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: hoppr-cyclonedx-models (==0.4.7)
+Requires-Dist: hoppr-cyclonedx-models (>=0.4.7,<0.5.0)
 Requires-Dist: in-toto (>=1.3.1,<2.0.0)
 Requires-Dist: jc (>=1.22.2,<2.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: oras (>=0.1.17,<0.2.0)
-Requires-Dist: packageurl-python (>=0.10.0,<0.11.0)
+Requires-Dist: packageurl-python (>=0,<1)
 Requires-Dist: pydantic-yaml (>=0.10.0,<0.11.0)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
+Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: securesystemslib (==0.26.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: types-PyYAML (>=6.0.5,<7.0.0)
 Project-URL: Repository, https://gitlab.com/hoppr/hoppr
 Description-Content-Type: text/markdown
 
 <img src="https://gitlab.com/hoppr/hoppr/-/raw/dev/media/hoppr-repo-banner.png" />
 <br />
 <br />
@@ -44,20 +45,22 @@
 
 - **Documentation**: <https://hoppr.dev>
 - **Source Code**: <https://gitlab.com/hoppr/hoppr>
 
 # Getting Started
 
 ## Basic Install [from PyPI](https://pypi.org/project/hoppr/)
+
 ```
 pip install hoppr
 ```
 
 ## Quickstart Tutorial
 
 Once you have Hoppr installed, we recommend the ["Your First Bundle" tutorial](https://hoppr.dev/docs/using-hoppr/tutorials/your-first-bundle) to understand the basics.
 
-# Join Us!
+# Join Us
 
-We're completely open source, [MIT licensed](LICENSE), and community friendly. Built with a plugin architecture, Hoppr enables users to extend its SBOM-processing capabilities through their own plugins and algorithms.  
-[Learn more about how to contribute](https://hoppr.dev/docs/category/contribute-to-hoppr), it's easy and we've got
+We're completely open source, [MIT licensed](LICENSE), and community friendly. Built with a plugin architecture, Hoppr enables users to extend its SBOM-processing capabilities through their own plugins and algorithms.
+[Learn more about how to contribute](https://hoppr.dev/docs/development/contributing/guide), it's easy and we've got
 a welcoming community!
+
```

