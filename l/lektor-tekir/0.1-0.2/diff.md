# Comparing `tmp/lektor-tekir-0.1.tar.gz` & `tmp/lektor-tekir-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-tekir-0.1.tar", last modified: Mon Jul  3 21:21:17 2023, max compression
+gzip compressed data, was "lektor-tekir-0.2.tar", last modified: Wed Jul 12 20:08:25 2023, max compression
```

## Comparing `lektor-tekir-0.1.tar` & `lektor-tekir-0.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.348130 lektor-tekir-0.1/
--rw-------   0 uyar      (1000) uyar      (1000)      179 2023-06-29 15:50:02.000000 lektor-tekir-0.1/.gitignore
--rw-------   0 uyar      (1000) uyar      (1000)       71 2023-06-29 15:50:02.000000 lektor-tekir-0.1/CHANGES.rst
--rw-------   0 uyar      (1000) uyar      (1000)     1491 2023-06-29 15:50:02.000000 lektor-tekir-0.1/LICENSE.txt
--rw-------   0 uyar      (1000) uyar      (1000)     3787 2023-07-03 21:21:17.348130 lektor-tekir-0.1/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      984 2023-07-03 21:19:30.000000 lektor-tekir-0.1/README.rst
--rw-------   0 uyar      (1000) uyar      (1000)       48 2023-06-29 15:50:02.000000 lektor-tekir-0.1/babel.cfg
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.344130 lektor-tekir-0.1/lektor_tekir/
--rw-------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 15:51:05.000000 lektor-tekir-0.1/lektor_tekir/__init__.py
--rw-------   0 uyar      (1000) uyar      (1000)     4751 2023-07-03 17:54:11.000000 lektor-tekir-0.1/lektor_tekir/api.py
--rw-------   0 uyar      (1000) uyar      (1000)      981 2023-07-02 17:28:45.000000 lektor-tekir-0.1/lektor_tekir/cli.py
--rw-------   0 uyar      (1000) uyar      (1000)     1371 2023-07-03 13:39:57.000000 lektor-tekir-0.1/lektor_tekir/dash.py
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.344130 lektor-tekir-0.1/lektor_tekir/static/
--rw-------   0 uyar      (1000) uyar      (1000)    42819 2023-06-29 15:51:05.000000 lektor-tekir-0.1/lektor_tekir/static/htmx.min.js
--rw-------   0 uyar      (1000) uyar      (1000)     3041 2023-07-03 17:37:04.000000 lektor-tekir-0.1/lektor_tekir/static/tekir-admin.css
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.344130 lektor-tekir-0.1/lektor_tekir/templates/
--rw-------   0 uyar      (1000) uyar      (1000)      996 2023-07-02 15:45:13.000000 lektor-tekir-0.1/lektor_tekir/templates/tekir_base.html
--rw-------   0 uyar      (1000) uyar      (1000)     5379 2023-07-03 20:57:04.000000 lektor-tekir-0.1/lektor_tekir/templates/tekir_content_edit.html
--rw-------   0 uyar      (1000) uyar      (1000)     2974 2023-07-03 20:53:10.000000 lektor-tekir-0.1/lektor_tekir/templates/tekir_contents.html
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.340130 lektor-tekir-0.1/lektor_tekir/translations/
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.340130 lektor-tekir-0.1/lektor_tekir/translations/tr/
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.348130 lektor-tekir-0.1/lektor_tekir/translations/tr/LC_MESSAGES/
--rw-------   0 uyar      (1000) uyar      (1000)     1379 2023-07-03 21:21:13.000000 lektor-tekir-0.1/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo
--rw-------   0 uyar      (1000) uyar      (1000)     2850 2023-07-03 20:57:32.000000 lektor-tekir-0.1/lektor_tekir/translations/tr/LC_MESSAGES/messages.po
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-03 21:21:17.344130 lektor-tekir-0.1/lektor_tekir.egg-info/
--rw-------   0 uyar      (1000) uyar      (1000)     3787 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      690 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/SOURCES.txt
--rw-------   0 uyar      (1000) uyar      (1000)        1 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/dependency_links.txt
--rw-------   0 uyar      (1000) uyar      (1000)       55 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/entry_points.txt
--rw-------   0 uyar      (1000) uyar      (1000)       82 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/requires.txt
--rw-------   0 uyar      (1000) uyar      (1000)       13 2023-07-03 21:21:17.000000 lektor-tekir-0.1/lektor_tekir.egg-info/top_level.txt
--rw-------   0 uyar      (1000) uyar      (1000)     2520 2023-07-03 20:57:18.000000 lektor-tekir-0.1/messages.pot
--rw-------   0 uyar      (1000) uyar      (1000)     1911 2023-06-30 11:14:37.000000 lektor-tekir-0.1/pyproject.toml
--rw-------   0 uyar      (1000) uyar      (1000)       38 2023-07-03 21:21:17.348130 lektor-tekir-0.1/setup.cfg
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/
+-rw-------   0 uyar      (1000) uyar      (1000)      179 2023-06-29 15:50:02.000000 lektor-tekir-0.2/.gitignore
+-rw-------   0 uyar      (1000) uyar      (1000)      332 2023-07-12 20:07:14.000000 lektor-tekir-0.2/CHANGES.rst
+-rw-------   0 uyar      (1000) uyar      (1000)     1491 2023-06-29 15:50:02.000000 lektor-tekir-0.2/LICENSE.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-12 20:08:25.521859 lektor-tekir-0.2/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)     1171 2023-07-12 17:56:26.000000 lektor-tekir-0.2/README.rst
+-rw-------   0 uyar      (1000) uyar      (1000)       48 2023-06-29 15:50:02.000000 lektor-tekir-0.2/babel.cfg
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/
+-rw-------   0 uyar      (1000) uyar      (1000)     6612 2023-07-12 18:06:32.000000 lektor-tekir-0.2/lektor_tekir/api.py
+-rw-------   0 uyar      (1000) uyar      (1000)      981 2023-07-07 10:58:40.000000 lektor-tekir-0.2/lektor_tekir/cli.py
+-rw-------   0 uyar      (1000) uyar      (1000)     1374 2023-07-12 18:56:35.000000 lektor-tekir-0.2/lektor_tekir/dash.py
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/static/
+-rw-------   0 uyar      (1000) uyar      (1000)    42819 2023-06-29 15:51:05.000000 lektor-tekir-0.2/lektor_tekir/static/htmx.min.js
+-rw-------   0 uyar      (1000) uyar      (1000)     5060 2023-07-12 18:20:59.000000 lektor-tekir-0.2/lektor_tekir/static/tekir-admin.css
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/templates/
+-rw-------   0 uyar      (1000) uyar      (1000)     1893 2023-07-11 09:09:41.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_base.html
+-rw-------   0 uyar      (1000) uyar      (1000)      988 2023-07-11 12:27:43.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_content_edit.html
+-rw-------   0 uyar      (1000) uyar      (1000)     2903 2023-07-12 18:59:22.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_contents.html
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.517859 lektor-tekir-0.2/lektor_tekir/translations/
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.517859 lektor-tekir-0.2/lektor_tekir/translations/tr/
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/
+-rw-------   0 uyar      (1000) uyar      (1000)     1909 2023-07-12 20:08:21.000000 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo
+-rw-------   0 uyar      (1000) uyar      (1000)     3936 2023-07-12 20:06:22.000000 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.po
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir.egg-info/
+-rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)      675 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/SOURCES.txt
+-rw-------   0 uyar      (1000) uyar      (1000)        1 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/dependency_links.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       55 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/entry_points.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       82 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/requires.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       13 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/top_level.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     3445 2023-07-12 20:06:12.000000 lektor-tekir-0.2/messages.pot
+-rw-------   0 uyar      (1000) uyar      (1000)     2047 2023-07-12 20:08:16.000000 lektor-tekir-0.2/pyproject.toml
+-rw-------   0 uyar      (1000) uyar      (1000)       93 2023-07-12 20:08:25.521859 lektor-tekir-0.2/setup.cfg
```

### Comparing `lektor-tekir-0.1/LICENSE.txt` & `lektor-tekir-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.1/PKG-INFO` & `lektor-tekir-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-tekir
-Version: 0.1
+Version: 0.2
 Summary: An alternative admin panel for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -64,32 +64,40 @@
 What -sort of- works, hopefully:
 
 - Navigating existing content.
 - Editing existing content.
 - Deleting content.
 - Deleting attachments.
 - Multiple language support in the UI (English and Turkish at the moment).
