# Comparing `tmp/wasc-0.4.0.tar.gz` & `tmp/wasc-1.0.0.tar.gz`

## Comparing `wasc-0.4.0.tar` & `wasc-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 wasc-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 wasc-0.4.0/requirements_dev.txt
--rw-r--r--   0        0        0    61569 2020-02-02 00:00:00.000000 wasc-0.4.0/test_culture.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wasc-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wasc-0.4.0/data/checkers.csv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.4.0/data/example_websites.csv
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 wasc-0.4.0/data/sub_list.csv
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/checkers.md
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/index.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/license.md
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 wasc-0.4.0/docs/releases.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/__main__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/abstract_checker.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/checker_factory.py
--rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/checkers.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/utils.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 wasc-0.4.0/src/wasc/cli/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_checker.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_checker_factory.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/data/checkers_example.csv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.4.0/tests/data/url_example.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wasc-0.4.0/.gitignore
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 wasc-0.4.0/README.md
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 wasc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 wasc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 wasc-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 wasc-1.0.0/requirements_dev.txt
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wasc-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 wasc-1.0.0/data/checkers.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-1.0.0/data/example_websites.csv
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wasc-1.0.0/docs/checkers.md
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 wasc-1.0.0/docs/index.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 wasc-1.0.0/docs/license.md
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 wasc-1.0.0/docs/releases.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/__main__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/abstract_checker.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/checker_factory.py
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/checkers.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/utils.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 wasc-1.0.0/src/wasc/cli/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/test_checker.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/test_checker_factory.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/data/checkers_example.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-1.0.0/tests/data/url_example.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wasc-1.0.0/.gitignore
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 wasc-1.0.0/README.md
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 wasc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 wasc-1.0.0/PKG-INFO
```

### Comparing `wasc-0.4.0/.github/workflows/docs.yml` & `wasc-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `wasc-0.4.0/docs/checkers.md` & `wasc-1.0.0/docs/checkers.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,68 @@
-# Checkers
-
-Wasc contains already defined checkers in `default_chekers.py`.
+Wasc contains already defined checkers in `chekers.py`.
 
 All checkers return `"échec"` on failure.
 
-Default checkers are listed below with their definition.
+Available checkers are listed below with their definition.
+
+- [`AccessChecker`](#accesschecker)
+- [`AccessLinkChecker`](#accesslinkchecker)
+- [`AccessRateChecker`](#accessratechecker)
+- [`ContactLinkChecker`](#contactlinkchecker)
+- [`DoctypeChecker`](#doctypechecker)
+- [`FooterChecker`](#footerchecker)
+- [`HeaderChecker`](#headerchecker)
+- [`HeadLvlChecker`](#headlvlchecker)
+- [`HeaderNbChecker`](#headernbchecker)
+- [`LangChecker`](#langchecker)
+- [`LegalChecker`](#legalchecker)
+
+## `AccessChecker`
+* Rule: `"Accessibilité : XX conforme"` exists in the page with `XX` in `["non", "partiellement", "totalement"]`
+* Rule: Search in `<footer>`, then `<div id="footer>`, then the whole page
+* Return: `XX conforme`
+
+## `AccessLinkChecker`
+* Rule: if `AccessChecker` is valid and it's a link returns it
+* Rule: if the previous rule fails, check each link in the page looking `accessibilit` in the text inside `<a>`
+* Rule: if the previous rule fails, check each link in the page looking `accessibilit` in the `href` attribute
+* Return: the link url
+
+## `AccessRateChecker`
+* Rule: if `AccessLinkChecker` is valid, get the page from the link.
+* Rule: the accessibility rate is in a tag containing "conformité" and a floating number directly followed by '%'
+* Return: the accessibility rate
+
+## `ContactLinkChecker`
+* Rule: Finds `contact` or `ecrire` in a link `<a>` tag
+* Return: the link url
 
 ## `DoctypeChecker`
 * Rule: the HTML document contains `<!DOCTYPE html>`
 * Rule: `<!DOCTYPE html>` is before `<html>`
 * Return: `html`
 
