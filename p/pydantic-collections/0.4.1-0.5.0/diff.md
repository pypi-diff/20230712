# Comparing `tmp/pydantic-collections-0.4.1.tar.gz` & `tmp/pydantic-collections-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydantic-collections-0.4.1.tar", last modified: Tue Jul 11 05:04:41 2023, max compression
+gzip compressed data, was "dist/pydantic-collections-0.5.0.tar", last modified: Wed Jul 12 08:23:44 2023, max compression
```

## Comparing `pydantic-collections-0.4.1.tar` & `pydantic-collections-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 pydantic-collections-0.4.1/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 pydantic-collections-0.4.1/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     3577 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     3184 2023-07-11 04:54:51.000000 pydantic-collections-0.4.1/README.md
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections/
--rw-rw-r--   0 roman     (1000) roman     (1000)      192 2023-07-11 04:53:14.000000 pydantic-collections-0.4.1/pydantic_collections/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     7006 2022-10-16 09:08:32.000000 pydantic-collections-0.4.1/pydantic_collections/_base_collection_model.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     3577 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      356 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       21 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       21 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/pydantic_collections.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      158 2021-10-22 13:36:03.000000 pydantic-collections-0.4.1/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-07-11 05:04:41.000000 pydantic-collections-0.4.1/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1178 2023-07-11 04:54:51.000000 pydantic-collections-0.4.1/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 pydantic-collections-0.5.0/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 pydantic-collections-0.5.0/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     4010 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3617 2023-07-12 08:21:52.000000 pydantic-collections-0.5.0/README.md
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      447 2023-07-12 06:18:04.000000 pydantic-collections-0.5.0/pydantic_collections/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     7006 2023-07-11 12:21:14.000000 pydantic-collections-0.5.0/pydantic_collections/_v1.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5286 2023-07-12 05:56:30.000000 pydantic-collections-0.5.0/pydantic_collections/_v2.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     4010 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      365 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       46 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       21 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/pydantic_collections.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      158 2021-10-22 13:36:03.000000 pydantic-collections-0.5.0/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-07-12 08:23:44.000000 pydantic-collections-0.5.0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1125 2023-07-12 05:52:01.000000 pydantic-collections-0.5.0/setup.py
```

### Comparing `pydantic-collections-0.4.1/LICENSE.txt` & `pydantic-collections-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydantic-collections-0.4.1/PKG-INFO` & `pydantic-collections-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: pydantic-collections
-Version: 0.4.1
-Summary: Collections of pydantic models
-Home-page: https://github.com/romis2012/pydantic-collections
-Author: Roman Snegirev
-Author-email: snegiryev@gmail.com
-License: Apache 2
-Keywords: python pydantic validation parsing serialization models
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # pydantic-collections
 
 [![Build Status](https://app.travis-ci.com/romis2012/pydantic-collections.svg?branch=master)](https://app.travis-ci.com/romis2012/pydantic-collections)
 [![Coverage Status](https://coveralls.io/repos/github/romis2012/pydantic-collections/badge.svg?branch=master&_=x)](https://coveralls.io/github/romis2012/pydantic-collections?branch=master)
 [![PyPI version](https://badge.fury.io/py/pydantic-collections.svg)](https://badge.fury.io/py/pydantic-collections)
 
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
 - Python>=3.7
-- pydantic>=1.8.2,<2.0
+- pydantic>=1.8.2,<3.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
@@ -56,19 +43,24 @@
 
  user_data = [
         {'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'},
         {'id': 2, 'name': 'Balaganov', 'birth_date': '2020-04-01T12:59:59'},
     ]
 
 users = UserCollection(user_data)
+
 print(users)
 #> UserCollection([User(id=1, name='Bender', birth_date=datetime.datetime(2010, 4, 1, 12, 59, 59)), User(id=2, name='Balaganov', birth_date=datetime.datetime(2020, 4, 1, 12, 59, 59))])
-print(users.dict())
+
+print(users.dict())  # pydantic v1.x
+print(users.model_dump())  # pydantic v2.x
 #> [{'id': 1, 'name': 'Bender', 'birth_date': datetime.datetime(2010, 4, 1, 12, 59, 59)}, {'id': 2, 'name': 'Balaganov', 'birth_date': datetime.datetime(2020, 4, 1, 12, 59, 59)}]
-print(users.json())
+
+print(users.json()) # pydantic v1.x
+print(users.model_dump_json()) # pydantic v2.x
 #> [{"id": 1, "name": "Bender", "birth_date": "2010-04-01T12:59:59"}, {"id": 2, "name": "Balaganov", "birth_date": "2020-04-01T12:59:59"}]
 ```
 
 #### Strict assignment validation
 
 By default `BaseCollectionModel` has a strict assignment check
 ```python
@@ -78,20 +70,33 @@
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})
 #> pydantic.error_wrappers.ValidationError: 1 validation error for UserCollection
 #> __root__ -> 2
 #>  instance of User expected (type=type_error.arbitrary_type; expected_arbitrary_type=User)
 ```
 
 This behavior can be changed via Model Config
+
+Pydantic v1.x
 ```python
+from pydantic_collections import BaseCollectionModel
 ...
 class UserCollection(BaseCollectionModel[User]):
     class Config:
         validate_assignment_strict = False
-        
+```
+
+Pydantic v2.x
+```python
+from pydantic_collections import BaseCollectionModel, CollectionModelConfig
+...
+class UserCollection(BaseCollectionModel[User]):
+    model_config = CollectionModelConfig(validate_assignment_strict=False)
+```
+
+```python
 users = UserCollection()
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})  # OK
 assert users[0].__class__ is User
 assert users[0].id == 1
 ```
 
 #### Using as a model field
@@ -109,9 +114,7 @@
     ]
 }
 
 container = UserContainer(**data)
 container.users.append(User(...))
 ...
 ```
-
-
```

### Comparing `pydantic-collections-0.4.1/README.md` & `pydantic-collections-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: pydantic-collections
+Version: 0.5.0
+Summary: Collections of pydantic models
+Home-page: https://github.com/romis2012/pydantic-collections
+Author: Roman Snegirev
+Author-email: snegiryev@gmail.com
+License: Apache 2
+Keywords: python pydantic validation parsing serialization models
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # pydantic-collections
 
 [![Build Status](https://app.travis-ci.com/romis2012/pydantic-collections.svg?branch=master)](https://app.travis-ci.com/romis2012/pydantic-collections)
 [![Coverage Status](https://coveralls.io/repos/github/romis2012/pydantic-collections/badge.svg?branch=master&_=x)](https://coveralls.io/github/romis2012/pydantic-collections?branch=master)
 [![PyPI version](https://badge.fury.io/py/pydantic-collections.svg)](https://badge.fury.io/py/pydantic-collections)
 
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
 - Python>=3.7
-- pydantic>=1.8.2,<2.0
+- pydantic>=1.8.2,<3.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
@@ -43,19 +56,24 @@
 
  user_data = [
         {'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'},
         {'id': 2, 'name': 'Balaganov', 'birth_date': '2020-04-01T12:59:59'},
     ]
 
 users = UserCollection(user_data)
+
 print(users)
 #> UserCollection([User(id=1, name='Bender', birth_date=datetime.datetime(2010, 4, 1, 12, 59, 59)), User(id=2, name='Balaganov', birth_date=datetime.datetime(2020, 4, 1, 12, 59, 59))])
-print(users.dict())
+
+print(users.dict())  # pydantic v1.x
+print(users.model_dump())  # pydantic v2.x
 #> [{'id': 1, 'name': 'Bender', 'birth_date': datetime.datetime(2010, 4, 1, 12, 59, 59)}, {'id': 2, 'name': 'Balaganov', 'birth_date': datetime.datetime(2020, 4, 1, 12, 59, 59)}]
-print(users.json())
+
+print(users.json()) # pydantic v1.x
+print(users.model_dump_json()) # pydantic v2.x
 #> [{"id": 1, "name": "Bender", "birth_date": "2010-04-01T12:59:59"}, {"id": 2, "name": "Balaganov", "birth_date": "2020-04-01T12:59:59"}]
 ```
 
 #### Strict assignment validation
 
 By default `BaseCollectionModel` has a strict assignment check
 ```python
@@ -65,20 +83,33 @@
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})
 #> pydantic.error_wrappers.ValidationError: 1 validation error for UserCollection
 #> __root__ -> 2
 #>  instance of User expected (type=type_error.arbitrary_type; expected_arbitrary_type=User)
 ```
 
 This behavior can be changed via Model Config
+
+Pydantic v1.x
 ```python
+from pydantic_collections import BaseCollectionModel
 ...
 class UserCollection(BaseCollectionModel[User]):
     class Config:
         validate_assignment_strict = False
-        
+```
+
+Pydantic v2.x
+```python
+from pydantic_collections import BaseCollectionModel, CollectionModelConfig
+...
+class UserCollection(BaseCollectionModel[User]):
+    model_config = CollectionModelConfig(validate_assignment_strict=False)
+```
+
+```python
 users = UserCollection()
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})  # OK
 assert users[0].__class__ is User
 assert users[0].id == 1
 ```
 
 #### Using as a model field
@@ -96,7 +127,9 @@
     ]
 }
 
 container = UserContainer(**data)
 container.users.append(User(...))
 ...
 ```
+
+
```

### Comparing `pydantic-collections-0.4.1/pydantic_collections/_base_collection_model.py` & `pydantic-collections-0.5.0/pydantic_collections/_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-collections-0.4.1/pydantic_collections.egg-info/PKG-INFO` & `pydantic-collections-0.5.0/pydantic_collections.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-collections
-Version: 0.4.1
+Version: 0.5.0
 Summary: Collections of pydantic models
 Home-page: https://github.com/romis2012/pydantic-collections
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: python pydantic validation parsing serialization models
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 The `pydantic-collections` package provides `BaseCollectionModel` class that allows you 
 to manipulate collections of [pydantic](https://github.com/samuelcolvin/pydantic) models 
 (and any other types supported by pydantic).
 
 
 ## Requirements
 - Python>=3.7
-- pydantic>=1.8.2,<2.0
+- pydantic>=1.8.2,<3.0
 
 
 ## Installation
 
 ```
 pip install pydantic-collections
 ```
@@ -56,19 +56,24 @@
 
  user_data = [
         {'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'},
         {'id': 2, 'name': 'Balaganov', 'birth_date': '2020-04-01T12:59:59'},
     ]
 
 users = UserCollection(user_data)
+
 print(users)
 #> UserCollection([User(id=1, name='Bender', birth_date=datetime.datetime(2010, 4, 1, 12, 59, 59)), User(id=2, name='Balaganov', birth_date=datetime.datetime(2020, 4, 1, 12, 59, 59))])
-print(users.dict())
+
+print(users.dict())  # pydantic v1.x
+print(users.model_dump())  # pydantic v2.x
 #> [{'id': 1, 'name': 'Bender', 'birth_date': datetime.datetime(2010, 4, 1, 12, 59, 59)}, {'id': 2, 'name': 'Balaganov', 'birth_date': datetime.datetime(2020, 4, 1, 12, 59, 59)}]
-print(users.json())
+
+print(users.json()) # pydantic v1.x
+print(users.model_dump_json()) # pydantic v2.x
 #> [{"id": 1, "name": "Bender", "birth_date": "2010-04-01T12:59:59"}, {"id": 2, "name": "Balaganov", "birth_date": "2020-04-01T12:59:59"}]
 ```
 
 #### Strict assignment validation
 
 By default `BaseCollectionModel` has a strict assignment check
 ```python
@@ -78,20 +83,33 @@
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})
 #> pydantic.error_wrappers.ValidationError: 1 validation error for UserCollection
 #> __root__ -> 2
 #>  instance of User expected (type=type_error.arbitrary_type; expected_arbitrary_type=User)
 ```
 
 This behavior can be changed via Model Config
+
+Pydantic v1.x
 ```python
+from pydantic_collections import BaseCollectionModel
 ...
 class UserCollection(BaseCollectionModel[User]):
     class Config:
         validate_assignment_strict = False
-        
+```
+
+Pydantic v2.x
+```python
+from pydantic_collections import BaseCollectionModel, CollectionModelConfig
+...
+class UserCollection(BaseCollectionModel[User]):
+    model_config = CollectionModelConfig(validate_assignment_strict=False)
+```
+
+```python
 users = UserCollection()
 users.append({'id': 1, 'name': 'Bender', 'birth_date': '2010-04-01T12:59:59'})  # OK
 assert users[0].__class__ is User
 assert users[0].id == 1
 ```
 
 #### Using as a model field
```

### Comparing `pydantic-collections-0.4.1/setup.py` & `pydantic-collections-0.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-import codecs
 import os
 import re
 import sys
 
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-version = None
-
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),
-                              'pydantic_collections', '__init__.py'), 'r', 'latin1') as fp:
-    try:
-        version = re.findall(r"^__version__ = '([^']+)'\r?$", fp.read(), re.M)[0]
-    except IndexError:
-        raise RuntimeError('Unable to determine version.')
+from setuptools import setup
 
 if sys.version_info < (3, 7, 1):
     raise RuntimeError('pydantic-collections requires Python 3.6.1+')
 
-with open('README.md') as f:
-    long_description = f.read()
+
+def get_version():
+    here = os.path.dirname(os.path.abspath(__file__))
+    filename = os.path.join(here, 'pydantic_collections', '__init__.py')
+    contents = open(filename).read()
+    pattern = r"^__version__ = '(.*?)'$"
+    return re.search(pattern, contents, re.MULTILINE).group(1)
+
+
+def get_long_description():
+    with open('README.md', mode='r', encoding='utf8') as f:
+        return f.read()
+
 
 setup(
     name='pydantic-collections',
     author='Roman Snegirev',
     author_email='snegiryev@gmail.com',
-    version=version,
+    version=get_version(),
     license='Apache 2',
     url='https://github.com/romis2012/pydantic-collections',
     description='Collections of pydantic models',
-    long_description=long_description,
+    long_description=get_long_description(),
     long_description_content_type='text/markdown',
     packages=['pydantic_collections'],
     keywords='python pydantic validation parsing serialization models',
-    install_requires=['pydantic>=1.8.2,<2.0']
+    install_requires=['pydantic>=1.8.2,<3.0', 'typing_extensions>=4.7.1'],
 )
```