-- Basic dark mode.
+- Light/dark mode toggle.
 
 What's planned in the short term:
 
 - Adding new content.
 - Adding attachments.
+- Editing system fields.
+- Dividing edit form fields into tabs.
+- Deploying the site.
+- Supporting Git.
 - Managing content translations.
-- TinyMCE and/or Quill integration.
+- TinyMCE, Quill or some other editor integration.
 
 What's planned in the longer term:
 
 - Managing databags.
 - Markdown editor integration.
 - Managing everything (templates, static assets, models, flow blocks, etc).
 
+It can be installed using pip::
+
+  pip install lektor-tekir
+
 To use it, run::
 
   lektor-tekir serve
 
-And then visit the URL "http://localhost:5000/admin-tekir/en/".
+And then visit the URL "http://localhost:5000/tekir-admin/en/".
 
 The ``lektor-tekir`` CLI is identical to the Lektor CLI
 except that it patches the ``serve`` command to enable its own panel.
 
 .. _Lektor: https://www.getlektor.com/
```

### Comparing `lektor-tekir-0.1/lektor_tekir/api.py` & `lektor-tekir-0.2/lektor_tekir/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright (C) 2023 H. Turgut Uyar <uyar@tekir.org>
 #
 # lektor-tekir is released under the BSD license.
 # Read the included LICENSE.txt file for details.
 
 from pathlib import Path
 from shutil import rmtree
