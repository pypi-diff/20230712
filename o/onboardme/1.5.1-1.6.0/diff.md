# Comparing `tmp/onboardme-1.5.1.tar.gz` & `tmp/onboardme-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.5.1.tar", max compression
+gzip compressed data, was "onboardme-1.6.0.tar", max compression
```

## Comparing `onboardme-1.5.1.tar` & `onboardme-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-06-04 15:12:08.268515 onboardme-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0    13530 2023-06-04 15:12:08.268515 onboardme-1.5.1/README.md
--rwxr-xr-x   0        0        0     7600 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/console_logging.py
--rw-r--r--   0        0        0     2095 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/constants.py
--rw-r--r--   0        0        0     5641 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     6182 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6276 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/misc.py
--rwxr-xr-x   0        0        0     9785 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1738 2023-06-04 15:12:08.300515 onboardme-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    14860 1970-01-01 00:00:00.000000 onboardme-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-12 16:51:37.982841 onboardme-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    13530 2023-07-12 16:51:37.982841 onboardme-1.6.0/README.md
+-rwxr-xr-x   0        0        0     7600 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2095 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/constants.py
+-rw-r--r--   0        0        0     5641 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     6182 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6276 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8720 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-07-12 16:51:38.014844 onboardme-1.6.0/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1738 2023-07-12 16:51:38.018844 onboardme-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14860 1970-01-01 00:00:00.000000 onboardme-1.6.0/PKG-INFO
```

### Comparing `onboardme-1.5.1/LICENSE.txt` & `onboardme-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/README.md` & `onboardme-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/__init__.py` & `onboardme-1.6.0/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/config/firewall/iptables.sh` & `onboardme-1.6.0/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/console_logging.py` & `onboardme-1.6.0/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/constants.py` & `onboardme-1.6.0/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/dot_files.py` & `onboardme-1.6.0/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/env_config.py` & `onboardme-1.6.0/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/firewall.py` & `onboardme-1.6.0/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/help_text.py` & `onboardme-1.6.0/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/ide_setup.py` & `onboardme-1.6.0/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/misc.py` & `onboardme-1.6.0/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/pkg_management.py` & `onboardme-1.6.0/onboardme/pkg_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,19 +119,14 @@
             if pkg_mngr == 'snap' and not shutil.which('snap'):
                 log.warn("snap is either not installed, or you need to log out"
                          "and back in (or reboot) for it to be available. "
                          "https://snapcraft.io/docs/installing-snap-on-debian")
                 # continues onto the next package manager
                 continue
 
-            if pkg_mngr == 'brew':
-                if 'Darwin' in OS:
-                    # this installs macOS brew taps
-                    install_brew_taps(pkg_mngr_dict['taps']['macOS'])
-
             # run package manager specific setup if needed: update/upgrade
             run_preinstall_cmds(pkg_cmds, pkg_groups, no_upgrade)
 
             # run the list command for the given package manager
             installed_pkgs = []
             list_cmd = pkg_cmds.get('list', None)
             if list_cmd:
@@ -207,40 +202,14 @@
                 else:
                     log.info(f"Upgrading {pkg} now...")
 
         # Actual installation
         subproc([install_cmd + pkg], quiet=True, env=install_env_vars)
 
 
-def install_brew_taps(taps: list) -> None:
-    """
-    Checks current brew taps, and then runs brew tap {tap} on any taps that are
-    in a list of git repos from packages.yaml, and aren't already tapped
-    """
-    log.info("Checking current taps.")
-    existing_taps = subproc(["brew tap"])
-    try:
-        current_taps = existing_taps.split('\n')
-    except Exception as e:
-        log.debug(e)
-        current_taps = []
-    
-    log.debug(f"taps list is: {taps}")
-    log.debug(f"Current taps are: {current_taps}")
-
-    # for each tap, complete cmd by prepending `brew tap`
-    for index, tap in enumerate(taps):
-        log.debug(f"index: {index} tap: {tap}")
-        # only brew tap if they don't already exist
-        if tap not in current_taps:
-            subproc(["brew tap " + tap])
-        else:
-            log.info(f"{tap} already installed. Moving on.")
-
-
 # not currently using zathura on macOS, so removing as it's untested
 # def check_zathura() -> None:
 #     """
 #     make sure zathura is installed on macos
 #     installs via brew if it's not installed
 #     always returns True if everything was successful
 #     """
```

### Comparing `onboardme-1.5.1/onboardme/subproc.py` & `onboardme-1.6.0/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/onboardme/sudo_setup.py` & `onboardme-1.6.0/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.1/pyproject.toml` & `onboardme-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.5.1"
+version       = "1.6.0"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.5.1/PKG-INFO` & `onboardme-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.5.1
+Version: 1.6.0
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
```

