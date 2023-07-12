# Comparing `tmp/cryptographyComplements-0.3.1.tar.gz` & `tmp/cryptographyComplements-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.3.1.tar", last modified: Fri Jul  7 17:46:00 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.3.2.tar", last modified: Wed Jul 12 17:25:09 2023, max compression
```

## Comparing `cryptographyComplements-0.3.1.tar` & `cryptographyComplements-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.724180 cryptographyComplements-0.3.1/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-07-07 17:46:00.723181 cryptographyComplements-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.705494 cryptographyComplements-0.3.1/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.1/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.1/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    15770 2023-07-07 17:41:22.000000 cryptographyComplements-0.3.1/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2182 2023-07-07 10:34:30.000000 cryptographyComplements-0.3.1/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     3002 2023-07-07 17:40:51.000000 cryptographyComplements-0.3.1/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.720162 cryptographyComplements-0.3.1/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-07-07 17:46:00.000000 cryptographyComplements-0.3.1/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:46:00.725181 cryptographyComplements-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-07-07 17:45:45.000000 cryptographyComplements-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.738794 cryptographyComplements-0.3.2/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-07-12 17:25:09.736615 cryptographyComplements-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.731896 cryptographyComplements-0.3.2/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.2/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-07-12 16:51:45.000000 cryptographyComplements-0.3.2/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    15876 2023-07-12 17:22:44.000000 cryptographyComplements-0.3.2/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2069 2023-07-12 17:15:11.000000 cryptographyComplements-0.3.2/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3002 2023-07-07 17:40:51.000000 cryptographyComplements-0.3.2/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.735595 cryptographyComplements-0.3.2/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-12 17:25:09.000000 cryptographyComplements-0.3.2/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:25:09.739786 cryptographyComplements-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-07-12 16:56:08.000000 cryptographyComplements-0.3.2/setup.py
```

### Comparing `cryptographyComplements-0.3.1/LICENSE` & `cryptographyComplements-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.1/PKG-INFO` & `cryptographyComplements-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.3.1/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.3.2/cryptographyComplements/cryptosystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,22 @@
             import decimal
 
             lenght = len(ciphertext)
 
             letters = {}
 
             for c in ciphertext:
-
                 try:
                     letters[c] += 1
 
                 except KeyError:
                     letters[c] = 1
 
 
             if ' ' in letters.keys():
-
                 lenght -= letters[' ']
 
             lettersFrequency = {}
 
             for letter in letters.keys():
 
                 if letter == ' ':
@@ -101,15 +99,15 @@
         "The RSA implementation, including the Creation of the Key, Encryption and Decryption."
 
         def KeyCreation(p: int, q: int) -> tuple:
             "Given two distinct primes: p and q. Return p, q, N=p*q, e=65537"
 
             N = p * q
 
-            e = 2**16 + 1
+            e = pow(2, 16) + 1
 
             return p, q, N, e
         
         def Encryption(plaintext: int, e: int, N: int) -> int:
             "Given the plaintext converted in an integer, the public encryption exponent (e) and N: product of p and q, return the plaintext encrypted."
 
             if not 1 <= plaintext < N:
@@ -131,7 +129,8 @@
 
             d = ExtendedEuclideanModularMultiplicativeInverse(e, n)
 
             plaintext = pow(ciphertext, d, N)
 
             return plaintext
 
+
```

### Comparing `cryptographyComplements-0.3.1/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.3.2/cryptographyComplements/mathFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 "In this script you can find all the mathematical functions relative to Number Theory."
-from cryptographyComplements.tools import Numbers # required class, because contains functions used by some of them below
-import math
 
 def EulerTotientFunction(n: int) -> int:
     "Calculate, from a given number, the Euler Totient function."
     
     if n <= 1:
         if n == 1:
             return 1
@@ -26,14 +24,16 @@
 
 
     return int(relativePrime)
 
 def EuclideanAlgorithm(a: int, b: int) -> int:
     "Given two numbers, a and b, calculate their Great Common Divisor."
 
+    import math
+
     q = math.floor(a/b)
     r = a-(b*q)
 
     if r == 0:
         return b
 
     q2 = math.floor(b/r)
