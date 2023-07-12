# Comparing `tmp/mpyl-1.0.7-py3-none-any.whl.zip` & `tmp/mpyl-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,91 +1,93 @@
-Zip file size: 136020 bytes, number of entries: 89
--rw-r--r--  2.0 unx      766 b- defN 23-Jul-03 10:09 mpyl/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Jul-03 10:09 mpyl/__main__.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-03 10:09 mpyl/constants.py
--rw-r--r--  2.0 unx    13948 b- defN 23-Jul-03 10:09 mpyl/project.py
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-03 10:09 mpyl/validation.py
--rw-r--r--  2.0 unx     2789 b- defN 23-Jul-03 10:09 mpyl/cli/__init__.py
--rw-r--r--  2.0 unx    11043 b- defN 23-Jul-03 10:09 mpyl/cli/build.py
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-03 10:09 mpyl/cli/health.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jul-03 10:09 mpyl/cli/meta_info.py
--rw-r--r--  2.0 unx     3853 b- defN 23-Jul-03 10:09 mpyl/cli/projects.py
--rw-r--r--  2.0 unx       34 b- defN 23-Jul-03 10:09 mpyl/cli/commands/__init__.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/__init__.py
--rw-r--r--  2.0 unx     3923 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/jenkins.py
--rw-r--r--  2.0 unx     5901 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/mpyl.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-03 10:09 mpyl/cli/commands/health/__init__.py
--rw-r--r--  2.0 unx     5535 b- defN 23-Jul-03 10:09 mpyl/cli/commands/health/checks.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-03 10:09 mpyl/cli/commands/projects/__init__.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-03 10:09 mpyl/cli/commands/projects/formatting.py
--rw-r--r--  2.0 unx      620 b- defN 23-Jul-03 10:09 mpyl/projects/__init__.py
--rw-r--r--  2.0 unx     2202 b- defN 23-Jul-03 10:09 mpyl/projects/find.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:09 mpyl/reporting/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/__init__.py
--rw-r--r--  2.0 unx     5213 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/markdown.py
--rw-r--r--  2.0 unx     1411 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/text.py
--rw-r--r--  2.0 unx     1139 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/__init__.py
--rw-r--r--  2.0 unx     8453 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/github.py
--rw-r--r--  2.0 unx     9331 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/jira.py
--rw-r--r--  2.0 unx     7997 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/slack.py
--rw-r--r--  2.0 unx     8433 b- defN 23-Jul-03 10:09 mpyl/schema/mpyl_config.schema.yml
--rw-r--r--  2.0 unx    25500 b- defN 23-Jul-03 10:09 mpyl/schema/project.schema.yml
--rw-r--r--  2.0 unx     2914 b- defN 23-Jul-03 10:09 mpyl/schema/run_properties.schema.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 10:09 mpyl/stages/__init__.py
--rw-r--r--  2.0 unx     3698 b- defN 23-Jul-03 10:09 mpyl/stages/discovery.py
--rw-r--r--  2.0 unx     6437 b- defN 23-Jul-03 10:09 mpyl/steps/__init__.py
--rw-r--r--  2.0 unx     1442 b- defN 23-Jul-03 10:09 mpyl/steps/collection.py
--rw-r--r--  2.0 unx     6085 b- defN 23-Jul-03 10:09 mpyl/steps/models.py
--rw-r--r--  2.0 unx     3505 b- defN 23-Jul-03 10:09 mpyl/steps/run.py
--rw-r--r--  2.0 unx     7278 b- defN 23-Jul-03 10:09 mpyl/steps/steps.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-03 10:09 mpyl/steps/build/__init__.py
--rw-r--r--  2.0 unx     2093 b- defN 23-Jul-03 10:09 mpyl/steps/build/docker_after_build.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Jul-03 10:09 mpyl/steps/build/dockerbuild.py
--rw-r--r--  2.0 unx      996 b- defN 23-Jul-03 10:09 mpyl/steps/build/echo.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Jul-03 10:09 mpyl/steps/build/sbt.py
--rw-r--r--  2.0 unx       60 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/__init__.py
--rw-r--r--  2.0 unx     2767 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
--rw-r--r--  2.0 unx     1196 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/echo.py
--rw-r--r--  2.0 unx     1472 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/ephemeral_docker_deploy.py
--rw-r--r--  2.0 unx     3896 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes.py
--rw-r--r--  2.0 unx     1588 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes_job.py
--rw-r--r--  2.0 unx     1571 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes_spark_job.py
--rw-r--r--  2.0 unx     3518 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/__init__.py
--rw-r--r--  2.0 unx    20536 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/chart.py
--rw-r--r--  2.0 unx     2989 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/helm.py
--rw-r--r--  2.0 unx     1732 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/rancher.py
--rw-r--r--  2.0 unx     4719 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/__init__.py
--rw-r--r--  2.0 unx      616 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/sealed_secret.py
--rw-r--r--  2.0 unx     5850 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/spark.py
--rw-r--r--  2.0 unx     2287 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/traefik.py
--rw-r--r--  2.0 unx   168371 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
--rw-r--r--  2.0 unx   151469 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
--rw-r--r--  2.0 unx    11703 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
--rw-r--r--  2.0 unx    42950 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-03 10:09 mpyl/steps/postdeploy/__init__.py
--rw-r--r--  2.0 unx     6496 b- defN 23-Jul-03 10:09 mpyl/steps/postdeploy/cypress_test.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jul-03 10:09 mpyl/steps/test/__init__.py
--rw-r--r--  2.0 unx     1560 b- defN 23-Jul-03 10:09 mpyl/steps/test/after_test.py
--rw-r--r--  2.0 unx     2596 b- defN 23-Jul-03 10:09 mpyl/steps/test/before_test.py
--rw-r--r--  2.0 unx     3886 b- defN 23-Jul-03 10:09 mpyl/steps/test/dockertest.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Jul-03 10:09 mpyl/steps/test/echo.py
--rw-r--r--  2.0 unx     5075 b- defN 23-Jul-03 10:09 mpyl/steps/test/sbt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 10:09 mpyl/utilities/__init__.py
--rw-r--r--  2.0 unx      768 b- defN 23-Jul-03 10:09 mpyl/utilities/cypress/__init__.py
--rw-r--r--  2.0 unx     6693 b- defN 23-Jul-03 10:09 mpyl/utilities/docker/__init__.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Jul-03 10:09 mpyl/utilities/github/__init__.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Jul-03 10:09 mpyl/utilities/jenkins/__init__.py
--rw-r--r--  2.0 unx     7903 b- defN 23-Jul-03 10:09 mpyl/utilities/jenkins/runner.py
--rw-r--r--  2.0 unx     1431 b- defN 23-Jul-03 10:09 mpyl/utilities/junit/__init__.py
--rw-r--r--  2.0 unx      254 b- defN 23-Jul-03 10:09 mpyl/utilities/logging/__init__.py
--rw-r--r--  2.0 unx      880 b- defN 23-Jul-03 10:09 mpyl/utilities/pyaml_env/__init__.py
--rw-r--r--  2.0 unx     7098 b- defN 23-Jul-03 10:09 mpyl/utilities/repo/__init__.py
--rw-r--r--  2.0 unx     4764 b- defN 23-Jul-03 10:09 mpyl/utilities/s3/__init__.py
--rw-r--r--  2.0 unx     1612 b- defN 23-Jul-03 10:09 mpyl/utilities/sbt/__init__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-Jul-03 10:09 mpyl/utilities/subprocess/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6083 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/RECORD
-89 files, 677646 bytes uncompressed, 123522 bytes compressed:  81.8%
+Zip file size: 210548 bytes, number of entries: 91
+-rw-r--r--  2.0 unx      766 b- defN 23-Jul-12 12:32 mpyl/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Jul-12 12:32 mpyl/__main__.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-12 12:32 mpyl/constants.py
+-rw-r--r--  2.0 unx    14810 b- defN 23-Jul-12 12:32 mpyl/project.py
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-12 12:32 mpyl/validation.py
+-rw-r--r--  2.0 unx     2789 b- defN 23-Jul-12 12:32 mpyl/cli/__init__.py
+-rw-r--r--  2.0 unx    11043 b- defN 23-Jul-12 12:32 mpyl/cli/build.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-12 12:32 mpyl/cli/health.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jul-12 12:32 mpyl/cli/meta_info.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-Jul-12 12:32 mpyl/cli/projects.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-12 12:32 mpyl/cli/commands/__init__.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jul-12 12:32 mpyl/cli/commands/build/__init__.py
+-rw-r--r--  2.0 unx     4287 b- defN 23-Jul-12 12:32 mpyl/cli/commands/build/jenkins.py
+-rw-r--r--  2.0 unx     6555 b- defN 23-Jul-12 12:32 mpyl/cli/commands/build/mpyl.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-12 12:32 mpyl/cli/commands/health/__init__.py
+-rw-r--r--  2.0 unx     5535 b- defN 23-Jul-12 12:32 mpyl/cli/commands/health/checks.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-12 12:32 mpyl/cli/commands/projects/__init__.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-12 12:32 mpyl/cli/commands/projects/formatting.py
+-rw-r--r--  2.0 unx      620 b- defN 23-Jul-12 12:32 mpyl/projects/__init__.py
+-rw-r--r--  2.0 unx     2202 b- defN 23-Jul-12 12:32 mpyl/projects/find.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 12:32 mpyl/reporting/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-12 12:32 mpyl/reporting/formatting/__init__.py
+-rw-r--r--  2.0 unx     5213 b- defN 23-Jul-12 12:32 mpyl/reporting/formatting/markdown.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Jul-12 12:32 mpyl/reporting/formatting/text.py
+-rw-r--r--  2.0 unx     1139 b- defN 23-Jul-12 12:32 mpyl/reporting/targets/__init__.py
+-rw-r--r--  2.0 unx     8453 b- defN 23-Jul-12 12:32 mpyl/reporting/targets/github.py
+-rw-r--r--  2.0 unx     9331 b- defN 23-Jul-12 12:32 mpyl/reporting/targets/jira.py
+-rw-r--r--  2.0 unx     7997 b- defN 23-Jul-12 12:32 mpyl/reporting/targets/slack.py
+-rw-r--r--  2.0 unx     8536 b- defN 23-Jul-12 12:32 mpyl/schema/mpyl_config.schema.yml
+-rw-r--r--  2.0 unx    25500 b- defN 23-Jul-12 12:32 mpyl/schema/project.schema.yml
+-rw-r--r--  2.0 unx     2928 b- defN 23-Jul-12 12:32 mpyl/schema/run_properties.schema.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 12:32 mpyl/stages/__init__.py
+-rw-r--r--  2.0 unx     3698 b- defN 23-Jul-12 12:32 mpyl/stages/discovery.py
+-rw-r--r--  2.0 unx     6437 b- defN 23-Jul-12 12:32 mpyl/steps/__init__.py
+-rw-r--r--  2.0 unx     1442 b- defN 23-Jul-12 12:32 mpyl/steps/collection.py
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-12 12:32 mpyl/steps/models.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-Jul-12 12:32 mpyl/steps/run.py
+-rw-r--r--  2.0 unx     7278 b- defN 23-Jul-12 12:32 mpyl/steps/steps.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-12 12:32 mpyl/steps/build/__init__.py
+-rw-r--r--  2.0 unx     2334 b- defN 23-Jul-12 12:32 mpyl/steps/build/docker_after_build.py
+-rw-r--r--  2.0 unx     3111 b- defN 23-Jul-12 12:32 mpyl/steps/build/dockerbuild.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jul-12 12:32 mpyl/steps/build/echo.py
+-rw-r--r--  2.0 unx     2573 b- defN 23-Jul-12 12:32 mpyl/steps/build/sbt.py
+-rw-r--r--  2.0 unx       60 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/__init__.py
+-rw-r--r--  2.0 unx     2767 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/echo.py
+-rw-r--r--  2.0 unx     1472 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/ephemeral_docker_deploy.py
+-rw-r--r--  2.0 unx     3896 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/kubernetes.py
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/kubernetes_job.py
+-rw-r--r--  2.0 unx     1571 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/kubernetes_spark_job.py
+-rw-r--r--  2.0 unx     3518 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/__init__.py
+-rw-r--r--  2.0 unx    21329 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/chart.py
+-rw-r--r--  2.0 unx     2989 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/helm.py
+-rw-r--r--  2.0 unx     1732 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/rancher.py
+-rw-r--r--  2.0 unx     4719 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/prometheus.py
+-rw-r--r--  2.0 unx      616 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/sealed_secret.py
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/spark.py
+-rw-r--r--  2.0 unx     2287 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/traefik.py
+-rw-r--r--  2.0 unx   582149 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/schema/monitoring.coreos.com_prometheuses.schema.yml
+-rw-r--r--  2.0 unx   168371 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
+-rw-r--r--  2.0 unx   151469 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
+-rw-r--r--  2.0 unx    11703 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+-rw-r--r--  2.0 unx    42950 b- defN 23-Jul-12 12:32 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-12 12:32 mpyl/steps/postdeploy/__init__.py
+-rw-r--r--  2.0 unx     8161 b- defN 23-Jul-12 12:32 mpyl/steps/postdeploy/cypress_test.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-12 12:32 mpyl/steps/test/__init__.py
+-rw-r--r--  2.0 unx     1560 b- defN 23-Jul-12 12:32 mpyl/steps/test/after_test.py
+-rw-r--r--  2.0 unx     2596 b- defN 23-Jul-12 12:32 mpyl/steps/test/before_test.py
+-rw-r--r--  2.0 unx     3886 b- defN 23-Jul-12 12:32 mpyl/steps/test/dockertest.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-12 12:32 mpyl/steps/test/echo.py
+-rw-r--r--  2.0 unx     5075 b- defN 23-Jul-12 12:32 mpyl/steps/test/sbt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 12:32 mpyl/utilities/__init__.py
+-rw-r--r--  2.0 unx      953 b- defN 23-Jul-12 12:32 mpyl/utilities/cypress/__init__.py
+-rw-r--r--  2.0 unx     6909 b- defN 23-Jul-12 12:32 mpyl/utilities/docker/__init__.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Jul-12 12:32 mpyl/utilities/github/__init__.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jul-12 12:32 mpyl/utilities/jenkins/__init__.py
+-rw-r--r--  2.0 unx     7903 b- defN 23-Jul-12 12:32 mpyl/utilities/jenkins/runner.py
+-rw-r--r--  2.0 unx     1431 b- defN 23-Jul-12 12:32 mpyl/utilities/junit/__init__.py
+-rw-r--r--  2.0 unx      254 b- defN 23-Jul-12 12:32 mpyl/utilities/logging/__init__.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Jul-12 12:32 mpyl/utilities/pyaml_env/__init__.py
+-rw-r--r--  2.0 unx     7342 b- defN 23-Jul-12 12:32 mpyl/utilities/repo/__init__.py
+-rw-r--r--  2.0 unx     4764 b- defN 23-Jul-12 12:32 mpyl/utilities/s3/__init__.py
+-rw-r--r--  2.0 unx     1612 b- defN 23-Jul-12 12:32 mpyl/utilities/sbt/__init__.py
+-rw-r--r--  2.0 unx     2326 b- defN 23-Jul-12 12:32 mpyl/utilities/subprocess/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6083 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8090 b- defN 23-Jul-12 12:33 mpyl-1.0.8.dist-info/RECORD
+91 files, 1267826 bytes uncompressed, 197640 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -159,23 +159,29 @@
 
 Filename: mpyl/steps/deploy/k8s/rancher.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/__init__.py
 Comment: 
 