+## `FooterChecker`
+* Rule: the HTML document contains `<footer>`
+* Return: `présent` if the tag is found, else `échec`
+
+## `HeaderChecker`
+* Rule: the HTML document contains `<header>`
+* Return: `présent` if the tag is found, else `échec`
+
+## `HeadLvlChecker`
+* Rule: For each `<head>` tags in the page, calculate its depth
+* Return: the list of depth of `<head>` tags 
+
+## `HeaderNbChecker`
+* Rule: the HTML document contains `<head>`
+* Return: the number of `<head>` tags present on the page
+
 ## `LangChecker`
 * Rule: `<html>` has an attribute `lang`
 * Return: the value of `lang`
 
 ## `LegalChecker`
 * Rule: `"Mentions légales"` exists somewhere in the page
 * Rule: `"Mentions légales"` is a link `<a>` with attribute `href`
 * Return: the value of `href`
 
-## `AccessChecker`
-* Rule: `"Accessibilité : XX conforme"` exists somewhere in the page with `XX` in `["non", "partiellement", "totalement"]`
-* Return: `XX conforme`
-
-## `AccessLinkChecker`
-* Rule: if `AccessChecker` is valid, then if it's a link
-* Rule: if the previous rule fails, check each link in the page looking for keyword `accessibilite` at the end of URL
-* Return: the value of the link
-
-## `AccessRateChecker` (Todo)
-* Rule: if `AccessLinkChecker` is valid, get the page from the link. In this page, an accessibility rate is given as percent
-* Return: the accessibility rate
```

#### html2text {}

```diff
@@ -1,17 +1,28 @@
-# Checkers Wasc contains already defined checkers in `default_chekers.py`. All
-checkers return `"Ã©chec"` on failure. Default checkers are listed below with
-their definition. ## `DoctypeChecker` * Rule: the HTML document contains `
+Wasc contains already defined checkers in `chekers.py`. All checkers return
+`"Ã©chec"` on failure. Available checkers are listed below with their
+definition. - [`AccessChecker`](#accesschecker) - [`AccessLinkChecker`]
+(#accesslinkchecker) - [`AccessRateChecker`](#accessratechecker) -
+[`ContactLinkChecker`](#contactlinkchecker) - [`DoctypeChecker`]
+(#doctypechecker) - [`FooterChecker`](#footerchecker) - [`HeaderChecker`]
+(#headerchecker) - [`HeadLvlChecker`](#headlvlchecker) - [`HeaderNbChecker`]
+(#headernbchecker) - [`LangChecker`](#langchecker) - [`LegalChecker`]
+(#legalchecker) ## `AccessChecker` * Rule: `"AccessibilitÃ© : XX conforme"`
+exists in the page with `XX` in `["non", "partiellement", "totalement"]` *
+Rule: Search in ``, then `
+�©" and a floating number directly followed by '%' * Return: the accessibility
+rate ## `ContactLinkChecker` * Rule: Finds `contact` or `ecrire` in a link ``
+tag * Return: the link url ## `DoctypeChecker` * Rule: the HTML document
+contains `
 ` * Rule: `
 ` is before `
-` * Return: `html` ## `LangChecker` * Rule: `
+` * Return: `html` ## `FooterChecker` * Rule: the HTML document contains `` *
+Return: `prÃ©sent` if the tag is found, else `Ã©chec` ## `HeaderChecker` *
+Rule: the HTML document contains `` * Return: `prÃ©sent` if the tag is found,
+else `Ã©chec` ## `HeadLvlChecker` * Rule: For each `
+` tags in the page, calculate its depth * Return: the list of depth of `
+` tags ## `HeaderNbChecker` * Rule: the HTML document contains `
+` * Return: the number of `
+` tags present on the page ## `LangChecker` * Rule: `
 ` has an attribute `lang` * Return: the value of `lang` ## `LegalChecker` *
 Rule: `"Mentions lÃ©gales"` exists somewhere in the page * Rule: `"Mentions
-lÃ©gales"` is a link `` with attribute `href` * Return: the value of `href` ##
-`AccessChecker` * Rule: `"AccessibilitÃ© : XX conforme"` exists somewhere in
-the page with `XX` in `["non", "partiellement", "totalement"]` * Return: `XX
-conforme` ## `AccessLinkChecker` * Rule: if `AccessChecker` is valid, then if
-it's a link * Rule: if the previous rule fails, check each link in the page
-looking for keyword `accessibilite` at the end of URL * Return: the value of
-the link ## `AccessRateChecker` (Todo) * Rule: if `AccessLinkChecker` is valid,
-get the page from the link. In this page, an accessibility rate is given as
-percent * Return: the accessibility rate
+lÃ©gales"` is a link `` with attribute `href` * Return: the value of `href`
```

### Comparing `wasc-0.4.0/docs/license.md` & `wasc-1.0.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `wasc-0.4.0/docs/releases.md` & `wasc-1.0.0/docs/releases.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 
 `pip install -U wasc`
 
 You can determine your currently installed version using:
 
 ```bash
 $ wasc --version
-wasc, version 0.3.0
+wasc, version 1.0.0
 ```
 
 ## Maintenance team
 The current and past members of the wasc team.
 
 [@gcollet](https://github.com/gcollet)
 
+## Version 1.0.0 (2023-07-12)
+* 11 checkers available (docs are updated)
+* Use trafilatura parallel download of webpages
+* Better accessibility link and rate detection
+* Bugfix: Better URL management with urllib.urljoin
+* Bugfix: Use trafilatura extract feature for accessibility rate detection
 ## Version 0.4.0 (2023-07-10)
 * Use trafilatura instead of requests to download webpages -> this allows to use simple parallel downloads
 * Moreover, trafilatura extract text and will be usefull for text searching
 * New checkers: 
     * HeaderChecker: detects <header> tag
     * FooterChecker: detects <footer> tag
     * AccessRateChecker: finds the accessibility rate in accessibility statement
```

### Comparing `wasc-0.4.0/src/wasc/cli/__init__.py` & `wasc-1.0.0/src/wasc/cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 # SPDX-License-Identifier: CECILL-2.1
 import json
 import sys
 
 import bs4
 import click
 import pandas as pd
-import requests
 from tqdm import tqdm
 from trafilatura.downloads import add_to_compressed_dict, buffered_downloads, load_download_buffer
 
 from wasc.__about__ import __version__
 from wasc.checker_factory import checker_factory
-from wasc.utils import HEADER, read_checkers, read_websites
+from wasc.utils import FAIL, OK, read_checkers, read_websites
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 DEFAULT_CHECKERS = [
     "AccessChecker", "AccessLinkChecker", "AccessRateChecker",
     "DoctypeChecker", "LangChecker", "LegalChecker",
     "ContactLinkChecker"
 ]
@@ -25,26 +24,33 @@
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("websites", type=click.Path(exists=True))
 @click.option("-c", "--checkers", type=click.Path(exists=True),
               help="Checkers list to use")
 @click.option("-f", "--output_format", default = "json",
               type=click.Choice(["json", "csv"], case_sensitive=False),
               help="Output format [default=json]")
+@click.option("-l", "--list_checkers", is_flag=True, default=False,
+              help="List known checkers [default=False]")
 @click.option("-o", "--output", default=sys.stdout,
               type=click.File("w"),
               help="Output file [default=stdout]")
 @click.version_option(version=__version__, prog_name="wasc")
-def wasc(websites, checkers, output, output_format):
+def wasc(websites, checkers, output_format, list_checkers, output):
     """
     Websites Accessibility Criteria Checker,
     helps to evaluate accessibility criteria on a list of websites
 
     WEBSITES is a CSV file containing a list of websites as couples
     "label";"URL"
     """
+    # If list_checkers then list checkers and stops
+    if list_checkers:
+        for checker in checker_factory.available():
+            click.echo(checker)
+        return
     # Reads and creates checker list
     checker_names = DEFAULT_CHECKERS
     if checkers:
         click.echo(f"Read checkers from {checkers}")
         checker_names = read_checkers(checkers)
     else :
         click.echo("Use default checkers")
@@ -66,44 +72,24 @@
     results = []
     with tqdm(total=len(url_list)) as pbar:
         for url, response in buffered_downloads(mybuffer, threads, decode=False):
             label = websites_dict[url.strip("/")]
             bs_obj = None
             error = ""
             if response:
-                if response.status == 200 :
+                if response.status == OK :
                     bs_obj = bs4.BeautifulSoup(response.data, "html.parser")
                 else:
                     error = "HTML Error Status " + str(response.status)
             else:
                 error = "Problème lors du téléchargement"
             starter = [label, url, error]
-            analysis = ["échec" for _ in checkers_list]
-            if not error:
-                analysis = [checker.execute(bs_obj, url) if bs_obj else "" for checker in checkers_list]
+            analysis = [checker.execute(bs_obj, url) if bs_obj else FAIL for checker in checkers_list]
             results.append(starter + analysis)
             pbar.update(1)
-    # results = []
-    # for i in tqdm(range(len(websites))):
-    #     label, url = websites[i]
-    #     bs_obj = None
-    #     error = ""
-    #     try:
-    #         response = requests.get(url, headers=HEADER, timeout = 1)
-    #         if response.status_code == requests.codes.ok :
-    #             bs_obj = bs4.BeautifulSoup(response.content, "html.parser")
-    #         else:
-    #             error = "HTML Error Status " + str(response.status_code)
-    #     except Exception as e:
-    #         error = str(e)
-    #     starter = [label, url, error]
-    #     analysis = ["échec" for _ in checkers_list]
-    #     if not error:
-    #         analysis = [checker.execute(bs_obj, url) if bs_obj else "" for checker in checkers_list]
-    #     results.append(starter + analysis)
 
     # Creates the DataFrame from results
     df = pd.DataFrame(results, columns=column_names)
     df.set_index(["Organisation"], inplace=True)
 
     # Output results given -o output and -f output_format
     if output == sys.stdout:
```

### Comparing `wasc-0.4.0/tests/test_checker.py` & `wasc-1.0.0/tests/test_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 from bs4 import BeautifulSoup
 
 import wasc.checkers as dft
+from wasc.utils import FAIL, PRESENT
 
 BS_PARSER = "html.parser"
 
 DEFAULT_HTML_HEAD = "<!DOCTYPE html><html><head></head><body><div>"
 DEFAULT_HTML_TAIL = "</div></body></html>"
 DEFAULT_HTML_ROOT = "https://www.example.com"
+DESIGN_NUM = "https://design.numerique.gouv.fr"
+HTML_BODY_ONLY = "<!DOCTYPE html><html><body></body></html>"
 
 class TestDoctypeChecker:
     def test_doctype_checker_init(self):
         doctype_checker = dft.DoctypeChecker()
         assert doctype_checker.name == "DoctypeChecker"
         assert doctype_checker.description == "Doctype"
 
@@ -23,21 +26,21 @@
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert doctype_checker.execute(basic_webpage, "") == "html"
 
     def test_doctype_checker_bad_doctype(self):
         test_html = "<!DOCTYPE notvalid><html></html>"
         doctype_checker = dft.DoctypeChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert doctype_checker.execute(basic_webpage, "") == dft.FAIL
+        assert doctype_checker.execute(basic_webpage, "") == FAIL
 
     def test_doctype_checker_no_doctype(self):
         test_html = "<html></html>"
         doctype_checker = dft.DoctypeChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert doctype_checker.execute(basic_webpage, "") == dft.FAIL
+        assert doctype_checker.execute(basic_webpage, "") == FAIL
 
 class TestLangChecker:
     def test_lang_checker_init(self):
         lang_checker = dft.LangChecker()
         assert lang_checker.name == "LangChecker"
         assert lang_checker.description == "Lang"
 
@@ -47,33 +50,33 @@
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert lang_checker.execute(basic_webpage, "") == "fr"
 
     def test_lang_checker_empty(self):
         test_html = "<!DOCTYPE html><html></html>"
         lang_checker = dft.LangChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert lang_checker.execute(basic_webpage, "") == dft.FAIL
+        assert lang_checker.execute(basic_webpage, "") == FAIL
 
 class TestAccessChecker:
     def test_access_checker_init(self):
         access_checker = dft.AccessChecker()
         assert access_checker.name == "AccessChecker"
         assert access_checker.description == "Mention accessibilité"
 
     def test_access_checker_fail1(self):
         test_html = DEFAULT_HTML_HEAD + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_checker.execute(basic_webpage, "") == dft.FAIL
+        assert access_checker.execute(basic_webpage, "") == FAIL
 
     def test_access_checker_fail2(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : conforme partiellement" + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_checker.execute(basic_webpage, "") == dft.FAIL
+        assert access_checker.execute(basic_webpage, "") == FAIL
 
     def test_access_checker_valid_non(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : non conforme" + DEFAULT_HTML_TAIL
         access_checker = dft.AccessChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert access_checker.execute(basic_webpage, "") == "non conforme"
 
@@ -103,15 +106,15 @@
         answer = DEFAULT_HTML_ROOT + "/accessibilite"
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_access_link_checker_fail_mention(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : totalement conforme" + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_access_link_checker_valid_other(self):
         test_html = DEFAULT_HTML_HEAD + '<a href="/accessibilite/">Accessibilité</a>' + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == DEFAULT_HTML_ROOT + "/accessibilite"
 
@@ -122,15 +125,15 @@
         answer = DEFAULT_HTML_ROOT + "/misc/accessibilite"
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_access_link_checker_fail_href(self):
         test_html = DEFAULT_HTML_HEAD + "<a>Accessibilité</a>" + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_access_link_checker_decla(self):
         test_link = '<a href="/misc/accessibilite/">Déclaration d\'accessibilité</a>'
         test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = DEFAULT_HTML_ROOT + "/misc/accessibilite"
@@ -146,28 +149,28 @@
         """
         Be Careful, this test use a real url that may change over time
         """
         test_link = '<a href="/misc/accessibilite/">Accessibilité : totalement conforme</a>'
         test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
         access_rate_checker = dft.AccessRateChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_rate_checker.execute(basic_webpage, "https://design.numerique.gouv.fr") == "100%"
+        assert access_rate_checker.execute(basic_webpage, DESIGN_NUM) == "100%"
 
     def test_access_rate_checker_fail_link(self):
         test_html = DEFAULT_HTML_HEAD + "Accessibilité : non conforme" + DEFAULT_HTML_TAIL
         access_rate_checker = dft.AccessRateChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_access_rate_checker_fail_link2(self):
         test_link = '<a href="/misc/accessibilite/">Accessibilité : totalement conforme</a>'
         test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
         access_rate_checker = dft.AccessRateChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert access_rate_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
 class TestLegalChecker:
     def test_mention_legales_checker_init(self):
         mention_legales_checker = dft.LegalChecker()
         assert mention_legales_checker.name == "LegalChecker"
         assert mention_legales_checker.description == "Mentions légales"
 
@@ -185,15 +188,15 @@
         answer = DEFAULT_HTML_ROOT + "/misc/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_mention_legales_fail_mention(self):
         test_html = DEFAULT_HTML_HEAD + "Mentions légales" + DEFAULT_HTML_TAIL
         mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_mention_legales_valid_dftlink(self):
         test_html = DEFAULT_HTML_HEAD + "foo" + DEFAULT_HTML_TAIL
         mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = "https://www.gouvernement.fr/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, "https://www.gouvernement.fr/") == answer
@@ -212,15 +215,15 @@
     def test_head_nb_valid_02(self):
         test_html = DEFAULT_HTML_HEAD + "<head></head>" + DEFAULT_HTML_TAIL
         head_nb_checker = dft.HeadNbChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = 2
         assert head_nb_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
     def test_head_nb_fail(self):
-        test_html = "<!DOCTYPE html><html><body></body></html>"
+        test_html = HTML_BODY_ONLY
         head_nb_checker = dft.HeadNbChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = 0
         assert head_nb_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
 class TestHeadLvlChecker:
     def test_head_lvl_checker_init(self):
@@ -236,55 +239,76 @@
     def test_head_lvl_valid_02(self):
         test_html = DEFAULT_HTML_HEAD + "<head></head>" + DEFAULT_HTML_TAIL
         head_lvl_checker = dft.HeadLvlChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = [1,3]
         assert head_lvl_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
     def test_head_lvl_fail(self):
-        test_html = "<!DOCTYPE html><html><body></body></html>"
+        test_html = HTML_BODY_ONLY
         head_lvl_checker = dft.HeadLvlChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = []
         assert head_lvl_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
 class TestHeaderChecker:
     def test_header_checker_init(self):
         header_checker = dft.HeaderChecker()
         assert header_checker.name == "HeaderChecker"
         assert header_checker.description == "Header"
 
     def test_header_checker_fail(self):
-        test_html = "<!DOCTYPE html><html><body></body></html>"
+        test_html = HTML_BODY_ONLY
         header_checker = dft.HeaderChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_header_checker_present(self):
         test_html = "<!DOCTYPE html><html><body><header></header></body></html>"
         header_checker = dft.HeaderChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.PRESENT
+        assert header_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == PRESENT
 
 class TestFooterChecker:
     def test_footer_checker_init(self):
         footer_checker = dft.FooterChecker()
         assert footer_checker.name == "FooterChecker"
         assert footer_checker.description == "Footer"
 
     def test_footer_checker_fail(self):
-        test_html = "<!DOCTYPE html><html><body></body></html>"
+        test_html = HTML_BODY_ONLY
         footer_checker = dft.FooterChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.FAIL
+        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_footer_checker_present(self):
         test_html = "<!DOCTYPE html><html><body><footer></footer></body></html>"
         footer_checker = dft.FooterChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
-        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == dft.PRESENT
+        assert footer_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == PRESENT
 
 class TestContactLinkChecker:
     def test_contact_link_checker_init(self):
         contact_link_checker = dft.ContactLinkChecker()
         assert contact_link_checker.name == "ContactLinkChecker"
         assert contact_link_checker.description == "Lien Contact"
 
+    def test_contact_link_checker_valid(self):
+        test_link = '<a href="/contact">Nous contacter</a>'
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        contact_link_checker = dft.ContactLinkChecker()
+        answer = "https://design.numerique.gouv.fr/contact"
+        assert contact_link_checker.execute(basic_webpage, DESIGN_NUM) == answer
+
+    def test_contact_link_checker_no_href(self):
+        test_link = "<a>Nous contacter</a>"
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        contact_link_checker = dft.ContactLinkChecker()
+        assert contact_link_checker.execute(basic_webpage, DESIGN_NUM) == FAIL
+
+    def test_contact_link_checker_bad_link(self):
+        test_link = '<a href="/foo">Nous contacter</a>'
+        test_html = DEFAULT_HTML_HEAD + test_link + DEFAULT_HTML_TAIL
+        basic_webpage = BeautifulSoup(test_html, BS_PARSER)
+        contact_link_checker = dft.ContactLinkChecker()
+        assert contact_link_checker.execute(basic_webpage, DESIGN_NUM) == FAIL
```

### Comparing `wasc-0.4.0/tests/test_checker_factory.py` & `wasc-1.0.0/tests/test_checker_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 import wasc.checker_factory as fact
 
-FAIL = "échec"
+
 class TmpChecker:
     pass
 
 class TestCheckerFactory:
     def test_checker_factory_init(self):
         tmp_factory = fact.CheckerFactory()
         assert isinstance(tmp_factory, fact.CheckerFactory)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wasc-0.4.0/tests/test_utils.py` & `wasc-1.0.0/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,22 +36,14 @@
 
 EXAMPLE_TEST_URL = "https://www.example.com/fr/test"
 EXAMPLE_ROOT = "https://www.example.com/fr"
 EXAMPLE_ROOT_SLASH = "https://www.example.com/fr/"
 
 class TestCheckAndCorrectUrl:
     def test_empty(self):
-        assert utils.check_and_correct_url("", "") == "/"
+        assert not utils.check_and_correct_url("", "")
 
     def test_correct(self):
         assert utils.check_and_correct_url(EXAMPLE_TEST_URL, "https://www.example.com") == EXAMPLE_TEST_URL
-
-    def test_overlap(self):
-        assert utils.check_and_correct_url("/fr/test", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
-        assert utils.check_and_correct_url("fr/test", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
-        assert utils.check_and_correct_url("/fr/test", EXAMPLE_ROOT) == EXAMPLE_TEST_URL
-
-    def test_compose(self):
-        assert utils.check_and_correct_url("test", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
-        assert utils.check_and_correct_url("/test", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
-        assert utils.check_and_correct_url("/test/", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
-        assert utils.check_and_correct_url("/test/", EXAMPLE_ROOT) == EXAMPLE_TEST_URL
+        assert utils.check_and_correct_url("/fr/test/", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
+        assert utils.check_and_correct_url("fr/test/", EXAMPLE_ROOT_SLASH) == EXAMPLE_TEST_URL
+        assert utils.check_and_correct_url("/fr/test/", EXAMPLE_ROOT) == EXAMPLE_TEST_URL
```

### Comparing `wasc-0.4.0/LICENSE.txt` & `wasc-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wasc-0.4.0/README.md` & `wasc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wasc-0.4.0/pyproject.toml` & `wasc-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 [tool.hatch.envs.default.env-vars]
 WASC_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.build.env-vars]
 WACS_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.default.scripts]
+profile = "python -m cProfile -s cumtime src/wasc/__main__.py {args:tests}"
 test = "pytest -v {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 lcov = "coverage lcov"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
```

### Comparing `wasc-0.4.0/PKG-INFO` & `wasc-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasc
-Version: 0.4.0
+Version: 1.0.0
 Summary: Web Accessibility Simple Checker
 Project-URL: Documentation, https://github.com/gcollet/wasc#readme
 Project-URL: Issues, https://github.com/gcollet/wasc/issues
 Project-URL: Source, https://github.com/gcollet/wasc
 Author-email: Guillaume Collet <bilouweb@free.fr>, Juliette Francis <juliette.francis@etudiant.univ-rennes.fr>
 License-Expression: CECILL-2.1
 License-File: LICENSE.txt
```

