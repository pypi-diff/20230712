# Comparing `tmp/re_action_template-2.1.1-py3-none-any.whl.zip` & `tmp/re_action_template-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 14539 bytes, number of entries: 8
+Zip file size: 14523 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 action_template/__init__.py
 -rwxr-xr-x  2.0 unx      156 b- defN 80-Jan-01 00:00 action_template/__main__.py
 -rw-r--r--  2.0 unx     2259 b- defN 80-Jan-01 00:00 action_template/main.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4348 b- defN 80-Jan-01 00:00 re_action_template-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.1.1.dist-info/RECORD
-8 files, 38188 bytes uncompressed, 13321 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4308 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.1.2.dist-info/RECORD
+8 files, 38148 bytes uncompressed, 13305 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: action_template/__main__.py
 Comment: 
 
 Filename: action_template/main.py
 Comment: 
 
-Filename: re_action_template-2.1.1.dist-info/LICENSE
+Filename: re_action_template-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: re_action_template-2.1.1.dist-info/METADATA
+Filename: re_action_template-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: re_action_template-2.1.1.dist-info/WHEEL
+Filename: re_action_template-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: re_action_template-2.1.1.dist-info/entry_points.txt
+Filename: re_action_template-2.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_action_template-2.1.1.dist-info/RECORD
+Filename: re_action_template-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_action_template-2.1.1.dist-info/LICENSE` & `re_action_template-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_action_template-2.1.1.dist-info/METADATA` & `re_action_template-2.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-action-template
-Version: 2.1.1
+Version: 2.1.2
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -25,52 +25,47 @@
 `action-template` runs the Jinja2 templating engine against any given files during a GitHub workflow, and makes the GitHub context available to it.
 
 ## Usage
 
 action-template can be used as a GitHub Action;
 
 ```yml
-name: Generate README.md
+name: Sample Workflow
 
 on:
   push:
     branches:
       - master
-    paths:
-      - 'README.md.template'
-  workflow_dispatch:
-
-defaults:
-  run:
-    shell: bash --login {0}
 
 permissions:
   contents: write
 
 jobs:
-  run-templating:
+  templating:
     runs-on: ubuntu-latest
     steps:
-      - uses: release-engineers/action-setup-bash@v1
       - uses: actions/checkout@v3
+        with:
+          ref: master
       - uses: release-engineers/action-template@v2
         with:
           source: 'README.md.template'
           target: 'README.md'
-      - run: |
-          git config --global user.name "github-actions[bot]"
-          git config --global user.email "github-actions[bot]@users.noreply.github.com"
+      - shell: bash
+        run: |
+          git config --global --add safe.directory '*'
+          git config --local user.name 'github-actions[bot]'
+          git config --local user.email 'github-actions[bot]@users.noreply.github.com'
           git add README.md
-          git commit --no-verify -m "docs: Regenerate README.md"
-          
-          # rebase and push in a retry loop
-          for i in {1..5}; do
-            git pull --rebase && git push && break || sleep 1
-          done
-
+          if git commit --no-verify -m "docs: Regenerate README.md"; then
+            # rebase and push in a retry loop
+            for i in {1..5}; do
+              git pull --rebase && git push && break || sleep 1
+            done
+          fi
 ```
 
 ## Features
 
 ### GitHub Context
 
 The GitHub context available to workflows is also available to templates like so;
