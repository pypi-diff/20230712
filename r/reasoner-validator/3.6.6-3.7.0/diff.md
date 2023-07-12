# Comparing `tmp/reasoner_validator-3.6.6.tar.gz` & `tmp/reasoner_validator-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.6.6.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.0.tar", max compression
```

## Comparing `reasoner_validator-3.6.6.tar` & `reasoner_validator-3.7.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1153 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/LICENSE
--rw-r--r--   0        0        0    12620 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/README.md
--rw-r--r--   0        0        0      131 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/conf.py
--rw-r--r--   0        0        0    19640 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35958 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2094 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/pyproject.toml
--rw-r--r--   0        0        0    38154 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    63014 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39199 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    28625 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11484 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14019 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    11621 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      709 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/tests/conftest.py
--rw-r--r--   0        0        0   114459 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62106 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    38058 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_response_validator.py
--rw-r--r--   0        0        0     5997 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_semver.py
--rw-r--r--   0        0        0     2209 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26558 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_validate.py
--rw-r--r--   0        0        0    20333 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_workflows.py
--rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 reasoner_validator-3.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/LICENSE
+-rw-r--r--   0        0        0    12703 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/README.md
+-rw-r--r--   0        0        0      131 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/conf.py
+-rw-r--r--   0        0        0    19869 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-12 20:29:09.211841 reasoner_validator-3.7.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36258 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2177 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0    38452 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    75056 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39514 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/message.py
+-rw-r--r--   0        0        0    29459 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11643 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    12532 2023-07-12 20:29:09.215841 reasoner_validator-3.7.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      774 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/conftest.py
+-rw-r--r--   0        0        0   117951 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40085 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26808 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_validate.py
+-rw-r--r--   0        0        0    21576 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-12 20:29:09.219841 reasoner_validator-3.7.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.0/PKG-INFO
```

### Comparing `reasoner_validator-3.6.6/LICENSE` & `reasoner_validator-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/README.md` & `reasoner_validator-3.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,29 +140,29 @@
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
   "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
