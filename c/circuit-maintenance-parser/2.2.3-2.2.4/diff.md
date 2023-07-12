# Comparing `tmp/circuit_maintenance_parser-2.2.3.tar.gz` & `tmp/circuit_maintenance_parser-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuit_maintenance_parser-2.2.3.tar", max compression
+gzip compressed data, was "circuit_maintenance_parser-2.2.4.tar", max compression
```

## Comparing `circuit_maintenance_parser-2.2.3.tar` & `circuit_maintenance_parser-2.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     7118 2023-03-21 14:44:54.855067 circuit_maintenance_parser-2.2.3/CHANGELOG.md
--rw-r--r--   0        0        0      533 2023-03-21 14:44:54.855067 circuit_maintenance_parser-2.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    10174 2023-03-21 14:44:54.855067 circuit_maintenance_parser-2.2.3/LICENSE
--rw-r--r--   0        0        0    20212 2023-03-21 14:44:54.855067 circuit_maintenance_parser-2.2.3/README.md
--rw-r--r--   0        0        0     2632 2023-03-21 14:44:54.859067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-21 14:44:54.859067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/cli.py
--rw-r--r--   0        0        0      124 2023-03-21 14:44:54.859067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/constants.py
--rwxr-xr-x   0        0        0  4395375 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/data/worldcities.csv
--rw-r--r--   0        0        0     4237 2023-03-21 14:44:54.859067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/data.py
--rw-r--r--   0        0        0      800 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/errors.py
--rw-r--r--   0        0        0     7562 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/output.py
--rw-r--r--   0        0        0     9381 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parser.py
--rw-r--r--   0        0        0        0 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/__init__.py
--rw-r--r--   0        0        0     2905 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/aquacomms.py
--rw-r--r--   0        0        0     3304 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/aws.py
--rw-r--r--   0        0        0     4248 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/bso.py
--rw-r--r--   0        0        0    10731 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/cogent.py
--rw-r--r--   0        0        0     3802 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/colt.py
--rw-r--r--   0        0        0     7224 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/equinix.py
--rw-r--r--   0        0        0     3438 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/gtt.py
--rw-r--r--   0        0        0     4574 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/hgc.py
--rw-r--r--   0        0        0     6373 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/lumen.py
--rw-r--r--   0        0        0     2812 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/megaport.py
--rw-r--r--   0        0        0     2826 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/momentum.py
--rw-r--r--   0        0        0     4305 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/seaborn.py
--rw-r--r--   0        0        0     3926 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/sparkle.py
--rw-r--r--   0        0        0     7922 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/telstra.py
--rw-r--r--   0        0        0     5014 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/turkcell.py
--rw-r--r--   0        0        0     3056 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/verizon.py
--rw-r--r--   0        0        0     6746 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/zayo.py
--rw-r--r--   0        0        0     7125 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/processor.py
--rw-r--r--   0        0        0        0 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/processors/__init__.py
--rw-r--r--   0        0        0    13684 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/provider.py
--rw-r--r--   0        0        0     5350 2023-03-21 14:44:54.883067 circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/utils.py
--rw-r--r--   0        0        0     2874 2023-03-21 14:45:04.491278 circuit_maintenance_parser-2.2.3/pyproject.toml
--rw-r--r--   0        0        0    21688 1970-01-01 00:00:00.000000 circuit_maintenance_parser-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     7251 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0      533 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    10174 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/LICENSE
+-rw-r--r--   0        0        0    20212 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/README.md
+-rw-r--r--   0        0        0     2632 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/__init__.py
+-rw-r--r--   0        0        0     2126 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/cli.py
+-rw-r--r--   0        0        0      124 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/constants.py
+-rwxr-xr-x   0        0        0  4395375 2023-07-12 16:20:37.859200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/data/worldcities.csv
+-rw-r--r--   0        0        0     4237 2023-07-12 16:20:37.831200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/data.py
+-rw-r--r--   0        0        0      800 2023-07-12 16:20:37.859200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/errors.py
+-rw-r--r--   0        0        0     7562 2023-07-12 16:20:37.859200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/output.py
+-rw-r--r--   0        0        0     9381 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parser.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/aquacomms.py
+-rw-r--r--   0        0        0     3304 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/aws.py
+-rw-r--r--   0        0        0     4248 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/bso.py
+-rw-r--r--   0        0        0    10731 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/cogent.py
+-rw-r--r--   0        0        0     3802 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/colt.py
+-rw-r--r--   0        0        0     7224 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/equinix.py
+-rw-r--r--   0        0        0     3438 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/gtt.py
+-rw-r--r--   0        0        0     4574 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/hgc.py
+-rw-r--r--   0        0        0     6373 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/lumen.py
+-rw-r--r--   0        0        0     2812 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/megaport.py
+-rw-r--r--   0        0        0     2826 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/momentum.py
+-rw-r--r--   0        0        0     4305 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/seaborn.py
+-rw-r--r--   0        0        0     3926 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/sparkle.py
+-rw-r--r--   0        0        0     7922 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/telstra.py
+-rw-r--r--   0        0        0     5014 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/turkcell.py
+-rw-r--r--   0        0        0     3056 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/verizon.py
+-rw-r--r--   0        0        0     6746 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/zayo.py
+-rw-r--r--   0        0        0     7125 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/processor.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/processors/__init__.py
+-rw-r--r--   0        0        0    13684 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/provider.py
+-rw-r--r--   0        0        0     5385 2023-07-12 16:20:37.863200 circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/utils.py
+-rw-r--r--   0        0        0     2886 2023-07-12 16:20:58.367389 circuit_maintenance_parser-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0    21449 1970-01-01 00:00:00.000000 circuit_maintenance_parser-2.2.4/PKG-INFO
```

### Comparing `circuit_maintenance_parser-2.2.3/CHANGELOG.md` & `circuit_maintenance_parser-2.2.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # Changelog
 
