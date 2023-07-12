# Comparing `tmp/ColabTurtleArbreBinaire-0.0.3.tar.gz` & `tmp/ColabTurtleArbreBinaire-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabTurtleArbreBinaire-0.0.3.tar", last modified: Wed Jul 12 13:20:18 2023, max compression
+gzip compressed data, was "ColabTurtleArbreBinaire-0.0.4.tar", last modified: Wed Jul 12 13:29:42 2023, max compression
```

## Comparing `ColabTurtleArbreBinaire-0.0.3.tar` & `ColabTurtleArbreBinaire-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-12 13:20:18.615316 ColabTurtleArbreBinaire-0.0.3/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-12 13:20:18.614143 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     3832 2023-07-12 13:20:18.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      293 2023-07-12 13:20:18.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-12 13:20:18.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       16 2023-07-12 13:20:18.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       24 2023-07-12 13:20:18.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)    38552 2023-07-11 17:21:22.000000 ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.py
--rw-r--r--   0 matt       (501) staff       (20)     1061 2023-07-11 17:54:16.000000 ColabTurtleArbreBinaire-0.0.3/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     3832 2023-07-12 13:20:18.614868 ColabTurtleArbreBinaire-0.0.3/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     3407 2023-07-12 13:17:24.000000 ColabTurtleArbreBinaire-0.0.3/README.md
--rw-r--r--   0 matt       (501) staff       (20)      539 2023-07-12 13:20:04.000000 ColabTurtleArbreBinaire-0.0.3/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-07-12 13:20:18.615437 ColabTurtleArbreBinaire-0.0.3/setup.cfg
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-12 13:29:42.833485 ColabTurtleArbreBinaire-0.0.4/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-12 13:29:42.830673 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     3946 2023-07-12 13:29:42.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      293 2023-07-12 13:29:42.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-12 13:29:42.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       16 2023-07-12 13:29:42.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)       24 2023-07-12 13:29:42.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)    38552 2023-07-11 17:21:22.000000 ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.py
+-rw-r--r--   0 matt       (501) staff       (20)     1061 2023-07-11 17:54:16.000000 ColabTurtleArbreBinaire-0.0.4/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     3946 2023-07-12 13:29:42.832688 ColabTurtleArbreBinaire-0.0.4/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     3521 2023-07-12 13:26:10.000000 ColabTurtleArbreBinaire-0.0.4/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      539 2023-07-12 13:29:19.000000 ColabTurtleArbreBinaire-0.0.4/pyproject.toml
+-rw-r--r--   0 matt       (501) staff       (20)       38 2023-07-12 13:29:42.833684 ColabTurtleArbreBinaire-0.0.4/setup.cfg
```

### Comparing `ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.egg-info/PKG-INFO` & `ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabTurtleArbreBinaire
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module using ColabTurtlePlus to draw binary trees
 Author-email: Matthieu Bensussan <matthieu.bensussan@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
     - `v` la valeur de sa racine ;
     - `sag` son sous-arbre de gauche ;
     - `sad` son sous-arbre de droite.
 
 Ce module est destiné à l'enseignement de l'informatique. Il a pour but de
 fournir un support graphique pour accompagner les élèves dans l'apprentissage
 des algorithmes classiques sur les arbres binaires (de recherche). Il ne 
-fourni pas cependant ces algorithmes qui seront abordés en classe avec le
+fournit pas cependant ces algorithmes qui seront abordés en classe avec le
 professeur.
 
 ## Installation
 
 Il faut préalablement installer le module en exécutant la commande shell
 suivante dans une cellule :
 
@@ -148,7 +148,10 @@
 `'suffixe'` ou `'postfixe'`.
 
 ### Animation de l'insertion d'une valeur dans un arbre binaire de recherche
 
 ```python
 dessiner_insertion(abr0, 34)
 ```
+
+*Remarque.* L'animation montre simplement où le noeud sera ajouté sans modifier
+l'arbre passé en paramètre.
```

### Comparing `ColabTurtleArbreBinaire-0.0.3/ColabTurtleArbreBinaire.py` & `ColabTurtleArbreBinaire-0.0.4/ColabTurtleArbreBinaire.py`

 * *Files identical despite different names*

### Comparing `ColabTurtleArbreBinaire-0.0.3/LICENSE` & `ColabTurtleArbreBinaire-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabTurtleArbreBinaire-0.0.3/PKG-INFO` & `ColabTurtleArbreBinaire-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabTurtleArbreBinaire
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module using ColabTurtlePlus to draw binary trees
 Author-email: Matthieu Bensussan <matthieu.bensussan@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
     - `v` la valeur de sa racine ;
     - `sag` son sous-arbre de gauche ;
     - `sad` son sous-arbre de droite.
 
 Ce module est destiné à l'enseignement de l'informatique. Il a pour but de
 fournir un support graphique pour accompagner les élèves dans l'apprentissage
 des algorithmes classiques sur les arbres binaires (de recherche). Il ne 
-fourni pas cependant ces algorithmes qui seront abordés en classe avec le
+fournit pas cependant ces algorithmes qui seront abordés en classe avec le
 professeur.
 
 ## Installation
 
 Il faut préalablement installer le module en exécutant la commande shell
 suivante dans une cellule :
 
@@ -148,7 +148,10 @@
 `'suffixe'` ou `'postfixe'`.
 
 ### Animation de l'insertion d'une valeur dans un arbre binaire de recherche
 
 ```python
 dessiner_insertion(abr0, 34)
 ```
+
+*Remarque.* L'animation montre simplement où le noeud sera ajouté sans modifier
+l'arbre passé en paramètre.
```

### Comparing `ColabTurtleArbreBinaire-0.0.3/README.md` & `ColabTurtleArbreBinaire-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     - `v` la valeur de sa racine ;
     - `sag` son sous-arbre de gauche ;
     - `sad` son sous-arbre de droite.
 
 Ce module est destiné à l'enseignement de l'informatique. Il a pour but de
 fournir un support graphique pour accompagner les élèves dans l'apprentissage
 des algorithmes classiques sur les arbres binaires (de recherche). Il ne 
-fourni pas cependant ces algorithmes qui seront abordés en classe avec le
+fournit pas cependant ces algorithmes qui seront abordés en classe avec le
 professeur.
 
 ## Installation
 
 Il faut préalablement installer le module en exécutant la commande shell
 suivante dans une cellule :
 
@@ -135,8 +135,11 @@
 *Remarque.* `'largeur'` peut être remplacé par `'infixe'`, `'préfixe'`,
 `'suffixe'` ou `'postfixe'`.
 
 ### Animation de l'insertion d'une valeur dans un arbre binaire de recherche
 
 ```python
 dessiner_insertion(abr0, 34)
-```
+```
+
+*Remarque.* L'animation montre simplement où le noeud sera ajouté sans modifier
+l'arbre passé en paramètre.
```

### Comparing `ColabTurtleArbreBinaire-0.0.3/pyproject.toml` & `ColabTurtleArbreBinaire-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ColabTurtleArbreBinaire"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Matthieu Bensussan", email="matthieu.bensussan@gmail.com" },
 ]
 description = "A module using ColabTurtlePlus to draw binary trees"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