-  "sources": {
+  "target_provenance": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
-- An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
+- An **optional** `target_provenance` with an object dictionary (example shown) specifying the ARA and KP infores-specified knowledge sources expected to be recovered in the TRAPI query results (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "target_provenance" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
 First install the web-specific dependencies.
```

### Comparing `reasoner_validator-3.6.6/docs/Makefile` & `reasoner_validator-3.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/docs/conf.py` & `reasoner_validator-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/docs/index.rst` & `reasoner_validator-3.7.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 Top level programmatic validation of a TRAPI Response uses a TRAPIResponseValidator class wrapper as follows (sample script):
 
 .. code-block:: python
 
     #!/usr/bin/env python
     from typing import Optional, List, Dict
     from reasoner_validator import TRAPIResponseValidator
+    from reasoner_validator import MESSAGE_CATALOG
 
     SAMPLE_RESPONSE = {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
@@ -82,15 +83,15 @@
                 }
             }
         ]
     }
 
     }
     validator = TRAPIResponseValidator(
-        trapi_version="1.4.1",
+        trapi_version="1.4.2",
 
         # If omit or set the Biolink Model version parameter to None,
         # then the current Biolink Model Toolkit default release applies
         biolink_version="3.5.0",
 
         # 'sources' are set to trigger checking of expected edge knowledge source provenance
         sources={
@@ -107,102 +108,96 @@
     # but rather, return validation outcomes as a dictionary of validation messsages
     # Here, the 'message' parameter here is just the Python equivalent dictionary of the
     # TRAPI.Message JSON schema model component of the TRAPI Response (not the full TRAPI Response...yet)
 
     # this method validates a complete TRAPI Response JSON result
     validator.check_compliance_of_trapi_response(response=SAMPLE_RESPONSE)
 
-    # Messages are retrieved from the validator object as follows:
-    messages: Dict[
-                str,  # message type (errors|warnings|information)
-                Dict[
-                    str,  # message 'code' as indexing key
-                    # Dictionary of 'identifier' indexed messages with parameters
-                    # (Maybe None, if code doesn't have any additional parameters)
-                    Optional[
-                        Dict[
-                            str,  # key is the message-unique template 'identifier' value of parameterized messages
-                            Optional[
-                                List[
-                                    # Each reported message adds a dictionary of such parameters
-                                    # to the list here; these are not guaranteed to be unique
-                                    Dict[str, str]
-                                ]
-                            ]
-                        ]
-                    ]
-                ]
-            ] = validator.get_messages()
+    # Raw message data is retrieved from the validator object as follows:
+    messages: MESSAGE_CATALOG = validator.get_messages()
 
     # this method dumps a human readable text report of
     # the validation messages (default) to stdout
     # See the method signature for options that
     # allow customization of the text format.
     validator.dump()
 
 The 'messages' returned are partitioned into 'information', 'warning', 'error' and 'critical' (error) messages
 in a dictionary looking something like the following (as an example):
 
-Note that the trapi_version parameter to the TRAPIResponseValidator can also be a local path to a .yaml TRAPI schema file, which is read in and used as the validation standard. In such a case, though, it is necessary to encode the TRAPI version in the root filename, e.g. my_trapi_schema_1.4.0-beta5.yaml
-
 .. code-block:: python
 
     messages: Dict[str, List[Dict[str,str]]] = {
         "information": {
             "info.excluded": {
-                # the uniquely discriminating 'identifier' here is the edge_id
-                "(ZFIN:ZDB-GENE-060825-345$biolink:Gene)--[biolink:active_in]->(GO:0042645$biolink:CellularComponent)": None
-                # messages with only a contextual identifier may have no additional parameters
+                # source scope of the validation error ("global" or some knowledge source path string
+                "global": {
+                    # the uniquely discriminating 'identifier' here is the edge_id
+                    "(ZFIN:ZDB-GENE-060825-345$biolink:Gene)--[biolink:active_in]->(GO:0042645$biolink:CellularComponent)": None
+                    # messages with only a contextual identifier may have no additional parameters
                 },
                 {...}  # another message (same code type)
-            ,
+            },
             "info.compliant": None  # parameterless messages don't have distinct instances
              # other 'info' code-indexed messages
         },
         "warnings": {
             "warning.edge.predicate.non_canonical": {
-                # the uniquely discriminating 'identifier' here is the is the predicate term
-                "biolink:participates_in":
-                {   # the secondary context is the 'edge_id'
-                    "edge_id": "a--['biolink:participates_in']->b",
-                },
-                {...}  # another predicate indexed message (same code type)
-
+                "infores:chebi -> infores:molepro -> infores:arax": {
+                    # the uniquely discriminating 'identifier' here is the is the predicate term
+                    "biolink:participates_in":
+                    {   # the secondary context is the 'edge_id'
+                        "edge_id": "a--['biolink:participates_in']->b",
+                    },
+                    {...}  # another predicate indexed message (same code type)                
+                }
             },
             "warning.trapi.response.status.unknown" {
-                "500": None  # unexpected http status code returned
+                "global": {
+                    "500": None  # unexpected http status code returned
+                }
             },
             # other 'warning' code-indexed messages
         },
         "errors": {
             "error.biolink.model.noncompliance": {
-                "biolink:vitamin": {
-                    "biolink_release": "3.4.5"
+                "infores:chebi -> infores:molepro -> infores:arax": {
+                    "biolink:vitamin": {
+                        "biolink_release": "3.4.5"
+                    }
                 }
             },
             # other 'errors' code-indexed messages
         },
         "critical": {
             "critical.trapi.request.invalid": {
-                # subject node descriptor is the 'identifier'
-                "CHEBI:37565[biolink:SmallMolecule]":
-                {
-                    "test": "raise_subject_entity"
-                    "reason": "has no 'is_a' parent since it is either not an ontology term or does not map onto a parent ontology term."
-                },
-                {...} # another message (same code type)
+                "global": {
+                    # subject node descriptor is the 'identifier'
+                    "CHEBI:37565[biolink:SmallMolecule]":
+                    {
+                        "test": "raise_subject_entity"
+                        "reason": "has no 'is_a' parent since it is either not an ontology term or does not map onto a parent ontology term."
+                    },
+                    {...} # another message (same code type)                
+                }
             },
             # other 'critical' code-indexed messages
         }
     }
 
 
 Every message has a 'code' and optional context-specific parameters which correspond to
 named fields in the Python string templates found in the `reasoner_validator package 'codes.yaml' file <https://github.com/NCATSTranslator/reasoner-validator/blob/master/reasoner_validator/codes.yaml>`_.
 
+Note that the trapi_version parameter to the TRAPIResponseValidator can also be a local path to a .yaml TRAPI schema file, which is read in and used as the validation standard. In such a case, though, it is necessary to encode the TRAPI version as a suffix to the root filename, e.g. my_trapi_schema_1.4.0-beta5.yaml. Note that the TRAPI version suffix to the root file name is assumed to be delimited by a leading underscore character. The simplistic parsing of this version is as follows:
+
+.. code-block:: python
+    root_path: str = string.replace(".yaml", "")
+    semver_string = root_path.split("_")[-1]
+
 Python API
 ----------
 .. toctree::
    :maxdepth: 2
 
    TRAPI Response Validation <reasoner_validator>
    TRAPI Schema Validation <reasoner_validator.trapi>
@@ -249,15 +244,15 @@
         # If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
         # Otherwise, the TRAPI Response 'schema_version' (not 'latest') becomes the default validation version.
 
-        trapi_version="1.4.1",
+        trapi_version="1.4.2",
 
         # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
         # Otherwise, the TRAPI Response stated 'biolink_version' (not BMT) becomes the default validation version.
@@ -304,15 +299,15 @@
 --------------
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data as input to the **/validate** endpoint:
 
 .. code-block:: json
 
     {
-        "schema_version": "1.4.1",
+        "schema_version": "1.4.2",
         "biolink_version": "3.5.0",
         "message": {
             "query_graph": {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {"categories": ["biolink:Drug"]}
                 },
@@ -368,42 +363,48 @@
     }
 
 then, one should typically get a response body like the following JSON validation result back:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.4.1",
-      "biolink_version": "3.4.3",
+      "trapi_version": "1.4.2",
+      "biolink_version": "3.5.0",
       "messages": {
         "critical": {},
         "errors": {
           "error.knowledge_graph.node.category.missing": {
-            "MONDO:0005148": [
-              {
-                "context": "Knowledge Graph"
-              }
-            ]
+             "infores:chebi -> infores:molepro -> infores:arax": {
+                "MONDO:0005148": [
+                  {
+                    "context": "Knowledge Graph"
+                  }
+                ]
+            }
           }
         },
         "warnings": {
           "warning.knowledge_graph.node.id.unmapped_prefix": {
-            "CHEBI:6801": [
-              {
-                "categories": "['biolink:Drug']"
-              }
-            ]
+            "infores:chebi -> infores:molepro -> infores:arax": {
+                "CHEBI:6801": [
+                  {
+                    "categories": "['biolink:Drug']"
+                  }
+                ]
+            }
           },
           "warning.knowledge_graph.edge.provenance.kp.missing": {
-            "infores:panther": [
-              {
-                "kp_source_type": "biolink:primary_knowledge_source",
-                "identedge_idifier": "CHEBI:6801--biolink:treats->MONDO:0005148"
-              }
-            ]
+            "infores:chebi -> infores:molepro -> infores:arax": {
+                "infores:panther": [
+                  {
+                    "kp_source_type": "biolink:primary_knowledge_source",
+                    "identifier": "CHEBI:6801--biolink:treats->MONDO:0005148"
+                  }
+                ]
+            }
           }
         },
         "information": {}
       }
     }
 
 Validation Code Definitions
```

### Comparing `reasoner_validator-3.6.6/docs/make.bat` & `reasoner_validator-3.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.0/docs/validation_codes_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -894,14 +894,22 @@
 
 **Message:** Node has deprecated category
 
 **Context:** node_id, identifier
 
 **Description:** Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
 
+### warning.knowledge_graph.node.category.abstract_or_mixin
+
+**Message:** Node has a abstract or mixin category
+
+**Context:** node_id, identifier
+
+**Description:** Node category is abstract or a mixin in the current model. Please consider selecting a more specific, concrete Biolink Model category?
+
 ### warning.knowledge_graph.node.id.unmapped_prefix
 
 **Message:** Node identifier found unmapped to target categories for node
 
 **Context:** identifier, categories
 
 **Description:** Node CURIE identifier namespace not found among any 'id_prefix' slot values in specified categories in the validating Biolink Model version?
```

### Comparing `reasoner_validator-3.6.6/pyproject.toml` & `reasoner_validator-3.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.6.6"
+version = "3.7.0"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -38,37 +38,41 @@
     { path = "tests" },
     { path = "docs" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bmt = "^1.1.0"
-jsonschema = "^4.17.0"
+
+# jsonschema needs to be pinned to <= 4.18.0 for now,
+# since 4.18.0 appeared to break something for the
+# access and processing of JSON schemata
+jsonschema = "~4.17.3"
+
 PyYAML = "^6.0"
 requests = "^2.28.1"
 pydantic = "^1.10.11"
 urllib3 = "^1.26.15"
 numpydoc = {version = "^1.5.0", optional = true}
 sphinx = {version = "^5.3.0", optional = true}
 myst-parser = {version = "^0.18.1", optional = true}
 fastapi = {version = "^0.68", optional = true}
 uvicorn = {version = "^0.15", optional = true}
-pytest-cov = {version = "^4.0.0", optional = true}
-pytest = {version = "^7.2.2", optional = true}
+pytest-cov = {version = "^4.0.0"}
+pytest = {version = "^7.2.2"}
 sphinx-rtd-theme = {version = "^1.2.1", optional = true}
 
 
 [tool.poetry.urls]
 "Change Log" = "https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/NCATSTranslator/reasoner-validator/issues"
 
 [tool.poetry.extras]
 docs = ["numpydoc", "sphinx", "myst-parser", "sphinx-rtd-theme"]
 web = ["fastapi", "uvicorn"]
-dev = ["pytest", "pytest-cov"]
 
 [tool.coverage.run]
 source = ["reasoner_validator"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/__init__.py` & `reasoner_validator-3.7.0/reasoner_validator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,38 +42,34 @@
     TRAPI Validator is an overall wrapper class for validating
     conformance of TRAPI Responses to TRAPI and the Biolink Model.
     """
     def __init__(
             self,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
-            sources: Optional[Dict] = None,
             strict_validation: bool = False,
             suppress_empty_data_warnings: bool = False
     ):
         """
         :param trapi_version: version of component against which to validate the message (mandatory, no default)
         :type trapi_version: str
         :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
                                 validated (Default: if None, use the Biolink Model Toolkit default version).
         :type biolink_version: Optional[str] = None
-        :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation.
-        :type sources: Dict
         :param strict_validation: if True, some tests validate as 'error'; None or False, simply issue a 'warning'
         :type strict_validation: Optional[bool] = None
         :param suppress_empty_data_warnings: validation normally reports empty Message query graph, knowledge graph
                        and results as warnings. This flag suppresses the reporting of such warnings (default: False).
         :type suppress_empty_data_warnings: bool
         """
         ValidationReporter.__init__(
             self,
             prefix="Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
-            sources=sources,
             strict_validation=strict_validation
         )
         self._is_trapi_1_4: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
 
     def is_trapi_1_4(self) -> bool:
         assert self.trapi_version
@@ -131,15 +127,16 @@
                     step.pop('parameters')
         return response
 
     def check_compliance_of_trapi_response(
             self,
             response: Optional[Dict],
             max_kg_edges: int = 0,
-            max_results: int = 0
+            max_results: int = 0,
+            target_provenance: Optional[Dict] = None
     ):
         """
         One stop validation of all components of a TRAPI-schema compliant
         Query.Response, including its Message against a designated Biolink Model release.
         The high level structure of a Query.Response is described in
         https://github.com/NCATSTranslator/ReasonerAPI/blob/master/docs/reference.md#response-.
 
@@ -155,14 +152,16 @@
         :type response: Optional[Dict]
         :param max_kg_edges: integer maximum number of edges to be validated from the
                                      knowledge graph of the response. A value of zero triggers validation
                                       of all edges in the knowledge graph (Default: 0 - use all edges)
         :type max_kg_edges: int
         :param max_results: target sample number of results to validate (default: 0 for 'use all results').
         :type max_results: int
+        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :type target_provenance: Dict
 
         :returns: Validator cataloging "information", "warning" and "error" messages (could be empty)
         :rtype: ValidationReporter
         """
         if not (response and "message" in response):
             if not self.suppress_empty_data_warnings:
                 self.report("error.trapi.response.empty")
@@ -191,15 +190,15 @@
         status: Optional[str] = response['status'] if 'status' in response else None
         if status and status not in ["OK", "Success", "QueryNotTraversable", "KPsNotAvailable"]:
             self.report("warning.trapi.response.status.unknown", identifier=status)
 
         # Sequentially validate the Query Graph, Knowledge Graph then validate
         # the Results (which rely on the validity of the other two components)
         elif self.has_valid_query_graph(message) and \
-                self.has_valid_knowledge_graph(message, max_kg_edges):
+                self.has_valid_knowledge_graph(message, max_kg_edges, target_provenance):
             self.has_valid_results(message, max_results)
 
     @staticmethod
     def sample_results(results: List, sample_size: int = 0) -> List:
         """
         Subsample the results to a maximum size of 'sample_size'
 
@@ -308,23 +307,30 @@
                         self.merge(biolink_validator)
                         # 'info' and 'warning' messages do
                         # not fully invalidate the query_graph
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    def has_valid_knowledge_graph(self, message: Dict, edges_limit: int = 0) -> bool:
+    def has_valid_knowledge_graph(
+            self,
+            message: Dict,
+            edges_limit: int = 0,
+            target_provenance: Optional[Dict] = None
+    ) -> bool:
         """
         Validate a TRAPI Knowledge Graph.
 
         :param message: input message expected to contain the 'knowledge_graph'
         :type message: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
                             triggers validation of all edges in the knowledge graph (Default: 0 - use all edges)
         :type edges_limit: int
+        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :type target_provenance: Dict
 
         :return: bool, False, if validation errors
         """
         # This integrity constraint may not really be necessary
         # since negative numbers are functionally equivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
 
@@ -366,15 +372,15 @@
                     # Conduct validation of Biolink Model compliance of the
                     # Knowledge Graph, if Biolink validation not suppressed...
                     biolink_validator: BiolinkValidator = \
                         check_biolink_model_compliance_of_knowledge_graph(
                             graph=kg_sample,
                             trapi_version=self.trapi_version,
                             biolink_version=self.biolink_version,
-                            sources=self.sources,
+                            target_provenance=target_provenance,
                             # the ValidationReporter calling this function *might*
                             # have an explicit strict_validation override (if not None)
                             strict_validation=self.strict_validation
                         )
                     if biolink_validator.has_messages():
                         self.merge(biolink_validator)
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.0/reasoner_validator/biolink/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -141,38 +141,38 @@
     Wrapper class for Biolink Model validation.
     """
     def __init__(
         self,
         graph_type: TRAPIGraphType,
         trapi_version: Optional[str] = None,
         biolink_version: Optional[str] = None,
-        sources: Optional[Dict[str, str]] = None,
+        target_provenance: Optional[Dict[str, str]] = None,
         strict_validation: bool = False
     ):
         """
         Biolink Validator constructor.
 
         :param graph_type: type of graph data being validated
         :type graph_type: TRAPIGraphType
         :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
         :type trapi_version: Optional[str] or None
         :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
         :type biolink_version: Optional[str] or None
-        :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
-        :type sources: Optional[Dict[str,str]]
+        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :type target_provenance: Optional[Dict[str,str]]
         """
         BMTWrapper.__init__(self, biolink_version=biolink_version)
         ValidationReporter.__init__(
             self,
             prefix=f"Biolink Validation of {graph_type.value}",
             trapi_version=trapi_version,
             biolink_version=self.get_resolved_biolink_version(),
-            sources=sources,
             strict_validation=strict_validation
         )
+        self.target_provenance: Optional[Dict] = target_provenance
         self.graph_type: TRAPIGraphType = graph_type
         self.nodes: Set[str] = set()
 
     def minimum_required_biolink_version(self, version: str) -> bool:
         """
         :param version: simple 'major.minor.patch' Biolink Model SemVer
         :return: True if current version is equal to, or newer than, a targeted 'minimum_version'
@@ -326,185 +326,265 @@
 
             # constraints  # TODO: how do we validate node constraints?
             pass
 
     def set_nodes(self, nodes: Set):
         self.nodes.update(nodes)
 
-    def validate_element_status(self, context: str, identifier: str, edge_id: str) -> Optional[Element]:
+    def validate_element_status(
+            self,
+            context: str,
+            identifier: str,
+            edge_id: str,
+            source_trail: Optional[str] = None
+    ) -> Optional[Element]:
         """
         Detect element missing from Biolink, or is deprecated, abstract or mixin, signalled as a failure or warning.
 
         :param context: str, parsing context (e.g. 'Node')
         :param identifier: str, name of the putative Biolink element ('class')
         :param edge_id: str, identifier of enclosing edge containing the element (e.g. the 'edge_id')
-
+        :param source_trail: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         :return: Optional[Element], Biolink Element resolved to 'name' if element no validation error; None otherwise.
         """
         element: Optional[Element] = self.bmt.get_element(identifier)
         if not element:
-            self.report(code=f"error.{context}.unknown", identifier=identifier, edge_id=edge_id)
+            self.report(
+                code=f"error.{context}.unknown",
+                source_trail=source_trail,
+                identifier=identifier,
+                edge_id=edge_id
+            )
             return None
 
         if element.deprecated:
             # We won't index the instances where the deprecated element is seen, since we assume that
             # component developers learning about the issue will globally fix it in their graphs
-            self.report(code=f"warning.{context}.deprecated", identifier=identifier)
+            self.report(
+                code=f"warning.{context}.deprecated",
+                source_trail=source_trail,
+                identifier=identifier
+            )
             # return None - a deprecated term is not treated as a failure but just as a warning
 
         if element.abstract:
             if self.strict_validation:
-                self.report(code=f"error.{context}.abstract", identifier=identifier, edge_id=edge_id)
+                self.report(
+                    code=f"error.{context}.abstract",
+                    source_trail=source_trail,
+                    identifier=identifier,
+                    edge_id=edge_id
+                )
                 return None
             else:
-                self.report(code=f"info.{context}.abstract", identifier=identifier, edge_id=edge_id)
+                self.report(
+                    code=f"info.{context}.abstract",
+                    source_trail=source_trail,
+                    identifier=identifier,
+                    edge_id=edge_id
+                )
 
         elif self.bmt.is_mixin(identifier):
             # A mixin cannot be instantiated ...
             if self.strict_validation:
-                self.report(code=f"error.{context}.mixin", identifier=identifier, edge_id=edge_id)
+                self.report(
+                    code=f"error.{context}.mixin",
+                    source_trail=source_trail,
+                    identifier=identifier,
+                    edge_id=edge_id
+                )
                 return None
             else:
-                self.report(code=f"info.{context}.mixin", identifier=identifier, edge_id=edge_id)
+                self.report(
+                    code=f"info.{context}.mixin",
+                    source_trail=source_trail,
+                    identifier=identifier,
+                    edge_id=edge_id
+                )
 
         return element
 
-    def get_target_sources(self) -> Tuple[Optional[str], Optional[str], Optional[str]]:
+    def get_target_provenance(self) -> Tuple[Optional[str], Optional[str], Optional[str]]:
         """
-        Returns infores prefix normalized validation caller provided tTarget provenance sources metadata.
+        Returns infores-prefix-normalized target provenance metadata.
         :return: Tuple[Optional[str], Optional[str], Optional[str]] of ara_source, kp_source, kp_source_type
         """
         ara_source: Optional[str] = None
         kp_source: Optional[str] = None
         kp_source_type: Optional[str] = None
-        if self.sources:
-            if 'ara_source' in self.sources and self.sources['ara_source']:
-                ara_source: str = self.sources['ara_source']
+        if self.target_provenance:
+            if 'ara_source' in self.target_provenance and self.target_provenance['ara_source']:
+                ara_source: str = self.target_provenance['ara_source']
                 if not ara_source.startswith("infores:"):
                     ara_source = f"infores:{ara_source}"
-            if 'kp_source' in self.sources and self.sources['kp_source']:
-                kp_source: str = self.sources['kp_source']
+            if 'kp_source' in self.target_provenance and self.target_provenance['kp_source']:
+                kp_source: str = self.target_provenance['kp_source']
                 if not kp_source.startswith("infores:"):
                     kp_source = f"infores:{kp_source}"
-            kp_source_type = self.sources['kp_source_type'] \
-                if 'kp_source_type' in self.sources and self.sources['kp_source_type'] else 'aggregator'
+            kp_source_type = self.target_provenance['kp_source_type'] \
+                if 'kp_source_type' in self.target_provenance and self.target_provenance['kp_source_type'] else 'aggregator'
             kp_source_type = f"biolink:{kp_source_type}_knowledge_source"
 
         return ara_source, kp_source, kp_source_type
 
     def validate_provenance(
             self,
             edge_id,
             ara_source, found_ara_knowledge_source,
             kp_source, found_kp_knowledge_source, kp_source_type,
-            found_primary_knowledge_source
+            found_primary_knowledge_source,
+            source_trail: Optional[str]
     ):
         """
-        Validates ARA and KP sources based on surveyed Edge slots (in 'attributes' pre-1.4.0; in 'sources', post-1.4.0).
+        Validates ARA and KP infores knowledge sources based on surveyed Edge slots
+        (recorded in edge "attributes" pre-1.4.0; in "sources", post-1.4.0).
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param ara_source: str, user specified target ARA infores
         :param found_ara_knowledge_source: bool, True if target ARA infores knowledge source was found
         :param kp_source: str, user specified target KP infores
         :param found_kp_knowledge_source:  bool, True if target KP infores knowledge source was found
         :param kp_source_type:  str, user specified KP knowledge source type (i.e. primary, aggregate, etc.)
+        :param source_trail: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         :param found_primary_knowledge_source: List[str], list of all infores discovered tagged as 'primary'
         :return:
         """
         if ara_source and not found_ara_knowledge_source:
             # found target ARA knowledge source (if applicable)
             self.report(
                 code="warning.knowledge_graph.edge.provenance.ara.missing",
+                source_trail=source_trail,
                 identifier=ara_source,
                 edge_id=edge_id
             )
 
         if kp_source and not found_kp_knowledge_source:
             # found target KP knowledge source (if applicable)
             self.report(
                 code="warning.knowledge_graph.edge.provenance.kp.missing",
+                source_trail=source_trail,
                 identifier=kp_source,
                 kp_source_type=kp_source_type,
-                identedge_idifier=edge_id
+                edge_id=edge_id
             )
 
         if not found_primary_knowledge_source:
             # Found a primary tagged source...
             self.report(
                 code="error.knowledge_graph.edge.provenance.missing_primary",
+                source_trail=source_trail,
                 identifier=edge_id
             )
         elif len(found_primary_knowledge_source) > 1:
             # ... but only one!
             self.report(
                 code="warning.knowledge_graph.edge.provenance.multiple_primary",
+                source_trail=source_trail,
                 identifier=edge_id,
                 sources=",".join(found_primary_knowledge_source)
             )
 
-    def validate_attributes(self, edge_id: str, edge: Dict):
+    def validate_attributes(
+            self,
+            edge_id: str,
+            edge: Dict,
+            source_trail: Optional[str] = None
+    ) -> Optional[str]:
         """
-        Validate Knowledge Edge Attributes.
+        Validate Knowledge Edge Attributes. For TRAPI 1.3.0, may also return an ordered audit trail of Edge provenance
+        infores-specified knowledge sources, as parsed in from the list of attributes (returns 'None' otherwise).
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
-        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        :param source_trail: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
+        :return: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         """
+        # in TRAPI 1.4.0, the source_trail is parsed in from the Edge.sources annotation, hence
+        # the source_trail is already known and given to this method for reporting purposes here
+
+        # Otherwise, in TRAPI 1.3.0, the 'sources' may be compiled here, in this method, from the attributes
+        # themselves, then a newly generated 'source_trail', returned for use by the rest of the application
+        sources: Dict[str, List[str]] = dict()
+
         # we only report errors about missing or empty edge attributes if TRAPI 1.3.0 or earlier,
         # and Biolink Validation is not suppressed, since we can't fully validate provenance)
         # since earlier TRAPI releases are minimally expected to record provenance attributes
         # we only report this for TRAPI < 1.4 when Biolink Validation is done given that
         # without Biolink validation, provenance cannot be reliably assessed
 
+        # We can already use 'source_trail' here in the report in case it was
+        # already pre-computed by the validate_sources parsing of TRAPI 1.4.0;
+        # if TRAPI 1.3.0 is the validation standard, the 'source_trail' would
+        # be undefined here, since we can't figure it out without attributes!
         if 'attributes' not in edge:
             if self.validate_biolink() and not self.minimum_required_trapi_version("1.4.0-beta"):
-                self.report(code="error.knowledge_graph.edge.attribute.missing", identifier=edge_id)
+                self.report(
+                    code="error.knowledge_graph.edge.attribute.missing",
+                    identifier=edge_id,
+                    source_trail=source_trail
+                )
         elif not edge['attributes']:
             if self.validate_biolink() and not self.minimum_required_trapi_version("1.4.0-beta"):
-                self.report(code="error.knowledge_graph.edge.attribute.empty", identifier=edge_id)
+                self.report(
+                    code="error.knowledge_graph.edge.attribute.empty",
+                    identifier=edge_id,
+                    source_trail=source_trail
+                )
         elif not isinstance(edge['attributes'], List):
-            self.report(code="error.knowledge_graph.edge.attribute.not_array", identifier=edge_id)
+            self.report(
+                code="error.knowledge_graph.edge.attribute.not_array",
+                identifier=edge_id,
+                source_trail=source_trail
+            )
         else:
             attributes = edge['attributes']
 
+            # TODO: EDeutsch feedback: maybe we don't need to capture TRAPI 1.3.0 attribute-defined 'sources'
+            # raise NotImplementedError("Implement capture of 'sources' from TRAPI 1.3.0 attributes!")
+            # source_trail = self.build_source_trail(sources) if sources else None
+
             ara_source: Optional[str]
             kp_source: Optional[str]
             kp_source_type: Optional[str]
-            ara_source, kp_source, kp_source_type = self.get_target_sources()
+            ara_source, kp_source, kp_source_type = self.get_target_provenance()
 
             # Expecting ARA and KP 'aggregator_knowledge_source' attributes?
             found_ara_knowledge_source = False
             found_kp_knowledge_source = False
 
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
 
             for attribute in attributes:
 
                 # Validate attribute_type_id
                 if 'attribute_type_id' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.missing",
-                        identifier=edge_id
+                        identifier=edge_id,
+                        source_trail=source_trail
                     )
                 elif not attribute['attribute_type_id']:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.empty",
-                        identifier=edge_id
+                        identifier=edge_id,
+                        source_trail=source_trail
                     )
                 elif 'value' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.missing",
-                        identifier=edge_id
+                        identifier=edge_id,
+                        source_trail=source_trail
                     )
                 elif not attribute['value'] or \
                         str(attribute['value']).upper() in ["N/A", "NONE", "NULL"]:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.empty",
-                        identifier=edge_id
+                        identifier=edge_id,
+                        source_trail=source_trail
                     )
                 else:
                     attribute_type_id: str = attribute['attribute_type_id']
                     value = attribute['value']
 
                     # TODO: there seems to be non-uniformity in provenance attribute values for some KP/ARA's
                     #       in which a value is returned as a Python list (of at least one element?) instead
@@ -513,31 +593,34 @@
                     if not isinstance(value, List):
                         value = [value]
 
                     if not is_curie(attribute_type_id):
                         self.report(
                             code="error.knowledge_graph.edge.attribute.type_id.not_curie",
                             identifier=attribute_type_id,
-                            edge_id=edge_id
+                            edge_id=edge_id,
+                            source_trail=source_trail
                         )
                     elif self.validate_biolink():
                         # 'attribute_type_id' is a CURIE, but how well does it map?
                         prefix = attribute_type_id.split(":", 1)[0]
                         if prefix == 'biolink':
                             biolink_class = self.validate_element_status(
                                 context="knowledge_graph.edge.attribute.type_id",
                                 identifier=attribute_type_id,
-                                edge_id=edge_id
+                                edge_id=edge_id,
+                                source_trail=source_trail
                             )
                             if biolink_class:
                                 if not self.bmt.is_association_slot(attribute_type_id):
                                     self.report(
                                         code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
                                         identifier=attribute_type_id,
-                                        edge_id=edge_id
+                                        edge_id=edge_id,
+                                        source_trail=source_trail
                                     )
 
                                 else:
                                     # it is a Biolink 'association_slot' but now, validate what kind?
 
                                     # TODO: only check knowledge_source provenance here for now.
                                     #       Are there other association_slots to be validated here too?
@@ -563,15 +646,16 @@
 
                                         # ... now, check the infores values against various expectations
                                         for infores in value:
                                             if not infores.startswith("infores:"):
                                                 self.report(
                                                     code="error.knowledge_graph.edge.provenance.infores.missing",
                                                     identifier=str(infores),
-                                                    edge_id=edge_id
+                                                    edge_id=edge_id,
+                                                    source_trail=source_trail
                                                 )
                                             else:
                                                 if attribute_type_id == "biolink:primary_knowledge_source":
                                                     found_primary_knowledge_source.append(infores)
 
                                                 if ara_source and \
                                                         attribute_type_id == "biolink:aggregator_knowledge_source" and \
@@ -584,30 +668,34 @@
 
                         # if not a Biolink 'association_slot', at least, check if the 'attribute_type_id' has a
                         # namespace (prefix) known to Biolink. We won't call it a hard error, but issue a warning
                         elif not self.bmt.get_element_by_prefix(attribute_type_id):
                             self.report(
                                 code="warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
                                 identifier=attribute_type_id,
-                                edge_id=edge_id
+                                edge_id=edge_id,
+                                source_trail=source_trail
                             )
 
             # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
             if not self.minimum_required_trapi_version("1.4.0-beta") and self.validate_biolink():
                 # After all the attributes have been scanned,
                 # check for provenance. Treat as warnings for now.
                 # Note that provenance checking is only done when Biolink validation is done
                 # (since the various flags are not properly set above, for the test)
                 self.validate_provenance(
                     edge_id,
                     ara_source, found_ara_knowledge_source,
                     kp_source, found_kp_knowledge_source, kp_source_type,
-                    found_primary_knowledge_source
+                    found_primary_knowledge_source,
+                    source_trail=source_trail
                 )
 
+        return source_trail  # may be 'None' if the required attributes are missing
+
     def validate_attribute_constraints(self, edge_id: str, edge: Dict):
         """
         Validate Query Edge Attributes.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
@@ -731,73 +819,85 @@
                     qualifier_set: List = qualifier_set_entry['qualifier_set']
                     self.validate_qualifier_entry(
                         context="query_graph.edge.qualifier_constraints.qualifier_set",
                         edge_id=edge_id,
                         qualifiers=qualifier_set
                     )
 
-    def validate_infores(self, context: str, edge_id: str, identifier: str):
+    def validate_infores(self, context: str, edge_id: str, identifier: str) -> bool:
         code_prefix: str = f"error.knowledge_graph.edge.sources.retrieval_source.{context}.infores"
         if not is_curie(identifier):
             self.report(
                 code=f"{code_prefix}.not_curie",
                 identifier=identifier,
                 edge_id=edge_id
             )
-        elif not identifier.startswith("infores:"):
+            return False
+
+        if not identifier.startswith("infores:"):
             # not sure how absolute the need is for this to be an Infores. We'll be lenient for now?
             self.report(
                 code=f"{code_prefix}.invalid",
                 identifier=identifier,
                 edge_id=edge_id
             )
+            return False
+
         # TODO: infores is causing too much instability for now so support has been removed from BMT
         # TODO: reimplement using YAML version of infores catalog
-        # elif not self.bmt.get_infores_details(identifier):
+        # if not self.bmt.get_infores_details(identifier):
         #     # if this method returns 'None' then this is an unregistered infores?
         #     self.report(
         #         code=f"{code_prefix}.unknown",
         #         identifier=identifier,
         #         edge_id=edge_id
         #     )
+        #     return False
 
-    def validate_sources(self, edge_id: str, edge: Dict):
+        # Infores validates properly here
+        return True
+
+    def validate_sources(self, edge_id: str, edge: Dict) -> Optional[str]:
         """
         Validate (TRAPI 1.4.0-beta ++) Edge.sources provenance.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
-        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        :return: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         """
-        # we ought not to have to test for the absence of the 'sources' tag
+        sources: Dict[str, List[str]] = dict()
+        # we ought not to have to test for the absence of the "sources" tag
         # if general TRAPI schema validation is run, since it will catch such missing data
         # however, this method may be directly run on invalid TRAPI data, so...
-        if 'sources' not in edge:
+        if "sources" not in edge:
             self.report(code="error.knowledge_graph.edge.sources.missing", identifier=edge_id)
-        elif not edge['sources']:
-            # Cardinality of 'sources' array is also validated by the TRAPI schema
+        elif not edge["sources"]:
+            # Cardinality of "sources" array is also validated by the TRAPI schema
             # but for the same reasons noted above, we check again here.
             self.report(code="error.knowledge_graph.edge.sources.empty", identifier=edge_id)
-        elif not isinstance(edge['sources'], List):
+        elif not isinstance(edge["sources"], List):
             self.report(code="error.knowledge_graph.edge.sources.not_array", identifier=edge_id)
         else:
-            edge_sources = edge['sources']
+            # by this point, we have verified that we have a "sources" list of
+            # at least one (hopefully properly formatted RetrievalSource) entry
+            edge_sources = edge["sources"]
 
-            # The RetrievalSource items in the 'sources' array is also partially validated insofar as JSONSchema can
+            # The RetrievalSource items in the "sources" array is also partially validated insofar as JSONSchema can
             # validate based on the TRAPI schema; however, some kinds of validation are either not deterministic from
             # the schema. The remainder of this method validates an initial basic 'semantic' subset of RetrievalSource
             # content for which the validation is both easy and deemed generally useful. This includes detection of
             # anticipated Edge provenance roles (i.e. mandatory 'primary' and tests against expected provenance tags)
+            # and the capture of the 'provenance audit trail' of sources, for reporting purposes
 
             # Method caller associated Edge sources to be checked
 
             ara_source: Optional[str]
             kp_source: Optional[str]
             kp_source_type: Optional[str]
-            ara_source, kp_source, kp_source_type = self.get_target_sources()
+            ara_source, kp_source, kp_source_type = self.get_target_provenance()
 
             # Expecting ARA and KP 'aggregator_knowledge_source' attributes?
             found_ara_knowledge_source = False
             found_kp_knowledge_source = False
 
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
@@ -822,95 +922,192 @@
                         code="error.knowledge_graph.edge.sources.retrieval_source.resource_role.empty",
                         identifier=edge_id
                     )
                     continue
 
                 resource_id: str = retrieval_source["resource_id"]
                 resource_role: str = retrieval_source["resource_role"]
-                self. validate_infores(context="resource_id", edge_id=edge_id, identifier=resource_id)
-                if resource_id == ara_source:
-                    found_ara_knowledge_source = True
-                if resource_id == kp_source and resource_role == kp_source_type:
-                    found_kp_knowledge_source = True
-
-                # ... even if the resource_id fails aspects of validation, we'll keep going...
-
-                # 2. 'resource_role': will have already been TRAPI validated, but is at least one
-                #    (but only one?) of 'RetrievalSource' entries the mandatory 'primary'?
-                if resource_id and resource_role == "primary_knowledge_source":
-                    # the cardinality of this will be checked below...
-                    found_primary_knowledge_source.append(resource_id)
-
-                # 3. If provided (Optional), are all 'upstream_resource_ids' well-formed Infores CURIES
-                #    and may include some expected Infores entries (from target sources noted above)?
-                if "upstream_resource_ids" in retrieval_source:
-                    upstream_resource_ids: Optional[List[str]] = retrieval_source["upstream_resource_ids"]
-                    # Note: the TRAPI schema doesn't currently tag this field as nullable, so we check
-                    if upstream_resource_ids:
-                        for identifier in upstream_resource_ids:
-                            self.validate_infores(
-                                context="upstream_resource_ids",
-                                edge_id=edge_id,
-                                identifier=identifier
-                            )
-                            if resource_id == ara_source:
-                                found_ara_knowledge_source = True
+                if not self. validate_infores(
+                        context="resource_id",
+                        edge_id=edge_id,
+                        identifier=resource_id
+                ):
+                    # if not validated, we should probably not
+                    # continue using the 'resource_id' from here
+                    continue
+
+                else:
+                    # start capturing the "sources" audit trail here
+                    if resource_id not in sources:
+                        sources[resource_id] = list()
+
+                    if resource_id == ara_source:
+                        found_ara_knowledge_source = True
+
+                    if resource_id == kp_source and resource_role == kp_source_type:
+                        found_kp_knowledge_source = True
+
+                    # ... even if the resource_id fails aspects of validation, we'll keep going...
+
+                    # 2. 'resource_role': will have already been TRAPI validated, but is at least one
+                    #    (but only one?) of 'RetrievalSource' entries the mandatory 'primary'?
+                    if resource_id and resource_role == "primary_knowledge_source":
+                        # the cardinality of this will be checked below...
+                        found_primary_knowledge_source.append(resource_id)
+
+                    # 3. If provided (Optional), are all 'upstream_resource_ids' well-formed Infores CURIES
+                    #    and may include some expected Infores entries (from target sources noted above)?
+
+                    if "upstream_resource_ids" in retrieval_source:
+                        upstream_resource_ids: Optional[List[str]] = retrieval_source["upstream_resource_ids"]
+                        # Note: the TRAPI schema doesn't currently tag this field as nullable, so we check
+                        if upstream_resource_ids:
+                            for identifier in upstream_resource_ids:
+
+                                if not self.validate_infores(
+                                    context="upstream_resource_ids",
+                                    edge_id=edge_id,
+                                    identifier=identifier
+                                ):
+                                    # if not validated, we should probably not
+                                    # continue using the 'identifier' from here
+                                    continue
 
-                            # we don't worry about kp_source_type here since it is
-                            # not directly annotated with the upstream_resource_ids
-                            if resource_id == kp_source:
-                                found_kp_knowledge_source = True
-
-                # 4. If provided (Optional), we *could* check the optional 'source_record_urls'
-                #    if they are all resolvable URLs (but maybe we do not attempt this for now...)
-                #
-                # if "source_record_urls" in retrieval_source:
-                #     source_record_urls: Optional[List[str]] = retrieval_source["source_record_urls"]
+                                else:
+                                    if identifier == ara_source:
+                                        found_ara_knowledge_source = True
+
+                                    # we don't worry about kp_source_type here since it is
+                                    # not directly annotated with the upstream_resource_ids
+                                    if identifier == kp_source:
+                                        found_kp_knowledge_source = True
+
+                                    # Capture the upstream 'upstream_resource_id' source here
+                                    sources[resource_id].append(identifier)
+
+                    # 4. If provided (Optional), we *could* check the optional 'source_record_urls'
+                    #    if they are all resolvable URLs (but maybe we do not attempt this for now...)
+                    #
+                    # if "source_record_urls" in retrieval_source:
+                    #     source_record_urls: Optional[List[str]] = retrieval_source["source_record_urls"]
+
+            # After all the "sources" RetrievalSource entries have been scanned,
+            # then perform a complete validation check for complete expected provenance.
+            source_trail: Optional[str] = self.build_source_trail(sources) if sources else None
 
-            # TODO: After all the 'sources' RetrievalSource entries have been scanned, then
-            #       perform a complete validation check for complete expected provenance.
             self.validate_provenance(
                 edge_id,
                 ara_source, found_ara_knowledge_source,
                 kp_source, found_kp_knowledge_source, kp_source_type,
-                found_primary_knowledge_source
+                found_primary_knowledge_source,
+                source_trail=source_trail
             )
 
-    def validate_predicate(self, edge_id: str, predicate: str):
+            return source_trail  # may be empty if required RetrievalSource 'sources' entries are missing
+
+    def validate_predicate(self, edge_id: str, predicate: str, source_trail: Optional[str] = None):
         """
-        :param edge_id: identifier of the edge whose predicate is being validated
-        :param predicate: putative Biolink Model predicate to be validated
+        :param edge_id: str, identifier of the edge whose predicate is being validated
+        :param predicate: str, putative Biolink Model predicate to be validated
+        :param source_trail: str, putative Biolink Model predicate to be validated
         :return:
         """
         graph_type_context: str = self.graph_type.name.lower()
         if graph_type_context != "input_edge":
             graph_type_context += ".edge"
         context: str = f"{graph_type_context}.predicate"
 
         # Validate the putative predicate as *not* being abstract, deprecated or a mixin
         biolink_class = self.validate_element_status(
             context=context,
             identifier=predicate,
-            edge_id=edge_id
+            edge_id=edge_id,
+            source_trail=source_trail
         )
         if biolink_class:
             if not self.bmt.is_predicate(predicate):
                 self.report(
                     code=f"error.{context}.invalid",
+                    source_trail=source_trail,
                     identifier=predicate,
                     edge_id=edge_id
                 )
             elif self.minimum_required_biolink_version("2.2.0") and \
                     not self.bmt.is_translator_canonical_predicate(predicate):
                 self.report(
                     code=f"warning.{context}.non_canonical",
+                    source_trail=source_trail,
                     identifier=predicate,
                     edge_id=edge_id
                 )
 
+    @staticmethod
+    def build_source_trail(sources: Optional[Dict[str, List[str]]]) -> Optional[str]:
+        """
+        Returns a 'source_trail' path from 'primary_knowledge_source' upwards. The "sources" should
+        have at least one and only one primary knowledge source (with an empty 'upstream_resource_ids' list).
+
+        :param sources: Optional[Dict[str, List[str]]], catalog of upstream knowledge sources indexed by resource_id's
+        :return: Optional[str] source ("audit") trail ('path') from primary to topmost wrapper knowledge source infores
+        """
+        if sources:
+            # Example "sources"...:
+            # {
+            #     "infores:chebi": [],
+            #     "infores:biothings-explorer": ["infores:chebi"],
+            #     "infores:molepro": ["infores:biothings-explorer"],
+            #     "infores:arax": ["infores:molepro"]
+            # }
+            #
+            source_paths: Dict = {
+                upstream_resource_ids[0] if upstream_resource_ids else "primary": downstream_id
+                for downstream_id, upstream_resource_ids in sources.items()
+            }
+
+            # ...reversed and flattened into "source_paths"...:
+            # {
+            #     "infores:biothings-explorer": "infores:molepro",
+            #     "infores:chebi": "infores:biothings-explorer",
+            #     "infores:molepro": "infores:arax",
+            #     "primary": "infores:chebi"
+            # }
+            current_resource = source_paths["primary"] if "primary" in source_paths else None
+            # current_resource == "infores:chebi"  # could be 'None' if no primary resources available?
+            source_trail: Optional[str] = None
+            if current_resource is not None:
+                source_trail = current_resource
+                while True:
+                    if current_resource in source_paths:
+                        current_resource = source_paths[current_resource]
+                        source_trail += f" -> {current_resource}"
+                    else:
+                        break  # this should 'break' at "infores:arax"
+            else:
+                # Missing the primary resource? With a bit more effort
+                # Infer the path from the other direction?
+                reverse_source_path: Dict = dict()
+                for upstream_id, downstream_id in source_paths.items():
+                    if downstream_id not in source_paths:
+                        source_trail = f"{upstream_id} -> {downstream_id}"
+                        current_resource = upstream_id
+                    else:
+                        reverse_source_path[downstream_id] = upstream_id
+
+                while True:
+                    if current_resource in reverse_source_path:
+                        current_resource = reverse_source_path[current_resource]
+                        source_trail = f"{current_resource} -> " + source_trail
+                    else:
+                        break
+
+            # "infores:chebi -> infores:biothings-explorer -> infores:molepro -> infores:arax"
+            return source_trail
+        else:
+            return None
+
     def validate_graph_edge(self, edge: Dict):
         """
         Validate slot properties of a relationship ('biolink:Association') edge.
 
         :param edge: dictionary of slot properties of the edge.
         :type edge: dict[str, str]
         """
@@ -929,75 +1126,130 @@
 
         object_id = edge['object'] if 'object' in edge else None
 
         edge_id = f"{str(subject_id)}--{edge_label}->{str(object_id)}"
 
         context: str = self.graph_type.name.lower()
 
+        # 7 July 2023: since edge provenance annotation is somewhat
+        # orthogonal to the contents of the edge itself, we move the
+        # attribute validation ahead of Edge semantic validation,
+        # which allows us to capture the Edge provenance audit trail
+        # for reasoner-validator issue#86 - edge sources reporting.
+        #
+        # Validate edge attributes (or attribute_constraints)
+        # and (Biolink) edge qualifiers (or qualifier_constraints)
+        source_trail: Optional[str] = None
+        if self.graph_type is TRAPIGraphType.Knowledge_Graph:
+
+            # Edge "qualifiers" field is only recorded as an
+            # Edge property, from TRAPI 1.3.0-beta onwards
+            if self.minimum_required_trapi_version("1.3.0-beta"):
+                self.validate_qualifiers(edge_id=edge_id, edge=edge)
+
+            # Edge provenance "sources" field is only recorded
+            # as an Edge property, from TRAPI 1.4.0-beta onwards
+            if self.minimum_required_trapi_version("1.4.0-beta"):
+                # For TRAPI 1.4.0, the 'source_trail' is parsed in by 'validate_sources'...
+                source_trail = self.validate_sources(edge_id=edge_id, edge=edge)
+
+                # ...then the 'validate_sources' computed 'source_trail' is communicated
+                #    to 'validate_attributes' for use in attribute validation reporting
+                self.validate_attributes(edge_id=edge_id, edge=edge, source_trail=source_trail)
+            else:
+                # For TRAPI 1.3.0, the 'sources' are discovered internally by 'validate_attributes'
+                # and the resulting source_trail returned, for further external reporting purposes
+                source_trail = self.validate_attributes(edge_id=edge_id, edge=edge)
+        else:
+            self.validate_attribute_constraints(edge_id=edge_id, edge=edge)
+
+            # Edge "qualifiers" field is only recorded as an
+            # Edge property, from TRAPI 1.3.0-beta onwards
+            # We don't care about 'source_trail' here, for the Query Graph edges
+            if self.minimum_required_trapi_version("1.3.0-beta"):
+                self.validate_qualifier_constraints(edge_id=edge_id, edge=edge)
+
         # Validate Subject node
         if not subject_id:
-            self.report(code=f"error.{context}.edge.subject.missing", identifier=edge_id)
+            self.report(
+                code=f"error.{context}.edge.subject.missing",
+                source_trail=source_trail,
+                identifier=edge_id
+            )
 
         elif subject_id not in self.nodes:
             self.report(
                 code=f"error.{context}.edge.subject.missing_from_nodes",
+                source_trail=source_trail,
                 identifier=subject_id,
                 edge_id=edge_id
             )
 
         # Validate Predicates
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
             if not predicate:
                 self.report(
                     code="error.knowledge_graph.edge.predicate.missing",
+                    source_trail=source_trail,
                     context=self.graph_type.value,
                     identifier=edge_id
                 )
             elif self.validate_biolink():
-                self.validate_predicate(edge_id=edge_id, predicate=predicate)
+                self.validate_predicate(
+                    edge_id=edge_id,
+                    predicate=predicate,
+                    source_trail=source_trail
+                )
 
         else:  # is a Query Graph...
             if predicates is None:
                 # Query Graphs can have a missing or null predicates slot
                 pass
             elif not isinstance(predicates, List):
-                self.report(code="error.query_graph.edge.predicate.not_array", identifier=edge_id)
+                self.report(
+                    code="error.query_graph.edge.predicate.not_array",
+                    source_trail=source_trail,
+                    identifier=edge_id
+                )
             elif len(predicates) == 0:
-                self.report(code="error.query_graph.edge.predicate.empty_array", identifier=edge_id)
+                self.report(
+                    code="error.query_graph.edge.predicate.empty_array",
+                    source_trail=source_trail,
+                    identifier=edge_id
+                )
             elif self.validate_biolink():
                 # Should now be a non-empty list of CURIES
                 # which should validate as Biolink Predicates
                 for predicate in predicates:
                     if not predicate:
                         continue  # sanity check
-                    self.validate_predicate(edge_id=edge_id, predicate=predicate)
+                    self.validate_predicate(
+                        edge_id=edge_id,
+                        predicate=predicate,
+                        source_trail=source_trail
+                    )
 
         # Validate Object Node
         if not object_id:
-            self.report(code=f"error.{context}.edge.object.missing", identifier=edge_id)
+            self.report(
+                code=f"error.{context}.edge.object.missing",
+                source_trail=source_trail,
+                identifier=edge_id
+            )
         elif object_id not in self.nodes:
             self.report(
                 code=f"error.{context}.edge.object.missing_from_nodes",
+                source_trail=source_trail,
                 identifier=object_id,
                 edge_id=edge_id
             )
 
-        # Validate edge attributes (or attribute_constraints)
-        # and (Biolink 3) edge qualifiers (or qualifier_constraints)
-        if self.graph_type is TRAPIGraphType.Knowledge_Graph:
-            self.validate_attributes(edge_id=edge_id, edge=edge)
-            self.validate_qualifiers(edge_id=edge_id, edge=edge)
-
-            # Edge provenance 'sources' field is only recorded in
-            # Edge attributes, from TRAPI 1.4.0-beta onwards
-            if self.minimum_required_trapi_version("1.4.0-beta"):
-                self.validate_sources(edge_id=edge_id, edge=edge)
-        else:
-            self.validate_attribute_constraints(edge_id=edge_id, edge=edge)
-            self.validate_qualifier_constraints(edge_id=edge_id, edge=edge)
+    # TODO: 11-July-2023: Certain specific 'abstract' or 'mixin' categories used in Knowledge Graphs
+    #                     are being validated for now as 'warnings', for short term validation purposes
+    CATEGORY_INCLUSIONS = ["biolink:BiologicalEntity"]
 
     def validate_category(
             self,
             context: str,
             node_id: Optional[str],
             category: Optional[str]
     ) -> ClassDefinition:
@@ -1015,22 +1267,31 @@
 
         :return: category as a ClassDefinition, only returned if 'concrete'; None otherwise.
         """
         biolink_class: Optional[ClassDefinition] = None
         if category:
             biolink_class = self.bmt.get_element(category)
             if biolink_class:
+                # 'category' is known to Biolink... good start!
                 if biolink_class.deprecated:
                     self.report(
                         code=f"warning.{context}.node.category.deprecated",
                         identifier=category,
                         node_id=node_id
                     )
                 if biolink_class.abstract or self.bmt.is_mixin(category):
-                    biolink_class = None
+                    # See above note about CATEGORY_INCLUSIONS
+                    if context == "knowledge_graph" and category in self.CATEGORY_INCLUSIONS:
+                        self.report(
+                            code=f"warning.{context}.node.category.abstract_or_mixin",
+                            identifier=category,
+                            node_id=node_id
+                        )
+                    else:
+                        biolink_class = None
                 elif not self.bmt.is_category(category):
                     self.report(
                         code=f"error.{context}.node.category.not_a_category",
                         identifier=category,
                         node_id=node_id
                     )
                     biolink_class = None
@@ -1257,30 +1518,30 @@
     return validator
 
 
 def check_biolink_model_compliance_of_knowledge_graph(
     graph: Dict,
     trapi_version: Optional[str] = None,
     biolink_version: Optional[str] = None,
-    sources: Optional[Dict] = None,
+    target_provenance: Optional[Dict] = None,
     strict_validation: Optional[bool] = None
 ) -> BiolinkValidator:
     """
     Strict validation of a TRAPI-schema compliant Message Knowledge Graph against a designated Biolink Model release.
 
     :param graph: knowledge graph to be validated.
     :type graph: Dict
     :param trapi_version: TRAPI schema (SemVer) release against which the knowledge graph is to be
                             validated (Default: if None, use the latest available version).
     :type trapi_version: Optional[str] = None
     :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
                             validated (Default: if None, use the Biolink Model Toolkit default version).
     :type biolink_version: Optional[str] = None
-    :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
-    :type sources: Dict
+    :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance validation
+    :type target_provenance: Dict
     :param strict_validation: if True, abstract and mixin elements validate as 'error'; False, issue 'info' message.
     :type strict_validation: Optional[bool] = None; defaults to 'True' if not set
 
     :returns: Biolink Model validator cataloging validation messages (maybe empty)
     :rtype: BiolinkValidator
     """
     # One typically will want stringent validation for Knowledge Graphs; however,
@@ -1290,12 +1551,12 @@
         # abstract and mixins in TRAPI Responses (and Requests)
         strict_validation = True
 
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         trapi_version=trapi_version,
         biolink_version=biolink_version,
-        sources=sources,
+        target_provenance=target_provenance,
         strict_validation=strict_validation
     )
     validator.check_biolink_model_compliance(graph)
     return validator
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.0/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -698,14 +698,20 @@
       category:
         deprecated:
           $message: "Node has deprecated category"
           $context:
             - node_id
             - identifier
           $description: "Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?"
