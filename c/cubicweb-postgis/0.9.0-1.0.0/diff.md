# Comparing `tmp/cubicweb-postgis-0.9.0.tar.gz` & `tmp/cubicweb-postgis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-postgis-0.9.0.tar", last modified: Fri Apr  8 20:47:58 2022, max compression
+gzip compressed data, was "cubicweb-postgis-1.0.0.tar", last modified: Wed Jul 12 10:35:27 2023, max compression
```

## Comparing `cubicweb-postgis-0.9.0.tar` & `cubicweb-postgis-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.139644 cubicweb-postgis-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2792 2022-04-08 20:47:58.139644 cubicweb-postgis-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2157 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.127643 cubicweb-postgis-0.9.0/cubicweb_postgis/
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.135644 cubicweb-postgis-0.9.0/cubicweb_postgis/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      281 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.135644 cubicweb-postgis-0.9.0/cubicweb_postgis/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/migration/precreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.139644 cubicweb-postgis-0.9.0/cubicweb_postgis/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/schema/_ext.postgres.sql
--rw-rw-rw-   0 root         (0) root         (0)     8576 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/cubicweb_postgis/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.135644 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2792 2022-04-08 20:47:55.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2022-04-08 20:47:57.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-08 20:47:55.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-04-08 20:47:56.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-08 20:47:55.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2022-04-08 20:47:56.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-04-08 20:47:57.000000 cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-08 20:47:58.147644 cubicweb-postgis-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2659 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.139644 cubicweb-postgis-0.9.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:47:58.139644 cubicweb-postgis-0.9.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1149 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/test/test_postgis.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/test/test_schema_owl.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-08 20:46:33.000000 cubicweb-postgis-0.9.0/tox.ini
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.184730 cubicweb-postgis-1.0.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      497 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2772 2023-07-12 10:35:27.184730 cubicweb-postgis-1.0.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2157 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/README.rst
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/cubicweb_postgis/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      246 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      847 2023-07-07 11:56:50.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/__pkginfo__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/cubicweb_postgis/i18n/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      259 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/i18n/en.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      259 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/i18n/es.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      281 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/i18n/fr.po
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/cubicweb_postgis/migration/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1003 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/migration/precreate.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/cubicweb_postgis/schema/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1083 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/schema/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/schema/_ext.postgres.sql
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8569 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/site_cubicweb.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3378 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/cubicweb_postgis/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2772 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      734 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       44 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-03 14:05:46.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       17 2023-07-12 10:35:27.000000 cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-07-12 10:35:27.184730 cubicweb-postgis-1.0.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2627 2023-07-07 11:54:55.000000 cubicweb-postgis-1.0.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/test/
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 10:35:27.180729 cubicweb-postgis-1.0.0/test/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        8 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/test/data/bootstrap_cubes
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1125 2023-07-03 14:00:25.000000 cubicweb-postgis-1.0.0/test/data/schema.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3010 2023-07-07 11:54:55.000000 cubicweb-postgis-1.0.0/test/test_postgis.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1279 2023-07-07 11:54:55.000000 cubicweb-postgis-1.0.0/test/test_schema_owl.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1119 2023-07-12 10:34:53.000000 cubicweb-postgis-1.0.0/tox.ini
```

### Comparing `cubicweb-postgis-0.9.0/PKG-INFO` & `cubicweb-postgis-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-postgis
-Version: 0.9.0
+Version: 1.0.0
 Summary: Test for postgis
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-postgis
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -79,9 +78,7 @@
 	   'bottom': 48})
 
    # get all cities at a given distance from a point, sorted by distance
    rql('Any C, ST_DISTANCE(G, ST_SETSRID(ST_MAKEPOINT(2.2, 48.4), 4326)) '
        'ORDERBY 5 WHERE '
 	   'C geometry G HAVING ('
 	   ' ST_DWITHIN(G, ST_SETSRID(ST_MAKEPOINT(2.2, 48.4), 4326), 0.1) = TRUE)')
