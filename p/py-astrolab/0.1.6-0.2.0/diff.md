# Comparing `tmp/py_astrolab-0.1.6.tar.gz` & `tmp/py_astrolab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.1.6.tar", max compression
+gzip compressed data, was "py_astrolab-0.2.0.tar", max compression
```

## Comparing `py_astrolab-0.1.6.tar` & `py_astrolab-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.1.6/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.1.6/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16850 2023-06-21 20:38:42.474113 py_astrolab-0.1.6/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.1.6/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    72284 2023-07-09 14:33:18.004388 py_astrolab-0.1.6/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.1.6/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.1.6/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    61624 2023-07-09 13:46:32.333795 py_astrolab-0.1.6/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.1.6/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.1.6/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.1.6/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.1.6/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2356 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5061 2023-05-31 21:03:53.211311 py_astrolab-0.1.6/py_astrolab/types.py
--rwxr-xr-x   0        0        0     5952 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-07-09 14:33:08.497846 py_astrolab-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.0/py_astrolab/__init__.py
+-rw-r--r--   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.0/py_astrolab/aspects.py
+-rw-r--r--   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.0/py_astrolab/charts/__init__.py
+-rw-r--r--   0        0        0    73247 2023-07-12 13:04:58.545802 py_astrolab-0.2.0/py_astrolab/charts/charts_svg.py
+-rw-r--r--   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.0/py_astrolab/charts/templates/basic.xml
+-rw-r--r--   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.0/py_astrolab/charts/templates/extended.xml
+-rw-r--r--   0        0        0    61624 2023-07-09 13:46:32.333795 py_astrolab-0.2.0/py_astrolab/charts/templates/minimal.xml
+-rw-r--r--   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.0/py_astrolab/charts/wonderful_mistake.py
+-rw-r--r--   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.0/py_astrolab/fetch_geonames.py
+-rw-r--r--   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.0/py_astrolab/kr.config.json
+-rw-r--r--   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.2.0/py_astrolab/main.py
+-rw-r--r--   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.0/py_astrolab/print_all_data.py
+-rw-r--r--   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.0/py_astrolab/relationship_score.py
+-rw-r--r--   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.0/py_astrolab/report.py
+-rw-r--r--   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.0/py_astrolab/types.py
+-rw-r--r--   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.0/py_astrolab/utilities.py
+-rw-r--r--   0        0        0      689 2023-07-12 13:34:09.729189 py_astrolab-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.0/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 py_astrolab-0.2.0/setup.py
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.0/PKG-INFO
```

### Comparing `py_astrolab-0.1.6/py_astrolab/__init__.py` & `py_astrolab-0.2.0/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/aspects.py` & `py_astrolab-0.2.0/py_astrolab/aspects.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,16 +216,16 @@
         if user[p1_name]['element'] == user[p2_name]['element'] and aspect['aspect'] == 'square':
             is_fake_aspect = True
         if aspect['aspect'] in {'trine', 'conjunction'}:
             if user[p1_name]['element'] != user[p2_name]['element']:
                 if aspect['orbit'] > 3:
                     is_fake_aspect = True
         elif aspect['aspect'] == 'opposition':
-            p1_sign = user[p1_name]['sign']
-            p2_sign = user[p2_name]['sign']
+            p1_sign = user[p1_name]['signs'][0]
+            p2_sign = user[p2_name]['signs'][0]
             p1_sign_opposite = self.user.signs_dict[p1_sign]['opposite']
             if not p1_sign_opposite.startswith(p2_sign):
                 is_fake_aspect = True
         return is_fake_aspect
 
     def get_relevant_aspects(self):
         """ 
@@ -305,16 +305,16 @@
         if user_1[p1_name]['element'] == user_2[p2_name]['element'] and aspect['aspect'] == 'square':
             is_fake_aspect = True
         if aspect['aspect'] in {'trine', 'conjunction'}:
             if user_1[p1_name]['element'] != user_2[p2_name]['element']:
                 if aspect['orbit'] > 3:
                     is_fake_aspect = True
         elif aspect['aspect'] == 'opposition':
-            p1_sign = user_1[p1_name]['sign']
-            p2_sign = user_2[p2_name]['sign']
+            p1_sign = user_1[p1_name]['signs'][0]
+            p2_sign = user_2[p2_name]['signs'][0]
             p1_sign_opposite = self.first_user.signs_dict[p1_sign]['opposite']
             if not p1_sign_opposite.startswith(p2_sign):
                 is_fake_aspect = True
         return is_fake_aspect
 
     def get_all_aspects(self):
         """
