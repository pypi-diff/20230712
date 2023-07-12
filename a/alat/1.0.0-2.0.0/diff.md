# Comparing `tmp/alat-1.0.0.tar.gz` & `tmp/alat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alat-1.0.0.tar", last modified: Thu Nov 10 14:00:21 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `alat-1.0.0.tar` & `alat-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxrwxr-x   0 can       (1000) can       (1000)        0 2022-11-10 14:00:21.362080 alat-1.0.0/
--rw-rw-r--   0 can       (1000) can       (1000)     1098 2022-10-10 10:20:35.000000 alat-1.0.0/LICENSE
--rw-rw-r--   0 can       (1000) can       (1000)     1103 2022-11-10 14:00:21.362080 alat-1.0.0/PKG-INFO
--rw-rw-r--   0 can       (1000) can       (1000)      615 2022-11-10 10:46:33.000000 alat-1.0.0/README.md
--rw-rw-r--   0 can       (1000) can       (1000)      602 2022-11-10 13:49:18.000000 alat-1.0.0/pyproject.toml
--rw-rw-r--   0 can       (1000) can       (1000)       38 2022-11-10 14:00:21.362080 alat-1.0.0/setup.cfg
-drwxrwxr-x   0 can       (1000) can       (1000)        0 2022-11-10 14:00:21.358080 alat-1.0.0/src/
-drwxrwxr-x   0 can       (1000) can       (1000)        0 2022-11-10 14:00:21.362080 alat-1.0.0/src/alat/
--rw-rw-r--   0 can       (1000) can       (1000)     1133 2022-11-10 10:46:05.000000 alat-1.0.0/src/alat/__init__.py
--rw-rw-r--   0 can       (1000) can       (1000)     8554 2022-10-31 17:56:30.000000 alat-1.0.0/src/alat/apps.py
--rw-rw-r--   0 can       (1000) can       (1000)    33718 2022-11-09 14:10:31.000000 alat-1.0.0/src/alat/base.py
--rw-rw-r--   0 can       (1000) can       (1000)    12336 2022-10-30 04:54:10.000000 alat-1.0.0/src/alat/base2.py
--rw-rw-r--   0 can       (1000) can       (1000)     7478 2022-11-09 14:13:40.000000 alat-1.0.0/src/alat/crypt.py
--rw-rw-r--   0 can       (1000) can       (1000)     1194 2022-10-09 05:16:40.000000 alat-1.0.0/src/alat/exceptions.py
--rw-rw-r--   0 can       (1000) can       (1000)    17862 2022-10-31 16:12:36.000000 alat-1.0.0/src/alat/vectors.py
-drwxrwxr-x   0 can       (1000) can       (1000)        0 2022-11-10 14:00:21.362080 alat-1.0.0/src/alat.egg-info/
--rw-rw-r--   0 can       (1000) can       (1000)     1103 2022-11-10 14:00:21.000000 alat-1.0.0/src/alat.egg-info/PKG-INFO
--rw-rw-r--   0 can       (1000) can       (1000)      294 2022-11-10 14:00:21.000000 alat-1.0.0/src/alat.egg-info/SOURCES.txt
--rw-rw-r--   0 can       (1000) can       (1000)        1 2022-11-10 14:00:21.000000 alat-1.0.0/src/alat.egg-info/dependency_links.txt
--rw-rw-r--   0 can       (1000) can       (1000)        5 2022-11-10 14:00:21.000000 alat-1.0.0/src/alat.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/__init__.py
+-rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/apps.py
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/crypts.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/errors.py
+-rw-r--r--   0        0        0    42621 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/matrices.py
+-rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 alat-2.0.0/src/alat/vectors.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 alat-2.0.0/LICENSE
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 alat-2.0.0/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 alat-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 alat-2.0.0/PKG-INFO
```

### Comparing `alat-1.0.0/LICENSE` & `alat-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2022] [ALAT: Advanced Linear Algebra Toolkit]
+Copyright (c) [2023] [ALAT: Advanced Linear Algebra Toolkit]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `alat-1.0.0/src/alat/crypt.py` & `alat-2.0.0/src/alat/crypts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,216 @@
-# Cryptography for ALAT (Advanced Linear Algebra Toolkit)
+# Cryptography methods in ALAT (Advanced Linear Algebra Toolkit)
 
-from .exceptions import (
-   DimensionError, 
-   InconsistentCharacterError, 
-   InvertibleMatrixError,
-)
-from .base import cross_mul
-from .base2 import (
-   isinvertible, 
-   inverse, 
+from .errors import (
+   InconsistentCharacterError,
+   InvertibleMatixError,
 )
+from alat.matrices import Matrices
 
-__all__ = ["Crypt"]
+__all__ = ["Crypts"]
 
-numbers = {
+ALL_CHARS = {
    "0": 0, "1": 1, "2": 2, "3": 3, "4": 4, "5": 5, "6": 6, "7": 7, 
    "8": 8, "9": 9, 
-}
 
-alphabets = {
    "A": 10, "B": 11, "C": 12, "D": 13, "E": 14, "F": 15, "G": 16,   
    "H": 17, "I": 18, "J": 19, "K": 20, "L": 21, "M": 22, "N": 23,   
    "O": 24, "P": 25, "Q": 26, "R": 27, "S": 28, "T": 29, "U": 30,   
    "V": 31, "W": 32, "X": 33, "Y": 34, "Z": 35, "a": 36, "b": 37, 
    "c": 38, "d": 39, "e": 40, "f": 41, "g": 42, "h": 43, "i": 44, 
    "j": 45, "k": 46, "l": 47, "m": 48, "n": 49, "o": 50, "p": 51, 
    "q": 52, "r": 53, "s": 54, "t": 55, "u": 56, "v": 57, "w": 58, 
    "x": 59, "y": 60, "z": 61, 
-}
 
-whitespaces = {
-   "!": 62, "'": 63, "^": 64, "$": 65, "%": 66, "&": 67, "/": 68, 
-   "(": 69, ")": 70, "{": 71, "}": 72, "[": 73, "]": 74, "=": 75, 
-   "*": 76, "-": 77, "?": 78, "_": 79, "~": 80, ";": 81, ",": 82, 
-   "`": 83, ".": 84, ":": 85, "<": 86, ">": 87, "|": 88, '"': 89,      
-   "@": 90, "é": 91, " ": 92
+   "é": 62, "!": 63, "'": 64, "^": 65, "+": 66, "%": 67, "&": 68, 
+   "/": 69, "(": 70, ")": 71, "=": 72, "?": 73, "_": 74, ";": 75, 
+   ":": 76, "\"": 77, ">": 78, "<": 79, "|": 80, "#": 81, "$": 82, 
+   "{": 83, "[": 84, "]": 85, "}": 86, "*": 87, "\\": 88, "-": 89, 
+   "@": 90, "€": 91, "~": 92, ",": 93, "`": 94, ".": 95, " ": 96,
 }
 
