# Comparing `tmp/kobold-7.tar.gz` & `tmp/kobold-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kobold-7.tar", last modified: Fri Sep 25 19:07:00 2015, max compression
+gzip compressed data, was "dist/kobold-9.tar", last modified: Wed Jan 27 20:35:03 2016, max compression
```

## Comparing `kobold-7.tar` & `kobold-9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2015-09-25 19:07:00.000000 kobold-7/
-drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        7 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/top_level.txt
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        1 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/dependency_links.txt
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      176 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/PKG-INFO
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)       20 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/requires.txt
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      433 2015-09-25 19:07:00.000000 kobold-7/kobold.egg-info/SOURCES.txt
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)       59 2015-09-25 19:07:00.000000 kobold-7/setup.cfg
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      200 2015-09-25 19:06:26.000000 kobold-7/setup.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      176 2015-09-25 19:07:00.000000 kobold-7/PKG-INFO
-drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2015-09-25 19:07:00.000000 kobold-7/kobold/
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        0 2015-06-15 19:04:48.000000 kobold-7/kobold/__init__.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1230 2015-09-25 18:59:43.000000 kobold-7/kobold/response.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     4007 2015-08-04 21:56:46.000000 kobold-7/kobold/doubles.py
-drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2015-09-25 19:07:00.000000 kobold-7/kobold/tests/
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        0 2015-06-15 20:42:51.000000 kobold-7/kobold/tests/__init__.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     6482 2015-09-09 21:03:40.000000 kobold-7/kobold/tests/test_compare.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     3933 2015-07-16 15:45:53.000000 kobold-7/kobold/tests/test_doubles.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     2267 2015-07-06 19:09:39.000000 kobold-7/kobold/tests/test_assertions.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1065 2015-07-27 19:35:50.000000 kobold-7/kobold/tests/test_swap.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)    15061 2015-09-09 21:34:48.000000 kobold-7/kobold/compare.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      448 2015-08-10 19:40:14.000000 kobold-7/kobold/hash_functions.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      950 2015-07-16 15:54:27.000000 kobold-7/kobold/assertions.py
--rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1050 2015-09-09 21:35:12.000000 kobold-7/kobold/swap.py
+drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2016-01-27 20:35:03.000000 kobold-9/
+drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)       47 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/pbr.json
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        7 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/top_level.txt
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        1 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/dependency_links.txt
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      176 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/PKG-INFO
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)       21 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/requires.txt
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      458 2016-01-27 20:35:03.000000 kobold-9/kobold.egg-info/SOURCES.txt
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)       59 2016-01-27 20:35:03.000000 kobold-9/setup.cfg
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      200 2016-01-27 20:32:55.000000 kobold-9/setup.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      176 2016-01-27 20:35:03.000000 kobold-9/PKG-INFO
+drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2016-01-27 20:35:03.000000 kobold-9/kobold/
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        0 2015-06-15 19:04:48.000000 kobold-9/kobold/__init__.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1230 2015-09-30 16:10:09.000000 kobold-9/kobold/response.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     4198 2016-01-25 20:27:57.000000 kobold-9/kobold/doubles.py
+drwxrwxr-x   0 krieghan  (1000) krieghan  (1000)        0 2016-01-27 20:35:03.000000 kobold-9/kobold/tests/
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)        0 2015-06-15 20:42:51.000000 kobold-9/kobold/tests/__init__.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     7998 2015-11-09 20:57:36.000000 kobold-9/kobold/tests/test_compare.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     4511 2016-01-25 20:34:25.000000 kobold-9/kobold/tests/test_doubles.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     2267 2015-07-06 19:09:39.000000 kobold-9/kobold/tests/test_assertions.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1065 2015-07-27 19:35:50.000000 kobold-9/kobold/tests/test_swap.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)    16028 2015-11-16 21:06:42.000000 kobold-9/kobold/compare.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      448 2015-08-10 19:40:14.000000 kobold-9/kobold/hash_functions.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)      950 2015-07-16 15:54:27.000000 kobold-9/kobold/assertions.py
+-rw-rw-r--   0 krieghan  (1000) krieghan  (1000)     1050 2015-10-05 16:30:16.000000 kobold-9/kobold/swap.py
```

### Comparing `kobold-7/kobold/response.py` & `kobold-9/kobold/response.py`

 * *Files identical despite different names*

### Comparing `kobold-7/kobold/doubles.py` & `kobold-9/kobold/doubles.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
         else:
             return types.MethodType(self, instance)
 
+    def __getattr__(self, attr):
+        try:
+            return super(SpyFunction, self).__getattr__(attr)
+        except AttributeError:
+            return getattr(self.stub_function, attr)
+
 def get_spy_class(*methods_to_add):
 
     class SpyClass(object):
         pass
 
     methods_to_add = set(methods_to_add)
     methods_to_add.add('__init__')
@@ -125,9 +131,7 @@
 
         if stub_type == 'callable':
             return stub_value(*args, **kwargs)
 
         if stub_type == 'exception':
             raise stub_value
 
