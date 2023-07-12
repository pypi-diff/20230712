# Comparing `tmp/harmonydata-0.2.0.tar.gz` & `tmp/harmonydata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonydata-0.2.0.tar", last modified: Sat Jun 10 22:07:07 2023, max compression
+gzip compressed data, was "harmonydata-0.5.0.tar", last modified: Wed Jul 12 20:42:09 2023, max compression
```

## Comparing `harmonydata-0.2.0.tar` & `harmonydata-0.5.0.tar`

### file list

```diff
@@ -1,65 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-10 22:06:55.000000 harmonydata-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-10 22:06:55.000000 harmonydata-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-10 22:07:07.364794 harmonydata-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-10 22:06:55.000000 harmonydata-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-10 22:06:55.000000 harmonydata-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 22:07:07.364794 harmonydata-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-10 22:06:55.000000 harmonydata-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/matching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/default_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/excel_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/pdf_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/text_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_words.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/sequence_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/smart_document_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/excel_to_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/tika_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/wrapper_all_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/schemas/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/errors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/exceptions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/requests/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/responses/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/util/file_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmonydata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_excel_openpyxl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_excel_xlsxwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-12 20:41:59.000000 harmonydata-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 20:41:59.000000 harmonydata-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-12 20:42:09.906849 harmonydata-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-12 20:41:59.000000 harmonydata-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 20:41:59.000000 harmonydata-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 20:42:09.906849 harmonydata-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-12 20:41:59.000000 harmonydata-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117644 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/matching/default_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/matching/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/matching/negator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/excel_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/pdf_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/parsing/text_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/dictionary_options_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/ensemble_named_entity_recogniser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/options_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/options_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/rule_based_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/sequence_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/smart_document_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/smart_table_analyser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/spacy_ner_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_extraction/spacy_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/text_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/parsing/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/util/camelot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/util/excel_to_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/util/tesseract_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/util/tika_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/parsing/wrapper_all_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/schemas/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/enums/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/enums/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/schemas/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/errors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.902849 harmonydata-0.5.0/src/harmony/schemas/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/exceptions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/src/harmony/schemas/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/requests/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/src/harmony/schemas/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/responses/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/schemas/text_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/src/harmony/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/src/harmony/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/util/file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-12 20:41:59.000000 harmonydata-0.5.0/src/harmony/util/model_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/src/harmonydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-12 20:42:09.000000 harmonydata-0.5.0/src/harmonydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-12 20:42:09.000000 harmonydata-0.5.0/src/harmonydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:42:09.000000 harmonydata-0.5.0/src/harmonydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 20:42:09.000000 harmonydata-0.5.0/src/harmonydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:42:09.000000 harmonydata-0.5.0/src/harmonydata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:09.906849 harmonydata-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-12 20:41:59.000000 harmonydata-0.5.0/tests/test_convert_excel_openpyxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-12 20:41:59.000000 harmonydata-0.5.0/tests/test_convert_excel_xlsxwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-12 20:41:59.000000 harmonydata-0.5.0/tests/test_convert_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-12 20:41:59.000000 harmonydata-0.5.0/tests/test_convert_text.py
```

### Comparing `harmonydata-0.2.0/LICENSE` & `harmonydata-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/setup.py` & `harmonydata-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 import setuptools
 
-with open('README.md', 'r', encoding='utf-8') as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='harmonydata',
-    author='Thomas Wood',
-    author_email='thomas@fastdatascience.com',
-    description='Harmony Tool for Retrospective Data Harmonisation',
-    keywords='harmony, harmonisation, harmonization, harmonise, harmonize',
+    name="harmonydata",
+    author="Thomas Wood",
+    author_email="thomas@fastdatascience.com",
+    description="Harmony Tool for Retrospective Data Harmonisation",
+    keywords="harmony, harmonisation, harmonization, harmonise, harmonize",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/harmonydata/harmony',
+    long_description_content_type="text/markdown",
+    url="https://github.com/harmonydata/harmony",
     project_urls={
-        'Documentation': 'https://harmonydata.org/',
-        'Bug Reports':
-        'https://github.com/harmonydata/harmony/issues',
-        'Source Code': 'https://github.com/harmonydata/harmony',
+        "Documentation": "https://harmonydata.org/",
+        "Bug Reports": "https://github.com/harmonydata/harmony/issues",
+        "Source Code": "https://github.com/harmonydata/harmony",
         # 'Funding': '',
         # 'Say Thanks!': '',
     },
