# Comparing `tmp/datastax-0.3.1.tar.gz` & `tmp/datastax-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastax-0.3.1.tar", last modified: Wed Apr  6 12:21:56 2022, max compression
+gzip compressed data, was "datastax-0.4.0.tar", last modified: Wed Jul 12 03:19:41 2023, max compression
```

## Comparing `datastax-0.3.1.tar` & `datastax-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-06 12:21:44.000000 datastax-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8027 2022-04-06 12:21:56.422718 datastax-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6395 2022-04-06 12:21:44.000000 datastax-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.418718 datastax-0.3.1/datastax/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax/arrays/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/arrays/priority_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/arrays/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/arrays/stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax/linkedlists/
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/circular_linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/doubly_circular_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/doubly_linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/lru_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax/linkedlists/private_lists/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/private_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/private_lists/circular_linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/private_lists/doubly_circular_llist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/private_lists/doubly_linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/private_lists/linked_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/linkedlists/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax/trees/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/avl_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/expression_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/fibonacci_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/min_heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/min_segment_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax/trees/private_trees/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7471 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5148 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/private_trees/threaded_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     8672 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/splay_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/sum_segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-04-06 12:21:44.000000 datastax-0.3.1/datastax/trees/threaded_binary_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:21:56.422718 datastax-0.3.1/datastax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8027 2022-04-06 12:21:55.000000 datastax-0.3.1/datastax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-04-06 12:21:56.000000 datastax-0.3.1/datastax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 12:21:55.000000 datastax-0.3.1/datastax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 12:21:54.000000 datastax-0.3.1/datastax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-04-06 12:21:56.000000 datastax-0.3.1/datastax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-06 12:21:56.422718 datastax-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2022-04-06 12:21:44.000000 datastax-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 03:19:31.000000 datastax-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-12 03:19:41.368094 datastax-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-12 03:19:31.000000 datastax-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax/Arrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/priority_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/AbstractLists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/LRUCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Utils/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/datastax/trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/avl_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/expression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/fibonacci_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/heap_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/huffman_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/min_heap_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/min_segment_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/datastax/trees/private_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/huffman_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/red_black_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/segment_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/threaded_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/red_black_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/splay_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/sum_segment_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/threaded_binary_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:19:41.368094 datastax-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-12 03:19:31.000000 datastax-0.4.0/setup.py
```

### Comparing `datastax-0.3.1/LICENSE` & `datastax-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/README.md` & `datastax-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,88 @@
-    updated: Wednesday, 6th April 2022
+    updated: Sunday, 11th July 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
-    <img width=200 src="https://github.com/warmachine028/datastax/blob/main/assets/icon.png" alt="datastax"></a>
-    <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic"> Simplicity meets intelligence</p>
-    <a href="https://pypi.org/project/datastax" ><img alt="PyPI" src="https://img.shields.io/pypi/v/datastax?color=blueviolet"></a>
+        <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
+    </a>
+    <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
+    <a href="https://pypi.org/project/datastax">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/datastax?color=blueviolet">
+    </a>
     <a href="https://pypi.org/project/datastax/#files"><img alt="PyPI Downloads" src="https://img.shields.io/pypi/dm/datastax.svg?label=Pypi%20downloads"></a>
     <br>
-    <a href="https://github.com/warmachine028/datastax/releases/"> <img src="https://img.shields.io/github/v/release/warmachine028/datastax?color=brightgreen"></a>
-    <a href="https://github.com/warmachine028/datastax/releases/tag/"> <img src="https://img.shields.io/github/v/release/warmachine028/datastax?color=lightgreen&include_prereleases&label=pre%20release"> </a>
+    <a href="https://github.com/warmachine028/datastax/releases/"> 
+        <img src="https://img.shields.io/github/v/release/warmachine028/datastax?color=brightgreen">
+    </a>
+    <a href="https://github.com/warmachine028/datastax/releases/tag/"> 
+        <img src="https://img.shields.io/github/v/release/warmachine028/datastax?color=lightgreen&include_prereleases&label=pre%20release"> 
+    </a>
     <br>
     <img src="https://img.shields.io/github/stars/warmachine028/datastax">