+Filename: mpyl/steps/deploy/k8s/resources/prometheus.py
+Comment: 
+
 Filename: mpyl/steps/deploy/k8s/resources/sealed_secret.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/spark.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/traefik.py
 Comment: 
 
+Filename: mpyl/steps/deploy/k8s/resources/schema/monitoring.coreos.com_prometheuses.schema.yml
+Comment: 
+
 Filename: mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
@@ -243,26 +249,26 @@
 
 Filename: mpyl/utilities/sbt/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/subprocess/__init__.py
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/LICENSE
+Filename: mpyl-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/METADATA
+Filename: mpyl-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/WHEEL
+Filename: mpyl-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/entry_points.txt
+Filename: mpyl-1.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/top_level.txt
+Filename: mpyl-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mpyl-1.0.7.dist-info/RECORD
+Filename: mpyl-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpyl/project.py

```diff
@@ -187,24 +187,51 @@
     def from_config(values: dict):
         if not values:
             return None
         return Probe(path=TargetProperty.from_config(values["path"]), values=values)
 
 
 @dataclass(frozen=True)
+class Alert:
+    name: str
+    expr: str
+    for_duration: str
+    description: str
+    severity: str
+
+    @staticmethod
+    def from_config(values: dict):
+        name = values.get("name")
+        expr = values.get("expr")
+        for_duration = values.get("forDuration")
+        description = values.get("description")
+        severity = values.get("severity")
+        if not name or not expr or not for_duration or not description or not severity:
+            raise KeyError(
+                "Alerts must have a name, expr, forDuration, description and severity set."
+            )
+        return Alert(name, expr, for_duration, description, severity)
+
+
+@dataclass(frozen=True)
 class Metrics:
     path: str
+    port: Optional[str]
     enabled: bool
+    alerts: list[Alert]
 
     @staticmethod
     def from_config(values: dict):
         if not values:
             return None
         return Metrics(
-            path=values.get("path", "/metrics"), enabled=values.get("enabled", False)
+            path=values.get("path", "/metrics"),
+            port=values.get("port", None),
+            enabled=values.get("enabled", False),
+            alerts=[Alert.from_config(v) for v in values.get("alerts", [])],
         )
 
 
 @dataclass(frozen=True)
 class Resources:
     instances: Optional[TargetProperty[int]]
     cpus: Optional[TargetProperty[float]]
```

## mpyl/cli/projects.py

```diff
@@ -11,14 +11,15 @@
 from . import (
     CliContext,
     CONFIG_PATH_HELP,
     create_console_logger,
     parse_config_from_supplied_location,
 )
 from .commands.projects.formatting import print_project
+from .commands.build.mpyl import find_build_set
 from ..constants import DEFAULT_CONFIG_FILE_NAME
 from ..project import validate_project, load_project, Project
 from ..utilities.pyaml_env import parse_config
 from ..utilities.repo import Repository, RepoConfig
 
 
 @dataclass
@@ -95,32 +96,52 @@
 @click.pass_obj
 def show_project(obj, name):
     print_project(
         obj.cli.repo, obj.cli.console, f"{name}/{Project.project_yaml_path()}"
     )
 
 
-@projects.command(help="Validate the yaml of found projects against their schema")
+@projects.command(help="Validate the yaml of changed projects against their schema")
+@click.option(
+    "--all",
+    "all_",
+    is_flag=True,
+    help="Validate all project yaml's, regardless of changes on branch",
+)
 @click.pass_obj
-def lint(obj: ProjectsContext):
-    found_projects = obj.cli.repo.find_projects(obj.filter)
+def lint(obj: ProjectsContext, all_):
+    project_paths = []
+    if all_:
+        project_paths = obj.cli.repo.find_projects(obj.filter)
+    else:
+        branch = obj.cli.repo.get_branch
+        changes = (
+            obj.cli.repo.changes_in_branch_including_local()
+            if branch
+            else obj.cli.repo.changes_in_merge_commit()
+        )
+        build_set = find_build_set(obj.cli.repo, changes, False)
+        for all_projects in build_set.values():
+            for project in all_projects:
+                project_paths.append(project.path)
+
     invalid = 0
     valid = 0
-    for project in found_projects:
+    for project_path in set(project_paths):
         try:
-            project_path = Path(obj.cli.repo.root_dir()) / Path(project)
-            with open(project_path, encoding="utf-8") as file:
+            path = Path(obj.cli.repo.root_dir()) / Path(project_path)
+            with open(path, encoding="utf-8") as file:
                 validate_project(file)
         except jsonschema.exceptions.ValidationError as exc:
-            obj.cli.console.print(f"❌ {project}: {exc.message}")
+            obj.cli.console.print(f"❌ {project_path}: {exc.message}")
             invalid += 1
         else:
             valid += 1
             if obj.cli.verbose:
-                obj.cli.console.print(f"✅ {project}")
+                obj.cli.console.print(f"✅ {project_path}")
     obj.cli.console.print(
         f"Validated {valid + invalid} projects. {valid} valid, {invalid} invalid"
     )
     if invalid > 0:
         click.get_current_context().exit(1)
```