+## v2.2.4 - 2023-07-12
+
+- #230 - Swap out tzwhere for TimezoneFinder
+- #234 - Added upper bound to pydantic dependency
+
+### Changed
+
 ## v2.2.3 - 2023-03-21
 
 ### Changed
 
 - #216 - Allow Lumen maintenance multiple windows to be parsed
 - #212 - Updated documentation: Contribution section
 - #210 - Ability to parse multiple maintenance windows from Zayo
-- #190 - Update Telstra for new notificaiton format
+- #190 - Update Telstra for new notification format
 
 ### Fixed
 
 - #222 - Fix e22 tests when combining data from multiple maintenances
 
 ## v2.2.2 - 2023-01-27
```

### Comparing `circuit_maintenance_parser-2.2.3/CONTRIBUTING.md` & `circuit_maintenance_parser-2.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/LICENSE` & `circuit_maintenance_parser-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/README.md` & `circuit_maintenance_parser-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/__init__.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/cli.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/cli.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/data/worldcities.csv` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/data/worldcities.csv`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/data.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/data.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/errors.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/errors.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/output.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/output.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parser.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parser.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/aquacomms.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/aquacomms.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/aws.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/aws.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/bso.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/bso.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/cogent.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/cogent.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/colt.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/colt.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/equinix.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/equinix.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/gtt.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/gtt.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/hgc.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/hgc.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/lumen.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/lumen.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/megaport.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/megaport.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/momentum.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/momentum.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/seaborn.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/seaborn.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/sparkle.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/sparkle.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/telstra.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/telstra.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/turkcell.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/turkcell.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/verizon.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/verizon.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/parsers/zayo.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/parsers/zayo.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/processor.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/processor.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/provider.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/provider.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.2.3/circuit_maintenance_parser/utils.py` & `circuit_maintenance_parser-2.2.4/circuit_maintenance_parser/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import logging
 from typing import Tuple, Dict, Union
 import csv
 
 from geopy.exc import GeocoderUnavailable, GeocoderTimedOut, GeocoderServiceError  # type: ignore
 from geopy.geocoders import Nominatim  # type: ignore
-from tzwhere import tzwhere  # type: ignore
+from timezonefinder import TimezoneFinder  # type: ignore
 import backoff  # type: ignore
 
 from .errors import ParserError
 
 logger = logging.getLogger(__name__)
 
 dirname = os.path.dirname(__file__)
