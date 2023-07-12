# Comparing `tmp/pelican-sitemap-1.0.2.tar.gz` & `tmp/pelican_sitemap-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-sitemap-1.0.2.tar", last modified: Sat Aug 22 07:45:11 2020, max compression
+gzip compressed data, was "pelican_sitemap-1.0.3.tar", max compression
```

## Comparing `pelican-sitemap-1.0.2.tar` & `pelican_sitemap-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3224 2020-08-22 07:44:15.457873 pelican-sitemap-1.0.2/README.md
--rw-r--r--   0        0        0       31 2020-08-22 07:44:15.457873 pelican-sitemap-1.0.2/pelican/plugins/sitemap/__init__.py
--rw-r--r--   0        0        0     9774 2020-08-22 07:44:15.461873 pelican-sitemap-1.0.2/pelican/plugins/sitemap/sitemap.py
--rw-r--r--   0        0        0     2118 2020-08-22 07:45:10.730089 pelican-sitemap-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4136 2020-08-22 07:45:11.142815 pelican-sitemap-1.0.2/setup.py
--rw-r--r--   0        0        0     4668 2020-08-22 07:45:11.143222 pelican-sitemap-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3409 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/README.md
+-rw-r--r--   0        0        0       37 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/__init__.py
+-rw-r--r--   0        0        0     9896 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/sitemap.py
+-rw-r--r--   0        0        0      157 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/test_data/article1.md
+-rw-r--r--   0        0        0      636 2023-07-12 08:41:16.770682 pelican_sitemap-1.0.3/pelican/plugins/sitemap/test_sitemap.py
+-rw-r--r--   0        0        0     2678 2023-07-12 08:41:28.066763 pelican_sitemap-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 pelican_sitemap-1.0.3/PKG-INFO
```

### Comparing `pelican-sitemap-1.0.2/README.md` & `pelican_sitemap-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Sitemap
 =======
 