+from uuid import uuid4
 
-from flask import Blueprint, g, request
+from flask import Blueprint, Response, g, render_template, request, url_for
 from flask_babel import gettext as _
+from lektor.types.flow import FlowBlock
 
 
 MULTILINE = {"text", "strings", "markdown", "html", "rst", "flow"}
 
 
-bp = Blueprint("admin_tekir_api", __name__, url_prefix="/admin-tekir/api")
+bp = Blueprint("tekir_admin_api", __name__, url_prefix="/tekir-admin/api")
 
 
 @bp.route("/page-count")
 def page_count():
-    root_path = Path(g.admin_context.pad.env.root_path)
+    root_path = Path(g.admin_context.pad.root.source_filename).parent
     pages = {c.parent for c in root_path.glob("**/contents*.lr")}
     return str(len(pages))
 
 
 def field_entry(field, field_name=None):
     if field_name is None:
         field_name = field.name
@@ -36,26 +38,26 @@
         if value == default:
             value = None
     if value is not None:
         value = value.strip()
     if not value:
         return None
     if field.type.name in MULTILINE:
-        stripped = "\n".join(line.strip() for line in value.splitlines())
+        stripped = "\n".join(line.rstrip() for line in value.splitlines())
         return f"{field.name}:\n\n{stripped}"
     else:
         return f"{field.name}: {value}"
 
 
 def flowblock_entry(node, field):
     block_data = [k for k in request.form if k.startswith(f"{field.name}-")]
     if len(block_data) == 0:
         return None
     block_indexes = []
-    for i in [int(k.split("-")[1]) for k in block_data]:
+    for i in [k.split("-")[1] for k in block_data]:
         if i not in block_indexes:
             block_indexes.append(i)
     entries = []
     for i in block_indexes:
         prefix = f"{field.name}-{i}-"
         block_fields = [k for k in request.form if k.startswith(prefix)]
         block_types = {f.split("-")[2] for f in block_fields}