+        abstract_or_mixin:
+          $message: "Node has a abstract or mixin category"
+          $context:
+            - node_id
+            - identifier
+          $description: "Node category is abstract or a mixin in the current model. Please consider selecting a more specific, concrete Biolink Model category?"
       id:
         unmapped_prefix:
           $message: "Node identifier found unmapped to target categories for node"
           $context:
             - identifier
             - categories
           $description: "Node CURIE identifier namespace not found among any 'id_prefix' slot values in specified categories in the validating Biolink Model version?"
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/report.py` & `reasoner_validator-3.7.0/reasoner_validator/report.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from typing import Optional, Dict, List
 from sys import stdout
 from io import StringIO
 import copy
 
 from json import dumps, JSONEncoder
 
+from reasoner_validator.message import (
+    MESSAGE_CATALOG,
+    MESSAGE_PARTITION,
+    SCOPED_MESSAGES,
+    IDENTIFIED_MESSAGES,
+    MESSAGE_PARAMETERS
+)
 from reasoner_validator.validation_codes import CodeDictionary
 from reasoner_validator.versioning import SemVer, SemVerError, get_latest_version
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -48,85 +55,35 @@
     }
 
     def __init__(
             self,
             prefix: Optional[str] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
-            sources: Optional[Dict] = None,
             strict_validation: bool = False
     ):
         """
         :param prefix: named context of the Validator, used as a prefix in validation messages.
         :type prefix: str
         :param trapi_version: version of component against which to validate the message.
                               Could be a TRAPI release SemVer or a Git branch identifier.
         :type trapi_version: Optional[str], target version of TRAPI upon which the validation is attempted
         :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
                                 validated (Default: if None, use the Biolink Model Toolkit default version).
         :type biolink_version: Optional[str] = None
-        :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
-        :type sources: Dict
         :param strict_validation: if True, abstract and mixin elements validate as 'error';
                                   if None or False, just issue a 'warning'
         :type strict_validation: Optional[bool] = None
         """
         self.prefix: str = prefix if prefix else ""
         self.trapi_version = get_latest_version(trapi_version) \
             if trapi_version else get_latest_version(self.DEFAULT_TRAPI_VERSION)
         self.biolink_version = biolink_version
