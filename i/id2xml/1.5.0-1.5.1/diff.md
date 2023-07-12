# Comparing `tmp/id2xml-1.5.0.tar.gz` & `tmp/id2xml-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/id2xml-1.5.0.tar", last modified: Tue Sep  3 12:30:28 2019, max compression
+gzip compressed data, was "id2xml-1.5.1.tar", last modified: Wed Jul 12 19:43:14 2023, max compression
```

## Comparing `id2xml-1.5.0.tar` & `id2xml-1.5.1.tar`

### file list

```diff
@@ -1,58 +1,29 @@
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:28.000000 id2xml-1.5.0/
--rw-r--r--   0 henrik    (1000) henrik    (1000)     5923 2019-08-30 16:28:08.000000 id2xml-1.5.0/setup.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1167 2017-09-23 15:46:21.000000 id2xml-1.5.0/README.rst
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1507 2017-05-04 22:29:07.000000 id2xml-1.5.0/LICENSE
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/bin/
--rwxr-xr-x   0 henrik    (1000) henrik    (1000)     8251 2019-09-03 07:04:54.000000 id2xml-1.5.0/bin/mkrelease
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/
--rw-r--r--   0 henrik    (1000) henrik    (1000)        7 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/top_level.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)       43 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/entry_points.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)        1 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/dependency_links.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)        1 2017-05-28 12:53:31.000000 id2xml-1.5.0/id2xml.egg-info/not-zip-safe
--rw-r--r--   0 henrik    (1000) henrik    (1000)     4182 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/PKG-INFO
--rw-r--r--   0 henrik    (1000) henrik    (1000)       56 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/requires.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1515 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml.egg-info/SOURCES.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)       38 2019-09-03 12:30:28.000000 id2xml-1.5.0/setup.cfg
--rw-r--r--   0 henrik    (1000) henrik    (1000)     4351 2019-09-03 06:40:58.000000 id2xml-1.5.0/Makefile
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml/
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/id2xml/data/
--rw-r--r--   0 henrik    (1000) henrik    (1000)    51940 2017-05-04 22:29:07.000000 id2xml-1.5.0/id2xml/data/v3.rng
--rw-r--r--   0 henrik    (1000) henrik    (1000)    22756 2017-06-26 13:48:57.000000 id2xml-1.5.0/id2xml/data/v3.rnc
--rw-r--r--   0 henrik    (1000) henrik    (1000)     7330 2017-05-04 22:29:07.000000 id2xml-1.5.0/id2xml/data/v2.rnc
--rw-r--r--   0 henrik    (1000) henrik    (1000)    17351 2017-05-04 22:29:07.000000 id2xml-1.5.0/id2xml/data/v2.rng
--rw-r--r--   0 henrik    (1000) henrik    (1000)      201 2019-09-03 12:30:14.000000 id2xml-1.5.0/id2xml/__init__.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)    10748 2019-08-29 19:38:22.000000 id2xml-1.5.0/id2xml/run.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     6459 2018-12-31 16:08:43.000000 id2xml-1.5.0/id2xml/utils.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     6167 2017-05-18 22:58:32.000000 id2xml-1.5.0/id2xml/debug.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1391 2019-09-03 06:47:11.000000 id2xml-1.5.0/id2xml/id2xml.1.gz
--rw-r--r--   0 henrik    (1000) henrik    (1000)   130537 2019-09-03 06:55:51.000000 id2xml-1.5.0/id2xml/parser.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     4182 2019-09-03 12:30:28.000000 id2xml-1.5.0/PKG-INFO
--rw-r--r--   0 henrik    (1000) henrik    (1000)    20632 2019-09-03 12:30:14.000000 id2xml-1.5.0/changelog
--rw-r--r--   0 henrik    (1000) henrik    (1000)       43 2017-09-23 15:35:08.000000 id2xml-1.5.0/requirements.txt
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/test/
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:28.000000 id2xml-1.5.0/test/ok/
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1185 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-perc-dtls-tunnel-01.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)      293 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-netmod-revised-datastores-02.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)        0 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-baba-iot-problems-03.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     4154 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-jones-cose-rsa-03.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)      820 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-httpbis-header-structure-01.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)      410 2018-10-12 13:58:54.000000 id2xml-1.5.0/test/ok/rfc7842.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)    99454 2017-07-01 19:42:22.000000 id2xml-1.5.0/test/ok/draft-ietf-trill-directory-assist-mechanisms-12a.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)    14263 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-6man-rfc2460bis-11.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     4095 2017-07-01 19:42:22.000000 id2xml-1.5.0/test/ok/draft-nottingham-rfc5988bis-05.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1028 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-ospf-encapsulation-cap-02.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     2592 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-sparks-genarea-review-tracker-03.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     3729 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-mip4-multiple-tunnel-support-07.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     5760 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-curdle-cms-ecdh-new-curves-07.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)      383 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-i2nsf-client-facing-interface-req-01.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)   124436 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/rfc5661.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     2253 2018-10-12 13:58:54.000000 id2xml-1.5.0/test/ok/rfc7629.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     2633 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-sipcore-name-addr-guidance-01.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     3982 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-curdle-cms-eddsa-signatures-05.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     8481 2018-10-12 13:58:54.000000 id2xml-1.5.0/test/ok/draft-miek-test.diff
--rw-r--r--   0 henrik    (1000) henrik    (1000)     2077 2017-09-18 15:08:23.000000 id2xml-1.5.0/test/ok/draft-ietf-v6ops-rfc7084-bis-01.diff
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2019-09-03 12:30:27.000000 id2xml-1.5.0/test/in/
--rw-r--r--   0 henrik    (1000) henrik    (1000)   125741 2017-07-26 16:38:55.000000 id2xml-1.5.0/test/in/draft-ietf-trill-directory-assist-mechanisms-12a.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)    38466 2017-01-15 16:06:31.000000 id2xml-1.5.0/test/in/draft-ietf-mip4-multiple-tunnel-support-07.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)    31063 2017-05-14 21:08:48.000000 id2xml-1.5.0/test/in/draft-miek-test.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)      325 2018-12-25 16:13:32.000000 id2xml-1.5.0/MANIFEST.in
+drwxr-xr-x   0 kesara     (501) staff       (20)        0 2023-07-12 19:43:14.729301 id2xml-1.5.1/
+-rw-r--r--   0 kesara     (501) staff       (20)     1507 2023-07-12 19:39:27.000000 id2xml-1.5.1/LICENSE
+-rw-r--r--   0 kesara     (501) staff       (20)      325 2023-07-12 19:39:27.000000 id2xml-1.5.1/MANIFEST.in
+-rw-r--r--   0 kesara     (501) staff       (20)     4137 2023-07-12 19:39:27.000000 id2xml-1.5.1/Makefile
+-rw-r--r--   0 kesara     (501) staff       (20)     3176 2023-07-12 19:43:14.729179 id2xml-1.5.1/PKG-INFO
+-rw-r--r--   0 kesara     (501) staff       (20)     1167 2023-07-12 19:39:27.000000 id2xml-1.5.1/README.rst
+-rw-r--r--   0 kesara     (501) staff       (20)    20835 2023-07-12 19:39:27.000000 id2xml-1.5.1/changelog
+drwxr-xr-x   0 kesara     (501) staff       (20)        0 2023-07-12 19:43:14.727595 id2xml-1.5.1/id2xml/
+-rw-r--r--   0 kesara     (501) staff       (20)      202 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/__init__.py
+drwxr-xr-x   0 kesara     (501) staff       (20)        0 2023-07-12 19:43:14.728911 id2xml-1.5.1/id2xml/data/
+-rw-r--r--   0 kesara     (501) staff       (20)     7330 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/data/v2.rnc
+-rw-r--r--   0 kesara     (501) staff       (20)    17351 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/data/v2.rng
+-rw-r--r--   0 kesara     (501) staff       (20)    22756 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/data/v3.rnc
+-rw-r--r--   0 kesara     (501) staff       (20)    51940 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/data/v3.rng
+-rw-r--r--   0 kesara     (501) staff       (20)     6167 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/debug.py
+-rw-r--r--   0 kesara     (501) staff       (20)   130702 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/parser.py
+-rw-r--r--   0 kesara     (501) staff       (20)    10748 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/run.py
+-rw-r--r--   0 kesara     (501) staff       (20)     6459 2023-07-12 19:39:27.000000 id2xml-1.5.1/id2xml/utils.py
+drwxr-xr-x   0 kesara     (501) staff       (20)        0 2023-07-12 19:43:14.728325 id2xml-1.5.1/id2xml.egg-info/
+-rw-r--r--   0 kesara     (501) staff       (20)     3176 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/PKG-INFO
+-rw-r--r--   0 kesara     (501) staff       (20)      444 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/SOURCES.txt
+-rw-r--r--   0 kesara     (501) staff       (20)        1 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/dependency_links.txt
+-rw-r--r--   0 kesara     (501) staff       (20)       42 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/entry_points.txt
+-rw-r--r--   0 kesara     (501) staff       (20)        1 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/not-zip-safe
+-rw-r--r--   0 kesara     (501) staff       (20)       56 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/requires.txt
+-rw-r--r--   0 kesara     (501) staff       (20)        7 2023-07-12 19:43:14.000000 id2xml-1.5.1/id2xml.egg-info/top_level.txt
+-rw-r--r--   0 kesara     (501) staff       (20)       43 2023-07-12 19:39:27.000000 id2xml-1.5.1/requirements.txt
+-rw-r--r--   0 kesara     (501) staff       (20)       38 2023-07-12 19:43:14.729334 id2xml-1.5.1/setup.cfg
+-rw-r--r--   0 kesara     (501) staff       (20)     5923 2023-07-12 19:39:27.000000 id2xml-1.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `id2xml-1.5.0/setup.py` & `id2xml-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/README.rst` & `id2xml-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/LICENSE` & `id2xml-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/Makefile` & `id2xml-1.5.1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,21 @@
 	draft-ietf-httpbis-header-structure-01.txt		\
 	draft-ietf-i2nsf-client-facing-interface-req-01.txt	\
 	draft-ietf-mip4-multiple-tunnel-support-07.txt		\
 	draft-ietf-netmod-revised-datastores-02.txt		\
 	draft-ietf-ospf-encapsulation-cap-02.txt		\
 	draft-ietf-perc-dtls-tunnel-01.txt			\
 	draft-ietf-sipcore-name-addr-guidance-01.txt		\
-	draft-ietf-v6ops-rfc7084-bis-01.txt			\
 	draft-jones-cose-rsa-03.txt				\
 	draft-miek-test.txt					\
 	draft-sparks-genarea-review-tracker-03.txt		\
 	rfc5661.txt						\
 	rfc7629.txt						\
 	rfc7752.txt						\
 	rfc7842.txt						\
-	draft-ietf-curdle-cms-ecdh-new-curves-07.txt		\
-	draft-ietf-sidr-bgpsec-protocol-23mod.txt		\
-	draft-ietf-bess-evpn-vpws-14b.txt			\
-	draft-ietf-trill-rbridge-multilevel-07a.txt		\
 # draft-ietf-curdle-cms-ecdh-new-curves-07.txt is a modified copy, with
 # some reference fixes
 
 textfiles= $(addprefix test/in/, $(testfiles))
 resfiles = $(addprefix test/out/, $(testfiles))
 okfiles  = $(addprefix test/ok/, $(testfiles))
 origxml  = $(addsuffix .xml, $(basename $(okfiles)))
@@ -103,15 +98,15 @@
 test/out/%.raw: test/out/%.txt
 	id2xml --strip-only $< -o - | sed -r -e '/[Tt]able [Oo]f [Cc]ontents?/,/^[0-9]+\./d' > $@
 
 test/out/%.diff:	test/in/%.raw test/out/%.raw 
 	diff $(word 1,$^) $(word 2,$^) > $@ || true
 
 test/out/%.txt:	test/out/%.xml
-	xml2rfc $< -o $@
+	xml2rfc --legacy $< -o $@
 
 test/out/%.xml:	test/in/%.txt $(pyfiles)
 	@echo ""
 	id2xml $< -o $@
 
 test/out/%.v3.xml:	test/in/%.txt $(pyfiles)
 	@echo ""
```