@@ -109,36 +111,79 @@
     path = request.args.get("path")
     node = g.admin_context.tree.get(path)
     content = get_content(node)
     source = Path(node._primary_record.source_filename)
     old_content = source.read_text()
     if content == old_content:
         return _("No changes.")
-    source.write_text(content)
-    return _("Content saved.")
+    else:
+        source.write_text(content)
+        return _("Content saved.")
 
 
 @bp.route("/check-changes", methods=["POST"])
 def check_changes():
     g.lang_code = request.args.get("lang", "en")
     path = request.args.get("path")
     node = g.admin_context.tree.get(path)
     content = get_content(node)
-    source = Path(node._primary_record.source_filename)
+    record = node._primary_record
+    source = Path(record.source_filename)
+    record_url = url_for("tekir_admin.contents", path=record.path)
     old_content = source.read_text()
-    if content != old_content:
-        return _("There are unsaved changes. Do you want to continue?")
-    return _("Are you sure?")
+    if content == old_content:
+        response = Response("")
+        response.headers["HX-Redirect"] = record_url
+    else:
+        message = _("There are unsaved changes. Do you want to continue?")
+        trigger = '{"showChanges": {"href": "%s"}}' % record_url
+        response = Response(message)
+        response.headers["HX-Trigger"] = trigger
+    return response
+
+
+@bp.route("/check-delete", methods=["POST"])
+def check_delete():
+    g.lang_code = request.args.get("lang", "en")
+    items = request.form.getlist("selected-items")
+    root_path = Path(g.admin_context.pad.root.source_filename).parent
+    result = []
+    for path in items:
+        record = g.admin_context.tree.get(path)._primary_record
+        if record.is_attachment:
+            result.append(record.path[1:])
+        else:
+            item_dir = Path(record.source_filename).parent
+            for item in item_dir.glob("**/*"):
+                if item.is_file():
+                    item_path = str(item.relative_to(root_path))
+                    result.append(item_path)
+    return "\n".join(f'<li>{p}</li>' for p in sorted(result))
+
+
+@bp.route("/delete-content", methods=["POST"])
+def delete_content():
+    g.lang_code = request.args.get("lang", "en")
+    items = request.form.getlist("selected-items")
+    for path in items:
+        record = g.admin_context.tree.get(path)._primary_record
+        if record.is_attachment:
+            filename = record.source_filename.rstrip(".lr")
+            Path(filename).unlink()
+        else:
+            item_dir = Path(record.source_filename).parent
+            rmtree(item_dir)
+    return _("Deleted.")
 
 
-@bp.route("/delete-item")
-def delete_item():
+@bp.route("/new-flowblock")
+def new_flowblock():
     g.lang_code = request.args.get("lang", "en")
+    flow_type = request.args.get("flow_type")
+    field_name = request.args.get("field_name")
     path = request.args.get("path")
     record = g.admin_context.tree.get(path)._primary_record
-    if record.is_attachment:
-        filename = record.source_filename.rstrip(".lr")
-        Path(filename).unlink()
-    else:
-        dirname = Path(record.source_filename).parent
-        rmtree(dirname)
-    return _("Deleted.")
+    block = FlowBlock(data={"_flowblock": flow_type}, pad=record.pad,
+                      record=record)
+    return render_template("tekir_flowblock.html", block=block,
+                           field_name=field_name,
+                           block_index=f"uuid_{uuid4().hex}")
```

### Comparing `lektor-tekir-0.1/lektor_tekir/cli.py` & `lektor-tekir-0.2/lektor_tekir/cli.py`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.1/lektor_tekir/dash.py` & `lektor-tekir-0.2/lektor_tekir/dash.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 # Read the included LICENSE.txt file for details.
 
 from pathlib import Path
 
 from flask import Blueprint, g, render_template, request
 
 
-bp = Blueprint("admin_tekir", __name__, url_prefix="/admin-tekir/<lang_code>",
+bp = Blueprint("tekir_admin", __name__, url_prefix="/tekir-admin/<lang_code>",
                template_folder=Path(__file__).parent / "templates",
                static_folder=Path(__file__).parent / "static")
 
 
 @bp.url_defaults
 def add_language_code(endpoint, values):
     values.setdefault("lang_code", g.lang_code)
 
 
 @bp.url_value_preprocessor
-def pull_lang_code(endpoint, values):
+def pull_language_code(endpoint, values):
     g.lang_code = values.pop("lang_code")
 
 
 @bp.route("/")
 def summary():
     return render_template("tekir_summary.html")
 
 
-@bp.route("/contents/")
+@bp.route("/contents")
 def contents():
     path = request.args.get("path", "/")
     record = g.admin_context.tree.get(path)._primary_record
     parents = []
     current = record
     while current.parent:
         current = current.parent
```