-        self.sources: Optional[Dict] = sources
         self.strict_validation: Optional[bool] = strict_validation
-        #
-        # self.messages have dictionary structure something like the following:
-        #
-        # self.messages = {
-        #     "information": {
-        #         "info.input_edge.node.category.abstract": [
-        #             {  # parameters of a distinct message
-        #               "name": <name-parameter>
-        #             },
-        #             { <parameters of second reported message...> },
-        #             etc...
-        #         ],
-        #         # codes without parameters can just be set to an empty list?
-        #         "info.compliant.message": []
-        #
-        #     },
-        #     "warnings":  {
-        #       ...<similar to information data structure above>
-        #     },
-        #     "errors": {
-        #       ...<similar to information data structure above>
-        #     },
-        #     "critical": {
-        #       ...<similar to information data structure above>
-        #     }
-        # }
-        #
-        self.messages: Dict[
-            str,  # message type (critical/errors/warnings/information)
-            Dict[
-                str,  # message 'code' as indexing key
-                # Dictionary of 'identifier' indexed messages with parameters
-                # (Maybe None, if code doesn't have any additional parameters)
-                Optional[
-                    Dict[
-                        str,  # key is the message-unique template 'identifier' value of parameterized messages
-                        Optional[
-                            List[
-                                # Each reported message adds a dictionary of such parameters
-                                # to the list here; these are not guaranteed to be unique
-                                Dict[str, str]
-                            ]
-                        ]
-                    ]
-                ]
-            ]
-        ] = {
+        self.messages: MESSAGE_CATALOG = {
             "critical": dict(),
             "errors": dict(),
             "warnings": dict(),
             "information": dict()
         }
 
     def get_trapi_version(self) -> str:
@@ -154,18 +111,17 @@
         :rtype biolink_version: str
         """
         return self.biolink_version
 
     def validate_biolink(self) -> bool:
         """
         Predicate to check if the Biolink (version) is
-        tagged to 'suppress" compliance validation.
+        tagged to 'suppress' compliance validation.
 
-        :return: returns 'True' if Biolink Validation is expected.
-        :rtype bool
+        :return: bool, returns 'True' if Biolink Validation is expected.
         """
         return self.biolink_version is None or self.biolink_version.lower() != "suppress"
 
     def is_strict_validation(self) -> bool:
         """
         :return: bool, value of validation strictness set in the ValidationReporter.
         """
@@ -247,123 +203,122 @@
         if message_type in ['info', 'warning', 'error', 'critical']:
             return message_type
         else:
             raise NotImplementedError(
                 f"ValidationReport.get_message_type(): {code} is unknown code type: {message_type}"
             )
 
-    def report(self, code: str, **message):
+    def report(self, code: str, source_trail: Optional[str] = None, **message):
         """
-        Capture a single validation message, as per specified 'code' (with any code-specific contextural parameters)
-        :param code: 
-        :param message: named parameters representing extra (str-formatted) context for the given code message
+        Capture a single validation message, as per specified 'code' (with any code-specific contextural parameters).
+
+        :param code: str, dot delimited validation path code
+        :param source_trail, Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
+                             Defaults to "global" if not specified.
+        :param message: **Dict, named parameters representing extra (str-formatted) context for the given code message
         :return: None (internally record the validation message)
         """
         # Sanity check: that the given code has been registered in the codes.yaml file
         assert CodeDictionary.get_code_entry(code) is not None, f"ValidationReporter.report: unknown code '{code}'"
 
         message_type_id = self.get_message_type(code)
         message_type = self._message_type_name[message_type_id]
         if code not in self.messages[message_type]:
-            self.messages[message_type][code] = None
-        if message:
-            # Should have at least an "identifier" parameter
-            if self.messages[message_type][code] is None:
-                self.messages[message_type][code] = dict()
+            self.messages[message_type][code] = dict()
+
+        # Set current scope of validation message
+        if source_trail is not None and source_trail not in self.messages[message_type][code]:
+            scope = self.messages[message_type][code][source_trail] = dict()
+        else:
+            scope = self.messages[message_type][code]["global"] = dict()
 
+        if message:
             # If a message has any parameters, then one of them is
             # expected to be a message indexing identifier
             if "identifier" in message:
                 message_identifier = message.pop("identifier")
                 if not message:
                     # the message_identifier was the only parameter to keep track of...
-                    self.messages[message_type][code][message_identifier] = None
+                    scope[message_identifier] = None
                 else:
                     # keep track of additional parameters in a list of dictionaries
                     # (may have additional, currently unavoidable, content duplication?)
-                    if message_identifier not in self.messages[message_type][code] or \
-                            self.messages[message_type][code][message_identifier] is None:
-                        self.messages[message_type][code][message_identifier] = list()
+                    if message_identifier not in scope or scope[message_identifier] is None:
+                        scope[message_identifier] = list()
 
-                    self.messages[message_type][code][message_identifier].append(message)
+                    scope[message_identifier].append(message)
 
         # else: additional parameters are None
 
-    def add_messages(self, new_messages: Dict[
-            str,  # message type (info/warning/error/critical)
-            Dict[
-                str,  # message 'code' as indexing key
-
-                # List of Dictionaries of parameters
-                # (Maybe None, if specific code doesn't
-                # have additional associated parameters)
-                Optional[Dict[str, Optional[List[Dict[str, str]]]]]
-            ]
-    ]):
+    def add_messages(self, new_messages: MESSAGE_CATALOG):
         """
         Batch addition of a dictionary of messages to a ValidationReporter instance.
         :param new_messages: Dict[str, Dict], with key one of "information", "warnings", "errors" or "critical",
                               with 'code' keyed dictionaries of (structured) message parameters.
         """
         for message_type in self.messages:   # 'info', 'warning', 'error', 'critical'
             if message_type in new_messages:
                 message_type_contents = new_messages[message_type]
-                for code, content in message_type_contents.items():   # codes.yaml message codes
+                for code, details in message_type_contents.items():   # codes.yaml message codes
                     if code not in self.messages[message_type]:
-                        self.messages[message_type][code] = None
-                    if content:
-                        # content is of type Dict[str, Optional[List[Dict[str, str]]]]
-                        # where dictionary keys are a set of message discriminating 'identifier'
-                        identifier: str
-                        parameters: Optional[List[Dict[str, str]]]
-                        for identifier, parameters in content.items():
-                            if self.messages[message_type][code] is None:
-                                self.messages[message_type][code] = dict()
-                            if parameters:
-                                # additional parameters seen?
-                                if identifier not in self.messages[message_type][code] or \
-                                        self.messages[message_type][code][identifier] is None:
-                                    self.messages[message_type][code][identifier] = list()
-
-                                self.messages[message_type][code][identifier].extend(parameters)
-                            else:
-                                # the message 'identifier' is the only parameter
-                                self.messages[message_type][code][identifier] = None
+                        self.messages[message_type][code] = dict()
+
+                    # 'source' scope is 'global' or a source trail path string, from primary to topmost aggregator
+                    for source, content in details.items():
+                        scope = self.messages[message_type][code][source] = dict()
+                        if content:
+                            # content is of type Dict[str, Optional[List[Dict[str, str]]]]
+                            # where dictionary keys are a set of message discriminating 'identifier'
+                            identifier: str
+                            parameters: Optional[List[Dict[str, str]]]
+                            for identifier, parameters in content.items():
+                                if self.messages[message_type][code] is None:
+                                    self.messages[message_type][code] = dict()
+                                if parameters:
+                                    # additional parameters seen?
+                                    if identifier not in self.messages[message_type][code] or \
+                                            scope[identifier] is None:
+                                        scope[identifier] = list()
+
+                                    scope[identifier].extend(parameters)
+                                else:
+                                    # the message 'identifier' is the only parameter
+                                    scope[identifier] = None
 
-    def get_messages(self) -> Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]]:
+    def get_messages(self) -> MESSAGE_CATALOG:
         """
         Get copy of all messages as a Python data structure.
         :return: Dict (copy) of all validation messages in the ValidationReporter.
         """
         return copy.deepcopy(self.messages)
 
-    def get_info(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
+    def get_info(self) -> MESSAGE_PARTITION:
         """
-        Get copy of all recorded information messages.
+        Get copy of all recorded 'information' messages.
         :return: List, copy of all information messages.
         """
         return copy.deepcopy(self.messages["information"])
 
-    def get_warnings(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
+    def get_warnings(self) -> MESSAGE_PARTITION:
         """
-        Get copy of all recorded warning messages.
+        Get copy of all recorded 'warning' messages.
         :return: List, copy of all warning messages.
         """
         return copy.deepcopy(self.messages["warnings"])
 
-    def get_errors(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
+    def get_errors(self) -> MESSAGE_PARTITION:
         """
-        Get copy of all recorded error messages.
+        Get copy of all recorded 'error' messages.
         :return: List, copy of all error messages.
         """
         return copy.deepcopy(self.messages["errors"])
 
-    def get_critical(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
+    def get_critical(self) -> MESSAGE_PARTITION:
         """
-        Get copy of all recorded critical error messages.
+        Get copy of all recorded 'critical' error messages.
         :return: List, copy of all critical error messages.
         """
         return copy.deepcopy(self.messages["critical"])
 
     ############################
     # General Instance methods #
     ############################
@@ -432,28 +387,34 @@
         #         "trapi_version": "1.3",
         #         "biolink_version": "3.0.2",
         #         "messages": {
         #             "information": [],
         #             "warnings": [
         #                 {
         #                     "warning.predicate.non_canonical": {
-        #                         "biolink:participates_in": {
-        #                               "edge_id": "a--['biolink:participates_in']->b"
+        #                         "infores:molepro -> infores:arax": {  # local source scope of error
+        #                             "biolink:participates_in": {
+        #                                   "edge_id": "a--['biolink:participates_in']->b"
+        #                             }
         #                         }
         #                     }
         #                 }
         #             ],
         #             "errors": [
         #                 {
-        #                     "error.knowledge_graph.empty_nodes": None
+        #                     "error.knowledge_graph.empty_nodes": {
+        #                         "global": None  # scope of error
+        #                     }
         #                 }
         #             ],
         #             "critical": [
         #                 {
-        #                     "critical.trapi.validation": None
+        #                     "critical.trapi.validation": {
+        #                         "global": None   # scope of critical error
+        #                     }
         #                 }
         #             ]
         #         }
         #     }
         #
         # where 'tag' == 'messages' and we have a non-empty "errors" set of messages
         #
@@ -505,127 +466,160 @@
             if not compact_format:
                 print(f"\n\033[4m{title}\033[0m", file=file)
                 print(file=file)
             else:
                 # compact also ignores underlining
                 print(title, file=file)
 
-        message_type: str
-        coded_messages: Dict
-        # Top level partition of messages into 'critical', 'error', 'warning' or 'info'
-        for message_type, coded_messages in self.messages.items():
-
-            # if there are coded validation messages for a
-            # given message type: 'critical', 'error', 'warning' or 'info' ...
-            if coded_messages:
-
-                # ... then iterate through them and print them out
-
-                if not compact_format:
-                    print(f"\033[4m{message_type.capitalize()}\033[0m", file=file)
-                    print(file=file)
-                else:
-                    # compact also ignores underlining
-                    print(f"\n{message_type.capitalize()}:", file=file)
+        print(
+            "Validation against TRAPI " +
+            f"'{str(self.trapi_version if self.trapi_version is not None else 'Default')}' version " +
+            "and Biolink Model " +
+            f"'{str(self.biolink_version if self.biolink_version is not None else 'Default')}' version.",
+            file=file
+        )
+
+        if self.has_messages():
+
+            # self.messages is a MESSAGE_CATALOG where MESSAGE_CATALOG is Dict[<message type>, MESSAGE_PARTITION]
+            # <message type> is the top level partition of messages into 'critical', 'error', 'warning' or 'info'
+            message_type: str
+            coded_messages: MESSAGE_PARTITION
+            for message_type, coded_messages in self.messages.items():
+
+                # if there are coded validation messages for a
+                # given message type: 'critical', 'error', 'warning' or 'info' ...
+                if coded_messages:
+
+                    # ... then iterate through them and print them out
 
-                code: str  # validation codes
-                messages_by_code:  Optional[
-                    Dict[
-                        str,      # Keys are 'identifiers' associated with the validation code
-                        Optional[
-                            List[
-                                Dict[str, str]
-                            ]
-                        ]
-                    ]
-                ]
-
-                # Grouping message outputs by validation codes
-                for code, messages_by_code in coded_messages.items():
-
-                    code_label: str = CodeDictionary.validation_code_tag(code)
-                    print(
-                        f"* {code_label}:\n"
-                        f"=> {CodeDictionary.get_message_template(code)}",
-                        file=file
-                    )
                     if not compact_format:
+                        print(f"\033[4m{message_type.capitalize()}\033[0m", file=file)
                         print(file=file)
-
-                    if messages_by_code is not None:
-
-                        # Codes with associated parameters should have
-                        # an embedded dictionary with 'identifier' keys
-
-                        ids_per_row: int = 0
-                        num_ids: int = len(messages_by_code.keys())
-                        more_ids: int = num_ids - id_rows if num_ids > id_rows else 0
-
-                        for identifier, messages in messages_by_code.items():
-
-                            if messages is None:
-
-                                # For codes solely with a list of 'identifier' parameters associated
-                                # with the message, just print the identifier
-
-                                print(f"\t# {identifier}", file=file)
-
-                                if not compact_format:
-                                    print(file=file)
-
-                            else:
-                                # Code has list of dictionaries of additional context for messages.
-                                # In this case, the keys of the dictionary are the 'identifier'
-                                # strings and the values are lists of dictionaries, each of which
-                                # contains the additional contextual parameters for one message
-                                print(f"\t# {identifier}:", file=file)
-
-                                first_message: bool = True
-                                messages_per_row: int = 0
-                                num_messages: int = len(messages)
-                                more_msgs: int = num_messages - msg_rows if num_messages > msg_rows else 0
-
-                                for parameters in messages:
-
-                                    if first_message:
-                                        tags = tuple(parameters.keys())
-                                        print(f"\t- {' | '.join(tags)}: ", file=file)
-                                        first_message = False
-
-                                    print(f"\t\t{' | '.join(parameters.values())}", file=file)
-
-                                    messages_per_row += 1
-                                    if msg_rows and messages_per_row >= msg_rows:
-                                        if more_msgs:
-                                            print(
-                                                f"\t{str(more_msgs)} more messages for identifier '{identifier}'...",
-                                                file=file
-                                            )
-                                        break
-
-                                if not compact_format:
-                                    print(file=file)
-
-                            ids_per_row += 1
-                            if id_rows and ids_per_row >= id_rows:
-                                if more_ids:
-                                    print(
-                                        f"{str(more_ids)} more identifiers for code '{code_label}'...",
-                                        file=file
-                                    )
-                                break
-
+                    else:
+                        # compact also ignores underlining
+                        print(f"\n{message_type.capitalize()}:", file=file)
+
+                    # 'coded_messages' is a MESSAGE_PARTITION where
+                    # MESSAGE_PARTITION is Dict[<validation code>, SCOPED_MESSAGES]
+
+                    # 'validation code' is the dot-delimited string
+                    # representation of the YAML path of the message codes.yaml
+                    code: str
+                    messages_by_code:  SCOPED_MESSAGES
+
+                    # Grouping message outputs by validation codes
+                    for code, messages_by_code in coded_messages.items():
+
+                        code_label: str = CodeDictionary.validation_code_tag(code)
+                        print(
+                            f"* {code_label}:\n"
+                            f"=> {CodeDictionary.get_message_template(code)}",
+                            file=file
+                        )
                         if not compact_format:
                             print(file=file)
 
-                    # else:
-                    #     For codes with associated non-parametric templates,
-                    #     just printing the template (done above) suffices
+                        # 'messages_by_code' is a SCOPED_MESSAGES where
+                        # SCOPED_MESSAGES is Dict[<scope>, Optional[IDENTIFIED_MESSAGES]]
 
-            # else: print nothing if a given message_type has no messages
+                        # <scope> is "global" or source trail path string
+                        scope: str
+                        messages_by_scope: Optional[IDENTIFIED_MESSAGES]
+                        for scope, messages_by_scope in messages_by_code.items():
+
+                            print(f"\t$ {scope}", file=file)
+
+                            # Codes with associated parameters should have
+                            # an embedded dictionary with 'identifier' keys
+
+                            ids_per_row: int = 0
+                            num_ids: int = len(messages_by_scope.keys())
+                            more_ids: int = num_ids - id_rows if num_ids > id_rows else 0
+
+                            # 'messages_by_scope' is Optional[IDENTIFIED_MESSAGES] where
+                            # 'IDENTIFIED_MESSAGES' is Dict[<identifier>, Optional[List[MESSAGE_PARAMETERS]]]
+
+                            # An entry of 'messages_by_scope' may be None if the given message code
+                            # has no additional parameters that distinguish instances of context (e.g. edge id?)
+                            # where the validation message occurs for the given identifier.
+
+                            # unique 'identifier' discriminator of the
+                            # (TRAPI or Biolink) token target of the validation
+                            identifier: str
+                            messages: Optional[List[MESSAGE_PARAMETERS]]
+                            for identifier, messages in messages_by_scope.items():
+
+                                if messages is None:
+
+                                    # For codes whose context of validation is solely discerned
+                                    # with their identifier, just print out the identifier
+
+                                    print(f"\t\t# {identifier}", file=file)
+
+                                    if not compact_format:
+                                        print(file=file)
+
+                                else:
+                                    # Since we have already checked if messages is None above, then we assume here that
+                                    # 'messages' is a List[MESSAGE_PARAMETERS] which records distinct additional context
+                                    # for a list of messages associated with a given code.
+                                    print(f"\t\t# {identifier}:", file=file)
+
+                                    first_message: bool = True
+                                    messages_per_row: int = 0
+                                    num_messages: int = len(messages)
+                                    more_msgs: int = num_messages - msg_rows if num_messages > msg_rows else 0
+
+                                    # 'messages' is an instance List[MESSAGE_PARAMETERS] where every entry of
+                                    # 'MESSAGE_PARAMETERS' is a dictionary of additional parameters documenting
+                                    # one specific instance of validation message related to the given identifier,
+                                    # where the keys are validation code specific (documented in codes.yaml)
+                                    parameters: MESSAGE_PARAMETERS
+                                    for parameters in messages:
+
+                                        if first_message:
+                                            tags = tuple(parameters.keys())
+                                            print(f"\t\t- {' | '.join(tags)}: ", file=file)
+                                            first_message = False
+
+                                        print(f"\t\t\t{' | '.join(parameters.values())}", file=file)
+
+                                        messages_per_row += 1
+                                        if msg_rows and messages_per_row >= msg_rows:
+                                            if more_msgs:
+                                                print(
+                                                    f"\t\t{str(more_msgs)} more messages " +
+                                                    f"for identifier '{identifier}'...",
+                                                    file=file
+                                                )
+                                            break
+
+                                    if not compact_format:
+                                        print(file=file)
+
+                                ids_per_row += 1
+                                if id_rows and ids_per_row >= id_rows:
+                                    if more_ids:
+                                        print(
+                                            f"{str(more_ids)} more identifiers for code '{code_label}'...",
+                                            file=file
+                                        )
+                                    break
+
+                            if not compact_format:
+                                print(file=file)
+
+                        # else:
+                        #     For codes with associated non-parametric templates,
+                        #     just printing the template (done above) suffices
+
+                # else: print nothing if a given message_type has no messages
+        else:
+            print(f"Hurray! No validation messages reported!", file=file)
 
     def dumps(
             self,
             id_rows: int = 0,
             msg_rows: int = 0,
             compact_format: bool = True
     ) -> str:
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.0/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.0/reasoner_validator/trapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,33 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 TRAPI_1_3_0_SEMVER = SemVer.from_string("v1.3.0")
 TRAPI_1_3_0: str = str(TRAPI_1_3_0_SEMVER)
 
-TRAPI_1_4_0_SEMVER = SemVer.from_string("v1.4.0")
-TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
-# patch version to fix 'auxiliary_graphs' model in 1.4.0
-TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
-TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
-
 TRAPI_1_4_0_BETA_SEMVER = SemVer.from_string("v1.4.0-beta")
 TRAPI_1_4_0_BETA = str(TRAPI_1_4_0_BETA_SEMVER)
 
 TRAPI_1_4_0_BETA2_SEMVER = SemVer.from_string("v1.4.0-beta2")
 TRAPI_1_4_0_BETA3_SEMVER = SemVer.from_string("v1.4.0-beta3")
 TRAPI_1_4_0_BETA4_SEMVER = SemVer.from_string("v1.4.0-beta4")
 
-LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_1_SEMVER
+TRAPI_1_4_0_SEMVER = SemVer.from_string("v1.4.0")
+TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
+
+# patch version to fix 'auxiliary_graphs' model in 1.4.0
+TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
+TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
+
+# patch version to fix '#components/schemas/AuxiliaryGraph' bug
+TRAPI_1_4_2_SEMVER = SemVer.from_string("v1.4.2")
+TRAPI_1_4_2: str = str(TRAPI_1_4_2_SEMVER)
+
+LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_2_SEMVER
 LATEST_TRAPI_RELEASE: str = str(LATEST_TRAPI_RELEASE_SEMVER)
 
 LATEST_TRAPI_MAJOR_RELEASE_SEMVER: SemVer = SemVer.from_string("v1.4", core_fields=['major', 'minor'])
 LATEST_TRAPI_MAJOR_RELEASE: str = str(LATEST_TRAPI_MAJOR_RELEASE_SEMVER)
 
 # For testing, set TRAPI API query POST timeouts to 10 minutes == 600 seconds
 DEFAULT_TRAPI_POST_TIMEOUT = 600.0
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.0/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.0/reasoner_validator/validation_codes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 from os.path import join, abspath, dirname
-from typing import Optional, Any, Dict, List, Tuple
+from typing import Optional, Any, Dict, List, Tuple, Union, NamedTuple
 
 from yaml import load, BaseLoader
 import logging
 
+from reasoner_validator.message import SCOPED_MESSAGES, IDENTIFIED_MESSAGES
+
 logger = logging.getLogger(__name__)
 
 DEFAULT_CODES_DOCUMENTATION_FILE = abspath(join(dirname(__file__), "..", "docs", "validation_codes_dictionary.md"))
 
 
 class CodeDictionary:
 
@@ -181,78 +183,80 @@
         tag: str = ' '.join(code_parts) if code_parts else path[-1].capitalize()
         return tag
 
     @classmethod
     def display(
             cls,
             code: str,  # code for specific validation message template
-            parameters: Optional[
-                Dict[
-                    str,  # message template 'identifier' key value
-                    Optional[
-                        List[
-                            Dict[str, str]  # dictionary of other template parameters (if present)
-                        ]
-                    ]
-                ]
-            ] = None,
+            messages: Optional[SCOPED_MESSAGES] = None,
             add_prefix: bool = False
-    ) -> List[str]:
+    ) -> Dict[str, List[str]]:
         """
         Generate one or more full messages from provided Validation Reporter code
         and associated parameters (if applicable).
 
-        :param code: str,  valid (dot delimited YAML key path) identified code,
-                           which should be registered in the project codes.yaml file.
-        :param parameters: Optional[Dict[str, Optional[List[Dict[str, str]]]]], collection of all
-                           message parameters dictionaries associated with list of messages of the given code,
-                           indexed by their unique 'identifier' template field (note: all messages with
-                           one or more template parameters are expected to have an 'identifier' parameter,
-                           the values for which corresponding to the keys of the dictionary. The value of those
-                           keys are either 'None' if the identifier is the only template parameter, or alternately,
-                           a list of dictionaries containing all the other expected parameters keys and their values
-                           for every distinct message).
+        :param code: str, valid (dot delimited YAML key path) identified code,
+                          which should be registered in the project codes.yaml file.
+        :param messages: Optional[SCOPED_MESSAGES], collection of scoped validation messages (Default: None)
+                         If this parameter specified as None, then it is actually taken to be {"global": None}
         :param add_prefix: bool, flag to prepend a prefix for the message type
                            (i.e. critical, error, warning, info) to displayed messages (default: False)
 
-        :return: List[str], list of decoded messages
+        :return: Dict[str, List[str]], scope-indexed dictionary of lists of decoded messages for a given code
         """
+        # All validation messages have a context, even if just "global" with no other distinguishing parameters.
+        if messages is None:
+            messages = {"global": None}
+
         value: Optional[Tuple[str, Dict[str, str]]] = cls.get_code_subtree(code, is_leaf=True)
         assert value, f"CodeDictionary.display(): unknown message code {code}"
 
         message_type = cls.get_message_type(code)
         message_type_prefix: str = f"{message_type.upper()} - " if add_prefix else ""
         context: str = cls.validation_code_tag(code) + ": " if add_prefix else ""
 
         template: str = cls.get_message_template(code)
+        message_set: Dict = dict()
 
-        if parameters:
-            # Message template parameterized with one or more sets of additional
-            # named message parameters, assumed to be referenced by the template
-            message_list: List = list()
-            for identifier in parameters.keys():
-                other_parameters: Optional[List[Dict[str, str]]] = parameters[identifier]
-                identifier_dict: Dict = {'identifier': identifier}
-                if other_parameters:
-                    # is a list of one or more dictionaries of additional parameters
-                    for another_parameter_dict in other_parameters:
-                        # make copies, to be safe...
-                        content: Dict = identifier_dict.copy()
-                        content.update(another_parameter_dict)
-                        message_list.append(
-                            f"{message_type_prefix}{context}{template.format(**content)}"
+        # 'messages' is an instance of 'SCOPED_MESSAGES' that is a Dict[<scope>, Optional[IDENTIFIED_MESSAGES]]
+        # where <scope> is either "global" or a "sources trail" string designating the audit trail from the
+        # 'primary_knowledge_source' up to topmost 'aggregator_knowledge_source' which reported the validation message,
+        # and the (Optional) 'IDENTIFIED_MESSAGES' are validation contexts possibly discriminated by a specific
+        # target entity (identifier) of the validation, plus any (Optional) additional parameters.
+        scope: str
+        parameters: Optional[IDENTIFIED_MESSAGES]
+        for scope, parameters in messages.items():
+            message_set[scope] = list()
+            if parameters:
+                # A non-null IDENTIFIED_MESSAGES entry is a dictionary of additional validation message parameters
+                # indexed by an identifier discriminating the (Biolink or TRAPI) target of the validation.
+                # A given validation code may or may not have additional parameters (as documented in the codes.yaml).
+                # If such parameters are expected, then they will be documented in a List[MESSAGE_PARAMETERS].
+                for identifier in parameters.keys():
+                    other_parameters: Optional[IDENTIFIED_MESSAGES] = parameters[identifier]
+                    identifier_dict: Dict = {'identifier': identifier}
+                    if other_parameters:
+                        # is a list of one or more dictionaries of additional parameters
+                        for another_parameter_dict in other_parameters:
+                            # make copies, to be safe...
+                            content: Dict = identifier_dict.copy()
+                            content.update(another_parameter_dict)
+                            message_set[scope].append(
+                                f"{message_type_prefix}{context}{template.format(**content)}"
+                            )
+                    else:
+                        message_set[scope].append(
+                            f"{message_type_prefix}{context}{template.format(**identifier_dict)}"
                         )
-                else:
-                    message_list.append(
-                        f"{message_type_prefix}{context}{template.format(**identifier_dict)}"
-                    )
-            return message_list
-        else:
-            # simple scalar message without parameterization?
-            return [f"{message_type_prefix}{context}{template}"]
+
+            else:
+                # simple scalar message without identification and parameterization?
+                message_set[scope].append(f"{message_type_prefix}{context}{template}")
+
+        return message_set
 
     @classmethod
     def _dump_code_markdown_entries(cls, root: str, code_subtree: Dict, markdown_file):
         for tag, value in code_subtree.items():
             if cls.MESSAGE not in value:
                 # Recurse down to leaf of tree
                 cls._dump_code_markdown_entries(f"{root}.{tag}", value, markdown_file)
```

### Comparing `reasoner_validator-3.6.6/reasoner_validator/versioning.py` & `reasoner_validator-3.7.0/reasoner_validator/versioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Utilities."""
 from typing import NamedTuple, Optional, List
-from sys import stderr
 from os import environ
 from re import sub, compile
 import requests
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
@@ -57,16 +56,19 @@
         string: str,
         ignore_prefix: bool = False,
         core_fields: List[str] = ('major', 'minor', 'patch'),
         ext_fields: List[str] = ('prerelease', 'buildmetadata')
 
     ):
         """
-        Initializes a SemVer from a string.  This is an 'augmented' SemVer which may also have
-        an alphabetic prefix (for example, a 'v' for 'version' designation of a GitHub release)
+        Initializes a SemVer from a string.  This is an 'augmented' SemVer which may also have an alphabetic prefix
+        (for example, a 'v' for 'version' designation of a GitHub release). Note that the string may be a
+        YAML file (path) name. In such a case, the SemVer is assumed to be encoded as a suffix in the root file name
+        just before the .yaml file extension - e.g. my_schema_3.2.1-beta5.yaml - where the version suffix string
+        is assumed to be delimited by a leading underscore character (i.e. "3.2.1-beta5" in the above example).
 
         :param string: str, string encoding the SemVer.
         :param ignore_prefix: bool, if set, any alphabetic prefix of the SemVer string is ignored (not recorded)
                               the SemVer string value, e.g. a Git Release 'v' character (i.e. v1.2.3); Default: False.
         :param core_fields: List[str], list of names of core SemVer field to explicitly set (may NOT be empty?)
                                        (default: ['major', 'minor', 'patch']).
         :param ext_fields: List[str], list of names of extended SemVer fields to explicitly set (maybe empty?)
@@ -80,24 +82,34 @@
         assert len(core_fields) >= 1 and 'major' in core_fields
         assert len(core_fields) >= 2 and 'major' in core_fields and 'minor' in core_fields
         assert all([field in ['prerelease', 'buildmetadata'] for field in ext_fields])
 
         # If the string is a file path, generically detected using the .yaml file extension,
         # then assume that the file path string encodes the SemVer string, as a part of the
         # root file name just before the .yaml file extension, e.g. my_schema_3.2.1-beta5.yaml
+        #
+        # Note that the TRAPI version suffix to the root file name
+        # is assumed to be delimited by a leading underscore character.
         if string.endswith(".yaml"):
             root_path: str = string.replace(".yaml", "")
             semver_string = root_path.split("_")[-1]
         else:
             semver_string = string
 
         match = semver_pattern.fullmatch(semver_string)
 
         if match is None:
-            raise SemVerError(f"'{string}' is not a valid release version")
+            if string.endswith(".yaml"):
+                raise SemVerError(
+                    "the mandatory TRAPI 'Semantic Version' suffix string of the root file (path) name:\n"
+                    f"\t'{string}'\nof your local YAML schema file, must delimited from the prefix of "
+                    f"the root file (path) name by a leading underscore character!"
+                )
+            else:
+                raise SemVerError(f"'{string}' is not a valid release version!")
 
         captured = match.groupdict()
         missing_fields_errmsg = f"SemVer '{string}' is missing expected fields: {', '.join(core_fields)}"
 
         observed_prefix = captured["prefix"] if not ignore_prefix else ""
         core_field_values: List[int] = list()
         for field in ['major', 'minor', 'patch']:
```

### Comparing `reasoner_validator-3.6.6/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.0/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
-from typing import Tuple, Optional, Dict
+from typing import Tuple, Optional, Dict, List
 from sys import stderr
 from copy import deepcopy
 from pprint import PrettyPrinter
 import logging
 import pytest
 from bmt import Toolkit
 from linkml_runtime.linkml_model import SlotDefinition
@@ -990,15 +990,15 @@
     ]
 )
 def test_pre_trapi_1_4_0_validate_missing_or_empty_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         trapi_version=TRAPI_1_3_0,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        sources=query[1]
+        target_provenance=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
 @pytest.mark.parametrize(
     "query",
@@ -1051,15 +1051,15 @@
         # CHEMBL.COMPOUND:CHEMBL112--biolink:occurs_together_in_literature_with->NCBIGene:762
     ]
 )
 def test_post_1_4_0_trapi_validate_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        sources=query[1]
+        target_provenance=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
 @pytest.mark.parametrize(
     "query",
@@ -1133,15 +1133,15 @@
 )
 def test_pre_1_4_0_validate_provenance(query: Tuple):
     """TRAPI pre-1.4.0 releases recorded provenance in attributes. This unit test checks for this"""
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         trapi_version=TRAPI_1_3_0,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        sources=query[1]
+        target_provenance=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
 @pytest.mark.parametrize(
     "query",
@@ -1292,15 +1292,15 @@
     ]
 )
 def test_latest_validate_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         # trapi_version="latest",
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        sources=query[1]
+        target_provenance=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
 def qualifier_validator(
         tested_method,
@@ -2072,15 +2072,44 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Knowledge Graph Node element 'biolink:NonsenseCategory' is unknown!"
             "error.knowledge_graph.node.category.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 9: abstract category in Knowledge Graphs? Itself ignored now during validation,
+            # Query 9: unknown category specified
+            {
+                "nodes": {
+                    "NCBIGene:29974": {
+                       "categories": [
+                           "biolink:BiologicalEntity"
+                       ]
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "NCBIGene:29974",
+                        "predicate": "biolink:physically_interacts_with",
+                        "object": "NCBIGene:29974",
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node has deprecated category!"
+            "warning.knowledge_graph.node.category.abstract_or_mixin"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 10: abstract category in Knowledge Graphs? Itself ignored now during validation,
             #          although if at least one 'concrete' class is not given, other related
             #          validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Entity",
@@ -2108,15 +2137,15 @@
                     }
                 }
             },
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 10: mixin category in Knowledge Graphs? Itself ignored now during validation,
+            # Query 11: mixin category in Knowledge Graphs? Itself ignored now during validation,
             #          although if at least one 'concrete' class is not given with id_prefix mappings,
             #          other related validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:GeneOrGeneProduct",
@@ -2173,15 +2202,15 @@
         #         }
         #     },
         #  f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Knowledge Graph Node element 'biolink:OntologyClass' is deprecated!"
         #     "warning.knowledge_graph.node.category.deprecated"
         # ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 11: invalid node CURIE prefix namespace, for specified category
+            # Query 12: invalid node CURIE prefix namespace, for specified category
             {
                 "nodes": {
                     "FOO:1234": {
                        "categories": [
                            "biolink:Gene"
                        ],
                     },
@@ -2213,15 +2242,15 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node 'FOO:1234' " +
             # "is unmapped to the target categories: ['biolink:Gene']?"
             "warning.knowledge_graph.node.id.unmapped_prefix"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 12: missing or empty subject, predicate, object values
+            # Query 13: missing or empty subject, predicate, object values
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     }
@@ -2244,15 +2273,15 @@
             # ditto for predicate and object... but identical code pattern thus we only test missing subject id here
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'None--biolink:interacts_with->NCBIGene:29974' " +
             # "has a missing or empty 'subject' slot value!"
             "error.knowledge_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 13: 'subject' id is missing from the nodes catalog
+            # Query 14: 'subject' id is missing from the nodes catalog
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2279,15 +2308,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'subject' id 'NCBIGene:12345' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.subject.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 14: predicate is unknown
+            # Query 15: predicate is unknown
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2314,15 +2343,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:unknown_predicate' is unknown!"
             "error.knowledge_graph.edge.predicate.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 15: predicate is invalid - may be a valid Biolink element but is not a predicate
+            # Query 16: predicate is invalid - may be a valid Biolink element but is not a predicate
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2349,15 +2378,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:has_unit' is invalid!"
             "error.knowledge_graph.edge.predicate.invalid"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 16: predicate is a mixin - not allowed in Knowledge Graphs
+            # Query 17: predicate is a mixin - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "HGNC:3059": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2384,15 +2413,15 @@
                 }
             },
             # "{KNOWLEDGE_GRAPH_PREFIX}: ERROR -Predicate element 'biolink:increases_amount_or_activity of' is a mixin!"
             "error.knowledge_graph.edge.predicate.mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 17: predicate is abstract - not allowed in Knowledge Graphs
+            # Query 18: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
                        "categories": [
                            "biolink:InformationContentEntity"
                        ]
                     },
@@ -2419,15 +2448,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:contributor' is abstract!"
             "error.knowledge_graph.edge.predicate.abstract"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 18: predicate is non-canonical
+            # Query 19: predicate is non-canonical
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2454,15 +2483,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge predicate 'biolink:affected_by' is non-canonical?"
             "warning.knowledge_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 19: 'object' id is missing from the nodes catalog
+            # Query 20: 'object' id is missing from the nodes catalog
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2490,15 +2519,15 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'object' id " +
             # f"'PUBCHEM.COMPOUND:678' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 20: attribute 'attribute_type_id' is missing
+            # Query 21: attribute 'attribute_type_id' is missing
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2525,15 +2554,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'attribute_type_id' key!"
             "error.knowledge_graph.edge.attribute.type_id.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: attribute 'value' is missing?
+            # Query 22: attribute 'value' is missing?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2560,15 +2589,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'value' key!"
             "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: 'attribute_type_id' is not a CURIE
+            # Query 23: 'attribute_type_id' is not a CURIE
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2595,15 +2624,15 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute_type_id 'not_a_curie' is not a CURIE!"
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
+            # Query 24: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2631,15 +2660,15 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id "
             # "'biolink:synonym' is not a biolink:association_slot?"
             "warning.knowledge_graph.edge.attribute.type_id.not_association_slot"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
+            # Query 25: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2668,15 +2697,15 @@
                     }
                 }
             },
             ""  # this should recognize the 'attribute_type_id' as a Biolink CURIE
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
+            # Query 26: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2702,15 +2731,15 @@
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id 'foo:bar' " +
             # f"has a CURIE prefix namespace unknown to Biolink!"
             "warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix"
         ),
-        (   # Query 26:  # An earlier Biolink Model won't recognize a category not found in its specified release
+        (   # Query 27:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
@@ -2730,15 +2759,15 @@
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                     }
                 }
             },
             "error.knowledge_graph.node.category.unknown"
         ),
-        (   # Query 27:  #'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
+        (   # Query 28:  #'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
@@ -2767,15 +2796,15 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 28: 'attribute_type_id' is not a 'biolink:association_slot'
+            # Query 29: 'attribute_type_id' is not a 'biolink:association_slot'
             #           (biolink:synonym is a node property) but...
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
@@ -2858,24 +2887,59 @@
         graph=edge_without_attributes,
         trapi_version=TRAPI_1_3_0,
         biolink_version=SUPPRESS_BIOLINK_MODEL_VALIDATION
     )
     check_messages(validator, "")
 
 
-SAMPLE_RETRIEVAL_SOURCE = {
+SAMPLE_PRIMARY_RETRIEVAL_SOURCE = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "infores:chebi",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source",
+
+    # nothing upstream... it' primary!
+    "upstream_resource_ids": []
+}
+
+SAMPLE_KP_RETRIEVAL_SOURCE = {
     # required, infores CURIE to an Information Resource
     "resource_id": "infores:molepro",
 
     # required, string drawn from the TRAPI ResourceRoleEnum
     # values that were formerly recorded as TRAPI attributes
     # are now presented as first class edge annotation
-    "resource_role": "primary_knowledge_source"
+    "resource_role": "aggregator_knowledge_source",
+
+    # primary knowledge source is 'upstream'
+    "upstream_resource_ids": ["infores:chebi"]
+}
+
+SAMPLE_ARA_RETRIEVAL_SOURCE = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "infores:arax",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "aggregator_knowledge_source",
+
+    # KP is 'upstream'
+    "upstream_resource_ids": ["infores:molepro"]
 }
 
+SAMPLE_SOURCES_ARRAY = [
+    SAMPLE_PRIMARY_RETRIEVAL_SOURCE,
+    SAMPLE_KP_RETRIEVAL_SOURCE,
+    SAMPLE_ARA_RETRIEVAL_SOURCE
+]
+
 SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ID = {
     # required, string drawn from the TRAPI ResourceRoleEnum
     # values that were formerly recorded as TRAPI attributes
     # are now presented as first class edge annotation
     "resource_role": "primary_knowledge_source"
 }
 
@@ -2911,18 +2975,42 @@
     # required, string drawn from the TRAPI ResourceRoleEnum
     # values that were formerly recorded as TRAPI attributes
     # are now presented as first class edge annotation
     "resource_role": "primary_knowledge_source"
 }
 
 
+def test_build_source_trail():
+    sources: Dict[str, List[str]] = {
+        "infores:chebi": [],
+        "infores:biothings-explorer": ["infores:chebi"],
+        "infores:molepro": ["infores:biothings-explorer"],
+        "infores:arax": ["infores:molepro"]
+    }
+    assert BiolinkValidator.build_source_trail(sources) == \
+           "infores:chebi -> infores:biothings-explorer -> infores:molepro -> infores:arax"
+
+    # even though a primary_knowledge_source appears to be missing
+    # we are able to infer a path on a putative primary source
+    sources: Optional[Dict[str, List[str]]] = {
+        "infores:biothings-explorer": ["infores:chebi"],
+        "infores:molepro": ["infores:biothings-explorer"],
+        "infores:arax": ["infores:molepro"]
+    }
+    assert BiolinkValidator.build_source_trail(sources) == \
+           "infores:chebi -> infores:biothings-explorer -> infores:molepro -> infores:arax"
+
+
 @pytest.mark.parametrize(
     "sources,validation_code",
     [
-        ([SAMPLE_RETRIEVAL_SOURCE], ""),  # No validation code generated?
+        ([SAMPLE_PRIMARY_RETRIEVAL_SOURCE], ""),  # No validation code generated?
+        ([SAMPLE_KP_RETRIEVAL_SOURCE], "error.knowledge_graph.edge.provenance.missing_primary"),
+        ([SAMPLE_ARA_RETRIEVAL_SOURCE], "error.knowledge_graph.edge.provenance.missing_primary"),
+        (SAMPLE_SOURCES_ARRAY, ""),             # No validation code generated?
         (None, "error.knowledge_graph.edge.sources.missing"),
         ([], "error.knowledge_graph.edge.sources.empty"),
         ("not-an-array", "error.knowledge_graph.edge.sources.not_array"),
         (
             [SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ID],
             "error.knowledge_graph.edge.sources.retrieval_source.resource_id.empty"
         ),
```

### Comparing `reasoner_validator-3.6.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
           description: The least critical level of logs to return
           oneOf:
             - $ref: '#/components/schemas/LogLevel'
           nullable: true
         workflow:
           description: List of workflow steps to be executed.
           oneOf:
-            - $ref: http://standards.ncats.io/workflow/1.3.4/schema
+            - $ref: http://standards.ncats.io/workflow/1.3.5/schema
           nullable: true
         submitter:
           type: string
           description: >-
             Any string for self-identifying the submitter of a query. The
             purpose of this optional field is to aid in the tracking of
             the source of queries for development and issue resolution.
@@ -503,15 +503,15 @@
         auxiliary_graphs:
           type: object
           description: >-
             Dictionary of AuxiliaryGraph instances that are used by Knowledge
             Graph Edges and Result Analyses. These are referenced elsewhere by
             the dictionary key.
           additionalProperties:
-            $ref: '#components/schemas/AuxiliaryGraph'
+            $ref: '#/components/schemas/AuxiliaryGraph'
           nullable: true
       additionalProperties: false
     LogEntry:
       description: >-
         The LogEntry object contains information useful for tracing
         and debugging across Translator components.  Although an
         individual component (for example, an ARA or KP) may have its
```

### Comparing `reasoner_validator-3.6.6/tests/test_response_validator.py` & `reasoner_validator-3.7.0/tests/test_response_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from json import dump
 
 from copy import deepcopy
 
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
-from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_1
+from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
 
 from tests import PATCHED_140_SCHEMA_FILEPATH
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
@@ -89,16 +89,16 @@
                    "value_type_id": "biolink:InformationResource"
                }
             ],
         }
     }
 
 _TEST_KG_1 = {
-    'nodes': _TEST_NODES_1,
-    'edges': _TEST_EDGES_1
+    "nodes": _TEST_NODES_1,
+    "edges": _TEST_EDGES_1
 }
 
 _TEST_RESULTS_1 = [
         {
             "node_bindings": {
                 "type-2 diabetes": [{"id": "MONDO:0005148"}],
                 "drug": [{"id": "ncats.drug:9100L32L2N"}]
@@ -126,16 +126,16 @@
                    "value_type_id": "biolink:InformationResource"
                }
            ],
         }
     }
 
 _TEST_KG_2 = {
-    'nodes': _TEST_NODES_1,
-    'edges': _TEST_EDGES_2
+    "nodes": _TEST_NODES_1,
+    "edges": _TEST_EDGES_2
 }
 
 _TEST_QG_2 = {
     "nodes": {
         "paper": {
             "categories": ["biolink:InformationContentEntity"]
         },
@@ -179,16 +179,16 @@
                    "value": "infores:automat-text-mining-provider"
                }
            ],
         }
     }
 
 _TEST_KG_3 = {
-    'nodes': _TEST_NODES_2,
-    'edges': _TEST_EDGES_3
+    "nodes": _TEST_NODES_2,
+    "edges": _TEST_EDGES_3
 }
 
 _TEST_RESULTS_2 = [
         {
             "node_bindings": {
                 "paper": [{"id": "PMID:11156626"}],
                 "author": [{"id": "ORCID:0000-0002-4447-5978"}]
@@ -221,20 +221,20 @@
                }
            ],
         }
     }
 
 
 _TEST_KG_4 = {
-    'nodes': _TEST_NODES_1,
-    'edges': _TEST_EDGES_4
+    "nodes": _TEST_NODES_1,
+    "edges": _TEST_EDGES_4
 }
 
 # From Implementation Guidlines circa June 2023
-_TEST_TRAPI_1_4_1_FULL_SAMPLE = {
+_TEST_TRAPI_1_4_2_FULL_SAMPLE = {
     "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
             "edges": {
@@ -250,16 +250,38 @@
             "edges": {
                 "df87ff82": {
                     "subject": "ncats.drug:9100L32L2N",
                     "predicate": "biolink:treats",
                     "object": "MONDO:0005148",
                     "sources": [
                         {
+                            "resource_id": "infores:chebi",
+                            "resource_role": "primary_knowledge_source",
+                            "upstream_resource_ids": []
+                        },
+                        {
+                            "resource_id": "infores:biothings-explorer",
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:chebi"
+                            ]
+                        },
+                        {
                             "resource_id": "infores:molepro",
-                            "resource_role": "primary_knowledge_source"
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:biothings-explorer"
+                            ]
+                        },
+                        {
+                            "resource_id": "infores:arax",
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:molepro"
+                            ]
                         }
                     ]
                 }
             }
         },
         "auxiliary_graphs": {
             "a0": {
@@ -294,119 +316,119 @@
                     }
                 ]
             }
         ]
     }
 }
 
-_TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_1_FULL_SAMPLE)
-_TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
 
 
 @pytest.mark.parametrize(
     "query",
     [
-        (   # Query 0 - No 'workflow' key in TRAPI Response
+        (   # Query 0 - No "workflow" key in TRAPI Response
             {
-                'message': {}
+                "message": {}
             },
         ),
-        (   # Query 1 - Null 'workflow' key value
+        (   # Query 1 - Null "workflow" key value
             {
-                'message': {},
-                'workflow': None
+                "message": {},
+                "workflow": None
             },
         ),
-        (  # Query 2 - Null 'workflow' key list
+        (  # Query 2 - Null "workflow" key list
             {
-                'message': {},
-                'workflow': []
+                "message": {},
+                "workflow": []
             },
         ),
-        (  # Query 3 - 'runner_parameters' is Null
+        (  # Query 3 - "runner_parameters" is Null
             {
-                'message': {},
-                'workflow': [
+                "message": {},
+                "workflow": [
                     {
-                        'runner_parameters': None,
-                        'id': 'sort_results_score',
-                        'parameters': {"ascending_or_descending": "ascending"}
+                        "runner_parameters": None,
+                        "id": "sort_results_score",
+                        "parameters": {"ascending_or_descending": "ascending"}
                     }
                 ]
             },
         ),
-        (  # Query 4 - 'parameters' is Null
+        (  # Query 4 - "parameters" is Null
             {
-                'message': {},
-                'workflow': [
-                    {'runner_parameters': {'allowlist': ["infores:aragorn"]}, 'id': 'lookup', 'parameters': None}
+                "message": {},
+                "workflow": [
+                    {"runner_parameters": {"allowlist": ["infores:aragorn"]}, "id": "lookup", "parameters": None}
                 ]
             },
         ),
-        (  # Query 5 - both 'parameters' and 'runner_parameters' are Null
+        (  # Query 5 - both "parameters" and "runner_parameters" are Null
             {
-                'message': {},
-                'workflow': [
-                    {'runner_parameters': None, 'id': 'lookup', 'parameters': None}
+                "message": {},
+                "workflow": [
+                    {"runner_parameters": None, "id": "lookup", "parameters": None}
                 ]
             },
         ),
         (   # Query 6 - Now, we patch the Message itself when it is not empty - knowledge graph is nullable
             {
-                'message': {
-                    'knowledge_graph': None
+                "message": {
+                    "knowledge_graph": None
                 }
             },
         ),
         (   # Query 7 - Now, we patch the Message itself when it is not empty
             {
-                'message': {
-                    'knowledge_graph': {
-                        'nodes': {},
-                        'edges': {}
+                "message": {
+                    "knowledge_graph": {
+                        "nodes": {},
+                        "edges": {}
                     }
                 }
             },
         ),
         (   # Query 8 - Now, we patch the Message itself when it is not empty
             {
-                'message': {
-                    'knowledge_graph': {
-                        'nodes': {},
-                        'edges': {}
+                "message": {
+                    "knowledge_graph": {
+                        "nodes": {},
+                        "edges": {}
                     }
                 }
             },
         ),
-        (   # Query 9 - Now, we patch the Message.knowledge_edge.sources itself when it is not empty
+        (   # Query 9 - Now, we patch the "Message.knowledge_edge.sources" itself when it is not empty
             {
-                'message': {
-                    'knowledge_graph': {
-                        'nodes': {},
-                        'edges': {
+                "message": {
+                    "knowledge_graph": {
+                        "nodes": {},
+                        "edges": {
                             "alice-in-wonderland": {
-                                 'subject': "tweedle-dee",
-                                 'predicate': "and",
-                                 'object': "tweedle-dum",
-                                 'sources': [
+                                 "subject": "tweedle-dee",
+                                 "predicate": "and",
+                                 "object": "tweedle-dum",
+                                 "sources": [
                                      {
-                                         'resource_id': "infores:rabbit-hole",
-                                         'resource_role': "primary_knowledge_source"
+                                         "resource_id": "infores:rabbit-hole",
+                                         "resource_role": "primary_knowledge_source"
                                      }
                                  ]
                             }
                         }
                     }
                 }
             },
         ),
         (   # Query 10 - Now, we patch the Message itself when it is not empty
             {
-                'message': {
-                    'auxiliary_graphs': None
+                "message": {
+                    "auxiliary_graphs": None
                 }
             },
         )
     ]
 )
 def test_sanitize_trapi_query(query: Tuple):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
@@ -587,15 +609,15 @@
                     "results": {"invalid results"}
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
-            # "Validate TRAPI Response: ERROR - the 'Response.Message.Results' field
+            # "Validate TRAPI Response: ERROR - the "Response.Message.Results" field
             # is not TRAPI schema validated since it has the wrong format!"
             "critical.trapi.validation"
         ),
         (
             # Query 8 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Empty Results detected next - just issue a warning?
             {
@@ -609,15 +631,15 @@
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned empty Message.results?"
             "warning.trapi.response.results.empty"
         ),
         (
-            # Query 9 - Full Message, without 'sources' and 'strict_validation': False - should pass?
+            # Query 9 - Full Message, without "sources" and "strict_validation": False - should pass?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
@@ -639,15 +661,15 @@
             TRAPI_1_3_0,
             None,
             None,
             True,
             ""
         ),
         (
-            # Query 11 - Full Message, with strict validation and non-null sources that match
+            # Query 11 - Full Message, with "strict validation" and non-null sources" that match
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
@@ -696,15 +718,15 @@
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
             "warning.knowledge_graph.edge.provenance.ara.missing"
         ),
         (
-            # Query 14 - Full Message, with strict validation and a non-null sources data that matches
+            # Query 14 - Full Message, with "strict validation" and a non-null "sources" data that matches
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
@@ -715,15 +737,15 @@
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
             ""
         ),
         (
-            # Query 15 - Full Message, with strict validation and a non-null sources KP that matches
+            # Query 15 - Full Message, with "strict validation" and a non-null "sources" KP that matches
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
@@ -755,15 +777,15 @@
                 "kp_source_type": "aggregator"
             },
             True,
             "error.knowledge_graph.edge.provenance.missing_primary"
         ),
         (
             # Query 17 - Full Message, with strict validation and
-            #            non-null kp_source_type results, has multiple primary knowledge sources
+            #            non-null kp_source_type results, has multiple "primary knowledge sources"
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_4,
                     "results": _TEST_RESULTS_1
                 }
             },
@@ -775,15 +797,15 @@
                 "kp_source_type": "aggregator"
             },
             True,
             "warning.knowledge_graph.edge.provenance.multiple_primary"
         ),
         (
             # Query 18 - Full Message, with non-strict validation.
-            #            Both knowledge graph nodes have 'mixin' categories,
+            #            Both knowledge graph nodes have "mixin" categories,
             #            the list of categories for knowledge graphs
             #            must have at least one concrete category,
             #            hence, a validation error is now reported:
             {
                 "message": {
                     "query_graph": _TEST_QG_2,
                     "knowledge_graph": _TEST_KG_3,
@@ -809,55 +831,55 @@
             None,
             None,
             True,
             "error.query_graph.edge.predicate.abstract"
         ),
         (
             # Query 20 - Valid full Message, under strict validation.
-            #            Message is valid, but the 'workflow' field is not an array?
+            #            Message is valid, but the "workflow" field is not an array?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": "workflows-not-an-array"
             },
             TRAPI_1_3_0,
             None,
             None,
             True,
-            # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array"
+            # "Validate TRAPI Response: ERROR - TRAPI schema error: the "workflow" field must be an array"
             "critical.trapi.validation"
         ),
         (
             # Query 21 - Valid full Message, under strict validation.
-            #            Message is valid, the 'workflow' field is an array,
+            #            Message is valid, the "workflow" field is an array,
             #            but the single list entry is an invalid workflow spec?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": ["not-a-valid-workflow-spec"]
             },
             TRAPI_1_3_0,
             None,
             None,
             True,
-            # Validate TRAPI Response: ERROR - TRAPI schema error: the 'workflow' field must be an array of
-            # a 'workflow' JSON objects, with contents as defined by the workflow schema.
+            # Validate TRAPI Response: ERROR - TRAPI schema error: the "workflow" field must be an array of
+            # a "workflow" JSON objects, with contents as defined by the workflow schema.
             "critical.trapi.validation"
         ),
         (
             # Query 22 - Valid full Message, under strict validation.
-            #            Message is valid, the 'workflow' field is an array,
+            #            Message is valid, the "workflow" field is an array,
             #            but the single list entry is in the workflow schema
-            #            and has at least the one required field 'id'
+            #            and has at least the one required field "id"
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [{"id": "annotate"}]
@@ -865,25 +887,25 @@
             TRAPI_1_3_0,
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
-            # Query 23 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
-            #            but the single list entry is an elaborated 'real world' workflow spec,
+            # Query 23 - Valid full Message, under strict validation. Message is valid, the "workflow" field is array,
+            #            but the single list entry is an elaborated "real world" workflow spec,
             #            but one entry overlay_compute_ngd is incomplete - doesn't fully validate!
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [
-                    {  # 'real' world workflow spec from E. Deutsch
+                    {  # "real" world workflow spec from E. Deutsch
                       "id": "fill",
                       "parameters": {
                         "allowlist": [
                           "infores-rtx-kg2"
                         ]
                       }
                     },
@@ -904,29 +926,29 @@
                     }
                 ]
             },
             TRAPI_1_3_0,
             None,
             None,
             True,
-            # "Validate TRAPI Response: ERROR - TRAPI schema validation error: the 'workflow'
-            # field entry overlay_compute_ngd is missing a required parameter 'qnodes_keys'
+            # "Validate TRAPI Response: ERROR - TRAPI schema validation error: the "workflow"
+            # field entry overlay_compute_ngd is missing a required parameter "qnodes_keys"
             "critical.trapi.validation"
         ),
         (
-            # Query 24 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
-            #            but the single list entry is an elaborated 'real world' workflow spec
+            # Query 24 - Valid full Message, under strict validation. Message is valid, the "workflow" field is array,
+            #            but the single list entry is an elaborated "real world" workflow spec
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [
-                    {  # 'real' world workflow spec from E. Deutsch
+                    {  # "real" world workflow spec from E. Deutsch
                       "id": "fill",
                       "parameters": {
                         "allowlist": [
                           "infores-rtx-kg2"
                         ]
                       }
                     },
@@ -952,15 +974,15 @@
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
             # Query 25 - Valid full Message, under strict validation. Message is valid,
-            #            the 'workflow' field is an array, but runner_parameters is None.
+            #            the "workflow" field is an array, but runner_parameters is None.
             #            This is technically invalid, but we have a code patch which should filter it out (for now)
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
@@ -976,31 +998,30 @@
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
         ),
         (   # Query 26 - We throw a full TRAPI JSON example here (taken directly from the
             #            TRAPI implementation guidelines...) just for fun and profit
-            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
-            TRAPI_1_4_1,
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE,
+            TRAPI_1_4_2,
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
         )
     ]
 )
 def test_check_biolink_model_compliance_of_trapi_response(query: Tuple):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
         trapi_version=query[1],
         biolink_version=query[2],
-        sources=query[3],
         strict_validation=query[4]
     )
-    validator.check_compliance_of_trapi_response(response=query[0])
+    validator.check_compliance_of_trapi_response(response=query[0], target_provenance=query[3])
     check_messages(validator, query[5], no_errors=True)
 
 
 @pytest.mark.parametrize(
     "response,trapi_version,biolink_version,sources,strict_validation,code",
     [
         (   # Query 0 - Completely empty Response.Message
@@ -1104,49 +1125,49 @@
             None,
             None,
             False,
             ""
         ),
         (
             # Query 7 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
-            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE,
             # 25 June 2023 1.4.0 trapi_version with
             # defective auxiliary_graphs schema model
             # now temporarily patched?
-            TRAPI_1_4_1,
+            TRAPI_1_4_2,
             None,
             None,
             False,
             ""  # would be a "critical.trapi.validation" if the schema was unpatched
         ),
         (
             # Query 8 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
-            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE,
             # patched 1.4.0 test schema - fixed critical
             # TRAPI schema parsing error with auxiliary_graphs
             PATCHED_140_SCHEMA_FILEPATH,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 9 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
-            _TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
             # 25 June 2023 1.4.0 trapi_version with
             # defective auxiliary_graphs schema model
-            TRAPI_1_4_1,
+            TRAPI_1_4_2,
             None,
             None,
             False,
             ""  # nullable: true allows this outcome
         ),
         (
             # Query 10 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
-            _TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
             # patched 1.4.0 test schema - fixed critical
             # TRAPI schema parsing error with auxiliary_graphs
             PATCHED_140_SCHEMA_FILEPATH,
             None,
             None,
             False,
             ""  # should still work if nullable: true
@@ -1155,13 +1176,34 @@
 )
 def test_check_biolink_model_compliance_of_trapi_response_suppressing_empty_data_warnings(
         response, trapi_version, biolink_version, sources, strict_validation, code
 ):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
         trapi_version=trapi_version,
         biolink_version=biolink_version,
-        sources=sources,
         strict_validation=strict_validation,
         suppress_empty_data_warnings=True
     )
-    validator.check_compliance_of_trapi_response(response=response)
+    validator.check_compliance_of_trapi_response(response=response, target_provenance=sources)
     check_messages(validator, code, no_errors=True)
+
+
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_REPORTABLE_ERRORS = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
+sample_message = _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_REPORTABLE_ERRORS["message"]
+sample_qgraph = sample_message["query_graph"]
+sample_kg = sample_message["knowledge_graph"]
+sample_kg_node_missing_category = sample_kg["nodes"]["MONDO:0005148"].pop("categories")
+sample_kg_edge_missing_node_subject = sample_kg["edges"]["df87ff82"].pop("subject")
+sample_kg_edge_abstract_predicate = sample_kg["edges"]["df87ff82"]["predicate"] = "biolink:not_a_predicate"
+
+
+@pytest.mark.parametrize(
+    "response",
+    [
+        _TEST_TRAPI_1_4_2_FULL_SAMPLE,
+        _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_REPORTABLE_ERRORS
+    ]
+)
+def test_dump_report_of_biolink_model_compliance_of_trapi_response_with_errors(response: Dict):
+    validator: TRAPIResponseValidator = TRAPIResponseValidator()
+    validator.check_compliance_of_trapi_response(response=response)
+    validator.dump()
```

### Comparing `reasoner_validator-3.6.6/tests/test_semver.py` & `reasoner_validator-3.7.0/tests/test_semver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 """Test semantic version handling."""
 import pytest
 
-from tests import PATCHED_SCHEMA_VERSION, PATCHED_140_SCHEMA_FILEPATH
-from reasoner_validator.versioning import semver_pattern, SemVer, SemVerUnderspecified
+from tests import (
+    PATCHED_SCHEMA_VERSION,
+    PATCHED_140_SCHEMA_FILEPATH,
+    BROKEN_SCHEMA_FILEPATH
+)
+from reasoner_validator.versioning import (
+    semver_pattern,
+    SemVer,
+    SemVerError,
+    SemVerUnderspecified
+)
 
 
 def test_regex_pattern():
     # test the semver pattern directly
     assert semver_pattern.fullmatch("1.2.3")
     assert semver_pattern.fullmatch("1.2")
     assert semver_pattern.fullmatch("1")
@@ -161,10 +170,11 @@
 
 
 sample_schema_version = SemVer.from_string(PATCHED_SCHEMA_VERSION)
 sample_schema_file_semver = SemVer.from_string(PATCHED_140_SCHEMA_FILEPATH)
 
 
 def test_schema_file_versioning():
-
     # Sample schema file has internal version type
     assert sample_schema_file_semver == sample_schema_version
+    with pytest.raises(SemVerError):
+        SemVer.from_string(BROKEN_SCHEMA_FILEPATH)
```

### Comparing `reasoner_validator-3.6.6/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.0/tests/test_trapi_versioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test TRAPI version handling."""
 from typing import Dict, Optional
 
 import pytest
 
 from reasoner_validator.versioning import get_latest_version
 from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, load_schema, TRAPIAccessError
