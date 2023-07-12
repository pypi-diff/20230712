# Comparing `tmp/ntdsdotsqlite-1.1.1.tar.gz` & `tmp/ntdsdotsqlite-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-1.1.1.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-1.1.2.tar", max compression
```

## Comparing `ntdsdotsqlite-1.1.1.tar` & `ntdsdotsqlite-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      821 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0      376 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/basehandler.py
--rw-r--r--   0        0        0     7755 2023-07-10 06:36:05.781938 ntdsdotsqlite-1.1.1/ntdsdotsqlite/computerhandler.py
--rw-r--r--   0        0        0     2066 2023-07-10 06:29:54.936247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/containerhandler.py
--rw-r--r--   0        0        0    10571 2023-07-10 06:44:44.229932 ntdsdotsqlite-1.1.1/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     6847 2023-07-10 06:29:54.937247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/domainhandler.py
--rw-r--r--   0        0        0     1743 2023-07-10 06:29:54.937913 ntdsdotsqlite-1.1.1/ntdsdotsqlite/grouphandler.py
--rw-r--r--   0        0        0     3279 2023-07-10 06:29:54.938417 ntdsdotsqlite-1.1.1/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     5733 2023-07-10 06:46:22.669573 ntdsdotsqlite-1.1.1/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     2054 2023-07-10 06:29:54.938417 ntdsdotsqlite-1.1.1/ntdsdotsqlite/organizationalunithandler.py
--rw-r--r--   0        0        0     8022 2023-07-10 06:36:02.910641 ntdsdotsqlite-1.1.1/ntdsdotsqlite/personhandler.py
--rw-r--r--   0        0        0     2022 2023-07-10 06:29:54.939050 ntdsdotsqlite-1.1.1/ntdsdotsqlite/trusteddomainhandler.py
--rw-r--r--   0        0        0     3561 2023-07-10 06:29:54.939050 ntdsdotsqlite-1.1.1/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      691 2023-07-10 07:11:25.333467 ntdsdotsqlite-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1494 2023-07-10 06:29:54.934246 ntdsdotsqlite-1.1.1/README.md
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.1/setup.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.2/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.2/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0      376 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.2/ntdsdotsqlite/basehandler.py
+-rw-r--r--   0        0        0     7755 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.2/ntdsdotsqlite/computerhandler.py
+-rw-r--r--   0        0        0     2066 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.2/ntdsdotsqlite/containerhandler.py
+-rw-r--r--   0        0        0    10573 2023-07-12 12:04:13.309593 ntdsdotsqlite-1.1.2/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     6847 2023-07-12 12:03:37.827503 ntdsdotsqlite-1.1.2/ntdsdotsqlite/domainhandler.py
+-rw-r--r--   0        0        0     1743 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/grouphandler.py
+-rw-r--r--   0        0        0     3279 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5733 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     2054 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/organizationalunithandler.py
+-rw-r--r--   0        0        0     8022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/personhandler.py
+-rw-r--r--   0        0        0     2022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/trusteddomainhandler.py
+-rw-r--r--   0        0        0     3561 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      691 2023-07-12 12:04:52.566005 ntdsdotsqlite-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.2/README.md
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.2/setup.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.2/PKG-INFO
```

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/computerhandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/computerhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/containerhandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/containerhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/decrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             tmpNTHash = decryptAES(
                 peklist[int(pekIndex[8:10])],
                 encryptedHash['EncryptedHash'][:16],
                 encryptedHash['KeyMaterial']
             )
         else:
             tmpNTHash = removeRC4Layer(peklist, encryptedHash)
-        return hexlify(removeDESLayer(tmpNTHash, rid))
+        return bytes.hex(removeDESLayer(tmpNTHash, rid))
     else:
         return default
 
 
 def decrypt_history(peklist, account, key):
     history = list()
     if key == "nt":
```

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/domainhandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/domainhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/grouphandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/grouphandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/model.sql`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/organizationalunithandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/organizationalunithandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/personhandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/personhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/trusteddomainhandler.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/trusteddomainhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-1.1.2/ntdsdotsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/pyproject.toml` & `ntdsdotsqlite-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "1.1.1"
+version = "1.1.2"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-1.1.1/README.md` & `ntdsdotsqlite-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.1/setup.py` & `ntdsdotsqlite-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['dissect[ese]>=3.5,<4.0', 'impacket>=0.10,<0.11', 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['ntdsdotsqlite = ntdsdotsqlite.__main__:main']}
 
 setup_kwargs = {
     'name': 'ntdsdotsqlite',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'A small utility to get an SQLite  database from an NTDS.DIT file.',
     'long_description': '# NTDS.Sqlite\n\nThis software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.\n\n# Installation\n\n`python -m pip install ntdsdotsqlite`\n\n# Usage\n\n`ntdsdotsqlite NTDS.DIT --system SYSTEM -o NTDS.sqlite`\n\n```\nusage: NTDS.sqlite [-h] [--system SYSTEM] -o OUTFILE NTDS\n\nThis tool helps dumping NTDS.DIT file to an SQLite database\n\npositional arguments:\n  NTDS                  The NTDS.DIT file\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --system SYSTEM       The SYSTEM hive to decrypt hashes. If not provided, hashes will be encrypted inside the sqlite database.\n  -o OUTFILE, --outfile OUTFILE\n                        The sqlite database. Example : NTDS.sqlite\n```\n\n# SQL model\n\nThe SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !\n\n# Performances\n\nPerformances can be a bit low for huge NTDS files. The whole NTDS is not stored in memory to prevent memory exhaustion when working on huge files (NTDS databases can grow to several gigabytes).\n',
     'author': 'Virgile Jarry',
     'author_email': 'virgile@mailbox.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/almandin/ntdsdotsqlite',
```

### Comparing `ntdsdotsqlite-1.1.1/PKG-INFO` & `ntdsdotsqlite-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 1.1.1
+Version: 1.1.2
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

