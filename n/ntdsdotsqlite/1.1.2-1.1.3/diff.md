# Comparing `tmp/ntdsdotsqlite-1.1.2.tar.gz` & `tmp/ntdsdotsqlite-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-1.1.2.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-1.1.3.tar", max compression
```

## Comparing `ntdsdotsqlite-1.1.2.tar` & `ntdsdotsqlite-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.2/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      821 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.2/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0      376 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.2/ntdsdotsqlite/basehandler.py
--rw-r--r--   0        0        0     7755 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.2/ntdsdotsqlite/computerhandler.py
--rw-r--r--   0        0        0     2066 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.2/ntdsdotsqlite/containerhandler.py
--rw-r--r--   0        0        0    10573 2023-07-12 12:04:13.309593 ntdsdotsqlite-1.1.2/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     6847 2023-07-12 12:03:37.827503 ntdsdotsqlite-1.1.2/ntdsdotsqlite/domainhandler.py
--rw-r--r--   0        0        0     1743 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/grouphandler.py
--rw-r--r--   0        0        0     3279 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     5733 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.2/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     2054 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/organizationalunithandler.py
--rw-r--r--   0        0        0     8022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/personhandler.py
--rw-r--r--   0        0        0     2022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/trusteddomainhandler.py
--rw-r--r--   0        0        0     3561 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.2/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      691 2023-07-12 12:04:52.566005 ntdsdotsqlite-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1494 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.2/README.md
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.2/setup.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.3/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.3/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0      376 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.3/ntdsdotsqlite/basehandler.py
+-rw-r--r--   0        0        0     7755 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.3/ntdsdotsqlite/computerhandler.py
+-rw-r--r--   0        0        0     2066 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.3/ntdsdotsqlite/containerhandler.py
+-rw-r--r--   0        0        0    10591 2023-07-12 13:03:48.088424 ntdsdotsqlite-1.1.3/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     6842 2023-07-12 13:02:53.633713 ntdsdotsqlite-1.1.3/ntdsdotsqlite/domainhandler.py
+-rw-r--r--   0        0        0     1743 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/grouphandler.py
+-rw-r--r--   0        0        0     3279 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5733 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     2054 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/organizationalunithandler.py
+-rw-r--r--   0        0        0     8022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/personhandler.py
+-rw-r--r--   0        0        0     2022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/trusteddomainhandler.py
+-rw-r--r--   0        0        0     3561 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      717 2023-07-12 13:05:31.989042 ntdsdotsqlite-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.3/README.md
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.3/setup.py
+-rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.3/PKG-INFO
```

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/computerhandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/computerhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/containerhandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/containerhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/decrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                 encryptedHistory['EncryptedHash'],
                 encryptedHistory['KeyMaterial']
             )
             for i in range(0, len(tmpHistory) // 16):
                 NTHash = removeDESLayer(tmpHistory[i * 16:(i + 1) * 16], rid)
                 history.append(bytes.hex(NTHash))
         else:
-            tmpNTHistory = removeRC4Layer(encryptedHistory)
+            tmpNTHistory = removeRC4Layer(peklist, encryptedHistory)
             for i in range(0, len(tmpNTHistory) // 16):
                 NTHash = removeDESLayer(tmpNTHistory[i * 16:(i + 1) * 16], rid)
                 history.append(bytes.hex(NTHash))
         return history
     else:  # key = lm
         if account["encrypted_lmPwdHistory"] is None:
             return list()
@@ -229,15 +229,15 @@
                 pekIndex = hexlify(cipherText['Header'])
                 plainText = decryptAES(
                     peklist[int(pekIndex[8:10])],
                     cipherText['EncryptedHash'][4:],
                     cipherText['KeyMaterial']
                 )
             else:
-                plainText = removeRC4Layer(cipherText)
+                plainText = removeRC4Layer(peklist, cipherText)
             haveInfo = len(plainText) > 0x6f + 2 + 4
     if haveInfo:
         answers = []
         try:
             userProperties = samr.USER_PROPERTIES(plainText)
         except:
             return list()
```

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/domainhandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/domainhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,26 +68,26 @@
                 # extract pek if bootkey available
                 if self.bootkey is not None:
                     peklist = row.get(self.attributes["pekList"])
                     encryptedPekList = PEKLIST_ENC(peklist)
                     if encryptedPekList['Header'][:4] == b'\x02\x00\x00\x00':
                         # Up to Windows 2012 R2 looks like header starts this way
                         md5h = md5()