### Comparing `lektor-tekir-0.1/lektor_tekir/static/htmx.min.js` & `lektor-tekir-0.2/lektor_tekir/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.1/lektor_tekir/translations/tr/LC_MESSAGES/messages.po` & `lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.po`

 * *Files 25% similar despite different names*

```diff
@@ -3,111 +3,158 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-03 23:57+0300\n"
+"POT-Creation-Date: 2023-07-12 23:06+0300\n"
 "PO-Revision-Date: 2023-06-25 21:11+0300\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: lektor_tekir/api.py:115
+#: lektor_tekir/api.py:117
 msgid "No changes."
 msgstr "Değişiklik yok."
 
-#: lektor_tekir/api.py:117
+#: lektor_tekir/api.py:120
 msgid "Content saved."
 msgstr "İçerik kaydedildi."
 
-#: lektor_tekir/api.py:129
+#: lektor_tekir/api.py:137
 msgid "There are unsaved changes. Do you want to continue?"
 msgstr "Kaydedilmemiş değişiklikler var. Devam etmek istiyor musunuz?"
 
-#: lektor_tekir/api.py:130
-msgid "Are you sure?"
-msgstr "Emin misiniz?"
-
-#: lektor_tekir/api.py:144
+#: lektor_tekir/api.py:175
 msgid "Deleted."
 msgstr "Silindi."
 
-#: lektor_tekir/templates/tekir_base.html:7
-#: lektor_tekir/templates/tekir_base.html:13
+#: lektor_tekir/templates/tekir_base.html:6
+#: lektor_tekir/templates/tekir_base.html:14
 msgid "Admin Panel"
 msgstr "Yönetim Paneli"
 
-#: lektor_tekir/templates/tekir_base.html:22
+#: lektor_tekir/templates/tekir_base.html:26
+msgid "Toggle light mode"
+msgstr "Aydınlık moda geç"
+
+#: lektor_tekir/templates/tekir_base.html:29
+msgid "Toggle dark mode"
+msgstr "Karanlık moda geç"
+
+#: lektor_tekir/templates/tekir_base.html:36
+msgid "main navigation"
+msgstr "ana navigasyon"
+
+#: lektor_tekir/templates/tekir_base.html:38
 msgid "Summary"
 msgstr "Özet"
 
-#: lektor_tekir/templates/tekir_base.html:23
+#: lektor_tekir/templates/tekir_base.html:39
 msgid "Content"
 msgstr "İçerik"
 
-#: lektor_tekir/templates/tekir_content_edit.html:38
-#: lektor_tekir/templates/tekir_contents.html:28
-#: lektor_tekir/templates/tekir_contents.html:42
-#: lektor_tekir/templates/tekir_contents.html:54
-msgid "Delete"
-msgstr "Sil"
-
-#: lektor_tekir/templates/tekir_content_edit.html:40
-msgid "Move up"
-msgstr "Yukarı"
-
-#: lektor_tekir/templates/tekir_content_edit.html:64
+#: lektor_tekir/templates/tekir_content_edit.html:12
 msgid "Save"
 msgstr "Kaydet"
 
-#: lektor_tekir/templates/tekir_content_edit.html:66
+#: lektor_tekir/templates/tekir_content_edit.html:14
 msgid "Done"
 msgstr "Bitti"
 
-#: lektor_tekir/templates/tekir_content_edit.html:71
+#: lektor_tekir/templates/tekir_content_edit.html:19
 msgid "Close"
 msgstr "Kapat"
 
-#: lektor_tekir/templates/tekir_content_edit.html:76
+#: lektor_tekir/templates/tekir_content_edit.html:24
 msgid "Continue"
 msgstr "Devam et"
 
-#: lektor_tekir/templates/tekir_content_edit.html:77
-#: lektor_tekir/templates/tekir_contents.html:55
+#: lektor_tekir/templates/tekir_content_edit.html:25
 msgid "Cancel"
 msgstr "Vazgeç"
 
-#: lektor_tekir/templates/tekir_contents.html:7
+#: lektor_tekir/templates/tekir_contents.html:5
+msgid "You are here:"
+msgstr "Buradasınız:"
+
+#: lektor_tekir/templates/tekir_contents.html:8
+#: lektor_tekir/templates/tekir_contents.html:10
 msgid "home"
 msgstr "ana sayfa"
 
-#: lektor_tekir/templates/tekir_contents.html:18
+#: lektor_tekir/templates/tekir_contents.html:17
 msgid "Edit"
 msgstr "Düzenle"
 
-#: lektor_tekir/templates/tekir_contents.html:22
+#: lektor_tekir/templates/tekir_contents.html:21
 msgid "Subpages"
 msgstr "Altsayfalar"
 
-#: lektor_tekir/templates/tekir_contents.html:36
+#: lektor_tekir/templates/tekir_contents.html:27
+#: lektor_tekir/templates/tekir_contents.html:55
+msgid "Select"
+msgstr "Seç"
+
+#: lektor_tekir/templates/tekir_contents.html:28
+msgid "Title"
+msgstr "Başlık"
+
+#: lektor_tekir/templates/tekir_contents.html:29
+msgid "Type"
+msgstr "Tip"
+
+#: lektor_tekir/templates/tekir_contents.html:43
+#: lektor_tekir/templates/tekir_contents.html:69
+msgid "Delete selected items"
+msgstr "Seçilenleri sil"
+
+#: lektor_tekir/templates/tekir_contents.html:49
 msgid "Attachments"
 msgstr "Ekler"
 
-#: lektor_tekir/templates/tekir_contents.html:42
-msgid "attachment"
-msgstr "ek"
-
-#: lektor_tekir/templates/tekir_contents.html:51
-msgid "Do you really want to delete this content?"
-msgstr "Bu içeriği silmek istediğinizden emin misiniz?"
+#: lektor_tekir/templates/tekir_contents.html:56
+msgid "File name"
+msgstr "Dosya adı"
+
+#: lektor_tekir/templates/tekir_contents.html:76
+msgid "This operation will delete the following content items:"
+msgstr "Bu işlem aşağıdaki içerik unsurlarını silecek:"
+
+#: lektor_tekir/templates/tekir_contents.html:78
+msgid "Do you want to continue?"
+msgstr "Devam etmek istiyor musunuz?"
+
+#: lektor_tekir/templates/tekir_contents.html:79
+msgid "Yes, delete"
+msgstr "Evet, sil"
+
+#: lektor_tekir/templates/tekir_contents.html:80
+msgid "No, cancel"
+msgstr "Hayır, vazgeç"
+
+#: lektor_tekir/templates/tekir_fields.html:47
+msgid "Add"
+msgstr "Ekle"
+
+#: lektor_tekir/templates/tekir_fields.html:64
+msgid "Delete"
+msgstr "Sil"
+
+#: lektor_tekir/templates/tekir_fields.html:65
+msgid "Move up"
+msgstr "Yukarı"
+
+#: lektor_tekir/templates/tekir_fields.html:66
+msgid "Move down"
+msgstr "Aşağı"
 
 #: lektor_tekir/templates/tekir_summary.html:4
 msgid "Number of Pages"
 msgstr "Sayfa Sayısı"
```

