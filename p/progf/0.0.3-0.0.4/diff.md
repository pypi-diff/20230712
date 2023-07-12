# Comparing `tmp/progf-0.0.3-py3-none-any.whl.zip` & `tmp/progf-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17413 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-17 01:45 Project/__init__.py
--rw-rw-rw-  2.0 fat      388 b- defN 23-Jun-15 11:30 Project/drawable.py
--rw-rw-rw-  2.0 fat    23608 b- defN 23-Jun-17 00:46 Project/games.py
--rw-rw-rw-  2.0 fat     1670 b- defN 23-Jun-17 01:00 Project/object.py
--rw-rw-rw-  2.0 fat    24281 b- defN 23-Jun-15 11:30 Project/project.py
+Zip file size: 17426 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-12 11:00 Project/__init__.py
+-rw-rw-rw-  2.0 fat      246 b- defN 23-Jun-17 02:27 Project/drawable.py
+-rw-rw-rw-  2.0 fat    23720 b- defN 23-Jul-12 10:59 Project/games.py
+-rw-rw-rw-  2.0 fat     1680 b- defN 23-Jul-12 11:04 Project/object.py
+-rw-rw-rw-  2.0 fat    24283 b- defN 23-Jul-12 10:59 Project/project.py
 -rw-rw-rw-  2.0 fat    12216 b- defN 23-Jun-15 10:02 Project/project_image.jpg
 -rw-rw-rw-  2.0 fat     2079 b- defN 23-Jun-15 10:40 Project/sound.py
 -rw-rw-rw-  2.0 fat      851 b- defN 23-Jun-15 12:00 Project/standard.py
--rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-17 02:05 progf-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 02:05 progf-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 02:05 progf-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      892 b- defN 23-Jun-17 02:05 progf-0.0.3.dist-info/RECORD
-12 files, 66527 bytes uncompressed, 15941 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat      421 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      892 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/RECORD
+12 files, 66509 bytes uncompressed, 15954 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: Project/sound.py
 Comment: 
 
 Filename: Project/standard.py
 Comment: 
 
-Filename: progf-0.0.3.dist-info/METADATA
+Filename: progf-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: progf-0.0.3.dist-info/WHEEL
+Filename: progf-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: progf-0.0.3.dist-info/top_level.txt
+Filename: progf-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: progf-0.0.3.dist-info/RECORD
+Filename: progf-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Project/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.1'
+__version__ = '0.0.4'
```

## Project/drawable.py

```diff
@@ -1,15 +1,12 @@
 import pygame
 
 
 class Image:
     def __init__(self, image, size):
-        self.image = pygame.transform.scale(pygame.image.load(image), size)
+        self.image = pygame.image.load(image)
         self.size = size
 
-    def update(self):
-        self.image = pygame.transform.scale(pygame.image.load(self.image), self.size)
-
 
 class Color:
     def __init__(self, red, green, blue):
         self.color = (red, green, blue)
```

## Project/games.py

```diff
@@ -1,12 +1,13 @@
 import pygame
 
 import Project.project as project
 import Project.standard as standard
 import Project.drawable as drawable
+import gamgam.Center
 
 def KEYPRESSEVENT(gameEvent):
     if gameEvent.key == pygame.K_a:
         standard.Input.Press("A")
     elif gameEvent.key == pygame.K_b:
         standard.Input.Press("B")
     elif gameEvent.key == pygame.K_c:
@@ -576,8 +577,11 @@
     standard.Input.mouse_pos = project.Vector2(pygame.mouse.get_pos()[0], pygame.mouse.get_pos()[1])
     if type(standard.Game.scenes[standard.Game.now].back) == drawable.Color:
         standard.Game.screen.fill(standard.Game.scenes[standard.Game.now].back.color)
     else:
         standard.Game.screen.blit(standard.Game.scenes[standard.Game.now].back.image)
     standard.Game.update()
     standard.Input.init()
+    standard.Time.update()
+    standard.Frame.fps_pls()
+    standard.Frame.fps_check()
     pygame.display.flip()
```

## Project/object.py

```diff
@@ -29,27 +29,27 @@
         self.components = []
         self.back = back
 
     def start(self):
         pass
 
     def update(self):
-        self.back.update()
         self.show()
         for i in self.components:
             i.update()
 
     def end(self):
         pass
 
     def show(self):
