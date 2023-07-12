# Comparing `tmp/whoisdomain-1.20230627.3.tar.gz` & `tmp/whoisdomain-1.20230712.2.tar.gz`

## Comparing `whoisdomain-1.20230627.3.tar` & `whoisdomain-1.20230712.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/main.py
--rw-r--r--   0        0        0   131880 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/.gitignore
--rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/pyproject.toml
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.3/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/main.py
+-rw-r--r--   0        0        0   132217 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/.gitignore
+-rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/pyproject.toml
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/PKG-INFO
```

### Comparing `whoisdomain-1.20230627.3/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230712.2/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/_1_query.py` & `whoisdomain-1.20230712.2/whoisdomain/_1_query.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/_2_parse.py` & `whoisdomain-1.20230712.2/whoisdomain/_2_parse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230712.2/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/__init__.py` & `whoisdomain-1.20230712.2/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/exceptions.py` & `whoisdomain-1.20230712.2/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/main.py` & `whoisdomain-1.20230712.2/whoisdomain/main.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230712.2/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
 ZZ["edu"] = {
     "extend": "com",
     "registrant": r"Registrant:\s*(.+)",
     "creation_date": r"Domain record activated:\s?(.+)",
     "updated_date": r"Domain record last updated:\s?(.+)",
     "expiration_date": r"Domain expires:\s?(.+)",
-    "name_servers": r"Name Servers:\s?\t(.+)\n\t(.+)\n",
+    "name_servers": r"Name Servers:\s?(?:\t(.+)\n)(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?",
 }
 
 # estonian
 ZZ["ee"] = {
     "extend": "com",
     "domain_name": r"Domain:\nname:\s+(.+\.ee)\n",
     "registrar": r"Registrar:\nname:\s+(.+)\n",
@@ -1941,19 +1941,25 @@
 ZZ["my"] = {"extend": "_privateReg"}
 ZZ["pk"] = {"extend": "_privateReg"}
 ZZ["py"] = {"extend": "_privateReg"}  # Paraguay:https://www.iana.org/domains/root/db/py.html
 ZZ["com.py"] = {"extend": "_privateReg"}
 ZZ["sr"] = {"extend": "_privateReg"}
 
 # Kenia
+# ke : http://www.kenic.or.ke/index.php/en/ke-domains/ke-domains
 ZZ["ke"] = {"extend": "com", "_server": "whois.kenic.or.ke"}
-ZZ["co.ke"] = {"extend": "ke"}
-ZZ["or.ke"] = {"extend": "ke"}
 ZZ["ac.ke"] = {"extend": "ke"}
+ZZ["co.ke"] = {"extend": "ke"}
 ZZ["go.ke"] = {"extend": "ke"}
+ZZ["info.ke"] = {"extend": "ke"}
+ZZ["me.ke"] = {"extend": "ke"}
+ZZ["mobi.ke"] = {"extend": "ke"}
+ZZ["ne.ke"] = {"extend": "ke"}
+ZZ["or.ke"] = {"extend": "ke"}
+ZZ["sc.ke"] = {"extend": "ke"}
 
 # https://www.iana.org/domains/root/db/td.html
 # td = {"extend": "_privateReg"} # Chad (French: Tchad) made available for use in 1997.
 
 ZZ["tk"] = {"extend": "_privateReg"}
 ZZ["to"] = {"extend": "_privateReg"}  #
 ZZ["uy"] = {"extend": "_privateReg"}  # Uruguay
```

### Comparing `whoisdomain-1.20230627.3/.gitignore` & `whoisdomain-1.20230712.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/README.md` & `whoisdomain-1.20230712.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
  * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
  * withRedacted: bool = False has been added to query(), if set to True any redacted fields will now be shown also (also supported in the cli whoisdomain as --withRedacted)
  * a analizer directory is presend in the github repo that will be used to look for new IANA tls's currently unsupported but maching known whois servers
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
+## Notes for Mac users
+  * it has been observed that the default cli whois on Mac is showing each forward step in its output, this makes parsing the result very unreliable.
+  * using a brew install whois will give in general better results.
+
 ## Docker
  * docker pull mbootgithub/whoisdomain:latest
  * docker run mbootgithub/whoisdomain -V # show version
  * docker run mbootgithub/whoisdomain -d google.com # run one domain
  * docker run mbootgithub/whoisdomain -a # run all tld
  * docker run mbootgithub/whoisdomain -d google.com -j | jq -r . # run one domains , output in json and reformat with jq
  * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '.expiration_date' # output only expire date
@@ -198,8 +202,10 @@
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
-  * add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
+  * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
+  * 1.20230627.3 additional kenia second level domains
+  * 1.20230712.1 tld .edu now can have up to 10 nameservers; remove action on pull request
```

### Comparing `whoisdomain-1.20230627.3/pyproject.toml` & `whoisdomain-1.20230712.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230627.3/PKG-INFO` & `whoisdomain-1.20230712.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230627.3
+Version: 1.20230712.2
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -52,14 +52,18 @@
  * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
  * withRedacted: bool = False has been added to query(), if set to True any redacted fields will now be shown also (also supported in the cli whoisdomain as --withRedacted)
  * a analizer directory is presend in the github repo that will be used to look for new IANA tls's currently unsupported but maching known whois servers
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
+## Notes for Mac users
+  * it has been observed that the default cli whois on Mac is showing each forward step in its output, this makes parsing the result very unreliable.
+  * using a brew install whois will give in general better results.
+
 ## Docker
  * docker pull mbootgithub/whoisdomain:latest
  * docker run mbootgithub/whoisdomain -V # show version
  * docker run mbootgithub/whoisdomain -d google.com # run one domain
  * docker run mbootgithub/whoisdomain -a # run all tld
  * docker run mbootgithub/whoisdomain -d google.com -j | jq -r . # run one domains , output in json and reformat with jq
  * docker run mbootgithub/whoisdomain -d google.com -j | jq -r '.expiration_date' # output only expire date
@@ -219,8 +223,10 @@
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
-  * add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
+  * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
+  * 1.20230627.3 additional kenia second level domains
+  * 1.20230712.1 tld .edu now can have up to 10 nameservers; remove action on pull request
```

