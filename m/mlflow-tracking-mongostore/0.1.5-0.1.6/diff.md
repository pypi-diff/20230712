# Comparing `tmp/mlflow_tracking_mongostore-0.1.5-py3-none-any.whl.zip` & `tmp/mlflow_tracking_mongostore-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18222 bytes, number of entries: 9
+Zip file size: 18245 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_tracking_mongostore/__init__.py
--rw-r--r--  2.0 unx     9301 b- defN 23-Jul-09 10:10 mlflow_tracking_mongostore/models.py
+-rw-r--r--  2.0 unx     9406 b- defN 23-Jul-12 10:35 mlflow_tracking_mongostore/models.py
 -rw-r--r--  2.0 unx    43818 b- defN 23-Jul-08 17:57 mlflow_tracking_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1389 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/RECORD
-9 files, 67014 bytes uncompressed, 16660 bytes compressed:  75.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1389 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/RECORD
+9 files, 67119 bytes uncompressed, 16683 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mlflow_tracking_mongostore/models.py
 Comment: 
 
 Filename: mlflow_tracking_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/METADATA
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/WHEEL
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/entry_points.txt
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/top_level.txt
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.5.dist-info/RECORD
+Filename: mlflow_tracking_mongostore-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_tracking_mongostore/models.py

```diff
@@ -37,27 +37,28 @@
 RUN_COLLECTION_NAME = "mlflow_run"
 METRIC_COLLECTION_NAME = "mlflow_metric"
 
 
 def get_workspace_id():
     if request:
         if request.headers:
-            if request.headers:
-                return request.headers.get("Workspace-Id", None)
+            if "Workspace-Id" in request.headers:
+                return request.headers["Workspace-Id"]
     return None
 
 
 class CustomQuerySet(QuerySet):
     def __call__(self, q_obj=None, **query):
 
         q_obj = q_obj if q_obj else Q()
 
         # Combine the existing query with the new filter
         workspace_id = get_workspace_id()
-        if workspace_id:
+        if workspace_id is not None:
+            q_obj &= Q(mlflow_workspace_id__exists=True, mlflow_workspace_id__ne="")
             q_obj &= Q(mlflow_workspace_id=workspace_id)
 
         # call the super class's __call__ with the updated query.
         return super().__call__(q_obj, **query)
 
 
 def compare_attr(val1, comp, val2):
@@ -135,15 +136,15 @@
     exp_id = StringField(max_length=32, db_field="id")
     name = StringField(required=True, max_length=200)
     artifact_location = StringField(max_length=256)
     lifecycle_stage = StringField(max_length=50, default=LifecycleStage.ACTIVE)
     tags = ListField(EmbeddedDocumentField(MongoExperimentTag))
     creation_time = LongField()
     last_update_time = LongField()
-    mlflow_workspace_id = StringField(max_length=32)
+    mlflow_workspace_id = StringField(max_length=36)
 
     meta = {
         "collection": EXPERIMENT_COLLECTION_NAME,
         "strict": False,
         "queryset_class": CustomQuerySet,
     }
 
@@ -236,15 +237,15 @@
     source_version = StringField(max_length=50)
     lifecycle_stage = StringField(max_length=20, default=LifecycleStage.ACTIVE)
     artifact_uri = StringField(max_length=200)
 
     experiment_id = ReferenceField(
         "MongoExperiment", reverse_delete_rule=CASCADE, db_field="mlflow_experiment_id"
     )
-    mlflow_workspace_id = StringField(max_length=32)
+    mlflow_workspace_id = StringField(max_length=36)
 
     latest_metrics = ListField(EmbeddedDocumentField(MongoLatestMetric))
     params = ListField(EmbeddedDocumentField(MongoParam))
     # tags = ListField(EmbeddedDocumentField(MongoTag))
     tags = EmbeddedDocumentListField(MongoTag)
 
     meta = {"collection": RUN_COLLECTION_NAME, "queryset_class": CustomQuerySet}
```

## Comparing `mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE` & `mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_tracking_mongostore-0.1.5.dist-info/METADATA` & `mlflow_tracking_mongostore-0.1.6.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tracking-mongostore
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mlflow plugin to use MongoDB as backend for MLflow tracking service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
```