-                        md5h.update(self.bootKey)
+                        md5h.update(self.bootkey)
                         for i in range(1000):
                             md5h.update(encryptedPekList['KeyMaterial'])
                         tmpKey = md5h.digest()
                         rc4 = ARC4.new(tmpKey)
                         decryptedPekList = PEKLIST_PLAIN(
                             rc4.encrypt(encryptedPekList['EncryptedPek'])
                         )
                         PEKLen = len(PEK_KEY())
                         for i in range(len(decryptedPekList['DecryptedPek']) // PEKLen):
                             cursor = i * PEKLen
-                            pek = self.PEK_KEY(
+                            pek = PEK_KEY(
                                 decryptedPekList['DecryptedPek'][cursor:cursor+PEKLen]
                             )
                             self.pek.append(pek['Key'])
 
                     elif encryptedPekList['Header'][:4] == b'\x03\x00\x00\x00':
                         decryptedPekList = PEKLIST_PLAIN(
                             decryptAES(
```

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/grouphandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/grouphandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/model.sql`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/organizationalunithandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/organizationalunithandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/personhandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/personhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/trusteddomainhandler.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/trusteddomainhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-1.1.3/ntdsdotsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/pyproject.toml` & `ntdsdotsqlite-1.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "1.1.2"
+version = "1.1.3"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dissect = {extras = ["ese"], version = "^3.5"}
 impacket = "^0.10"
 tqdm = "^4.65.0"
+pycryptodomex = "^3.18.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ntdsdotsqlite = 'ntdsdotsqlite.__main__:main'
```

### Comparing `ntdsdotsqlite-1.1.2/README.md` & `ntdsdotsqlite-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.2/setup.py` & `ntdsdotsqlite-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 packages = \
 ['ntdsdotsqlite']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dissect[ese]>=3.5,<4.0', 'impacket>=0.10,<0.11', 'tqdm>=4.65.0,<5.0.0']
+['dissect[ese]>=3.5,<4.0',
+ 'impacket>=0.10,<0.11',
+ 'pycryptodomex>=3.18.0,<4.0.0',
+ 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['ntdsdotsqlite = ntdsdotsqlite.__main__:main']}
 
 setup_kwargs = {
     'name': 'ntdsdotsqlite',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'A small utility to get an SQLite  database from an NTDS.DIT file.',
     'long_description': '# NTDS.Sqlite\n\nThis software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.\n\n# Installation\n\n`python -m pip install ntdsdotsqlite`\n\n# Usage\n\n`ntdsdotsqlite NTDS.DIT --system SYSTEM -o NTDS.sqlite`\n\n```\nusage: NTDS.sqlite [-h] [--system SYSTEM] -o OUTFILE NTDS\n\nThis tool helps dumping NTDS.DIT file to an SQLite database\n\npositional arguments:\n  NTDS                  The NTDS.DIT file\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --system SYSTEM       The SYSTEM hive to decrypt hashes. If not provided, hashes will be encrypted inside the sqlite database.\n  -o OUTFILE, --outfile OUTFILE\n                        The sqlite database. Example : NTDS.sqlite\n```\n\n# SQL model\n\nThe SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !\n\n# Performances\n\nPerformances can be a bit low for huge NTDS files. The whole NTDS is not stored in memory to prevent memory exhaustion when working on huge files (NTDS databases can grow to several gigabytes).\n',
     'author': 'Virgile Jarry',
     'author_email': 'virgile@mailbox.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/almandin/ntdsdotsqlite',
```

### Comparing `ntdsdotsqlite-1.1.2/PKG-INFO` & `ntdsdotsqlite-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dissect[ese] (>=3.5,<4.0)
 Requires-Dist: impacket (>=0.10,<0.11)
+Requires-Dist: pycryptodomex (>=3.18.0,<4.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://github.com/almandin/ntdsdotsqlite/README.md
 Project-URL: Repository, https://github.com/almandin/ntdsdotsqlite
 Description-Content-Type: text/markdown
 
 # NTDS.Sqlite
```