-[![Build Status](https://img.shields.io/github/workflow/status/pelican-plugins/sitemap/build)](https://github.com/pelican-plugins/sitemap/actions) [![PyPI Version](https://img.shields.io/pypi/v/pelican-sitemap)](https://pypi.org/project/pelican-sitemap/)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/sitemap/main.yml?branch=main)](https://github.com/pelican-plugins/sitemap/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-sitemap)](https://pypi.org/project/pelican-sitemap/)
+![License](https://img.shields.io/pypi/l/pelican-sitemap?color=blue)
 
 This [Pelican][] plugin generates a site map in plain-text or XML format. You can use the `SITEMAP` variable in your settings file to configure the behavior of the plugin.
 
 Installation
 ------------
 
 This plugin can be installed via:
@@ -35,19 +37,23 @@
 
     - `pages`, the update frequency of the pages
 
     - `indexes`, the update frequency of the index pages
 
     Valid frequency values are `always`, `hourly`, `daily`, `weekly`, `monthly`, `yearly` and `never`.
 
-You can exclude URLs from being included in the site map via regular expressions. For example, to exclude all URLs containing `tag/` or `category/` you can use the following `SITEMAP` setting.
+* `exclude`, which is a list of regular expressions that will be used to exclude matched URLs from the sitemap if *any* of them match. For example:
 
 ```python
 SITEMAP = {
-    "exclude": ["tag/", "category/"]
+    "exclude": [
+        "^/noindex/",  # starts with "/noindex/"
+        "/tag/",       # contains "/tag/"
+        "\.json$",     # ends with ".json"
+    ]
 }
 ```
 
 If a key is missing or a value is incorrect, it will be replaced with the default value.
 
 You can also exclude an individual URL by adding metadata to it, setting `private` to `True`.
 
@@ -56,18 +62,14 @@
 > **Note:** `priorities` and `changefreqs` are information for search engines and are only used in the XML site maps. For more information, see: <https://www.sitemaps.org/protocol.html#xmlTagDefinitions>
 
 **Example**
 
 Here is an example configuration (it is also the default settings):
 
 ```python
-# Where your plug-ins reside
-PLUGIN_PATHS = ["/where/you/cloned/it/pelican-plugins/",]
-PLUGINS=["sitemap",]
-
 SITEMAP = {
     "format": "xml",
     "priorities": {
         "articles": 0.5,
         "indexes": 0.5,
         "pages": 0.5
     },
@@ -85,7 +87,12 @@
 Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
 
 To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
 [Pelican]: https://github.com/getpelican/pelican
 [existing issues]: https://github.com/pelican-plugins/sitemap/issues
 [Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
+
+License
+-------
+
+This project is licensed under the [AGPL-3.0](http://www.gnu.org/licenses/agpl-3.0-standalone.html) license.
```

### Comparing `pelican-sitemap-1.0.2/pelican/plugins/sitemap/sitemap.py` & `pelican_sitemap-1.0.3/pelican/plugins/sitemap/sitemap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-Sitemap
--------
-
-The sitemap plugin generates plain-text or XML sitemaps.
-"""
+"""The Sitemap plugin generates plain-text or XML sitemaps."""
 
-from __future__ import unicode_literals
 
 from codecs import open
 import collections
 from datetime import datetime
 from logging import info, warning
 import os.path
 import re
@@ -24,14 +17,16 @@
 
 XML_HEADER = """<?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9 http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd"
 xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
 """
 
+TXT_URL = "{0}/{1}\n"
+
 XML_URL = """
 <url>
 <loc>{0}/{1}</loc>
 <lastmod>{2}</lastmod>
 <changefreq>{3}</changefreq>
 <priority>{4}</priority>
 </url>
@@ -39,25 +34,28 @@
 
 XML_FOOTER = """
 </urlset>
 """
 
 
 def format_date(date):
+    """Format the date in the expected format."""
     if date.tzinfo:
         tz = date.strftime("%z")
         tz = tz[:-2] + ":" + tz[-2:]
     else:
         tz = "-00:00"
     return date.strftime("%Y-%m-%dT%H:%M:%S") + tz
 
 
-class SitemapGenerator(object):
-    def __init__(self, context, settings, path, theme, output_path, *null):
+class SitemapGenerator:
+    """Sitemap generator class."""
 
+    def __init__(self, context, settings, path, theme, output_path, *null):
+        """Initialize the sitemap generator."""
         self.output_path = output_path
         self.context = context
         self.now = datetime.now()
         self.siteurl = settings.get("SITEURL")
 
         self.default_timezone = settings.get("TIMEZONE", "UTC")
         self.timezone = getattr(self, "timezone", self.default_timezone)
@@ -79,19 +77,19 @@
 
         if not isinstance(config, dict):
             warning("sitemap plugin: the SITEMAP setting must be a dict")
         else:
             fmt = config.get("format")
             pris = config.get("priorities")
             chfreqs = config.get("changefreqs")
-            self.sitemapExclude = config.get("exclude", [])
+            self.sitemapExclude = [re.compile(x) for x in config.get("exclude", [])]
 
             if fmt not in ("xml", "txt"):
-                warning("sitemap plugin: SITEMAP['format'] must be `txt' or `xml'")
-                warning("sitemap plugin: Setting SITEMAP['format'] on `xml'")
+                warning("sitemap plugin: SITEMAP['format'] must be 'txt' or 'xml'")
+                warning("sitemap plugin: Setting SITEMAP['format'] to 'xml'")
             elif fmt == "txt":
                 self.format = fmt
                 return
 
             valid_keys = ("articles", "indexes", "pages")
             valid_chfreqs = (
                 "always",
@@ -107,40 +105,40 @@
                 # We use items for Py3k compat. .iteritems() otherwise
                 for k, v in pris.items():
                     if k in valid_keys and not isinstance(v, (int, float)):
                         default = self.priorities[k]
                         warning("sitemap plugin: priorities must be numbers")
                         warning(
                             "sitemap plugin: setting SITEMAP['priorities']"
-                            "['{0}'] on {1}".format(k, default)
+                            "['{}'] on {}".format(k, default)
                         )
                         pris[k] = default
                 self.priorities.update(pris)
             elif pris is not None:
                 warning("sitemap plugin: SITEMAP['priorities'] must be a dict")
                 warning("sitemap plugin: using the default values")
 
             if isinstance(chfreqs, dict):
                 # .items() for py3k compat.
                 for k, v in chfreqs.items():
                     if k in valid_keys and v not in valid_chfreqs:
                         default = self.changefreqs[k]
-                        warning("sitemap plugin: invalid changefreq `{0}'".format(v))
+                        warning(f"sitemap plugin: invalid changefreq '{v}'")
                         warning(
                             "sitemap plugin: setting SITEMAP['changefreqs']"
-                            "['{0}'] on '{1}'".format(k, default)
+                            "['{}'] on '{}'".format(k, default)
                         )
                         chfreqs[k] = default
                 self.changefreqs.update(chfreqs)
             elif chfreqs is not None:
                 warning("sitemap plugin: SITEMAP['changefreqs'] must be a dict")
                 warning("sitemap plugin: using the default values")
 
-    def write_url(self, page, fd):  # NOQA C901
-
+    def write_url(self, page, fd):
+        """Write the URL."""
         if getattr(page, "status", "published") != "published":
             return
 
         if getattr(page, "private", "False") == "True":
             return
 
         # We can disable categories/authors/etc by using False instead of ''
@@ -170,50 +168,50 @@
         else:
             pri = self.priorities["indexes"]
             chfreq = self.changefreqs["indexes"]
 
         pageurl = "" if page.url == "index.html" else page.url
 
         # Exclude URLs from the sitemap:
+        if any(x.search(pageurl) for x in self.sitemapExclude):
+            return
+
         if self.format == "xml":
-            flag = False
-            for regstr in self.sitemapExclude:
-                if re.match(regstr, pageurl):
-                    flag = True
-                    break
-            if not flag:
-                fd.write(XML_URL.format(self.siteurl, pageurl, lastmod, chfreq, pri))
+            fd.write(XML_URL.format(self.siteurl, pageurl, lastmod, chfreq, pri))
         else:
-            fd.write(self.siteurl + "/" + pageurl + "\n")
+            fd.write(TXT_URL.format(self.siteurl, pageurl))
 
     def get_date_modified(self, page, default):
+        """Return the page's modified date."""
         if hasattr(page, "modified"):
             if isinstance(page.modified, datetime):
                 return page.modified
             return get_date(page.modified)
         else:
             return default
 
     def set_url_wrappers_modification_date(self, wrappers):
-        for (wrapper, articles) in wrappers:
+        """Set the URL wrapper's modification date."""
+        for wrapper, articles in wrappers:
             lastmod = datetime.min.replace(tzinfo=self.timezone)
             for article in articles:
                 lastmod = max(lastmod, article.date.replace(tzinfo=self.timezone))
                 try:
                     modified = self.get_date_modified(article, datetime.min).replace(
                         tzinfo=self.timezone
                     )
                     lastmod = max(lastmod, modified)
                 except ValueError:
                     # Supressed: user will be notified.
                     pass
             setattr(wrapper, "modified", str(lastmod))
 
     def generate_output(self, writer):
-        path = os.path.join(self.output_path, "sitemap.{0}".format(self.format))
+        """Generate and write the output to disk."""
+        path = os.path.join(self.output_path, f"sitemap.{self.format}")
 
         pages = (
             self.context["pages"]
             + self.context["articles"]
             + [c for (c, a) in self.context["categories"]]
             + [t for (t, a) in self.context["tags"]]
             + [a for (a, b) in self.context["authors"]]
@@ -222,51 +220,47 @@
         self.set_url_wrappers_modification_date(self.context["categories"])
         self.set_url_wrappers_modification_date(self.context["tags"])
         self.set_url_wrappers_modification_date(self.context["authors"])
 
         for article in self.context["articles"]:
             pages += article.translations
 
-        info("writing {0}".format(path))
+        info(f"writing {path}")
 
         with open(path, "w", encoding="utf-8") as fd:
-
             if self.format == "xml":
                 fd.write(XML_HEADER)
             else:
                 fd.write(TXT_HEADER.format(self.siteurl))
 
             FakePage = collections.namedtuple(
                 "FakePage", ["status", "date", "url", "save_as"]
             )
 
             for standard_page in self.context["DIRECT_TEMPLATES"]:
-                standard_page_url = self.context.get(
-                    "{}_URL".format(standard_page.upper())
-                )
+                standard_page_url = self.context.get(f"{standard_page.upper()}_URL")
                 standard_page_save_as = self.context.get(
-                    "{}_SAVE_AS".format(standard_page.upper())
+                    f"{standard_page.upper()}_SAVE_AS"
                 )
 
                 # No save _SAVE_AS field means no output file. Skip.
                 if not standard_page_save_as:
                     continue
 
                 fake = FakePage(
                     status="published",
                     date=self.now,
-                    url=standard_page_url or "{}.html".format(standard_page),
+                    url=standard_page_url or f"{standard_page}.html",
                     save_as=standard_page_save_as,
                 )
                 self.write_url(fake, fd)
 
             # add template pages
             # We use items for Py3k compat. .iteritems() otherwise
-            for path, template_page_url in self.context["TEMPLATE_PAGES"].items():
-
+            for template_page_url in self.context["TEMPLATE_PAGES"].items():
                 # don't add duplicate entry for index page
                 if template_page_url == "index.html":
                     continue
 
                 fake = FakePage(
                     status="published",
                     date=self.now,
@@ -279,12 +273,14 @@
                 self.write_url(page, fd)
 
             if self.format == "xml":
                 fd.write(XML_FOOTER)
 
 
 def get_generators(generators):
+    """Return the Sitemap generator."""
     return SitemapGenerator
 
 
 def register():
+    """Register the plugin with Pelican."""
     signals.get_generators.connect(get_generators)
```

### Comparing `pelican-sitemap-1.0.2/setup.py` & `pelican_sitemap-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,131 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-sitemap
+Version: 1.0.3
+Summary: Pelican plugin to generate sitemap in plain-text or XML format
+Home-page: https://github.com/pelican-plugins/sitemap
+License: AGPL-3.0
+Keywords: pelican,plugin,sitemap
+Author: Pelican Dev Team
+Author-email: authors@getpelican.com
+Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: markdown
+Requires-Dist: markdown (>=3.2) ; extra == "markdown"
+Requires-Dist: pelican (>=4.5)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Funding, https://donate.getpelican.com/
+Project-URL: Issue Tracker, https://github.com/pelican-plugins/sitemap/issues
+Project-URL: Repository, https://github.com/pelican-plugins/sitemap
+Description-Content-Type: text/markdown
+
+Sitemap
+=======
+
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/sitemap/main.yml?branch=main)](https://github.com/pelican-plugins/sitemap/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-sitemap)](https://pypi.org/project/pelican-sitemap/)
+![License](https://img.shields.io/pypi/l/pelican-sitemap?color=blue)
+
+This [Pelican][] plugin generates a site map in plain-text or XML format. You can use the `SITEMAP` variable in your settings file to configure the behavior of the plugin.
+
+Installation
+------------
+
+This plugin can be installed via:
+
+    python -m pip install pelican-sitemap
+
+Usage
+-----
+
+The `SITEMAP` setting must be a Python dictionary and can contain these keys:
+
+* `format`, which sets the output format of the plugin (`xml` or `txt`)
+
+* `priorities`, which is a dictionary with three keys:
+
+    - `articles`, the priority for the URLs of the articles and their translations
+
+    - `pages`, the priority for the URLs of the static pages
+
+    - `indexes`, the priority for the URLs of the index pages, such as tags, author pages, categories indexes, archives, etc.
+
+    All the values of this dictionary must be decimal numbers between `0` and `1`.
+
+* `changefreqs`, which is a dictionary with three items:
+
+    - `articles`, the update frequency of the articles
+
+    - `pages`, the update frequency of the pages
+
+    - `indexes`, the update frequency of the index pages
+
+    Valid frequency values are `always`, `hourly`, `daily`, `weekly`, `monthly`, `yearly` and `never`.
+
+* `exclude`, which is a list of regular expressions that will be used to exclude matched URLs from the sitemap if *any* of them match. For example:
+
+```python
+SITEMAP = {
+    "exclude": [
+        "^/noindex/",  # starts with "/noindex/"
+        "/tag/",       # contains "/tag/"
+        "\.json$",     # ends with ".json"
+    ]
+}
+```
+
+If a key is missing or a value is incorrect, it will be replaced with the default value.
+
+You can also exclude an individual URL by adding metadata to it, setting `private` to `True`.
+
+The sitemap is saved in: `<output_path>/sitemap.<format>`
+
+> **Note:** `priorities` and `changefreqs` are information for search engines and are only used in the XML site maps. For more information, see: <https://www.sitemaps.org/protocol.html#xmlTagDefinitions>
 
-packages = \
-['pelican', 'pelican.plugins.sitemap']
+**Example**
 
-package_data = \
-{'': ['*']}
+Here is an example configuration (it is also the default settings):
 
-install_requires = \
-['pelican>=4.5,<5.0']
-
-extras_require = \
-{'markdown': ['markdown>=3.2.2,<4.0.0']}
-
-setup_kwargs = {
-    'name': 'pelican-sitemap',
-    'version': '1.0.2',
-    'description': 'Pelican plugin to generate sitemap in plain-text or XML format',
-    'long_description': 'Sitemap\n=======\n\n[![Build Status](https://img.shields.io/github/workflow/status/pelican-plugins/sitemap/build)](https://github.com/pelican-plugins/sitemap/actions) [![PyPI Version](https://img.shields.io/pypi/v/pelican-sitemap)](https://pypi.org/project/pelican-sitemap/)\n\nThis [Pelican][] plugin generates a site map in plain-text or XML format. You can use the `SITEMAP` variable in your settings file to configure the behavior of the plugin.\n\nInstallation\n------------\n\nThis plugin can be installed via:\n\n    python -m pip install pelican-sitemap\n\nUsage\n-----\n\nThe `SITEMAP` setting must be a Python dictionary and can contain these keys:\n\n* `format`, which sets the output format of the plugin (`xml` or `txt`)\n\n* `priorities`, which is a dictionary with three keys:\n\n    - `articles`, the priority for the URLs of the articles and their translations\n\n    - `pages`, the priority for the URLs of the static pages\n\n    - `indexes`, the priority for the URLs of the index pages, such as tags, author pages, categories indexes, archives, etc.\n\n    All the values of this dictionary must be decimal numbers between `0` and `1`.\n\n* `changefreqs`, which is a dictionary with three items:\n\n    - `articles`, the update frequency of the articles\n\n    - `pages`, the update frequency of the pages\n\n    - `indexes`, the update frequency of the index pages\n\n    Valid frequency values are `always`, `hourly`, `daily`, `weekly`, `monthly`, `yearly` and `never`.\n\nYou can exclude URLs from being included in the site map via regular expressions. For example, to exclude all URLs containing `tag/` or `category/` you can use the following `SITEMAP` setting.\n\n```python\nSITEMAP = {\n    "exclude": ["tag/", "category/"]\n}\n```\n\nIf a key is missing or a value is incorrect, it will be replaced with the default value.\n\nYou can also exclude an individual URL by adding metadata to it, setting `private` to `True`.\n\nThe sitemap is saved in: `<output_path>/sitemap.<format>`\n\n> **Note:** `priorities` and `changefreqs` are information for search engines and are only used in the XML site maps. For more information, see: <https://www.sitemaps.org/protocol.html#xmlTagDefinitions>\n\n**Example**\n\nHere is an example configuration (it is also the default settings):\n\n```python\n# Where your plug-ins reside\nPLUGIN_PATHS = ["/where/you/cloned/it/pelican-plugins/",]\nPLUGINS=["sitemap",]\n\nSITEMAP = {\n    "format": "xml",\n    "priorities": {\n        "articles": 0.5,\n        "indexes": 0.5,\n        "pages": 0.5\n    },\n    "changefreqs": {\n        "articles": "monthly",\n        "indexes": "daily",\n        "pages": "monthly"\n    }\n}\n```\n\nContributing\n------------\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[Pelican]: https://github.com/getpelican/pelican\n[existing issues]: https://github.com/pelican-plugins/sitemap/issues\n[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html\n',
-    'author': 'Pelican Dev Team',
-    'author_email': 'authors@getpelican.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pelican-plugins/sitemap',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
+```python
+SITEMAP = {
+    "format": "xml",
+    "priorities": {
+        "articles": 0.5,
+        "indexes": 0.5,
+        "pages": 0.5
+    },
+    "changefreqs": {
+        "articles": "monthly",
+        "indexes": "daily",
+        "pages": "monthly"
+    }
 }
+```
+
+Contributing
+------------
+
+Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
+
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
+
+[Pelican]: https://github.com/getpelican/pelican
+[existing issues]: https://github.com/pelican-plugins/sitemap/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
+
+License
+-------
 
+This project is licensed under the [AGPL-3.0](http://www.gnu.org/licenses/agpl-3.0-standalone.html) license.
 
-setup(**setup_kwargs)
```

