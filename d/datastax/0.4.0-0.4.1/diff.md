# Comparing `tmp/datastax-0.4.0.tar.gz` & `tmp/datastax-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastax-0.4.0.tar", last modified: Wed Jul 12 03:19:41 2023, max compression
+gzip compressed data, was "datastax-0.4.1.tar", last modified: Wed Jul 12 09:39:13 2023, max compression
```

## Comparing `datastax-0.4.0.tar` & `datastax-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 03:19:31.000000 datastax-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-12 03:19:41.368094 datastax-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-12 03:19:31.000000 datastax-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax/Arrays/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/priority_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Arrays/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/AbstractLists/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/CircularLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyCircularList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/DoublyNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/AbstractLists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/CircularLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyCircularList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/DoublyNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/LRUCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.364093 datastax-0.4.0/datastax/Lists/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Utils/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/Lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/datastax/trees/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/avl_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/expression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/fibonacci_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/min_heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/min_segment_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.368094 datastax-0.4.0/datastax/trees/private_trees/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/private_trees/threaded_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/splay_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/sum_segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 03:19:31.000000 datastax-0.4.0/datastax/trees/threaded_binary_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:19:41.360093 datastax-0.4.0/datastax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 03:19:41.000000 datastax-0.4.0/datastax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:19:41.368094 datastax-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-12 03:19:31.000000 datastax-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.885777 datastax-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 09:39:04.000000 datastax-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-12 09:39:13.885777 datastax-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-12 09:39:04.000000 datastax-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax/Arrays/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Arrays/AbstractArrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/PriorityQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Lists/AbstractLists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/LRUCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Utils/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/avl_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/expression_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/fibonacci_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/heap_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/huffman_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/min_heap_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/min_segment_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.885777 datastax-0.4.1/datastax/trees/private_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/huffman_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/red_black_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/segment_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/threaded_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/red_black_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/splay_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/sum_segment_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/threaded_binary_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:39:13.885777 datastax-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-12 09:39:04.000000 datastax-0.4.1/setup.py
```

### Comparing `datastax-0.4.0/LICENSE` & `datastax-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/PKG-INFO` & `datastax-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datastax
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python library to handle dataStructures
 Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax
 Author: Pritam K
 Author-email: pritamkundu771@gmail.com
 Maintainer: Pritam Kundu
 License: MIT
@@ -35,15 +35,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-    updated: Sunday, 11th July 2023
+    updated: Wednesday, 12th July 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -68,19 +68,18 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored linkedlists -> Lists
-- Refactored arrays -> Arrays
-- Refactored private_lists -> AbstractLists
-- Refactored AbstractLists by converting all items to AbstractClass to prevent direct initialization.
-- Module Conventions converted to uppercase CamelCase from lowercase snake_case
+- Refactored Array Contents
+- Added AbstractArray SubModule to abstract print logic
+- Added more test cases for Queues
+- Type Checked Arrays and Lists with mypy
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
@@ -239,8 +238,7 @@
 
 ## What's Next
 
 - Enhanced Documentation
 - Better TestCases for Huffman Tree
 - Better TestCases for Segment Trees
 - Test Cases for Fibonacci Tree
-- Refactoring Arrays SubPackage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datastax Version: 0.4.0 Summary: A python library
+Metadata-Version: 2.1 Name: datastax Version: 0.4.1 Summary: A python library
 to handle dataStructures Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax Author: Pritam K Author-
 email: pritamkundu771@gmail.com Maintainer: Pritam Kundu License: MIT Project-
 URL: Bug Tracker, https://github.com/warmachine028/datastax/issues Project-URL:
 Documentation, https://github.com/warmachine028/datastax#readme Project-URL:
 Source Code, https://github.com/warmachine028/datastax Platform: Windows
 Platform: Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier:
@@ -15,68 +15,66 @@
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Documentation
 Classifier: Topic :: Education :: Testing Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Software Development ::
 Documentation Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed Requires-Python: >=3.11 Description-Content-Type:
