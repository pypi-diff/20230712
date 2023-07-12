# Comparing `tmp/progf-0.0.4-py3-none-any.whl.zip` & `tmp/progf-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17426 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-12 11:00 Project/__init__.py
+Zip file size: 17436 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-12 13:49 Project/__init__.py
 -rw-rw-rw-  2.0 fat      246 b- defN 23-Jun-17 02:27 Project/drawable.py
--rw-rw-rw-  2.0 fat    23720 b- defN 23-Jul-12 10:59 Project/games.py
+-rw-rw-rw-  2.0 fat    23728 b- defN 23-Jul-12 13:49 Project/games.py
 -rw-rw-rw-  2.0 fat     1680 b- defN 23-Jul-12 11:04 Project/object.py
 -rw-rw-rw-  2.0 fat    24283 b- defN 23-Jul-12 10:59 Project/project.py
 -rw-rw-rw-  2.0 fat    12216 b- defN 23-Jun-15 10:02 Project/project_image.jpg
 -rw-rw-rw-  2.0 fat     2079 b- defN 23-Jun-15 10:40 Project/sound.py
 -rw-rw-rw-  2.0 fat      851 b- defN 23-Jun-15 12:00 Project/standard.py
--rw-rw-rw-  2.0 fat      421 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      892 b- defN 23-Jul-12 11:05 progf-0.0.4.dist-info/RECORD
-12 files, 66509 bytes uncompressed, 15954 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat      421 b- defN 23-Jul-12 13:50 progf-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 13:50 progf-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-12 13:50 progf-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      892 b- defN 23-Jul-12 13:50 progf-0.0.5.dist-info/RECORD
+12 files, 66517 bytes uncompressed, 15964 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: Project/sound.py
 Comment: 
 
 Filename: Project/standard.py
 Comment: 
 
-Filename: progf-0.0.4.dist-info/METADATA
+Filename: progf-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: progf-0.0.4.dist-info/WHEEL
+Filename: progf-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: progf-0.0.4.dist-info/top_level.txt
+Filename: progf-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: progf-0.0.4.dist-info/RECORD
+Filename: progf-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Project/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.4'
+__version__ = '0.0.5'
```

## Project/games.py

```diff
@@ -574,14 +574,14 @@
                 standard.Input.PressOut("MOUSE_UP")
             if event.button == 5:
                 standard.Input.PressOut("MOUSE_DOWN")
     standard.Input.mouse_pos = project.Vector2(pygame.mouse.get_pos()[0], pygame.mouse.get_pos()[1])
     if type(standard.Game.scenes[standard.Game.now].back) == drawable.Color:
         standard.Game.screen.fill(standard.Game.scenes[standard.Game.now].back.color)
     else:
-        standard.Game.screen.blit(standard.Game.scenes[standard.Game.now].back.image)
+        standard.Game.screen.blit(standard.Game.scenes[standard.Game.now].back.image, (0, 0))
     standard.Game.update()
     standard.Input.init()
     standard.Time.update()
     standard.Frame.fps_pls()
     standard.Frame.fps_check()
     pygame.display.flip()
```