### Comparing `lektor-tekir-0.1/lektor_tekir.egg-info/PKG-INFO` & `lektor-tekir-0.2/lektor_tekir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-tekir
-Version: 0.1
+Version: 0.2
 Summary: An alternative admin panel for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -64,32 +64,40 @@
 What -sort of- works, hopefully:
 
 - Navigating existing content.
 - Editing existing content.
 - Deleting content.
 - Deleting attachments.
 - Multiple language support in the UI (English and Turkish at the moment).
-- Basic dark mode.
+- Light/dark mode toggle.
 
 What's planned in the short term:
 
 - Adding new content.
 - Adding attachments.
+- Editing system fields.
+- Dividing edit form fields into tabs.
+- Deploying the site.
+- Supporting Git.
 - Managing content translations.
-- TinyMCE and/or Quill integration.
+- TinyMCE, Quill or some other editor integration.
 
 What's planned in the longer term:
 
 - Managing databags.
 - Markdown editor integration.
 - Managing everything (templates, static assets, models, flow blocks, etc).
 
+It can be installed using pip::
+
+  pip install lektor-tekir
+
 To use it, run::
 
   lektor-tekir serve
 
-And then visit the URL "http://localhost:5000/admin-tekir/en/".
+And then visit the URL "http://localhost:5000/tekir-admin/en/".
 
 The ``lektor-tekir`` CLI is identical to the Lektor CLI
 except that it patches the ``serve`` command to enable its own panel.
 
 .. _Lektor: https://www.getlektor.com/
