# Comparing `tmp/apache-airflow-providers-amazon-8.3.0rc4.tar.gz` & `tmp/apache-airflow-providers-amazon-8.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.3.0rc4.tar", last modified: Sun Jul  9 15:40:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.3.1rc1.tar", last modified: Wed Jul 12 19:13:17 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.3.0rc4.tar` & `apache-airflow-providers-amazon-8.3.1rc1.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.516250 apache-airflow-providers-amazon-8.3.0rc4/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-09 15:39:54.000000 apache-airflow-providers-amazon-8.3.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-09 15:40:03.517204 apache-airflow-providers-amazon-8.3.0rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6037 2023-07-09 15:39:54.000000 apache-airflow-providers-amazon-8.3.0rc4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:01.867625 apache-airflow-providers-amazon-8.3.0rc4/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:01.876421 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.075846 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-07-09 14:42:13.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.093181 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.490370 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/chime.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.537448 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.561816 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.576552 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/notifications/chime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.794637 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    43203 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    65010 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    35538 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.813815 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:02.957256 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.206172 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8287 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.341201 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/athena.py
--rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/base.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     8898 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/ecs.py
--rw-r--r--   0 root         (0) root         (0)     8445 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    11320 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/rds.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/sagemaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.400725 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/waiter.py
--rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/waiter_with_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.469308 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/athena.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)    40337 2023-07-09 15:39:54.000000 apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:40:03.511734 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8503 2023-07-09 15:40:01.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-09 15:40:00.000000 apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2243 2023-07-09 15:40:03.520574 apache-airflow-providers-amazon-8.3.0rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-09 15:39:54.000000 apache-airflow-providers-amazon-8.3.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.707884 apache-airflow-providers-amazon-8.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-12 19:13:17.708447 apache-airflow-providers-amazon-8.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.125784 apache-airflow-providers-amazon-8.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.126911 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.182164 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-07-12 19:08:31.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.188540 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.325764 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.342697 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.351106 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.356727 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/chime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.428699 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    43203 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    65010 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    35538 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.437271 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.503549 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.562416 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8531 2023-07-12 12:42:21.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.602264 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     8898 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     8445 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    11320 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.643330 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.682364 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)    40358 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.705666 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-07-12 19:13:17.710325 apache-airflow-providers-amazon-8.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/LICENSE` & `apache-airflow-providers-amazon-8.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/MANIFEST.in` & `apache-airflow-providers-amazon-8.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/PKG-INFO` & `apache-airflow-providers-amazon-8.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.0rc4
+Version: 8.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -80,28 +80,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc4``
+Release: ``8.3.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,8 +158,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/README.rst` & `apache-airflow-providers-amazon-8.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc4``
+Release: ``8.3.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -110,8 +110,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.3.0"
+__version__ = "8.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/chime.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/notifications/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/notifications/chime.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,47 +115,54 @@
         self.redshift_data_api_kwargs = redshift_data_api_kwargs
 
         if self.redshift_data_api_kwargs:
             for arg in ["sql", "parameters"]:
                 if arg in self.redshift_data_api_kwargs.keys():
                     raise AirflowException(f"Cannot include param '{arg}' in Redshift Data API kwargs")
 
-    def _build_copy_query(self, copy_destination: str, credentials_block: str, copy_options: str) -> str:
+    def _build_copy_query(
+        self, copy_destination: str, credentials_block: str, region_info: str, copy_options: str
+    ) -> str:
         column_names = "(" + ", ".join(self.column_list) + ")" if self.column_list else ""
         return f"""
                     COPY {copy_destination} {column_names}
                     FROM 's3://{self.s3_bucket}/{self.s3_key}'
                     credentials
                     '{credentials_block}'
+                    {region_info}
                     {copy_options};
         """
 
     def execute(self, context: Context) -> None:
         if self.method not in AVAILABLE_METHODS:
             raise AirflowException(f"Method not found! Available methods: {AVAILABLE_METHODS}")
 
         redshift_hook: RedshiftDataHook | RedshiftSQLHook
         if self.redshift_data_api_kwargs:
             redshift_hook = RedshiftDataHook(aws_conn_id=self.redshift_conn_id)
         else:
             redshift_hook = RedshiftSQLHook(redshift_conn_id=self.redshift_conn_id)
         conn = S3Hook.get_connection(conn_id=self.aws_conn_id)
-
+        region_info = ""
+        if conn.extra_dejson.get("region", False):
+            region_info = f"region '{conn.extra_dejson['region']}'"
         if conn.extra_dejson.get("role_arn", False):
             credentials_block = f"aws_iam_role={conn.extra_dejson['role_arn']}"
         else:
             s3_hook = S3Hook(aws_conn_id=self.aws_conn_id, verify=self.verify)
             credentials = s3_hook.get_credentials()
             credentials_block = build_credentials_block(credentials)
 
         copy_options = "\n\t\t\t".join(self.copy_options)
         destination = f"{self.schema}.{self.table}"
         copy_destination = f"#{self.table}" if self.method == "UPSERT" else destination
 
-        copy_statement = self._build_copy_query(copy_destination, credentials_block, copy_options)
+        copy_statement = self._build_copy_query(
+            copy_destination, credentials_block, region_info, copy_options
+        )
 
         sql: str | Iterable[str]
 
         if self.method == "REPLACE":
             sql = ["BEGIN;", f"DELETE FROM {destination};", copy_statement, "COMMIT"]
         elif self.method == "UPSERT":
             if isinstance(redshift_hook, RedshiftDataHook):
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/athena.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/base.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/ecs.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/eks.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/rds.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/s3.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/utils/waiter_with_logging.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/athena.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/athena.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/batch.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/batch.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr-serverless.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.3.1",
             "8.3.0",
             "8.2.0",
             "8.1.0",
             "8.0.0",
             "7.4.1",
             "7.4.0",
             "7.3.0",
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.0rc4
+Version: 8.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -80,28 +80,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc4``
+Release: ``8.3.1rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -158,8 +158,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/pyproject.toml` & `apache-airflow-providers-amazon-8.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/setup.cfg` & `apache-airflow-providers-amazon-8.3.1rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -66,10 +66,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc4
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc4/setup.py` & `apache-airflow-providers-amazon-8.3.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.3.0"
+version = "8.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
```