-class Crypt:
-   """Cryptography for ALAT (Advanced Linear Algebra Toolkit)."""
-
-   def to_matrix(self, msg, dim):
-      """Converts message to matrix form.
-      
-      ## Parameters:
-      `msg` argument represents message that will be converted to 
-      matrix and must be str. `dim` argument represents dimension
-      of matrix that will be created and must be tuple. For example:
-
-      >>> _msg = "What's going on!"
-      >>> print(len(_msg))
-      9
-      >>> result = Crypt().to_matrix(msg=_msg, dim=(4, 4))
-      >>> print(result)
-      [[32, 43, 36, 55], [63, 54, 92, 42], [50, 44, 49, 42], [92, 50,
-       49, 62]]
-
+class Crypts:
+   """ Cryptography methods in ALAT. 
+   
+   This class provide four basics methods for cryptography. First
+   is that 'convert the message to matrix'. Second is that 'encode
+   the message into a matrix'. Third is that 'decode the encoded 
+   matrix'. And lastly, 'convert the encoded matrix to message'.
+   """
+
+   def to_matrix(self, message: str, dim: tuple):
+      """ Convert the `message` to matrix whixh has `dim` dimension.
+      If there is missing elements, in this case, fill the missing 
+      elements with -1. For example: 
+
+      >>> message = "What is going on here !!!"
+      >>> result = Crypts().to_matrix(message=message, dim=(6, 6))
+      >>> for row in result:
+      ...   print(row)
+      [32, 43, 36, 55, 96, 44]
+      [54, 96, 42, 50, 44, 49]
+      [42, 96, 50, 49, 96, 43]
+      [40, 53, 40, 96, 63, 63]
+      [63, -1, -1, -1, -1, -1]
+      [-1, -1, -1, -1, -1, -1]
       """
-      _row, _matrix = [], []
-
-      if not isinstance(msg, str):
-         raise TypeError("'msg' argument must be str")
+      if not isinstance(message, str):
+         raise TypeError("'message' must be string")
       if not isinstance(dim, tuple):
-         raise TypeError("'dim' argument must be tuple")
-      # Be carefull! Length of message is to appropriate width 
-      # dimension of matrix that will be created.
-      if not len(msg) == dim[0] * dim[1] and not len(dim) == 2:
-         raise DimensionError("given 'dim' argument is not suitable")
-      # Each characters of message must be in alphabets, numbers, 
-      # or whitespaces.
-      for char in msg:
-         if char in numbers.keys():
-            _row.append(numbers[char])
-         elif char in alphabets.keys():
-            _row.append(alphabets[char])
-         elif char in whitespaces.keys():
-            _row.append(whitespaces[char])
-         else:
+         raise TypeError("'dim' must be tuple")
+      if len(dim) != 2:
+         raise ValueError(
+            "'dim' can just contain row and column info"
+         )
+      if dim[0] != dim[1]:
+         raise ValueError(
+            "Matrix that will be generated must be square"
+         )
+      # Generate the matrix from scratch.
+      array = []
+      # Find the id corresponding to characters.
+      for char in message:
+         if char in ALL_CHARS.keys():
+            array.append(ALL_CHARS[char])
+         else: # otherwise, raise error
             error_msg = "Inconsistent character: '%s'" % char
             raise InconsistentCharacterError(error_msg)
-         # And then generates main matrix from rows.
-         if len(_row) == dim[1]:
-            _matrix.append(list(_row))
-            _row = []
-
-      return _matrix
-
-   def encode(self, msg, dim, encoding_matrix, digits=18):
-      """Encodes raw matrix.
+      # Convert the 'array' to 'matrix'.
+      matrix = Matrices().arbitrary(-1, dim)
+      index = 0
+      for i in range(dim[0]):
+         for j in range(dim[1]):
+            # Make integer the elements of 'matrix'.
+            matrix[i][j] = int(matrix[i][j])
+            # Copy the 'array' elements into 'matrix'.
+            if index != len(array):
+               matrix[i][j] = array[index]
+               index += 1
+      
+      return matrix
+   
+   def encode(self, message: str, enocding_matrix: list[list], 
+              digits: int = 6):
+      """ Encode the `message` using `encoding_matrix`. An important
+      point is that `encoding_matrix` must be invertible. For example:
       
-      ## Parameters:
-      `msg` argument represents message that will be converted 
-      to matrix and must be string. `dim` argument represents 
-      dimension of matrix that will be created and must be tuple. 
-      `encoding_matrix` argument represents matrix that will be
-      encoded the message and must be invertible. For example:
-
-      >>> _msg = "What's going on!"
-      >>> print(len(_msg))
-      9
-      >>> _matrix = [
-         [4, -1, -3, 1], 
-         [-9, 4, 0, -9], 
-         [3, 2, 4, -9],
-         [8, 7, 0, 0]
+      >>> message = "What is going on here !!!"
+      >>> encoding_matrix = [
+         [1, 7, -4, -5, 1, 2],
+         [-2, 0, 0, -3, 0, 1],
+         [1, 0, -4, 0, -1, 9],
+         [2, -8, 8, 0, 1, -8],
+         [-1, -7, 4, 5, 0, 4],
+         [1, 7, 4, -5, 6, -2],
       ]
-      >>> result = Crypt().encode(msg=_msg, encoding_matrix=_matrix
-      dim=(4, 4), digits=18)
-      >>> print(result)
-      [[289.0, 597.0, 48.0, -679.0], [378.0, 631.0, 179.0, -1251.0], 
-      [287.0, 518.0, 46.0, -787.0], [561.0, 640.0, -80.0, -799.0]]
-
+      >>> result = Crypts().encode(message, encoding_matrix)
+      >>> for row in result:
+      ...   print(row)
+      [40.0, -580.0, 728.0, -29.0, 315.0, 287.0]
+      [9.0, 13.0, 388.0, -583.0, 356.0, 260.0]
+      [-55.0, -469.0, 580.0, -233.0, 299.0, 536.0]
+      [166.0, -488.0, 952.0, -359.0, 474.0, -149.0]
+      [62.0, 449.0, -264.0, -312.0, 57.0, 122.0]
+      [-2.0, 1.0, -8.0, 8.0, -7.0, -6.0]
       """