-    package_dir={'': 'src'},
-    packages=setuptools.find_packages(where='src'),
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     classifiers=[
         # see https://pypi.org/classifiers/
-        'Development Status :: 5 - Production/Stable',
-
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3 :: Only',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.6",
+    install_requires=[
+        "pydantic==1.10.7",
+        "pandas==2.0.0",
+        "tika==2.6.0",
+        "lxml==4.9.2",
+        "langdetect==1.0.9",
+        "XlsxWriter==3.0.9",
+        "openpyxl==3.1.2",
+        "spacy==3.5.3",
+        "wget==3.2",
     ],
-    python_requires='>=3.6',
-    install_requires=['pydantic==1.10.7','pandas==2.0.0','tika==2.6.0','lxml==4.9.2','langdetect==1.0.9','XlsxWriter==3.0.9','openpyxl==3.1.2','spacy==3.5.3'],
     extras_require={
-        'dev': ['check-manifest'],
+        "dev": ["check-manifest"],
         # 'test': ['coverage'],
     },
     # entry_points={
     #     'console_scripts': [  # This can provide executable scripts
     #         'run=examplepy:main',
     # You can execute `run` in bash to run `main()` in src/examplepy/__init__.py
     #     ],
```

### Comparing `harmonydata-0.2.0/src/harmony/__init__.py` & `harmonydata-0.5.0/src/harmony/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-__version__ = "0.2.0"
+__version__ = "0.5.0"
 
 # TODO: make these configurable at package level
 import os
-from .parsing.text_parser import convert_text_to_instruments
-from .parsing.excel_parser import convert_excel_to_instruments
-from .parsing.pdf_parser import convert_pdf_to_instruments
-from .parsing.wrapper_all_parsers import convert_files_to_instruments
-from .parsing import *
 from .schemas import *
-from .matching.matcher import match_instruments_with_function
-try:
-    from .matching.default_matcher import match_instruments
-except:
-    print ("Warning: transformers not available. To use transformers, run pip install sentence-transformers")
+from .examples import example_instruments
+from .util.model_downloader import download_models
 
-from .util.file_helper import load_instruments_from_local_file
+if os.environ.get("HARMONY_NO_PARSING") is None or os.environ.get("HARMONY_NO_PARSING") == "":
+    from .parsing.text_parser import convert_text_to_instruments
+    from .parsing.excel_parser import convert_excel_to_instruments
+    from .parsing.pdf_parser import convert_pdf_to_instruments
+    from .parsing.wrapper_all_parsers import convert_files_to_instruments
+    from .parsing import *
+    from .util.file_helper import load_instruments_from_local_file
+
+if os.environ.get("HARMONY_NO_MATCHING") is None or os.environ.get("HARMONY_NO_MATCHING") == "":
+    from .matching.matcher import match_instruments_with_function
+    try:
+        from .matching.default_matcher import match_instruments
+    except:
+        print ("Warning: transformers not available. To use transformers, run pip install sentence-transformers")
```

### Comparing `harmonydata-0.2.0/src/harmony/parsing/excel_parser.py` & `harmonydata-0.5.0/src/harmony/parsing/excel_parser.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_extractor.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/options_extractor.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_words.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/options_words.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 OPTIONS_WORDS = {'attractive', 'sometimes', 'some or a little of the time', 'true', 'some times', 'not at all', 'none',
-                  'somewhat true', 'not likely', 'often', 'cinco vezes', 'very likely', 'igual',
-                  'algumas vezes verdadeira', 'very easy', 'tanto quanto sabe', 'totally',
-                  'occasionally or a moderate amount of time', 'um pouco', 'extremamente', 'neither agree nor disagree',
-                  'unattractive', 'always', 'a lot', 'some of the time', 'mais ou menos verdadeiro', 'sim',
-                  'unappealing', 'raramente', 'concordo totalmente', 'totalmente de acordo', 'provavelmente não', 'não',
-                  '1-5 meses', 'fair', 'sempre', 'uma vez', 'às vezes', 'rarely', 'extremely difficult',
-                  'discordo totalmente', 'dificuldades graves', 'probably not', 'abaixo da média exigida pela escola',
-                  'neither likely nor unlikely', 'yes', 'nada', "i don't like it at all", 'limited a little', 'melhor',
-                  'não concordo nem discordo', 'mais que muito', 'probably', 'mais ou menos', 'strongly agree',
-                  'frequentemente', 'totally agree', 'insuficiente', 'mais de 1 ano', 'não gosto nada', 'very',
-                  'likely', 'not likely at all', 'concordo parcialmente', 'all of the time', 'extremely',
-                  'very important', 'strongly disagree', 'disagree slightly', 'none of these', 'uma pouco',
-                  'menos de 1 mês', 'duas vezes', 'more than half the days', 'disagree', 'excellent',
-                  'none of the time', 'not limited at all', 'uma pouco verdadeira', 'pior', 'poor', 'não sei',
-                  'agree strongly', 'falso', 'rarely or none of the time', 'muito', 'nunca', 'limited a lot',
-                  'somewhat appealing', 'verdade', 'certainly true', 'daily', 'not difficult at all', 'appealing',
-                  'somewhat disagree', 'quatro vezes', 'verdadeiro', 'disagree strongly', 'agree', 'several days',
-                  'não sabe', 'most of the time', '6-12 meses', 'discordo parcialmente', 'provavelmente',
-                  'a moderate amount of time', 'neither agree or disagree', 'about the same',
-                  'muitas vezes ou quase sempre', 'neutral', 'não sabe/não se aplica', 'difficult', 'never',
-                  'most or all of the time', 'a little', 'agree slightly', 'very appealing',
-                  'neither easy nor difficult', 'very good', 'não é verdadeito', 'pequenas dificuldades',
-                  'very difficult', 'mais de cinco vezes', 'dificuldades bem definidas', 'algumas vezes', 'definitely',
-                  'três vezes', 'nearly every day', 'good', 'no', 'not true', 'nunca ou raramente',
-                  'muito verdadeira ou frequentemente verdadeira', 'não é verdade', 'claro que compraria',
-                  'somewhat agree', 'easy'}
+                 'somewhat true', 'not likely', 'often', 'cinco vezes', 'very likely', 'igual',
+                 'algumas vezes verdadeira', 'very easy', 'tanto quanto sabe', 'totally',
+                 'occasionally or a moderate amount of time', 'um pouco', 'extremamente', 'neither agree nor disagree',
+                 'unattractive', 'always', 'a lot', 'some of the time', 'mais ou menos verdadeiro', 'sim',
+                 'unappealing', 'raramente', 'concordo totalmente', 'totalmente de acordo', 'provavelmente não', 'não',
+                 '1-5 meses', 'fair', 'sempre', 'uma vez', 'às vezes', 'rarely', 'extremely difficult',
+                 'discordo totalmente', 'dificuldades graves', 'probably not', 'abaixo da média exigida pela escola',
+                 'neither likely nor unlikely', 'yes', 'nada', "i don't like it at all", 'limited a little', 'melhor',
+                 'não concordo nem discordo', 'mais que muito', 'probably', 'mais ou menos', 'strongly agree',
+                 'frequentemente', 'totally agree', 'insuficiente', 'mais de 1 ano', 'não gosto nada', 'very',
+                 'likely', 'not likely at all', 'concordo parcialmente', 'all of the time', 'extremely',
+                 'very important', 'strongly disagree', 'disagree slightly', 'none of these', 'uma pouco',
+                 'menos de 1 mês', 'duas vezes', 'more than half the days', 'disagree', 'excellent',
+                 'none of the time', 'not limited at all', 'uma pouco verdadeira', 'pior', 'poor', 'não sei',
+                 'agree strongly', 'falso', 'rarely or none of the time', 'muito', 'nunca', 'limited a lot',
+                 'somewhat appealing', 'verdade', 'certainly true', 'daily', 'not difficult at all', 'appealing',
+                 'somewhat disagree', 'quatro vezes', 'verdadeiro', 'disagree strongly', 'agree', 'several days',
+                 'não sabe', 'most of the time', '6-12 meses', 'discordo parcialmente', 'provavelmente',
+                 'a moderate amount of time', 'neither agree or disagree', 'about the same',
+                 'muitas vezes ou quase sempre', 'neutral', 'não sabe/não se aplica', 'difficult', 'never',
+                 'most or all of the time', 'a little', 'agree slightly', 'very appealing',
+                 'neither easy nor difficult', 'very good', 'não é verdadeito', 'pequenas dificuldades',
+                 'very difficult', 'mais de cinco vezes', 'dificuldades bem definidas', 'algumas vezes', 'definitely',
+                 'três vezes', 'nearly every day', 'good', 'no', 'not true', 'nunca ou raramente',
+                 'muito verdadeira ou frequentemente verdadeira', 'não é verdade', 'claro que compraria',
+                 'somewhat agree', 'easy', "most days",
+                 "at least once a week",
+                 "at least once a month",
+                 "several times a year",
+                 "once a year or less",
+                 "never or almost never",
+                 "some days, but not all days",
+                 "every day",
+                 "more than once a day",
+                 "once a day",
+                 "less often but at least once a month",
+                 "less than once a month",
+                 "very confident",
+                 "slightly confident",
+                 "not at all confident",
+                 "very true",
+                 "partly true",
+                 "not true at all",
+                 "other", }
```

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/sequence_finder.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/sequence_finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 previous_idx, previous_seq_type, previous_value = test_sequence[-1]
                 # and value in (previous_value, previous_value + 1) \
                 if previous_seq_type == seq_type \
                         and bullet_texts[idx] != bullet_texts[previous_idx]:
                     candidate_sequences.append(test_sequence)
 
             if len(candidate_sequences) > 0:
-                sequence_to_append_to = sorted(candidate_sequences, key=lambda s: len(s), reverse=True)[0]
+                sequence_to_append_to = sorted(candidate_sequences, key=lambda s: len(s) + s[-1][0] / 1000, reverse=True)[0]
             else:
                 sequence_to_append_to = []
                 running_sequences.append(sequence_to_append_to)
             sequence_to_append_to.append((idx, seq_type, value))
 
     if len(running_sequences) > 0:
         sequences_long_to_short = sorted(running_sequences, key=lambda s: len(s), reverse=True)
```

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/smart_document_parser.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/smart_document_parser.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_wrapper.py` & `harmonydata-0.5.0/src/harmony/parsing/text_extraction/spacy_wrapper.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/text_parser.py` & `harmonydata-0.5.0/src/harmony/parsing/text_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import traceback
 from typing import List
 
 from langdetect import detect
 