```

### Comparing `lektor-tekir-0.1/lektor_tekir.egg-info/SOURCES.txt` & `lektor-tekir-0.2/lektor_tekir.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 CHANGES.rst
 LICENSE.txt
 README.rst
 babel.cfg
 messages.pot
 pyproject.toml
-lektor_tekir/__init__.py
+setup.cfg
 lektor_tekir/api.py
 lektor_tekir/cli.py
 lektor_tekir/dash.py
 lektor_tekir.egg-info/PKG-INFO
 lektor_tekir.egg-info/SOURCES.txt
 lektor_tekir.egg-info/dependency_links.txt
 lektor_tekir.egg-info/entry_points.txt
```

### Comparing `lektor-tekir-0.1/messages.pot` & `lektor-tekir-0.2/messages.pot`

 * *Files 14% similar despite different names*

```diff
@@ -4,109 +4,156 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-03 23:57+0300\n"
+"POT-Creation-Date: 2023-07-12 23:06+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: lektor_tekir/api.py:115
+#: lektor_tekir/api.py:117
 msgid "No changes."
 msgstr ""
 
-#: lektor_tekir/api.py:117
+#: lektor_tekir/api.py:120
 msgid "Content saved."
 msgstr ""
 
-#: lektor_tekir/api.py:129
+#: lektor_tekir/api.py:137
 msgid "There are unsaved changes. Do you want to continue?"
 msgstr ""
 
-#: lektor_tekir/api.py:130
-msgid "Are you sure?"
-msgstr ""
-
-#: lektor_tekir/api.py:144
+#: lektor_tekir/api.py:175
 msgid "Deleted."
 msgstr ""
 
-#: lektor_tekir/templates/tekir_base.html:7
-#: lektor_tekir/templates/tekir_base.html:13
+#: lektor_tekir/templates/tekir_base.html:6
+#: lektor_tekir/templates/tekir_base.html:14
 msgid "Admin Panel"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_base.html:22
