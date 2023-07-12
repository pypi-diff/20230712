# Comparing `tmp/sanctify-1.0.1.tar.gz` & `tmp/sanctify-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.1.tar", last modified: Mon Jul 10 07:28:08 2023, max compression
+gzip compressed data, was "sanctify-1.0.2.tar", last modified: Wed Jul 12 20:54:18 2023, max compression
```

## Comparing `sanctify-1.0.1.tar` & `sanctify-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.395044 sanctify-1.0.1/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.1/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10059 2023-07-10 07:28:08.394822 sanctify-1.0.1/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9344 2023-07-10 07:25:37.000000 sanctify-1.0.1/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1642 2023-07-10 07:27:50.000000 sanctify-1.0.1/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.393844 sanctify-1.0.1/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7047 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2593 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11965 2023-07-10 07:25:08.000000 sanctify-1.0.1/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8726 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3410 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     6399 2023-07-10 07:25:09.000000 sanctify-1.0.1/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.394607 sanctify-1.0.1/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10059 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-10 07:28:08.395081 sanctify-1.0.1/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:54:18.876271 sanctify-1.0.2/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.2/LICENSE.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10044 2023-07-12 20:54:18.875900 sanctify-1.0.2/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9429 2023-07-12 20:53:57.000000 sanctify-1.0.2/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1552 2023-07-12 20:54:04.000000 sanctify-1.0.2/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:54:18.875178 sanctify-1.0.2/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      833 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7629 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2613 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.2/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12024 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8744 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3417 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9129 2023-07-12 20:53:57.000000 sanctify-1.0.2/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:54:18.875676 sanctify-1.0.2/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10044 2023-07-12 20:54:18.000000 sanctify-1.0.2/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-12 20:54:18.000000 sanctify-1.0.2/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-12 20:54:18.000000 sanctify-1.0.2/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-12 20:54:18.000000 sanctify-1.0.2/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-12 20:54:18.876309 sanctify-1.0.2/setup.cfg
```

### Comparing `sanctify-1.0.1/LICENSE.txt` & `sanctify-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.1/PKG-INFO` & `sanctify-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.1
+Version: 1.0.2
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Sanctify
 
 Sanctify is a Python package designed to facilitate data cleansing and validation operations on pandas DataFrames. It provides a set of predefined transformations and validations that can be applied to different columns of a DataFrame based on a column mapping schema. The package allows you to define data types, transformations, and validations for each column, making it easy to clean and validate your data.
 
@@ -55,15 +53,15 @@
 from sanctify.processor import process_cleansed_df
 from sanctify.transformer import Transformer
 from sanctify.validator import Validator
 from functools import wraps
 
 
 class MyCustomDataTypes(StrEnum):
-    """Enumeration for different data types in a sheet."""
+    """Enumeration for different data types in a csv."""
 
     ACCOUNT = auto()
     NAME = auto()
     DOB = auto()
     PHONE = auto()
     ZIP_CODE = auto()
     AMOUNT = auto()
@@ -71,15 +69,15 @@
     DECIMAL = auto()
     SSN = auto()
     STATE = auto()
     DATE = auto()
 
 
 class MyMandatoryColumns(StrEnum):
-    """Enumeration for mandatory columns in the Skit."""
+    """Enumeration for mandatory columns in a csv."""
 
     ACCOUNT_NUMBER = "Account"
     STATE = "State"
     CALLER_NUMBER = "Phone"
     FIRST_NAME = "First Name"
     LAST_NAME = "Last Name"
     ZIP_CODE = "Zip Code"
@@ -232,21 +230,21 @@
 
 
 @time_profiler
 def test_csv_parsing():
     """Function to test parsing operations."""
     input_file_path = "<path to>/input.csv"
     cleansed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_input.csv"
+        "<path to>/CLEANSED_input.csv"
     )
     processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/PROCESSED_input.csv"
+        "<path to>/PROCESSED_input.csv"
     )
     cleansed_processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_PROCESSED_input.csv"
+        "<path to>/CLEANSED_PROCESSED_input.csv"
     )
 
     input_df = pd.read_csv(input_file_path, dtype=str)
     cleanser = Cleanser(df=input_df, column_mapping_schema=COLUMN_MAPPING_SCHEMA)
 
     # Step 2: Read the CSV data
 