### Comparing `id2xml-1.5.0/id2xml/data/v3.rng` & `id2xml-1.5.1/id2xml/data/v3.rng`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/data/v3.rnc` & `id2xml-1.5.1/id2xml/data/v3.rnc`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/data/v2.rnc` & `id2xml-1.5.1/id2xml/data/v2.rnc`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/data/v2.rng` & `id2xml-1.5.1/id2xml/data/v2.rng`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/run.py` & `id2xml-1.5.1/id2xml/run.py`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/utils.py` & `id2xml-1.5.1/id2xml/utils.py`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/debug.py` & `id2xml-1.5.1/id2xml/debug.py`

 * *Files identical despite different names*

### Comparing `id2xml-1.5.0/id2xml/parser.py` & `id2xml-1.5.1/id2xml/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1770,15 +1770,18 @@
             self.skip(line.txt)
         else:
             self.err(line.num, "Unrecognized copyright section title: '%s'" % line.txt)
         self.skip(boilerplate['base_copyright_header'] % date['year'])
         self.skip(boilerplate['base_copyright_body'])
         text = self.next_text()
         if text and text.startswith(boilerplate['ipr_200902_copyright_ietfbody'][:32]):
-            self.skip(boilerplate['ipr_200902_copyright_ietfbody'])
+            if 'Revised BSD' in text:
+                self.skip(boilerplate['ipr_200902_copyright_ietfbody'].replace('Simplified', 'Revised'))
+            else:
+                self.skip(boilerplate['ipr_200902_copyright_ietfbody'])
         text = self.next_text()
         if text and text.startswith(boilerplate['ipr_pre5378Trust200902_copyright'][:32]):
             self.skip(boilerplate['ipr_pre5378Trust200902_copyright'])
             self.root.set('ipr', 'pre5378Trust200902')
 
     @dtrace
     def read_authors_addresses(self):
```

### Comparing `id2xml-1.5.0/changelog` & `id2xml-1.5.1/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+id2xml (1.5.1) ietf; urgency=medium
+
+  * test: Improve tests (#14)
+
+  * fix: Parse boilerplate with revised BSD license (#13)
+
+ -- Kesara Rathnayake  <kesara@staff.ietf.org>  12 Jul 2023 21:47:44 +1200
+
 id2xml (1.5.0) ietf; urgency=medium
 
   * Fixed a few Python 3.x nits in the parser code.
 
   * Changed generated anchor slugs so as to not collide with IDs used by 
     xml2rfc, which in v3 mode reserves certain prefixes used for section, 
     figure and table anchors and fragment identifiers.  Also fixed an xml2rfc
```