-from tests import PATCHED_140_SCHEMA_FILEPATH
+from tests import PATCHED_140_SCHEMA_FILEPATH, BROKEN_SCHEMA_FILEPATH
 
 
 def test_release_tag_is_none():
     trapi_version:  Optional[str] = get_latest_version(release_tag=None)
     assert trapi_version is None
 
 
@@ -34,15 +34,15 @@
 
 
 def test_semver_spec_trapi_version_without_prefix():
     trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_RELEASE[1:])
     assert trapi_version == LATEST_TRAPI_RELEASE
 
 
-def test_schema_spec_trapi_version():
+def test_schema_file_spec_trapi_version():
     trapi_version = get_latest_version(release_tag=PATCHED_140_SCHEMA_FILEPATH)
     assert trapi_version is not None
     assert trapi_version.endswith(".yaml")
 
 
 def test_load_schema_with_semver_trapi_version():
     trapi_version: str = get_latest_version(release_tag="1")
@@ -54,14 +54,14 @@
     trapi_version: str = get_latest_version(release_tag="master")
     schema: Dict = load_schema(trapi_version)
     assert schema
     with pytest.raises(ValueError):
         load_schema(target="not-a-branch-name")
 
 
-def test_load_schema_with_schema_trapi_version():
+def test_load_schema_with_schema_file_spec_trapi_version():
     trapi_version: str = get_latest_version(release_tag=PATCHED_140_SCHEMA_FILEPATH)
     assert trapi_version is not None
     schema: Dict = load_schema(trapi_version)
     assert schema
     with pytest.raises(TRAPIAccessError):
         load_schema(target="not-a-trapi-schema.yaml")