-msgid "Summary"
+#: lektor_tekir/templates/tekir_base.html:26
+msgid "Toggle light mode"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_base.html:23
-msgid "Content"
+#: lektor_tekir/templates/tekir_base.html:29
+msgid "Toggle dark mode"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:38
-#: lektor_tekir/templates/tekir_contents.html:28
-#: lektor_tekir/templates/tekir_contents.html:42
-#: lektor_tekir/templates/tekir_contents.html:54
-msgid "Delete"
+#: lektor_tekir/templates/tekir_base.html:36
+msgid "main navigation"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:40
-msgid "Move up"
+#: lektor_tekir/templates/tekir_base.html:38
+msgid "Summary"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:64
+#: lektor_tekir/templates/tekir_base.html:39
+msgid "Content"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_content_edit.html:12
 msgid "Save"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:66
+#: lektor_tekir/templates/tekir_content_edit.html:14
 msgid "Done"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:71
+#: lektor_tekir/templates/tekir_content_edit.html:19
 msgid "Close"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:76
+#: lektor_tekir/templates/tekir_content_edit.html:24
 msgid "Continue"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_content_edit.html:77
-#: lektor_tekir/templates/tekir_contents.html:55
+#: lektor_tekir/templates/tekir_content_edit.html:25
 msgid "Cancel"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:7
+#: lektor_tekir/templates/tekir_contents.html:5
+msgid "You are here:"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:8
+#: lektor_tekir/templates/tekir_contents.html:10
 msgid "home"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:18
+#: lektor_tekir/templates/tekir_contents.html:17
 msgid "Edit"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:22
+#: lektor_tekir/templates/tekir_contents.html:21
 msgid "Subpages"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:36
+#: lektor_tekir/templates/tekir_contents.html:27
+#: lektor_tekir/templates/tekir_contents.html:55
+msgid "Select"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:28
+msgid "Title"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:29
+msgid "Type"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:43
+#: lektor_tekir/templates/tekir_contents.html:69
+msgid "Delete selected items"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:49
 msgid "Attachments"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:42
-msgid "attachment"
+#: lektor_tekir/templates/tekir_contents.html:56
+msgid "File name"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:76
+msgid "This operation will delete the following content items:"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:78
+msgid "Do you want to continue?"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:79
+msgid "Yes, delete"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:80
+msgid "No, cancel"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_fields.html:47
+msgid "Add"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_fields.html:64
+msgid "Delete"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_fields.html:65
+msgid "Move up"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:51
-msgid "Do you really want to delete this content?"
+#: lektor_tekir/templates/tekir_fields.html:66
+msgid "Move down"
 msgstr ""
 
 #: lektor_tekir/templates/tekir_summary.html:4
 msgid "Number of Pages"
 msgstr ""
```

### Comparing `lektor-tekir-0.1/pyproject.toml` & `lektor-tekir-0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lektor-tekir"
-version = "0.1"
+version = "0.2"
 description = "An alternative admin panel for Lektor."
 readme = "README.rst"
 
 authors = [{name = "H. Turgut Uyar", email = "uyar@tekir.org"}]
 license = {file = "LICENSE.txt"}
 
 keywords = ["lektor", "cms"]
@@ -43,15 +43,15 @@
 [project.scripts]
 lektor-tekir = "lektor_tekir.cli:main"
 
 [project.urls]
 repository = "https://github.com/uyar/lektor-tekir"
 
 [tool.setuptools.package-data]
-lektor_tekir = ["**/*.mo"]
+lektor_tekir = ["translations/**"]
 
 [tool.ruff]
 select = ["E", "F", "I"]
 ignore = ["E731"]
 line-length = 79
 
 [tool.ruff.isort]
@@ -66,23 +66,31 @@
 [testenv:style]
 skip_install = true
 deps =
     ruff
 commands =
     ruff lektor_tekir
 
+[testenv:flake8]
+skip_install = true
+deps =
+    flake8
+    flake8-isort
+commands =
+    flake8 lektor_tekir
+
 [testenv:package]
 skip_install = true
 deps =
     babel
     build
     twine
 commands =
     pybabel compile -d lektor_tekir/translations/
-    python -c "import shutil; shutil.rmtree('dist')"
+    python -c "import shutil; shutil.rmtree('dist', ignore_errors=True)"
     python -m build
     twine check dist/*
 """
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