@@ -65,15 +65,15 @@
         x = x0 - (a // b)*x1
         y = y0 - (a // b)*y1
         a, b, x0, x1, y0, y1 = b, r, x1, x, y1, y
 
     return a, x0, y0 # a is the GCD of a and b
 
 def MultiplicativeOrder(a: int, n: int) -> int:
-    "Calculate the multiplicative order of a in mod n. The function if n is relatively prime to a then it will return the Carmichael function, in any other case it will use the bruteforce algorithm."
+    "Calculate the multiplicative order of a in mod n. The function if n is relatively prime to a it will return the Carmichael function, in any other case it will use the bruteforce algorithm."
 
     if EuclideanAlgorithm(a, n) == 1:
         Carmichael = CarmichaelFunction(n)
         return Carmichael
     
     k = 0
 
@@ -124,14 +124,17 @@
 
         x = value + (n * value2)
 
         return x
     
 def ChineseRemainderTheorem(congruences:list, modulo: list) -> int:
     "From a list of congruences and a list of modulos, tuples are accepted too, of the same lenght, calculate the Chinese Remainder Theorem. \n\nIf there is a solution it will be returned as a number, but if there isn't it will return None."
+    
+    from cryptographyComplements.tools import Numbers
+
     try:
         for i in range(0, len(modulo)):
             if i == (len(modulo)-1):
                 break
 
             try:
                 # check if the numbers are relatively prime, if not there isn't a solution to the congruence
@@ -270,34 +273,36 @@
     if pow(a, (p-1)*(q-1)//g, p*q) != 1:
         return False
 
     return True
 
 def PrimeNumberTheorem(n: int) -> float:
     "Calculate the Prime Number Theorem for n using n/ln(n). The value returned is an approximation."
+
+    import math
+
     if n <= 1:
         return 0.0
-    return n / (math.log(n))
+    return n / (math.log(n)) # here log is the natural logarithm ln(x)
 
 from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
 class FactorizationMethods:
     "This class contains factorization methods, including special purpose and general purpose ones."
 
     def TrialDivision(n: int, maxN: int) -> list:
         "This factorization method uses the trial division and it's a special purpose algorithm, so it's not recommended for numbers that could be possibly be prime, or for large composites.\n\nNote: maxN defines the maximum value for which will be searched primes that factorize n. It has been implemented to avoid large computations. \nIf you want to search up to n, just put maxN=n"
 
+        from cryptographyComplements.tools import Numbers
+
         if MillerRabinPrimalityTest(n, 100):
             return [n]        
 
         primeFactors = []
         keep = n
 
-        import math
-
-        # for i in range(2, n+1):
         for i in range(2, maxN+1):
 
             flag = False
 
             if n / i % 1 == 0:
 
                 for prime in primeFactors:
@@ -349,14 +354,16 @@
             d = ExtendedEuclideanAlgorithm(a-1, n)[0]
             if 1 < d < n:
                 return d
 
     def FermatFactorizationAlgorithm(n: int) -> None|tuple|bool:
         "The Fermat factorization algorithm is exponential and special purpose. \n\nIf n it's not odd, it will return None, in any other case it will return a nontrivial divisor of n or it will return True if n is prime."
 
+        import math
+
         if n % 2 == 0:
             return None
         
         rad = math.ceil(math.sqrt(n))
         maxN = math.ceil((n+9)/6)
 
         steps = 1
@@ -379,14 +386,16 @@
                 return (int(a-b), int(a+b))
             
         return True
 
 def CarmichaelFunction(n: int) -> int:
     "Calculate the Carmichael function for n."
 
+    from cryptographyComplements.tools import Numbers
+
     factorization = FactorizationMethods.TrialDivision(n, n)
 
     powers = {}
 
     for prime in factorization:
         try:
             powers[prime] += 1
@@ -418,14 +427,16 @@
         
         if MillerRabinPrimalityTest(i, 100):
             return i
         
 def SieveOfEratosthenes(n: int) -> list:
     "Calculate all the prime numbers less than n using the Sieve of Eratosthenes."
 
+    import math
+
     nums = [i for i in range(2, n+1)]
 
     maxN = math.ceil(math.sqrt(n))
 
     for p in nums:
 
         if p > maxN:
```

### Comparing `cryptographyComplements-0.3.1/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.3.2/cryptographyComplements/primalityTests.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,50 +10,44 @@
     lucaslehmerSequence = MersennePrime.LucasLehmerModuloNumbers(n-1, mersenne)
 
     if lucaslehmerSequence[n-2] % mersenne == 0:
         return True
     
     return False
     
-from cryptographyComplements.mathFunctions import FermatLittleTheorem
-import random
 def FermatPrimalityTest(n: int, k: int) -> bool:
     "Given an integer n and k: the number of times to test for primality, the function will return false and it's a composite number or it will return true and it would be a prime number or a Carmichael number. \n\nThis primality test is probabilistic."
 
+    from cryptographyComplements.mathFunctions import FermatLittleTheorem
+    import random
+
     for i in range(k):
 
         a = random.randint(2, n-1)
 
         if FermatLittleTheorem(a, n) != 1:
             return False
 
     return True
 
 
 def MillerRabinPrimalityTest(n: int, k: int) -> bool:
     "Given a number: n, to check and k: the number of test to execute, see whether the number is a possible prime or a composite. This primality test is probabilistic."
 
-    if n <= 1:
-        return False
+    import random
 
-    if n % 2 == 0:
-        if n == 2:
-            return True
-        return False
-    
-    if n % 5 == 0:
-        if n == 5:
-            return True
+    if n < 2 or n % 1 != 0:
         return False
 
-    if n == 3: # needs to be checked here to avoid a ValueError, or if you are working only with large numbers you can disable this if statement
+    if n in (2, 3): # this numbers need to be checked here to avoid endless while loop for 2, Value Error for 3 | The causes are written on Miller-Rabin documentation page
         return True
     
     q = (n - 1) // 2
     p = 1
+
     while q % 2 == 0:
         q //= 2
         p += 1
 
     for i in range(k):
         a = random.randint(2, n - 2)
 
@@ -66,9 +60,8 @@
                 return False
         
             x = y
 
         if y != 1:
             return False
         
-    return True
-
+    return True
```

### Comparing `cryptographyComplements-0.3.1/cryptographyComplements/tools.py` & `cryptographyComplements-0.3.2/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.1/setup.py` & `cryptographyComplements-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import decimal
 
 setup(
     name='cryptographyComplements',
-    version='0.3.1',
+    version='0.3.2',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