```

### Comparing `reasoner_validator-3.6.6/tests/test_validate.py` & `reasoner_validator-3.7.0/tests/test_validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -614,15 +614,15 @@
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_latest_trapi_missing_key_message_edge_component_validation(trapi_version: str):
     """Test Message.KnowledgeGraph.Edge components missing their required keys
        in TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         validator.validate({
-            # missing required 'subject', 'predicate', 'object' and 'sources'
+            # missing required 'subject', 'predicate', 'object' and "sources"
             "foo": {},
             "bar": {},
         }, "Edge")
 
 
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_latest_trapi_null_message_edge_component_validation(trapi_version: str):
@@ -648,56 +648,56 @@
         faulty_predicate = SAMPLE_LATEST_TEST_EDGE.copy()
         # predicate is not a Biolink predicate term CURIE
         faulty_predicate["predicate"] = "not-a-biolink-predicate-CURIE"
         validator.validate(faulty_predicate, "Edge")
 
 
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
-def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version: str):
+def test_latest_trapi_more_flawed_message_edge_retrieval_sources_component_validation(trapi_version: str):
     """Test various invalid Message.KnowledgeGraph.Edge.sources values in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
-        faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
-        # 'sources' is not an array (of RetrievalSource objects)
-        faulty_sources["sources"] = "not-an-array"
-        validator.validate(faulty_sources, "Edge")
-    with pytest.raises(ValidationError):
-        faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
-        # items in the 'sources' array must be a non-empty array of (RetrievalSource) objects
-        faulty_sources["sources"] = list()
-        validator.validate(faulty_sources, "Edge")
-    with pytest.raises(ValidationError):
-        faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
-        # items in the 'sources' array must be (RetrievalSource) objects
-        faulty_sources["sources"] = ["not-a-json-object"]
-        validator.validate(faulty_sources, "Edge")
-    with pytest.raises(ValidationError):
-        faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
-        # items in the 'sources' array must be RetrievalSource objects
-        faulty_sources["sources"] = [{"not-an-RetrievalSource-key": "something"}]
-        validator.validate(faulty_sources, "Edge")
+        faulty_target_provenance = SAMPLE_LATEST_TEST_EDGE.copy()
+        # "target_provenance" is not an array (of RetrievalSource objects)
+        faulty_target_provenance["target_provenance"] = "not-an-array"
+        validator.validate(faulty_target_provenance, "Edge")
+    with pytest.raises(ValidationError):
+        faulty_target_provenance = SAMPLE_LATEST_TEST_EDGE.copy()
+        # items in the "target_provenance" array must be a non-empty array of (RetrievalSource) objects
+        faulty_target_provenance["target_provenance"] = list()
+        validator.validate(faulty_target_provenance, "Edge")
+    with pytest.raises(ValidationError):
+        faulty_target_provenance = SAMPLE_LATEST_TEST_EDGE.copy()
+        # items in the "target_provenance" array must be (RetrievalSource) objects
+        faulty_target_provenance["target_provenance"] = ["not-a-json-object"]
+        validator.validate(faulty_target_provenance, "Edge")
+    with pytest.raises(ValidationError):
+        faulty_target_provenance = SAMPLE_LATEST_TEST_EDGE.copy()
+        # items in the "target_provenance" array must be RetrievalSource objects
+        faulty_target_provenance["target_provenance"] = [{"not-an-RetrievalSource-key": "something"}]
+        validator.validate(faulty_target_provenance, "Edge")
 
 
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
-def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version: str):
+def test_latest_trapi_more_flawed_message_edge_retrieval_sources_component_validation(trapi_version: str):
     """Test various invalid Message.KnowledgeGraph.Edge.sources values in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         faulty_rs = SAMPLE_RETRIEVAL_SOURCE.copy()
-        # items in the 'sources' array must be
+        # items in the "target_provenance" array must be
         # RetrievalSource objects with a 'resource' key
         faulty_rs.pop("resource_id")
         validator.validate(faulty_rs, "RetrievalSource")
     with pytest.raises(ValidationError):
         faulty_rs = SAMPLE_RETRIEVAL_SOURCE.copy()
-        # items in the 'sources' array must be
+        # items in the "target_provenance" array must be
         # RetrievalSource objects with a 'resource' key
         faulty_rs.pop("resource_role")
         validator.validate(faulty_rs, "RetrievalSource")
     with pytest.raises(ValidationError):
         faulty_rs = SAMPLE_RETRIEVAL_SOURCE.copy()
-        # items in the 'sources' array must be
+        # items in the "target_provenance" array must be
         # RetrievalSource objects with a 'resource' key
         faulty_rs["resource_role"] = "not_a_ResourceRoleEnum_enum_value"
         validator.validate(faulty_rs, "RetrievalSource")
```

### Comparing `reasoner_validator-3.6.6/tests/test_validation_report.py` & `reasoner_validator-3.7.0/tests/test_validation_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Testing Validation Report methods"""
 from typing import Optional, Dict, Tuple, List
 from sys import stderr
 
 import pytest
 