@@ -286,7 +284,10 @@
 
 if __name__ == "__main__":
     test_csv_parsing()  # TIME TAKEN TO test_csv_parsing = x.yza seconds
 ```
 
 ## Contributing
 Contributions to Sanctify are welcome! If you find any bugs, have feature requests, or want to contribute code, please open an issue or submit a pull request on the [GitHub repository](https://github.com/skit-ai/sanctify/).
+
+## Code Coverage
+[![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
```

### Comparing `sanctify-1.0.1/README.md` & `sanctify-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from sanctify.processor import process_cleansed_df
 from sanctify.transformer import Transformer
 from sanctify.validator import Validator
 from functools import wraps
 
 
 class MyCustomDataTypes(StrEnum):
-    """Enumeration for different data types in a sheet."""
+    """Enumeration for different data types in a csv."""
 
     ACCOUNT = auto()
     NAME = auto()
     DOB = auto()
     PHONE = auto()
     ZIP_CODE = auto()
     AMOUNT = auto()
@@ -54,15 +54,15 @@
     DECIMAL = auto()
     SSN = auto()
     STATE = auto()
     DATE = auto()
 
 
 class MyMandatoryColumns(StrEnum):
-    """Enumeration for mandatory columns in the Skit."""
+    """Enumeration for mandatory columns in a csv."""
 
     ACCOUNT_NUMBER = "Account"
     STATE = "State"
     CALLER_NUMBER = "Phone"
     FIRST_NAME = "First Name"
     LAST_NAME = "Last Name"
     ZIP_CODE = "Zip Code"
@@ -215,21 +215,21 @@
 
 
 @time_profiler
 def test_csv_parsing():
     """Function to test parsing operations."""
     input_file_path = "<path to>/input.csv"
     cleansed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_input.csv"
+        "<path to>/CLEANSED_input.csv"
     )
     processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/PROCESSED_input.csv"
+        "<path to>/PROCESSED_input.csv"
     )
     cleansed_processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_PROCESSED_input.csv"
+        "<path to>/CLEANSED_PROCESSED_input.csv"
     )
 
     input_df = pd.read_csv(input_file_path, dtype=str)
     cleanser = Cleanser(df=input_df, column_mapping_schema=COLUMN_MAPPING_SCHEMA)
 
     # Step 2: Read the CSV data
 
@@ -269,7 +269,10 @@
 
 if __name__ == "__main__":
     test_csv_parsing()  # TIME TAKEN TO test_csv_parsing = x.yza seconds
 ```
 
 ## Contributing
 Contributions to Sanctify are welcome! If you find any bugs, have feature requests, or want to contribute code, please open an issue or submit a pull request on the [GitHub repository](https://github.com/skit-ai/sanctify/).
+
+## Code Coverage
+[![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
```

### Comparing `sanctify-1.0.1/pyproject.toml` & `sanctify-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -59,24 +59,22 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Allowed config based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/skit-ai/sanctify"
 "Bug Tracker" = "https://github.com/skit-ai/sanctify/issues"
```

### Comparing `sanctify-1.0.1/sanctify/cleanser.py` & `sanctify-1.0.2/sanctify/cleanser.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,7 +175,24 @@
             duplicate_rows = self.df.duplicated(subset=columns, keep="first")
 
             error_message = f"Duplicate entry for {', '.join(columns)} passed"
             self.df.loc[duplicate_rows, DefaultColumns.ERROR.value] = error_message
             result = self.df
 
         return result
+
+    def drop_fully_duplicate_rows(self, inplace: bool = True) -> pd.DataFrame:
+        """
+        Drops rows from the DataFrame that are fully duplicates.
+
+        Args:
+            inplace (bool): Whether to drop rows in-place or return a new DataFrame.
+
+        Returns:
+            pd.DataFrame: The DataFrame with fully duplicate rows dropped.
+        """
+        if inplace is True:
+            self.df.drop_duplicates(inplace=inplace, ignore_index=True)
+        else:
+            self.df = self.df.drop_duplicates(inplace=inplace, ignore_index=True)
+
+        return self.df
```

### Comparing `sanctify-1.0.1/sanctify/constants.py` & `sanctify-1.0.2/sanctify/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """
     Enum representing abstract data types.
     """
 
     TEXT = auto()
     DECIMAL = auto()
     EMAIL = auto()
+    NUMBER = auto()
 
 
 class Constants(StrEnum):
     """
     Enum representing various constants.
     """