-        self.back.image = pygame.transform.rotate(self.back.image, self.transform.rotation)
-        rect = self.back.image.get_rect()
+        image = pygame.transform.scale(self.back.image, self.back.size)
+        image = pygame.transform.rotozoom(image, self.transform.rotation, 1)
+        rect = image.get_rect()
         rect.center = (self.transform.position.x, self.transform.position.y)
-        standard.Game.screen.blit(self.back.image, rect)
+        standard.Game.screen.blit(image, rect)
 
     def set_component(self, component):
         self.components.append(component)
         component.now = self
         component.start()
```

## Project/project.py

```diff
@@ -271,15 +271,15 @@
                     i[1] = time() / 1000000
 
             for i in self.invokes:
                 if i[0].count == i[1]:
                     self.del_function(i[0].name)
             for i in range(len(self.timers)):
                 if self.timers[i][0] <= 0:
-                    self.del_timer(i)
+                    self.stop_timer(i)
         else:
             now = time() / 1000000
             for i in self.invokes:
                 if i[0].state == 1:
                     if now - i[0].time >= i[0].num:
                         i[0].function()
                         i[0].time = time() / 1000000
@@ -290,15 +290,15 @@
                     i[1] = time() / 1000000
 
             for i in self.invokes:
                 if i[0].count == i[1]:
                     self.del_function(i[0].name)
             for i in range(len(self.timers)):
                 if self.timers[i][0] <= 0:
-                    self.del_timer(i)
+                    self.stop_timer(i)
 
 
 class Function:
     def __init__(self, name, function, time, num, count):
         self.name = name
         self.function = function
         self.time = time
```

## Comparing `progf-0.0.3.dist-info/RECORD` & `progf-0.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Project/__init__.py,sha256=07NzQXBgNlnw5kSN6ZYxE9By-_RuH3Jyy58Z74sIio0,21
-Project/drawable.py,sha256=7wFg1S8dC9A_xRAT30zTzlyl8IvdcjP81ukeGXJ0QL4,388
-Project/games.py,sha256=-CPdOteT0s_3LmIMXeNoLb8FCI9qjCgehjPwkxJwRSE,23608
-Project/object.py,sha256=k2DqvMf7gPq0i3fCRpQQ9LNDTjvdLkQ0NiacEHOV4nQ,1670
-Project/project.py,sha256=RyLR4-iYzKddD0ZUj3K1hM81LLfOcgzUn9id5HbF-Bc,24281
+Project/__init__.py,sha256=Qkdiz6Ybn1PE1SlWhKAQBmETf7pQ0yr5HmkqLVDxsqE,21
+Project/drawable.py,sha256=CZLrMdOVPuRZKUjcGbwV1pTZ2o34jeKVyFzIVpXIH98,246
+Project/games.py,sha256=Pb0E1YvHAKdXByOZZOKs3mt0it69jibPW_iSXOaIBW8,23720
+Project/object.py,sha256=qI-1wO6oDllic2mJJ7WkhrPAc5FgzMqsxp2sdolsv0E,1680
+Project/project.py,sha256=j4BgXD8Hf_Xp3ouppdjV7_w1txOJ3NxiPD36HkFZcCg,24283
 Project/project_image.jpg,sha256=enqA2lv7tmLTAE983Z5JIM2nHQ5jEowcVbI5ZO9kSgI,12216
 Project/sound.py,sha256=_4ZHfFBtr7UkSM0ke-OTrCQJmMqvrf0tu4mNvheICGA,2079
 Project/standard.py,sha256=iyL1DYspb9JnN0phHk2NMJ5dN3wY39QvVvCNvMcqXrA,851
-progf-0.0.3.dist-info/METADATA,sha256=5_XqtXdivBb1v_Ozhpt7dGokhv-9GQ6LfI6TjCahcZ8,421
-progf-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-progf-0.0.3.dist-info/top_level.txt,sha256=ffhzYv37LT3D__gNgNQkVZzA105DtjzlATiBjvDSmwU,8
-progf-0.0.3.dist-info/RECORD,,
+progf-0.0.4.dist-info/METADATA,sha256=J64u2JqEoH7IzdOnnnFjCW-ZntHylsea5KwMuDKrsyY,421
+progf-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+progf-0.0.4.dist-info/top_level.txt,sha256=ffhzYv37LT3D__gNgNQkVZzA105DtjzlATiBjvDSmwU,8
+progf-0.0.4.dist-info/RECORD,,
```

