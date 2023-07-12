# Comparing `tmp/coc.py-2.4.1.tar.gz` & `tmp/coc.py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc.py-2.4.1.tar", last modified: Thu May 18 19:36:05 2023, max compression
+gzip compressed data, was "coc.py-3.0.0.tar", last modified: Wed Jul 12 16:06:03 2023, max compression
```

## Comparing `coc.py-2.4.1.tar` & `coc.py-3.0.0.tar`

### file list

```diff
@@ -1,61 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.229443 coc.py-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 19:35:54.000000 coc.py-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 19:35:54.000000 coc.py-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-18 19:36:05.229443 coc.py-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-18 19:35:54.000000 coc.py-2.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (123)    80631 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.221443 coc.py-2.4.1/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.229443 coc.py-2.4.1/coc/static/
--rw-r--r--   0 runner    (1001) docker     (123)   135500 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (123)   271286 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   130902 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/object_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    43766 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (123)    53705 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (123)   575079 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 19:35:54.000000 coc.py-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 19:35:54.000000 coc.py-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:36:05.229443 coc.py-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 19:35:54.000000 coc.py-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.561758 coc.py-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 16:05:33.000000 coc.py-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 16:05:33.000000 coc.py-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-12 16:06:03.561758 coc.py-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-12 16:05:33.000000 coc.py-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.533758 coc.py-3.0.0/coc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83126 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39787 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.529758 coc.py-3.0.0/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.533758 coc.py-3.0.0/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.533758 coc.py-3.0.0/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.533758 coc.py-3.0.0/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23265 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21407 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19577 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.561758 coc.py-3.0.0/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1195393 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1592822 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   576615 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (123)   179971 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (123)   412500 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (123) 21604615 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82024 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-07-12 16:05:33.000000 coc.py-3.0.0/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:06:03.533758 coc.py-3.0.0/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-12 16:06:03.000000 coc.py-3.0.0/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-12 16:06:03.000000 coc.py-3.0.0/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:06:03.000000 coc.py-3.0.0/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 16:06:03.000000 coc.py-3.0.0/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 16:06:03.000000 coc.py-3.0.0/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-12 16:05:33.000000 coc.py-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 16:05:33.000000 coc.py-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:06:03.561758 coc.py-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 16:05:33.000000 coc.py-3.0.0/setup.py
```

### Comparing `coc.py-2.4.1/LICENSE` & `coc.py-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/PKG-INFO` & `coc.py-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.4.1
+Version: 3.0.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-2.4.1/README.rst` & `coc.py-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/__init__.py` & `coc.py-3.0.0/coc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "2.4.1"
+__version__ = "3.0.0"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
@@ -50,15 +50,14 @@
     InvalidArgument,
     InvalidCredentials,
     Forbidden,
     Maintenance,
     GatewayError,
     PrivateWarLog,
 )
-from .login import login, login_with_keys
 from .hero import Hero, Pet
 from .http import BasicThrottler, BatchThrottler, HTTPClient
 from .iterators import (
     ClanIterator,
     PlayerIterator,
     ClanWarIterator,
     LeagueWarIterator,
@@ -74,15 +73,15 @@
     LegendStatistics,
     LoadGameData,
     Location,
     PlayerHouseElement,
     Timestamp,
     TimeDelta,
     Label,
-    WarLeague,
+    BaseLeague
 )
 from .players import Player, ClanMember, RankedPlayer
 from .player_clan import PlayerClan
 from .raid import RaidClan, RaidMember, RaidLogEntry, RaidDistrict, RaidAttack
 from .spell import Spell
 from .troop import Troop
 from .war_clans import WarClan, ClanWarLeagueClan
```

### Comparing `coc.py-2.4.1/coc/abc.py` & `coc.py-3.0.0/coc/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         cls.range = try_enum(UnitStat, troop_meta.get("AttackRange"))
         cls.dps = try_enum(UnitStat, troop_meta.get("DPS"))
         cls.ground_target = _get_maybe_first(troop_meta, "GroundTargets",
                                              default=True)
         cls.hitpoints = try_enum(UnitStat, troop_meta.get("Hitpoints"))
 
         # get production building
-        production_building = troop_meta.get("ProductionBuilding", [None])[0]
+        production_building = troop_meta.get("ProductionBuilding", [None])[0] if troop_meta.get("ProductionBuilding") else None
         if production_building == "Barrack":
             cls.is_elixir_troop = True
         elif production_building == "Dark Elixir Barrack":
             cls.is_dark_troop = True
         elif production_building == "SiegeWorkshop":
             cls.is_siege_machine = True
         elif production_building == "Spell Forge":
@@ -322,43 +322,49 @@
 
     FILE_PATH = NotImplemented
     data_object = NotImplemented
 
     def __init__(self):
         self.loaded = False
 
-    def _load_json(self, object_ids, english_aliases, lab_to_townhall):
+    def _load_json(self, english_aliases, lab_to_townhall):
         with open(self.FILE_PATH) as fp:
             data = ujson.load(fp)
 
+        id = 2000
         for c, [supercell_name, meta] in enumerate(data.items()):
+
             # Not interested if it doesn't have a TID, since it likely isn't a real troop.
             if not meta.get("TID"):
                 continue
 
             # Some duplication with tutorial goblins and barbs which we don't care about
             if "Tutorial" in supercell_name:
                 continue
 
             # SC game files have "DisableProduction" true for all pet objects, which we want
-            if "DisableProduction" in meta and "pets" not in str(
-                    self.FILE_PATH):
+            if True in meta.get("DisableProduction", [False]) and "pets" not in str(self.FILE_PATH):
+                continue
+
+            #hacky but the aliases convert so that isnt great
+            IGNORED_PETS = ["Unused", "PhoenixEgg"]
+            if "pets" in str(self.FILE_PATH) and supercell_name in IGNORED_PETS:
                 continue
 
             # A bit of a hacky way to create a "copy" of a new Troop object that hasn't been initiated yet.
             new_item = type(self.data_object.__name__,
                             self.data_object.__bases__,
                             dict(self.data_object.__dict__))
             new_item._load_json_meta(
                 meta,
-                id=object_ids.get(supercell_name, c),
-                name=english_aliases[meta["TID"][0]][0],
+                id=id,
+                name=english_aliases[meta["TID"][0]]["EN"][0],
                 lab_to_townhall=lab_to_townhall,
             )