-
-
```

### Comparing `kobold-7/kobold/tests/test_compare.py` & `kobold-9/kobold/tests/test_compare.py`

 * *Files 13% similar despite different names*

```diff
@@ -184,8 +184,52 @@
         expected = set([1, 2, 3])
         actual = set([1, 3, 4])
         self.assertEqual(
             (set([2]), set([4])),
             compare.compare(expected, actual))
 
 
+    def test_tuples(self):
+        expected = (1, 2, 3, 4)
+        actual = (1, 2, 4, 4)
+        self.assertEqual(
+            (('_', '_', 3, '_'), ('_', '_', 4, '_')),
+            compare.compare(expected, actual))
+
+    def test_list_of_tuples(self):
+        expected = [(1, 2), (3, 4), (5, 6)]
+        actual = [(1, 2), (3, 5), (5, 6)]
+        self.assertEqual(
+            (['_', ('_', 4), '_'], ['_', ('_', 5), '_']),
+            compare.compare(expected, actual))
+
+    def test_tuple_of_tuples(self):
+        expected = ((1, 2), (3, 4), (5, 6))
+        actual = ((1, 2), (3, 5), (5, 6))
+        self.assertEqual(
+            (('_', ('_', 4), '_'), ('_', ('_', 5), '_')),
+            compare.compare(expected, actual))
+
+    def test_tuple_of_lists(self):
+        expected = ([1, 2], [3, 4], [5, 6])
+        actual = ([1, 2], [3, 5], [5, 6])
+        self.assertEqual(
+            (('_', ['_', 4], '_'), ('_', ['_', 5], '_')),
+            compare.compare(expected, actual))
+
+    def test_sets_of_distinct_tuples(self):
+        expected = set([(1, 2)])
+        actual = set([(3, 4)])
+        self.assertEqual(
+            (set([(1, 2)]), set([(3, 4)])),
+            compare.compare(expected, actual))
+
+    def test_sets_of_intersecting_tuples(self):
+        expected = set([(1, 2)])
+        actual = set([(2, 3)])
+        self.assertEqual(
+            (set([(1, 2)]), set([(2, 3)])),
+            compare.compare(
+                expected, 
+                actual,
+                type_compare={'ordered' : False}))
```

### Comparing `kobold-7/kobold/tests/test_doubles.py` & `kobold-9/kobold/tests/test_doubles.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,7 +115,21 @@
         self.assertEquals(1, spy_function(1))
         self.assertEquals(1, spy_function("apple"))
         self.assertEquals(1, spy_function(keyword="orange"))
 
         self.assertEquals([((1,), {}), (("apple",), {}), ((), {'keyword' : 'orange'})],
                           spy_function.calls)
 
+
+class TestRoutableSpyFunction(unittest.TestCase):
+    def test_delegation(self):
+        spy_function = doubles.SpyFunction(
+                stub_function_factory=doubles.RoutableStubFunction)
+        spy_function.add_route(
+                condition=(1, 1),
+                stub_type='value',
+                stub_value=1)
+        self.assertEquals(1, spy_function(1, 1))
+        self.assertRaises(doubles.StubRoutingException,
+                          spy_function,
+                          1, 2)
+        self.assertEquals([((1, 1), {}), ((1, 2), {})], spy_function.calls)
```

### Comparing `kobold-7/kobold/tests/test_assertions.py` & `kobold-9/kobold/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `kobold-7/kobold/tests/test_swap.py` & `kobold-9/kobold/tests/test_swap.py`

 * *Files identical despite different names*

### Comparing `kobold-7/kobold/compare.py` & `kobold-9/kobold/compare.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,24 +48,25 @@
                 return True
             except:
                 return False
         elif self.rule is None or self.rule == 'no_rules':
             return True
         
 class ListDiff(list):
-    def __init__(self, arr=None):
+    def __init__(self, arr=None, display_type=list):
         if arr is None:
             arr = []
         self.with_positions = arr
+        self.display_type = display_type
         val = [x for x in arr if x != '_']
         super(ListDiff, self).__init__(val)
 
     def display(self):
         to_display = []
-        return self.with_positions
+        return self.display_type(self.with_positions)
 
     def append_match(self):
         self.with_positions.append('_')
 
     def append(self, value):
         super(ListDiff, self).append(value)
         self.with_positions.append(value)
@@ -112,19 +113,25 @@
                 return ("dontcare: %s" % expected.rule,
                         actual)
         elif (acts_like_a_hash(expected) and 
               acts_like_a_hash(actual)):
             return cls.hash_compare(expected, 
                                     actual, 
                                     type_compare)
+        elif (isinstance(expected, tuple) and isinstance(actual, tuple)):
+            return cls.list_compare(expected,
+                                    actual,
+                                    type_compare,
+                                    iter_type=tuple)
         elif (acts_like_a_list(expected) and 
               acts_like_a_list(actual)):
             return cls.list_compare(expected, 
                                     actual,
-                                    type_compare)
+                                    type_compare,
+                                    iter_type=list)
         elif (type(expected) == re._pattern_type and 
               isinstance(actual, basestring)):
             match = expected.match(actual)
             if match:
                 return 'match'
             else:
                 return ('regex: %s' % expected.pattern, actual)
