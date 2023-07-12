# Comparing `tmp/bestPR-0.6.7-py3-none-any.whl.zip` & `tmp/bestPR-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1904 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     1604 b- defN 23-Jul-12 07:39 bestPR/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-12 07:39 bestPR-0.6.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      167 b- defN 23-Jul-12 07:39 bestPR-0.6.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 07:39 bestPR-0.6.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-12 07:39 bestPR-0.6.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      455 b- defN 23-Jul-12 07:39 bestPR-0.6.7.dist-info/RECORD
-6 files, 2325 bytes uncompressed, 1074 bytes compressed:  53.8%
+Zip file size: 1928 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     1568 b- defN 23-Jul-12 07:40 bestPR/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-12 07:44 bestPR-0.6.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      288 b- defN 23-Jul-12 07:44 bestPR-0.6.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 07:44 bestPR-0.6.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-12 07:44 bestPR-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      455 b- defN 23-Jul-12 07:44 bestPR-0.6.9.dist-info/RECORD
+6 files, 2410 bytes uncompressed, 1098 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: bestPR/__init__.py
 Comment: 
 
-Filename: bestPR-0.6.7.dist-info/LICENSE.txt
+Filename: bestPR-0.6.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: bestPR-0.6.7.dist-info/METADATA
+Filename: bestPR-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: bestPR-0.6.7.dist-info/WHEEL
+Filename: bestPR-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: bestPR-0.6.7.dist-info/top_level.txt
+Filename: bestPR-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bestPR-0.6.7.dist-info/RECORD
+Filename: bestPR-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestPR/__init__.py

```diff
@@ -1,38 +1,42 @@
-# -*- coding: utf-8 -*-
+#Libraries
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
+from sklearn.metrics import mean_squared_error, mean_absolute_error
 from sklearn.linear_model import Lasso
 from sklearn.preprocessing import StandardScaler
 
 class polyBest:
     def __init__(data, X, y, param, split, scale):
         data.X = X
         data.y = y
         data.param=param
         data.split=split
         data.scale = scale
 
         data.msescore=[]
         data.maescore=[]
+        
         X_train, X_test, y_train, y_test = train_test_split(data.X, data.y, test_size = data.split)
+        
         if(scale):
             scaler = StandardScaler()
             X_train = scaler.fit_transform(X_train)
             X_test = scaler.transform(X_test)
+        
         for i in range(len(data.param)):
-            print("h")
+            
             polynomial_features= PolynomialFeatures(degree=i+1)
             X_train_trf = polynomial_features.fit_transform(X_train)
             X_test_trf = polynomial_features.fit_transform(X_test)
+            
             lasso1=Lasso(alpha=data.param[i])
             lasso1.fit(X_train_trf, y_train)
             y_predlasso1 = lasso1.predict(X_test_trf)
-            #Finding MSE of prediction with training target
+            
             err = mean_squared_error(y_predlasso1, y_test)
             data.msescore.append(err)
             err1 = mean_absolute_error(y_predlasso1, y_test)
             data.maescore.append(err1)
 
     def mseScore(data):
         return data.msescore
```