+from reasoner_validator.message import MESSAGE_CATALOG, SCOPED_MESSAGES
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.validation_codes import CodeDictionary
 from reasoner_validator.versioning import get_latest_version
 
 TEST_TRAPI_VERSION = get_latest_version(ValidationReporter.DEFAULT_TRAPI_VERSION)
 TEST_BIOLINK_VERSION = "2.4.8"
 
@@ -155,37 +156,51 @@
     info_attribute = CodeDictionary.get_description("warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix")
     assert info_attribute is not None
     assert info_attribute.startswith("Non-Biolink CURIEs are tolerated")
     assert CodeDictionary.get_description("foo.bar") is None
 
 
 def test_message_display():
-    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in CodeDictionary.display(
-        code="info.compliant",
+    scoped_messages = CodeDictionary.display(code="info.compliant", add_prefix=True)
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display("error.knowledge_graph.nodes.empty", add_prefix=True)
+    assert "ERROR - Knowledge Graph Nodes: No nodes found!" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display(
+        code="info.excluded",
+
+        # this code has "global" scope plus
+        # an "identifier" context, but no other parameters
+        messages={
+            "global": {"a->biolink:related_to->b": None}
+        },
         add_prefix=True
     )
-    assert "ERROR - Knowledge Graph Nodes: No nodes found!" \
-           in CodeDictionary.display("error.knowledge_graph.nodes.empty", add_prefix=True)
     assert "INFO - Excluded: All test case S-P-O triples from " + \
-           "resource test location, or specific user excluded S-P-O triples" \
-           in CodeDictionary.display(
-                code="info.excluded",
-                parameters={"a->biolink:related_to->b": None},  # this code has no other parameters
-                add_prefix=True
-            )
+           "resource test location, or specific user excluded S-P-O triples" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display(
+        code="info.input_edge.predicate.abstract",
+
+        # this code has "global" scope, an "identifier" context
+        # plus one other parameter named 'edge_id'
+        messages={
+            "infores:chebi->infores:molepro->infores:arax": {
+                "biolink:contributor": [
+                    {
+                        "edge_id": "a->biolink:related_to->b"
+                    }
+                ]
+            }
+        },
+        add_prefix=True
+    )
     assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" \
-           in CodeDictionary.display(
-                code="info.input_edge.predicate.abstract",
-                parameters={
-                    "biolink:contributor": [
-                        {"edge_id": "a->biolink:related_to->b"}
-                    ]
-                },  # this code has one other parameter named 'element_name'
-                add_prefix=True
-            )
+           in scoped_messages["infores:chebi->infores:molepro->infores:arax"]
 
 
 def test_unknown_message_code():
     with pytest.raises(AssertionError):
         CodeDictionary.display(code="foo.bar")
 
 