```

### Comparing `py_astrolab-0.1.6/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.2.0/py_astrolab/charts/charts_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,15 @@
         # pie slices
         offset = 360 - self.houses_degree_ut[6]
         # check transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             dropin = 0
         else:
             dropin = self.c1
-        slice = '<path d="M' + str(r) + ',' + str(r) + ' L' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + ',' + str(dropin + self.__sliceToY(num, r-dropin, offset)) + ' A' + str(
+        slice = f'<path class="zodiac" id="zodiac{type}" d="M' + str(r) + ',' + str(r) + ' L' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + ',' + str(dropin + self.__sliceToY(num, r-dropin, offset)) + ' A' + str(
             r-dropin) + ',' + str(r-dropin) + ' 0 0,0 ' + str(dropin + self.__sliceToX(num+1, r-dropin, offset)) + ',' + str(dropin + self.__sliceToY(num+1, r-dropin, offset)) + ' z" style="' + style + '"/>'
         # symbols
         offset = offset + 15
         # check transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             dropin = 54
         else:
@@ -472,54 +472,48 @@
         return output
 
     def __makeHouses(self, r):
         path = ""
 
         xr = 12
         for i in range(xr):
-            # check transit
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 160
                 roff = 72
                 t_roff = 36
             else:
                 dropin = self.c3
                 roff = self.c2
 
-            # offset is negative desc houses_degree_ut[6]
             offset = (int(self.houses_degree_ut[int(xr/2)]) / -1) + int(self.houses_degree_ut[i])
             x1 = self.__sliceToX(0, (r-dropin), offset) + dropin
             y1 = self.__sliceToY(0, (r-dropin), offset) + dropin
             x2 = self.__sliceToX(0, r-roff, offset) + roff
             y2 = self.__sliceToY(0, r-roff, offset) + roff
 
             if i < (xr-1):
-                text_offset = offset + \
-                    int(self.__degreeDiff(self.houses_degree_ut[(
-                        i+1)], self.houses_degree_ut[i]) / 6)
+                text_offset = offset + int(self.__degreeDiff(self.houses_degree_ut[(i+1)], self.houses_degree_ut[i]) / 6)
+                next_offset = (int(self.houses_degree_ut[int(xr/2)]) / -1) + int(self.houses_degree_ut[i+1])
             else:
-                text_offset = offset + \
-                    int(self.__degreeDiff(
-                        self.houses_degree_ut[0], self.houses_degree_ut[(xr-1)]) / 6)
+                text_offset = offset + int(self.__degreeDiff(self.houses_degree_ut[0], self.houses_degree_ut[(xr-1)]) / 6)
+                next_offset = (int(self.houses_degree_ut[int(xr/2)]) / -1) + int(self.houses_degree_ut[0])
 
             linecolor = self.colors_settings['houses_radix_line']
 
             # Transit houses lines.
             if self.chart_type == "Transit" or self.chart_type == "Composite":
-
-                # Degrees for point zero.
-
                 zeropoint = 360 - self.houses_degree_ut[6]
                 t_offset = zeropoint + self.t_houses_degree_ut[i]
                 if t_offset > 360:
                     t_offset = t_offset - 360
                 t_x1 = self.__sliceToX(0, (r-t_roff), t_offset) + t_roff
                 t_y1 = self.__sliceToY(0, (r-t_roff), t_offset) + t_roff
                 t_x2 = self.__sliceToX(0, r, t_offset)
                 t_y2 = self.__sliceToY(0, r, t_offset)
+
                 if i < 11:
                     t_text_offset = t_offset + \
                         int(self.__degreeDiff(self.t_houses_degree_ut[(
                             i+1)], self.t_houses_degree_ut[i]) / 2)
                 else:
                     t_text_offset = t_offset + \
                         int(self.__degreeDiff(
@@ -527,56 +521,64 @@
                 # linecolor
                 if i == 0 or i == 9 or i == 6 or i == 3:
                     t_linecolor = linecolor
                 else:
                     t_linecolor = self.colors_settings['houses_transit_line']
                 xtext = self.__sliceToX(0, (r-8), t_text_offset) + 8
                 ytext = self.__sliceToY(0, (r-8), t_text_offset) + 8
-
                 if self.chart_type == "Transit":
                     path = path + '<text style="fill: #00f; fill-opacity: 0; font-size: 14px"><tspan x="' + \
                         str(xtext-3)+'" y="'+str(ytext+3) + \
                         '">'+str(i+1)+'</tspan></text>'
                     path = path + '<line x1="'+str(t_x1)+'" y1="'+str(t_y1)+'" x2="'+str(t_x2)+'" y2="'+str(
-                        t_y2)+'" style="stroke: '+t_linecolor+'; stroke-width: 2px; stroke-opacity:0;"/>'
+                        t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:0;"/>'
 
                 else:
                     path = path + '<text style="fill: #00f; fill-opacity: .4; font-size: 14px"><tspan x="' + \
                         str(xtext-3)+'" y="'+str(ytext+3) + \
                         '">'+str(i+1)+'</tspan></text>'
                     path = path + '<line x1="'+str(t_x1)+'" y1="'+str(t_y1)+'" x2="'+str(t_x2)+'" y2="'+str(
-                        t_y2)+'" style="stroke: '+t_linecolor+'; stroke-width: 2px; stroke-opacity:.3;"/>'
+                        t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:.3;" class="house" id="house{i+1}"/>'
 
-            # if transit
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 84
-
-            dropin = 48
-
             if i+1 == 1:
                 house_number = 'I'
             elif i+1 == 4:
                 house_number = 'IV'
             elif i+1 == 7:
                 house_number = 'VII'
             elif i+1 == 10:
                 house_number = 'X'
             else:
                 house_number = i+1
-
             xtext = self.__sliceToX(
-                0, (r-dropin), text_offset) + dropin  # was 132
+                0, (r-48), text_offset) + 48  # was 132
             ytext = self.__sliceToY(
-                0, (r-dropin), text_offset) + dropin  # was 132
-            path = path + '<line x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
-                y2)+'" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-opacity:.4;"/>'
+                0, (r-48), text_offset) + 48  # was 132
+            x3 = self.__sliceToX(0, (r-dropin), next_offset) + dropin
+            y3 = self.__sliceToY(0, (r-dropin), next_offset) + dropin
+            x4 = self.__sliceToX(0, r-roff, next_offset) + roff
+            y4 = self.__sliceToY(0, r-roff, next_offset) + roff
+            # Inizia al bordo inferiore della cuspide della casa corrente
+            path_data = f"M {x1},{y1} "
+            # Vai al bordo superiore lungo la cuspide
+            path_data += f"L {x2},{y2} "
+            # Segui l'arco superiore alla prossima cuspide
+            path_data += f"A {r-roff},{r-roff} 0 0,0 {x4},{y4} "
+            # Vai al bordo inferiore lungo la cuspide
+            path_data += f"L {x3},{y3} "
+            # Segui l'arco inferiore indietro alla cuspide della casa corrente
+            path_data += f"A {r-dropin},{r-dropin} 0 0,1 {x1},{y1} "
+            # Chiudi il percorso (anche se non necessario perché le coordinate finali e iniziali coincidono)
+            path_data += "Z"
+            path = path + '<path d="'+path_data+'" class="house" id="house'+str(i+1)+'" fill="transparent" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-opacity:.4;"/>'
             path = path + '<text style="fill: #000000; fill-opacity: .4; font-size: 14px; font-weight: bold"><tspan x="' + \
                 str(xtext-10)+'" y="'+str(ytext+3) + \
                 '">'+str(house_number)+'</tspan></text>'