-      # 'encoding_matrix' must be invertible
-      if not isinvertible(encoding_matrix):
-         raise InvertibleMatrixError("given matrix must be invertible")
-      # Firstly, converts message to a matrix.
-      _to_matrix = self.to_matrix(msg, dim)
-      _encode = cross_mul(_to_matrix, encoding_matrix, digits)
-
-      return _encode
-
-   def decode(self, encoded_matrix, decoding_matrix, digits=18):
-      """Decodes encoded message.
-      
-      ## Parameters:
-      `encoded_matrix` argument represents encoded matrix. 
-      `decoding_matrix` represents matrix that will decode encoded 
-      matrix and must be invertible. For example:
-
-      >>> _msg = "What's going on!"
-      >>> _matrix = [
-         [4, -1, -3, 1], 
-         [-9, 4, 0, -9], 
-         [3, 2, 4, -9],
-         [8, 7, 0, 0]
+      if not Matrices().isinvertible(enocding_matrix):
+         raise InvertibleMatixError(
+            "'encoding_matrix' must be invertible"
+         )
+      # Get the dimension of 'encoding_matrix'.
+      dim = Matrices().dim(enocding_matrix)
+      # Convert the 'message' to 'matrix'.
+      matrix = self.to_matrix(message, dim)
+      # Multiply the 'matrix' and 'encoding_matrix' as cross.
+      encode = Matrices().cross_mul(matrix, enocding_matrix, digits)
+
+      return encode
+
+   def decode(self, encoded_msg: list[list], 
+              encoding_matrix: list[list], digis: int = 6):
+      """ Decode the encoded message using `encoding_matrix`. An 
+      important point is that `encoding_matrix` must be invertible.
+      For example: 
+
+      >>> encoded_msg = [
+         [40.0, -580.0, 728.0, -29.0, 315.0, 287.0],
+         [9.0, 13.0, 388.0, -583.0, 356.0, 260.0],
+         [-55.0, -469.0, 580.0, -233.0, 299.0, 536.0],
+         [166.0, -488.0, 952.0, -359.0, 474.0, -149.0],
+         [62.0, 449.0, -264.0, -312.0, 57.0, 122.0],
+         [-2.0, 1.0, -8.0, 8.0, -7.0, -6.0],
       ]