@@ -188,17 +195,18 @@
         else:
             return (expected_return, actual_return)
 
     @classmethod
     def ordered_list_compare(cls,
                              expected,
                              actual,
-                             type_compare):
-        expected_elements = ListDiff()
-        actual_elements = ListDiff()
+                             type_compare,
+                             iter_type=list):
+        expected_elements = ListDiff(display_type=iter_type)
+        actual_elements = ListDiff(display_type=iter_type)
 
         for i in range(max(len(expected), len(actual))):
             if len(expected) > i:
                 expected_value = expected[i]
             else:
                 expected_value = NotPresent
             if len(actual) > i:
@@ -224,15 +232,16 @@
             return (expected_elements.display(),
                     actual_elements.display())
 
     @classmethod
     def unordered_list_compare(cls,
                                expected,
                                actual,
-                               type_compare):
+                               type_compare,
+                               iter_type=list):
         # Make a list of all the indexes of the "expected" list 
         # and the "actual" list.  
         # Iterate through the "expected" list.  For each item,
         # try to find a corresponding match in the "actual" list
         # (by iterating through that - n^2 style).
         # If a match is found, remove the corresponding indexes
         # from the "expected" and "actual" lists.  What we're left
@@ -307,16 +316,16 @@
             if missing_actual_index is not None:
                 displayed_actuals[missing_actual_index] = displayed_actual
 
         # For each element of the expected and actual lists,
         # if there was a match, just append the "match" character
         # (_).  If there wasn't a match, append the in-order diff
         # from above.
-        expected_return = ListDiff()
-        actual_return = ListDiff()
+        expected_return = ListDiff(display_type=iter_type)
+        actual_return = ListDiff(display_type=iter_type)
         for i in range(len(expected)):
             if i in missing_expected_indexes:
                 expected_return.append(displayed_expecteds[i])
             else:
                 expected_return.append_match()
 
         for j in range(len(actual)):
@@ -332,15 +341,16 @@
             return (expected_return.display(),
                     actual_return.display())
                                  
     @classmethod
     def list_compare(cls,
                      expected,
                      actual,
-                     type_compare):
+                     type_compare,
+                     iter_type=list):
         default_type_compare =\
             {'hash' : 'full',
              'ordered' : True}
 
         type_compare =\
             combine(default_type_compare, type_compare)
 
@@ -349,20 +359,22 @@
             expected = list(expected)
             actual = list(actual)
         else:
             isset = False
 
         if type_compare['ordered'] and not isset:
             ret = cls.ordered_list_compare(expected,
-                                            actual,
-                                            type_compare)
+                                           actual,
+                                           type_compare,
+                                           iter_type=iter_type)
         else:
             ret = cls.unordered_list_compare(expected,
-                                              actual,
-                                              type_compare)
+                                             actual,
+                                             type_compare,
+                                             iter_type=iter_type)
         if ret == 'match' or not isset:
             return ret
         else:
             ret_exp, ret_act = ret
             ret_exp = [x for x in ret_exp if x != '_']
             ret_act = [x for x in ret_act if x != '_']
             return (set(ret_exp), set(ret_act))
@@ -372,16 +384,18 @@
     # for intelligently displaying unordered diffs of lists
     @classmethod
     def display(cls, element, other_element):
         if type(element) == DontCare:
             return "dontcare: %s" % expected.rule
         elif acts_like_a_hash(element) and acts_like_a_hash(other_element):
             return cls.display_hash(element, other_element)
+        elif isinstance(element, tuple) and isinstance(other_element, tuple):
+            return cls.display_list(element, other_element, iter_type=tuple)
         elif acts_like_a_list(element) and acts_like_a_list(other_element):
-            return cls.display_list(element, other_element)
+            return cls.display_list(element, other_element, iter_type=list)
         elif type(element) == re._pattern_type:
             return 'regex: %s' % element.pattern
         elif type(other_element).__name__ == 'ParsingHint':
             return cls.display(other_element.parse(element), other_element.payload)
         elif type(element).__name__ == 'ParsingHint':
             return cls.display(element.payload, element.parse(element))
         else:
@@ -392,15 +406,15 @@
         display_hash = {}
         for key in one_hash.keys():
             display_hash[key] = cls.display(one_hash.get(key), other_hash.get(key))
 
         return display_hash
 
     @classmethod
-    def display_list(cls, one_list, other_list):
+    def display_list(cls, one_list, other_list, iter_type=list):
         max_len = max(len(one_list), len(other_list))
         display_list = []
 
         for i in range(max_len):
             if i > len(one_list):
                 element = NotPresent
             else:
@@ -408,9 +422,10 @@
 
             if i > len(other_list):
                 other_element = NotPresent
             else:
                 other_element = other_list[i]
 
             display_list.append(cls.display(element, other_element))
+        return iter_type(display_list)
```

### Comparing `kobold-7/kobold/assertions.py` & `kobold-9/kobold/assertions.py`

 * *Files identical despite different names*

### Comparing `kobold-7/kobold/swap.py` & `kobold-9/kobold/swap.py`

 * *Files identical despite different names*

