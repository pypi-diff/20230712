# Comparing `tmp/Signal8-4.5.tar.gz` & `tmp/Signal8-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.5.tar", last modified: Fri Jun 30 20:07:50 2023, max compression
+gzip compressed data, was "Signal8-4.6.tar", last modified: Wed Jul 12 17:50:29 2023, max compression
```

## Comparing `Signal8-4.5.tar` & `Signal8-4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:50.901990 Signal8-4.5/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.5/LICENSE
--rw-rw-rw-   0        0        0     4769 2023-06-30 20:07:50.899988 Signal8-4.5/PKG-INFO
--rw-rw-rw-   0        0        0     4271 2023-06-22 19:39:26.000000 Signal8-4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:50.839987 Signal8-4.5/Signal8/
--rw-rw-rw-   0        0        0    12400 2023-06-30 19:02:52.000000 Signal8-4.5/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.5/Signal8/__init__.py
--rw-rw-rw-   0        0        0      208 2023-06-30 18:57:45.000000 Signal8-4.5/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:50.894987 Signal8-4.5/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.5/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.5/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.5/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.5/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11954 2023-06-30 18:56:28.000000 Signal8-4.5/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.5/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:50.861988 Signal8-4.5/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4769 2023-06-30 20:07:50.000000 Signal8-4.5/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-30 20:07:50.000000 Signal8-4.5/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 20:07:50.000000 Signal8-4.5/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 20:07:50.000000 Signal8-4.5/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 20:07:50.902990 Signal8-4.5/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-30 20:06:14.000000 Signal8-4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.731246 Signal8-4.6/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.6/LICENSE
+-rw-rw-rw-   0        0        0     4768 2023-07-12 17:50:29.729246 Signal8-4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.652247 Signal8-4.6/Signal8/
+-rw-rw-rw-   0        0        0    12543 2023-07-12 17:48:53.000000 Signal8-4.6/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.6/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-07-09 23:27:47.000000 Signal8-4.6/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.724248 Signal8-4.6/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.6/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.6/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.6/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.6/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11954 2023-06-30 18:56:28.000000 Signal8-4.6/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.6/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.695245 Signal8-4.6/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4768 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:50:29.732245 Signal8-4.6/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-07-12 17:49:09.000000 Signal8-4.6/setup.py
```

### Comparing `Signal8-4.5/LICENSE` & `Signal8-4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.5/PKG-INFO` & `Signal8-4.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.5
+Version: 4.6
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -47,22 +47,22 @@
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :---------------: | :--------------------------------------------: |
-| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
-|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
+|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
 |   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
-|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
-|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
+| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
+|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
+| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
+| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
```

### Comparing `Signal8-4.5/README.md` & `Signal8-4.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :---------------: | :--------------------------------------------: |
-| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
-|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
+|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
 |   ``corners``    | ![1686604788813](image/README/1686604788813.png) |
-|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
-|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
+| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
+|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
+| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
+| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
```

### Comparing `Signal8-4.5/Signal8/Signal8.py` & `Signal8-4.6/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,22 @@
     # Get constraints on entities given problem instance name
     def _set_problem_instance(self, world, instance_name):
         instance_constr = get_problem_instance(instance_name)
         world.problem_instance = instance_name
         world.instance_constr = instance_constr
     
     # Generate valid points according to some condition
-    def _generate_position(self, np_random, condition, circle=False):
+    def _generate_position(self, np_random, condition, circle=False, bounds=(-1, 1)):
         while True:
             if circle:
                 theta = np_random.uniform(0, 2*np.pi)
                 r = 0.5 * np.sqrt(np_random.uniform(0, 1))
                 point = np.array([r * np.cos(theta), r * np.sin(theta)])
             else:
-                point = np_random.uniform(-1, +1, 2)
+                point = np_random.uniform(bounds[0], bounds[1], 2)  # use the bounds here
             if condition(point):
                 break
         return point
 
     # Check if point is outside of triangular obstacle regions
     def _outside_triangle(self, point, paths, epsilon):
         enlarged_paths = []
@@ -146,38 +146,39 @@
                     y_constraints=y_constraints,
                     epsilon=epsilon, 
                     )
 
             agent.state.p_pos = self._generate_position(np_random, condition)
             agent.goal.state.p_pos = self._generate_position(np_random, condition)
     
-    # Reset all large obstacles to a position that does not intersect with the agents and is within its shape
+    # Reset all large obstacles to a position that does not intersect with the agents and is within its shape                
     def _reset_large_obstacles(self, world, np_random, paths):
         def inside_shape_condition(point):
             return any(path.contains_points(point[None, :]) for path in paths)    
-        
+
         occupied = set()
         num_shapes = len(world.instance_constr)
         circle = True if world.problem_instance in ['circle', 'solar_system'] else False    
-        
+        radius = world.large_obstacles[0].size  # get the radius of the obstacle
+
         for i, large_obstacle in enumerate(world.large_obstacles):            
             large_obstacle.state.p_vel = np.zeros(world.dim_p)
-            
+
             while True:
-                pos = self._generate_position(np_random, inside_shape_condition, circle=circle)
+                pos = self._generate_position(np_random, inside_shape_condition, circle=circle, bounds=(-1+radius, 1-radius))  # adjust the bounds here
                 shape_idx = next((i for i, path in enumerate(paths) if path.contains_points(pos[None, :])), None)
-                
+
                 if i % num_shapes == 0:
                     occupied.clear()
-                
+
                 if shape_idx not in occupied:
                     large_obstacle.state.p_pos = pos
                     occupied.add(shape_idx)
                     break
-    
+
     def _reset_small_obstacles(self, world, np_random, paths):
         epsilon = world.small_obstacles[0].size + world.large_obstacles[0].size
 
         agent_positions = [agent.state.p_pos for agent in world.agents]
         goal_positions = [goal.state.p_pos for goal in world.goals]
         large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
```

### Comparing `Signal8-4.5/Signal8/utils/core.py` & `Signal8-4.6/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.5/Signal8/utils/problems.py` & `Signal8-4.6/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.5/Signal8/utils/simple_env.py` & `Signal8-4.6/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.5/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.6/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.5/Signal8.egg-info/PKG-INFO` & `Signal8-4.6/Signal8.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.5
+Version: 4.6
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -47,22 +47,22 @@
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :---------------: | :--------------------------------------------: |
-| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
-|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
+|    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
 |   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
-|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
-|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
-|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
+| ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
+|   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
+| ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
+| ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
```

### Comparing `Signal8-4.5/setup.py` & `Signal8-4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.5",
+    version="4.6",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

