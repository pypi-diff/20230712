# Comparing `tmp/flask_validators-0.7.tar.gz` & `tmp/flask_validators-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_validators-0.7.tar", last modified: Wed Jul 12 10:44:45 2023, max compression
+gzip compressed data, was "flask_validators-1.0.tar", last modified: Wed Jul 12 10:45:41 2023, max compression
```

## Comparing `flask_validators-0.7.tar` & `flask_validators-1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11504 2023-07-12 10:44:45.081282 flask_validators-0.7/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11124 2023-07-12 10:41:20.000000 flask_validators-0.7/README.md
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.077949 flask_validators-0.7/flask_validators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      299 2023-07-12 09:39:41.000000 flask_validators-0.7/flask_validators/__init__.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/flask_validators/controllers/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      121 2023-07-12 07:54:56.000000 flask_validators-0.7/flask_validators/controllers/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      217 2023-07-12 07:55:02.000000 flask_validators-0.7/flask_validators/controllers/error_handler.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-0.7/flask_validators/controllers/validator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/flask_validators/decorators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      119 2023-07-12 09:37:40.000000 flask_validators-0.7/flask_validators/decorators/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     7244 2023-07-12 10:29:44.000000 flask_validators-0.7/flask_validators/decorators/validation_decorator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/flask_validators/models/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      375 2023-07-12 10:31:46.000000 flask_validators-0.7/flask_validators/models/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5731 2023-07-10 09:41:11.000000 flask_validators-0.7/flask_validators/models/fields.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5423 2023-07-10 09:41:57.000000 flask_validators-0.7/flask_validators/models/schema.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     2530 2023-07-12 09:22:12.000000 flask_validators-0.7/flask_validators/models/validate_db.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      462 2023-07-12 10:30:46.000000 flask_validators-0.7/flask_validators/models/validate_llm.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/flask_validators.egg-info/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11504 2023-07-12 10:44:45.000000 flask_validators-0.7/flask_validators.egg-info/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      736 2023-07-12 10:44:45.000000 flask_validators-0.7/flask_validators.egg-info/SOURCES.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-12 10:44:45.000000 flask_validators-0.7/flask_validators.egg-info/dependency_links.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       24 2023-07-12 10:44:45.000000 flask_validators-0.7/flask_validators.egg-info/requires.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-12 10:44:45.000000 flask_validators-0.7/flask_validators.egg-info/top_level.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-12 10:44:45.081282 flask_validators-0.7/setup.cfg
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      723 2023-07-12 10:44:43.000000 flask_validators-0.7/setup.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:44:45.081282 flask_validators-0.7/tests/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-0.7/tests/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     2742 2023-07-12 10:30:32.000000 flask_validators-0.7/tests/test_flask.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-0.7/tests/test_schemas.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-0.7/tests/test_validations.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11323 2023-07-12 10:45:41.762050 flask_validators-1.0/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11017 2023-07-12 10:45:21.000000 flask_validators-1.0/README.md
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/flask_validators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      299 2023-07-12 09:39:41.000000 flask_validators-1.0/flask_validators/__init__.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/flask_validators/controllers/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      121 2023-07-12 07:54:56.000000 flask_validators-1.0/flask_validators/controllers/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      217 2023-07-12 07:55:02.000000 flask_validators-1.0/flask_validators/controllers/error_handler.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-1.0/flask_validators/controllers/validator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/flask_validators/decorators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      119 2023-07-12 09:37:40.000000 flask_validators-1.0/flask_validators/decorators/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     7244 2023-07-12 10:29:44.000000 flask_validators-1.0/flask_validators/decorators/validation_decorator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/flask_validators/models/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      375 2023-07-12 10:31:46.000000 flask_validators-1.0/flask_validators/models/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5731 2023-07-10 09:41:11.000000 flask_validators-1.0/flask_validators/models/fields.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5423 2023-07-10 09:41:57.000000 flask_validators-1.0/flask_validators/models/schema.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     2530 2023-07-12 09:22:12.000000 flask_validators-1.0/flask_validators/models/validate_db.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      462 2023-07-12 10:30:46.000000 flask_validators-1.0/flask_validators/models/validate_llm.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/flask_validators.egg-info/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)    11323 2023-07-12 10:45:41.000000 flask_validators-1.0/flask_validators.egg-info/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      736 2023-07-12 10:45:41.000000 flask_validators-1.0/flask_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-12 10:45:41.000000 flask_validators-1.0/flask_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       24 2023-07-12 10:45:41.000000 flask_validators-1.0/flask_validators.egg-info/requires.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-12 10:45:41.000000 flask_validators-1.0/flask_validators.egg-info/top_level.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-12 10:45:41.762050 flask_validators-1.0/setup.cfg
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      727 2023-07-12 10:45:39.000000 flask_validators-1.0/setup.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-12 10:45:41.762050 flask_validators-1.0/tests/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-1.0/tests/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     2742 2023-07-12 10:30:32.000000 flask_validators-1.0/tests/test_flask.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-1.0/tests/test_schemas.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-1.0/tests/test_validations.py
```

### Comparing `flask_validators-0.7/PKG-INFO` & `flask_validators-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_validators
-Version: 0.7
+Version: 1.0
 Summary: Flask request validation
 Author: Dimitri Zhorzholiani
 Author-email: zhorzholiani.dimitri@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