-
-
```

### Comparing `cubicweb-postgis-0.9.0/README.rst` & `cubicweb-postgis-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis/__pkginfo__.py` & `cubicweb-postgis-1.0.0/cubicweb_postgis/__pkginfo__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # pylint: disable=W0622
 """cubicweb-postgis application packaging information"""
 
-modname = 'postgis'
-distname = 'cubicweb-%s' % modname
+modname = "postgis"
+distname = f"cubicweb-{modname}"
 
-numversion = (0, 9, 0)
-version = '.'.join(str(num) for num in numversion)
+numversion = (1, 0, 0)
+version = ".".join(str(num) for num in numversion)
 
-license = 'LGPL'
-author = 'LOGILAB S.A. (Paris, FRANCE)'
-author_email = 'contact@logilab.fr'
-description = 'Test for postgis'
-web = 'https://forge.extranet.logilab.fr/cubicweb/cubes/%s' % distname
+license = "LGPL"
+author = "LOGILAB S.A. (Paris, FRANCE)"
+author_email = "contact@logilab.fr"
+description = "Test for postgis"
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    'cubicweb': ">= 3.26.19, < 3.38.0",
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.0.0, < 2.0.0",
 }
+
 __recommends__ = {}
 
 classifiers = [
-    'Environment :: Web Environment',
-    'Framework :: CubicWeb',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 2',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: JavaScript',
-    'Topic :: Scientific/Engineering :: GIS',
-    'Topic :: Database',
+    "Environment :: Web Environment",
+    "Framework :: CubicWeb",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: JavaScript",
+    "Topic :: Scientific/Engineering :: GIS",
+    "Topic :: Database",
 ]
```

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis/migration/precreate.py` & `cubicweb-postgis-1.0.0/cubicweb_postgis/migration/precreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis/schema/__init__.py` & `cubicweb-postgis-1.0.0/cubicweb_postgis/schema/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2012-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -15,15 +14,15 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """cubicweb-postgis schema"""
 from yams.buildobjs import make_type
 
 
-Geometry = make_type('Geometry')
+Geometry = make_type("Geometry")
 # Example of use:
 #     Geometry(geom_type='POINT', srid=-1, coord_dimension=2)
 
 
-Geography = make_type('Geography')
+Geography = make_type("Geography")
 # Example of use:
 #     Geography(geom_type='POINT', coord_dimension=2)
```

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis/site_cubicweb.py` & `cubicweb-postgis-1.0.0/cubicweb_postgis/site_cubicweb.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,346 +7,347 @@
 from yams import register_base_type
 
 from rql.utils import register_function
 
 from cubicweb_postgis import _GEOM_PARAMETERS, _GEOG_PARAMETERS
 
 # register new base type
-register_base_type(_('Geometry'), _GEOM_PARAMETERS)
-register_base_type(_('Geography'), _GEOG_PARAMETERS)
+register_base_type(_("Geometry"), _GEOM_PARAMETERS)
+register_base_type(_("Geography"), _GEOG_PARAMETERS)
 
 
 def pg_geometry_sqltype(rdef):
     """Return a PostgreSQL column type corresponding to rdef's geom_type, srid
     and coord_dimension.
     """
     target_geom_type = rdef.geom_type
-    if rdef.coord_dimension is not None and rdef.coord_dimension >= 3:  # XXX: handle 2D+M
-        target_geom_type += 'Z'
+    if (
+        rdef.coord_dimension is not None and rdef.coord_dimension >= 3
+    ):  # XXX: handle 2D+M
+        target_geom_type += "Z"
     if rdef.coord_dimension == 4:
-        target_geom_type += 'M'
+        target_geom_type += "M"
     assert target_geom_type
     assert rdef.srid
-    return 'geometry(%s, %s)' % (target_geom_type, rdef.srid)
+    return f"geometry({target_geom_type}, {rdef.srid})"
 
 
 def pg_geography_sqltype(rdef):
-    """Return a PostgreSQL column type corresponding to rdef's geom_type and srid
-    """
+    """Return a PostgreSQL column type corresponding to rdef's geom_type and srid"""
     srid = rdef.srid or 4326