## mpyl/cli/commands/build/__init__.py

```diff
@@ -5,17 +5,17 @@
 from enum import Enum
 
 from rich.console import Console
 
 
 @dataclass(frozen=True)
 class Sound(Enum):
-    SUCCESS = 'Glass.aiff'
-    FAILURE = 'Sosumi.aiff'
+    SUCCESS = "Glass.aiff"
+    FAILURE = "Sosumi.aiff"
 
 
 def play_sound(sound: Sound):
-    if shutil.which('afplay') is None:
+    if shutil.which("afplay") is None:
         Console().bell()
         return
 
-    os.system(f'afplay /System/Library/Sounds/{sound.value}')
+    os.system(f"afplay /System/Library/Sounds/{sound.value}")
```

## mpyl/cli/commands/build/jenkins.py

```diff
@@ -29,68 +29,103 @@
     follow: bool
     tag: Optional[str] = None
 
 
 def get_token(github_config: GithubConfig):
     if github_config.token:
         return github_config.token
-    return subprocess.run(['gh', 'auth', 'token'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                          check=True).stdout.decode('utf-8').strip()
+    return (
+        subprocess.run(
+            ["gh", "auth", "token"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            check=True,
+        )
+        .stdout.decode("utf-8")
+        .strip()
+    )
 
 
-def __get_pr_pipeline(config: dict, git_repo: Repository, pipeline: str, status: Status) -> Optional[Pipeline]:
+def __get_pr_pipeline(
+    config: dict, git_repo: Repository, pipeline: str, status: Status
+) -> Optional[Pipeline]:
     github_config = GithubConfig.from_config(config)
     github = Github(login_or_token=get_token(github_config))
 
     repo = github.get_repo(github_config.repository)
 
     branch = git_repo.get_branch
     if not branch:
-        status.console.log('Could not determine current branch')
+        status.console.log("Could not determine current branch")
         return None
 
     if git_repo.main_branch == branch:
-        status.console.log(f'On main branch ({branch}), cannot determine which PR to build')
+        status.console.log(
+            f"On main branch ({branch}), cannot determine which PR to build"
+        )
         return None
     try:
         pull = get_pr_for_branch(repo, branch)
-        return Pipeline(target=Target.PULL_REQUEST, tag=f'{pull.number}', url=pull.html_url, pipeline=pipeline,
-                        body=pull.body, jenkins_config=JenkinsConfig.from_config(config))
+        return Pipeline(
+            target=Target.PULL_REQUEST,
+            tag=f"{pull.number}",
+            url=pull.html_url,
+            pipeline=pipeline,
+            body=pull.body,
+            jenkins_config=JenkinsConfig.from_config(config),
+        )
     except ValueError as exc:
         status.console.log(exc)
         return None
 
 
 def run_jenkins(run_config: JenkinsRunParameters):
     log_console = Console(log_path=False, log_time=False)
-    with log_console.status('Fetching Github info.. [bright_blue]>gh pr view[/bright_blue]') as status:
+    with log_console.status(
+        "Fetching Github info.. [bright_blue]>gh pr view[/bright_blue]"
+    ) as status:
         config = run_config.config
 
         with Repository(RepoConfig.from_config(config)) as git_repo:
             try:
-                pipeline_info = Pipeline(
-                    target=Target.ACCEPTANCE, tag=run_config.tag, url="https://tag-url",
-                    pipeline=run_config.pipeline, body="",
-                    jenkins_config=JenkinsConfig.from_config(config)) if run_config.tag \
-                    else __get_pr_pipeline(config, git_repo, run_config.pipeline, status)
+                pipeline_info = (
+                    Pipeline(
+                        target=Target.ACCEPTANCE,
+                        tag=run_config.tag,
+                        url="https://tag-url",
+                        pipeline=run_config.pipeline,
+                        body="",
+                        jenkins_config=JenkinsConfig.from_config(config),
+                    )
+                    if run_config.tag
+                    else __get_pr_pipeline(
+                        config, git_repo, run_config.pipeline, status
+                    )
+                )
                 if not pipeline_info:
                     return
 
                 status.start()
-                status.update(f'Fetching Jenkins info for {pipeline_info.human_readable()} ...')
-
-                runner = JenkinsRunner(pipeline=pipeline_info,
-                                       jenkins=Jenkins(baseurl=JenkinsConfig.from_config(config).url,
-                                                       username=run_config.jenkins_user,
-                                                       password=run_config.jenkins_password),
-                                       status=status,
-                                       follow=run_config.follow,
-                                       verbose=run_config.verbose)
+                status.update(
+                    f"Fetching Jenkins info for {pipeline_info.human_readable()} ..."
+                )
+
+                runner = JenkinsRunner(
+                    pipeline=pipeline_info,
+                    jenkins=Jenkins(
+                        baseurl=JenkinsConfig.from_config(config).url,
+                        username=run_config.jenkins_user,
+                        password=run_config.jenkins_password,
+                    ),
+                    status=status,
+                    follow=run_config.follow,
+                    verbose=run_config.verbose,
+                )
                 runner.run(run_config.pipeline_parameters)
             except requests.ConnectionError:
                 play_sound(Sound.FAILURE)
-                status.console.log('⚠️ Could not connect. Are you on VPN?')
+                status.console.log("⚠️ Could not connect. Are you on VPN?")
             except Exception as exc:
-                status.console.print(Markdown(f'Unexpected exception: {exc}'))
+                status.console.print(Markdown(f"Unexpected exception: {exc}"))
                 if run_config.verbose:
                     status.console.print_exception()
                 raise exc
```

## mpyl/cli/commands/build/mpyl.py