@@ -16,18 +16,14 @@
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
-<p align="center">
-  <img src="./carbon.png" alt="CLI" width="738">
-</p>
-
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator. 
 3. The validation schema specifies the structure of the expected data and the validation rules for each field.
@@ -219,12 +215,9 @@
     # Validation logic
     if valid:
         return True, None
     else:
         return False, 'Validation failed.'
 ```
 
-## Currently Working
-Currently I am working on database integration support, any help will be appreciated
-
 ## Error Handling
 If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
```

### Comparing `flask_validators-0.7/README.md` & `flask_validators-1.0/flask_validators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+Metadata-Version: 2.1
+Name: flask-validators
+Version: 1.0
+Summary: Flask request validation
+Author: Dimitri Zhorzholiani
+Author-email: zhorzholiani.dimitri@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Flask Validator
 
 Flask Validator is a powerful package designed to simplify data validation in Flask applications. It provides an easy-to-use interface for defining data validation rules and seamlessly integrates with Flask routes using a custom decorator.
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
-<p align="center">
-  <img src="./carbon.png" alt="CLI" width="738">
-</p>
-
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator. 
 3. The validation schema specifies the structure of the expected data and the validation rules for each field.
@@ -207,12 +215,9 @@
     # Validation logic
     if valid:
         return True, None
     else:
         return False, 'Validation failed.'
 ```
 
-## Currently Working
-Currently I am working on database integration support, any help will be appreciated
-
 ## Error Handling
-If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
+If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
```

### Comparing `flask_validators-0.7/flask_validators/controllers/validator.py` & `flask_validators-1.0/flask_validators/controllers/validator.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/flask_validators/decorators/validation_decorator.py` & `flask_validators-1.0/flask_validators/decorators/validation_decorator.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/flask_validators/models/fields.py` & `flask_validators-1.0/flask_validators/models/fields.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/flask_validators/models/schema.py` & `flask_validators-1.0/flask_validators/models/schema.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/flask_validators/models/validate_db.py` & `flask_validators-1.0/flask_validators/models/validate_db.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/flask_validators.egg-info/PKG-INFO` & `flask_validators-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: flask-validators
-Version: 0.7
-Summary: Flask request validation
-Author: Dimitri Zhorzholiani
-Author-email: zhorzholiani.dimitri@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Flask Validator
 
 Flask Validator is a powerful package designed to simplify data validation in Flask applications. It provides an easy-to-use interface for defining data validation rules and seamlessly integrates with Flask routes using a custom decorator.
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
@@ -219,12 +207,9 @@
     # Validation logic
     if valid:
         return True, None
     else:
         return False, 'Validation failed.'
 ```
 
-## Currently Working
-Currently I am working on database integration support, any help will be appreciated
-
 ## Error Handling
-If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
+If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
```

### Comparing `flask_validators-0.7/flask_validators.egg-info/SOURCES.txt` & `flask_validators-1.0/flask_validators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/setup.py` & `flask_validators-1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r', encoding='utf-8') as f:
+with open('READMEPypi.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="flask_validators",
-    version="0.7",
+    version="1.0",
     packages=find_packages(),
     description="Flask request validation",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Dimitri Zhorzholiani",
     author_email="zhorzholiani.dimitri@gmail.com",
     classifiers=[
```

### Comparing `flask_validators-0.7/tests/test_flask.py` & `flask_validators-1.0/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.7/tests/test_validations.py` & `flask_validators-1.0/tests/test_validations.py`

 * *Files identical despite different names*