-    return 'geography(%s, %s)' % (rdef.geom_type, srid)
+    return f"geography({rdef.geom_type}, {srid})"
 
 
 # Add the datatype to the helper mapping
-pghelper = get_db_helper('postgres')
-pghelper.TYPE_MAPPING['Geometry'] = pg_geometry_sqltype
-pghelper.TYPE_MAPPING['Geography'] = pg_geography_sqltype
-
-sqlitehelper = get_db_helper('sqlite')
-sqlitehelper.TYPE_MAPPING['Geometry'] = 'text'
-sqlitehelper.TYPE_MAPPING['Geography'] = 'text'
+pghelper = get_db_helper("postgres")
+pghelper.TYPE_MAPPING["Geometry"] = pg_geometry_sqltype
+pghelper.TYPE_MAPPING["Geography"] = pg_geography_sqltype
+
+sqlitehelper = get_db_helper("sqlite")
+sqlitehelper.TYPE_MAPPING["Geometry"] = "text"
+sqlitehelper.TYPE_MAPPING["Geography"] = "text"
 
 
 # Add a converter for Geometry
 def convert_geom(x):
     if isinstance(x, SQLExpression):
         return x
     if isinstance(x, (tuple, list)):
         # We give the (Geometry, SRID)
-        return SQLExpression('ST_GeomFromText(%(geo)s, %(srid)s)', geo=x[0], srid=x[1])
+        return SQLExpression("ST_GeomFromText(%(geo)s, %(srid)s)", geo=x[0], srid=x[1])
     # We just give the Geometry
-    return SQLExpression('ST_GeomFromText(%(geo)s, %(srid)s)', geo=x, srid=-1)
+    return SQLExpression("ST_GeomFromText(%(geo)s, %(srid)s)", geo=x, srid=-1)
 
 
 def convert_geog(x):
     # takes only a Geometry type, assumes GPS srid
-    return SQLExpression('ST_GeogFromText(%(geo)s)', geo=x)
+    return SQLExpression("ST_GeogFromText(%(geo)s)", geo=x)
 
 
 # Add the converter function to the known SQL_CONVERTERS
-pghelper.TYPE_CONVERTERS['Geometry'] = convert_geom
-pghelper.TYPE_CONVERTERS['Geography'] = convert_geog
+pghelper.TYPE_CONVERTERS["Geometry"] = convert_geom
+pghelper.TYPE_CONVERTERS["Geography"] = convert_geog
 
 # actually don't care of sqlite, it's just to make it possible to test