```diff
@@ -10,14 +10,15 @@
 from rich.logging import RichHandler
 from rich.markdown import Markdown
 
 from ....project import load_project, Stage, Project
 from ....reporting.formatting.markdown import run_result_to_markdown
 from ....reporting.targets import Reporter
 from ....stages.discovery import for_stage, find_invalidated_projects_per_stage
+from ....steps.collection import StepsCollection
 from ....steps.models import RunProperties
 from ....steps.run import RunResult
 from ....steps.steps import Steps, ExecutionException
 from ....utilities.repo import Repository, RepoConfig, Revision
 
 
 @dataclass(frozen=True)
@@ -41,106 +42,157 @@
     run_config: MpylRunConfig
     parameters: MpylCliParameters
 
 
 FORMAT = "%(name)s  %(message)s"
 
 
-def get_build_plan(logger: logging.Logger, repo: Repository, mpyl_run_parameters: MpylRunParameters) -> RunResult:
+def get_build_plan(
+    logger: logging.Logger, repo: Repository, mpyl_run_parameters: MpylRunParameters
+) -> RunResult:
     params = mpyl_run_parameters.parameters
-    branch = repo.get_branch or mpyl_run_parameters.run_config.run_properties.versioning.branch
+    branch = (
+        repo.get_branch
+        or mpyl_run_parameters.run_config.run_properties.versioning.branch
+    )
     logger.info(f"Running with {params}")
     if branch:
         if repo.main_branch_pulled:
-            logger.info(f'Branch `{repo.main_branch}` already present locally. Skipping pull.')
+            logger.info(
+                f"Branch `{repo.main_branch}` already present locally. Skipping pull."
+            )
         else:
-            logger.info(f'Pulling `{repo.main_branch}` from {repo.get_remote_url}')
+            logger.info(f"Pulling `{repo.main_branch}` from {repo.get_remote_url}")
             pull_result = repo.pull_main_branch()
-            logger.info(f'Pulled `{pull_result[0].remote_ref_path.strip()}` to local')
-        changes = repo.changes_in_branch_including_local() if params.local else repo.changes_in_branch()
+            logger.info(f"Pulled `{pull_result[0].remote_ref_path.strip()}` to local")
+        changes = (
+            repo.changes_in_branch_including_local()
+            if params.local
+            else repo.changes_in_branch()
+        )
     else:
-        changes = repo.changes_in_tagged_commit(params.tag) if params.tag else repo.changes_in_merge_commit()
-    logger.debug(f'Changes: {changes}')
+        changes = (
+            repo.changes_in_tagged_commit(params.tag)
+            if params.tag
+            else repo.changes_in_merge_commit()
+        )
+    logger.debug(f"Changes: {changes}")
 
-    projects_per_stage: dict[Stage, set[Project]] = find_build_set(repo, changes, params.all)
-    return RunResult(run_properties=mpyl_run_parameters.run_config.run_properties, run_plan=projects_per_stage)
+    projects_per_stage: dict[Stage, set[Project]] = find_build_set(
+        repo, changes, params.all
+    )
+    return RunResult(
+        run_properties=mpyl_run_parameters.run_config.run_properties,
+        run_plan=projects_per_stage,
+    )
 
 
-def run_mpyl(mpyl_run_parameters: MpylRunParameters, reporter: Optional[Reporter]) -> RunResult:
+def run_mpyl(
+    mpyl_run_parameters: MpylRunParameters, reporter: Optional[Reporter]
+) -> RunResult:
     params = mpyl_run_parameters.parameters
     console_properties = mpyl_run_parameters.run_config.run_properties.console
-    console = Console(markup=False, width=None if params.local else console_properties.width, no_color=False,
-                      log_path=False, color_system='256')
+    console = Console(
+        markup=False,
+        width=None if params.local else console_properties.width,
+        no_color=False,
+        log_path=False,
+        color_system="256",
+    )
     logging.raiseExceptions = False
     logging.basicConfig(
-        level="DEBUG" if params.verbose else console_properties.log_level, format=FORMAT, datefmt="[%X]",
-        handlers=[RichHandler(markup=False, console=console, show_path=params.local)]
+        level="DEBUG" if params.verbose else console_properties.log_level,
+        format=FORMAT,
+        datefmt="[%X]",
+        handlers=[RichHandler(markup=False, console=console, show_path=params.local)],
     )
-    logger = logging.getLogger('mpyl')
+    logger = logging.getLogger("mpyl")
     try:
-        with Repository(RepoConfig.from_config(mpyl_run_parameters.run_config.config)) as repo:
-
+        with Repository(
+            RepoConfig.from_config(mpyl_run_parameters.run_config.config)
+        ) as repo:
             run_plan = get_build_plan(logger, repo, mpyl_run_parameters)
 
             if not run_plan.run_plan.items():
                 logger.info("Nothing to do. Exiting..")
                 return run_plan
 
             logger.info("Build plan:")
             console.print(Markdown(f"\n\n{run_result_to_markdown(run_plan)}"))
 
             run_result: RunResult = run_plan
             if reporter:
                 reporter.send_report(run_plan)
             try:
-                steps = Steps(logger=logger, properties=mpyl_run_parameters.run_config.run_properties)
-                run_result = run_build(run_plan, steps, reporter, mpyl_run_parameters.parameters.local)
+                steps = Steps(
+                    logger=logger,
+                    properties=mpyl_run_parameters.run_config.run_properties,
+                    steps_collection=StepsCollection(
+                        logger=logger, base_path="src" if params.local else None
+                    ),
+                )
+                run_result = run_build(
+                    run_plan, steps, reporter, mpyl_run_parameters.parameters.local
+                )
             except ValidationError as exc:
-                console.log(f'Schema validation failed {exc.message} at `{".".join(map(str, exc.path))}`')
+                console.log(
+                    f'Schema validation failed {exc.message} at `{".".join(map(str, exc.path))}`'
+                )
                 raise exc
             except ExecutionException as exc:
                 run_result.exception = exc
-                console.log(f'Exception during build execution: {exc}')
+                console.log(f"Exception during build execution: {exc}")
                 console.print_exception()
 
             console.print(Markdown(run_result_to_markdown(run_result)))
             return run_result
 
     except Exception as exc:
-        console.log(f'Unexpected exception: {exc}')
+        console.log(f"Unexpected exception: {exc}")
         console.print_exception()
         raise exc
 
 
-def find_build_set(repo: Repository, changes_in_branch: list[Revision], build_all: bool) -> dict[Stage, set[Project]]:
+def find_build_set(
+    repo: Repository, changes_in_branch: list[Revision], build_all: bool
+) -> dict[Stage, set[Project]]:
     project_paths = repo.find_projects()
-    all_projects = set(map(lambda p: load_project(Path(""), Path(p), False), project_paths))
+    all_projects = set(
+        map(lambda p: load_project(Path(""), Path(p), False), project_paths)
+    )
 
     if build_all:
-        return {Stage.BUILD: for_stage(all_projects, Stage.BUILD),
-                Stage.TEST: for_stage(all_projects, Stage.TEST),
-                Stage.DEPLOY: for_stage(all_projects, Stage.DEPLOY),
-                Stage.POST_DEPLOY: for_stage(all_projects, Stage.POST_DEPLOY)}
+        return {
+            Stage.BUILD: for_stage(all_projects, Stage.BUILD),
+            Stage.TEST: for_stage(all_projects, Stage.TEST),
+            Stage.DEPLOY: for_stage(all_projects, Stage.DEPLOY),
+            Stage.POST_DEPLOY: for_stage(all_projects, Stage.POST_DEPLOY),
+        }
 
     return find_invalidated_projects_per_stage(all_projects, changes_in_branch)
 
 
-def run_build(accumulator: RunResult, executor: Steps, reporter: Optional[Reporter] = None, dry_run: bool = True):
+def run_build(
+    accumulator: RunResult,
+    executor: Steps,
+    reporter: Optional[Reporter] = None,
+    dry_run: bool = True,
+):
     try:
         for stage, projects in accumulator.run_plan.items():
             for proj in projects:
                 result = executor.execute(stage, proj, dry_run)
                 accumulator.append(result)
                 if reporter:
                     reporter.send_report(accumulator)
 
                 if not result.output.success and stage == Stage.DEPLOY:
-                    logging.warning(f'Deployment failed for {proj.name}')
+                    logging.warning(f"Deployment failed for {proj.name}")
                     return accumulator
 
             if accumulator.failed_result:
-                logging.warning(f'One of the builds failed at {stage}')
+                logging.warning(f"One of the builds failed at {stage}")
                 return accumulator
         return accumulator
     except ExecutionException as exc:
         accumulator.exception = exc
         return accumulator
```

## mpyl/schema/mpyl_config.schema.yml

```diff
@@ -69,14 +69,17 @@
         description: 'Path to cypress source code'
       recordKey:
         type: string
         description: 'Key for recording runs to cypress dashboard'
       kubectlConfigPath:
         type: string
         description: 'Path to kubectl config file'
+      ciBuildId:
+        type: [ string, null ]
+        description: 'Build id for cypress dashboard'
     required:
       - cypressSourceCodePath
   Kubernetes:
     type: object
     additionalProperties: false
     properties:
       rancher:
@@ -334,8 +337,8 @@
     properties:
       accessKeyId:
         type: string
       secretAccessKey:
         type: string
     required:
       - accessKeyId
-      - secretAccessKey
+      - secretAccessKey
```

## mpyl/schema/run_properties.schema.yml

```diff
@@ -51,15 +51,15 @@
         description: defines the run properties
         type: object
         additionalProperties: false
         properties:
           deploy_target:
             description: The deploy target.
             type: ["string", "null"]
-            enum: [ null,  'PullRequest', 'PullRequestBase', 'Production' ]
+            enum: [ null,  'PullRequest', 'PullRequestBase', 'Acceptance', 'Production' ]
       console:
         type: object
         additionalProperties: false
         properties:
           width:
             description: "The width of the console in characters, 0 means no limit"
             type: integer
```

## mpyl/steps/models.py

```diff
@@ -121,15 +121,15 @@
         )
         console = ConsoleProperties.from_configuration(build)
 
         return RunProperties(
             details=RunContext.from_configuration(build["run"]),
             target=Target(
                 build["parameters"].get("deploy_target", None)
-                or Target.PULL_REQUEST.value
+                or Target.PULL_REQUEST.value  # pylint: disable=no-member
             ),
             versioning=versioning,
             config=config,
             console=console,
         )
```

## mpyl/steps/build/docker_after_build.py

```diff
@@ -9,43 +9,61 @@
 from .. import Step, Meta
 from ..models import Input, Output, Artifact, ArtifactType
 from ...project import Stage
 from ...utilities.docker import DockerConfig, login
 
 
 class AfterBuildDocker(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='After Docker Build',
-            description='Push docker image to registry',
-            version='0.0.1',
-            stage=Stage.BUILD
-        ), ArtifactType.DOCKER_IMAGE, ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="After Docker Build",
+                description="Push docker image to registry",
+                version="0.0.1",
+                stage=Stage.BUILD,
+            ),
+            ArtifactType.DOCKER_IMAGE,
+            ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         built_image = step_input.required_artifact
         if not built_image:
             self._logger.warn("After docker has image required artifact")
-            return Output(success=False, message=f"After docker has image required artifact {step_input.project.name}")
+            return Output(
+                success=False,
+                message=f"After docker has image required artifact {step_input.project.name}",
+            )
 
-        image_name = built_image.spec['image']
-        self._logger.debug(f'Image to publish: {image_name}')
+        image_name = built_image.spec["image"]
+        self._logger.debug(f"Image to publish: {image_name}")
 
         docker_config = DockerConfig.from_dict(step_input.run_properties.config)
 
         full_image_path = os.path.join(docker_config.host_name, image_name)
-        artifact = Artifact(ArtifactType.DOCKER_IMAGE, step_input.run_properties.versioning.revision, self.meta.name,
-                            {'image': full_image_path})
+        artifact = Artifact(
+            ArtifactType.DOCKER_IMAGE,
+            step_input.run_properties.versioning.revision,
+            self.meta.name,
+            {"image": full_image_path},
+        )
 
         if step_input.dry_run:
-            return Output(success=True, message=f"Dry run. Not pushing {image_name} to {docker_config.host_name}",
-                          produced_artifact=artifact)
+            return Output(
+                success=True,
+                message=f"Dry run. Not pushing {image_name} to {docker_config.host_name}",
+                produced_artifact=artifact,
+            )
 
         login(logger=self._logger, docker_config=docker_config)
         image = docker.image.inspect(image_name)
-        self._logger.debug(f'Found image {image}')
+        self._logger.debug(f"Found image {image}")
         docker.image.tag(image, full_image_path)
 
         docker.image.push(full_image_path, quiet=False)
 
-        return Output(success=True, message=f"Pushed {full_image_path}", produced_artifact=artifact)
+        return Output(
+            success=True,
+            message=f"Pushed {full_image_path}",
+            produced_artifact=artifact,
+        )
```

## mpyl/steps/build/dockerbuild.py

