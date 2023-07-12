# Comparing `tmp/visonicalarm2-3.1.2.tar.gz` & `tmp/visonicalarm2-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visonicalarm2-3.1.2.tar", last modified: Fri Jan 14 08:48:42 2022, max compression
+gzip compressed data, was "/mnt/c/github/VisonicAlarm2-master/dist/tmpt1iU0l/visonicalarm2-3.1.3.tar", last modified: Wed Jul 12 15:52:53 2023, max compression
```

## Comparing `visonicalarm2-3.1.2.tar` & `visonicalarm2-3.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2022-01-14 08:48:42.773012 visonicalarm2-3.1.2/
--rwxrwxrwx   0 anders    (1000) anders    (1000)      441 2022-01-14 08:48:42.773012 visonicalarm2-3.1.2/PKG-INFO
--rwxrwxrwx   0 anders    (1000) anders    (1000)     1922 2022-01-14 08:21:51.000000 visonicalarm2-3.1.2/README.md
--rwxrwxrwx   0 anders    (1000) anders    (1000)       38 2022-01-14 08:48:42.773012 visonicalarm2-3.1.2/setup.cfg
--rwxrwxrwx   0 anders    (1000) anders    (1000)      515 2022-01-14 08:48:28.000000 visonicalarm2-3.1.2/setup.py
-drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2022-01-14 08:48:42.663230 visonicalarm2-3.1.2/visonic/
--rwxrwxrwx   0 anders    (1000) anders    (1000)        0 2022-01-14 08:21:51.000000 visonicalarm2-3.1.2/visonic/__init__.py
--rwxrwxrwx   0 anders    (1000) anders    (1000)    29787 2022-01-14 08:48:20.000000 visonicalarm2-3.1.2/visonic/alarm.py
-drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2022-01-14 08:48:42.741752 visonicalarm2-3.1.2/visonicalarm2.egg-info/
--rwxrwxrwx   0 anders    (1000) anders    (1000)      441 2022-01-14 08:48:42.000000 visonicalarm2-3.1.2/visonicalarm2.egg-info/PKG-INFO
--rwxrwxrwx   0 anders    (1000) anders    (1000)      203 2022-01-14 08:48:42.000000 visonicalarm2-3.1.2/visonicalarm2.egg-info/SOURCES.txt
--rwxrwxrwx   0 anders    (1000) anders    (1000)        1 2022-01-14 08:48:42.000000 visonicalarm2-3.1.2/visonicalarm2.egg-info/dependency_links.txt
--rwxrwxrwx   0 anders    (1000) anders    (1000)        8 2022-01-14 08:48:42.000000 visonicalarm2-3.1.2/visonicalarm2.egg-info/top_level.txt
+drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/
+-rwxrwxrwx   0 anders    (1000) anders    (1000)      441 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/PKG-INFO
+-rwxrwxrwx   0 anders    (1000) anders    (1000)     1877 2023-07-12 15:49:14.000000 visonicalarm2-3.1.3/README.md
+-rwxrwxrwx   0 anders    (1000) anders    (1000)       38 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/setup.cfg
+-rwxrwxrwx   0 anders    (1000) anders    (1000)      499 2023-07-12 15:49:14.000000 visonicalarm2-3.1.3/setup.py
+drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonic/
+-rwxrwxrwx   0 anders    (1000) anders    (1000)    29163 2023-07-12 15:49:14.000000 visonicalarm2-3.1.3/visonic/alarm.py
+-rwxrwxrwx   0 anders    (1000) anders    (1000)        0 2023-07-12 15:49:14.000000 visonicalarm2-3.1.3/visonic/__init__.py
+drwxrwxrwx   0 anders    (1000) anders    (1000)        0 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonicalarm2.egg-info/
+-rwxrwxrwx   0 anders    (1000) anders    (1000)        1 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonicalarm2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 anders    (1000) anders    (1000)      441 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonicalarm2.egg-info/PKG-INFO
+-rwxrwxrwx   0 anders    (1000) anders    (1000)      203 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonicalarm2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 anders    (1000) anders    (1000)        8 2023-07-12 15:52:53.000000 visonicalarm2-3.1.3/visonicalarm2.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `visonicalarm2-3.1.2/README.md` & `visonicalarm2-3.1.3/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
-<br><a href="https://www.buymeacoffee.com/4nd3rs" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" width="150px" height="35px" alt="Buy Me A Coffee" style="height: 35px !important;width: 150px !important;" ></a>
-
-## Information
-A simple library for the Visonic PowerMaster API written in Python 3. It is only tested with a PowerMaster-10 using a PowerLink 3 IP module. The PowerLink 3 is a requirement for this library to work.
-
-The **host**, **user_code**, **panel_id**, **user_email**, **user_password** are the same you are using when logging in to your system via the Visonic-GO/BW app,
-and **app_id** is just a uniqe id generated from this site: https://www.uuidgenerator.net/ so make sure you replace 00000000-0000-0000-0000-000000000000 with an ID that you generate with that site. There is only support for the -1 partition.
-
-Please be sure that the user is the MASTER USER and you alredy added your panel in your registered account
-
-
-## Installation
-Install with pip3
-```
-$ sudo pip3 install visonicalarm2
-```
-
-## Code examples
-### Current status
-Getting the current alarm status. Available states are 'AWAY', 'HOME', 'ARMING' or 'DISARM'.
-```python
-#!/usr/bin/env python3
-from visonic import alarm
-import logging
-_LOGGER = logging.getLogger(__name__)
-
-def main():
-	hostname  = 'YOURALARMCOMPANY.tycomonitor.com'
-	user_code = '0000'
-	app_id   = '00000000-0000-0000-0000-000000000000'
-	panel_id  = '99999'
-	partition = '-1'
-	user_email = "your@email.com"
-	user_password = "yourpassword"
-
-	api = alarm.System(hostname, app_id, user_code, user_email, user_password, panel_id, partition)
-
-	res = api.connect()
-	res = api.update_devices()
-	api.print_system_devices()
-
-if __name__ == '__main__':
-	main()
-
+[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
+<br><a href="https://www.buymeacoffee.com/4nd3rs" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" width="150px" height="35px" alt="Buy Me A Coffee" style="height: 35px !important;width: 150px !important;" ></a>
+
+## Information
+A simple library for the Visonic PowerMaster API written in Python 3. It is only tested with a PowerMaster-10 using a PowerLink 3 IP module. The PowerLink 3 is a requirement for this library to work.
+
+The **host**, **user_code**, **panel_id**, **user_email**, **user_password** are the same you are using when logging in to your system via the Visonic-GO/BW app,
+and **app_id** is just a uniqe id generated from this site: https://www.uuidgenerator.net/ so make sure you replace 00000000-0000-0000-0000-000000000000 with an ID that you generate with that site. There is only support for the -1 partition.
+
+Please be sure that the user is the MASTER USER and you alredy added your panel in your registered account
+
+
+## Installation
+Install with pip3
+```
+$ sudo pip3 install visonicalarm2
+```
+
+## Code examples
+### Current status
+Getting the current alarm status. Available states are 'AWAY', 'HOME', 'ARMING' or 'DISARM'.
+```python
+#!/usr/bin/env python3
+from visonic import alarm
+import logging
+_LOGGER = logging.getLogger(__name__)
+
+def main():
+	hostname  = 'YOURALARMCOMPANY.tycomonitor.com'
+	user_code = '0000'
+	app_id   = '00000000-0000-0000-0000-000000000000'
+	panel_id  = '99999'
+	partition = '-1'
+	user_email = "your@email.com"
+	user_password = "yourpassword"
+
+	api = alarm.System(hostname, app_id, user_code, user_email, user_password, panel_id, partition)
+
+	res = api.connect()
+	res = api.update_devices()
+	api.print_system_devices()
+
+if __name__ == '__main__':
+	main()
+
 ```
```