```

### html2text {}

```diff
@@ -1,39 +1,38 @@
-Metadata-Version: 2.1 Name: re-action-template Version: 2.1.1 Summary: License:
+Metadata-Version: 2.1 Name: re-action-template Version: 2.1.2 Summary: License:
 SSPL-1.0 Author: Philipp Gayret Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: Markdown (>=3.3.6,<4.0.0) Requires-
 Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: jinja2 (>=3.0.3,<4.0.0) Requires-
 Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown  # release-
 engineers/action-template [![Status: Production ready](https://img.shields.io/
 badge/status-production_ready-green)](https://release-engineers.com/open-
 source-badges/) [![PyPI version](https://badge.fury.io/py/re-action-
 template.svg)](https://badge.fury.io/py/re-action-template) `action-template`
 runs the Jinja2 templating engine against any given files during a GitHub
 workflow, and makes the GitHub context available to it. ## Usage action-
-template can be used as a GitHub Action; ```yml name: Generate README.md on:
-push: branches: - master paths: - 'README.md.template' workflow_dispatch:
-defaults: run: shell: bash --login {0} permissions: contents: write jobs: run-
-templating: runs-on: ubuntu-latest steps: - uses: release-engineers/action-
-setup-bash@v1 - uses: actions/checkout@v3 - uses: release-engineers/action-
-template@v2 with: source: 'README.md.template' target: 'README.md' - run: | git
-config --global user.name "github-actions[bot]" git config --global user.email
-"github-actions[bot]@users.noreply.github.com" git add README.md git commit --
-no-verify -m "docs: Regenerate README.md" # rebase and push in a retry loop for
-i in {1..5}; do git pull --rebase && git push && break || sleep 1 done ``` ##
-Features ### GitHub Context The GitHub context available to workflows is also
-available to templates like so; ``` {{ github.repository }} ``` When evaluated
-becomes: ``` release-engineers/action-template ``` ### Load Files The example
-workflow under the Usage paragraph was loaded using; ```yml {{ load('.github/
-workflows/example.yml') }} ``` ### Load JSON Parse and handle JSON data from
-files in the working directory like so; ``` {{ load_json('tests/data/
-data.json').info.from_json }} ``` When evaluated becomes: ``` This text is a
-JSON value in a file. ``` ### Load YAML Parse and handle YAML data from files
-in the working directory like so; ``` {{ load_yaml('tests/data/
+template can be used as a GitHub Action; ```yml name: Sample Workflow on: push:
+branches: - master permissions: contents: write jobs: templating: runs-on:
+ubuntu-latest steps: - uses: actions/checkout@v3 with: ref: master - uses:
+release-engineers/action-template@v2 with: source: 'README.md.template' target:
+'README.md' - shell: bash run: | git config --global --add safe.directory '*'
+git config --local user.name 'github-actions[bot]' git config --local
+user.email 'github-actions[bot]@users.noreply.github.com' git add README.md if
+git commit --no-verify -m "docs: Regenerate README.md"; then # rebase and push
+in a retry loop for i in {1..5}; do git pull --rebase && git push && break ||
+sleep 1 done fi ``` ## Features ### GitHub Context The GitHub context available
+to workflows is also available to templates like so; ``` {{ github.repository
+}} ``` When evaluated becomes: ``` release-engineers/action-template ``` ###
+Load Files The example workflow under the Usage paragraph was loaded using;
+```yml {{ load('.github/workflows/example.yml') }} ``` ### Load JSON Parse and
+handle JSON data from files in the working directory like so; ``` {{ load_json
+('tests/data/data.json').info.from_json }} ``` When evaluated becomes: ``` This
+text is a JSON value in a file. ``` ### Load YAML Parse and handle YAML data
+from files in the working directory like so; ``` {{ load_yaml('tests/data/
 data.yml').info.from_yaml }} ``` When evaluated becomes: ``` This text is a
 YAML value in a file ``` ### Load Markdown Table of Contents as HTML Parse and
 obtain a Markdown table of contents from files in the working directory like
 so; ``` {{ load_markdown_toc('tests/data/data.md') }} ``` When evaluated
 becomes: ```
     * Header_One
           o Header_Two
```

## Comparing `re_action_template-2.1.1.dist-info/RECORD` & `re_action_template-2.1.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 action_template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 action_template/__main__.py,sha256=L--CQs0rPatHtlKm0clm-1TxXD5DXPSAoFsTyrnk28A,156
 action_template/main.py,sha256=t9FPEE3g_69sgo-s5tjKUcYxBj7Ez-Z2IrypGy95Egg,2259
-re_action_template-2.1.1.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
-re_action_template-2.1.1.dist-info/METADATA,sha256=zMXpzoCL_71GAd42ZNTu8Jw44jlMro-ITbdWSkYIZAs,4348
-re_action_template-2.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-re_action_template-2.1.1.dist-info/entry_points.txt,sha256=DbdYeQoeg8Pnk2GzJr9LUgK9nDHUnNIpyxZVPMByx3c,65
-re_action_template-2.1.1.dist-info/RECORD,,
+re_action_template-2.1.2.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
+re_action_template-2.1.2.dist-info/METADATA,sha256=9ItD8HgQuxzVl3LdU6Ad9V7eqEJtyJiTKmpnbxZmz3k,4308
+re_action_template-2.1.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+re_action_template-2.1.2.dist-info/entry_points.txt,sha256=DbdYeQoeg8Pnk2GzJr9LUgK9nDHUnNIpyxZVPMByx3c,65
+re_action_template-2.1.2.dist-info/RECORD,,
```

