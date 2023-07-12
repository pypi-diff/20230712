# Comparing `tmp/secureli-0.6.9.tar.gz` & `tmp/secureli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.6.9.tar", max compression
+gzip compressed data, was "secureli-0.7.0.tar", max compression
```

## Comparing `secureli-0.6.9.tar` & `secureli-0.7.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0    11343 2023-07-10 20:30:46.617324 secureli-0.6.9/LICENSE
--rw-r--r--   0        0        0    11614 2023-07-10 20:30:46.617324 secureli-0.6.9/README.md
--rw-r--r--   0        0        0     2043 2023-07-10 20:30:46.617324 secureli-0.6.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0     6906 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/__init__.py
--rw-r--r--   0        0        0    11925 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/actions/update.py
--rw-r--r--   0        0        0     6450 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/main.py
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     3632 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-07-10 20:30:46.617324 secureli-0.6.9/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0     1271 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      748 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      619 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1363 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      437 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0     1349 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0    12318 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_config.py
--rw-r--r--   0        0        0    16779 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/language_support.py
--rw-r--r--   0        0        0     4545 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3048 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0      254 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/hash.py
--rw-r--r--   0        0        0     1372 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-07-10 20:30:46.621324 secureli-0.6.9/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-12 18:29:37.501287 secureli-0.7.0/LICENSE
+-rw-r--r--   0        0        0    11614 2023-07-12 18:29:37.505287 secureli-0.7.0/README.md
+-rw-r--r--   0        0        0     2043 2023-07-12 18:29:37.505287 secureli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/actions/update.py
+-rw-r--r--   0        0        0     6450 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     3632 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/base-pre-commit.yaml
+-rw-r--r--   0        0        0     4883 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0      659 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      115 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      130 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0      618 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0      367 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      232 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      228 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      714 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/language_config.py
+-rw-r--r--   0        0        0    18724 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4470 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3048 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-12 18:29:37.505287 secureli-0.7.0/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.7.0/PKG-INFO
```

### Comparing `secureli-0.6.9/LICENSE` & `secureli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/README.md` & `secureli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/pyproject.toml` & `secureli-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.6.9"
+version = "0.7.0"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.6.9/secureli/abstractions/echo.py` & `secureli-0.7.0/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/abstractions/lexer_guesser.py` & `secureli-0.7.0/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/abstractions/pre_commit.py` & `secureli-0.7.0/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/actions/action.py` & `secureli-0.7.0/secureli/actions/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,35 +95,35 @@
 
         config = SecureliConfig() if reset else self.action_deps.secureli_config.load()
 
         if not config.languages or not config.version_installed:
             return self._install_secureli(folder_path, always_yes)
         else:
             available_version = self.action_deps.language_support.version_for_language(
-                config.languages[0]
+                config.languages
             )
 
             # Check for a new version and prompt for upgrade if available
             if available_version != config.version_installed:
                 return self._upgrade_secureli(config, available_version, always_yes)
 
             # Validates the current .pre-commit-config.yaml against the generated config
             config_validation_result = (
                 self.action_deps.language_support.validate_config(
-                    language=config.languages[0]
+                    languages=config.languages
                 )
             )
 
             # If config mismatch between available version and current version prompt for upgrade
             if not config_validation_result.successful:
                 self.action_deps.echo.print(config_validation_result.output)
                 return self._update_secureli(always_yes)
 
             self.action_deps.echo.print(
-                f"SeCureLI is installed and up-to-date (language = {config.languages[0]})"
+                f"SeCureLI is installed and up-to-date (languages = {config.languages})"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.UP_TO_DATE,
                 config=config,
             )
 
     def _upgrade_secureli(
@@ -147,17 +147,15 @@
             self.action_deps.echo.warning("User canceled upgrade process")
             return VerifyResult(
                 outcome=VerifyOutcome.UPGRADE_CANCELED,
                 config=config,
             )
 
         try:
-            metadata = self.action_deps.language_support.apply_support(
-                config.languages[0]
-            )
+            metadata = self.action_deps.language_support.apply_support(config.languages)
 
             # Update config with new version installed and save it
             config.version_installed = metadata.version
             self.action_deps.secureli_config.save(config)
             self.action_deps.echo.print("SeCureLI has been upgraded successfully")
             return VerifyResult(
                 outcome=VerifyOutcome.UPGRADE_SUCCEEDED,
@@ -204,51 +202,47 @@
                 raise ValueError("No supported languages found in current repository")
 
             self.action_deps.echo.print("Detected the following languages:")
             for language, percentage in analyze_result.language_proportions.items():
                 self.action_deps.echo.print(
                     f"- {language}: {percentage:.0%}", color=Color.MAGENTA, bold=True
                 )
-            overall_language = list(analyze_result.language_proportions.keys())
-            self.action_deps.echo.print(
-                f"Overall Detected Language: {overall_language[0]}"
-            )
+            languages = list(analyze_result.language_proportions.keys())
+            self.action_deps.echo.print(f"Overall Detected Languages: {languages}")
 
-            metadata = self.action_deps.language_support.apply_support(
-                overall_language[0]
-            )
+            metadata = self.action_deps.language_support.apply_support(languages)
 
         except (ValueError, LanguageNotSupportedError, InstallFailedError) as e:
             self.action_deps.echo.error(
                 f"SeCureLI could not be installed due to an error: {str(e)}"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.INSTALL_FAILED,
             )
 
         config = SecureliConfig(
-            languages=overall_language,
+            languages=languages,
             version_installed=metadata.version,
         )
         self.action_deps.secureli_config.save(config)
 
         if secret_test_id := metadata.security_hook_id:
             self.action_deps.echo.print(
-                f"{config.languages[0]} supports secrets detection; running {secret_test_id}."
+                f"{config.languages} supports secrets detection; running {secret_test_id}."
             )
             self.action_deps.scanner.scan_repo(
                 ScanMode.ALL_FILES, specific_test=secret_test_id
             )
         else:
             self.action_deps.echo.warning(
-                f"{config.languages[0]} does not support secrets detection, skipping"
+                f"{config.languages} does not support secrets detection, skipping"
             )
 
         self.action_deps.echo.print(
-            f"SeCureLI has been installed successfully (language = {config.languages[0]})"
+            f"SeCureLI has been installed successfully (languages = {config.languages})"
         )
 
         return VerifyResult(
             outcome=VerifyOutcome.INSTALL_SUCCEEDED,
             config=config,
             analyze_result=analyze_result,
         )
```

### Comparing `secureli-0.6.9/secureli/actions/build.py` & `secureli-0.7.0/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/actions/initializer.py` & `secureli-0.7.0/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/actions/scan.py` & `secureli-0.7.0/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/actions/setup.py` & `secureli-0.7.0/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/actions/update.py` & `secureli-0.7.0/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/container.py` & `secureli-0.7.0/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/main.py` & `secureli-0.7.0/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/repositories/repo_files.py` & `secureli-0.7.0/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/repositories/secureli_config.py` & `secureli-0.7.0/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/repositories/settings.py` & `secureli-0.7.0/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/resources/files/build.txt` & `secureli-0.7.0/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.7.0/secureli/resources/files/base-pre-commit.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,27 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
     -   id: check-added-large-files
+    -   id: check-ast
+    -   id: check-docstring-first
     -   id: check-executables-have-shebangs
     -   id: check-shebang-scripts-are-executable
     -   id: check-merge-conflict
     -   id: check-toml
     -   id: check-json
     -   id: check-xml
     -   id: check-yaml
+    -   id: debug-statements
     -   id: detect-aws-credentials
         args: [--allow-missing-credentials]
     -   id: detect-private-key
+    -   id: name-tests-test
+        args: [--pytest-test-first]
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
 -   repo: https://github.com/Yelp/detect-secrets
     rev: v1.4.0
     hooks:
     -   id: detect-secrets
--   repo: https://github.com/pre-commit/mirrors-eslint
-    rev: 'v8.42.0'
-    hooks:
-    -   id: eslint
-        files: \.[t]sx?$  # *.ts and *.tsx
-        types: [file]
-        args: ['--config', '.secureli/typescript.eslintrc.yaml', '--fix']
-        additional_dependencies:
-        -   eslint@8.42.0
-        -   eslint-config-google@0.7.1
-        -   '@typescript-eslint/eslint-plugin@5.59.11'
-        -   '@typescript-eslint/parser@5.59.11'
-        -   typescript@5.1.3
-        -   eslint-config-prettier@8.8.0
--   repo: https://github.com/pre-commit/mirrors-prettier
-    rev: 'v2.7.1'
-    hooks:
-    -   id: prettier
-        args:
-          - --single-quote
-          - --trailing-comma
-          - all
```

### Comparing `secureli-0.6.9/secureli/resources/read_resource.py` & `secureli-0.7.0/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/resources/slugify.py` & `secureli-0.7.0/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/git_ignore.py` & `secureli-0.7.0/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/language_analyzer.py` & `secureli-0.7.0/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/language_config.py` & `secureli-0.7.0/secureli/services/language_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/language_support.py` & `secureli-0.7.0/secureli/services/language_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,29 @@
     The result of checking for unexpected repos in config
     """
 
     missing_repos: Optional[list[str]] = []
     unexpected_repos: Optional[list[str]] = []
 
 
+class LinterConfig(pydantic.BaseModel):
+    language: str
+    linter_data: list[Any]
+
+
+class BuildConfigResult(pydantic.BaseModel):
+    """Result about building config for all laguages"""
+
+    successful: bool
+    languages_added: list[str]
+    config_data: dict
+    linter_configs: list[LinterConfig]
+    version: str
+
+
 class LanguageSupportService:
     """
     Orchestrates a growing list of security best practices for languages. Installs
     them for the provided language.
     """
 
     def __init__(
@@ -81,67 +96,65 @@
         data_loader: Callable[[str], str],
     ):
         self.git_ignore = git_ignore
         self.pre_commit_hook = pre_commit_hook
         self.language_config = language_config
         self.data_loader = data_loader
 
-    def version_for_language(self, language: str) -> str:
+    def version_for_language(self, languages: list[str]) -> str:
         """
         May eventually grow to become a combination of pre-commit hook and other elements
-        :param language: The language to determine the version of the current config
+        :param languages: List of languages to determine the version of the current config
         :raises LanguageNotSupportedError if support for the language is not provided
         :return: The version of the current config for the provided language available for install
         """
         # For now, just a passthrough to pre-commit hook abstraction
-        return self.language_config.get_language_config(language).version
+        return self._build_pre_commit_config(languages).version
 
-    def apply_support(self, language: str) -> LanguageMetadata:
+    def apply_support(self, languages: list[str]) -> LanguageMetadata:
         """
         Applies Secure Build support for the provided language
-        :param language: The language to provide support for
+        :param languages: list of languages to provide support for
         :raises LanguageNotSupportedError if support for the language is not provided
         :return: Metadata including version of the language configuration that was just installed
         as well as a secret-detection hook ID, if present.
         """
 
         path_to_pre_commit_file = Path(".pre-commit-config.yaml")
 
         # Raises a LanguageNotSupportedError if language doesn't resolve to a yaml file
-        language_config_result = self.language_config.get_language_config(language)
+        language_config_result = self._build_pre_commit_config(languages)
 
-        if language_config_result.linter_config.successful:
-            self._write_pre_commit_configs(
-                language, language_config_result.linter_config.linter_data
-            )
+        if len(language_config_result.linter_configs) > 0:
+            self._write_pre_commit_configs(language_config_result.linter_configs)
 
         with open(path_to_pre_commit_file, "w") as f:
-            f.write(language_config_result.config_data)
+            f.write(yaml.dump(language_config_result.config_data))
 
         # Start by identifying and installing the appropriate pre-commit template (if we have one)
-        self.pre_commit_hook.install(language)
+        self.pre_commit_hook.install(languages)
 
         # Add .secureli/ to the gitignore folder if needed
         self.git_ignore.ignore_secureli_files()
 
         return LanguageMetadata(
             version=language_config_result.version,
-            security_hook_id=self.secret_detection_hook_id(language),
+            security_hook_id=self.secret_detection_hook_id(languages),
         )
 
-    def secret_detection_hook_id(self, language: str) -> Optional[str]:
+    def secret_detection_hook_id(self, languages: list[str]) -> Optional[str]:
         """
         Checks the configuration of the provided language to determine if any configured
         hooks are usable for init-time secrets detection. These supported hooks are derived
         from secrets_detecting_repos.yaml in the resources
-        :param language: The language to check support for
+        :param languages: list of languages to check support for
         :return: The hook ID to use for secrets analysis if supported, otherwise None.
         """
-        language_config = self.language_config.get_language_config(language)
-        config = yaml.safe_load(language_config.config_data)
+        language_config = self._build_pre_commit_config(languages)
+        config = language_config.config_data
         secrets_detecting_repos_data = self.data_loader("secrets_detecting_repos.yaml")
         secrets_detecting_repos = yaml.safe_load(secrets_detecting_repos_data)
 
         # Make sure the repos and configuration don't care about case sensitivity
         all_repos = config.get("repos", [])
         repos = [repo["repo"].lower() for repo in all_repos]
         secrets_detecting_repos = {
@@ -167,50 +180,48 @@
                 if hook_id in secrets_detecting_repos[repo_name]
             ]
             if secrets_detecting_hooks:
                 return secrets_detecting_hooks[0]
 
         return None
 
-    def validate_config(self, language: str) -> ValidateConfigResult:
+    def validate_config(self, languages: list[str]) -> ValidateConfigResult:
         """
         Validates that the current configuration matches the expected configuration generated
         by secureli.
-        :param language: The language to validate against
+        :param language: List of languages to validate against
         :return: Returns a boolean indicating whether the configs match
         """
         current_config = yaml.dump(self.get_current_configuration())
-        generated_config = self.language_config.get_language_config(language=language)
+        generated_config = self._build_pre_commit_config(languages)
         current_hash = self.get_current_config_hash()
         expected_hash = generated_config.version
         output = ""
 
         config_matches = current_hash == expected_hash
 
         if not config_matches:
             output += "SeCureLI has detected that the .pre-commit-config.yaml file does not match the expected configuration.\n"
             output += "This often occurs when the .pre-commit-config.yaml file has been modified directly.\n"
             output += "All changes to SeCureLI's configuration should be performed through the .secureli.yaml file.\n"
             output += "\n"
             output += self._compare_repo_versions(
                 current_config=yaml.safe_load(current_config),
-                expected_config=yaml.safe_load(generated_config.config_data),
+                expected_config=generated_config.config_data,
             )
 
         return ValidateConfigResult(successful=config_matches, output=output)
 
-    def get_configuration(self, language: str) -> HookConfiguration:
+    def get_configuration(self, languages: list[str]) -> HookConfiguration:
         """
         Creates a basic, serializable configuration out of the combined specified language config
-        :param language: The language to load the configuration for
+        :param languages: list of languages to get config for.
         :return: A serializable Configuration model
         """
-        config = yaml.safe_load(
-            self.language_config.get_language_config(language).config_data
-        )
+        config = self._build_pre_commit_config(languages).config_data
 
         def create_repo(raw_repo: dict) -> Repo:
             return Repo(
                 repo=raw_repo.get("repo", "unknown"),
                 revision=raw_repo.get("rev", "unknown"),
                 hooks=[hook.get("id", "unknown") for hook in raw_repo.get("hooks", [])],
             )
@@ -239,14 +250,52 @@
         :return: Returns a hash derived from the
         """
         config_data = yaml.dump(self.get_current_configuration())
         config_hash = hash_config(config_data)
 
         return config_hash
 
+    def _build_pre_commit_config(self, languages: list[str]) -> BuildConfigResult:
+        """
+        Builds the final .pre-commit-config.yaml from all supported repo languages. Also returns any and all
+        linter configuration data.
+        :param langauges: list of languages to get calculated configuration for.
+        :return: BuildConfigResult
+        """
+        config_data = []
+        successful_languages = []
+        linter_configs: list[LinterConfig] = []
+
+        languages.append("base")
+
+        for language in languages:
+            result = self.language_config.get_language_config(language)
+            if result.config_data:
+                successful_languages.append(language)
+                linter_configs.append(
+                    LinterConfig(
+                        language=language, linter_data=result.linter_config.linter_data
+                    )
+                ) if result.linter_config.successful else None
+                data = yaml.safe_load(result.config_data)
+                for config in data["repos"]:
+                    config_data.append(config)
+
+        languages.remove("base")
+        config = {"repos": config_data}
+        version = hash_config(yaml.dump(config))
+
+        return BuildConfigResult(
+            successful=True if len(config_data) > 0 else False,
+            languages_added=successful_languages,
+            config_data=config,
+            version=version,
+            linter_configs=linter_configs,
+        )
+
     def _get_list_of_repo_urls(self, repo_list: list[dict]) -> list[str]:
         """
         Parses a list containing repo dictionaries and returns a list of repo urls
         :param repo_list: List of dictionaries containing repo configurations
         :return: A list of repo urls.
         """
         urls = []
@@ -383,43 +432,44 @@
             current_repos=current_config_repos,
             expected_repos=expected_config_repos,
         )
 
         return output
 
     def _write_pre_commit_configs(
-        self, language: str, linter_config: list[Any]
+        self, all_linter_configs: list[LinterConfig]
     ) -> LanguageLinterWriteResult:
         """
         Install any config files for given language to support any pre-commit commands.
         i.e. Javascript ESLint requires a .eslintrc file to sufficiently use plugins and allow
         for further customization for repo's flavor of Javascript
         :param language: repo language
         :return: LanguageLinterWriteResult
         """
 
-        num_configs_wrote = 0
+        num_configs_success = 0
         num_configs_non_success = 0
-        non_success_warnings = list[str]()
+        non_success_messages = list[str]()
 
-        # if successfully loaded any language specific configs
-        for config in linter_config:
-            try:
-                for key in config:
-                    config_name = f"{slugify(language)}.{key}.yaml"
-                    path_to_config_file = Path(f".secureli/{config_name}")
+        # parse through languages for their linter config if any.
+        for language_linter_configs in all_linter_configs:
+            # parse though each config for the given language.
+            for config in language_linter_configs.linter_data:
+                try:
+                    config_name = list(config.keys())[0]
+                    # generate relative file name and path.
+                    config_file_name = f"{slugify(language_linter_configs.language)}.{config_name}.yaml"
+                    path_to_config_file = Path(f".secureli/{config_file_name}")
 
                     with open(path_to_config_file, "w") as f:
-                        f.write(yaml.dump(config[key]))
+                        f.write(yaml.dump(config[config_name]))
 
-                    num_configs_wrote += 1
-            except Exception as e:
-                num_configs_non_success += 1
-                non_success_warnings.append(
-                    f"Unable to install config: {config_name}. {e}"
-                )
+                    num_configs_success += 1
+                except Exception as e:
+                    num_configs_non_success += 1
+                    non_success_messages.append(f"Unable to install config: {e}")
 
         return LanguageLinterWriteResult(
-            num_successful=num_configs_wrote,
+            num_successful=num_configs_success,
             num_non_success=num_configs_non_success,
-            non_success_messages=non_success_warnings,
+            non_success_messages=non_success_messages,
         )
```

### Comparing `secureli-0.6.9/secureli/services/logging.py` & `secureli-0.7.0/secureli/services/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """A distinct entry in the log captured following actions like scan and init"""
 
     id: str = generate_unique_id()
     timestamp: datetime = datetime.utcnow()
     username: str = git_user_email()
     machineid: str = platform.uname().node
     secureli_version: str = secureli_version()
-    primary_language: Optional[str]
+    languages: Optional[list[str]]
     status: LogStatus
     action: LogAction
     hook_config: Optional[HookConfiguration]
     failure: Optional[LogFailure] = None
     total_failure_count: Optional[int]
     failure_count_details: Optional[object]
 
@@ -75,25 +75,23 @@
     def success(self, action: LogAction) -> LogEntry:
         """
         Capture that a successful conclusion has been reached for an action
         :param action: The action that succeeded
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
-            self.language_support.get_configuration(secureli_config.languages[0])
+            self.language_support.get_configuration(secureli_config.languages)
             if secureli_config.languages
             else None
         )
         log_entry = LogEntry(
             status=LogStatus.success,
             action=action,
             hook_config=hook_config,
-            primary_language=secureli_config.languages[0]
-            if secureli_config.languages
-            else None,
+            languages=secureli_config.languages if secureli_config.languages else None,
         )
         self._log(log_entry)
 
         return log_entry
 
     def failure(
         self,
@@ -107,28 +105,26 @@
         :param action: The action that failed
         :param details: Details about the failure
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
             None
             if not secureli_config.languages
-            else self.language_support.get_configuration(secureli_config.languages[0])
+            else self.language_support.get_configuration(secureli_config.languages)
         )
         log_entry = LogEntry(
             status=LogStatus.failure,
             action=action,
             failure=LogFailure(
                 details=details,
             ),
             total_failure_count=total_failure_count,
             failure_count_details=individual_failure_count,
             hook_config=hook_config,
-            primary_language=secureli_config.languages[0]
-            if secureli_config.languages
-            else None,
+            languages=secureli_config.languages if secureli_config.languages else None,
         )
         self._log(log_entry)
 
         return log_entry
 
     def _log(self, log_entry: LogEntry):
         """Commit a log entry to the branch log file"""
```

### Comparing `secureli-0.6.9/secureli/services/scanner.py` & `secureli-0.7.0/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/secureli_ignore.py` & `secureli-0.7.0/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/services/updater.py` & `secureli-0.7.0/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/settings.py` & `secureli-0.7.0/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/utilities/git_meta.py` & `secureli-0.7.0/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/utilities/patterns.py` & `secureli-0.7.0/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/secureli/utilities/usage_stats.py` & `secureli-0.7.0/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.9/PKG-INFO` & `secureli-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.6.9
+Version: 0.7.0
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

