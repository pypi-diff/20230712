# Comparing `tmp/pso2keras-0.1.0-py3-none-any.whl.zip` & `tmp/pso2keras-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15668 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      208 b- defN 23-Jul-11 16:02 pso/__init__.py
--rw-rw-r--  2.0 unx    19700 b- defN 23-Jul-11 19:33 pso/optimizer.py
+Zip file size: 15628 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      135 b- defN 23-Jul-12 19:18 pso/__init__.py
+-rw-rw-r--  2.0 unx    19527 b- defN 23-Jul-12 19:11 pso/optimizer.py
 -rw-rw-r--  2.0 unx    18459 b- defN 23-Jul-09 14:46 pso/optimizer_target.py
 -rw-rw-r--  2.0 unx    10234 b- defN 23-Jul-06 13:57 pso/particle.py
--rw-rw-r--  2.0 unx     7772 b- defN 23-Jul-12 09:26 pso2keras-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-12 09:26 pso2keras-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-Jul-12 09:26 pso2keras-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      604 b- defN 23-Jul-12 09:26 pso2keras-0.1.0.dist-info/RECORD
-8 files, 57073 bytes uncompressed, 14628 bytes compressed:  74.4%
+-rw-rw-r--  2.0 unx     7838 b- defN 23-Jul-12 19:29 pso2keras-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-12 19:29 pso2keras-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-Jul-12 19:29 pso2keras-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      604 b- defN 23-Jul-12 19:29 pso2keras-0.1.1.dist-info/RECORD
+8 files, 56893 bytes uncompressed, 14588 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: pso/optimizer_target.py
 Comment: 
 
 Filename: pso/particle.py
 Comment: 
 
-Filename: pso2keras-0.1.0.dist-info/METADATA
+Filename: pso2keras-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pso2keras-0.1.0.dist-info/WHEEL
+Filename: pso2keras-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pso2keras-0.1.0.dist-info/top_level.txt
+Filename: pso2keras-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pso2keras-0.1.0.dist-info/RECORD
+Filename: pso2keras-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pso/__init__.py

```diff
@@ -1,11 +1,9 @@
 from .optimizer import Optimizer
 from .particle import Particle
-# from .optimizer_target import Optimizer_Target
 
-__version__ = '0.1.0'
+__version__ = "0.1.0"
 
 __all__ = [
-    'Optimizer',
-    'Particle',
-    # 'Optimizer_Target'
-]
+    "Optimizer",
+    "Particle",
+]
```

## pso/optimizer.py

```diff
@@ -10,18 +10,15 @@
 from tqdm import tqdm
 
 from .particle import Particle
 
 gpus = tf.config.experimental.list_physical_devices("GPU")
 if gpus:
     try:
-        # tf.config.experimental.set_visible_devices(gpus[0], "GPU")
-        # print(tf.config.experimental.get_visible_devices("GPU"))
         tf.config.experimental.set_memory_growth(gpus[0], True)
-        # print("set memory growth")
     except RuntimeError as e:
         print(e)
 
 
 class Optimizer:
     """
     particle swarm optimization
```

## Comparing `pso2keras-0.1.0.dist-info/METADATA` & `pso2keras-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pso2keras
-Version: 0.1.0
+Version: 0.1.1
 Summary: Particle Swarm Optimization to tensorflow package
 Home-page: https://github.com/jung-geun/PSO
 Author: pieroot
 Author-email: jgbong0306@gmail.com
 Keywords: pso,tensorflow,keras
-Requires-Python: >=3.8
+Requires-Python: ==3.8
 Description-Content-Type: text/markdown
-Requires-Dist: tqdm
+Requires-Dist: tqdm (==4.65.0)
+Requires-Dist: tensorflow (==2.11.0)
+Requires-Dist: keras (==2.11.0)
 Requires-Dist: numpy
-Requires-Dist: tensorflow
-Requires-Dist: keras
+Requires-Dist: pandas
+Requires-Dist: ipython
 
 # PSO 알고리즘 구현 및 새로운 시도
 
 pso 알고리즘을 사용하여 새로운 학습 방법을 찾는중 입니다
 병렬처리로 사용하는 논문을 찾아보았지만 이보다 더 좋은 방법이 있을 것 같아서 찾아보고 있습니다 - \[1]
 
 기본 pso 알고리즘의 수식은 다음과 같습니다
@@ -109,27 +111,27 @@
     c1=0.8,
     w_min=0.6,
     w_max=1.2,
     negative_swarm=0.1,
     mutation_swarm=0.2,
     particle_min=-3,
     particle_max=3,
-    )
+)
 
 best_score = pso_xor.fit(
     x_test,
     y_test,
     epochs=200,
     save=True,
     save_path="./result/xor",
     renewal="acc",
     empirical_balance=False,
     Dispersion=False,
     check_point=25,
-    )
+)
 
 ```
 
 위의 파라미터 기준 10 세대 근처부터 정확도가 100%가 나오는 것을 확인하였습니다
 ![xor](./history_plt/xor_2_10.png)
 
 2. iris 문제
@@ -192,15 +194,15 @@
     epochs=200,
     save=True,
     save_path="./result/mnist",
     renewal="acc",
     empirical_balance=False,
     Dispersion=False,
     check_point=25
-    )
+)
 ```
 
 위의 파라미터 기준 현재 정확도 43.38%를 보이고 있습니다
 ![mnist](./history_plt/mnist_mse_43.38.png)
 
 ### Trouble Shooting
```

## Comparing `pso2keras-0.1.0.dist-info/RECORD` & `pso2keras-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pso/__init__.py,sha256=DZKvY2yyNfsN7m9ACU8Zea0kBomalcFo1WjI7zPFIkg,208
-pso/optimizer.py,sha256=-rLCg06N25Gs6gG764j9A9M6lDttF_d4BR07tPt6kuQ,19700
+pso/__init__.py,sha256=gyZDIHWSLbMLW7AeO3W3lfdDI8RvIXrrCJ72-UB6LtI,135
+pso/optimizer.py,sha256=tBOUuXaUJiE99Sh5v1qES_4bO0mMRy6G7BgA-ZpE6EI,19527
 pso/optimizer_target.py,sha256=Q4c1dRe50Y05978VmGtfDlpPP8eshP4V0DnFWC3CfdA,18459
 pso/particle.py,sha256=52wfm3CkyqNQJWG2cJk-GcShjFHKVWYGLrzm6_b2RE0,10234
-pso2keras-0.1.0.dist-info/METADATA,sha256=TvAh0kq8rUSQ66MpLe7Py1GE76da5zPqQvYvnkYomIQ,7772
-pso2keras-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pso2keras-0.1.0.dist-info/top_level.txt,sha256=foX_ZxA6yk0xj45mTlvK0jYRIYGpFBZp7BuGq5wcPGc,4
-pso2keras-0.1.0.dist-info/RECORD,,
+pso2keras-0.1.1.dist-info/METADATA,sha256=e81pD-xpzbhBVthOjWJokpomXXZWN2K9CTCQbZnSvss,7838
+pso2keras-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pso2keras-0.1.1.dist-info/top_level.txt,sha256=foX_ZxA6yk0xj45mTlvK0jYRIYGpFBZp7BuGq5wcPGc,4
+pso2keras-0.1.1.dist-info/RECORD,,
```