-      >>> _encoded = Crypt().encode(msg=_msg, encoding_matrix=_matrix
-      dim=(4, 4), digits=18)
-      >>> print(_encoded)
-      [[289.0, 597.0, 48.0, -679.0], [378.0, 631.0, 179.0, -1251.0], 
-      [287.0, 518.0, 46.0, -787.0], [561.0, 640.0, -80.0, -799.0]]
-
-      >>> result = Crypt().decode(_encoded, _matrix, digits=18)
-      >>> print(result)
-      [[32.0, 43.0, 36.0, 55.0], [63.0, 54.0, 92.0, 42.0], [50.0, 44.0,
-      49.0, 42.0], [92.0, 50.0, 49.0, 62.0]]
-
+      >>> encoding_matrix = [
+         [1, 7, -4, -5, 1, 2],
+         [-2, 0, 0, -3, 0, 1],
+         [1, 0, -4, 0, -1, 9],
+         [2, -8, 8, 0, 1, -8],
+         [-1, -7, 4, 5, 0, 4],
+         [1, 7, 4, -5, 6, -2],
+      ]
+      >>> result = Crypts().decode(encoded_msg, encoding_matrix)
+      >>> for row in result:
+      ...   print(row)
+      [32, 43, 36, 55, 96, 44]
+      [54, 96, 42, 50, 44, 49]
+      [42, 96, 50, 49, 96, 43]
+      [40, 53, 40, 96, 63, 63]
+      [63, -1, -1, -1, -1, -1]
+      [-1, -1, -1, -1, -1, -1]
       """
-      if not isinvertible(decoding_matrix):
-         raise InvertibleMatrixError("given matrix must be invertible")
-      # Firstly, finds inverse of 'decoding_matrix'.
-      _inverse = inverse(decoding_matrix, digits)
-      # And then, multiplies encoded matrix with decoding matrix.
-      _decode = cross_mul(encoded_matrix, _inverse, digits)
-      # Finally, we round each value of matrix.
-      for i in range(len(_decode)):
-         for j in range(len(_decode[0])):
-            _decode[i][j] = float(round(_decode[i][j]))
-
-      return _decode
-
-   def to_str(self, encoded_matrix, decoding_matrix, digits=18):
-      """Converts encoded matrix to message.
-      
-      ## Parameters:
-      `encoded_matrix` argument represents encoded matrix. 
-      `decoding_matrix` argument represents decoding matrix that will
-      decode encoded matrix and must be invertible. For example:
-
-      >>> _msg = "What's going on!"
-      >>> _matrix = [
-         [4, -1, -3, 1], 
-         [-9, 4, 0, -9], 
-         [3, 2, 4, -9],
-         [8, 7, 0, 0]
+      if not Matrices().ismatrix(encoded_msg):
+         raise Matrices("Inconsistent matrix defination")
+      if not Matrices().isinvertible(encoding_matrix):
+         raise InvertibleMatixError(
+            "'encoding_matrix' must be invertible"
+         )
+      # Reverse the 'encoding_matrix'.
+      inverse = Matrices().inverse(encoding_matrix, digis)
+      # Multiply the 'inv' and 'encoded_msg'.
+      decode = Matrices().cross_mul(encoded_msg, inverse, digis)
+      # And lastly, round the elements of 'decode'.
+      for i in range(len(encoding_matrix)):
+         for j in range(len(encoding_matrix[0])):
+            decode[i][j] = round(decode[i][j])
+
+      return decode
+   
+   def to_message(self, encoded_msg: list[list], 
+                  encoding_matrix: list[list], digis: int = 6):
+      """ Convert the encoded matrix to message. An important point
+      is that `encoding_matrix` must be invertible. For example:
+
+      >>> encoded_msg = [
+         [40.0, -580.0, 728.0, -29.0, 315.0, 287.0],
+         [9.0, 13.0, 388.0, -583.0, 356.0, 260.0],
+         [-55.0, -469.0, 580.0, -233.0, 299.0, 536.0],
+         [166.0, -488.0, 952.0, -359.0, 474.0, -149.0],
+         [62.0, 449.0, -264.0, -312.0, 57.0, 122.0],
+         [-2.0, 1.0, -8.0, 8.0, -7.0, -6.0],
       ]
-      >>> _encoded = Crypt().encode(msg=_msg, encoding_matrix=_matrix
-      dim=(4, 4), digits=18)
-      >>> print(_encoded)
-      [[289.0, 597.0, 48.0, -679.0], [378.0, 631.0, 179.0, -1251.0], 
-      [287.0, 518.0, 46.0, -787.0], [561.0, 640.0, -80.0, -799.0]]
-
-      >>> result = Crypt().to_str(_encoded, _matrix, digits=18)
+      >>> encoding_matrix = [
+         [1, 7, -4, -5, 1, 2],
+         [-2, 0, 0, -3, 0, 1],
+         [1, 0, -4, 0, -1, 9],
+         [2, -8, 8, 0, 1, -8],
+         [-1, -7, 4, 5, 0, 4],
+         [1, 7, 4, -5, 6, -2],
+      ]
+      >>> result = Crypts().to_message(encoded_msg, encoding_matrix)
       >>> print(result)
-      "What's going on!"
-
+      "What is going on here !!!"
       """
-      # Converts encoded matrix to string. For that, replaces keys and
-      # values of numbers, alphabets, whitespaces.
-      _alphabets, _numbers, _whitespaces = {}, {}, {}
-      for key, value in numbers.items():
-         _numbers[value] = key
-      for key, value in alphabets.items():
-         _alphabets[value] = key
-      for key, value in whitespaces.items():
-         _whitespaces[value] = key
-      # And then, decodes encoded matrix.
-      _decode = self.decode(encoded_matrix, decoding_matrix, digits)
-      _string = ""
-      # Lastly, concats characters.
-      for row in _decode:
-         for char in row:
-            if char in _alphabets.keys():
-               _string += _alphabets[char]
-            elif char in _numbers.keys():
-               _string += _numbers[char]
-            else:
-               _string += _whitespaces[char]
+      # Decode the encoded message to raw matrix.
+      decode = self.decode(encoded_msg, encoding_matrix, digis)
+      # Repalce the key and value of 'ALL_CHARS'.
+      all_chars = {}
+      for key, value in ALL_CHARS.items():
+         all_chars[value] = key
+      # Find the characters corresponding to numbers.
+      message = ""
+      for row in decode:
+         for number in row:
+            if number != -1:
+               message += all_chars[number]
+
+      return message
 
-      return _string
```