```

### Comparing `sanctify-1.0.1/sanctify/processor.py` & `sanctify-1.0.2/sanctify/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     match data_type_name_for_column:
         case PrimitiveDataTypes.BOOLEAN.value:
             return [Transformer.parse_boolean]
 
         case PrimitiveDataTypes.FLOAT.value | AbstractDataTypes.DECIMAL.value:
             return [float]
 
-        case PrimitiveDataTypes.INTEGER.value:
+        case PrimitiveDataTypes.INTEGER.value | AbstractDataTypes.NUMBER.value:
             return [int]
 
         case PrimitiveDataTypes.STRING.value | AbstractDataTypes.TEXT.value:
             return [str]
 
         case _:
             return []
@@ -168,15 +168,15 @@
             data_type_config_for_column.get(Constants.POST_PROCESSING_DATA_TYPE.value, ""),
             None,
         )
     else:
         return dtype_in_col_config
 
 
-def apply_functions(value, functions: list[Callable | tuple[Callable, dict]]) -> pd.Series:
+def apply_functions(value, col_name: str, functions: list[Callable | tuple[Callable, dict]]) -> pd.Series:
     """
     Applies a series of transformation and validation functions to a value.
 
     Args:
         value: The value to apply the functions to.
         functions (list[Callable]): List of transformation and validation functions.
         functions (tuple[Callable, dict]]): List of tuple of transformation and validation functions and additional kwargs.
@@ -199,15 +199,15 @@
 
         try:
             func_value = func(func_value, **kwargs)
 
         except Exception as err:
             logger.error(f"FAILED: {func.__name__ = } with {value = } | {kwargs = } | {(str(err)) = }")
             logger.error(f"{err = }")
-            error_message = f"@validation_error@ : {str(err)} | {func_value}"
+            error_message = f"{col_name} : {str(err)} | {func_value}"
             func_value = None
             break
 
         logger.debug(f"Result: {func.__name__ = } with {value = } | {kwargs = } | {func_value = }")
 
     # Return the modified value and error message (if any)
     return pd.Series(
@@ -279,15 +279,15 @@
         logger.debug(f"Running {col_name}: {transformations = }")
         logger.debug(f"Running {col_name}: {validations = }")
 
         data_type_name_for_column: str = col_config.get(Constants.DATA_TYPE.value)
         primitive_data_type_classes = handle_additional_transformations_and_validations(
             data_type_name_for_column=data_type_name_for_column
         )
-        applied_series = df[col_name].apply(apply_functions, functions=transformations + validations)
+        applied_series = df[col_name].apply(apply_functions, col_name=col_name, functions=transformations + validations)
 
         # Update cell values
         successful_rows = applied_series[DefaultColumns.ERROR.value].isnull()
         df.loc[successful_rows, col_name] = applied_series.loc[successful_rows, DefaultColumns.VALUE_PLACEHOLDER.value]
 
         # Update "Error" column for errored rows
         errored_rows = applied_series[DefaultColumns.ERROR.value].notnull()
```

### Comparing `sanctify-1.0.1/sanctify/transformer.py` & `sanctify-1.0.2/sanctify/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         Raises:
             ValidationError: If the input string is not a valid boolean.
         """
         bool_string = str(value).lower()
         if bool_string in {"true", "false"}:
             return str(value).lower() == "true"
         else:
-            raise ValidationError(f"Invalid boolean input: {bool_string = } | ({type(value)}, {value})")
+            raise ValidationError(f"Invalid boolean input: {bool_string = }")
 
     @staticmethod
     def remove_dot_from_string(value: str) -> str:
         """
         Removes all dots from a string except for "jr." and "sr.".
 
         Args:
@@ -171,15 +171,15 @@
             logger.exception(f"{str(err) = }")
             raise err
 
         try:
             parsed_datetime = parser.parse(value, dayfirst=day_first, yearfirst=year_first)
         except parser.ParserError as err:
             logger.exception(f"{str(err) = } | DEBUG: {error_message}")
-            raise err
+            raise ValidationError(f"Invalid date passed: {str(err)}")
         else:
             if return_datetime is True:
                 return parsed_datetime
             else:
                 return str(parsed_datetime.date())
 
     @staticmethod
@@ -247,15 +247,15 @@
                 return int(cleaned_number.removeprefix("0"))
 
             else:
                 phone_number = phonenumbers.parse(number=cleaned_number)
 
         except phonenumbers.NumberParseException as err:
             # Raise an error if the phone number is invalid
-            raise ValidationError(f"{cleaned_number}: Invalid phone number | {str(err) = }")
+            raise ValidationError(f"{cleaned_number}: Invalid phone number | {str(err)}")
 
         else:
             return phone_number.national_number
 
     @staticmethod
     def extract_country_code(value: str) -> int | str | ValidationError:
         """