```diff
@@ -21,50 +21,75 @@
 from logging import Logger
 
 from .docker_after_build import AfterBuildDocker
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...constants import BUILD_ARTIFACTS_FOLDER
 from ...project import Stage
-from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, login
+from ...utilities.docker import (
+    DockerConfig,
+    build,
+    docker_image_tag,
+    docker_file_path,
+    login,
+)
 
-DOCKER_IGNORE_DEFAULT = ['**/target/*', f'**/{BUILD_ARTIFACTS_FOLDER}/*']
+DOCKER_IGNORE_DEFAULT = ["**/target/*", f"**/{BUILD_ARTIFACTS_FOLDER}/*"]
 
 
 class BuildDocker(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger=logger, meta=Meta(
-            name='Docker Build',
-            description='Build docker image',
-            version='0.0.1',
-            stage=Stage.BUILD
-        ), produced_artifact=ArtifactType.DOCKER_IMAGE, required_artifact=ArtifactType.NONE,
-                         after=AfterBuildDocker(logger=logger))
+        super().__init__(
+            logger=logger,
+            meta=Meta(
+                name="Docker Build",
+                description="Build docker image",
+                version="0.0.1",
+                stage=Stage.BUILD,
+            ),
+            produced_artifact=ArtifactType.DOCKER_IMAGE,
+            required_artifact=ArtifactType.NONE,
+            after=AfterBuildDocker(logger=logger),
+        )
 
     def execute(self, step_input: Input) -> Output:
         docker_config = DockerConfig.from_dict(step_input.run_properties.config)
         build_target = docker_config.build_target
         if not build_target:
-            raise ValueError('docker.buildTarget must be specified')
+            raise ValueError("docker.buildTarget must be specified")
 
         image_tag = docker_image_tag(step_input)
-        dockerfile = docker_file_path(project=step_input.project, docker_config=docker_config)
+        dockerfile = docker_file_path(
+            project=step_input.project, docker_config=docker_config
+        )
 
         if not step_input.dry_run:
             # log in to registry, because we may need to pull in a base image
             login(logger=self._logger, docker_config=docker_config)
 
-        success = build(logger=self._logger, root_path=docker_config.root_folder,
-                        file_path=dockerfile, image_tag=image_tag,
-                        target=build_target)
-        artifact = input_to_artifact(ArtifactType.DOCKER_IMAGE, step_input, spec={'image': image_tag})
+        success = build(
+            logger=self._logger,
+            root_path=docker_config.root_folder,
+            file_path=dockerfile,
+            image_tag=image_tag,
+            target=build_target,
+        )
+        artifact = input_to_artifact(
+            ArtifactType.DOCKER_IMAGE, step_input, spec={"image": image_tag}
+        )
 
-        with open('.dockerignore', 'w+', encoding='utf-8') as ignore_file:
-            contents = '\n'.join(DOCKER_IGNORE_DEFAULT)
+        with open(".dockerignore", "w+", encoding="utf-8") as ignore_file:
+            contents = "\n".join(DOCKER_IGNORE_DEFAULT)
             ignore_file.write(contents)
 
         if success:
-            return Output(success=True, message=f"Built {step_input.project.name}", produced_artifact=artifact)
-
-        return Output(success=False, message=f"Failed to build docker image for {step_input.project.name}",
-                      produced_artifact=None)
+            return Output(
+                success=True,
+                message=f"Built {step_input.project.name}",
+                produced_artifact=artifact,
+            )
+
+        return Output(
+            success=False,
+            message=f"Failed to build docker image for {step_input.project.name}",
+            produced_artifact=None,
+        )
```

## mpyl/steps/build/echo.py

```diff
@@ -5,21 +5,32 @@
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
 from ...utilities.docker import docker_image_tag
 
 
 class BuildEcho(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Echo Build',
-            description='Dummy build step to test the framework',
-            version='0.0.1',
-            stage=Stage.BUILD
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.NONE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Echo Build",
+                description="Dummy build step to test the framework",
+                version="0.0.1",
+                stage=Stage.BUILD,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.NONE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         self._logger.info(f"Building project {step_input.project.name}")
-        artifact = input_to_artifact(ArtifactType.DOCKER_IMAGE, step_input,
-                                     spec={'image': docker_image_tag(step_input)})
-        return Output(success=True, message=f"Built {step_input.project.name}", produced_artifact=artifact)
+        artifact = input_to_artifact(
+            ArtifactType.DOCKER_IMAGE,
+            step_input,
+            spec={"image": docker_image_tag(step_input)},
+        )
+        return Output(
+            success=True,
+            message=f"Built {step_input.project.name}",
+            produced_artifact=artifact,
+        )
```

## mpyl/steps/build/sbt.py

```diff
@@ -16,44 +16,58 @@
 
 class BuildSbt(Step):
     def __init__(self, logger: Logger) -> None:
         self.logger = logger
         super().__init__(
             logger=logger,
             meta=Meta(
-                name='Sbt Build',
-                description='Build sbt project',
-                version='0.0.1',
-                stage=Stage.BUILD
+                name="Sbt Build",
+                description="Build sbt project",
+                version="0.0.1",
+                stage=Stage.BUILD,
             ),
             produced_artifact=ArtifactType.DOCKER_IMAGE,
             required_artifact=ArtifactType.NONE,
-            after=AfterBuildDocker(logger=logger)
+            after=AfterBuildDocker(logger=logger),
         )
 
     def execute(self, step_input: Input) -> Output:
         image_name = docker_image_tag(step_input)
         command = self._construct_sbt_command(step_input, image_name)
 
         output = custom_check_output(self.logger, command=command)
-        artifact = input_to_artifact(ArtifactType.DOCKER_IMAGE, step_input, {'image': image_name})
+        artifact = input_to_artifact(
+            ArtifactType.DOCKER_IMAGE, step_input, {"image": image_name}
+        )
         if output.success:
-            return Output(success=True, message=f"Built {step_input.project.name}", produced_artifact=artifact)
+            return Output(
+                success=True,
+                message=f"Built {step_input.project.name}",
+                produced_artifact=artifact,
+            )
 
-        return Output(success=False, message=f"Failed to build sbt project for {step_input.project.name}",
-                      produced_artifact=None)
+        return Output(
+            success=False,
+            message=f"Failed to build sbt project for {step_input.project.name}",
+            produced_artifact=None,
+        )
 
     @staticmethod
     def _construct_sbt_command(step_input: Input, image_name: str):
-        check_fmt: Optional[str] = \
-            'scalafmtCheckAll' if step_input.run_properties.target == Target.PULL_REQUEST else None
+        check_fmt: Optional[str] = (
+            "scalafmtCheckAll"
+            if step_input.run_properties.target == Target.PULL_REQUEST
+            else None
+        )
         commands: list[str] = [
-            command for command in [
-                f'project {step_input.project.name}',
+            command
+            for command in [
+                f"project {step_input.project.name}",
                 f'set docker / imageNames := Seq(ImageName("{image_name}"))',
                 check_fmt,
-                'docker'
-            ] if command is not None
+                "docker",
+            ]
+            if command is not None
         ]
         config = SbtConfig.from_config(config=step_input.run_properties.config)
         command = config.to_command(config.build_with_client, commands)
         return command
```

## mpyl/steps/deploy/k8s/chart.py

```diff
@@ -39,14 +39,15 @@
 from ruamel.yaml import YAML
 
 from . import substitute_namespaces
 from .resources import (
     CustomResourceDefinition,
     to_dict,
 )  # pylint: disable = no-name-in-module
+from .resources.prometheus import V1PrometheusRule
 from .resources.sealed_secret import V1SealedSecret
 from .resources.spark import (
     to_spark_body,
     get_spark_config_map_data,
     V1SparkApplication,
 )
 from .resources.traefik import (
@@ -64,14 +65,15 @@
     Resources,
     Target,
     Kubernetes,
     Job,
     Traefik,
     Host,
     get_env_variables,
+    Alert,
 )
 from ....stages.discovery import DeploySet
 
 yaml = YAML()
 
 # Determined (unscientifically) to be sensible factors.
 # Based on actual CPU usage, pods rarely use more than 10% of the allocated CPU. 60% usage is healthy, so we
@@ -331,14 +333,22 @@
         return V1ConfigMap(
             api_version="v1",
             kind="ConfigMap",
             data=get_spark_config_map_data(),
             metadata=self._to_object_meta(),
         )
 
+    def to_prometheus_rule(self, alerts: list[Alert]) -> V1PrometheusRule:
+        return V1PrometheusRule(
+            metadata=self._to_object_meta(
+                name=f"{self.project.name.lower()}-prometheus-rule"
+            ),
+            alerts=alerts,
+        )
+
     def __find_default_port(self) -> int:
         found = next(iter(self.mappings.keys()))
         if found:
             return int(found)
         raise KeyError("No default port found. Did you define a port mapping?")
 
     def create_host_wrappers(self) -> list[HostWrapper]:
@@ -445,16 +455,17 @@
             },
         )
 
     def _get_image(self):
         docker_image = self.step_input.required_artifact
         if not docker_image or docker_image.artifact_type != ArtifactType.DOCKER_IMAGE:
             raise ValueError(
+                # pylint: disable-next=no-member
                 f"Required artifact of type {ArtifactType.DOCKER_IMAGE.name} must be defined"
-            )  # pylint: disable=E1101
+            )
         return docker_image.spec["image"]
 
     def _get_resources(self):
         resources = self.project.kubernetes.resources
         defaults = self.config_defaults.resources_defaults
         return ChartBuilder._to_resources(resources, defaults, self.target)
 
@@ -583,23 +594,38 @@
 
         return chart
 
 
 def to_service_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
     return (
         builder.to_common_chart()
-        | {
-            "deployment": builder.to_deployment(),
-            "service": builder.to_service(),
-            "ingress-https-route": builder.to_ingress_routes(),
-        }
+        | _to_service_components_chart(builder)
         | builder.to_middlewares()
     )
 
 
+def _to_service_components_chart(builder):
+    common_chart = {
+        "deployment": builder.to_deployment(),
+        "service": builder.to_service(),
+        "ingress-https-route": builder.to_ingress_routes(),
+    }
+    prometheus_chart = (
+        {
+            "prometheus-rule": builder.to_prometheus_rule(
+                alerts=builder.project.kubernetes.metrics.alerts
+            )
+        }
+        if builder.project.kubernetes.metrics
+        and builder.project.kubernetes.metrics.enabled
+        else {}
+    )
+    return common_chart | prometheus_chart
+
+
 def to_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
     return builder.to_common_chart() | {"job": builder.to_job()}
 
 
 def to_cron_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
     return builder.to_common_chart() | {"cronjob": builder.to_cron_job()}
```

## mpyl/steps/postdeploy/cypress_test.py