-text/markdown License-File: LICENSE updated: Sunday, 11th July 2023
+text/markdown License-File: LICENSE updated: Wednesday, 12th July 2023
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
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored linkedlists -> Lists - Refactored arrays -> Arrays - Refactored
-private_lists -> AbstractLists - Refactored AbstractLists by converting all
-items to AbstractClass to prevent direct initialization. - Module Conventions
-converted to uppercase CamelCase from lowercase snake_case ## Table of Contents
-- [Introduction](#introduction) - [Problem Statement](#problem-statement) -
-[Benefits](#benefits) - [Requirements](#requirements) - [Installation]
-(#installation) - [Usage](#usage) - [What's Next](#whats-next) ## Introduction
-- This library offers a simple yet powerful solution for implementing common
-abstract data structures. - With a pure Python implementation, it provides
-representations of tree, linked list, and array-based data structures
-accessible through a basic command prompt interface. - The package includes
-visualization features that enhance the understanding of each data structure. -
-Students can greatly benefit from utilizing this package for their learning and
-educational purposes. - Please note that this project is currently a work in
-progress and undergoing active development. ## Problem Statement - Many CS
-students encounter difficulties in comprehending the intricate internal
-architecture of complex Abstract Data Types (ADTs) during the initial stages of
-their B.Tech course. - When attempting to solve coding challenges that involve
-writing test cases using these ADTs, it becomes excessively burdensome to
-manually create these data structures from scratch. - Furthermore, while
-developing programs that implement these ADTs, numerous errors are encountered
-due to the inability to visualize and understand the underlying processes of
-these data structures. ## Benefits - Swift installation process - Efficient and
-prompt updates - Minimal disk space usage due to its small size - No additional
-modules or dependencies needed - Developed entirely from scratch - Upcoming
-user-friendly documentation - Command line demonstration for easy usage ##
-Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
-to the latest python version) ## Installation 1. Use the python package manager
-[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
-datastax ``` ## Usage ### Demo - To get a demo of the library use the following
-command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
-```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
-LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
-> trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
-``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
-1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
+Refactored Array Contents - Added AbstractArray SubModule to abstract print
+logic - Added more test cases for Queues - Type Checked Arrays and Lists with
+mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
+(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
+[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
+Introduction - This library offers a simple yet powerful solution for
+implementing common abstract data structures. - With a pure Python
+implementation, it provides representations of tree, linked list, and array-
+based data structures accessible through a basic command prompt interface. -
+The package includes visualization features that enhance the understanding of
+each data structure. - Students can greatly benefit from utilizing this package
+for their learning and educational purposes. - Please note that this project is
+currently a work in progress and undergoing active development. ## Problem
+Statement - Many CS students encounter difficulties in comprehending the
+intricate internal architecture of complex Abstract Data Types (ADTs) during
+the initial stages of their B.Tech course. - When attempting to solve coding
+challenges that involve writing test cases using these ADTs, it becomes
+excessively burdensome to manually create these data structures from scratch. -
+Furthermore, while developing programs that implement these ADTs, numerous
+errors are encountered due to the inability to visualize and understand the
+underlying processes of these data structures. ## Benefits - Swift installation
+process - Efficient and prompt updates - Minimal disk space usage due to its
+small size - No additional modules or dependencies needed - Developed entirely
+from scratch - Upcoming user-friendly documentation - Command line
+demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
+(Suggesting you to always update to the latest python version) ## Installation
+1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
+install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
+demo of the library use the following command - **Windows**: ```bash > py -
+m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
+_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
+> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
+Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
+guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
+Singly Linked List: HEAD TAIL âââââââ¥âââââ
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ âââââââ¥âââââ â 1
-â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
+âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
+----->â 4 â -----> NULL âââââââ¨âââââ
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ âââââââ¨âââââ 2.
-Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
@@ -106,8 +104,8 @@
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
 db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
 Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree - Refactoring Arrays SubPackage
+Tree
```

### Comparing `datastax-0.4.0/README.md` & `datastax-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-    updated: Sunday, 11th July 2023
+    updated: Wednesday, 12th July 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -27,19 +27,18 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored linkedlists -> Lists
-- Refactored arrays -> Arrays
-- Refactored private_lists -> AbstractLists
-- Refactored AbstractLists by converting all items to AbstractClass to prevent direct initialization.
-- Module Conventions converted to uppercase CamelCase from lowercase snake_case
+- Refactored Array Contents
+- Added AbstractArray SubModule to abstract print logic
+- Added more test cases for Queues
+- Type Checked Arrays and Lists with mypy
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
@@ -198,8 +197,7 @@
 
 ## What's Next
 
 - Enhanced Documentation
 - Better TestCases for Huffman Tree
 - Better TestCases for Segment Trees
 - Test Cases for Fibonacci Tree
-- Refactoring Arrays SubPackage
```

#### html2text {}

```diff
@@ -1,61 +1,59 @@
- updated: Sunday, 11th July 2023
+ updated: Wednesday, 12th July 2023
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
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored linkedlists -> Lists - Refactored arrays -> Arrays - Refactored
-private_lists -> AbstractLists - Refactored AbstractLists by converting all
-items to AbstractClass to prevent direct initialization. - Module Conventions
-converted to uppercase CamelCase from lowercase snake_case ## Table of Contents
-- [Introduction](#introduction) - [Problem Statement](#problem-statement) -
-[Benefits](#benefits) - [Requirements](#requirements) - [Installation]
-(#installation) - [Usage](#usage) - [What's Next](#whats-next) ## Introduction
-- This library offers a simple yet powerful solution for implementing common
-abstract data structures. - With a pure Python implementation, it provides
-representations of tree, linked list, and array-based data structures
-accessible through a basic command prompt interface. - The package includes
-visualization features that enhance the understanding of each data structure. -
-Students can greatly benefit from utilizing this package for their learning and
-educational purposes. - Please note that this project is currently a work in
-progress and undergoing active development. ## Problem Statement - Many CS
-students encounter difficulties in comprehending the intricate internal
-architecture of complex Abstract Data Types (ADTs) during the initial stages of
-their B.Tech course. - When attempting to solve coding challenges that involve
-writing test cases using these ADTs, it becomes excessively burdensome to
-manually create these data structures from scratch. - Furthermore, while
-developing programs that implement these ADTs, numerous errors are encountered
-due to the inability to visualize and understand the underlying processes of
-these data structures. ## Benefits - Swift installation process - Efficient and
-prompt updates - Minimal disk space usage due to its small size - No additional
-modules or dependencies needed - Developed entirely from scratch - Upcoming
-user-friendly documentation - Command line demonstration for easy usage ##
-Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
-to the latest python version) ## Installation 1. Use the python package manager
-[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
-datastax ``` ## Usage ### Demo - To get a demo of the library use the following
-command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
-```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
-LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
-> trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
-``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
-1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
+Refactored Array Contents - Added AbstractArray SubModule to abstract print
+logic - Added more test cases for Queues - Type Checked Arrays and Lists with
+mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
+(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
+[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
+Introduction - This library offers a simple yet powerful solution for
+implementing common abstract data structures. - With a pure Python
+implementation, it provides representations of tree, linked list, and array-
+based data structures accessible through a basic command prompt interface. -
+The package includes visualization features that enhance the understanding of
+each data structure. - Students can greatly benefit from utilizing this package
+for their learning and educational purposes. - Please note that this project is
+currently a work in progress and undergoing active development. ## Problem
+Statement - Many CS students encounter difficulties in comprehending the
+intricate internal architecture of complex Abstract Data Types (ADTs) during
+the initial stages of their B.Tech course. - When attempting to solve coding
+challenges that involve writing test cases using these ADTs, it becomes
+excessively burdensome to manually create these data structures from scratch. -
+Furthermore, while developing programs that implement these ADTs, numerous
+errors are encountered due to the inability to visualize and understand the
+underlying processes of these data structures. ## Benefits - Swift installation
+process - Efficient and prompt updates - Minimal disk space usage due to its
+small size - No additional modules or dependencies needed - Developed entirely
+from scratch - Upcoming user-friendly documentation - Command line
+demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
+(Suggesting you to always update to the latest python version) ## Installation
+1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
+install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
+demo of the library use the following command - **Windows**: ```bash > py -
+m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
+_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
+> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
+Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
+guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
+Singly Linked List: HEAD TAIL âââââââ¥âââââ
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ âââââââ¥âââââ â 1
-â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
+âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
+----->â 4 â -----> NULL âââââââ¨âââââ
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ âââââââ¨âââââ 2.
-Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
@@ -85,8 +83,8 @@
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
 db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
 Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree - Refactoring Arrays SubPackage
+Tree
```

### Comparing `datastax-0.4.0/datastax/Arrays/priority_queue.py` & `datastax-0.4.1/datastax/Arrays/PriorityQueue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Priority Queue implementation using Lists (Pseudo Arrays)
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 
-from datastax.Arrays.queue import Queue
+from datastax.Arrays.Queue import Queue
 from datastax.errors import OverFlowError, UnderFlowError
 
 
 class PriorityQueue(Queue):
-    def __init__(self, *, capacity: int = None,
-                 custom_comparator: Callable = None):
+    comparator: Callable
+
+    def __init__(self, *, capacity: Optional[int] = None,
+                 custom_comparator: Optional[Callable] = None):
         super().__init__(capacity=capacity)
         self.comparator = custom_comparator or max
 
     def swap(self, index1: int, index2: int) -> None:
         array = self._array
         array[index1], array[index2] = array[index2], array[index1]
```

### Comparing `datastax-0.4.0/datastax/Arrays/queue.py` & `datastax-0.4.1/datastax/Arrays/AbstractArrays/Queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,81 @@
-# Queue Implementation using Lists (Pseudo Arrays)
-import math
-from typing import Any, Union
-
-from datastax.errors import OverFlowError, UnderFlowError
+from abc import ABC as AbstractClass, abstractmethod
+from typing import Any
+from datastax.Utils import Commons
+from datastax.Arrays.AbstractArrays.Array import Array
 
 
-class Queue:
-    def __init__(self, *, capacity: int = None):
-        self._capacity = capacity if capacity is not None else math.inf
-        self._array: list[Any] = []
-        self._front = self._rear = 0
+class Queue(Array, AbstractClass):
+    _rear = 0
+    _front = 0
 
-    @property
-    def array(self) -> list[Any]:
-        return self._array[self._front:self._rear]
+    def append(self, data: Any) -> None:
+        raise NotImplementedError
+
+    def insert(self, data: Any) -> None:
+        raise NotImplementedError
+
+    def pop(self) -> Any:
+        raise NotImplementedError
 
     @property
     def front(self) -> int:
         return self._front
 
     @property
+    def array(self) -> list[Any]:
+        return self._array[self.front:self.rear] if self._array else []
+
+    @property
     def rear(self) -> int:
         return self._rear
 
-    def is_full(self) -> bool:
-        return len(self._array) == self._capacity
-
-    def is_empty(self) -> bool:
-        return not self._array
-
-    def enqueue(self, item: Any) -> int:
-        if self.is_full():
-            raise OverFlowError(self)
-
-        self._array.append(item)
-        self._rear += 1
-        return 0
-
-    def dequeue(self) -> Union[int, Any]:
-        if self.is_empty() or self._front >= self._rear:
-            raise UnderFlowError(self)
-        deleted_item = self._array[self._front]
-        self._front += 1
-        return deleted_item
-
-    def peek(self) -> Any:
-        if self.is_empty() or self._front >= self._rear:
-            return "QUEUE EMPTY"
-        return self._array[self._front]
-
-    # private method to mangle string __repr__
-    @staticmethod
-    def _mangled(item: Any) -> str:
-        if '\n' in str(item):
-            return f"{str(type(item))[8:-2].split('.')[-1]}@{id(item)}"
-        return str(item)
-
     def __str__(self):
         if self.is_empty():
             return '┌───────────────────┐\n' \
                    '│    QUEUE EMPTY    │\n' \
                    '└───────────────────┘'
         padding = 4
         max_breadth = max(
-            len((self._mangled(item))) for item in self._array
+            len((Commons.repr(item))) for item in self.array
         ) + padding
         middle_part = 'FRONT -> │'
         upper_part = f"\n{' ' * (len(middle_part) - 1)}┌"
         lower_part = f"{' ' * (len(middle_part) - 1)}└"
-        if self._front:  # Representing Garbage Values with '╳'
-            for _ in self._array[:self._front]:
+        if self.front:  # Representing Garbage Values with '╳'
+            for _ in self._array[:self.front]:
                 middle_part += f"{'╳'.center(max_breadth)}│"
                 upper_part += f"{'─' * max_breadth}┬"
                 lower_part += f"{'─' * max_breadth}┴"
             upper_part = upper_part[:-1] + '╥'
             middle_part = middle_part[:-1] + '║'
             lower_part = lower_part[:-1] + '╨'
-        for item in self._array[self._front:]:
-            middle_part += f'{self._mangled(item).center(max_breadth)}│'
+        for item in self._array[self.front:]:
+            middle_part += f'{Commons.repr(item).center(max_breadth)}│'
             upper_part += f"{'─' * max_breadth}┬"
             lower_part += f"{'─' * max_breadth}┴"
         upper_part = f"{upper_part[:-1]}"
         lower_part = f"{lower_part[:-1]}"
-        upper_part += f"{'╖' if len(self._array) == self._front else '┐'}\n"
+        upper_part += f"{'╖' if len(self._array) == self.front else '┐'}\n"
         middle_part += ' <- REAR\n'
-        lower_part += f"{'╜' if len(self._array) == self._front else '┘'}\n"
+        lower_part += f"{'╜' if len(self._array) == self.front else '┘'}\n"
         return upper_part + middle_part + lower_part
 
-    def __repr__(self):
-        return self.__str__()
+    @abstractmethod
+    def is_empty(self) -> bool:
+        ...
+
+    @abstractmethod
+    def is_full(self) -> bool:
+        ...
+
+    @abstractmethod
+    def enqueue(self, item: Any) -> int:
+        ...
+
+    @abstractmethod
+    def dequeue(self) -> Any:
+        ...
+
+    @abstractmethod
+    def peek(self) -> Any:
+        ...
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/CircularLinkedList.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/CircularLinkedList.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import Optional
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 from datastax.Lists.AbstractLists.Node import Node
 
 
 class CircularLinkedList(LinkedList, ABC):
     def _max_width(self, node: Optional[Node]):
         max_width = 0
         ref = node
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/DoublyCircularList.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyCircularList.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 
 from datastax.Lists.AbstractLists.CircularLinkedList import CircularLinkedList
 from datastax.Lists.AbstractLists.DoublyLinkedList import DoublyLinkedList
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 
 
 class DoublyCircularList(DoublyLinkedList, CircularLinkedList, ABC):
 
     def __str__(self):
         if not self.head:
             return 'NULL'
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/DoublyLinkedList.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyLinkedList.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import Optional
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 from datastax.Lists.AbstractLists.DoublyNode import DoublyNode
 
 
 class DoublyLinkedList(LinkedList, ABC):
     _head: Optional[DoublyNode] = None
     _tail: Optional[DoublyNode] = None
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/DoublyNode.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 from typing import Optional, Self
 
 from datastax.Lists.AbstractLists.Node import Node
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 
 
 class DoublyNode(Node, ABC):
     _next: Optional[Self]
     _prev: Optional[Self]
 
     @property
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/LinkedList.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/LinkedList.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Any, Optional, Self
+from typing import Any, Optional, Self, Iterable
 from datastax.Lists.AbstractLists.Node import Node
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 from abc import abstractmethod, ABC as AbstractClass
 
 
 class LinkedList(AbstractClass):
     _head: Optional[Node] = None
     _tail: Optional[Node] = None
 
@@ -22,15 +22,15 @@
     @property
     def tail(self):
         return self._tail
 
     def __str__(self):
         start_padding = 1
         top = mid = dow = " " * start_padding
-        ref = self._head
+        ref = self.head
         max_width = self._max_width(ref) + 4
         nodes = 0
         while ref:
             top += f"┌{'─' * max_width}╥────┐   "
             mid += f"│{f'{Commons.repr(ref.data)}'.center(max_width)}║  ----->"
             dow += f"└{'─' * max_width}╨────┘   "
             ref = ref.next
@@ -63,9 +63,9 @@
         ...
 
     @abstractmethod
     def insert(self, data: Any) -> None:
         ...
 
     @abstractmethod
-    def _construct(self, array: Optional[list[Any]]) -> Self:
+    def _construct(self, array: Iterable[Any]) -> Self:
         ...
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/Node.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/Node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Self, Optional, Any
-from datastax.Lists.Utils import Commons
+from datastax.Utils import Commons
 from abc import ABC as AbstractClass, abstractmethod
 
 
 class Node(AbstractClass):
     data: Optional[Any]
     _next: Optional[Self]
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/Queue.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/Queue.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Optional, Any
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists.Node import Node
+from datastax.Utils import Commons
 
 
 class Queue(LinkedList, ABC):
     _capacity = 0
     _rear = 0
 
+    def append(self, data: Any) -> None:
+        raise NotImplementedError
+
+    def insert(self, data: Any) -> None:
+        raise NotImplementedError
+
     @property
     def capacity(self):
         return self._capacity
 
     def __str__(self, head: Optional[Node] = None):
-        def maximum_breadth(ref: Optional[Node]) -> int:
-            result = 0
-            while ref:
-                result = max(len(str(ref.data)), result)
-                ref = ref.next
-            return result
-
         if self.is_empty():
             return '╔═══════════════════╗\n' \
                    '║    QUEUE EMPTY    ║\n' \
                    '╚═══════════════════╝'
         padding = 4
-        max_breadth = maximum_breadth(self.head) + padding
+        ref = self.head
+        max_breadth = self._max_width(ref) + padding
         middle_part = 'FRONT -> '
-        upper_part = f"{' ' * (len(middle_part) - 1)} "
-        lower_part = f"{' ' * (len(middle_part) - 1)} "
-        temp = self.head
-        while temp:
-            item = temp.data
+        lower_part = upper_part = f"{' ' * (len(middle_part) - 1)} "
+        while ref:
+            item = ref.data
             upper_part += f"┌{'─' * max_breadth}┐   "
-            middle_part += f'|{str(item).center(max_breadth)}│ <-'
+            middle_part += f'|{Commons.repr(item).center(max_breadth)}│ <-'
             lower_part += f"└{'─' * max_breadth}┘   "
-            temp = temp.next
+            ref = ref.next
         upper_part = f"{upper_part[:-1]}\n"
         middle_part += ' REAR\n'
         lower_part = f"{lower_part[:-1]}\n"
 
         return upper_part + middle_part + lower_part
 
     @abstractmethod
-    def is_empty(self):
+    def is_empty(self) -> bool:
+        ...
+
+    @abstractmethod
+    def is_full(self) -> bool:
+        ...
+
+    @abstractmethod
+    def enqueue(self, item: Any) -> int:
+        ...
+
+    @abstractmethod
+    def dequeue(self) -> Any:
         ...
 
     @abstractmethod
-    def is_full(self):
+    def peek(self) -> str | Optional[Any]:
         ...
```

### Comparing `datastax-0.4.0/datastax/Lists/AbstractLists/__init__.py` & `datastax-0.4.1/datastax/Lists/AbstractLists/__init__.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/Lists/CircularLinkedList.py` & `datastax-0.4.1/datastax/Lists/CircularLinkedList.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
 
-from datastax.Lists import LinkedList
+from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import CircularLinkedList as AbstractList
 
 
-class CircularLinkedList(AbstractList,
-                         LinkedList):
+class CircularLinkedList(AbstractList, LinkedList):
     def append(self, data: Any) -> None:
         super().append(data)
         self.tail.set_next(self.head)
 
     def insert(self, data: Any):
         super().insert(data)
         self.tail.set_next(self.head)
```

### Comparing `datastax-0.4.0/datastax/Lists/DoublyLinkedList.py` & `datastax-0.4.1/datastax/Lists/DoublyLinkedList.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import Any, Optional, Iterable, Self
 
-from datastax.Lists import DoublyNode, LinkedList
+from datastax.Lists.DoublyNode import DoublyNode
+from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import DoublyLinkedList as AbstractList
 
 
 class DoublyLinkedList(AbstractList, LinkedList):
     def __init__(self, items: Optional[Iterable[Any]] = None,
                  head: Optional[DoublyNode] = None,
                  tail: Optional[DoublyNode] = None):
         if head and tail:
             head.set_next(tail)
             tail.set_prev(head)
         super().__init__(items, head, tail)
 
-    def _construct(self, array: Optional[list[Any]]) -> Self:
+    def _construct(self, array: Iterable[Any]) -> Self:
         return super()._construct(array)
 
-    def set_head(self, head: Optional[DoublyNode] = None):
+    def set_head(self, head):
         if head is not None and not isinstance(head, DoublyNode):
             raise TypeError("The 'head' parameter must be an "
                             "instance of DoublyNode or its subclass.")
         super().set_head(head)
 
-    def set_tail(self, tail: Optional[DoublyNode] = None):
+    def set_tail(self, tail):
         if tail is not None and not isinstance(tail, DoublyNode):
             raise TypeError("The 'tail' parameter must be an "
                             "instance of DoublyNode or its subclass.")
         super().set_tail(tail)
 
     def append(self, data: Any) -> None:
         node = DoublyNode(data)
```

### Comparing `datastax-0.4.0/datastax/Lists/DoublyNode.py` & `datastax-0.4.1/datastax/Lists/DoublyNode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Self, Optional
 
-from datastax.Lists import Node
+from datastax.Lists.Node import Node
 from datastax.Lists.AbstractLists import DoublyNode as AbstractNode
 
 
 class DoublyNode(AbstractNode, Node):
-    def __init__(self, data: Optional[Any] = None,
+    def __init__(self, data: Any,
                  _next: Optional[Self] = None,
                  prev: Optional[Self] = None):
         super().__init__(data)
         self.set_next(_next)
         self.set_prev(prev)
 
     def set_next(self, _next: Optional[Self] = None):
```

### Comparing `datastax-0.4.0/datastax/Lists/LRUCache.py` & `datastax-0.4.1/datastax/Lists/LRUCache.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,54 +9,57 @@
 
 The functions get and put must each run in O(1) average time complexity.
 
 LRU -> Least Recently used
 """
 from typing import Any
 
-from datastax.Lists import DoublyLinkedList, DoublyNode
+from datastax.Lists.DoublyLinkedList import DoublyLinkedList
+from datastax.Lists.DoublyNode import DoublyNode
 
 
 class LRUCache(DoublyLinkedList):
     def __init__(self, capacity: int):
         super().__init__()
         self._capacity = capacity
         self._cache: dict[int, DoublyNode] = {}
         self._head = DoublyNode('HEAD')
         self._tail = DoublyNode('TAIL')
         self.tail.set_prev(self.head)
         self.head.set_next(self.tail)
 
-    def get(self, key: int) -> int:
+    def get(self, key: int) -> int | None:
         if key not in self._cache:
             return -1
         node = self._cache[key]
         self._enqueue(node)
-        return node.data[1]
+        return node.data[1] if node.data else None
 
-    def put(self, key: int, value: int) -> None:
+    def put(self, key: int, value: int):
         if key not in self._cache:
             node = DoublyNode([key, value])
             if len(self._cache) == self._capacity:
                 self._dequeue()
         else:
             node = self._cache[key]
-            node.data[1] = value
+            if node.data:
+                node.data[1] = value
         self._enqueue(node)
 
-    def _enqueue(self, node: DoublyNode) -> None:
+    def _enqueue(self, node: DoublyNode):
         if node.prev:
             node.prev.set_next(node.next)
         if node.next:
             node.next.set_prev(node.prev)
         node.set_prev(self.tail.prev)
         node.set_next(self.tail)
         self.tail.prev.set_next(node)
         self.tail.set_prev(node)
-        self._cache[node.data[0]] = node
+        if node.data:
+            self._cache[node.data[0]] = node
 
     def _dequeue(self) -> None:
         node = self.head.next
         self.head.set_next(node.next)
         node.next.set_prev(node.prev)
         self._cache.pop(node.data[0])
```

### Comparing `datastax-0.4.0/datastax/Lists/LinkedList.py` & `datastax-0.4.1/datastax/Lists/LinkedList.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Optional, Iterable, Self
 
-from datastax.Lists import Node
+from datastax.Lists.Node import Node
 from datastax.Lists.AbstractLists import LinkedList as AbstractLinkedList
 
 
 class LinkedList(AbstractLinkedList):
     def __init__(
             self,
             items: Optional[Iterable[Any]] = None,
@@ -13,40 +13,39 @@
     ):
         if head and tail:
             head.set_next(tail)
         self.set_head(head)
         self.set_tail(tail)
         if tail and not head:
             self.set_head(tail)
-        self._construct(items)
+        self._construct(items if items else [])
 
     def __iter__(self):
         ref = self._head
         while ref:
             yield ref.data
             ref = ref.next
 
-    def set_head(self, head: Optional[Node]):
+    def set_head(self, head: Node | None):
         if head is None or isinstance(head, Node):
             self._head = head
             return
         raise TypeError("The 'head' parameter must be an "
                         "instance of Node or its subclass.")
 
-    def set_tail(self, tail: Optional[Node]):
+    def set_tail(self, tail: Node | None):
         if tail is None or isinstance(tail, Node):
             self._tail = tail or self.head
             return
         raise TypeError("The 'tail' parameter must be an "
                         "instance of Node or its subclass.")
 
-    def _construct(self, items: Optional[Iterable[Any]]) -> Self:
-        if items:
-            for item in items:
-                self.append(item)
+    def _construct(self, items: Iterable[Any]) -> Self:
+        for item in items:
+            self.append(item)
         return self
 
     def append(self, data: Any) -> None:
         node = Node(data)
         if self.tail and not self.head:
             self.set_head(self.tail)
         if not self.head:
```

### Comparing `datastax-0.4.0/datastax/Lists/Node.py` & `datastax-0.4.1/datastax/Lists/Node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Self, Optional
 
 from datastax.Lists.AbstractLists import Node as AbstractNode
 
 
 class Node(AbstractNode):
-    def __init__(self, data: Optional[Any] = None,
+    def __init__(self, data: Any,
                  _next: Optional[Self] = None):
         self.data = data
         self.set_next(_next)
 
     def set_next(self, _next: Optional[Self] = None):
         if _next is None or isinstance(_next, Node):
             self._next = _next
```

### Comparing `datastax-0.4.0/datastax/Lists/Queue.py` & `datastax-0.4.1/datastax/Lists/Queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # Queue implementation using LinkedList
 
 from sys import maxsize
-from typing import Any
-from datastax.Lists import Node
+from typing import Any, Optional, Sequence, Self
+from datastax.Lists.Node import Node
 from datastax.errors import OverFlowError, UnderFlowError
-from datastax.Lists import LinkedList
+from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import Queue as AbstractQueue
 
 
 class Queue(AbstractQueue, LinkedList):
-    def __init__(self, capacity: int = None, items: list[Any] = None):
+    def __init__(self, capacity: Optional[int] = None,
+                 items: Optional[list] = None):
         super().__init__()
         self._rear = 0
         self.set_capacity(capacity)
-        if items:
-            for item in items[:self.capacity]:
-                self.enqueue(item)
+        self._build(items if items else [])
+
+    def _build(self, items: Sequence[Any]) -> Self:
+        for item in items[:self.capacity]:
+            self.enqueue(item)
+        return self
 
     def is_empty(self) -> bool:
         return self.head is None
 
     def is_full(self) -> bool:
         return self._rear == self.capacity
 
-    def set_capacity(self, capacity: int):
+    def set_capacity(self, capacity: int | None):
         if capacity is None:
             self._capacity = maxsize
             return
         if not isinstance(capacity, int):
             raise TypeError("The 'capacity' parameter must be an "
                             "instance of int or its subclass.")
         if capacity < 0:
@@ -51,17 +55,11 @@
             raise UnderFlowError(self)
         deleted_node = self.head
         deleted_item = deleted_node.data
         self.set_head(self.head.next)
         self._rear -= 1
         return deleted_item
 
-    def peek(self) -> str:
+    def peek(self) -> str | Optional[Any]:
         if self.is_empty():
             return "QUEUE EMPTY"
-        return str(self._tail.data if self._tail else None)
-
-    def append(self, data: Any) -> None:
-        raise NotImplementedError
-
-    def insert(self, data: Any) -> None:
-        raise NotImplementedError
+        return self._tail.data if self._tail else None
```

### Comparing `datastax-0.4.0/datastax/__main__.py` & `datastax-0.4.1/datastax/__main__.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/errors.py` & `datastax-0.4.1/datastax/errors.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/__init__.py` & `datastax-0.4.1/datastax/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/avl_tree.py` & `datastax-0.4.1/datastax/trees/avl_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/binary_search_tree.py` & `datastax-0.4.1/datastax/trees/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/binary_tree.py` & `datastax-0.4.1/datastax/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/expression_tree.py` & `datastax-0.4.1/datastax/trees/expression_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/fibonacci_tree.py` & `datastax-0.4.1/datastax/trees/fibonacci_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/heap_tree.py` & `datastax-0.4.1/datastax/trees/heap_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/huffman_tree.py` & `datastax-0.4.1/datastax/trees/huffman_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/min_heap_tree.py` & `datastax-0.4.1/datastax/trees/min_heap_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/min_segment_tree.py` & `datastax-0.4.1/datastax/trees/min_segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/private_trees/binary_tree.py` & `datastax-0.4.1/datastax/trees/private_trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/private_trees/huffman_tree.py` & `datastax-0.4.1/datastax/trees/private_trees/huffman_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/private_trees/red_black_tree.py` & `datastax-0.4.1/datastax/trees/private_trees/red_black_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/private_trees/segment_tree.py` & `datastax-0.4.1/datastax/trees/private_trees/segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/private_trees/threaded_binary_tree.py` & `datastax-0.4.1/datastax/trees/private_trees/threaded_binary_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/red_black_tree.py` & `datastax-0.4.1/datastax/trees/red_black_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/splay_tree.py` & `datastax-0.4.1/datastax/trees/splay_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/sum_segment_tree.py` & `datastax-0.4.1/datastax/trees/sum_segment_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax/trees/threaded_binary_tree.py` & `datastax-0.4.1/datastax/trees/threaded_binary_tree.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.0/datastax.egg-info/PKG-INFO` & `datastax-0.4.1/datastax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datastax
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python library to handle dataStructures
 Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax
 Author: Pritam K
 Author-email: pritamkundu771@gmail.com
 Maintainer: Pritam Kundu
 License: MIT
@@ -35,15 +35,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-    updated: Sunday, 11th July 2023
+    updated: Wednesday, 12th July 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -68,19 +68,18 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored linkedlists -> Lists
-- Refactored arrays -> Arrays
-- Refactored private_lists -> AbstractLists
-- Refactored AbstractLists by converting all items to AbstractClass to prevent direct initialization.
-- Module Conventions converted to uppercase CamelCase from lowercase snake_case
+- Refactored Array Contents
+- Added AbstractArray SubModule to abstract print logic
+- Added more test cases for Queues
+- Type Checked Arrays and Lists with mypy
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
@@ -239,8 +238,7 @@
 
 ## What's Next
 
 - Enhanced Documentation
 - Better TestCases for Huffman Tree
 - Better TestCases for Segment Trees
 - Test Cases for Fibonacci Tree
-- Refactoring Arrays SubPackage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datastax Version: 0.4.0 Summary: A python library
+Metadata-Version: 2.1 Name: datastax Version: 0.4.1 Summary: A python library
 to handle dataStructures Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax Author: Pritam K Author-
 email: pritamkundu771@gmail.com Maintainer: Pritam Kundu License: MIT Project-
 URL: Bug Tracker, https://github.com/warmachine028/datastax/issues Project-URL:
 Documentation, https://github.com/warmachine028/datastax#readme Project-URL:
 Source Code, https://github.com/warmachine028/datastax Platform: Windows
 Platform: Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier:
@@ -15,68 +15,66 @@
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Documentation
 Classifier: Topic :: Education :: Testing Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Software Development ::
 Documentation Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed Requires-Python: >=3.11 Description-Content-Type:
-text/markdown License-File: LICENSE updated: Sunday, 11th July 2023
+text/markdown License-File: LICENSE updated: Wednesday, 12th July 2023
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
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored linkedlists -> Lists - Refactored arrays -> Arrays - Refactored
-private_lists -> AbstractLists - Refactored AbstractLists by converting all
-items to AbstractClass to prevent direct initialization. - Module Conventions
-converted to uppercase CamelCase from lowercase snake_case ## Table of Contents
-- [Introduction](#introduction) - [Problem Statement](#problem-statement) -
-[Benefits](#benefits) - [Requirements](#requirements) - [Installation]
-(#installation) - [Usage](#usage) - [What's Next](#whats-next) ## Introduction
-- This library offers a simple yet powerful solution for implementing common
-abstract data structures. - With a pure Python implementation, it provides
-representations of tree, linked list, and array-based data structures
-accessible through a basic command prompt interface. - The package includes
-visualization features that enhance the understanding of each data structure. -
-Students can greatly benefit from utilizing this package for their learning and
-educational purposes. - Please note that this project is currently a work in
-progress and undergoing active development. ## Problem Statement - Many CS
-students encounter difficulties in comprehending the intricate internal
-architecture of complex Abstract Data Types (ADTs) during the initial stages of
-their B.Tech course. - When attempting to solve coding challenges that involve
-writing test cases using these ADTs, it becomes excessively burdensome to
-manually create these data structures from scratch. - Furthermore, while
-developing programs that implement these ADTs, numerous errors are encountered
-due to the inability to visualize and understand the underlying processes of
-these data structures. ## Benefits - Swift installation process - Efficient and
-prompt updates - Minimal disk space usage due to its small size - No additional
-modules or dependencies needed - Developed entirely from scratch - Upcoming
-user-friendly documentation - Command line demonstration for easy usage ##
-Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
-to the latest python version) ## Installation 1. Use the python package manager
-[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
-datastax ``` ## Usage ### Demo - To get a demo of the library use the following
-command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
-```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
-LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
-> trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
-``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
-1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
+Refactored Array Contents - Added AbstractArray SubModule to abstract print
+logic - Added more test cases for Queues - Type Checked Arrays and Lists with
+mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
+(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
+[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
+Introduction - This library offers a simple yet powerful solution for
+implementing common abstract data structures. - With a pure Python
+implementation, it provides representations of tree, linked list, and array-
+based data structures accessible through a basic command prompt interface. -
+The package includes visualization features that enhance the understanding of
+each data structure. - Students can greatly benefit from utilizing this package
+for their learning and educational purposes. - Please note that this project is
+currently a work in progress and undergoing active development. ## Problem
+Statement - Many CS students encounter difficulties in comprehending the
+intricate internal architecture of complex Abstract Data Types (ADTs) during
+the initial stages of their B.Tech course. - When attempting to solve coding
+challenges that involve writing test cases using these ADTs, it becomes
+excessively burdensome to manually create these data structures from scratch. -
+Furthermore, while developing programs that implement these ADTs, numerous
+errors are encountered due to the inability to visualize and understand the
+underlying processes of these data structures. ## Benefits - Swift installation
+process - Efficient and prompt updates - Minimal disk space usage due to its
+small size - No additional modules or dependencies needed - Developed entirely
+from scratch - Upcoming user-friendly documentation - Command line
+demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
+(Suggesting you to always update to the latest python version) ## Installation
+1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
+install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
+demo of the library use the following command - **Windows**: ```bash > py -
+m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
+_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
+> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
+Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
+guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
+Singly Linked List: HEAD TAIL âââââââ¥âââââ
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ âââââââ¥âââââ â 1
-â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
+âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
+----->â 4 â -----> NULL âââââââ¨âââââ
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ âââââââ¨âââââ 2.
-Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
@@ -106,8 +104,8 @@
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
 db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
 Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree - Refactoring Arrays SubPackage
+Tree
```

### Comparing `datastax-0.4.0/datastax.egg-info/SOURCES.txt` & `datastax-0.4.1/datastax.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 setup.py
 datastax/__init__.py
 datastax/__main__.py
 datastax/errors.py
 datastax.egg-info/PKG-INFO
 datastax.egg-info/SOURCES.txt
 datastax.egg-info/dependency_links.txt
-datastax.egg-info/not-zip-safe
 datastax.egg-info/top_level.txt
+datastax/Arrays/PriorityQueue.py
+datastax/Arrays/Queue.py
+datastax/Arrays/Stack.py
 datastax/Arrays/__init__.py
-datastax/Arrays/priority_queue.py
-datastax/Arrays/queue.py
-datastax/Arrays/stack.py
+datastax/Arrays/AbstractArrays/Array.py
+datastax/Arrays/AbstractArrays/Queue.py
+datastax/Arrays/AbstractArrays/Stack.py
+datastax/Arrays/AbstractArrays/__init__.py
 datastax/Lists/CircularLinkedList.py
 datastax/Lists/DoublyCircularList.py
 datastax/Lists/DoublyLinkedList.py
 datastax/Lists/DoublyNode.py
 datastax/Lists/LRUCache.py
 datastax/Lists/LinkedList.py
 datastax/Lists/Node.py
@@ -26,16 +29,16 @@
 datastax/Lists/AbstractLists/DoublyCircularList.py
 datastax/Lists/AbstractLists/DoublyLinkedList.py
 datastax/Lists/AbstractLists/DoublyNode.py
 datastax/Lists/AbstractLists/LinkedList.py
 datastax/Lists/AbstractLists/Node.py
 datastax/Lists/AbstractLists/Queue.py
 datastax/Lists/AbstractLists/__init__.py
-datastax/Lists/Utils/Commons.py
-datastax/Lists/Utils/__init__.py
+datastax/Utils/Commons.py
+datastax/Utils/__init__.py
 datastax/trees/__init__.py
 datastax/trees/avl_tree.py
 datastax/trees/binary_search_tree.py
 datastax/trees/binary_tree.py
 datastax/trees/expression_tree.py
 datastax/trees/fibonacci_tree.py
 datastax/trees/heap_tree.py
```

### Comparing `datastax-0.4.0/setup.py` & `datastax-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         '      ii. Min Segment Tree\n'
         '   g. Huffman Tree\n'
         '   h. Red Black Tree\n'
         '   i. Fibonacci Tree\n'
         '   j. Splay Tree\n\n'
     )
     sys.stderr.write(f"Warning: Could not open README.md due {error}\n")
-
 setup(
     name='datastax',
     maintainer="Pritam Kundu",
     description='A python library to handle dataStructures',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/warmachine028/datastax',
@@ -89,19 +88,20 @@
 
         "Typing :: Typed"
     ],
     platforms=["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
     test_suite='pytest',
     version=datastax.__version__,
     python_requires='>=3.11',
-    zip_safe=False,
     packages=[
         'datastax',
+        'datastax/Utils',
         'datastax/Arrays',
+        'datastax/Arrays/AbstractArrays',
         'datastax/Lists',
-        'datastax/Lists/Utils',
         'datastax/Lists/AbstractLists',
         'datastax/trees',
         'datastax/trees/private_trees',
     ],
-    author_email='pritamkundu771@gmail.com'
+    author_email='pritamkundu771@gmail.com',
 )
+# python setup.py sdist bdist_wheel
```