@@ -35,15 +35,15 @@
     _db_location: Dict[Union[Tuple[str, str], str], Tuple[float, float]] = {}
     _timezone = None
 
     @classproperty
     def timezone(cls):  # pylint: disable=no-self-argument
         """Load the timezone resolver."""
         if cls._timezone is None:
-            cls._timezone = tzwhere.tzwhere()
+            cls._timezone = TimezoneFinder()
             logger.info("Loaded local timezone resolver.")
         return cls._timezone
 
     @classproperty
     def db_location(cls):  # pylint: disable=no-self-argument
         """Load the locations DB from CSV into a Dict."""
         if not cls._db_location:
@@ -106,20 +106,20 @@
 
         Args:
             city (str): Geographic location name
         """
         if self.timezone is not None:
             try:
                 latitude, longitude = self.get_location(city)
-                timezone = self.timezone.tzNameAt(latitude, longitude)  # pylint: disable=no-member
+                timezone = self.timezone.timezone_at(lat=latitude, lng=longitude)  # pylint: disable=no-member
                 if not timezone:
                     # In some cases, given a latitued and longitued, the tzwhere library returns
                     # an empty timezone, so we try with the coordinates from the API as an alternative
                     latitude, longitude = self.get_location_from_api(city)
-                    timezone = self.timezone.tzNameAt(latitude, longitude)  # pylint: disable=no-member
+                    timezone = self.timezone.timezone_at(lat=latitude, lng=longitude)  # pylint: disable=no-member
 
                 if timezone:
                     logger.debug("Matched city %s to timezone %s", city, timezone)
                     return timezone
             except Exception as exc:
                 logger.error("Cannot obtain the timezone for city %s: %s", city, exc)
                 raise ParserError(  # pylint: disable=raise-missing-from
```

### Comparing `circuit_maintenance_parser-2.2.3/pyproject.toml` & `circuit_maintenance_parser-2.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuit-maintenance-parser"
-version = "v2.2.3"
+version = "v2.2.4"
 description = "Python library to parse Circuit Maintenance notifications and return a structured data back"
 authors = ["Network to Code <opensource@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/networktocode/circuit-maintenance-parser"
 repository = "https://github.com/networktocode/circuit-maintenance-parser"
 readme = "README.md"
 keywords = ["parser", "circuit", "maintenance"]
@@ -20,20 +20,20 @@
     "CONTRIBUTING.md",
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=7.1, <9.0"
-pydantic = {version = ">= 1.8.0, != 1.9.*, >= 1.10.4", extras = ["dotenv"]}
+pydantic = {version = ">= 1.8.0, != 1.9.*, >= 1.10.4, < 2", extras = ["dotenv"]}
 icalendar = "^5.0.0"
 bs4 = "^0.0.1"
 lxml = "^4.6.2"
 geopy = "^2.1.0"
-tzwhere = "^3.0.3"
+timezonefinder = "^6.0.1"
 backoff = "^1.11.1"
 chardet = "^5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 requests_mock = "^1.7.0"
 pyyaml = "^6.0"
```

### Comparing `circuit_maintenance_parser-2.2.3/PKG-INFO` & `circuit_maintenance_parser-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: circuit-maintenance-parser
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python library to parse Circuit Maintenance notifications and return a structured data back
 Home-page: https://github.com/networktocode/circuit-maintenance-parser
 License: Apache-2.0
 Keywords: parser,circuit,maintenance
 Author: Network to Code
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: chardet (>=5,<6)
 Requires-Dist: click (>=7.1,<9.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0)
 Requires-Dist: icalendar (>=5.0.0,<6.0.0)
 Requires-Dist: lxml (>=4.6.2,<5.0.0)
-Requires-Dist: pydantic[dotenv] (>=1.10.4)
-Requires-Dist: tzwhere (>=3.0.3,<4.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.4,<2)
+Requires-Dist: timezonefinder (>=6.0.1,<7.0.0)
 Project-URL: Repository, https://github.com/networktocode/circuit-maintenance-parser
 Description-Content-Type: text/markdown
 
 # circuit-maintenance-parser
 
 `circuit-maintenance-parser` is a Python library that parses circuit maintenance notifications from Network Service Providers (NSPs), converting heterogeneous formats to a well-defined structured format.
```