-from harmony.parsing.text_extraction.smart_document_parser import parse_document
+from harmony.parsing.text_extraction.ensemble_named_entity_recogniser import extract_questions
 from harmony.schemas.enums.file_types import FileType
 from harmony.schemas.requests.text import RawFile, Instrument, Question
 
 
 def convert_text_to_instruments(file: RawFile) -> List[Instrument]:
     if file.file_type == FileType.txt:
         page_text = file.content
@@ -33,15 +33,15 @@
             if line.strip() == "":
                 continue
             line = re.sub(r'\s+', ' ', line)
             question = Question(question_no=len(questions) + 1, question_intro="", question_text=line.strip(),
                                 options=[])
             questions.append(question)
     else:
-        questions = parse_document(page_text)
+        questions, _, _ = extract_questions(page_text, file.tables)
 
     instrument = Instrument(
         file_id=file.file_id,
         instrument_id=file.file_id + "_0",
         instrument_name=file.file_name,
         file_name=file.file_name,
         file_type=file.file_type,
```

### Comparing `harmonydata-0.2.0/src/harmony/parsing/util/excel_to_pandas.py` & `harmonydata-0.5.0/src/harmony/parsing/util/excel_to_pandas.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/parsing/util/tika_wrapper.py` & `harmonydata-0.5.0/src/harmony/parsing/util/tika_wrapper.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/schemas/enums/languages.py` & `harmonydata-0.5.0/src/harmony/schemas/enums/languages.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/schemas/errors/base.py` & `harmonydata-0.5.0/src/harmony/schemas/errors/base.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/schemas/exceptions/base.py` & `harmonydata-0.5.0/src/harmony/schemas/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/src/harmony/schemas/requests/text.py` & `harmonydata-0.5.0/src/harmony/schemas/requests/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class RawFile(BaseModel):
     file_id: str = Field(None, description="Unique identifier for the file (UUID-4)")
     file_name: str = Field("Untitled file", description="The name of the input file")
     file_type: FileType = Field(description="The file type (pdf, xlsx, txt)")
     content: str = Field(description="The raw file contents")
     text_content: str = Field(None, description="The plain text content")
+    tables: list = Field([], description="The tables in the file")
 
     class Config:
         schema_extra = {
             "example": {
                 "file_id": "d39f31718513413fbfc620c6b6135d0c",
                 "file_name": "GAD-7.pdf",
                 "file_type": "pdf",
```

### Comparing `harmonydata-0.2.0/src/harmony/util/file_helper.py` & `harmonydata-0.5.0/src/harmony/util/file_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 
 def load_instruments_from_local_file(file_name: str) -> List[Instrument]:
     if file_name.lower().endswith("pdf"):
         file_type = "pdf"
     elif file_name.lower().endswith("xlsx"):
         file_type = "xlsx"
+    elif file_name.lower().endswith("docx"):
+        file_type = "docx"
     else:
         file_type = "txt"
 
-    if file_type == "pdf" or file_type == "xlsx":
+    if file_type == "pdf" or file_type == "xlsx" or file_type == "docx":
         with open(
                 file_name,
                 "rb") as f:
             file_as_bytes = f.read()
 
         file_as_base64 = base64.b64encode(file_as_bytes).decode('ascii')
```

### Comparing `harmonydata-0.2.0/src/harmonydata.egg-info/SOURCES.txt` & `harmonydata-0.5.0/src/harmonydata.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/harmony/__init__.py
+src/harmony/examples.py
 src/harmony/matching/__init__.py
 src/harmony/matching/default_matcher.py
 src/harmony/matching/matcher.py
+src/harmony/matching/negator.py
 src/harmony/parsing/__init__.py
 src/harmony/parsing/excel_parser.py
 src/harmony/parsing/pdf_parser.py
 src/harmony/parsing/text_parser.py
 src/harmony/parsing/wrapper_all_parsers.py
 src/harmony/parsing/text_extraction/__init__.py
+src/harmony/parsing/text_extraction/dictionary_options_matcher.py
+src/harmony/parsing/text_extraction/ensemble_named_entity_recogniser.py
 src/harmony/parsing/text_extraction/options_extractor.py
 src/harmony/parsing/text_extraction/options_words.py
+src/harmony/parsing/text_extraction/rule_based_extractor.py
 src/harmony/parsing/text_extraction/sequence_finder.py
 src/harmony/parsing/text_extraction/smart_document_parser.py
+src/harmony/parsing/text_extraction/smart_table_analyser.py
+src/harmony/parsing/text_extraction/spacy_ner_extractor.py
 src/harmony/parsing/text_extraction/spacy_options_matcher.py
 src/harmony/parsing/text_extraction/spacy_wrapper.py
 src/harmony/parsing/util/__init__.py
+src/harmony/parsing/util/camelot_wrapper.py
 src/harmony/parsing/util/excel_to_pandas.py
+src/harmony/parsing/util/tesseract_wrapper.py
 src/harmony/parsing/util/tika_wrapper.py
 src/harmony/schemas/__init__.py
+src/harmony/schemas/text_vector.py
 src/harmony/schemas/enums/__init__.py
 src/harmony/schemas/enums/file_types.py
 src/harmony/schemas/enums/languages.py
 src/harmony/schemas/errors/__init__.py
 src/harmony/schemas/errors/base.py
 src/harmony/schemas/exceptions/__init__.py
 src/harmony/schemas/exceptions/base.py
 src/harmony/schemas/requests/__init__.py
 src/harmony/schemas/requests/text.py
 src/harmony/schemas/responses/__init__.py
 src/harmony/schemas/responses/text.py
+src/harmony/services/__init__.py
 src/harmony/util/__init__.py
 src/harmony/util/file_helper.py
+src/harmony/util/model_downloader.py
 src/harmonydata.egg-info/PKG-INFO
 src/harmonydata.egg-info/SOURCES.txt
 src/harmonydata.egg-info/dependency_links.txt
 src/harmonydata.egg-info/requires.txt
 src/harmonydata.egg-info/top_level.txt
 tests/test_convert_excel_openpyxl.py
 tests/test_convert_excel_xlsxwriter.py
```

### Comparing `harmonydata-0.2.0/tests/test_convert_excel_openpyxl.py` & `harmonydata-0.5.0/tests/test_convert_excel_openpyxl.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/tests/test_convert_excel_xlsxwriter.py` & `harmonydata-0.5.0/tests/test_convert_excel_xlsxwriter.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.2.0/tests/test_convert_pdf.py` & `harmonydata-0.5.0/tests/test_convert_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import unittest
 
 from harmony import convert_pdf_to_instruments
 from harmony.schemas.requests.text import RawFile
+from harmony import download_models
 
 pdf_gad_7_2_questions = RawFile.parse_obj({
     "file_id": "d39f31718513413fbfc620c6b6135d0c",
     "file_name": "GAD-7.pdf",
     "file_type": "pdf",
     "content": "data:application/pdf;base64,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ZXJpZgovQ0lEU3lzdGVtSW5mbyA8PCAvUmVnaXN0cnkgKEFkb2JlKSAvT3JkZXJpbmcgKElkZW50aXR5KSAvU3VwcGxlbWVudCAwID4+Ci9Gb250RGVzY3JpcHRvciAxMiAwIFIKL0NJRFRvR0lETWFwIC9JZGVudGl0eQovVyBbMCBbNjAwIDYzNiAzMTggMzE4IDY5NCA1OTIgMzIwIDMyMCA2NDQgNjQwIDQ3OCA1NjUgNjAyIDY0NCA1MTMgMzE4IDU5NiA1NjQgNjQwIDYzNiA4NzUgNDAyIDY0MCA2NDAgNTYwIDg1NiA1NjUgXQpdCj4+CmVuZG9iagoxNSAwIG9iago8PCAvTGVuZ3RoIDU0NiA+PgpzdHJlYW0KL0NJREluaXQgL1Byb2NTZXQgZmluZHJlc291cmNlIGJlZ2luCjEyIGRpY3QgYmVnaW4KYmVnaW5jbWFwCi9DSURTeXN0ZW1JbmZvIDw8IC9SZWdpc3RyeSAoQWRvYmUpIC9PcmRlcmluZyAoVUNTKSAvU3VwcGxlbWVudCAwID4+IGRlZgovQ01hcE5hbWUgL0Fkb2JlLUlkZW50aXR5LVVDUyBkZWYKL0NNYXBUeXBlIDIgZGVmCjEgYmVnaW5jb2Rlc3BhY2VyYW5nZQo8MDAwMD4gPEZGRkY+CmVuZGNvZGVzcGFjZXJhbmdlCjIgYmVnaW5iZnJhbmdlCjwwMDAwPiA8MDAwMD4gPDAwMDA+CjwwMDAxPiA8MDAxQT4gWzwwMDMxPiA8MDAyRT4gPDAwMDk+IDwwMDQ2PiA8MDA2NT4gPDAwNkM+IDwwMDY5PiA8MDA2RT4gPDAwNjc+IDwwMDcyPiA8MDA3Nj4gPDAwNkY+IDwwMDc1PiA8MDA3Mz4gPDAwMkM+IDwwMDYxPiA8MDA3OD4gPDAwNjQ+IDwwMDMyPiA8MDA0RT4gPDAwNzQ+IDwwMDYyPiA8MDA3MD4gPDAwNjM+IDwwMDc3PiA8MDA3OT4gXQplbmRiZnJhbmdlCmVuZGNtYXAKQ01hcE5hbWUgY3VycmVudGRpY3QgL0NNYXAgZGVmaW5lcmVzb3VyY2UgcG9wCmVuZAplbmQKCmVuZHN0cmVhbQplbmRvYmoKNyAwIG9iago8PCAvVHlwZSAvRm9udAovU3VidHlwZSAvVHlwZTAKL0Jhc2VGb250IC9EZWphVnVTZXJpZgovRW5jb2RpbmcgL0lkZW50aXR5LUgKL0Rlc2NlbmRhbnRGb250cyBbMTQgMCBSXQovVG9Vbmljb2RlIDE1IDAgUj4+CmVuZG9iagoxNiAwIG9iago8PAovTGVuZ3RoIDQKPj4Kc3RyZWFtCv///+AKZW5kc3RyZWFtCmVuZG9iagozIDAgb2JqCjw8Ci9UeXBlIC9QYWdlcwovS2lkcyAKWwo2IDAgUgpdCi9Db3VudCAxCi9Qcm9jU2V0IFsvUERGIC9UZXh0IC9JbWFnZUIgL0ltYWdlQ10KPj4KZW5kb2JqCnhyZWYKMCAxOAowMDAwMDAwMDAwIDY1NTM1IGYgCjAwMDAwMDAwMTUgMDAwMDAgbiAKMDAwMDAwMDE2OSAwMDAwMCBuIAowMDAwMDA4MjQzIDAwMDAwIG4gCjAwMDAwMDAyMTggMDAwMDAgbiAKMDAwMDAwMDMxMyAwMDAwMCBuIAowMDAwMDAwMzUwIDAwMDAwIG4gCjAwMDAwMDgwNTIgMDAwMDAgbiAKMDAwMDAwMDY3MCAwMDAwMCBuIAowMDAwMDAxMjQ0IDAwMDAwIG4gCjAwMDAwMDA0ODQgMDAwMDAgbiAKMDAwMDAwMDY1MCAwMDAwMCBuIAowMDAwMDAxMjYzIDAwMDAwIG4gCjAwMDAwMDE1MzkgMDAwMDAgbiAKMDAwMDAwNzEzNSAwMDAwMCBuIAowMDAwMDA3NDU0IDAwMDAwIG4gCjAwMDAwMDgxODkgMDAwMDAgbiAKMDAwMDAwNzExNCAwMDAwMCBuIAp0cmFpbGVyCjw8Ci9TaXplIDE4IAovSW5mbyAxIDAgUgovUm9vdCAyIDAgUgo+PgpzdGFydHhyZWYKODM0MSAKJSVFT0YK"
 })
 
+download_models()
 
 class TestConvertPdf(unittest.TestCase):
 
     def test_single_instrument(self):
         self.assertEqual(1, len(convert_pdf_to_instruments(pdf_gad_7_2_questions)))
 
     def test_two_questions(self):
```

### Comparing `harmonydata-0.2.0/tests/test_convert_text.py` & `harmonydata-0.5.0/tests/test_convert_text.py`

 * *Files identical despite different names*