```

### Comparing `sanctify-1.0.1/sanctify/utils.py` & `sanctify-1.0.2/sanctify/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,18 @@
             ComparisonOperations.EQUALS_OPERATOR.value: lambda x, y: x == y,
             ComparisonOperations.NOT_EQUALS.value: lambda x, y: x != y,
             ComparisonOperations.NOT_EQUALS_OPERATOR.value: lambda x, y: x != y,
         }
         if operation in comparison_mapping:
             return comparison_mapping[operation](value, operand)
         else:
-            raise NotImplementedError(f"Unsupported: {err_message}")
+            raise NotImplementedError(f"Unsupported Comparision: {err_message}")
 
     except TypeError as err:
-        err = TypeError(f"Comparison Failed: {err_message}")
+        err = TypeError(f"System Error: {err_message}")
         logger.error(f"{str(err) = }")
         raise err
 
 
 def calculate_age(date_of_birth: date, current_date: date = date.today()) -> int:
     """
     Calculate the age based on the date of birth.
```

### Comparing `sanctify-1.0.1/sanctify.egg-info/PKG-INFO` & `sanctify-1.0.2/sanctify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.1
+Version: 1.0.2
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Sanctify
 
 Sanctify is a Python package designed to facilitate data cleansing and validation operations on pandas DataFrames. It provides a set of predefined transformations and validations that can be applied to different columns of a DataFrame based on a column mapping schema. The package allows you to define data types, transformations, and validations for each column, making it easy to clean and validate your data.
 
@@ -55,15 +53,15 @@
 from sanctify.processor import process_cleansed_df
 from sanctify.transformer import Transformer
 from sanctify.validator import Validator
 from functools import wraps
 
 
 class MyCustomDataTypes(StrEnum):
-    """Enumeration for different data types in a sheet."""
+    """Enumeration for different data types in a csv."""
 
     ACCOUNT = auto()
     NAME = auto()
     DOB = auto()
     PHONE = auto()
     ZIP_CODE = auto()
     AMOUNT = auto()
@@ -71,15 +69,15 @@
     DECIMAL = auto()
     SSN = auto()
     STATE = auto()
     DATE = auto()
 
 
 class MyMandatoryColumns(StrEnum):
-    """Enumeration for mandatory columns in the Skit."""
+    """Enumeration for mandatory columns in a csv."""
 
     ACCOUNT_NUMBER = "Account"
     STATE = "State"
     CALLER_NUMBER = "Phone"
     FIRST_NAME = "First Name"
     LAST_NAME = "Last Name"
     ZIP_CODE = "Zip Code"
@@ -232,21 +230,21 @@
 
 
 @time_profiler
 def test_csv_parsing():
     """Function to test parsing operations."""
     input_file_path = "<path to>/input.csv"
     cleansed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_input.csv"
+        "<path to>/CLEANSED_input.csv"
     )
     processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/PROCESSED_input.csv"
+        "<path to>/PROCESSED_input.csv"
     )
     cleansed_processed_output_file_path = (
-        "/Users/avijeetdiwaker/Downloads/CLEANSED_PROCESSED_input.csv"
+        "<path to>/CLEANSED_PROCESSED_input.csv"
     )
 
     input_df = pd.read_csv(input_file_path, dtype=str)
     cleanser = Cleanser(df=input_df, column_mapping_schema=COLUMN_MAPPING_SCHEMA)
 
     # Step 2: Read the CSV data
 
@@ -286,7 +284,10 @@
 
 if __name__ == "__main__":
     test_csv_parsing()  # TIME TAKEN TO test_csv_parsing = x.yza seconds
 ```
 
 ## Contributing
 Contributions to Sanctify are welcome! If you find any bugs, have feature requests, or want to contribute code, please open an issue or submit a pull request on the [GitHub repository](https://github.com/skit-ai/sanctify/).
+
+## Code Coverage
+[![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
```