```diff
@@ -1,13 +1,13 @@
 """ Step that runs relevant cypress tests in the post deploy stage """
-
+import itertools
 import os
 
+from concurrent.futures import ProcessPoolExecutor, Future
 from logging import Logger
-
 from python_on_whales import docker, Container, DockerException
 
 from .. import Step, Meta
 from ..models import ArtifactType, Input, Output, input_to_artifact
 from ...project import Stage, Target
 from ...utilities.cypress import CypressConfig
 from ...utilities.docker import execute_with_stream
@@ -24,15 +24,15 @@
                 version="0.0.1",
                 stage=Stage.POST_DEPLOY,
             ),
             produced_artifact=ArtifactType.JUNIT_TESTS,
             required_artifact=ArtifactType.NONE,
         )
 
-    def execute(self, step_input: Input) -> Output:
+    def execute(self, step_input: Input) -> Output:  # pylint: disable=too-many-locals
         if step_input.run_properties.target == Target.PRODUCTION:
             return Output(
                 success=True, message="Cypress tests are not run on production"
             )
 
         self._logger.info(
             f"Running cypress tests for project {step_input.project.name}"
@@ -40,110 +40,77 @@
         cypress_config = CypressConfig.from_config(step_input.run_properties.config)
         volume_path = os.path.join(os.getcwd(), cypress_config.cypress_source_code_path)
 
         if (
             step_input.project.dependencies
             and step_input.project.dependencies.postdeploy
         ):
-            specs_string = ", ".join(step_input.project.dependencies.postdeploy)
+            specs_string = ",".join(step_input.project.dependencies.postdeploy)
         else:
             raise ValueError("No cypress specs are defined in the project dependencies")
 
-        custom_image_tag = "mpyl/cypress"
-        docker.build(
-            context_path=volume_path,
-            tags=[custom_image_tag],
-            file=f"{volume_path}/Dockerfile-mpyl",
-        )
-        docker_container = docker.run(
-            image=custom_image_tag,
-            interactive=True,
-            detach=True,
-            volumes=[
-                (volume_path, "/cypress"),
-                (
-                    os.path.expanduser(cypress_config.kubectl_config_path),
-                    "/root/.kube/config",
-                ),
-            ],
-            workdir="/cypress",
-        )
-        if not isinstance(docker_container, Container):
-            raise TypeError("Docker run command should return a container")
-
+        docker_container = self._get_docker_container(volume_path, cypress_config)
         reports_folder = f"reports/{step_input.project.name}"
         artifact = input_to_artifact(
             artifact_type=ArtifactType.JUNIT_TESTS,
             step_input=step_input,
             spec={
                 TEST_OUTPUT_PATH_KEY: f"{volume_path}/{reports_folder}",
                 TEST_RESULTS_URL_KEY: "",
             },
         )
 
         try:
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command='bash -c "cp cypress.env.json.example cypress.env.json && '
-                f"sed -i 's/acceptance/"
-                f"{CypressTest._target_to_test_target(step_input.run_properties.target)}"
-                f"/' cypress.env.json && "
-                f"sed -i 's/{{PR_NUMBER}}/{step_input.run_properties.versioning.pr_number}/' "
-                'cypress.env.json"',
-                task_name="Preparing env file",
-            )
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command="yarn install",
-                task_name="Running yarn install",
-            )
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command="yarn cypress install",
-                task_name="Installing cypress",
-            )
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command="yarn cypress verify",
-                task_name="Verifying cypress",
-            )
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command="yarn tsc",
-                task_name="Compiling typescript",
-            )
-            execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command=f"rm -rf {reports_folder}",
-                task_name="Remove old report files",
-            )
-
-            run_command = (
-                f'bash -c "yarn cypress run --spec {specs_string} --reporter-options mochaFile='
-                f'"{reports_folder}/[hash].xml" || true"'
+            self._run_container_preparation_steps(
+                docker_container, step_input, reports_folder
             )
             record_key = cypress_config.record_key
+            run_command = ""
+
             if record_key:
+                ci_build_id = f"{cypress_config.ci_build_id}-{step_input.project.name}"
+                machines = [1, 2, 3, 4]
+                threads: list[Future] = []
+
+                for machine in machines:
+                    run_command = (
+                        f'bash -c "Xvfb :10{machine} & XDG_CONFIG_HOME=/tmp/cyhome{machine} '
+                        f"DISPLAY=:10{machine}  yarn cypress run --spec {specs_string} --ci-build-id "
+                        f"{ci_build_id} --parallel --reporter-options "
+                        f'"mochaFile={reports_folder}/[hash].xml" --record --key '
+                        'b6a2aab1-0b80-4ca0-a56c-1c8d98a8189c || true "'
+                    )
+                    executor = ProcessPoolExecutor(max_workers=len(machines))
+                    threads.append(
+                        executor.submit(
+                            execute_with_stream,
+                            logger=self._logger,
+                            container=docker_container,
+                            command=run_command,
+                            task_name="Running cypress tests parallel",
+                            multiprocess=True,
+                        )
+                    )
+
+                result: list[str] = list(
+                    itertools.chain.from_iterable(
+                        [thread.result() for thread in threads]
+                    )
+                )
+            else:
                 run_command = (
                     f'bash -c "yarn cypress run --spec {specs_string} --reporter-options '
-                    f'"mochaFile={reports_folder}/[hash].xml" --record --key '
-                    f'b6a2aab1-0b80-4ca0-a56c-1c8d98a8189c || true "'
+                    f'mochaFile="{reports_folder}/[hash].xml" || true"'
+                )
+                result = execute_with_stream(
+                    logger=self._logger,
+                    container=docker_container,
+                    command=run_command,
+                    task_name="Running cypress tests",
                 )
-            result = execute_with_stream(
-                logger=self._logger,
-                container=docker_container,
-                command=run_command,
-                task_name="Running cypress tests",
-            )
 
             for stdout in result:
                 if record_key and "Recorded Run" in stdout:
                     artifact.spec[TEST_RESULTS_URL_KEY] = stdout.rstrip().rsplit(
                         "Recorded Run: ", 1
                     )[1]
                 if "error Command failed with exit code" in stdout:
@@ -161,14 +128,87 @@
         return Output(
             success=True,
             message=f"Cypress tests for project {step_input.project.name} passed",
             produced_artifact=artifact,
         )
 
     @staticmethod
+    def _get_docker_container(
+        volume_path: str, cypress_config: CypressConfig
+    ) -> Container:
+        custom_image_tag = "mpyl/cypress"
+        docker.build(
+            context_path=volume_path,
+            tags=[custom_image_tag],
+            file=f"{volume_path}/Dockerfile-mpyl",
+        )
+        docker_container = docker.run(
+            image=custom_image_tag,
+            interactive=True,
+            detach=True,
+            volumes=[
+                (volume_path, "/cypress"),
+                (
+                    os.path.expanduser(cypress_config.kubectl_config_path),
+                    "/root/.kube/config",
+                ),
+            ],
+            workdir="/cypress",
+        )
+        if not isinstance(docker_container, Container):
+            raise TypeError("Docker run command should return a container")
+
+        return docker_container
+
+    def _run_container_preparation_steps(
+        self, docker_container: Container, step_input: Input, reports_folder: str
+    ) -> None:
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command=f"rm -rf {reports_folder} dist",
+            task_name="Remove old files",
+        )
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command='bash -c "cp cypress.env.json.example cypress.env.json && '
+            f"sed -i 's/acceptance/"
+            f"{CypressTest._target_to_test_target(step_input.run_properties.target)}"
+            f"/' cypress.env.json && "
+            f"sed -i 's/{{PR_NUMBER}}/{step_input.run_properties.versioning.pr_number}/' "
+            'cypress.env.json"',
+            task_name="Preparing env file",
+        )
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command="yarn install",
+            task_name="Running yarn install",
+        )
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command="yarn cypress install",
+            task_name="Installing cypress",
+        )
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command="yarn cypress verify",
+            task_name="Verifying cypress",
+        )
+        execute_with_stream(
+            logger=self._logger,
+            container=docker_container,
+            command="yarn tsc",
+            task_name="Compiling typescript",
+        )
+
+    @staticmethod
     def _target_to_test_target(target: Target) -> str:
         if target == Target.PULL_REQUEST_BASE:
             return "test"
         if target == Target.ACCEPTANCE:
             return "acceptance"
 
         return "pr"
```

## mpyl/utilities/cypress/__init__.py

```diff
@@ -1,24 +1,29 @@
 """Configuration required for running cypress"""
+import uuid
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class CypressConfig:
     cypress_source_code_path: str
     kubectl_config_path: str
     record_key: Optional[str]
+    ci_build_id: Optional[str]
 
     @staticmethod
     def from_config(config: dict):
         cypress_config = config.get("cypress")
         if not cypress_config:
             raise KeyError("Cypress section needs to be defined in mpyl_config.yml")
 
         return CypressConfig(
             cypress_source_code_path=cypress_config.get("cypressSourceCodePath"),
             record_key=cypress_config.get("recordKey"),
             kubectl_config_path=cypress_config.get(
                 "kubectlConfigPath", "~/.kube/config"
             ),
+            ci_build_id=cypress_config.get(
+                "ciBuildId", f"local{str(uuid.uuid4().int)[:10]}"
+            ).replace(" ", ""),
         )
```

## mpyl/utilities/docker/__init__.py

```diff
@@ -1,21 +1,20 @@
 """Docker related utility methods"""
 import logging
 import shlex
 
 from dataclasses import dataclass
-from itertools import tee
 from logging import Logger
 from traceback import print_exc
 from typing import Dict, Optional, Iterator, cast, Union
 import shutil
 from pathlib import Path
 from python_on_whales import docker, Image, Container, DockerException
 from python_on_whales.exceptions import NoSuchContainer
-from rich.text import Text
+from rich.logging import RichHandler
 
 from ..logging import try_parse_ansi
 from ...project import Project
 from ...steps.models import Input
 
 
 @dataclass(frozen=True)
@@ -63,22 +62,32 @@
                 docker_file_name=build_config["dockerFileName"],
             )
         except KeyError as exc:
             raise KeyError(f"Docker config could not be loaded from {config}") from exc
 
 
 def execute_with_stream(
-    logger: Logger, container: Container, command: str, task_name: str
+    logger: Logger,
+    container: Container,
+    command: str,
+    task_name: str,
+    multiprocess: bool = False,
 ):
+    if multiprocess:  # Logger settings need to be re-applied in each process
+        logger.setLevel(logging.INFO)
+        logger.addHandler(RichHandler())
+
     result = cast(
         Iterator[tuple[str, bytes]],
         container.execute(command=shlex.split(command), stream=True),
     )
     result_list = stream_docker_logging(logger, result, task_name)
 
+    logger.handlers.clear()
+
     return result_list
 
 
 def stream_docker_logging(
     logger: Logger,
     generator: Union[Iterator[str], Iterator[tuple[str, bytes]]],
     task_name: str,
```