-
+            id += 1
             self.items.append(new_item)
             self.item_lookup[new_item.name] = new_item
 
         self.loaded = True
 
     def load(
             self, data: dict, townhall: int, default: Type[DataContainer] = None,
```

### Comparing `coc.py-2.4.1/coc/clans.py` & `coc.py-3.0.0/coc/clans.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import typing
 
 
 from .players import ClanMember
-from .miscmodels import try_enum, ChatLanguage, Location, Label, WarLeague, CapitalDistrict
+from .miscmodels import try_enum, ChatLanguage, Location, Label, BaseLeague, CapitalDistrict
 from .utils import get, cached_property, correct_tag
 from .abc import BaseClan
 
 
 class RankedClan(BaseClan):
     """Represents the clan object returned by leader-board rankings.
 
@@ -44,44 +44,46 @@
     level: :class:`int`
         The clan's level.
     location: :class:`Location`
         The clan's location.
     member_count: :class:`int`
         The number of members in the clan.
     points: :class:`int`
-        The clan's trophy-count. If retrieving info for capital or versus leader-boards, this will be ``None``.
-    versus_points: :class:`int`
-        The clan's versus trophy count. If retrieving info for regular or capital leader boards, this will be ``None``.
+        The clan's trophy-count. If retrieving info for capital or builder base leader-boards, this will be ``None``.
+    builder_base_points: :class:`int`
+        The clan's builder base trophy count. If retrieving info for regular or capital leader boards, this will be
+        ``None``.
     capital_points: :class:`int`
-        The clan's capital trophy count. If retrieving info for regular or versus leader boards, this will be ``None``.
+        The clan's capital trophy count. If retrieving info for regular or builder base leader boards, this will be
+        ``None``.
     rank: :class:`int`
         The clan's rank in the leader board.
     previous_rank: :class:`int`
         The clan's rank in the previous season's leaderboard.
     """
 
     __slots__ = (
         "location",
         "member_count",
         "points",
-        "versus_points",
+        "builder_base_points",
         "capital_points",
         "rank",
         "previous_rank",
     )
 
     def __init__(self, *, data, client, **_):
         super().__init__(data=data, client=client)
         self._from_data(data)
 
     def _from_data(self, data: dict) -> None:
         data_get = data.get
 
         self.points: int = data_get("clanPoints")
-        self.versus_points: int = data_get("clanVersusPoints")
+        self.builder_base_points: int = data_get("clanBuilderBasePoints")
         self.capital_points: int = data_get("clanCapitalPoints")
         self.member_count: int = data_get("members")
         self.location = try_enum(Location, data=data_get("location"))
         self.rank: int = data_get("rank")
         self.previous_rank: int = data_get("previousRank")
 
 
@@ -106,33 +108,35 @@
         Indicates the clan's family friendly status. This can be True if family friendly, or False if not.
     description: :class:`str`
         The clan's public description.
     location: :class:`Location`
         The clan's location.
     points: :class:`int`
         The clan's trophy count. This is calculated according to members' trophy counts.
-    versus_points: :class:`int`
-        The clan's versus trophy count. This is calculated according to members' versus trophy counts.
+    builder_base_points: :class:`int`
+        The clan's builder base trophy count. This is calculated according to members' builder base trophy counts.
     capital_points: :class:`int`
         The clan's clan capital points. Unsure how this is calculated.
     required_trophies: :class:`int`
         The minimum trophies required to apply to this clan.
+    required_builder_base_trophies: :class:`int`
+        The minimum builder base trophies required to apply to this clan.
     required_townhall: :class:`int`
         The minimum townhall level required to apply to this clan.
     war_frequency: :class:`str`
         The frequency for when this clan goes to war.
         For example, this could be ``always``.
     war_win_streak: :class:`int`
         The clan's current war winning streak.
     war_wins: :class:`int`
         The number of wars the clan has won.
     war_ties: :class:`int`
-        The number of wars the clan has tied.
+        The number of wars the clan has tied. This is only available from the clan search endpoint else -1.
     war_losses: :class:`int`
-        The number of wars the clan has lost.
+        The number of wars the clan has lost.  This is only available from the clan search endpoint else -1.
     public_war_log: :class:`bool`
         Indicates if the clan has a public war log.
         If this is ``False``, operations to find the clan's current
         war may raise :exc:`PrivateWarLog`.
     member_count: :class:`int`
         The number of members in the clan.
     label_cls: :class:`coc.Label`
@@ -141,29 +145,30 @@
     member_cls: :class:`coc.ClanMember`
         The type which the members found in :attr:`Clan.members` will be of.
         Ensure any overriding of this inherits from :class:`coc.ClanMember`.
     capital_district_cls: :class:`coc.CapitalDistrict`
         The type which the clan capital districts found in
         :attr:`Clan.capital_districts` will be of. Ensure any overriding of
         this inherits from :class:`coc.CapitalDistrict`.
-    war_league: :class:`coc.WarLeague`
+    war_league: :class:`coc.BaseLeague`
         The clan's CWL league.
-    capital_league: :class:`coc.WarLeague`
+    capital_league: :class:`coc.BaseLeague`
         The clan's Clan Capital league.
     """
 
     __slots__ = (
         "type",
         "family_friendly",
         "description",
         "location",
         "points",
-        "versus_points",
+        "builder_base_points",
         "capital_points",
         "required_trophies",
+        "required_builder_base_trophies",
         "war_frequency",
         "war_win_streak",
         "war_wins",
         "war_ties",
         "war_losses",
         "public_war_log",
         "member_count",
@@ -196,43 +201,44 @@
 
         self._from_data(data)
 
     def _from_data(self, data: dict) -> None:
         data_get = data.get
 
         self.points: int = data_get("clanPoints")
-        self.versus_points: int = data_get("clanVersusPoints")
+        self.builder_base_points: int = data_get("clanBuilderBasePoints")
         self.capital_points: int = data_get("clanCapitalPoints")
         self.member_count: int = data_get("members")
         self.location = try_enum(Location, data=data_get("location"))
 
         # only available via /clans/{clanTag} or /clans endpoint
         self.type: str = data_get("type")
         self.family_friendly = data_get("isFamilyFriendly")
         self.required_trophies: int = data_get("requiredTrophies")
+        self.required_builder_base_trophies: int = data_get("requiredBuilderBaseTrophies")
         self.war_frequency: str = data_get("warFrequency")
         self.war_win_streak: int = data_get("warWinStreak")
         self.war_wins: int = data_get("warWins")
-        self.war_ties: int = data_get("warTies")
-        self.war_losses: int = data_get("warLosses")
+        self.war_ties: int = data_get("warTies", -1)
+        self.war_losses: int = data_get("warLosses", -1)
         self.public_war_log: bool = data_get("isWarLogPublic")
         self.description: str = data_get("description")
-        self.war_league = try_enum(WarLeague, data=data_get("warLeague"))
-        self.capital_league = try_enum(WarLeague, data=data_get("capitalLeague"))
+        self.war_league = try_enum(BaseLeague, data=data_get("warLeague"))
+        self.capital_league = try_enum(BaseLeague, data=data_get("capitalLeague"))
         self.chat_language = try_enum(ChatLanguage, data=data_get("chatLanguage"))
         self.required_townhall = data_get("requiredTownhallLevel")
 
         label_cls = self.label_cls
         self._iter_labels = (label_cls(data=ldata, client=self._client) for ldata in data_get("labels", []))
 
         # update members globally. only available via /clans/{clanTag}
         member_cls = self.member_cls
         member_data = data.get("memberList", [])
-        for rank, mdata in enumerate(sorted(member_data, key=lambda x: x["versusTrophies"], reverse=True), 1):
-            mdata["versusRank"] = rank
+        for rank, mdata in enumerate(sorted(member_data, key=lambda x: x["builderBaseTrophies"], reverse=True), 1):
+            mdata["builderBaseRank"] = rank
         self._iter_members = (
             member_cls(data=mdata, client=self._client, clan=self) for mdata in member_data
         )
 
         capital_district_cls = self.capital_district_cls
         if data_get("clanCapital"):
             self._iter_capital_districts = (capital_district_cls(data=cddata, client=self._client) for cddata in
```

### Comparing `coc.py-2.4.1/coc/client.py` & `coc.py-3.0.0/coc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from typing import AsyncIterator, Iterable, List, Optional, Type, Union, TYPE_CHECKING
 
 import ujson
 
 from .clans import Clan, RankedClan
 from .errors import Forbidden, GatewayError, NotFound, PrivateWarLog
 from .enums import WarRound
-from .miscmodels import GoldPassSeason, Label, League, Location, LoadGameData
+from .miscmodels import BaseLeague, GoldPassSeason, Label, League, Location, LoadGameData
 from .hero import HeroHolder, PetHolder
 from .http import HTTPClient, BasicThrottler, BatchThrottler
 from .iterators import (
     PlayerIterator,
     ClanIterator,
     ClanWarIterator,
     LeagueWarIterator,
@@ -59,15 +59,14 @@
 
 
 LOG = logging.getLogger(__name__)
 
 LEAGUE_WAR_STATE = "notInWar"
 KEY_MINIMUM, KEY_MAXIMUM = 1, 10
 
-OBJECT_IDS_PATH = Path(__file__).parent.joinpath(Path("static/object_ids.json"))
 ENGLISH_ALIAS_PATH = Path(__file__).parent.joinpath(Path("static/texts_EN.json"))
 BUILDING_FILE_PATH = Path(__file__).parent.joinpath(Path("static/buildings.json"))
 
 
 class ClashAccountScopes(Enum):
     """
     Values represent the scope required for each type of user. A USER is
@@ -240,17 +239,14 @@
             throttle_limit=self.throttle_limit,
             throttler=self.throttler,
             cache_max_size=self.cache_max_size,
             stats_max_size=self.stats_max_size,
         )
 
     def _load_holders(self):
-        with open(OBJECT_IDS_PATH) as fp:
-            object_ids = {v: k for k, v in ujson.load(fp).items()}
-
         with open(ENGLISH_ALIAS_PATH) as fp:
             english_aliases = ujson.load(fp)
 
         with open(BUILDING_FILE_PATH) as fp:
             buildings = ujson.load(fp)
 
         for supercell_name, data in buildings.items():
@@ -261,15 +257,15 @@
                 lab_to_townhall[0] = 2
                 break
         else:
             # if the files failed to load, fallback to the old formula of lab level = TH level - 2
             lab_to_townhall = {i-2: i for i in range(1, 15)}
 
         for holder in (self._troop_holder, self._spell_holder, self._hero_holder, self._pet_holder):