@@ -193,22 +208,24 @@
     reporter = ValidationReporter(prefix="First Validation Report", trapi_version=TEST_TRAPI_VERSION)
     reporter.report(code="info.compliant")
     reporter.report(
         code="info.input_edge.predicate.abstract",
         identifier="biolink:contributor",
         edge_id="a->biolink:contributor->b"
     )
-    report: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter.get_messages()
+    report: MESSAGE_CATALOG = reporter.get_messages()
     assert 'information' in report
     assert len(report['information']) > 0
-    messages: List[str] = list()
-    for code, parameters in report['information'].items():
-        messages.extend(CodeDictionary.display(code, parameters, add_prefix=True))
-    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in messages
-    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" in messages
+
+    displayed: List[str] = list()
+    for code, messages in report['information'].items():
+        scoped_messages = CodeDictionary.display(code, messages, add_prefix=True)
+        displayed.extend(scoped_messages["global"])
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in displayed
+    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" in displayed
 
 
 def test_messages():
     # Loading and checking a first reporter
     reporter1 = ValidationReporter(prefix="1st Test Message Set", trapi_version=TEST_TRAPI_VERSION)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() is None
@@ -247,96 +264,111 @@
     reporter3 = ValidationReporter()
     reporter3.report("error.trapi.response.query_graph.missing")
     reporter1.merge(reporter3)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
 
     # testing addition a few raw batch messages
-    new_messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = {
+    new_messages: MESSAGE_CATALOG = {
         "information": {
             "info.excluded": {
-                "Horace van der Gelder": None
+                "global": {
+                    "Horace van der Gelder": None
+                }
             }
         },
         "warnings": {
             "warning.knowledge_graph.node.id.unmapped_prefix": {
-                "Will Robinson": [
-                    {
-                        "categories": "Lost in Space"
-                    }
-                ]
+                "infores:earth -> infores:spaceship": {
+                    "Will Robinson": [
+                        {
+                            "categories": "Lost in Space"
+                        }
+                    ]
+                }
             }
         },
         "errors": {
             "error.biolink.model.noncompliance": {
-                "6.6.6": [
-                    {
-                        'reason': "Dave, this can only be due to human error..."
-                    }
-                ]
-
+                "global": {
+                    "6.6.6": [
+                        {
+                            'reason': "Dave, this can only be due to human error..."
+                        }
+                    ]
+                }
             }
         },
         "critical": {
             "critical.trapi.validation": {
-                "9.1.1": [
-                    {
-                        'component': 'Query',
-                        'reason': "Fire, Ambulance or Police?"
-                    }
-                ]
-
+                "global": {
+                    "9.1.1": [
+                        {
+                            'component': 'Query',
+                            'reason': "Fire, Ambulance or Police?"
+                        }
+                    ]
+                }
             }
         }
     }
     reporter1.add_messages(new_messages)
 
     # Verify what we have
-    messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter1.get_messages()
+    message_catalog: MESSAGE_CATALOG = reporter1.get_messages()
 
-    assert "information" in messages
-    assert len(messages['information']) > 0
+    assert "information" in message_catalog
+    assert len(message_catalog['information']) > 0
     information: List[str] = list()
-    for code, parameters in messages['information'].items():
-        information.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['information'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        information.append(value[0])
     assert "INFO - Excluded: All test case S-P-O triples from resource test location, " + \
            "or specific user excluded S-P-O triples" in information
 
-    assert "warnings" in messages
-    assert len(messages['warnings']) > 0
+    assert "warnings" in message_catalog
+    assert len(message_catalog['warnings']) > 0
     warnings: List[str] = list()
-    for code, parameters in messages['warnings'].items():
-        warnings.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['warnings'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        warnings.append(value[0])
     assert "WARNING - Knowledge Graph Node Id Unmapped: " + \
            "Node identifier found unmapped to target categories for node" in warnings
 
-    assert "errors" in messages
-    assert len(messages['errors']) > 0
+    assert "errors" in message_catalog
+    assert len(message_catalog['errors']) > 0
     errors: List[str] = list()
-    for code, parameters in messages['errors'].items():
-        errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['errors'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        errors.append(value[0])
     assert "ERROR - Biolink Model: S-P-O statement is not compliant to Biolink Model release" in errors
 
-    assert "critical" in messages
-    assert len(messages['critical']) > 0
+    assert "critical" in message_catalog
+    assert len(message_catalog['critical']) > 0
     critical: List[str] = list()
-    for code, parameters in messages['critical'].items():
-        critical.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['critical'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        critical.append(value[0])
     assert "CRITICAL - Trapi: Schema validation error" in critical
 
     obj = reporter1.to_dict()
     assert obj["trapi_version"] == TEST_TRAPI_VERSION
     assert obj["biolink_version"] == TEST_BIOLINK_VERSION
     assert "messages" in obj
     assert "critical" in obj["messages"]
     assert "critical.trapi.validation" in obj["messages"]["critical"]
-    messages: Optional[Dict[str, List[Dict[str, str]]]] = obj["messages"]["critical"]["critical.trapi.validation"]
-    assert messages, "Empty 'critical.trapi.validation' messages set?"
-    assert "9.1.1" in messages
-    message_subset: List = messages["9.1.1"]
+
+    message_catalog: SCOPED_MESSAGES = obj["messages"]["critical"]["critical.trapi.validation"]
+    assert message_catalog, "Empty 'critical.trapi.validation' messages set?"
+    assert "9.1.1" in message_catalog["global"]
+    message_subset: List = message_catalog["global"]["9.1.1"]
     assert "Fire, Ambulance or Police?"\
            in [message['reason'] for message in message_subset if 'reason' in message]
 
     for n in range(0, 10):
         reporter1.report(code="error.input_edge.node.category.missing", identifier=f"biolink:not_a_category_{n}")
 
     for c in range(0, 5):
@@ -369,15 +401,15 @@
         "ValidatorReporter.dump() resetting the title to a user string\n" +
         "and compressed using 'id_rows=1', 'msg_rows=1', 'compress=True':\n",
         file=stderr
     )
     reporter1.dump(title="My KP Validation Report", id_rows=1, msg_rows=1, compact_format=True, file=stderr)
 
     validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
-    assert validation_report.startswith("Critical:")
+    assert validation_report.startswith("Validation against TRAPI")
 
 
 def test_validator_method():
 
     reporter = ValidationReporter(
         prefix="Test Validator Method",
         trapi_version=TEST_TRAPI_VERSION,
@@ -403,28 +435,32 @@
         assert len(case) == 2
         assert case['some parameter'] == "some parameter value"
         assert case['another parameter'] == "some other parameter value"
         validator.report("warning.graph.empty", identifier="Fake")
 
     reporter.apply_validation(validator_method, test_data, **test_parameters)
 
-    messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter.get_messages()
+    message_catalog: MESSAGE_CATALOG = reporter.get_messages()
 
-    assert "warnings" in messages
-    assert len(messages['warnings']) > 0
+    assert "warnings" in message_catalog
+    assert len(message_catalog['warnings']) > 0
     warnings: List[str] = list()
-    for code, parameters in messages['warnings'].items():
-        warnings.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['warnings'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        warnings.append(value[0])
     assert "WARNING - Graph: Empty graph" in warnings
 
-    assert "errors" in messages
-    assert len(messages['errors']) > 0
+    assert "errors" in message_catalog
+    assert len(message_catalog['errors']) > 0
     errors: List[str] = list()
-    for code, parameters in messages['errors'].items():
-        errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    for code, messages in message_catalog['errors'].items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        errors.append(value[0])
     assert "ERROR - Knowledge Graph Edge Provenance Infores: " + \
            "Edge has provenance value which is not a well-formed InfoRes CURIE" in errors
 
 
 @pytest.mark.parametrize(
     "query",
     [
```

### Comparing `reasoner_validator-3.6.6/tests/test_workflows.py` & `reasoner_validator-3.7.0/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.6/PKG-INFO` & `reasoner_validator-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.6.6
+Version: 3.7.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -14,26 +14,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bmt (>=1.1.0,<2.0.0)
 Requires-Dist: fastapi (>=0.68,<0.69) ; extra == "web"
-Requires-Dist: jsonschema (>=4.17.0,<5.0.0)
+Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
 Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "dev"
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "dev"
+Requires-Dist: pytest (>=7.2.2,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.2.1,<2.0.0) ; extra == "docs"
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.15,<0.16) ; extra == "web"
 Project-URL: Bug Tracker, https://github.com/NCATSTranslator/reasoner-validator/issues
 Project-URL: Change Log, https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md
@@ -183,29 +182,29 @@
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
   "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
-  "sources": {
+  "target_provenance": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
-- An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
+- An **optional** `target_provenance` with an object dictionary (example shown) specifying the ARA and KP infores-specified knowledge sources expected to be recovered in the TRAPI query results (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "target_provenance" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
 First install the web-specific dependencies.
```