## mpyl/utilities/repo/__init__.py

```diff
@@ -134,20 +134,29 @@
         intersection = files_in_revision.intersection(files_touched_in_branch)
         return Revision(count, str(revision), intersection)
 
     def changes_in_branch(self) -> list[Revision]:
         revisions = list(
             reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD")))
         )
+
+        logging.debug(
+            f"Found {len(revisions)} revisions in branch: {[r.hexsha for r in revisions]}"
+        )
+
         if not revisions:
             return []
 
+        first_revision = (
+            revisions[0].hexsha if len(revisions) != 1 else self._config.main_branch
+        )
+
         files_touched_in_branch = set(
             self._repo.git.diff(
-                f"{revisions[0].hexsha}..{revisions[-1].hexsha}", name_only=True
+                f"{first_revision}..{revisions[-1].hexsha}", name_only=True
             ).splitlines()
         )
         return [
             self.__to_revision(count, rev, files_touched_in_branch)
             for count, rev in enumerate(revisions)
         ]
```

## Comparing `mpyl-1.0.7.dist-info/LICENSE` & `mpyl-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mpyl-1.0.7.dist-info/METADATA` & `mpyl-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpyl
-Version: 1.0.7
+Version: 1.0.8
 Summary: Modular Pipeline Library
 Home-page: https://vandebron.github.io/mpyl
 Author: Vandebron Energie BV
 Project-URL: Documentation, https://vandebron.github.io/mpyl
 Project-URL: Source, https://github.com/Vandebron/mpyl
 Project-URL: Tracker, https://github.com/Vandebron/mpyl/issues
 Classifier: Topic :: Software Development :: Build Tools
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mpyl Version: 1.0.7 Summary: Modular Pipeline
+Metadata-Version: 2.1 Name: mpyl Version: 1.0.8 Summary: Modular Pipeline
 Library Home-page: https://vandebron.github.io/mpyl Author: Vandebron Energie
 BV Project-URL: Documentation, https://vandebron.github.io/mpyl Project-URL:
 Source, https://github.com/Vandebron/mpyl Project-URL: Tracker, https://
 github.com/Vandebron/mpyl/issues Classifier: Topic :: Software Development ::
 Build Tools Classifier: Topic :: Utilities Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
```

## Comparing `mpyl-1.0.7.dist-info/RECORD` & `mpyl-1.0.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,91 @@
 mpyl/__init__.py,sha256=0A89yKV9DB7xfO0JBHPL_oBVPvLIIkMvUqmzkjtFVt4,766
 mpyl/__main__.py,sha256=2c9boQJDUA6b8p2umOych7HHlwmBdmsIQDLZcE_pBdo,215
 mpyl/constants.py,sha256=QjtU24q52cowD4mLr54Xa0XeclFZ_Bx-7BV7GzpUhyg,162
-mpyl/project.py,sha256=KZGpjTTiu7QiPiv1yCLRJrH-LW_X5INWwcaKv_XwQEE,13948
+mpyl/project.py,sha256=_1qNDVZWqgDLm0XMEcVdVPfa6f6GL_t_doy9Fh3aEbw,14810
 mpyl/validation.py,sha256=kcYjYZQx2UmeMRf_OXCrO5tkzrV6SlIDkFbSx5oBPHs,1710
 mpyl/cli/__init__.py,sha256=6J4nIg4-Zo2OCrMBZE-RzLyS7v81G3HtWXpX5Cx0quI,2789
 mpyl/cli/build.py,sha256=Byp-Nq2hVxvM_MszwliznGSqReL2My48MqLy5jFUGe4,11043
 mpyl/cli/health.py,sha256=2MMSEcw8ehtOWQYh1XnNMbJjOqnyKA7DZqH3a-9CdCM,341
 mpyl/cli/meta_info.py,sha256=TWSjF-wk4Strn8xaSgULUUhKBETuSvzQDuunex5FbJE,2170
-mpyl/cli/projects.py,sha256=Mp3CXic59ifTCiIVAevgwPPUMwASsWRFh6USff1EHfI,3853
+mpyl/cli/projects.py,sha256=7IRK_nNWPm6DSxN4f5fFS6uD78F7iiIrOiTxxAqiSZ0,4515
 mpyl/cli/commands/__init__.py,sha256=DaL5q4ibFJT7EMlgcQBSpAaaQNiBqnSJZ2WIKtPzLJk,34
-mpyl/cli/commands/build/__init__.py,sha256=Ox0F68re6bNGLBC4KEBLmXXSRf5OIJZ8N2Vens3rgEk,439
-mpyl/cli/commands/build/jenkins.py,sha256=GYXj4N0GLIm23Lx8hTIEhlGTxgUhyhYVnnhLD1LCfXQ,3923
-mpyl/cli/commands/build/mpyl.py,sha256=Zyu_nPYpQR4GrprwmOExACTSvC2cZJIl-UfvpMUuUic,5901
+mpyl/cli/commands/build/__init__.py,sha256=mB2oXyzf-5OL37AK8XPbR9qlD8f4sEKdLzRjzxXxmB8,439
+mpyl/cli/commands/build/jenkins.py,sha256=-n-X5Z7ow6u75-yjXanINZBZjg4ztExTuJqmrqE6yf8,4287
+mpyl/cli/commands/build/mpyl.py,sha256=ffXapT1XJwr7kQOzOtPHkAiPlaV9fcAw0G1dE3CNoaM,6555
 mpyl/cli/commands/health/__init__.py,sha256=Bx6QcWIN-EadbpSe1XAXs1aYCD7Ad8_t3lWRlGDsIr0,38
 mpyl/cli/commands/health/checks.py,sha256=rhRKiJrO1vTKojnH04HqW4r3uPIc2wkiFYnw-W7M6Uw,5535
 mpyl/cli/commands/projects/__init__.py,sha256=YoVobAUCYwqc23p-iAuQnpJQYpdri5ljtj8l_XKYOr0,46
 mpyl/cli/commands/projects/formatting.py,sha256=qpKokiaZdZ2ZezXuGy3Q3e3Fq9DKMq7gvruE779l9TA,1061
 mpyl/projects/__init__.py,sha256=31HPF5jDZK5UkQT8Zw0V0QSJLqzp8f2zFiWd-QkDjRE,620
 mpyl/projects/find.py,sha256=qAaYA1V2tNXAM_tq1-HwQV4fvCdwyPGa5InY0RZetm4,2202
 mpyl/reporting/__init__.py,sha256=vRvt_67opWXCfe_zYZChT-YhjoPOahAjLagoaVzOcFM,92
 mpyl/reporting/formatting/__init__.py,sha256=GAvYJpHT2SMQxjiLCSqFy57PNWsGI_Ow2bFnA8cX08k,76
 mpyl/reporting/formatting/markdown.py,sha256=dSArxUA0qiN6MzFlqSzIGcjDGY2iFhlZNXMuRwAGwDQ,5213
 mpyl/reporting/formatting/text.py,sha256=oihlYM4XVEjzYz5wq8uUViTypcR4yZ-Aw_ujnr396fE,1411
 mpyl/reporting/targets/__init__.py,sha256=31UWFweqJqvlE3WZBb2CMBIAnmJJRZpVBwpW-ma4MzA,1139
 mpyl/reporting/targets/github.py,sha256=J9lYoib_tLDPgQslzBgeYymk78g4yLMFWDLdlMSyMFs,8453
 mpyl/reporting/targets/jira.py,sha256=8D4LPBhIdYiH_oTgSd7d3nNjnacGEn2Qf4AC7RiFGJU,9331
 mpyl/reporting/targets/slack.py,sha256=gTD8MNNJchCFPwK4k0Rs7eNkUzpyKjnkjB6DwKRmu2I,7997
-mpyl/schema/mpyl_config.schema.yml,sha256=f7j-04KI0Im1CoOZZ-Dale-Sw4RSnX0fdzsJ72FGKU8,8433
+mpyl/schema/mpyl_config.schema.yml,sha256=XSFdyLzogEn_KmRngw2sqRcOWIl-XIr5wEPA7kCAvNI,8536
 mpyl/schema/project.schema.yml,sha256=Pn31oWBvupNXOVuUwykJv-P7C28eoELz5YwCJcKnntI,25500
-mpyl/schema/run_properties.schema.yml,sha256=mIPDvvwi_u3cQZW0FShFY1ZMdqT9AcCwg9Y3MA0xsSw,2914
+mpyl/schema/run_properties.schema.yml,sha256=zrcKWuXkfEBOe-6deRa8TUmJQjdOHPW3hB-X8G8a-Mc,2928
 mpyl/stages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mpyl/stages/discovery.py,sha256=HCiWshRKL9Rtgu-HzdR5U5St4hYOlCwFul3CASFcTE0,3698
 mpyl/steps/__init__.py,sha256=utJ4jkk9PP27FVsjDz7awvKAUJdII5GMT5SUM8tAwbw,6437
 mpyl/steps/collection.py,sha256=4VBv34RR261w7aGRFiyq9gkMuqRrDCctnD96wFMTvpM,1442
-mpyl/steps/models.py,sha256=VEeQ_XTC2aC1u_hXthFC1Y-HSR8ndS8NBltEO9pD-ZI,6085
+mpyl/steps/models.py,sha256=H4pymZwIyC7s6nWU0mpaeTEZZ4EXQYkz2S89qKAWEhs,6114
 mpyl/steps/run.py,sha256=kp1Qm3WM3FoIpXTwQ3ddlptyQ_kvC6gtP90-eIW39mc,3505
 mpyl/steps/steps.py,sha256=mUEhy78h3KFXfd5s0DBO3nXIbwcXhlXkR5Cya10wlbU,7278
 mpyl/steps/build/__init__.py,sha256=EyPUNNDMQfJK-RVjYM9WvPhEDITbu2n4fx9mxhGLlDs,59