-            holder._load_json(object_ids, english_aliases, lab_to_townhall)
+            holder._load_json(english_aliases, lab_to_townhall)
 
     def _create_holders(self):
         self._troop_holder, self._spell_holder, self._hero_holder, self._pet_holder = TroopHolder(), \
                                                                                       SpellHolder(), \
                                                                                       HeroHolder(), \
                                                                                       PetHolder()
 
@@ -578,15 +574,15 @@
             args['after'] = after
         if before:
             args['before'] = before
 
         data = await self.http.get_clan_members(clan_tag, **args)
         return [cls(data=mdata, client=self, **kwargs) for mdata in data.get("memberList", [])]
 
-    async def get_warlog(
+    async def get_war_log(
         self,
         clan_tag: str,
         cls: Type[ClanWarLogEntry] = ClanWarLogEntry,
         page: bool = False,
         *,
         limit: int = 0,
         after: str = "",
@@ -677,15 +673,15 @@
                                              model=cls,
                                              after=after,
                                              before=before)
         except Forbidden as exception:
             raise PrivateWarLog(exception.response,
                                 exception.reason) from exception
 
-    async def get_raidlog(
+    async def get_raid_log(
             self,
             clan_tag: str,
             cls: Type[RaidLogEntry] = RaidLogEntry,
             page: bool = False,
             *,
             limit: int = 0,
             after: str = "",
@@ -1122,15 +1118,15 @@
         except PrivateWarLog:
             get_war = None
 
         if get_war and get_war.state != LEAGUE_WAR_STATE:
             return get_war
 
         try:
-            league_group = await self.get_league_group(clan_tag,**kwargs)
+            league_group = await self.get_league_group(clan_tag, **kwargs)
         except (NotFound, GatewayError) as exception:
             # either they're not in cwl (NotFound)
             # or it's an API bug where league group endpoint will timeout when the clan is searching (GatewayError)
             if get_war is None:
                 raise PrivateWarLog(exception.response, exception.reason) from exception
             return get_war
 
@@ -1440,19 +1436,19 @@
             The top players for the requested location.
         """
         if not issubclass(cls, RankedPlayer):
             raise TypeError("cls must be a subclass of RankedPlayer.")
         data = await self.http.get_location_players(location_id, limit=limit, before=before, after=after)
         return [cls(data=n, client=self) for n in data["items"]]
 
-    async def get_location_clans_versus(
+    async def get_location_clans_builder_base(
         self, location_id: int = "global", *, limit: int = None,
             before: str = None, after: str = None, cls: Type[RankedClan] = RankedClan
     ) -> List[RankedClan]:
-        """Get clan versus rankings for a specific location
+        """Get clan builder base rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (global).
         limit : int
             The number of results to fetch.
@@ -1474,26 +1470,26 @@
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedClan`]
-            The top versus-clans for the requested location.
+            The top builder base-clans for the requested location.
         """
         if not issubclass(cls, RankedClan):
             raise TypeError("cls must be a subclass of RankedClan.")
-        data = await self.http.get_location_clans_versus(location_id, limit=limit, before=before, after=after)
+        data = await self.http.get_location_clans_builder_base(location_id, limit=limit, before=before, after=after)
         return [cls(data=n, client=self) for n in data["items"]]
 
-    async def get_location_players_versus(
+    async def get_location_players_builder_base(
         self, location_id: int = "global", *, limit: int = None,
             before: str = None, after: str = None, cls: Type[RankedPlayer] = RankedPlayer
     ) -> List[RankedPlayer]:
-        """Get player versus rankings for a specific location
+        """Get player builder base rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (global).
         limit : int
             The number of results to fetch.
@@ -1515,19 +1511,19 @@
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedPlayer`]
-            The top versus players for the requested location.
+            The top builder base players for the requested location.
         """
         if not issubclass(cls, RankedPlayer):
             raise TypeError("cls must be a subclass of RankedPlayer.")
-        data = await self.http.get_location_players_versus(location_id, limit=limit, before=before, after=after)
+        data = await self.http.get_location_players_builder_base(location_id, limit=limit, before=before, after=after)
         return [cls(data=n, client=self) for n in data["items"]]
 
     # leagues
 
     async def search_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
         """Get list of leagues.
 
@@ -1614,15 +1610,106 @@
         Returns
         --------
         :class:`League`
             The first league matching the league name. Could be ``None`` if not found.
         """
         return get(await self.search_leagues(), name=league_name)
 
-    async def search_war_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
+    async def search_builder_base_leagues(self, *, limit: int = None, before: str = None, after: str = None)-> List[
+        BaseLeague]:
+        """Get list of builder base leagues.
+
+        Parameters
+        -----------
+        limit : int
+            Number of items to fetch. Defaults to ``None`` (all leagues).
+        before : str, optional
+            For use with paging. Not implemented yet.
+        after: str, optional
+            For use with paging. Not implemented yet.
+
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+
+        Returns
+        --------
+        List[:class:`BaseLeague`]
+            The requested leagues.
+        """
+        data = await self.http.search_builder_base_leagues(limit=limit, before=before, after=after)
+        return [BaseLeague(data=n, client=self) for n in data["items"]]
+
+    async def get_builder_base_league(self, league_id: int) -> BaseLeague:
+        """
+        Get builder base league information
+
+        Parameters
+        -----------
+        league_id : str
+            The League ID to search for.
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        NotFound
+            No league was found with the supplied league ID.
+
+
+        Returns
+        --------
+        :class:`BaseLeague`
+            The league with the requested ID
+        """
+        data = await self.http.get_builder_base_league(league_id)
+        return BaseLeague(data=data, client=self)
+
+    async def get_builder_base_league_named(self, league_name: str) -> Optional[BaseLeague]:
+        """Get a builder base league by name.
+
+        This is somewhat equivalent to
+
+        .. code-block:: python3
+
+            leagues = await client.search_builder_base_leagues(limit=None)
+            return utils.get(leagues, name=league_name)
+
+
+        Parameters
+        -----------
+        league_name : str
+            The builder base league name to search for
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        Returns
+        --------
+        :class:`BaseLeague`
+            The first league matching the league name. Could be ``None`` if not found.
+        """
+        return get(await self.search_builder_base_leagues(), name=league_name)
+
+    async def search_war_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[BaseLeague]:
         """Get list of war leagues.
 
         Parameters
         -----------
         limit : int
             Number of items to fetch. Defaults to ``None`` (all leagues).
         before : str, optional
@@ -1638,21 +1725,21 @@
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
-        List[:class:`League`]
+        List[:class:`BaseLeague`]
             The requested leagues.
         """
         data = await self.http.search_war_leagues(limit=limit, before=before, after=after)
-        return [League(data=n, client=self) for n in data["items"]]
+        return [BaseLeague(data=n, client=self) for n in data["items"]]
 
-    async def get_war_league(self, league_id: int) -> League:
+    async def get_war_league(self, league_id: int) -> BaseLeague:
         """
         Get war league information
 
         Parameters
         -----------
         league_id : str
             The League ID to search for.
@@ -1667,21 +1754,21 @@
 
         NotFound
             No league was found with the supplied league ID.
 
 
         Returns
         --------
-        :class:`League`
+        :class:`BaseLeague`
             The league with the requested ID
         """
         data = await self.http.get_war_league(league_id)
-        return League(data=data, client=self)
+        return BaseLeague(data=data, client=self)
 
-    async def get_war_league_named(self, league_name: str) -> Optional[League]:
+    async def get_war_league_named(self, league_name: str) -> Optional[BaseLeague]:
         """Get a war league by name.
 
         This is somewhat equivalent to
 
         .. code-block:: python3
 
             leagues = await client.search_war_leagues(limit=None)
@@ -1699,20 +1786,20 @@
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
         Returns
         --------
-        :class:`League`
+        :class:`BaseLeague`
             The first league matching the league name. Could be ``None`` if not found.
         """
         return get(await self.search_war_leagues(), name=league_name)
 
-    async def search_capital_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
+    async def search_capital_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[BaseLeague]:
         """Get list of capital leagues.
 
         Parameters
         -----------
         limit : int
             Number of items to fetch. Defaults to ``None`` (all leagues).
         before : str, optional
@@ -1728,21 +1815,21 @@
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
-        List[:class:`League`]
+        List[:class:`BaseLeague`]
             The requested leagues.
         """
         data = await self.http.search_capital_leagues(limit=limit, before=before, after=after)
-        return [League(data=n, client=self) for n in data["items"]]
+        return [BaseLeague(data=n, client=self) for n in data["items"]]
 
-    async def get_capital_league(self, league_id: int) -> League:
+    async def get_capital_league(self, league_id: int) -> BaseLeague:
         """
         Get capital league information
 
         Parameters
         -----------
         league_id : str
             The League ID to search for.
@@ -1757,21 +1844,21 @@
 
         NotFound
             No league was found with the supplied league ID.
 
 
         Returns
         --------
-        :class:`League`
+        :class:`BaseLeague`
             The league with the requested ID
         """
         data = await self.http.get_capital_league(league_id)
-        return League(data=data, client=self)
+        return BaseLeague(data=data, client=self)
 
-    async def get_capital_league_named(self, league_name: str) -> Optional[League]:
+    async def get_capital_league_named(self, league_name: str) -> Optional[BaseLeague]:
         """Get a capital league by name.
 
         This is somewhat equivalent to
 
         .. code-block:: python3
 
             leagues = await client.search_capital_leagues(limit=None)
@@ -1789,15 +1876,15 @@
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
         Returns
         --------
-        :class:`League`
+        :class:`BaseLeague`
             The first league matching the league name. Could be ``None`` if not found.
         """
         return get(await self.search_capital_leagues(), name=league_name)
 
     async def get_seasons(self, league_id: int = 29000021) -> List[str]:
         """Get league seasons.
```

### Comparing `coc.py-2.4.1/coc/entry_logs.py` & `coc.py-3.0.0/coc/entry_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         return ClanWarLog(client=client, clan_tag=clan_tag, limit=limit,
                           page=page, json_resp=json_resp, model=model)
 
     @staticmethod
     async def _fetch_endpoint(client: Client, clan_tag: str,
                               fut: Optional[asyncio.Future] = None,
                               **options) -> dict:
-        result = await client.http.get_clan_warlog(clan_tag, **options, ignore_cache=True)
+        result = await client.http.get_clan_war_log(clan_tag, **options, ignore_cache=True)
         if fut:
             fut.set_result(result)
         return result
 
 
 class RaidLog(LogPaginator, ABC):
     """Represents a Generator for a RaidLog"""
@@ -231,11 +231,11 @@
         return RaidLog(client=client, clan_tag=clan_tag, limit=limit,
                        page=page, json_resp=json_resp, model=model)
 
     @staticmethod
     async def _fetch_endpoint(client: Client, clan_tag: str,
                               fut: Optional[asyncio.Future] = None,
                               **options) -> dict:
-        result = await client.http.get_clan_raidlog(clan_tag, **options)
+        result = await client.http.get_clan_raid_log(clan_tag, **options)
         if fut:
             fut.set_result(result)
         return result
```

### Comparing `coc.py-2.4.1/coc/enums.py` & `coc.py-3.0.0/coc/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     "Valkyrie",
     "Golem",
     "Witch",
     "Lava Hound",
     "Bowler",
     "Ice Golem",
     "Headhunter",
+    "Apprentice Warden"
 ]
 
 SIEGE_MACHINE_ORDER = [
     "Wall Wrecker",
     "Battle Blimp",
     "Stone Slammer",
     "Siege Barracks",
@@ -129,31 +130,35 @@
     "Inferno Dragon",
     "Super Minion",
     "Super Valkyrie",
     "Super Witch",
     "Ice Hound",
     "Super Bowler",
     "Super Miner",
+    "Super Hog Rider"
 ]
 
+#enum with only the actual troops, not sure why they were combined to begin with
+HV_TROOP_ORDER = HOME_TROOP_ORDER
 HOME_TROOP_ORDER = HOME_TROOP_ORDER + SIEGE_MACHINE_ORDER
 
 
 BUILDER_TROOPS_ORDER = [
     "Raged Barbarian",
     "Sneaky Archer",
     "Boxer Giant",
     "Beta Minion",
     "Bomber",
     "Baby Dragon",
     "Cannon Cart",
     "Night Witch",
     "Drop Ship",
-    "Super P.E.K.K.A",
+    "Power P.E.K.K.A",
     "Hog Glider",
+    "Electrofire Wizard"
 ]
 
 SPELL_ORDER = [
     "Lightning Spell",
     "Healing Spell",
     "Rage Spell",
     "Jump Spell",
@@ -164,15 +169,17 @@
     "Poison Spell",
     "Earthquake Spell",
     "Haste Spell",
     "Skeleton Spell",
     "Bat Spell",
 ]
 
-HERO_ORDER = ["Barbarian King", "Archer Queen", "Grand Warden", "Royal Champion", "Battle Machine"]
+HOME_BASE_HERO_ORDER = ["Barbarian King", "Archer Queen", "Grand Warden", "Royal Champion"]
+BUILDER_BASE_HERO_ORDER = ["Battle Machine", "Battle Copter"]
+HERO_ORDER = HOME_BASE_HERO_ORDER + BUILDER_BASE_HERO_ORDER
 
 PETS_ORDER = [
     "L.A.S.S.I",
     "Electro Owl",
     "Mighty Yak",
     "Unicorn",
     "Frosty",
@@ -235,8 +242,8 @@
 UNRANKED_LEAGUE_DATA = {
     "id": 29000000,
     "name": "Unranked",
     "iconUrls": {
         "small": "https://api-assets.clashofclans.com/leagues/72/e--YMyIexEQQhE4imLoJcwhYn6Uy8KqlgyY3_kFV6t4.png",
         "tiny": "https://api-assets.clashofclans.com/leagues/36/e--YMyIexEQQhE4imLoJcwhYn6Uy8KqlgyY3_kFV6t4.png",
     },
-}
+}
```

### Comparing `coc.py-2.4.1/coc/errors.py` & `coc.py-3.0.0/coc/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,16 +49,22 @@
             This could be an empty string if nothing was given
 
     """
 
     __slots__ = ("response", "status", "message", "reason", "_data")
 
     def _from_response(self, response, data):
-        self.response = response
-        self.status = response.status
+        if isinstance(response, int):
+            self.status = response
+            self.response = None
+        elif isinstance(response, ClientResponse):
+            self.response = response
+            self.status = response.status
+        else:
+            self.response = self.status = None
 
         if isinstance(data, dict):
             self.reason = data.get("reason", "Unknown")
             self.message = data.get("message")
         elif isinstance(data, str):
             self.reason = data
             self.message = None
@@ -69,15 +75,15 @@
         fmt = "{0.reason} (status code: {0.status})"
         if self.message:
             fmt += ": {0.message}"
 
         super().__init__(fmt.format(self))
 
     def __init__(self, response=None, data=None):
-        if isinstance(response, ClientResponse):
+        if isinstance(response, (ClientResponse, int)):
             self._from_response(response, data)
         else:
             self.response = None
             self.status = 0
             self.reason = None
             self.message = response
```

### Comparing `coc.py-2.4.1/coc/events.py` & `coc.py-3.0.0/coc/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,15 +783,15 @@
 
     async def _raid_poller(self):
         # pylint: disable=broad-except, protected-access
         try:
             age = 0
             while self.loop.is_running():
                 try:
-                    [raid_log_entry] = await self.get_raidlog("#2PP", limit=1)
+                    [raid_log_entry] = await self.get_raid_log("#2PP", limit=1)
                     raid_log_entry: coc.raid.RaidLogEntry
                 except Maintenance:
                     await asyncio.sleep(15)
                 except Exception:
                     await asyncio.sleep(DEFAULT_SLEEP)
                 else:
                     if raid_log_entry.start_time.seconds_until + age > 0 and raid_log_entry.end_time.seconds_until > 0:
```

### Comparing `coc.py-2.4.1/coc/events.pyi` & `coc.py-3.0.0/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/ext/discordlinks/__init__.py` & `coc.py-3.0.0/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/ext/fullwarapi/__init__.py` & `coc.py-3.0.0/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/ext/triggers/cron.py` & `coc.py-3.0.0/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/ext/triggers/triggers.py` & `coc.py-3.0.0/coc/ext/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/hero.py` & `coc.py-3.0.0/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/http.py` & `coc.py-3.0.0/coc/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -260,15 +260,28 @@
             kwargs["headers"]["Content-Type"] = "application/json"
 
         cache_control_key = route.url
         cache = self.cache
         # the cache will be cleaned once it becomes stale / a new object is available from the api.
         if isinstance(cache, FIFO) and not self.client.realtime and not kwargs.get("ignore_cache", False):
             try:
-                return cache[cache_control_key]
+                data = cache[cache_control_key]
+                status_code = data.get("status_code")
+                if data.get("timestamp") and data.get("timestamp") + data.get("_response_retry", 0) < datetime.utcnow().timestamp():
+                    self._cache_remove(cache_control_key)
+                elif not status_code or 200 <= status_code < 300:
+                    return data
+                elif status_code == 400:
+                    raise InvalidArgument(400, data)
+                elif status_code == 403:
+                    raise Forbidden(403, data)
+                elif status_code == 404:
+                    raise NotFound(404, data)
+                elif status_code == 503:
+                    raise Maintenance(503, data)
             except KeyError:
                 pass
 
         for tries in range(5):
             try:
                 async with self.__lock, self.__throttle:
                     start = perf_counter()
@@ -277,15 +290,16 @@
                         perf = (perf_counter() - start) * 1000
                         log_info = {"method": method, "url": url, "perf_counter": perf, "status": response.status}
                         if isinstance(self.stats, HTTPStats):
                             self.stats[route.stats_key] = perf
 
                         LOG.debug("API HTTP Request: %s", str(log_info))
                         data = await json_or_text(response)
-
+                        data["status_code"] = response.status
+                        data["timestamp"] = datetime.utcnow().timestamp()
                         try:
                             # set a callback to remove the item from cache once it's stale.
                             delta = int(response.headers["Cache-Control"].strip("max-age=").strip("public max-age="))
                             # encounter for changed description in cache control header. for realtime it is always
                             # 600 but that is not true. Correct is 0
                             data["_response_retry"] = delta if 'realtime' not in url else 0
                             if isinstance(cache, FIFO) and 'realtime' not in url:
@@ -366,15 +380,15 @@
 
     def get_clan(self, tag):
         return self.request(Route("GET", "/clans/{}".format(tag)))
 
     def get_clan_members(self, tag, **kwargs):
         return self.request(Route("GET", "/clans/{}/members".format(tag), **kwargs))
 
-    def get_clan_warlog(self, tag, **kwargs):
+    def get_clan_war_log(self, tag, **kwargs):
         return self.request(Route("GET", "/clans/{}/warlog".format(tag), **kwargs))
 
     def get_clan_current_war(self, tag, realtime=None):
         return self.request(Route("GET", "/clans/{}/currentwar".format(tag) + (
                                          '?realtime=true' if realtime or (realtime is None and self.client.realtime)
                                          else '')))
 
@@ -384,15 +398,15 @@
                                          else '')))
 
     def get_cwl_wars(self, war_tag, realtime = None):
         return self.request(Route("GET", "/clanwarleagues/wars/{}".format(war_tag) + (
                                          '?realtime=true' if realtime or (realtime is None and self.client.realtime)
                                          else '')))
 
-    def get_clan_raidlog(self, tag, **kwargs):
+    def get_clan_raid_log(self, tag, **kwargs):
         return self.request(Route("GET", "/clans/{}/capitalraidseasons".format(tag), **kwargs))
 
     # locations
 
     def search_locations(self, **kwargs):
         return self.request(Route("GET", "/locations", **kwargs))
 
@@ -401,43 +415,49 @@
 
     def get_location_clans(self, location_id, **kwargs):
         return self.request(Route("GET", "/locations/{}/rankings/clans".format(location_id), **kwargs))
 
     def get_location_players(self, location_id, **kwargs):
         return self.request(Route("GET", "/locations/{}/rankings/players".format(location_id), **kwargs))
 
-    def get_location_clans_versus(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/clans-versus".format(location_id), **kwargs))
+    def get_location_clans_builder_base(self, location_id, **kwargs):
+        return self.request(Route("GET", "/locations/{}/rankings/clans-builder-base".format(location_id), **kwargs))
 
     def get_location_clans_capital(self, location_id, **kwargs):
         return self.request(Route("GET", "/locations/{}/rankings/capitals".format(location_id), **kwargs))
 
-    def get_location_players_versus(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/players-versus".format(location_id), **kwargs))
+    def get_location_players_builder_base(self, location_id, **kwargs):
+        return self.request(Route("GET", "/locations/{}/rankings/players-builder-base".format(location_id), **kwargs))
 
     # leagues
 
     def search_leagues(self, **kwargs):
         return self.request(Route("GET", "/leagues", **kwargs))
 
     def search_capital_leagues(self, **kwargs):
         return self.request(Route("GET", "/capitalleagues", **kwargs))
 
     def search_war_leagues(self, **kwargs):
         return self.request(Route("GET", "/warleagues", **kwargs))
 
+    def search_builder_base_leagues(self, **kwargs):
+        return self.request(Route("GET", "/builderbaseleagues", **kwargs))
+
     def get_league(self, league_id):
         return self.request(Route("GET", "/leagues/{}".format(league_id)))
 
     def get_capital_league(self, league_id):
         return self.request(Route("GET", "/capitalleagues/{}".format(league_id)))
 
     def get_war_league(self, league_id):
         return self.request(Route("GET", "/warleagues/{}".format(league_id)))
 
+    def get_builder_base_league(self, league_id):
+        return self.request(Route("GET", "/builderbaseleagues/{}".format(league_id)))
+
     def get_league_seasons(self, league_id, **kwargs):
         return self.request(Route("GET", "/leagues/{}/seasons".format(league_id), **kwargs))
 
     def get_league_season_info(self, league_id, season_id, **kwargs):
         return self.request(Route("GET", "/leagues/{}/seasons/{}".format(league_id, season_id), **kwargs))
 
     # players
```

### Comparing `coc.py-2.4.1/coc/iterators.py` & `coc.py-3.0.0/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/miscmodels.py` & `coc.py-3.0.0/coc/miscmodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from datetime import datetime
 from typing import Any, Type, TypeVar, Optional
+
+import coc
 from .enums import PlayerHouseElementType
 from .utils import from_timestamp
 
 T = TypeVar("T")
 
 
 def try_enum(_class: Type[T], data: Any, **kwargs) -> Optional[T]:
@@ -236,62 +238,78 @@
         self.id: int = data_get("id")
         self.name: str = data_get("name")
         self.is_country: bool = data_get("isCountry")
         self.country_code: str = data_get("countryCode")
         self.localised_name: str = data_get("localizedName")
 
 
-class League:
+class BaseLeague:
+    """Represents a basic league.
+
+    Attributes
+    -----------
+    id: :class:`int`: The league's unique ID
+    name: :class:`str`: The league's name, as it appears in-game."""
+
+    __slots__ = (
+        "id",
+        "name",
+        "_client"
+    )
+
+    def __init__(self, *, data, client=None):
+        # pylint: disable=invalid-name
+        self.id: int = data["id"]
+        self.name: str = data["name"]
+        self._client = client
+
+    def __repr__(self):
+        return "<%s id=%s name=%s>" % (self.__class__.__name__, self.id, self.name)
+
+    def __str__(self):
+        return self.name
+
+    def __eq__(self, other):
+        return isinstance(self, other.__class__) and other.id == self.id
+
+
+class League(BaseLeague):
     """Represents a Clash of Clans League
 
     Attributes
     -----------
     id:
         :class:`int`: The league ID.
     name:
         :class:`str`: The league name.
-    localised_name:
-        :class:`str`: A localised name of the location. The extent of the use of this is unknown at present.
-    localised_short_name:
-        :class:`str`: A localised short name of the location. The extent of the use of this is unknown at present.
     icon:
         :class:`Icon`: The league's icon.
     """
 
     __slots__ = (
-        "id",
-        "name",
-        "localised_short_name",
-        "localised_name",
         "icon",
-        "_client",
     )
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         attrs = [("id", self.id), ("name", self.name)]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.id == other.id
 
     def __init__(self, *, data, client):
-        self._client = client
+        super().__init__(data=data, client=client)
         self._from_data(data)
 
     def _from_data(self, data: dict) -> None:
         # pylint: disable=invalid-name
         data_get = data.get
-
-        self.id: int = data_get("id")
-        self.name: str = data_get("name")
-        self.localised_name: str = data_get("localizedName")
-        self.localised_short_name: str = data_get("localizedShortName")
         self.icon = try_enum(Icon, data=data_get("iconUrls"), client=self._client)
 
 
 class Season:
     """Represents a Clash of Clans Player's Season."""
 
     # pylint: disable=invalid-name
@@ -321,45 +339,46 @@
         :class:`int` - The player's legend trophies
     current_season:
         :class:`Season`: Legend statistics for this season.
     previous_season:
         :class:`Season`: Legend statistics for the previous season.
     best_season:
         :class:`Season`: Legend statistics for the player's best season.
-    previous_versus_season:
-        :class:`Season`: Legend statistics for the previous versus season.
-    best_versus_season:
-        :class:`Season`: Legend statistics for the player's best versus season.
+    previous_builder_base_season:
+        :class:`Season`: Legend statistics for the previous builder base season.
+    best_builder_base_season:
+        :class:`Season`: Legend statistics for the player's best builder base season.
     """
 
-    __slots__ = ("legend_trophies", "current_season", "previous_season", "best_season", "previous_versus_season", "best_versus_season")
+    __slots__ = ("legend_trophies", "current_season", "previous_season", "best_season", "previous_builder_base_season",
+                 "best_builder_base_season")
 
     def __repr__(self):
         attrs = [
             ("legend_trophies", self.legend_trophies),
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __eq__(self, other):
         return (
             isinstance(other, self.__class__)
             and self.best_season == other.best_season
             and self.current_season == other.current_season
-            and self.best_versus_season == other.best_versus_season
+            and self.best_builder_base_season == other.best_builder_base_season
             and self.previous_season == other.previous_season
-            and self.previous_versus_season == self.previous_versus_season
+            and self.previous_builder_base_season == self.previous_builder_base_season
         )
 
     def __init__(self, *, data):
         self.legend_trophies: int = data["legendTrophies"]
         self.current_season = try_enum(Season, data=data.get("currentSeason"))
         self.previous_season = try_enum(Season, data=data.get("previousSeason"))
         self.best_season = try_enum(Season, data=data.get("bestSeason"))
-        self.previous_versus_season = try_enum(Season, data=data.get("previousVersusSeason"))
-        self.best_versus_season = try_enum(Season, data=data.get("bestVersusSeason"))
+        self.previous_builder_base_season = try_enum(Season, data=data.get("previousBuilderBaseSeason"))
+        self.best_builder_base_season = try_enum(Season, data=data.get("bestBuilderBaseSeason"))
 
 
 class Badge:
     """Represents a Clash Of Clans Badge.
 
     Attributes
     -----------
@@ -606,41 +625,14 @@
     def __init__(self, *, data, client):
         # pylint: disable=invalid-name
         self.id: int = data.get("id")
         self.name: str = data.get("name")
         self.hall_level: int = data.get("districtHallLevel")
 
 
-class WarLeague:
-    """Represents a clan's CWL league.
-
-    Attributes
-    -----------
-    id: :class:`int`: The league's unique ID
-    name: :class:`str`: The league's name, as it appears in-game."""
-
-    __slots__ = (
-        "id",
-        "name",
-    )
-
-    def __init__(self, *, data):
-        # pylint: disable=invalid-name
-        self.id: int = data["id"]
-        self.name: str = data["name"]
-
-    def __repr__(self):
-        return "<%s id=%s name=%s>" % (self.__class__.__name__, self.id, self.name)
-
-    def __str__(self):
-        return self.name
-
-    def __eq__(self, other):
-        return isinstance(self, other.__class__) and other.id == self.id
-
 
 class ChatLanguage:
     """Represents a clan's chat language.
 
     Attributes
     ----------
     id: :class:`int`: The language's unique ID
```

### Comparing `coc.py-2.4.1/coc/player_clan.py` & `coc.py-3.0.0/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/players.py` & `coc.py-3.0.0/coc/players.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from typing import Optional, List, TYPE_CHECKING
 
 
-from .miscmodels import PlayerHouseElement, try_enum, Achievement, Label, League, LegendStatistics
+from .miscmodels import BaseLeague, PlayerHouseElement, try_enum, Achievement, Label, League, LegendStatistics
 from .enums import (
     Role,
     HERO_ORDER,
     BUILDER_TROOPS_ORDER,
     HOME_TROOP_ORDER,
     SPELL_ORDER,
     SIEGE_MACHINE_ORDER,
@@ -63,133 +63,158 @@
         The player's clan. If the player is clanless, this will be ``None``.
     role: :class:`Role`
         The member's role in a clan. To get a string as rendered in-game, do ``str(member.role)``.
     exp_level: :class:`int`
         The member's experience level.
     league: :class:`League`
         The member's current league.
+    builder_base_league: :class:`BaseLeague`
+        The member's current builder base league.
     trophies: :class:`int`
         The member's trophy count.
-    versus_trophies: :class:`int`
-        The member's versus trophy count.
+    builder_base_trophies: :class:`int`
+        The member's builder base trophy count.
     clan_rank: :class:`int`
         The member's rank in the clan.
     clan_previous_rank: :class:`int`
         The member's rank before the last leaderboard change
         (ie if Bob overtakes Jim in trophies, and they switch ranks on the leaderboard,
         and you want to find out their previous rankings, this will help.).
-    versus_rank: :class:`int`
-        The member's rank in the clan based on versus trophies.
+    builder_base_rank: :class:`int`
+        The member's rank in the clan based on builder base trophies.
     donations: :class:`int`
         The member's donation count for this season.
     received: :class:`int`
         The member's donations received count for this season.
     clan_cls: :class:`coc.Clan`
         The class to use to create the :attr:`ClanMember.clan` attribute.
         Ensure any overriding of this inherits from :class:`coc.Clan` or :class:`coc.PlayerClan`.
     league_cls: :class:`coc.League`
-        The class to use to create the :attr:`Clanmember.league` attribute.
+        The class to use to create the :attr:`ClanMember.league` attribute.
         Ensure any overriding of this inherits from :class:`coc.League`.
+    builder_base_league_cls: :class:`coc.League`
+        The class to use to create the :attr:`ClanMember.builder_base_league` attribute.
+        Ensure any overriding of this inherits from :class:`coc.BaseLeague`.
     """
 
     __slots__ = (
         "_client",
         "clan",
         "role",
         "exp_level",
         "league",
+        "builder_base_league",
         "trophies",
-        "versus_trophies",
+        "builder_base_trophies",
         "clan_rank",
         "clan_previous_rank",
-        "versus_rank",
+        "builder_base_rank",
         "donations",
         "received",
         "clan_cls",
         "league_cls",
+        "builder_base_league_cls",
+        "_player_house_elements",
+        "player_house_element_cls",
+        "_iter_player_house_elements",
+        "_cs_player_house_elements",
     )
 
     def __init__(self, *, data, client, clan=None, **_):
         super().__init__(data=data, client=client)
         self._client = client
         self.clan_cls = PlayerClan
         self.league_cls = League
+        self.builder_base_league_cls = BaseLeague
+        self.player_house_element_cls = PlayerHouseElement
+
         self._from_data(data)
         if clan:
             self.clan = clan
 
     def _from_data(self, data: dict) -> None:
         data_get = data.get
 
         self.exp_level: int = data_get("expLevel")
         self.trophies: int = data_get("trophies")
-        self.versus_trophies: int = data_get("versusTrophies")
+        self.builder_base_trophies: int = data_get("builderBaseTrophies")
         self.clan_rank: int = data_get("clanRank")
         self.clan_previous_rank: int = data_get("previousClanRank")
-        self.versus_rank: int = data.get("versusRank")
+        self.builder_base_rank: int = data.get("builderBaseRank")
         self.donations: int = data_get("donations")
         self.received: int = data_get("donationsReceived")
-
+        player_house_element_cls = self.player_house_element_cls
         self.clan = try_enum(self.clan_cls, data=data_get("clan"), client=self._client)
         self.league = try_enum(self.league_cls, data=data_get("league") or UNRANKED_LEAGUE_DATA, client=self._client)
+        self.builder_base_league = try_enum(self.builder_base_league_cls,
+                                            data=data_get("builderBaseLeague") or UNRANKED_LEAGUE_DATA,
+                                            client=self._client)
         self.role = data_get("role") and Role(value=data["role"])
+        self._iter_player_house_elements = (player_house_element_cls(data=adata)
+                                            for adata in data_get("playerHouse", {}).get("elements", []))
 
     async def get_detailed_clan(self) -> Optional["Clan"]:
         """Get clan details for the player's clan. If the player's clan is ``None``,this will return ``None``.
 
         Example
         ---------
 
         .. code-block:: python3
 
             player = await client.get_player('tag')
             clan = await player.get_detailed_clan()
         """
         return self.clan and await self._client.get_clan(self.clan.tag)
 
+    @cached_property("_cs_player_house_elements")
+    def player_house_elements(self) -> List[PlayerHouseElement]:
+        """List[:class:`PlayerHouseElement`]: A :class:`List` of :class:`PlayerHouseElement`s that the player has."""
+        return list(self._iter_player_house_elements)
+
 
 class RankedPlayer(ClanMember):
     """Represents a leaderboard-ranked player.
 
     Attributes
     ----------
     attack_wins: :class:`int`
-        The player's number of attack wins. If retrieving info for versus leader-boards, this will be ``None``.
+        The player's number of attack wins. If retrieving info for builder base leader-boards, this will be ``None``.
     defense_wins: :class:`int`
-        The player's number of defense wins. If retrieving info for versus leader-boards, this will be ``None``.
-    versus_trophies: :class:`int`
-        The player's versus trophy count. If retrieving info for regular leader-boards, this will be ``None``.
+        The player's number of defense wins. If retrieving info for builder base leader-boards, this will be ``None``.
+    builder_base_trophies: :class:`int`
+        The player's builder base trophy count. If retrieving info for regular leader-boards, this will be ``None``.
     rank: :class:`int`
         The player's rank in the clan leaderboard.
     previous_rank: :class:`int`
         The member's rank before the last clan leaderboard change
         (ie if Bob overtakes Jim in trophies, and they switch ranks on the leaderboard,
         and you want to find out their previous rankings, this will help.).
     """
 
-    __slots__ = ("attack_wins", "defense_wins", "versus_trophies", "rank", "previous_rank")
+    __slots__ = ("attack_wins", "defense_wins", "builder_base_trophies", "rank", "previous_rank")
 
     def _from_data(self, data: dict) -> None:
         super()._from_data(data)
 
         data_get = data.get
         self.attack_wins: int = data_get("attackWins")
         self.defense_wins: int = data_get("defenseWins")
-        self.versus_trophies: int = data_get("versusTrophies")
+        self.builder_base_trophies: int = data_get("builderBaseTrophies")
         self.rank: int = data_get("rank")
         self.previous_rank: int = data_get("previousRank")
 
 
 class Player(ClanMember):
     """Represents a Clash of Clans Player.
 
     Attributes
     ----------
     achievement_cls: :class:`Achievement`
-        The constructor used to create the :attr:`Player.achievements` list. This must inherit from :class:`Achievement`.
+        The constructor used to create the :attr:`Player.achievements` list.
+        This must inherit from :class:`Achievement`.
     hero_cls: :class:`Hero`
         The constructor used to create the :attr:`Player.heroes` list. This must inherit from :class:`Hero`.
     label_cls: :class:`Label`
         The constructor used to create the :attr:`Player.labels` list. This must inherit from :class:`Label`.
     spell_cls: :class:`Spell`
         The constructor used to create the :attr:`Player.spells` list. This must inherit from :class:`Spell`.
     troop_cls: :class:`Troop`
@@ -204,18 +229,16 @@
         The player's total war stars.
     town_hall: :class:`int`
         The player's town hall level.
     town_hall_weapon: Optional[:class:`int`]
         The player's town hall weapon level, or ``None`` if it doesn't exist.
     builder_hall: :class:`int`
         The player's builder hall level, or 0 if it hasn't been unlocked.
-    best_versus_trophies: :class:`int`
-        The player's best versus trophy count.
-    versus_attack_wins: :class:`int`
-        The number of versus attacks the player has won
+    best_builder_base_trophies: :class:`int`
+        The player's best builder base trophy count.
     clan_capital_contributions: :class:`int`
         The player's total contribution to clan capitals
     legend_statistics: Optional[:class:`LegendStatistics`]
         The player's legend statistics, or ``None`` if they have never been in the legend league.
     war_opted_in: Optional[:class:`bool`]
         Whether the player has selected that they are opted "in" (True) for wars, or opted "out" (False).
         This will be ``None`` if the player is not in a clan.
@@ -226,47 +249,42 @@
         "attack_wins",
         "defense_wins",
         "best_trophies",
         "war_stars",
         "town_hall",
         "town_hall_weapon",
         "builder_hall",
-        "best_versus_trophies",
-        "versus_attack_wins",
+        "best_builder_base_trophies",
         "clan_capital_contributions",
         "legend_statistics",
         "war_opted_in",
         "_achievements",
-        "_player_house_elements",
         "_heroes",
         "_pets",
         "_labels",
         "_spells",
         "_home_troops",
         "_builder_troops",
         "_super_troops",
         "achievement_cls",
-        "player_house_element_cls",
         "hero_cls",
         "label_cls",
         "spell_cls",
         "troop_cls",
         "pet_cls",
 
         "_iter_achievements",
-        "_iter_player_house_elements",
         "_iter_heroes",
         "_iter_labels",
         "_iter_spells",
         "_iter_troops",
         "_iter_pets",
 
         "_cs_labels",
         "_cs_achievements",
-        "_cs_player_house_elements",
         "_cs_troops",
         "_cs_home_troops",
         "_cs_builder_troops",
         "_cs_siege_machines",
         "_cs_pets",
         "_cs_super_troops",
         "_cs_heroes",
@@ -285,15 +303,14 @@
         self._spells = None  # type: Optional[dict]
         self._home_troops: dict = {}
         self._builder_troops: dict = {}
         self._super_troops: list = []
         self._pets = None # type: Optional[dict]
 
         self.achievement_cls = Achievement
-        self.player_house_element_cls = PlayerHouseElement
         self.hero_cls = Hero
         self.label_cls = Label
         self.spell_cls = Spell
         self.troop_cls = Troop
         self.pet_cls = Pet
 
         if self._client and self._client._troop_holder.loaded:
@@ -317,42 +334,38 @@
         self.attack_wins: int = data_get("attackWins")
         self.defense_wins: int = data_get("defenseWins")
         self.best_trophies: int = data_get("bestTrophies")
         self.war_stars: int = data_get("warStars")
         self.town_hall: int = data_get("townHallLevel")
         self.town_hall_weapon: int = data_get("townHallWeaponLevel")
         self.builder_hall: int = data_get("builderHallLevel", 0)
-        self.best_versus_trophies: int = data_get("bestVersusTrophies")
-        self.versus_attack_wins: int = data_get("versusBattleWins")
+        self.best_builder_base_trophies: int = data_get("bestBuilderBaseTrophies")
         self.clan_capital_contributions: int = data_get("clanCapitalContributions")
         self.legend_statistics = try_enum(LegendStatistics, data=data_get("legendStatistics"))
 
         try:
             self.war_opted_in: Optional[bool] = True if data["warPreference"] == "in" else False
         except KeyError:
             # not in a clan / war preference not there
             self.war_opted_in: Optional[bool] = None
 
         label_cls = self.label_cls
         achievement_cls = self.achievement_cls
-        player_house_element_cls = self.player_house_element_cls
         troop_loader = self._client._troop_holder.load if self._client else None
         hero_loader =  self._client._hero_holder.load if self._client else None
         spell_loader = self._client._spell_holder.load if self._client else None
         pet_loader = self._client._pet_holder.load if self._client else None
 
         if self._game_files_loaded:
             pet_lookup = [p.name for p in self._client._pet_holder.items]
         else:
             pet_lookup = PETS_ORDER
 
         self._iter_labels = (label_cls(data=ldata, client=self._client) for ldata in data_get("labels", []))
         self._iter_achievements = (achievement_cls(data=adata) for adata in data_get("achievements", []))
-        self._iter_player_house_elements = (player_house_element_cls(data=adata)
-                                            for adata in data_get("playerHouse", {}).get("elements", []))
         self._iter_troops = (
             troop_loader(
                 data=tdata,
                 townhall=self.town_hall,
                 default=self.troop_cls,
                 load_game_data=self._load_game_data,
             ) for tdata in data_get("troops", []) if tdata["name"] not in pet_lookup
@@ -425,19 +438,14 @@
                         item._load_from_parent(holder.get(item.name))
 
     @cached_property("_cs_labels")
     def labels(self) -> List[Label]:
         """List[:class:`Label`]: A :class:`List` of :class:`Label`s that the player has."""
         return list(self._iter_labels)
 
-    @cached_property("_cs_player_house_elements")
-    def player_house_elements(self) -> List[PlayerHouseElement]:
-        """List[:class:`PlayerHouseElement`]: A :class:`List` of :class:`PlayerHouseElement`s that the player has."""
-        return list(self._iter_player_house_elements)
-
     @cached_property("_cs_achievements")
     def achievements(self) -> List[Achievement]:
         """List[:class:`Achievement`]: A list of the player's achievements."""
         # at the time of writing, the API presents achievements in the order
         # added to the game which doesn't match in-game order.
         achievement_dict = {a.name: a for a in self._iter_achievements}
         sorted_achievements = {}
@@ -566,15 +574,17 @@
 
         This will return hero pets in the order found in the Pet House in-game.
 
         This includes:
         - Hero pets only.
         """
         order = {k: v for v, k in enumerate(PETS_ORDER)}
-        return list(sorted(self._iter_pets, key=lambda t: order.get(t.name, 0)))
+        pets = list(sorted(self._iter_pets, key=lambda t: order.get(t.name, 0)))
+        self._pets = {p.name: p for p in pets}
+        return pets
 
     def get_pet(self, name: str, default_value=None) -> Optional[Pet]:
         """Gets the pet with the given name.
 
         Parameters
         -----------
         name: :class:`str`
@@ -585,15 +595,15 @@
         Returns
         --------
         Optional[:class:`Pet`]
             The returned pet or the ``default_value`` if not found, which defaults to ``None``.
 
         """
         if not self._pets:
-            _ = self._pets
+            _ = self.pets
 
         try:
             return self._pets[name]
         except KeyError:
             return default_value
 
     @cached_property("_cs_super_troops")
```

### Comparing `coc.py-2.4.1/coc/raid.py` & `coc.py-3.0.0/coc/raid.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,15 @@
         return (isinstance(other, RaidDistrict)
                 and self.id == other.id
                 and self.raid_clan == other.raid_clan)
 
     __slots__ = ("id",
                  "name",
                  "hall_level",
+                 "stars",
                  "destruction",
                  "attack_count",
                  "looted",
                  "attacks",
                  "raid_log_entry",
                  "raid_clan",
                  "_client",
@@ -221,35 +222,39 @@
         return self.name
 
     def __repr__(self):
         attrs = [("id", self.id),
                  ("raid_log_entry", repr(self.raid_log_entry)),
                  ("raid_clan", repr(self.raid_clan)),
                  ("hall_level", self.hall_level),
+                 ("stars", self.stars),
                  ("destruction", self.destruction)]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __init__(self, *, data, client, raid_log_entry, raid_clan):
         self.id: int = data.get("id")
         self.name: str = data.get("name")
         self.hall_level: int = data.get("districtHallLevel")
+        self.stars: int = data.get("stars")
         self.destruction: float = data.get("destructionPercent")
         self.attack_count: int = data.get("attackCount")
         self.looted: int = data.get("totalLooted")
         self.raid_log_entry = raid_log_entry  # type: RaidLogEntry
         self.raid_clan = raid_clan  # type: RaidClan
         self._raw_data = data if client and client.raw_attribute else None
         self._client = client
         if data.get("attacks", None):
             self.attacks: List[RaidAttack] = [RaidAttack(data=adata, client=client,
                                                          raid_log_entry=self.raid_log_entry,
                                                          raid_clan=self.raid_clan, district=self)
                                               for adata in data.get("attacks")]
         else:
             self.attacks = []
+        if self.destruction != 0 and self.stars == 0:  # attempt to fix an api bug responding with the wrong star count
+            self.stars = max(*[a.stars for a in self.attacks if a], self.stars)
 
 
 class RaidClan:
     """Represents the clan object returned by clan raid seasons.
 
         Attributes
         ----------
@@ -283,14 +288,15 @@
         "district_count",
         "destroyed_district_count",
         "raid_log_entry",
         "_districts",
         "_attacks",
         "_client",
         "_response_retry",
+        "_cs_raid_attacks",
         "_cs_raid_districts",
         "_cs_looted",
         "_iter_raid_districts",
         "_raw_data"
     )
 
     def __init__(self, *, data, client, raid_log_entry, index=0, **_):
```

### Comparing `coc.py-2.4.1/coc/spell.py` & `coc.py-3.0.0/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/troop.py` & `coc.py-3.0.0/coc/troop.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,50 +162,51 @@
         raise ValueError("The townhall level was not valid.")
 
 
 class TroopHolder(DataContainerHolder):
     items: List[Type[Troop]] = []
     item_lookup: Dict[Tuple[str, bool], Type[Troop]]
 
-    def _load_json(self, object_ids, english_aliases, lab_to_townhall):
+    def _load_json(self, english_aliases, lab_to_townhall):
         with open(TROOPS_FILE_PATH) as fp:
             troop_data = ujson.load(fp)
         with open(SUPER_TROOPS_FILE_PATH) as fp:
             super_troop_data = ujson.load(fp)
 
         super_data = {meta["Replacement"][0]: meta for _, meta in super_troop_data.items()}
 
+        id = 1000
         for supercell_name, troop_meta in troop_data.items():
+
             if not troop_meta.get("TID"):
                 continue
             if "Tutorial" in supercell_name:
                 continue
-            if "DisableProduction" in troop_meta:
+            if True in troop_meta.get("DisableProduction", [False]):
                 continue
-
             new_troop: Type[Troop] = type('Troop', Troop.__bases__, dict(Troop.__dict__))
             new_troop._load_json_meta(
                 troop_meta,
-                id=object_ids[supercell_name],
-                name=english_aliases[troop_meta["TID"][0]][0],
+                id=id,
+                name=english_aliases[troop_meta["TID"][0]]["EN"][0],
                 lab_to_townhall=lab_to_townhall,
             )
+            id += 1
             self.items.append(new_troop)
             self.item_lookup[(new_troop.name, new_troop._is_home_village)] = new_troop
-
             try:
                 super_meta = super_data[supercell_name]
             except KeyError:
                 pass
             else:
                 new_troop._inject_super_meta(super_meta)
 
         for troop in filter(lambda t: t.is_super_troop, self.items):
             sc_name = troop_data[troop._original]["TID"][0]
-            troop.original_troop = self.get(english_aliases[sc_name][0])
+            troop.original_troop = self.get(english_aliases[sc_name]["EN"][0])
 
         self.loaded = True
 
     def load(self, data, townhall: int, default: "Troop" = Troop, load_game_data: bool = None) -> Troop:
         if load_game_data is True:
             try:
                 troop = self.item_lookup[(data["name"], data["village"] == "home")]
```

### Comparing `coc.py-2.4.1/coc/utils.py` & `coc.py-3.0.0/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/war_attack.py` & `coc.py-3.0.0/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/war_clans.py` & `coc.py-3.0.0/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/war_members.py` & `coc.py-3.0.0/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc/wars.py` & `coc.py-3.0.0/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.1/coc.py.egg-info/PKG-INFO` & `coc.py-3.0.0/coc.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.4.1
+Version: 3.0.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-2.4.1/coc.py.egg-info/SOURCES.txt` & `coc.py-3.0.0/coc.py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 coc/enums.py
 coc/errors.py
 coc/events.py
 coc/events.pyi
 coc/hero.py
 coc/http.py
 coc/iterators.py
-coc/login.py
 coc/miscmodels.py
 coc/player_clan.py
 coc/players.py
 coc/raid.py
 coc/spell.py
 coc/troop.py
 coc/utils.py
@@ -38,14 +37,13 @@
 coc/ext/fullwarapi/__init__.py
 coc/ext/triggers/__init__.py
 coc/ext/triggers/cron.py
 coc/ext/triggers/triggers.py
 coc/static/buildings.json
 coc/static/characters.json
 coc/static/heroes.json
-coc/static/object_ids.json
 coc/static/pets.json
 coc/static/spells.json
 coc/static/supers.json
 coc/static/texts_EN.json
 coc/static/townhall_levels.json
 coc/static/update_static.py
```

### Comparing `coc.py-2.4.1/pyproject.toml` & `coc.py-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
-maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" }, { name = "lukasthaler" }, { name = "doluk" }]
-version = "2.4.1"
+maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" },
+    { name = "lukasthaler"}, { name = "doluk"}]
+version = "3.0.0"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

