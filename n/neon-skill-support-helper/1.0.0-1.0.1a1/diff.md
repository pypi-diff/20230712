# Comparing `tmp/neon-skill-support_helper-1.0.0.tar.gz` & `tmp/neon-skill-support_helper-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-support_helper-1.0.0.tar", last modified: Wed Jun 28 23:24:18 2023, max compression
+gzip compressed data, was "neon-skill-support_helper-1.0.1a1.tar", last modified: Wed Jul 12 02:24:41 2023, max compression
```

## Comparing `neon-skill-support_helper-1.0.0.tar` & `neon-skill-support_helper-1.0.1a1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.008517 neon-skill-support_helper-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-28 23:24:18.008517 neon-skill-support_helper-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.000517 neon-skill-support_helper-1.0.0/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/ask_description.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/cancelled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/confirm_support.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/email_signature.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/support.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/dialog/yes.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/de-de/vocab/contact_support.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/ask_description.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/cancelled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/confirm_support.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/email_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/email_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/email_signature.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/no_email.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/dialog/support.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/locale/en-us/intent/contact_support.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-28 23:24:17.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-28 23:24:18.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 23:24:17.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-28 23:24:17.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-28 23:24:17.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 23:24:17.000000 neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 23:24:18.008517 neon-skill-support_helper-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:24:18.004517 neon-skill-support_helper-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-28 23:24:12.000000 neon-skill-support_helper-1.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.892093 neon-skill-support_helper-1.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.892093 neon-skill-support_helper-1.0.1a1/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/ask_description.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/cancelled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/confirm_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/email_signature.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/support.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/dialog/yes.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/de-de/vocab/contact_support.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.892093 neon-skill-support_helper-1.0.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/ask_description.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/cancelled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/confirm_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/email_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/email_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/email_signature.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/no_email.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/dialog/support.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/locale/en-us/intent/contact_support.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 02:24:41.000000 neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:24:41.896093 neon-skill-support_helper-1.0.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-12 02:24:38.000000 neon-skill-support_helper-1.0.1a1/version.py
```

### Comparing `neon-skill-support_helper-1.0.0/LICENSE.md` & `neon-skill-support_helper-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/PKG-INFO` & `neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-support_helper
-Version: 1.0.0
+Name: neon-skill-support-helper
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-support_helper
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-support_helper-1.0.0/README.md` & `neon-skill-support_helper-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/__init__.py` & `neon-skill-support_helper-1.0.1a1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
+import shutil
 import sys
 import yaml
 
 from copy import deepcopy
 from datetime import datetime
 from glob import glob
 from os.path import join, basename, getsize
@@ -137,15 +137,15 @@
             except Exception as e:
                 LOG.exception(e)
         return attachments
 
     def _format_email_body(self, diagnostics: dict) -> str:
         """
         Format the diagnostic data with email dialog and return a string body
-        :param diagnostics: diagnostic data to format into the email
+        :param diagnostics: diagnostic data to format into the email.
         :returns: email body to send
         """
         return '\n\n'.join((self.translate("email_intro",
                                            {"email": self.support_email}),
                             diagnostics.get('user_description') or
                             "No Description Provided",
                             self.translate("email_signature")))
@@ -237,24 +237,37 @@
 
     def _get_attachments(self, info: dict) -> list:
         """
         Parse dict information into attachment files for a support email
         :param info: diagnostic information to parse into attachments
         :returns: list of output attachment files
         """
-        att_files = self._get_log_files()
+        log_files = self._get_log_files()
         tempdir = mkdtemp()
+        att_files = list()
+        # Make a temp copy of log files to optionally truncate before sending
+        for log_file in log_files:
+            output_file = join(tempdir, basename(log_file))
+            shutil.copyfile(log_file, output_file)
+            att_files.append(output_file)
+
         packages_file = join(tempdir, "python_packages.txt")
         diagnostics_file = join(tempdir, "diagnostics.txt")
+        core_config_file = join(tempdir, "core_config.txt")
 
         # Add `pip list` output to its own file
         with open(packages_file, 'w+') as f:
             f.write(info.pop('packages', ""))
         att_files.append(packages_file)
 
+        # Add core config output to its own file
+        with open(core_config_file, 'w+') as f:
+            yaml.dump(dict(self.config_core), f)
+        att_files.append(core_config_file)
+
         # Dump gathered diagnostics to separate file
         with open(diagnostics_file, 'w+') as f:
             yaml.dump(info, f)
         att_files.append(diagnostics_file)
 
         return att_files
```

### Comparing `neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/PKG-INFO` & `neon-skill-support_helper-1.0.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-support-helper
-Version: 1.0.0
+Name: neon-skill-support_helper
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-support_helper
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-support_helper-1.0.0/neon_skill_support_helper.egg-info/SOURCES.txt` & `neon-skill-support_helper-1.0.1a1/neon_skill_support_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/setup.py` & `neon-skill-support_helper-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/skill.json` & `neon-skill-support_helper-1.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/test/test_skill.py` & `neon-skill-support_helper-1.0.1a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.0.0/version.py` & `neon-skill-support_helper-1.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1a1"
```