-
         return path
 
     def __makePlanets(self, r):
 
         planets_degut = {}
 
         diff = range(len(self.planets_settings))
```

### Comparing `py_astrolab-0.1.6/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.2.0/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.2.0/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.2.0/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/fetch_geonames.py` & `py_astrolab-0.2.0/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/kr.config.json` & `py_astrolab-0.2.0/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/main.py` & `py_astrolab-0.2.0/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/print_all_data.py` & `py_astrolab-0.2.0/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/relationship_score.py` & `py_astrolab-0.2.0/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.6/py_astrolab/report.py` & `py_astrolab-0.2.0/py_astrolab/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """
         Creates the planets table.
         """
 
         planets_data = [["Planet", "Sign", "Pos.", "Ret.", "House"]] + [
             [
                 planet.name,
-                planet.sign,
+                planet.signs[0],
                 round(float(planet.position), 2),
                 ("R" if planet.retrograde else "-"),
                 planet.house,
             ]
             for planet in self.instance.planets_list
         ]
 
@@ -55,15 +55,15 @@
 
     def get_houses_table(self) -> None:
         """
         Creates the houses table.
         """
 
         houses_data = [["House", "Sign", "Position"]] + [
-            [house.name, house.sign, round(float(house.position), 2)]
+            [house.name, house.signs, round(float(house.position), 2)]
             for house in self.instance.houses_list
         ]
 
         self.houses_table = AsciiTable(houses_data).table
 
     def print_report(self) -> None:
         """
```

### Comparing `py_astrolab-0.1.6/py_astrolab/types.py` & `py_astrolab-0.2.0/py_astrolab/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
     This is part of Kerykeion (C) 2022 Giacomo Battaglia
 """
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from ast import Dict
-from typing import Literal, Union, Optional
-from pydantic import BaseModel
+from typing import List, Literal, Optional, Union
 