-    <a href= "https://github.com/warmachine028/datastax/blob/main/LICENSE"><img src="https://img.shields.io/github/license/warmachine028/datastax?color=orange"></a>
-    <a href="https://github.com/warmachine028/datastax/network/members"><img src="https://img.shields.io/github/forks/warmachine028/datastax?color=cyan"></a>
+    <a href= "https://github.com/warmachine028/datastax/blob/main/LICENSE">
+        <img src="https://img.shields.io/github/license/warmachine028/datastax?color=orange">
+    </a>
+    <a href="https://github.com/warmachine028/datastax/network/members">
+        <img src="https://img.shields.io/github/forks/warmachine028/datastax?color=cyan">
+    </a>
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Added Mandatory Keyword arguments to avoid confusion in:
-  - Arrays 
-  - ThreadedBinaryTree 
-- Added High Quality PNGs in README.md
+- Refactored linkedlists -> Lists
+- Refactored arrays -> Arrays
+- Refactored private_lists -> AbstractLists
+- Refactored AbstractLists by converting all items to AbstractClass to prevent direct initialization.
+- Module Conventions converted to uppercase CamelCase from lowercase snake_case
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
 - [What's Next](#whats-next)
 
 ## Introduction
 
-- This is a very simple yet powerful project to implement day to day abstract data structures
-- A pure implementation of Python in representing Tree, Linkedlist and Array based datastructures in basic command
-  prompt
-- It helps visualize each data structure for better understanding
-- Students can be beneficial in using this Package
-- This project is still under construction
+- This library offers a simple yet powerful solution for implementing common abstract data structures.
+- With a pure Python implementation, it provides representations of tree, linked list, and array-based data structures
+  accessible through a basic command prompt interface.
+- The package includes visualization features that enhance the understanding of each data structure.
+- Students can greatly benefit from utilizing this package for their learning and educational purposes.
+- Please note that this project is currently a work in progress and undergoing active development.
 
 ## Problem Statement
 
-- Often at the beginning of B.Tech Course, CS students face a lot of problems understanding the internal architecture of
-  complex ADTs.
-- While solving coding challenges locally where test cases have to be written using these ADTs, it becomes really
-  cumbersome to write these data structures from scratch.
-- Also, when writing programs which implements these ADS, we encounter lots of errors just because we are unable to
-  preview what's actually going on under the hood.
+- Many CS students encounter difficulties in comprehending the intricate internal architecture of complex
+  Abstract Data Types (ADTs) during the initial stages of their B.Tech course.
+- When attempting to solve coding challenges that involve writing test cases using these ADTs, it becomes excessively
+  burdensome to manually create these data structures from scratch.
+- Furthermore, while developing programs that implement these ADTs, numerous errors are encountered due to the
+  inability to visualize and understand the underlying processes of these data structures.
 
 ## Benefits
 
-- Instant installation
-- Quick Updates
-- Very small size
-- No extra modules required
-- Written purely from scratch
-- Easy Documentation [Upcoming]
-- Command Line Demo
+- Swift installation process
+- Efficient and prompt updates
+- Minimal disk space usage due to its small size
+- No additional modules or dependencies needed
+- Developed entirely from scratch
+- Upcoming user-friendly documentation
+- Command line demonstration for easy usage
 
 ## Requirements
 
-- Runs on latest Python 3.7+
-- (WARNING: Though the module might run on py 3.7 error free, but it has been tested for 3.9+)
+- Runs on latest Python 3.11+
 - (Suggesting you to always update to the latest python version)
-- This Library requires no extra modules
 
 ## Installation
 
 1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to install datastax.
 
 ```bash
 pip install datastax
@@ -129,65 +139,67 @@
   ...
 ```
 
 ### Practical Usage
 
 - **Queue**
 
-![queue](./assets/Usage/queue.png)
+![queue](https://github.com/warmachine028/datastax/assets/75939390/0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409)
 
-![queue_output](./assets/Usage/queue_output.png)
+![queue_output](https://github.com/warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde)
 
----------------------------------------------------
+------------------------------------
+---------------
 
 - **BinaryTree**
 
-![BinaryTree](./assets/Usage/binaryTree.png)
+![binaryTree](https://github.com/warmachine028/datastax/assets/75939390/7228c4b4-def7-4c6b-9e29-e6e244c2c4c1)
 
-![BinaryTree_output](./assets/Usage/binaryTree_output.png)
+![binaryTree_output](https://github.com/warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c)
 
 ---------------------------------------------------
 
 - **MinHeapTree**
 
-![MinHeapTree](./assets/Usage/mht.png)
+![mht](https://github.com/warmachine028/datastax/assets/75939390/1c00a207-9ea0-4965-898f-29e37883fac5)
 
-![MinHeapTree_output](./assets/Usage/mht_output.png)
+![mht_output](https://github.com/warmachine028/datastax/assets/75939390/fcfe24d9-6b80-4b16-873c-3f5c3d808d70)
 
 ---------------------------------------------------
 
 - **ThreadedBinaryTree**
 
-![ThreadedBinaryTree](./assets/Usage/tbt.png)
+![tbt](https://github.com/warmachine028/datastax/assets/75939390/ab2f2572-1474-4d82-9138-b8ee85869114)
 
-![ThreadedBinaryTree_output](./assets/Usage/tbt_output.png)
+![tbt_output](https://github.com/warmachine028/datastax/assets/75939390/9e77c5dc-082c-471b-90d5-33792673bdf3)
 
 ---------------------------------------------------
 
 - **SumSegmentTree**
 
-![SumSegmentTree](./assets/Usage/sst.png)
+![sst](https://github.com/warmachine028/datastax/assets/75939390/7bdcfd6e-37ac-4421-b6d2-acd59cf4976c)
 
-![SumSegmentTree_Output](./assets/Usage/sst_output.png)
+![sst_output](https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-88c7-40e4dcc11215)
 
 ---------------------------------------------------
 
 - **HuffmanTree**
 
-![HuffmanTree](./assets/Usage/hft.png)
+![hft](https://github.com/warmachine028/datastax/assets/75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e)
 
-![HuffmanTree_Output](./assets/Usage/hft_output.png)
+![hft_output](https://github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-8dbf91c008a2)
 
 ---------------------------------------------------
 
 - **RedBlackTree**
 
-![RedBlackTree](./assets/Usage/rbt.png)
+![rbt](https://github.com/warmachine028/datastax/assets/75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba)
 
-![RedBlackTreeOutput](./assets/Usage/rbt_output.png)
+![rbt_output](https://github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-db84dbf274f0)
 
 ## What's Next
 
 - Enhanced Documentation
 - Better TestCases for Huffman Tree
 - Better TestCases for Segment Trees
 - Test Cases for Fibonacci Tree
+- Refactoring Arrays SubPackage
```

#### html2text {}

```diff
@@ -1,50 +1,55 @@
- updated: Wednesday, 6th April 2022
+ updated: Sunday, 11th July 2023
                                   [datastax]
                          Simplicity meets intelligence
                            [PyPI] [PyPI_Downloads]
             [https://img.shields.io/github/v/release/warmachine028/
      datastax?color=brightgreen] [https://img.shields.io/github/v/release/
                                 warmachine028/
       datastax?color=lightgreen&include_prereleases&label=pre%20release]
     [https://img.shields.io/github/stars/warmachine028/datastax] [https://
  img.shields.io/github/license/warmachine028/datastax?color=orange] [https://
         img.shields.io/github/forks/warmachine028/datastax?color=cyan]
-# [dataStax](https://github.com/warmachine028/datastax) ## What's New? - Added
-Mandatory Keyword arguments to avoid confusion in: - Arrays -
-ThreadedBinaryTree - Added High Quality PNGs in README.md ## Table of Contents
+# [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
+Refactored linkedlists -> Lists - Refactored arrays -> Arrays - Refactored
+private_lists -> AbstractLists - Refactored AbstractLists by converting all
+items to AbstractClass to prevent direct initialization. - Module Conventions
+converted to uppercase CamelCase from lowercase snake_case ## Table of Contents
 - [Introduction](#introduction) - [Problem Statement](#problem-statement) -
 [Benefits](#benefits) - [Requirements](#requirements) - [Installation]
 (#installation) - [Usage](#usage) - [What's Next](#whats-next) ## Introduction
-- This is a very simple yet powerful project to implement day to day abstract
-data structures - A pure implementation of Python in representing Tree,
-Linkedlist and Array based datastructures in basic command prompt - It helps
-visualize each data structure for better understanding - Students can be
-beneficial in using this Package - This project is still under construction ##
-Problem Statement - Often at the beginning of B.Tech Course, CS students face a
-lot of problems understanding the internal architecture of complex ADTs. -
-While solving coding challenges locally where test cases have to be written
-using these ADTs, it becomes really cumbersome to write these data structures
-from scratch. - Also, when writing programs which implements these ADS, we
-encounter lots of errors just because we are unable to preview what's actually
-going on under the hood. ## Benefits - Instant installation - Quick Updates -
-Very small size - No extra modules required - Written purely from scratch -
-Easy Documentation [Upcoming] - Command Line Demo ## Requirements - Runs on
-latest Python 3.7+ - (WARNING: Though the module might run on py 3.7 error
-free, but it has been tested for 3.9+) - (Suggesting you to always update to
-the latest python version) - This Library requires no extra modules ##
-Installation 1. Use the python package manager [pip](https://pip.pypa.io/en/
-stable/) to install datastax. ```bash pip install datastax ``` ## Usage ###
-Demo - To get a demo of the library use the following command - **Windows**:
-```bash > py -m datastax ``` - **Unix based systems**: ```bash $ python3 -
-m datastax ``` - _Result_ ```bash Available modules are: 1. LinkedLists 2.
-Trees 3. Arrays Usage > py datastax  [data] Data Structures: -> trees
-Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS ``` -
-Then follow as the instruction guides ```bash > py -m datastax linkedlist 1 2 3
-4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
+- This library offers a simple yet powerful solution for implementing common
+abstract data structures. - With a pure Python implementation, it provides
+representations of tree, linked list, and array-based data structures
+accessible through a basic command prompt interface. - The package includes
+visualization features that enhance the understanding of each data structure. -
+Students can greatly benefit from utilizing this package for their learning and
+educational purposes. - Please note that this project is currently a work in
+progress and undergoing active development. ## Problem Statement - Many CS
+students encounter difficulties in comprehending the intricate internal
+architecture of complex Abstract Data Types (ADTs) during the initial stages of
+their B.Tech course. - When attempting to solve coding challenges that involve
+writing test cases using these ADTs, it becomes excessively burdensome to
+manually create these data structures from scratch. - Furthermore, while
+developing programs that implement these ADTs, numerous errors are encountered
+due to the inability to visualize and understand the underlying processes of
+these data structures. ## Benefits - Swift installation process - Efficient and
+prompt updates - Minimal disk space usage due to its small size - No additional
+modules or dependencies needed - Developed entirely from scratch - Upcoming
+user-friendly documentation - Command line demonstration for easy usage ##
+Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
+to the latest python version) ## Installation 1. Use the python package manager
+[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
+datastax ``` ## Usage ### Demo - To get a demo of the library use the following
+command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
+```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
+LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
+> trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
+``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
+1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
 âââââââ¥âââââ âââââââ¥âââââ
 âââââââ¥âââââ âââââââ¥âââââ â 1
 â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
 âââââââ¨âââââ âââââââ¨âââââ
 âââââââ¨âââââ âââââââ¨âââââ 2.
 Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
@@ -52,24 +57,36 @@
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ ... ``` ### Practical Usage
-- **Queue** ![queue](./assets/Usage/queue.png) ![queue_output](./assets/Usage/
-queue_output.png) --------------------------------------------------- -
-**BinaryTree** ![BinaryTree](./assets/Usage/binaryTree.png) !
-[BinaryTree_output](./assets/Usage/binaryTree_output.png) ---------------------
------------------------------- - **MinHeapTree** ![MinHeapTree](./assets/Usage/
-mht.png) ![MinHeapTree_output](./assets/Usage/mht_output.png) -----------------
----------------------------------- - **ThreadedBinaryTree** !
-[ThreadedBinaryTree](./assets/Usage/tbt.png) ![ThreadedBinaryTree_output](./
-assets/Usage/tbt_output.png) --------------------------------------------------
-- - **SumSegmentTree** ![SumSegmentTree](./assets/Usage/sst.png) !
-[SumSegmentTree_Output](./assets/Usage/sst_output.png) ------------------------
---------------------------- - **HuffmanTree** ![HuffmanTree](./assets/Usage/
-hft.png) ![HuffmanTree_Output](./assets/Usage/hft_output.png) -----------------
----------------------------------- - **RedBlackTree** ![RedBlackTree](./assets/
-Usage/rbt.png) ![RedBlackTreeOutput](./assets/Usage/rbt_output.png) ## What's
-Next - Enhanced Documentation - Better TestCases for Huffman Tree - Better
-TestCases for Segment Trees - Test Cases for Fibonacci Tree
+- **Queue** ![queue](https://github.com/warmachine028/datastax/assets/75939390/
+0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409) ![queue_output](https://github.com/
+warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde) --
+---------------------------------- --------------- - **BinaryTree** !
+[binaryTree](https://github.com/warmachine028/datastax/assets/75939390/
+7228c4b4-def7-4c6b-9e29-e6e244c2c4c1) ![binaryTree_output](https://github.com/
+warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c) --
+------------------------------------------------- - **MinHeapTree** ![mht]
+(https://github.com/warmachine028/datastax/assets/75939390/1c00a207-9ea0-4965-
+898f-29e37883fac5) ![mht_output](https://github.com/warmachine028/datastax/
+assets/75939390/fcfe24d9-6b80-4b16-873c-3f5c3d808d70) -------------------------
+-------------------------- - **ThreadedBinaryTree** ![tbt](https://github.com/
+warmachine028/datastax/assets/75939390/ab2f2572-1474-4d82-9138-b8ee85869114) !
+[tbt_output](https://github.com/warmachine028/datastax/assets/75939390/
+9e77c5dc-082c-471b-90d5-33792673bdf3) -----------------------------------------
+---------- - **SumSegmentTree** ![sst](https://github.com/warmachine028/
+datastax/assets/75939390/7bdcfd6e-37ac-4421-b6d2-acd59cf4976c) ![sst_output]
+(https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-
+88c7-40e4dcc11215) --------------------------------------------------- -
+**HuffmanTree** ![hft](https://github.com/warmachine028/datastax/assets/
+75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e) ![hft_output](https://
+github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
+8dbf91c008a2) --------------------------------------------------- -
+**RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
+75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
+github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
+db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
+Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
+Tree - Refactoring Arrays SubPackage
```

### Comparing `datastax-0.3.1/datastax/__main__.py` & `datastax-0.4.0/datastax/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 import sys
 
-from datastax import linkedlists as ll, trees, arrays
+from datastax import Lists, trees, Arrays
 
 
 def main():
     if len(sys.argv) > 1:
         data_structure = sys.argv[1].lower()
         # take User given data or default
         data = sys.argv[2:] if len(sys.argv) > 2 else [*range(5)]
         if data_structure in ('array', 'arrays'):
-            queue = arrays.Queue(len(data))
-            stack = arrays.Stack(len(data))
-            p_queue = arrays.PriorityQueue(len(data))
+            queue = Arrays.Queue(capacity=len(data))
+            stack = Arrays.Stack(capacity=len(data))
+            p_queue = Arrays.PriorityQueue(capacity=len(data))
             for i in data:
                 stack.push(i)
                 queue.enqueue(i)
                 p_queue.enqueue(i)
             print("Visuals for Arrays:\n\n"
                   f"1. Stack: \n"
                   f"{stack}\n\n"
                   f"2. Queue: \n"
                   f"{queue}\n\n"
                   f"3. Priority Queue: \n"
                   f"{p_queue}\n\n")
         elif data_structure in ('linkedlist', "linkedlists"):
             print("Visuals for LinkedLists:\n\n"
-                  f"1. Singly Linked List: \n"
-                  f"{ll.LinkedList(data)}\n\n"
+                  f"1. Linked List: \n"
+                  f"{Lists.LinkedList(data)}\n\n"
                   f"2. Doubly Linked List: \n"
-                  f"{ll.DoublyLinkedList(data)}\n\n"
+                  f"{Lists.DoublyLinkedList(data)}\n\n"
                   f"3. Circular Linked List: \n"
-                  f"{ll.CircularLinkedList(data)}\n\n"
+                  f"{Lists.CircularLinkedList(data)}\n\n"
                   f"4. Doubly Circular List: \n"
-                  f"{ll.DoublyCircularList(data)}\n\n"
+                  f"{Lists.DoublyCircularList(data)}\n\n"
                   f"5. Queue: \n"
-                  f"{ll.Queue(None, data)}\n\n")
+                  f"{Lists.Queue(None, data)}\n\n"
+                  f"6. LRU Cache: \n"
+                  f"{Lists.LRUCache(capacity=10)}\n\n"
+                  )
         elif data_structure in ('tree', 'trees'):
             print("Visuals for Trees:\n\n"
                   f"1. Binary Tree \n"
                   f"{trees.BinaryTree(data)}\n\n"
                   f"2. Binary Search Tree \n"
                   f"{trees.BinarySearchTree(data)}\n\n"
                   f"3. AVL Tree \n"
                   f"{trees.AVLTree(data)}\n\n")
         else:
             print("This module is not available yet")
     else:
         print("$ py datastax <data-structure> [data]\n"
               "Data Structures: \n"
               "->  trees          Hierarchical DS\n"
-              "->  linkedlists    Linear DS\n"
+              "->  lists          Linear DS\n"
               "->  arrays         Fixed Size Linear DS")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `datastax-0.3.1/datastax/arrays/priority_queue.py` & `datastax-0.4.0/datastax/Arrays/priority_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Priority Queue implementation using Lists (Pseudo Arrays)
 from typing import Any, Callable
 
-from datastax.arrays.queue import Queue
+from datastax.Arrays.queue import Queue
 from datastax.errors import OverFlowError, UnderFlowError
 
 
 class PriorityQueue(Queue):
     def __init__(self, *, capacity: int = None,
                  custom_comparator: Callable = None):
         super().__init__(capacity=capacity)
```

### Comparing `datastax-0.3.1/datastax/arrays/queue.py` & `datastax-0.4.0/datastax/Arrays/queue.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/arrays/stack.py` & `datastax-0.4.0/datastax/Arrays/stack.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/errors.py` & `datastax-0.4.0/datastax/errors.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/linkedlists/circular_linked_list.py` & `datastax-0.4.0/datastax/Lists/DoublyCircularList.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from __future__ import annotations
+from typing import Any, Optional, Self
 
-from typing import Any, Optional
+from datastax.Lists import DoublyLinkedList
+from datastax.Lists.AbstractLists import DoublyCircularList as AbstractList
 
-from datastax.linkedlists.linked_list import LinkedList
-from datastax.linkedlists.private_lists import circular_linked_list
 
+class DoublyCircularList(AbstractList, DoublyLinkedList):
 
-class CircularLinkedList(circular_linked_list.CircularLinkedList,
-                         LinkedList):
-    def _construct(self, array: Optional[list[Any]]) -> CircularLinkedList:
+    def _construct(self, array: Optional[list[Any]]) -> Self:
         if array and array[0] is not None:
             for item in array:
                 self.append(item)
         return self
 
     def append(self, data: Any) -> None:
         super().append(data)
-        self.tail.next = self.head
+        self.head.set_prev(self.tail)
+        self.tail.set_next(self.head)
 
-    def insert(self, data: Any):
+    def insert(self, data: Any) -> None:
         super().insert(data)
-        self.tail.next = self.head
+        self.head.set_prev(self.tail)
+        self.tail.set_next(self.head)
```

### Comparing `datastax-0.3.1/datastax/linkedlists/lru_cache.py` & `datastax-0.4.0/datastax/Lists/LRUCache.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 The functions get and put must each run in O(1) average time complexity.
 
 LRU -> Least Recently used
 """
 from typing import Any
 
-from datastax.linkedlists import DoublyLinkedList, DoublyNode
+from datastax.Lists import DoublyLinkedList, DoublyNode
 
 
 class LRUCache(DoublyLinkedList):
     def __init__(self, capacity: int):
         super().__init__()
         self._capacity = capacity
         self._cache: dict[int, DoublyNode] = {}
         self._head = DoublyNode('HEAD')
         self._tail = DoublyNode('TAIL')
-        self.tail.prev = self.head
-        self.head.next = self.tail
+        self.tail.set_prev(self.head)
+        self.head.set_next(self.tail)
 
     def get(self, key: int) -> int:
         if key not in self._cache:
             return -1
         node = self._cache[key]
         self._enqueue(node)
         return node.data[1]
@@ -41,27 +41,27 @@
         else:
             node = self._cache[key]
             node.data[1] = value
         self._enqueue(node)
 
     def _enqueue(self, node: DoublyNode) -> None:
         if node.prev:
-            node.prev.next = node.next
+            node.prev.set_next(node.next)
         if node.next:
-            node.next.prev = node.prev
-        node.prev = self.tail.prev
-        node.next = self.tail
-        self.tail.prev.next = node
-        self.tail.prev = node
+            node.next.set_prev(node.prev)
+        node.set_prev(self.tail.prev)
+        node.set_next(self.tail)
+        self.tail.prev.set_next(node)
+        self.tail.set_prev(node)
         self._cache[node.data[0]] = node
 
     def _dequeue(self) -> None:
         node = self.head.next
-        self.head.next = node.next
-        node.next.prev = node.prev
+        self.head.set_next(node.next)
+        node.next.set_prev(node.prev)
         self._cache.pop(node.data[0])
 
     def append(self, data) -> None:
         raise NotImplementedError
 
     def insert(self, data: Any):
         return NotImplementedError
```

### Comparing `datastax-0.3.1/datastax/linkedlists/private_lists/circular_linked_list.py` & `datastax-0.4.0/datastax/Lists/AbstractLists/LinkedList.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,71 @@
-from __future__ import annotations
+from typing import Any, Optional, Self
+from datastax.Lists.AbstractLists.Node import Node
+from datastax.Lists.Utils import Commons
+from abc import abstractmethod, ABC as AbstractClass
 
-from typing import Any, Optional
 
-from datastax.linkedlists.private_lists.linked_list import (
-    Node,
-    LinkedList,
-    _mangled
-)
+class LinkedList(AbstractClass):
+    _head: Optional[Node] = None
+    _tail: Optional[Node] = None
 
-
-class CircularLinkedList(LinkedList):
-    def _construct(self, array: Optional[list[Any]]) -> CircularLinkedList:
-        raise NotImplementedError
-
-    @staticmethod
-    def _max_width(node: Optional[Node]):
+    def _max_width(self, node: Optional[Node]):
         max_width = 0
-        ref = node
-        while ref:
-            max_width = max(max_width, len(_mangled(ref.data)))
-            ref = ref.next
-            if ref is node:
-                break
+        while node:
+            max_width = max(max_width, len(Commons.repr(node.data)))
+            node = node.next
         return max_width
 
+    @property
+    def head(self):
+        return self._head
+
+    @property
+    def tail(self):
+        return self._tail
+
     def __str__(self):
-        if not self.head:
-            return 'NULL'
-        start_padding = 6
-        top = ' ' * start_padding
-        mid = ' ╭─-->'
-        dow = ' │    '
-        ref = self.head
+        start_padding = 1
+        top = mid = dow = " " * start_padding
+        ref = self._head
         max_width = self._max_width(ref) + 4
         nodes = 0
         while ref:
             top += f"┌{'─' * max_width}╥────┐   "
-            mid += (
-                f"│{f'{_mangled(ref.data)}'.center(max_width)}║  "
-                f"{('-' if ref.next != self.head else '─') * 5}>"
-            )
+            mid += f"│{f'{Commons.repr(ref.data)}'.center(max_width)}║  ----->"
             dow += f"└{'─' * max_width}╨────┘   "
             ref = ref.next
             nodes += 1
-            if ref is self.head:
-                break
 
         length_per_node = max_width + 7
         heading = self._draw_heading(nodes, length_per_node, start_padding)
-        top += '\n'
-        mid = f"{mid[:-1]}╮\n"
-        dow = f'{dow[:-1]}│\n'
-        footing = self._draw_footing(nodes, length_per_node, start_padding)
-        return heading + top + mid + dow + footing
+        top += "\n"
+        mid += f"{' ' if mid[-1] == '>' else ''}NULL\n"
+        dow += "\n"
+
+        return heading + top + mid + dow
 
-    @staticmethod
-    def _draw_footing(n: int, lpn: int, start_padding: int) -> str:
+    def _draw_heading(self, n: int, lpn: int, start_padding: int) -> str:
         if n == 0:
-            return ' '
-        spaces = '─' * 3
+            return " "
+        head, tail = "HEAD".center(lpn), "TAIL".center(lpn)
+        spaces = " " * 3
+        if self._head is self._tail:
+            return f"{' ' * start_padding}{head}\n" \
+                   f"{' ' * start_padding}{tail}\n"
         return (
-            f" ╰{'─' * (start_padding - 2)}{'─' * lpn * n}"
-            f"{spaces * (n - 1)}──╯\n"
+            f"{' ' * start_padding}"
+            f"{head}{' ' * lpn * (n - 2)}"
+            f"{spaces * (n - 1)}{tail}\n"
         )
 
-    def __iter__(self):
-        ref = self.head
-        while ref:
-            yield ref.data
-            ref = ref.next
-            if ref is self.head:
-                break
+    @abstractmethod
+    def append(self, data: Any) -> None:
+        ...
+
+    @abstractmethod
+    def insert(self, data: Any) -> None:
+        ...
+
+    @abstractmethod
+    def _construct(self, array: Optional[list[Any]]) -> Self:
+        ...
```

### Comparing `datastax-0.3.1/datastax/linkedlists/private_lists/doubly_circular_llist.py` & `datastax-0.4.0/datastax/Lists/AbstractLists/DoublyCircularList.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-from __future__ import annotations
+from abc import ABC
 
-from typing import Any, Optional
+from datastax.Lists.AbstractLists.CircularLinkedList import CircularLinkedList
+from datastax.Lists.AbstractLists.DoublyLinkedList import DoublyLinkedList
+from datastax.Lists.Utils import Commons
 
-from datastax.linkedlists.private_lists.circular_linked_list import (
-    CircularLinkedList
-)
-from datastax.linkedlists.private_lists.doubly_linked_list import (
-    DoublyLinkedList,
-    _mangled
-)
 
-
-class DoublyCircularList(DoublyLinkedList, CircularLinkedList):
-    def _construct(self, array: Optional[list[Any]]) -> DoublyCircularList:
-        raise NotImplementedError
+class DoublyCircularList(DoublyLinkedList, CircularLinkedList, ABC):
 
     def __str__(self):
         if not self.head:
             return 'NULL'
         start_padding = 6
         top = '    '
         mid = ' ╭─'
@@ -25,15 +17,15 @@
         ref = self.head
         max_width = self._max_width(ref) + 4
         nodes = 0
         while ref:
             top += f" ┌────╥{'─' * max_width}╥────┐  "
             mid += (
                 f"---->  ║"
-                f"{f'{_mangled(ref.data)}'.center(max_width)}"
+                f"{f'{Commons.repr(ref.data)}'.center(max_width)}"
                 f"║  <---"
             )
             dow += f" └────╨{'─' * max_width}╨────┘  "
             ref = ref.next
             nodes += 1
             if ref is self.head:
                 break
```

### Comparing `datastax-0.3.1/datastax/linkedlists/queue.py` & `datastax-0.4.0/datastax/Lists/Queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,67 @@
-# Queue implementation using LinkedLists
-from __future__ import annotations
+# Queue implementation using LinkedList
 
 from sys import maxsize
-from typing import Any, Optional
-
+from typing import Any
+from datastax.Lists import Node
 from datastax.errors import OverFlowError, UnderFlowError
-from datastax.linkedlists.linked_list import LinkedList, Node
+from datastax.Lists import LinkedList
+from datastax.Lists.AbstractLists import Queue as AbstractQueue
 
 
-class Queue(LinkedList):
-    def __init__(self, capacity: int = None, array: list[Any] = None):
+class Queue(AbstractQueue, LinkedList):
+    def __init__(self, capacity: int = None, items: list[Any] = None):
         super().__init__()
         self._rear = 0
-        if capacity is not None and capacity < 0:
-            print("Capacity can't be negative"
-                  "Setting unbounded capacity")
-        self._capacity = maxsize
-        if capacity is not None and capacity > 0:
-            self._capacity = capacity
-        if array and array[0] is not None:
-            for item in array[:self._capacity]:
+        self.set_capacity(capacity)
+        if items:
+            for item in items[:self.capacity]:
                 self.enqueue(item)
 
     def is_empty(self) -> bool:
         return self.head is None
 
     def is_full(self) -> bool:
-        return self._rear == self._capacity
+        return self._rear == self.capacity
+
+    def set_capacity(self, capacity: int):
+        if capacity is None:
+            self._capacity = maxsize
+            return
+        if not isinstance(capacity, int):
+            raise TypeError("The 'capacity' parameter must be an "
+                            "instance of int or its subclass.")
+        if capacity < 0:
+            raise ValueError("Capacity can't be negative")
+        self._capacity = capacity
 
     def enqueue(self, data: Any) -> int:
         if self.is_full():
             raise OverFlowError(self)
-        super().append(data)
+        node = Node(data)
+        if not self.head:
+            self.set_head(node)
+        else:
+            self.tail.set_next(node)
+        self.set_tail(node)
         self._rear += 1
         return 0
 
     def dequeue(self) -> Any:
         if self.is_empty():
             raise UnderFlowError(self)
         deleted_node = self.head
         deleted_item = deleted_node.data
-        self._head = self.head.next
+        self.set_head(self.head.next)
         self._rear -= 1
         return deleted_item
 
     def peek(self) -> str:
         if self.is_empty():
             return "QUEUE EMPTY"
         return str(self._tail.data if self._tail else None)
 
     def append(self, data: Any) -> None:
         raise NotImplementedError
 
     def insert(self, data: Any) -> None:
         raise NotImplementedError
-
-    def __str__(self, head: Node = None):
-        def maximum_breadth(ref: Optional[Node]) -> int:
-            result = 0
-            while ref:
-                result = max(len(str(ref.data)), result)
-                ref = ref.next
-            return result
-
-        if self.is_empty():
-            return '╔═══════════════════╗\n' \
-                   '║    QUEUE EMPTY    ║\n' \
-                   '╚═══════════════════╝'
-        padding = 4
-        max_breadth = maximum_breadth(self.head) + padding
-        middle_part = 'FRONT -> '
-        upper_part = f"{' ' * (len(middle_part) - 1)} "
-        lower_part = f"{' ' * (len(middle_part) - 1)} "
-        temp = self.head
-        while temp:
-            item = temp.data
-            upper_part += f"┌{'─' * max_breadth}┐   "
-            middle_part += f'|{str(item).center(max_breadth)}│ <-'
-            lower_part += f"└{'─' * max_breadth}┘   "
-            temp = temp.next
-        upper_part = f"{upper_part[:-1]}\n"
-        middle_part += ' REAR\n'
-        lower_part = f"{lower_part[:-1]}\n"
-
-        return upper_part + middle_part + lower_part
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `datastax-0.3.1/datastax/trees/__init__.py` & `datastax-0.4.0/datastax/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/avl_tree.py` & `datastax-0.4.0/datastax/trees/avl_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/binary_search_tree.py` & `datastax-0.4.0/datastax/trees/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/binary_tree.py` & `datastax-0.4.0/datastax/trees/binary_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datastax.errors import (
     PathNotGivenError,
     PathNotFoundError,
     PathAlreadyOccupiedWarning,
     NodeNotFoundWarning,
     DeletionFromEmptyTreeWarning,
 )
-from datastax.linkedlists import Queue
+from datastax.Lists import Queue
 from datastax.trees.private_trees import binary_tree
 from datastax.trees.private_trees.binary_tree import TreeNode
 
 
 class BinaryTree(binary_tree.BinaryTree):
     def insert_path(self, data: Any, path: list[str] = None) -> None:
         node = TreeNode(data)
@@ -43,15 +43,15 @@
                           PathAlreadyOccupiedWarning)
 
     # Helper function to construct tree by level order -> Array to tree
     def _construct(self, array: list[Any] = None) -> Optional[BinaryTree]:
         if not array or array[0] is None:
             return None
 
-        queue = Queue(len(array))
+        queue = Queue(capacity=len(array))
         current = 0
         root = self.root
         if not root:
             root = TreeNode(array[0])
             current = 1
         queue.enqueue(root)
         while not queue.is_empty() and current < len(array):
@@ -76,15 +76,15 @@
         Deletes a node which has the data and replaces with RightMost Leaf Node
         :param data: An item corresponding to the node to be deleted
         :return: returns data if node is found else None and raises warning
         """
         if not self.root or data is None:
             return self.delete_deepest()
 
-        queue = Queue(len(self.array_repr))
+        queue = Queue(capacity=len(self.array_repr))
         queue.enqueue(self.root)
         del_node = None
         while not queue.is_empty():
             node = queue.dequeue()
             if node.data == data:
                 del_node = node
                 break
@@ -106,15 +106,15 @@
         return del_data
 
     def delete_deepest(self) -> Optional[Any]:
         """
         Deletes the rightmost leaf node
         :return: data if tree is not empty else None
         """
-        queue = Queue(len(self.array_repr))
+        queue = Queue(capacity=len(self.array_repr))
         if self.root:
             queue.enqueue(self.root)
         parent = None
         while not queue.is_empty():
             node = queue.dequeue()
             if node.left:
                 queue.enqueue(node.left)
@@ -140,16 +140,17 @@
             warnings.warn(
                 "Deletion Unsuccessful. Can't delete from empty Tree",
                 DeletionFromEmptyTreeWarning
             )
         return data
 
     def insert(self, item: Any):
+
         temp = None if item is None else TreeNode(item)
-        queue = Queue(len(self.array_repr))
+        queue = Queue(capacity=len(self.array_repr))
         if self.root:
             queue.enqueue(self.root)
         while not queue.is_empty():
             node = queue.dequeue()
             if node.left:
                 queue.enqueue(node.left)
             else:
```

### Comparing `datastax-0.3.1/datastax/trees/expression_tree.py` & `datastax-0.4.0/datastax/trees/expression_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Expression Tree Implementation
 from __future__ import annotations
 
 from typing import Optional, Union, Any
 
-from datastax.arrays import Stack
+from datastax.Arrays import Stack
 from datastax.errors import (
     UnmatchedBracketPairError, InvalidExpressionError,
     UnderFlowError, OverFlowError
 )
 from datastax.trees.private_trees.binary_tree import TreeNode, BinaryTree
```

### Comparing `datastax-0.3.1/datastax/trees/fibonacci_tree.py` & `datastax-0.4.0/datastax/trees/fibonacci_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/heap_tree.py` & `datastax-0.4.0/datastax/trees/heap_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/huffman_tree.py` & `datastax-0.4.0/datastax/trees/huffman_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Implementation of Variable size Huffman Coding Tree
 from __future__ import annotations
 
 from collections import Counter
 from typing import Any, Optional, Union
 
-from datastax.arrays import PriorityQueue
+from datastax.Arrays import PriorityQueue
 from datastax.trees.private_trees import huffman_tree
 from datastax.trees.private_trees.huffman_tree import HuffmanNode
 
 
 class HuffmanTable(huffman_tree.HuffmanTable):
     def _calculate_size(self):
         size = 0
@@ -79,15 +79,15 @@
         self._huffman_code = ''.join(
             self.huffman_code_of(character) for character in self._data
         )
         pass
 
     def size_calculator(self) -> Optional[tuple[int, int]]:
         """
-        Calculates the actual encoding size and total 
+        Calculates the actual encoding size and total
         huffman encoding size with table included
         """
         if not self.root or not self.huffman_table:
             return None
         fixed_encoding = huffman_encoding = 0
         frequency = self.huffman_table.frequency
```

### Comparing `datastax-0.3.1/datastax/trees/min_heap_tree.py` & `datastax-0.4.0/datastax/trees/min_heap_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/min_segment_tree.py` & `datastax-0.4.0/datastax/trees/min_segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/private_trees/binary_tree.py` & `datastax-0.4.0/datastax/trees/private_trees/binary_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Private module to separate print logic from main logic of BinaryTree
 from __future__ import annotations
 
 import math
 from typing import Any, Optional
 
-from datastax.linkedlists import Queue
+from datastax.Lists import Queue
 
 
 def _node_builder(data: Optional[str], piece_width: int) -> str:
     value: str = data or ''
     gap1 = int(math.ceil(piece_width / 2 - len(value) / 2))
     gap2 = int(math.floor(piece_width / 2 - len(value) / 2))
     return f"{' ' * gap1}{value}{' ' * gap2}"
```

### Comparing `datastax-0.3.1/datastax/trees/private_trees/huffman_tree.py` & `datastax-0.4.0/datastax/trees/private_trees/huffman_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/private_trees/red_black_tree.py` & `datastax-0.4.0/datastax/trees/private_trees/red_black_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/private_trees/segment_tree.py` & `datastax-0.4.0/datastax/trees/private_trees/segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/private_trees/threaded_binary_tree.py` & `datastax-0.4.0/datastax/trees/private_trees/threaded_binary_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Private module to separate print logic from insertion logic
 from __future__ import annotations
 
 from itertools import chain
 from typing import Optional, Any
 
-from datastax.linkedlists import Queue
+from datastax.Lists import Queue
 from datastax.trees import (
     BinaryTree,
     AVLTree,
     HeapTree,
     MinHeapTree
 )
 from datastax.trees.private_trees import binary_tree
```

### Comparing `datastax-0.3.1/datastax/trees/red_black_tree.py` & `datastax-0.4.0/datastax/trees/red_black_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/splay_tree.py` & `datastax-0.4.0/datastax/trees/splay_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/sum_segment_tree.py` & `datastax-0.4.0/datastax/trees/sum_segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/datastax/trees/threaded_binary_tree.py` & `datastax-0.4.0/datastax/trees/threaded_binary_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.3.1/setup.py` & `datastax-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 
 try:  # https://stackoverflow.com/questions/30700166/python-open-file-error
     with codecs.open("README.md", 'r', errors='ignore', encoding='utf8') as f:
         readme_contents = f.read()
 
 except Exception as error:
     readme_contents = (
-        'This library which supports ADTs like Linkedlists and Trees and its '
+        'This library which supports ADTs like LinkedLists and Trees and its '
         'types. This instant library is solely written from scratch and '
         'requires no additional libraries to be installed. It solves the '
         'purpose of writing programs for complex data structures from scratch,'
         ' visualizing ADTs and simplify  writing its inner architectures. This'
         ' Module Supports the following dataStructures:\n'
         '1. Arrays:\n'
         '   a. Queue\n'
         '   b. Stack\n\n'
         '   c. Priority Queue\n\n'
-        '2. LinkedLists:\n'
+        '2. Lists:\n'
         '   a. Singly Linked List\n'
         '   b. Doubly Linked List\n'
         '   c. Circular Linked List\n'
         '   d. Doubly Circular List\n'
         '   e. Queue\n\n'
+        '   f. LRU Cache\n\n'
         '3. Trees:\n'
         '   a. Binary Tree\n'
         '   b. Binary Search Tree\n'
         '   c. AVL Tree\n'
         '   d. Heap Tree\n'
         '   e. Min Heap Tree\n'
         '   f. Expression Tree\n'
@@ -42,64 +43,65 @@
         '   h. Red Black Tree\n'
         '   i. Fibonacci Tree\n'
         '   j. Splay Tree\n\n'
     )
     sys.stderr.write(f"Warning: Could not open README.md due {error}\n")
 
 setup(
-        name='datastax',
-        maintainer="Pritam K",
-        description='A python library to handle dataStructures',
-        long_description=readme_contents,
-        long_description_content_type='text/markdown',
-        url='https://github.com/warmachine028/datastax',
-        author='Pritam K',
-        download_url="https://pypi.python.org/pypi/datastax",
-        project_urls={
-            'Bug Tracker': 'https://github.com/warmachine028/datastax/issues',
-            'Documentation': 'https://github.com/warmachine028/'
-                             'datastax#readme',
-            'Source Code': 'https://github.com/warmachine028/datastax',
-        },
-        license='MIT',
-        classifiers=[
-            "Development Status :: 4 - Beta",
-
-            "Intended Audience :: Education",
-            "Intended Audience :: Developers",
-            "Intended Audience :: End Users/Desktop",
-            "Intended Audience :: Science/Research",
-
-            "License :: OSI Approved :: MIT License",
-
-            "Operating System :: OS Independent",
-
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3.10",
-            "Programming Language :: Python :: 3.11",
-
-            "Topic :: Documentation",
-            "Topic :: Education :: Testing",
-            "Topic :: Scientific/Engineering :: Visualization",
-            "Topic :: Software Development :: Documentation",
-            "Topic :: Software Development :: Libraries :: Python Modules",
-            "Topic :: Software Development :: Testing :: Unit",
-
-            "Typing :: Typed"
-        ],
-        platforms=["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
-        test_suite='pytest',
-        version=datastax.__version__,
-        python_requires='>=3.7',
-        zip_safe=False,
-        packages=[
-            'datastax',
-            'datastax/arrays',
-            'datastax/linkedlists',
-            'datastax/trees',
-            'datastax/linkedlists/private_lists',
-            'datastax/trees/private_trees',
-        ],
-        author_email='pritamkundu771@gmail.com'
+    name='datastax',
+    maintainer="Pritam Kundu",
+    description='A python library to handle dataStructures',
+    long_description=readme_contents,
+    long_description_content_type='text/markdown',
+    url='https://github.com/warmachine028/datastax',
+    author='Pritam K',
+    download_url="https://pypi.python.org/pypi/datastax",
+    project_urls={
+        'Bug Tracker': 'https://github.com/warmachine028/datastax/issues',
+        'Documentation':
+            'https://github.com/warmachine028/datastax#readme',
+        'Source Code': 'https://github.com/warmachine028/datastax',
+    },
+    license='MIT',
+    classifiers=[
+        "Development Status :: 4 - Beta",
+
+        "Intended Audience :: Education",
+        "Intended Audience :: Developers",
+        "Intended Audience :: End Users/Desktop",
+        "Intended Audience :: Science/Research",
+
+        "License :: OSI Approved :: MIT License",
+
+        "Operating System :: OS Independent",
+
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+
+        "Topic :: Documentation",
+        "Topic :: Education :: Testing",
+        "Topic :: Scientific/Engineering :: Visualization",
+        "Topic :: Software Development :: Documentation",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Testing :: Unit",
+
+        "Typing :: Typed"
+    ],
+    platforms=["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
+    test_suite='pytest',
+    version=datastax.__version__,
+    python_requires='>=3.11',
+    zip_safe=False,
+    packages=[
+        'datastax',
+        'datastax/Arrays',
+        'datastax/Lists',
+        'datastax/Lists/Utils',
+        'datastax/Lists/AbstractLists',
+        'datastax/trees',
+        'datastax/trees/private_trees',
+    ],
+    author_email='pritamkundu771@gmail.com'
 )
```