-mpyl/steps/build/docker_after_build.py,sha256=nok2HRrH66e9FBvfwEKnalJhX3io__PQZaq_fR0S8BI,2093
-mpyl/steps/build/dockerbuild.py,sha256=6lqVqiuGYk8ISuzTterTFdcIWqUkvSOUCOCDmjHkM2s,2865
-mpyl/steps/build/echo.py,sha256=EwOHLpyD--1joICl7kNnh6p_JfguCSQX4WirA_5BNn8,996
-mpyl/steps/build/sbt.py,sha256=rvJzIVgsx6KrX5HW_jqEhu6yV2QAttEXQRJ3A7XJJ-k,2402
+mpyl/steps/build/docker_after_build.py,sha256=b_9eaTytpKvQru_uDhAqiq9AygP36WteFpwrSo5Z2zk,2334
+mpyl/steps/build/dockerbuild.py,sha256=tlW5ck0shy8ZuMYruWnn-RuvbQybpgur8Jwi-syV05U,3111
+mpyl/steps/build/echo.py,sha256=v1Wdo3jkO4ximPR1fU45Lm0G-fQQ2SZcVt9ahdPNjA8,1132
+mpyl/steps/build/sbt.py,sha256=cqWa8CrbUi80MPn_G41dNlRF8xdZg5ytiYGCUi1zxIE,2573
 mpyl/steps/deploy/__init__.py,sha256=14PYgOvt7YEO2Zw4kEeZxWUNBR7Lz91nSoJZpvJHqzE,60
 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=Fcq2555DwX2dUrBcuqLCb5-2lJ_PGqYkiP-NJwglvGY,2767
 mpyl/steps/deploy/echo.py,sha256=pB63Cox_7Bn0wbhlP5Aj9dGh1E8aUGY7pv0HDdIOqao,1196
 mpyl/steps/deploy/ephemeral_docker_deploy.py,sha256=3YUqRWlFD3YVlNR8s5Shfa1KTdQg8vsWZ_omdMY_8b4,1472
 mpyl/steps/deploy/kubernetes.py,sha256=-VjRR5Hk_3MH5xQX7CTbvWpBkT-WbFJX1kECTcy1WP8,3896
 mpyl/steps/deploy/kubernetes_job.py,sha256=tFhY8RASKQ6OSEbxQgMYbcd9--83ibyPNivKxOfbFpY,1588
 mpyl/steps/deploy/kubernetes_spark_job.py,sha256=deKKaX-Ktrll47d_h-Pw1nda-5DfT96LupvWdKdLPSI,1571
 mpyl/steps/deploy/k8s/__init__.py,sha256=VRGBw1VFGB06UVYnMUk_ObK67GOfVx7EhVCO0LpYwfM,3518
-mpyl/steps/deploy/k8s/chart.py,sha256=Lfi30_1s5dshqvZkSlabp3xJpXPpTXj-Ebl6nUmdZKY,20536
+mpyl/steps/deploy/k8s/chart.py,sha256=X5tvoy-Qvt26AV0CbU_14AR4dWsWAhj3cK4Iu18OchI,21329
 mpyl/steps/deploy/k8s/helm.py,sha256=GHDQjdsFuL54l__gP47REVJWZPr9Acbh20b75fQsEEI,2989
 mpyl/steps/deploy/k8s/rancher.py,sha256=m40g7kGc-09OML4NMtOpnrM8mkZxSIJzx24gc4GqUfk,1732
 mpyl/steps/deploy/k8s/resources/__init__.py,sha256=c2ZTt4SwsExUnF1Bu1N1kjxDNd6zTsYGX2G5btTMdNE,4719
+mpyl/steps/deploy/k8s/resources/prometheus.py,sha256=D63BckBFX2iZirZ3d2m5dvuKzWvWIXREZYobBg8NAP4,1200
 mpyl/steps/deploy/k8s/resources/sealed_secret.py,sha256=af8zae2HVCnT51aEq_3kKVHp86gf8UpzDWM87jSQoJ4,616
 mpyl/steps/deploy/k8s/resources/spark.py,sha256=GQUHogCmFl3GHAg54pyFlv1bAZAtk68c5vzRQwaWLDk,5850
 mpyl/steps/deploy/k8s/resources/traefik.py,sha256=COJ9ekK8EKtbABE2IWRRIfKCIbOl8DC9Tr_NAuUblCk,2287
+mpyl/steps/deploy/k8s/resources/schema/monitoring.coreos.com_prometheuses.schema.yml,sha256=CI7RZpvJ-ThZYVLXgVW4XP-8fgMVX7Fd5KDtRheOWbU,582149
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml,sha256=jTo3LZklRCZ1L7JZbUdcmhDWhk3VDJhrDz_OTHNUm58,168371
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml,sha256=s1rMobinpB3aXI1ONcuTMGLMIRRQ_qZrZtQTYZHcDFU,151469
 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml,sha256=3Oc1awM23acMS36kqpbfqwx6D8Sft4FnL8abNLgcwBI,11703
 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml,sha256=6QCi1F9LJ3cgmwaPBV8dWFvbXb2B5huKvfp4Pa1hoBw,42950
 mpyl/steps/postdeploy/__init__.py,sha256=cUDlHPzcW5zGGPxr9T77pATS5lwKnP9Ge8JroAGSvBg,64
-mpyl/steps/postdeploy/cypress_test.py,sha256=aZ_fmMsqq7eEsz4GzFS-DTEcdSl0rgOhPC4KLyYmlCA,6496
+mpyl/steps/postdeploy/cypress_test.py,sha256=jThGMjQ6X-IJgcdnHDR1w5haeuvTDCCdNAu1ofJJrq4,8161
 mpyl/steps/test/__init__.py,sha256=XL1gSbIMJYSFcy4Vf8YRbZM9yAs3Fzvq2tfX9xTDZX8,58
 mpyl/steps/test/after_test.py,sha256=TVRsdWxVRNagi5Ajqa1caP9EySnBmoSJP_j1in7GA30,1560
 mpyl/steps/test/before_test.py,sha256=agBmlSSoHJyK2truhSaVb_0K2trYeIAamDwxQ1ZLh50,2596
 mpyl/steps/test/dockertest.py,sha256=4ESQDmWflOKapVZux7VYDpjlCqv7QXmehFdiJaL39to,3886
 mpyl/steps/test/echo.py,sha256=5xfmhn7xbPCHQ7H_X49idHDv-FZK556kqFRqsUktJnI,1929
 mpyl/steps/test/sbt.py,sha256=26pkmwOvJRegrBRr6KzT3wHbuY-yFIqJ99FQEwCDiac,5075
 mpyl/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mpyl/utilities/cypress/__init__.py,sha256=-31jEaaANvamp7AjocY4D68esOWCxA6rIaz2j8-MOos,768
-mpyl/utilities/docker/__init__.py,sha256=7vk98Y8Obc6UOSq_4qAWSVpa_j7uyuGrF46AiMwZANI,6693
+mpyl/utilities/cypress/__init__.py,sha256=VQZtP7hiFhRNr0jIAutomuL0yjdEY1mWQLqhzC1ZRVA,953
+mpyl/utilities/docker/__init__.py,sha256=HgkXSCl0G-MvYxD1gfEcTQTsrNW6j5q0PXsR3s-RrnQ,6909
 mpyl/utilities/github/__init__.py,sha256=IPvxPLObUcqwVsWq46Yp6C6MNYFYALtxYTW6gu4F6II,1781
 mpyl/utilities/jenkins/__init__.py,sha256=850w2rxbeSGmYieBQ5VHuSM3pV6FG9Vbdf41Lwpi0_g,1551
 mpyl/utilities/jenkins/runner.py,sha256=ObgHVxZRxiFXUD6v-O55IH7Oh7GpKXqXKSxhg3RCF74,7903
 mpyl/utilities/junit/__init__.py,sha256=lybqA7y8gmOg7HFKdqZYdUf80Z-fCix-yhbjG8OKM4U,1431
 mpyl/utilities/logging/__init__.py,sha256=dlVErHdOt6YQ9LV91_7e1-XMTa4fagC-xl-GROppD5c,254
 mpyl/utilities/pyaml_env/__init__.py,sha256=Wa-KUCJy8hTFOAYXiZcOKo3_EXmnyD9AzeUuDqeLw24,880
-mpyl/utilities/repo/__init__.py,sha256=dGe6c4hATQqGQkpig7bn9iWkoknLEbBdsjdjDdaSJrQ,7098
+mpyl/utilities/repo/__init__.py,sha256=haxHfJmTIk3R2zhVnQjADffrY-xj-UQ7GUjtePGpCh8,7342
 mpyl/utilities/s3/__init__.py,sha256=Czr2nAMwU9eCqEvymGecNhxnYLwYSdHz9Yw13FwPY-A,4764
 mpyl/utilities/sbt/__init__.py,sha256=nM8iUUL92luMGoMQUPnJm2tJkAta0ct601dMj0oFDsg,1612
 mpyl/utilities/subprocess/__init__.py,sha256=KYzwKeOh-myUE2VSEL7NWVpiz-WsoTwRIgU8Y03Fo5I,2326
-mpyl-1.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mpyl-1.0.7.dist-info/METADATA,sha256=_GkVO_9gSq4wvvwK0Y6XIoiXuYGpHUI_7boN6HmGejo,6083
-mpyl-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mpyl-1.0.7.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
-mpyl-1.0.7.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
-mpyl-1.0.7.dist-info/RECORD,,
+mpyl-1.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mpyl-1.0.8.dist-info/METADATA,sha256=LL5eMc40dubIwSwugP7UNU1_3w2B9e6RbCBiRYwbjyw,6083
+mpyl-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mpyl-1.0.8.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
+mpyl-1.0.8.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
+mpyl-1.0.8.dist-info/RECORD,,
```