+from pydantic import BaseModel
 
 # Exceptions:
 
 
 class KerykeionException(Exception):
     """
     Custom Kerykeion Exception
@@ -137,15 +137,15 @@
     """   
         Kerykeion Point Model
     """
 
     name: Union[Planet, Houses, Axis]
     quality:  Quality
     element: Element
-    sign: Sign
+    signs: List[Sign]
     sign_num: Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
     position: float
     abs_pos: float
     emoji: str
     point_type: Literal['Planet', 'House', 'Axis']
     house: Optional[Literal[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]] = None
     retrograde: Optional[bool] = None
```

### Comparing `py_astrolab-0.1.6/py_astrolab/utilities.py` & `py_astrolab-0.2.0/py_astrolab/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,72 +40,96 @@
 
 def calculate_position(degree: Union[int, float], number_name: str, point_type: Literal["Planet", "House", "Axis"]) -> KerykeionPoint:
     """Utility function to create a dictionary deviding
     the houses or the planets list."""
 
     if degree < 30:
         dictionary = {"name": number_name, "quality": "Cardinal", "element":
-                      "Fire", "sign": "Ari", "sign_num": 0, "position": degree, "abs_pos": degree,
+                      "Fire", "signs": ["Ari"], "sign_num": 0, "position": degree, "abs_pos": degree,
                       "emoji": "♈️", "point_type": point_type}
+        if point_type == 'House' and degree > 0:
+            dictionary['signs'].append('Tau')
 
     elif degree < 60:
         result = degree - 30
         dictionary = {"name": number_name, "quality": "Fixed", "element":
-                      "Earth", "sign": "Tau", "sign_num": 1, "position": result, "abs_pos": degree,
+                      "Earth", "signs": ["Tau"], "sign_num": 1, "position": result, "abs_pos": degree,
                       "emoji": "♉️", "point_type": point_type}
+        if point_type == 'House' and degree > 30:
+            dictionary['signs'].append('Gem')
     elif degree < 90:
         result = degree - 60
         dictionary = {"name": number_name, "quality": "Mutable", "element":
-                      "Air", "sign": "Gem", "sign_num": 2, "position": result, "abs_pos": degree,
+                      "Air", "signs": ["Gem"], "sign_num": 2, "position": result, "abs_pos": degree,
                       "emoji": "♊️", "point_type": point_type}
+        if point_type == 'House' and degree > 60:
+            dictionary['signs'].append('Can')
     elif degree < 120:
         result = degree - 90
         dictionary = {"name": number_name, "quality": "Cardinal", "element":
-                      "Water", "sign": "Can", "sign_num": 3, "position": result, "abs_pos": degree,
+                      "Water", "signs": ["Can"], "sign_num": 3, "position": result, "abs_pos": degree,
                       "emoji": "♋️", "point_type": point_type}
+        if point_type == 'House' and degree > 90:
+            dictionary['signs'].append('Leo')
     elif degree < 150:
         result = degree - 120
         dictionary = {"name": number_name, "quality": "Fixed", "element":
-                      "Fire", "sign": "Leo", "sign_num": 4, "position": result, "abs_pos": degree,
+                      "Fire", "signs": ["Leo"], "sign_num": 4, "position": result, "abs_pos": degree,
                       "emoji": "♌️", "point_type": point_type}
+        if point_type == 'House' and degree > 120:
+            dictionary['signs'].append('Vir')
     elif degree < 180:
         result = degree - 150
         dictionary = {"name": number_name, "quality": "Mutable", "element":
-                      "Earth", "sign": "Vir", "sign_num": 5, "position": result, "abs_pos": degree,
+                      "Earth", "signs": ["Vir"], "sign_num": 5, "position": result, "abs_pos": degree,
                       "emoji": "♍️", "point_type": point_type}
+        if point_type == 'House' and degree > 150:
+            dictionary['signs'].append('Lib')
     elif degree < 210:
         result = degree - 180
         dictionary = {"name": number_name, "quality": "Cardinal", "element":
-                      "Air", "sign": "Lib", "sign_num": 6, "position": result, "abs_pos": degree,
+                      "Air", "signs": ["Lib"], "sign_num": 6, "position": result, "abs_pos": degree,
                       "emoji": "♎️", "point_type": point_type}
+        if point_type == 'House' and degree > 180:
+            dictionary['signs'].append('Sco')
     elif degree < 240:
         result = degree - 210
         dictionary = {"name": number_name, "quality": "Fixed", "element":
-                      "Water", "sign": "Sco", "sign_num": 7, "position": result, "abs_pos": degree,
+                      "Water", "signs": ["Sco"], "sign_num": 7, "position": result, "abs_pos": degree,
                       "emoji": "♏️", "point_type": point_type}
+        if point_type == 'House' and degree > 210:
+            dictionary['signs'].append('Sag')
     elif degree < 270:
         result = degree - 240
         dictionary = {"name": number_name, "quality": "Mutable", "element":
-                      "Fire", "sign": "Sag", "sign_num": 8, "position": result, "abs_pos": degree,
+                      "Fire", "signs": ["Sag"], "sign_num": 8, "position": result, "abs_pos": degree,
                       "emoji": "♐️", "point_type": point_type}
+        if point_type == 'House' and degree > 240:
+            dictionary['signs'].append('Cap')
     elif degree < 300:
         result = degree - 270
         dictionary = {"name": number_name, "quality": "Cardinal", "element":
-                      "Earth", "sign": "Cap", "sign_num": 9, "position": result, "abs_pos": degree,
+                      "Earth", "signs": ["Cap"], "sign_num": 9, "position": result, "abs_pos": degree,
                       "emoji": "♑️", "point_type": point_type}
+        if point_type == 'House' and degree > 270:
+            dictionary['signs'].append('Aqu')
     elif degree < 330:
         result = degree - 300
         dictionary = {"name": number_name, "quality": "Fixed", "element":
-                      "Air", "sign": "Aqu", "sign_num": 10, "position": result, "abs_pos": degree,
+                      "Air", "signs": ["Aqu"], "sign_num": 10, "position": result, "abs_pos": degree,
                       "emoji": "♒️", "point_type": point_type}
+        if point_type == 'House' and degree > 300:
+            dictionary['signs'].append('Pis')
     elif degree < 360:
         result = degree - 330
         dictionary = {"name": number_name, "quality": "Mutable", "element":
-                      "Water", "sign": "Pis", "sign_num": 11, "position": result, "abs_pos": degree,
+                      "Water", "signs": ["Pis"], "sign_num": 11, "position": result, "abs_pos": degree,
                       "emoji": "♓️", "point_type": point_type}
+        if point_type == 'House' and degree > 330:
+            dictionary['signs'].append('Ari')
     else:
         raise KerykeionException(
             f'Error in calculating positions! Degrees: {degree}')
 
     return KerykeionPoint(**dictionary)
 
 def dangerous_json_dump(subject, dump=True, new_output_directory=None):
```

### Comparing `py_astrolab-0.1.6/pyproject.toml` & `py_astrolab-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.1.6"
+version = "0.2.0"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.1.6/PKG-INFO` & `py_astrolab-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.1.6
+Version: 0.2.0
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