-sqlitehelper.TYPE_CONVERTERS['Geometry'] = str
-sqlitehelper.TYPE_CONVERTERS['Geography'] = str
+sqlitehelper.TYPE_CONVERTERS["Geometry"] = str
+sqlitehelper.TYPE_CONVERTERS["Geography"] = str
 
 
 class ST_EQUALS(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_INTERSECTS(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_INTERSECTION(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_OVERLAPS(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_CROSSES(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_TOUCHES(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_GEOMETRYN(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_WITHIN(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_CONTAINS(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_DWITHIN(FunctionDescr):
     minargs = 3
     maxargs = 4
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class ST_LENGTH(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_DISTANCE(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_DISTANCE_SPHERE(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_AREA(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_NUMINTERIORRINGS(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Int'
+    supported_backends = ("postgres",)
+    rtype = "Int"
 
 
 class ST_SIMPLIFY(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_TRANSFORM(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_ASGEOJSON(FunctionDescr):
     minargs = 1
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'String'
+    supported_backends = ("postgres",)
+    rtype = "String"
 
 
 class ST_AsEWKT(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'String'
+    supported_backends = ("postgres",)
+    rtype = "String"
 
 
 class ST_ASTEXT(FunctionDescr):
     minargs = 1
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'String'
+    supported_backends = ("postgres",)
+    rtype = "String"
 
 
 class ST_GEOMFROMTEXT(FunctionDescr):
     minargs = 1
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_GEOGFROMTEXT(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geography'
+    supported_backends = ("postgres",)
+    rtype = "Geography"
 
 
 class ST_COVERS(FunctionDescr):
     minargs = 1
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Bool'
+    supported_backends = ("postgres",)
+    rtype = "Bool"
 
 
 class GEOMETRY(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_UNION(FunctionDescr):
     aggregat = True
     minargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_COLLECT(FunctionDescr):
     aggregat = True
     minargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_CONVEXHULL(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_CONCAVEHULL(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class DISPLAY(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'String'
+    supported_backends = ("postgres",)
+    rtype = "String"
 
     def as_sql_postgres(self, args):
-        return 'ST_ASGeoJSON(ST_Transform(%s, %s))' % (args[0], args[1])
+        return f"ST_ASGeoJSON(ST_Transform({args[0]}, {args[1]}))"
 
 
 class ST_MAKEPOINT(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_SRID(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_SETSRID(FunctionDescr):
     minargs = 2
     maxargs = 2
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_X(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_Y(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_Z(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_M(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Float'
+    supported_backends = ("postgres",)
+    rtype = "Float"
 
 
 class ST_EXTENT(AggrFunctionDescr):
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_MAKEENVELOPE(FunctionDescr):
     minargs = 4
     maxargs = 5
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 class ST_CENTROID(FunctionDescr):
     minargs = 1
     maxargs = 1
-    supported_backends = ('postgres',)
-    rtype = 'Geometry'
+    supported_backends = ("postgres",)
+    rtype = "Geometry"
 
 
 register_function(ST_EQUALS)
 register_function(ST_INTERSECTS)
 register_function(ST_INTERSECTION)
 register_function(ST_OVERLAPS)
 register_function(ST_CROSSES)
```

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/PKG-INFO` & `cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-postgis
-Version: 0.9.0
+Version: 1.0.0
 Summary: Test for postgis
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-postgis
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -79,9 +78,7 @@
 	   'bottom': 48})
 
    # get all cities at a given distance from a point, sorted by distance
    rql('Any C, ST_DISTANCE(G, ST_SETSRID(ST_MAKEPOINT(2.2, 48.4), 4326)) '
        'ORDERBY 5 WHERE '
 	   'C geometry G HAVING ('
 	   ' ST_DWITHIN(G, ST_SETSRID(ST_MAKEPOINT(2.2, 48.4), 4326), 0.1) = TRUE)')
-
-
```

### Comparing `cubicweb-postgis-0.9.0/cubicweb_postgis.egg-info/SOURCES.txt` & `cubicweb-postgis-1.0.0/cubicweb_postgis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-postgis-0.9.0/setup.py` & `cubicweb-postgis-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,57 +27,56 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_postgis', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_postgis", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'postgis=cubicweb_postgis',
+        "cubicweb.cubes": [
+            "postgis=cubicweb_postgis",
         ],
     },
     zip_safe=False,
-    python_requires='>=2.7',
+    python_requires=">=2.7",
 )
```

### Comparing `cubicweb-postgis-0.9.0/test/test_postgis.py` & `cubicweb-postgis-1.0.0/test/test_postgis.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """cubicweb-postgis tests
 """
 
 from cubicweb.devtools import testlib
-from cubicweb.devtools import (startpgcluster, stoppgcluster,
-                               PostgresApptestConfiguration)
+from cubicweb.devtools import (
+    startpgcluster,
+    stoppgcluster,
+)
+from cubicweb.devtools.apptest_config import PostgresApptestConfiguration
 
 
 def setUpModule():
     startpgcluster(__file__)
 
 
 def tearDownModule():
@@ -31,39 +34,55 @@
 
 
 class PostgisTC(testlib.CubicWebTC):
     configcls = PostgresApptestConfiguration
 
     def test_geometry_srid(self):
         with self.admin_access.repo_cnx() as cnx:
-            cnx.create_entity('City', name=u'Paris', center_4326=(u'POINT(2.34 48.4)', 4326))
+            cnx.create_entity(
+                "City", name="Paris", center_4326=("POINT(2.34 48.4)", 4326)
+            )
             cnx.commit()
-            self.assertEqual(cnx.execute('Any ST_SRID(C) WHERE X center_4326 C')[0][0], 4326)
+            self.assertEqual(
+                cnx.execute("Any ST_SRID(C) WHERE X center_4326 C")[0][0], 4326
+            )
             # wrong srid
             with self.assertRaises(Exception) as ctx:
-                cnx.create_entity('City', name=u'Nantes', center_4326=(u'POINT(1.5 47.25)', -1))
+                cnx.create_entity(
+                    "City", name="Nantes", center_4326=("POINT(1.5 47.25)", -1)
+                )
             # psycopg2 < 2.8 raises DataError
             # psycopg2 >= 2.8 raises InvalidParameterValue
-            self.assertIn(ctx.exception.__class__.__name__, ('DataError', 'InvalidParameterValue'))
+            self.assertIn(
+                ctx.exception.__class__.__name__, ("DataError", "InvalidParameterValue")
+            )
 
     def test_geometry_nosrid(self):
         with self.admin_access.repo_cnx() as cnx:
-            cnx.create_entity('City', name=u'Paris', center_nosrid=(u'POINT(2.34 48.4)', 4326))
+            cnx.create_entity(
+                "City", name="Paris", center_nosrid=("POINT(2.34 48.4)", 4326)
+            )
             cnx.commit()
-            self.assertEqual(cnx.execute('Any ST_SRID(C) WHERE X center_nosrid C')[0][0], 4326)
-            cnx.create_entity('City', name=u'Nantes', center_nosrid=(u'POINT(1.5 47.25)', -1))
+            self.assertEqual(
+                cnx.execute("Any ST_SRID(C) WHERE X center_nosrid C")[0][0], 4326
+            )
+            cnx.create_entity(
+                "City", name="Nantes", center_nosrid=("POINT(1.5 47.25)", -1)
+            )
             cnx.commit()
 
 
 class PostgisSQLiteFakeTC(testlib.CubicWebTC):
-
     def test_schema(self):
-        sqlqs = "select sql from sqlite_master where type = 'table' and name = 'cw_City'"
+        sqlqs = (
+            "select sql from sqlite_master where type = 'table' and name = 'cw_City'"
+        )
         with self.admin_access.repo_cnx() as cnx:
-            self.assertTrue(cnx.find('CWEType', name=u'Geometry'))
+            self.assertTrue(cnx.find("CWEType", name="Geometry"))
             city_schema = cnx.system_sql(sqlqs).fetchall()[0][0]
-            self.assertIn('cw_center_4326 text', city_schema)
+            self.assertIn("cw_center_4326 text", city_schema)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

### Comparing `cubicweb-postgis-0.9.0/test/test_schema_owl.py` & `cubicweb-postgis-1.0.0/test/test_schema_owl.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <https://www.gnu.org/licenses/>.
 
 
 from xml.dom.minidom import parseString as parseXmlString
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class OWLViewTC(CubicWebTC):
-
+class OWLViewTC(WebCWTC):
     def test_owl_schema_valid_xml(self):
-        with self.new_access('admin').web_request() as req:
-            pageinfo = self.view('owl', req=req)
-            self.assertIn('owl', pageinfo.source.decode('utf-8'))
+        with self.new_access("admin").web_request() as req:
+            pageinfo = self.view("owl", req=req)
+            self.assertIn("owl", pageinfo.source.decode("utf-8"))
             self.assertTrue(parseXmlString(pageinfo.source))
 
 
 if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

### Comparing `cubicweb-postgis-0.9.0/tox.ini` & `cubicweb-postgis-1.0.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tox]
-envlist = py3, flake8, check-manifest, yamllint
+envlist = py3, flake8, check-manifest, yamllint, black
 
 [testenv]
 deps =
   psycopg2-binary
   pytest
+  webtest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
 
 [testenv:flake8]
 skip_install = true
 deps =
@@ -28,15 +29,15 @@
 
 [pytest]
 python_files = *test_*.py
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -46,7 +47,21 @@
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
 
+
+[testenv:black]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black --check .
+
+[testenv:black-run]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black .
```

