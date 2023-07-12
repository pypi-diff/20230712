# Comparing `tmp/sqlalchemy_mock-1.0.6.tar.gz` & `tmp/sqlalchemy_mock-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.6.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.7.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.6.tar` & `sqlalchemy_mock-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.6/README.md
--rw-r--r--   0        0        0      448 2023-07-03 19:55:22.578743 sqlalchemy_mock-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.6/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.6/sqlalchemy_mock/async_session.py
--rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.6/sqlalchemy_mock/execute.py
--rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.6/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     3508 2023-07-03 19:53:53.223210 sqlalchemy_mock-1.0.6/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     4625 2023-07-03 19:53:53.224051 sqlalchemy_mock-1.0.6/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.7/README.md
+-rw-r--r--   0        0        0      448 2023-07-12 20:58:25.988668 sqlalchemy_mock-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.7/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.7/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.7/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.7/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3508 2023-07-03 19:53:53.223210 sqlalchemy_mock-1.0.7/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     4860 2023-07-12 20:57:58.748570 sqlalchemy_mock-1.0.7/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.7/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.6/README.md` & `sqlalchemy_mock-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.6/sqlalchemy_mock/execute.py` & `sqlalchemy_mock-1.0.7/sqlalchemy_mock/execute.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.6/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.7/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.6/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.7/sqlalchemy_mock/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.6/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.7/sqlalchemy_mock/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         if not field in values:
             return False
 
     def _or_filter_handler(record: object, filter: object):
         result = False
         for part in filter:
             if not getattr(part.left, "clause_expr", None) is None and part.left.clause_expr.element.operator.__name__ == "comma_op":
-                record_field = getattr(record, part.left.clause_expr.element.clauses[0].name)
+                if isinstance(part.left.clause_expr.element.clauses[0], sqlalchemy.sql.elements.Cast):
+                    record_field = getattr(record, part.left.clause_expr.element.clauses[0].clause.name)
+                else:
+                    record_field = getattr(record, part.left.clause_expr.element.clauses[0].name)
+
                 if part.left.name in ("lower", "upper"):
                     record_field = getattr(record_field, part.left.name)()
 
                 if part.right.value in record_field:
                     result = True
 
         return result
```

### Comparing `sqlalchemy_mock-1.0.6/PKG-INFO` & `sqlalchemy_mock-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.6
+Version: 1.0.7
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

