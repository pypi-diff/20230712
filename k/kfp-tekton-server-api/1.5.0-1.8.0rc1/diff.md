# Comparing `tmp/kfp-tekton-server-api-1.5.0.tar.gz` & `tmp/kfp-tekton-server-api-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-server-api-1.5.0.tar", last modified: Fri Jan 27 08:26:08 2023, max compression
+gzip compressed data, was "kfp-tekton-server-api-1.8.0rc1.tar", last modified: Wed Jul 12 21:12:27 2023, max compression
```

## Comparing `kfp-tekton-server-api-1.5.0.tar` & `kfp-tekton-server-api-1.8.0rc1.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.096817 kfp-tekton-server-api-1.5.0/
--rw-r--r--   0 prashantsharma   (501) staff       (20)    11357 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/LICENSE
--rw-r--r--   0 prashantsharma   (501) staff       (20)      476 2023-01-27 08:26:08.097023 kfp-tekton-server-api-1.5.0/PKG-INFO
--rw-r--r--   0 prashantsharma   (501) staff       (20)    12028 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/README.md
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.047950 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4360 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/__init__.py
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.054165 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/
--rw-r--r--   0 prashantsharma   (501) staff       (20)      550 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/__init__.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    35965 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/experiment_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5362 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/healthz_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    34966 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/job_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    67675 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/pipeline_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    13684 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    58950 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/run_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    26295 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api_client.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    13326 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/configuration.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3805 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/exceptions.py
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.075350 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3412 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/__init__.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2883 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/job_mode.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4654 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     7258 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/protobuf_any.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     6722 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3188 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2906 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/run_metric_format.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4724 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_cron_schedule.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     7859 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_experiment.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2993 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_experiment_storage_state.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3481 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_get_healthz_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3772 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_get_template_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    14757 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_job.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5607 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_experiments_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5285 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_jobs_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5555 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5411 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_pipelines_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5191 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_runs_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3879 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_parameter.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5019 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_periodic_schedule.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    10884 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5064 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline_runtime.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     8412 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline_spec.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     9801 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline_version.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3878 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_read_artifact_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2926 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_relationship.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4401 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_report_run_metrics_request.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3607 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3999 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_key.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4904 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_reference.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3067 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_type.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    14108 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4137 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_detail.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     6345 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_metric.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2907 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_storage_state.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4514 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_status.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4374 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_trigger.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3578 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_url.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4819 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_value.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)    12344 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/rest.py
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.050443 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/
--rw-r--r--   0 prashantsharma   (501) staff       (20)      476 2023-01-27 08:26:08.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/PKG-INFO
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4296 2023-01-27 08:26:08.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 prashantsharma   (501) staff       (20)        1 2023-01-27 08:26:08.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 prashantsharma   (501) staff       (20)       48 2023-01-27 08:26:08.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/requires.txt
--rw-r--r--   0 prashantsharma   (501) staff       (20)       22 2023-01-27 08:26:08.000000 kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/top_level.txt
--rw-r--r--   0 prashantsharma   (501) staff       (20)       69 2023-01-27 08:26:08.097682 kfp-tekton-server-api-1.5.0/setup.cfg
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1232 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/setup.py
-drwxr-xr-x   0 prashantsharma   (501) staff       (20)        0 2023-01-27 08:26:08.096341 kfp-tekton-server-api-1.5.0/test/
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2068 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_experiment_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)      949 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_healthz_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1349 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_job_mode.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1714 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_job_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3357 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_pipeline_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1852 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_pipeline_spec_runtime_config.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1081 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1457 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_protobuf_any.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1925 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1847 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1439 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_run_metric_format.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2452 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_run_service_api.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1669 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_cron_schedule.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2114 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_experiment.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1540 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_experiment_storage_state.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1530 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_get_healthz_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1538 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_get_template_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4354 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_job.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2573 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_list_experiments_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     5064 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_list_jobs_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2996 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_list_pipeline_versions_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3697 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_list_pipelines_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4316 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_list_runs_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1450 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_parameter.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1724 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_periodic_schedule.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3575 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_pipeline.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1543 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_pipeline_runtime.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2242 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_pipeline_spec.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2473 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_pipeline_version.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1548 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_read_artifact_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1426 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_relationship.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1884 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_report_run_metrics_request.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1944 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_report_run_metrics_response.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1491 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_resource_key.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1735 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_resource_reference.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1428 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_resource_type.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     3638 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_run.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     4144 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_run_detail.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1534 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_run_metric.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1463 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_run_storage_state.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1626 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_status.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     2296 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_trigger.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1362 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_url.py
--rw-r--r--   0 prashantsharma   (501) staff       (20)     1457 2023-01-27 08:26:07.000000 kfp-tekton-server-api-1.5.0/test/test_v1_value.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.612959 kfp-tekton-server-api-1.8.0rc1/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/LICENSE
+-rw-r--r--   0 tommyli    (501) staff       (20)      455 2023-07-12 21:12:27.613173 kfp-tekton-server-api-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    13063 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.564331 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/
+-rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/__init__.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.570540 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/
+-rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api_client.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13319 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/configuration.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/exceptions.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.590901 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/
+-rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    11586 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13714 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4289 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_value.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/rest.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.566967 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)      455 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-12 21:12:27.613839 kfp-tekton-server-api-1.8.0rc1/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     1201 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.612449 kfp-tekton-server-api-1.8.0rc1/test/
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.5.0/LICENSE` & `kfp-tekton-server-api-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.5.0/README.md` & `kfp-tekton-server-api-1.8.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # kfp-tekton-server-api
-This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.5.0
-- Package version: 1.5.0
+- API version: 1.7.0
+- Package version: 1.8.0rc1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
-For more information, please visit [https://github.com/kubeflow/kfp-tekton](https://github.com/kubeflow/kfp-tekton)
+For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
@@ -79,67 +79,69 @@
 with kfp_tekton_server_api.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = kfp_tekton_server_api.ExperimentServiceApi(api_client)
     id = 'id_example' # str | The ID of the experiment to be archived.
 
     try:
         # Archives an experiment and the experiment's runs and jobs.
-        api_response = api_instance.archive_experiment(id)
+        api_response = api_instance.experiment_service_archive_experiment(id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling ExperimentServiceApi->archive_experiment: %s\n" % e)
+        print("Exception when calling ExperimentServiceApi->experiment_service_archive_experiment: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ExperimentServiceApi* | [**archive_experiment**](docs/ExperimentServiceApi.md#archive_experiment) | **POST** /apis/v1/experiments/{id}:archive | Archives an experiment and the experiment&#39;s runs and jobs.
-*ExperimentServiceApi* | [**create_experiment**](docs/ExperimentServiceApi.md#create_experiment) | **POST** /apis/v1/experiments | Creates a new experiment.
-*ExperimentServiceApi* | [**delete_experiment**](docs/ExperimentServiceApi.md#delete_experiment) | **DELETE** /apis/v1/experiments/{id} | Deletes an experiment without deleting the experiment&#39;s runs and jobs. To avoid unexpected behaviors, delete an experiment&#39;s runs and jobs before deleting the experiment.
-*ExperimentServiceApi* | [**get_experiment**](docs/ExperimentServiceApi.md#get_experiment) | **GET** /apis/v1/experiments/{id} | Finds a specific experiment by ID.
-*ExperimentServiceApi* | [**list_experiment**](docs/ExperimentServiceApi.md#list_experiment) | **GET** /apis/v1/experiments | Finds all experiments. Supports pagination, and sorting on certain fields.
-*ExperimentServiceApi* | [**unarchive_experiment**](docs/ExperimentServiceApi.md#unarchive_experiment) | **POST** /apis/v1/experiments/{id}:unarchive | Restores an archived experiment. The experiment&#39;s archived runs and jobs will stay archived.
-*HealthzServiceApi* | [**get_healthz**](docs/HealthzServiceApi.md#get_healthz) | **GET** /apis/v1/healthz | Get healthz data.
-*JobServiceApi* | [**create_job**](docs/JobServiceApi.md#create_job) | **POST** /apis/v1/jobs | Creates a new job.
-*JobServiceApi* | [**delete_job**](docs/JobServiceApi.md#delete_job) | **DELETE** /apis/v1/jobs/{id} | Deletes a job.
-*JobServiceApi* | [**disable_job**](docs/JobServiceApi.md#disable_job) | **POST** /apis/v1/jobs/{id}/disable | Stops a job and all its associated runs. The job is not deleted.
-*JobServiceApi* | [**enable_job**](docs/JobServiceApi.md#enable_job) | **POST** /apis/v1/jobs/{id}/enable | Restarts a job that was previously stopped. All runs associated with the job will continue.
-*JobServiceApi* | [**get_job**](docs/JobServiceApi.md#get_job) | **GET** /apis/v1/jobs/{id} | Finds a specific job by ID.
-*JobServiceApi* | [**list_jobs**](docs/JobServiceApi.md#list_jobs) | **GET** /apis/v1/jobs | Finds all jobs.
-*PipelineServiceApi* | [**create_pipeline**](docs/PipelineServiceApi.md#create_pipeline) | **POST** /apis/v1/pipelines | Creates a pipeline.
-*PipelineServiceApi* | [**create_pipeline_version**](docs/PipelineServiceApi.md#create_pipeline_version) | **POST** /apis/v1/pipeline_versions | Adds a pipeline version to the specified pipeline.
-*PipelineServiceApi* | [**delete_pipeline**](docs/PipelineServiceApi.md#delete_pipeline) | **DELETE** /apis/v1/pipelines/{id} | Deletes a pipeline and its pipeline versions.
-*PipelineServiceApi* | [**delete_pipeline_version**](docs/PipelineServiceApi.md#delete_pipeline_version) | **DELETE** /apis/v1/pipeline_versions/{version_id} | Deletes a pipeline version by pipeline version ID. If the deleted pipeline version is the default pipeline version, the pipeline&#39;s default version changes to the pipeline&#39;s most recent pipeline version. If there are no remaining pipeline versions, the pipeline will have no default version. Examines the run_service_api.ipynb notebook to learn more about creating a run using a pipeline version (https://github.com/kubeflow/pipelines/blob/master/tools/benchmarks/run_service_api.ipynb).
-*PipelineServiceApi* | [**get_pipeline**](docs/PipelineServiceApi.md#get_pipeline) | **GET** /apis/v1/pipelines/{id} | Finds a specific pipeline by ID.
-*PipelineServiceApi* | [**get_pipeline_version**](docs/PipelineServiceApi.md#get_pipeline_version) | **GET** /apis/v1/pipeline_versions/{version_id} | Gets a pipeline version by pipeline version ID.
-*PipelineServiceApi* | [**get_pipeline_version_template**](docs/PipelineServiceApi.md#get_pipeline_version_template) | **GET** /apis/v1/pipeline_versions/{version_id}/templates | Returns a YAML template that contains the specified pipeline version&#39;s description, parameters and metadata.
-*PipelineServiceApi* | [**get_template**](docs/PipelineServiceApi.md#get_template) | **GET** /apis/v1/pipelines/{id}/templates | Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.
-*PipelineServiceApi* | [**list_pipeline_versions**](docs/PipelineServiceApi.md#list_pipeline_versions) | **GET** /apis/v1/pipeline_versions | Lists all pipeline versions of a given pipeline.
-*PipelineServiceApi* | [**list_pipelines**](docs/PipelineServiceApi.md#list_pipelines) | **GET** /apis/v1/pipelines | Finds all pipelines.
-*PipelineServiceApi* | [**update_pipeline_default_version**](docs/PipelineServiceApi.md#update_pipeline_default_version) | **POST** /apis/v1/pipelines/{pipeline_id}/default_version/{version_id} | Update the default pipeline version of a specific pipeline.
+*ExperimentServiceApi* | [**experiment_service_archive_experiment**](docs/ExperimentServiceApi.md#experiment_service_archive_experiment) | **POST** /apis/v1/experiments/{id}:archive | Archives an experiment and the experiment&#39;s runs and jobs.
+*ExperimentServiceApi* | [**experiment_service_create_experiment**](docs/ExperimentServiceApi.md#experiment_service_create_experiment) | **POST** /apis/v1/experiments | Creates a new experiment.
+*ExperimentServiceApi* | [**experiment_service_delete_experiment**](docs/ExperimentServiceApi.md#experiment_service_delete_experiment) | **DELETE** /apis/v1/experiments/{id} | Deletes an experiment without deleting the experiment&#39;s runs and jobs. To avoid unexpected behaviors, delete an experiment&#39;s runs and jobs before deleting the experiment.
+*ExperimentServiceApi* | [**experiment_service_get_experiment**](docs/ExperimentServiceApi.md#experiment_service_get_experiment) | **GET** /apis/v1/experiments/{id} | Finds a specific experiment by ID.
+*ExperimentServiceApi* | [**experiment_service_list_experiment**](docs/ExperimentServiceApi.md#experiment_service_list_experiment) | **GET** /apis/v1/experiments | Finds all experiments. Supports pagination, and sorting on certain fields.
+*ExperimentServiceApi* | [**experiment_service_unarchive_experiment**](docs/ExperimentServiceApi.md#experiment_service_unarchive_experiment) | **POST** /apis/v1/experiments/{id}:unarchive | Restores an archived experiment. The experiment&#39;s archived runs and jobs will stay archived.
+*HealthzServiceApi* | [**healthz_service_get_healthz**](docs/HealthzServiceApi.md#healthz_service_get_healthz) | **GET** /apis/v1/healthz | Get healthz data.
+*JobServiceApi* | [**job_service_create_job**](docs/JobServiceApi.md#job_service_create_job) | **POST** /apis/v1/jobs | Creates a new job.
+*JobServiceApi* | [**job_service_delete_job**](docs/JobServiceApi.md#job_service_delete_job) | **DELETE** /apis/v1/jobs/{id} | Deletes a job.
+*JobServiceApi* | [**job_service_disable_job**](docs/JobServiceApi.md#job_service_disable_job) | **POST** /apis/v1/jobs/{id}/disable | Stops a job and all its associated runs. The job is not deleted.
+*JobServiceApi* | [**job_service_enable_job**](docs/JobServiceApi.md#job_service_enable_job) | **POST** /apis/v1/jobs/{id}/enable | Restarts a job that was previously stopped. All runs associated with the job will continue.
+*JobServiceApi* | [**job_service_get_job**](docs/JobServiceApi.md#job_service_get_job) | **GET** /apis/v1/jobs/{id} | Finds a specific job by ID.
+*JobServiceApi* | [**job_service_list_jobs**](docs/JobServiceApi.md#job_service_list_jobs) | **GET** /apis/v1/jobs | Finds all jobs.
+*PipelineServiceApi* | [**pipeline_service_create_pipeline**](docs/PipelineServiceApi.md#pipeline_service_create_pipeline) | **POST** /apis/v1/pipelines | Creates a pipeline.
+*PipelineServiceApi* | [**pipeline_service_create_pipeline_version**](docs/PipelineServiceApi.md#pipeline_service_create_pipeline_version) | **POST** /apis/v1/pipeline_versions | Adds a pipeline version to the specified pipeline.
+*PipelineServiceApi* | [**pipeline_service_delete_pipeline**](docs/PipelineServiceApi.md#pipeline_service_delete_pipeline) | **DELETE** /apis/v1/pipelines/{id} | Deletes a pipeline and its pipeline versions.
+*PipelineServiceApi* | [**pipeline_service_delete_pipeline_version**](docs/PipelineServiceApi.md#pipeline_service_delete_pipeline_version) | **DELETE** /apis/v1/pipeline_versions/{versionId} | Deletes a pipeline version by pipeline version ID. If the deleted pipeline version is the default pipeline version, the pipeline&#39;s default version changes to the pipeline&#39;s most recent pipeline version. If there are no remaining pipeline versions, the pipeline will have no default version. Examines the run_service_api.ipynb notebook to learn more about creating a run using a pipeline version (https://github.com/kubeflow/pipelines/blob/master/tools/benchmarks/run_service_api.ipynb).
+*PipelineServiceApi* | [**pipeline_service_get_pipeline**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline) | **GET** /apis/v1/pipelines/{id} | Finds a specific pipeline by ID.
+*PipelineServiceApi* | [**pipeline_service_get_pipeline_version**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline_version) | **GET** /apis/v1/pipeline_versions/{versionId} | Gets a pipeline version by pipeline version ID.
+*PipelineServiceApi* | [**pipeline_service_get_pipeline_version_template**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline_version_template) | **GET** /apis/v1/pipeline_versions/{versionId}/templates | Returns a YAML template that contains the specified pipeline version&#39;s description, parameters and metadata.
+*PipelineServiceApi* | [**pipeline_service_get_template**](docs/PipelineServiceApi.md#pipeline_service_get_template) | **GET** /apis/v1/pipelines/{id}/templates | Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.
+*PipelineServiceApi* | [**pipeline_service_list_pipeline_versions**](docs/PipelineServiceApi.md#pipeline_service_list_pipeline_versions) | **GET** /apis/v1/pipeline_versions | Lists all pipeline versions of a given pipeline.
+*PipelineServiceApi* | [**pipeline_service_list_pipelines**](docs/PipelineServiceApi.md#pipeline_service_list_pipelines) | **GET** /apis/v1/pipelines | Finds all pipelines.
+*PipelineServiceApi* | [**pipeline_service_update_pipeline_default_version**](docs/PipelineServiceApi.md#pipeline_service_update_pipeline_default_version) | **POST** /apis/v1/pipelines/{pipelineId}/default_version/{versionId} | Update the default pipeline version of a specific pipeline.
 *PipelineUploadServiceApi* | [**upload_pipeline**](docs/PipelineUploadServiceApi.md#upload_pipeline) | **POST** /apis/v1/pipelines/upload | 
 *PipelineUploadServiceApi* | [**upload_pipeline_version**](docs/PipelineUploadServiceApi.md#upload_pipeline_version) | **POST** /apis/v1/pipelines/upload_version | 
-*RunServiceApi* | [**archive_run**](docs/RunServiceApi.md#archive_run) | **POST** /apis/v1/runs/{id}:archive | Archives a run.
-*RunServiceApi* | [**create_run**](docs/RunServiceApi.md#create_run) | **POST** /apis/v1/runs | Creates a new run.
-*RunServiceApi* | [**delete_run**](docs/RunServiceApi.md#delete_run) | **DELETE** /apis/v1/runs/{id} | Deletes a run.
-*RunServiceApi* | [**get_run**](docs/RunServiceApi.md#get_run) | **GET** /apis/v1/runs/{run_id} | Finds a specific run by ID.
-*RunServiceApi* | [**list_runs**](docs/RunServiceApi.md#list_runs) | **GET** /apis/v1/runs | Finds all runs.
-*RunServiceApi* | [**read_artifact**](docs/RunServiceApi.md#read_artifact) | **GET** /apis/v1/runs/{run_id}/nodes/{node_id}/artifacts/{artifact_name}:read | Finds a run&#39;s artifact data.
-*RunServiceApi* | [**report_run_metrics**](docs/RunServiceApi.md#report_run_metrics) | **POST** /apis/v1/runs/{run_id}:reportMetrics | ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.
-*RunServiceApi* | [**retry_run**](docs/RunServiceApi.md#retry_run) | **POST** /apis/v1/runs/{run_id}/retry | Re-initiates a failed or terminated run.
-*RunServiceApi* | [**terminate_run**](docs/RunServiceApi.md#terminate_run) | **POST** /apis/v1/runs/{run_id}/terminate | Terminates an active run.
-*RunServiceApi* | [**unarchive_run**](docs/RunServiceApi.md#unarchive_run) | **POST** /apis/v1/runs/{id}:unarchive | Restores an archived run.
+*RunServiceApi* | [**run_service_archive_run**](docs/RunServiceApi.md#run_service_archive_run) | **POST** /apis/v1/runs/{id}:archive | Archives a run.
+*RunServiceApi* | [**run_service_create_run**](docs/RunServiceApi.md#run_service_create_run) | **POST** /apis/v1/runs | Creates a new run.
+*RunServiceApi* | [**run_service_delete_run**](docs/RunServiceApi.md#run_service_delete_run) | **DELETE** /apis/v1/runs/{id} | Deletes a run.
+*RunServiceApi* | [**run_service_get_run**](docs/RunServiceApi.md#run_service_get_run) | **GET** /apis/v1/runs/{runId} | Finds a specific run by ID.
+*RunServiceApi* | [**run_service_list_runs**](docs/RunServiceApi.md#run_service_list_runs) | **GET** /apis/v1/runs | Finds all runs.
+*RunServiceApi* | [**run_service_read_artifact**](docs/RunServiceApi.md#run_service_read_artifact) | **GET** /apis/v1/runs/{runId}/nodes/{nodeId}/artifacts/{artifactName}:read | Finds a run&#39;s artifact data.
+*RunServiceApi* | [**run_service_report_run_metrics**](docs/RunServiceApi.md#run_service_report_run_metrics) | **POST** /apis/v1/runs/{runId}:reportMetrics | ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.
+*RunServiceApi* | [**run_service_retry_run**](docs/RunServiceApi.md#run_service_retry_run) | **POST** /apis/v1/runs/{runId}/retry | Re-initiates a failed or terminated run.
+*RunServiceApi* | [**run_service_terminate_run**](docs/RunServiceApi.md#run_service_terminate_run) | **POST** /apis/v1/runs/{runId}/terminate | Terminates an active run.
+*RunServiceApi* | [**run_service_unarchive_run**](docs/RunServiceApi.md#run_service_unarchive_run) | **POST** /apis/v1/runs/{id}:unarchive | Restores an archived run.
 
 
 ## Documentation For Models
 
+ - [GooglerpcStatus](docs/GooglerpcStatus.md)
+ - [InlineObject](docs/InlineObject.md)
  - [JobMode](docs/JobMode.md)
  - [PipelineSpecRuntimeConfig](docs/PipelineSpecRuntimeConfig.md)
  - [ProtobufAny](docs/ProtobufAny.md)
  - [ReportRunMetricsResponseReportRunMetricResult](docs/ReportRunMetricsResponseReportRunMetricResult.md)
  - [ReportRunMetricsResponseReportRunMetricResultStatus](docs/ReportRunMetricsResponseReportRunMetricResultStatus.md)
  - [RunMetricFormat](docs/RunMetricFormat.md)
  - [V1CronSchedule](docs/V1CronSchedule.md)
@@ -157,15 +159,14 @@
  - [V1PeriodicSchedule](docs/V1PeriodicSchedule.md)
  - [V1Pipeline](docs/V1Pipeline.md)
  - [V1PipelineRuntime](docs/V1PipelineRuntime.md)
  - [V1PipelineSpec](docs/V1PipelineSpec.md)
  - [V1PipelineVersion](docs/V1PipelineVersion.md)
  - [V1ReadArtifactResponse](docs/V1ReadArtifactResponse.md)
  - [V1Relationship](docs/V1Relationship.md)
- - [V1ReportRunMetricsRequest](docs/V1ReportRunMetricsRequest.md)
  - [V1ReportRunMetricsResponse](docs/V1ReportRunMetricsResponse.md)
  - [V1ResourceKey](docs/V1ResourceKey.md)
  - [V1ResourceReference](docs/V1ResourceReference.md)
  - [V1ResourceType](docs/V1ResourceType.md)
  - [V1Run](docs/V1Run.md)
  - [V1RunDetail](docs/V1RunDetail.md)
  - [V1RunMetric](docs/V1RunMetric.md)
@@ -184,10 +185,10 @@
 - **Type**: API key
 - **API key parameter name**: authorization
 - **Location**: HTTP header
 
 
 ## Author
 
-prashsh1@in.ibm.com
+kubeflow-pipelines@google.com
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/__init__.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.5.0"
+__version__ = "1.8.0rc1"
 
 # import apis into sdk package
 from kfp_tekton_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_tekton_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_tekton_server_api.api.job_service_api import JobServiceApi
 from kfp_tekton_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
@@ -29,14 +29,16 @@
 from kfp_tekton_server_api.configuration import Configuration
 from kfp_tekton_server_api.exceptions import OpenApiException
 from kfp_tekton_server_api.exceptions import ApiTypeError
 from kfp_tekton_server_api.exceptions import ApiValueError
 from kfp_tekton_server_api.exceptions import ApiKeyError
 from kfp_tekton_server_api.exceptions import ApiException
 # import models into sdk package
+from kfp_tekton_server_api.models.googlerpc_status import GooglerpcStatus
+from kfp_tekton_server_api.models.inline_object import InlineObject
 from kfp_tekton_server_api.models.job_mode import JobMode
 from kfp_tekton_server_api.models.pipeline_spec_runtime_config import PipelineSpecRuntimeConfig
 from kfp_tekton_server_api.models.protobuf_any import ProtobufAny
 from kfp_tekton_server_api.models.report_run_metrics_response_report_run_metric_result import ReportRunMetricsResponseReportRunMetricResult
 from kfp_tekton_server_api.models.report_run_metrics_response_report_run_metric_result_status import ReportRunMetricsResponseReportRunMetricResultStatus
 from kfp_tekton_server_api.models.run_metric_format import RunMetricFormat
 from kfp_tekton_server_api.models.v1_cron_schedule import V1CronSchedule
@@ -54,15 +56,14 @@
 from kfp_tekton_server_api.models.v1_periodic_schedule import V1PeriodicSchedule
 from kfp_tekton_server_api.models.v1_pipeline import V1Pipeline
 from kfp_tekton_server_api.models.v1_pipeline_runtime import V1PipelineRuntime
 from kfp_tekton_server_api.models.v1_pipeline_spec import V1PipelineSpec
 from kfp_tekton_server_api.models.v1_pipeline_version import V1PipelineVersion
 from kfp_tekton_server_api.models.v1_read_artifact_response import V1ReadArtifactResponse
 from kfp_tekton_server_api.models.v1_relationship import V1Relationship
-from kfp_tekton_server_api.models.v1_report_run_metrics_request import V1ReportRunMetricsRequest
 from kfp_tekton_server_api.models.v1_report_run_metrics_response import V1ReportRunMetricsResponse
 from kfp_tekton_server_api.models.v1_resource_key import V1ResourceKey
 from kfp_tekton_server_api.models.v1_resource_reference import V1ResourceReference
 from kfp_tekton_server_api.models.v1_resource_type import V1ResourceType
 from kfp_tekton_server_api.models.v1_run import V1Run
 from kfp_tekton_server_api.models.v1_run_detail import V1RunDetail
 from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/__init__.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/job_service_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -20,65 +20,65 @@
 from kfp_tekton_server_api.api_client import ApiClient
 from kfp_tekton_server_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ExperimentServiceApi(object):
+class JobServiceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def archive_experiment(self, id, **kwargs):  # noqa: E501
-        """Archives an experiment and the experiment's runs and jobs.  # noqa: E501
+    def job_service_create_job(self, job, **kwargs):  # noqa: E501
+        """Creates a new job.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_experiment(id, async_req=True)
+        >>> thread = api.job_service_create_job(job, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be archived. (required)
-        :type id: str
+        :param job: The job to be created (required)
+        :type job: V1Job
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: V1Job
         """
         kwargs['_return_http_data_only'] = True
-        return self.archive_experiment_with_http_info(id, **kwargs)  # noqa: E501
+        return self.job_service_create_job_with_http_info(job, **kwargs)  # noqa: E501
 
-    def archive_experiment_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Archives an experiment and the experiment's runs and jobs.  # noqa: E501
+    def job_service_create_job_with_http_info(self, job, **kwargs):  # noqa: E501
+        """Creates a new job.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.archive_experiment_with_http_info(id, async_req=True)
+        >>> thread = api.job_service_create_job_with_http_info(job, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be archived. (required)
-        :type id: str
+        :param job: The job to be created (required)
+        :type job: V1Job
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -87,120 +87,124 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Job, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'job'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method archive_experiment" % key
+                    " to method job_service_create_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `archive_experiment`")  # noqa: E501
+        # verify the required parameter 'job' is set
+        if self.api_client.client_side_validation and ('job' not in local_var_params or  # noqa: E501
+                                                        local_var_params['job'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `job` when calling `job_service_create_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'job' in local_var_params:
+            body_params = local_var_params['job']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments/{id}:archive', 'POST',
+            '/apis/v1/jobs', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='object',  # noqa: E501
+            response_type='V1Job',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_experiment(self, body, **kwargs):  # noqa: E501
-        """Creates a new experiment.  # noqa: E501
+    def job_service_delete_job(self, id, **kwargs):  # noqa: E501
+        """Deletes a job.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_experiment(body, async_req=True)
+        >>> thread = api.job_service_delete_job(id, async_req=True)
         >>> result = thread.get()
 
-        :param body: The experiment to be created. (required)
-        :type body: V1Experiment
+        :param id: The ID of the job to be deleted (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Experiment
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_experiment_with_http_info(body, **kwargs)  # noqa: E501
+        return self.job_service_delete_job_with_http_info(id, **kwargs)  # noqa: E501
 
-    def create_experiment_with_http_info(self, body, **kwargs):  # noqa: E501
-        """Creates a new experiment.  # noqa: E501
+    def job_service_delete_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Deletes a job.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_experiment_with_http_info(body, async_req=True)
+        >>> thread = api.job_service_delete_job_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param body: The experiment to be created. (required)
-        :type body: V1Experiment
+        :param id: The ID of the job to be deleted (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -209,95 +213,91 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Experiment, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'body'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_experiment" % key
+                    " to method job_service_delete_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'body' is set
-        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
-                                                        local_var_params['body'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `body` when calling `create_experiment`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `job_service_delete_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in local_var_params:
-            body_params = local_var_params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments', 'POST',
+            '/apis/v1/jobs/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1Experiment',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_experiment(self, id, **kwargs):  # noqa: E501
-        """Deletes an experiment without deleting the experiment's runs and jobs. To avoid unexpected behaviors, delete an experiment's runs and jobs before deleting the experiment.  # noqa: E501
+    def job_service_disable_job(self, id, **kwargs):  # noqa: E501
+        """Stops a job and all its associated runs. The job is not deleted.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_experiment(id, async_req=True)
+        >>> thread = api.job_service_disable_job(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be deleted. (required)
+        :param id: The ID of the job to be disabled (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -306,26 +306,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_experiment_with_http_info(id, **kwargs)  # noqa: E501
+        return self.job_service_disable_job_with_http_info(id, **kwargs)  # noqa: E501
 
-    def delete_experiment_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Deletes an experiment without deleting the experiment's runs and jobs. To avoid unexpected behaviors, delete an experiment's runs and jobs before deleting the experiment.  # noqa: E501
+    def job_service_disable_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Stops a job and all its associated runs. The job is not deleted.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_experiment_with_http_info(id, async_req=True)
+        >>> thread = api.job_service_disable_job_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be deleted. (required)
+        :param id: The ID of the job to be disabled (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -356,22 +356,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_experiment" % key
+                    " to method job_service_disable_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `delete_experiment`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `job_service_disable_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -387,67 +387,67 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments/{id}', 'DELETE',
+            '/apis/v1/jobs/{id}/disable', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_experiment(self, id, **kwargs):  # noqa: E501
-        """Finds a specific experiment by ID.  # noqa: E501
+    def job_service_enable_job(self, id, **kwargs):  # noqa: E501
+        """Restarts a job that was previously stopped. All runs associated with the job will continue.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_experiment(id, async_req=True)
+        >>> thread = api.job_service_enable_job(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be retrieved. (required)
+        :param id: The ID of the job to be enabled (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Experiment
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_experiment_with_http_info(id, **kwargs)  # noqa: E501
+        return self.job_service_enable_job_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_experiment_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Finds a specific experiment by ID.  # noqa: E501
+    def job_service_enable_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Restarts a job that was previously stopped. All runs associated with the job will continue.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_experiment_with_http_info(id, async_req=True)
+        >>> thread = api.job_service_enable_job_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be retrieved. (required)
+        :param id: The ID of the job to be enabled (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -457,15 +457,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Experiment, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'id'
         ]
@@ -478,22 +478,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_experiment" % key
+                    " to method job_service_enable_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_experiment`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `job_service_enable_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -509,88 +509,68 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments/{id}', 'GET',
+            '/apis/v1/jobs/{id}/enable', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1Experiment',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_experiment(self, **kwargs):  # noqa: E501
-        """Finds all experiments. Supports pagination, and sorting on certain fields.  # noqa: E501
+    def job_service_get_job(self, id, **kwargs):  # noqa: E501
+        """Finds a specific job by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_experiment(async_req=True)
+        >>> thread = api.job_service_get_job(id, async_req=True)
         >>> result = thread.get()
 
-        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListExperiment call or can be omitted when fetching the first page.
-        :type page_token: str
-        :param page_size: The number of experiments to be listed per page. If there are more experiments than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
-        :type page_size: int
-        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" Ascending by default.
-        :type sort_by: str
-        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
-        :type filter: str
-        :param resource_reference_key_type: The type of the resource that referred to.
-        :type resource_reference_key_type: str
-        :param resource_reference_key_id: The ID of the resource that referred to.
-        :type resource_reference_key_id: str
+        :param id: The ID of the job to be retrieved (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListExperimentsResponse
+        :rtype: V1Job
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_experiment_with_http_info(**kwargs)  # noqa: E501
+        return self.job_service_get_job_with_http_info(id, **kwargs)  # noqa: E501
 
-    def list_experiment_with_http_info(self, **kwargs):  # noqa: E501
-        """Finds all experiments. Supports pagination, and sorting on certain fields.  # noqa: E501
+    def job_service_get_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Finds a specific job by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_experiment_with_http_info(async_req=True)
+        >>> thread = api.job_service_get_job_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListExperiment call or can be omitted when fetching the first page.
-        :type page_token: str
-        :param page_size: The number of experiments to be listed per page. If there are more experiments than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
-        :type page_size: int
-        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" Ascending by default.
-        :type sort_by: str
-        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
-        :type filter: str
-        :param resource_reference_key_type: The type of the resource that referred to.
-        :type resource_reference_key_type: str
-        :param resource_reference_key_id: The ID of the resource that referred to.
-        :type resource_reference_key_id: str
+        :param id: The ID of the job to be retrieved (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -599,62 +579,51 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListExperimentsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1Job, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'page_token',
-            'page_size',
-            'sort_by',
-            'filter',
-            'resource_reference_key_type',
-            'resource_reference_key_id'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_experiment" % key
+                    " to method job_service_get_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `job_service_get_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
-            query_params.append(('page_token', local_var_params['page_token']))  # noqa: E501
-        if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
-            query_params.append(('page_size', local_var_params['page_size']))  # noqa: E501
-        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
-            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
-        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
-            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
-        if 'resource_reference_key_type' in local_var_params and local_var_params['resource_reference_key_type'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.type', local_var_params['resource_reference_key_type']))  # noqa: E501
-        if 'resource_reference_key_id' in local_var_params and local_var_params['resource_reference_key_id'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.id', local_var_params['resource_reference_key_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -662,68 +631,88 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments', 'GET',
+            '/apis/v1/jobs/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1ListExperimentsResponse',  # noqa: E501
+            response_type='V1Job',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def unarchive_experiment(self, id, **kwargs):  # noqa: E501
-        """Restores an archived experiment. The experiment's archived runs and jobs will stay archived.  # noqa: E501
+    def job_service_list_jobs(self, **kwargs):  # noqa: E501
+        """Finds all jobs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unarchive_experiment(id, async_req=True)
+        >>> thread = api.job_service_list_jobs(async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be restored. (required)
-        :type id: str
+        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListJobs call or can be omitted when fetching the first page.
+        :type page_token: str
+        :param page_size: The number of jobs to be listed per page. If there are more jobs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
+        :type page_size: int
+        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\". Ascending by default.
+        :type sort_by: str
+        :param resource_reference_key_type: The type of the resource that referred to.
+        :type resource_reference_key_type: str
+        :param resource_reference_key_id: The ID of the resource that referred to.
+        :type resource_reference_key_id: str
+        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
+        :type filter: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: V1ListJobsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.unarchive_experiment_with_http_info(id, **kwargs)  # noqa: E501
+        return self.job_service_list_jobs_with_http_info(**kwargs)  # noqa: E501
 
-    def unarchive_experiment_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Restores an archived experiment. The experiment's archived runs and jobs will stay archived.  # noqa: E501
+    def job_service_list_jobs_with_http_info(self, **kwargs):  # noqa: E501
+        """Finds all jobs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unarchive_experiment_with_http_info(id, async_req=True)
+        >>> thread = api.job_service_list_jobs_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the experiment to be restored. (required)
-        :type id: str
+        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListJobs call or can be omitted when fetching the first page.
+        :type page_token: str
+        :param page_size: The number of jobs to be listed per page. If there are more jobs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
+        :type page_size: int
+        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\". Ascending by default.
+        :type sort_by: str
+        :param resource_reference_key_type: The type of the resource that referred to.
+        :type resource_reference_key_type: str
+        :param resource_reference_key_id: The ID of the resource that referred to.
+        :type resource_reference_key_id: str
+        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
+        :type filter: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -732,51 +721,62 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1ListJobsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'page_token',
+            'page_size',
+            'sort_by',
+            'resource_reference_key_type',
+            'resource_reference_key_id',
+            'filter'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method unarchive_experiment" % key
+                    " to method job_service_list_jobs" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `unarchive_experiment`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
+        if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
+            query_params.append(('pageToken', local_var_params['page_token']))  # noqa: E501
+        if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
+            query_params.append(('pageSize', local_var_params['page_size']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sortBy', local_var_params['sort_by']))  # noqa: E501
+        if 'resource_reference_key_type' in local_var_params and local_var_params['resource_reference_key_type'] is not None:  # noqa: E501
+            query_params.append(('resourceReferenceKey.type', local_var_params['resource_reference_key_type']))  # noqa: E501
+        if 'resource_reference_key_id' in local_var_params and local_var_params['resource_reference_key_id'] is not None:  # noqa: E501
+            query_params.append(('resourceReferenceKey.id', local_var_params['resource_reference_key_id']))  # noqa: E501
+        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
+            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -784,21 +784,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/experiments/{id}:unarchive', 'POST',
+            '/apis/v1/jobs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='object',  # noqa: E501
+            response_type='V1ListJobsResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/healthz_service_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -32,21 +32,21 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_healthz(self, **kwargs):  # noqa: E501
+    def healthz_service_get_healthz(self, **kwargs):  # noqa: E501
         """Get healthz data.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_healthz(async_req=True)
+        >>> thread = api.healthz_service_get_healthz(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -56,23 +56,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1GetHealthzResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_healthz_with_http_info(**kwargs)  # noqa: E501
+        return self.healthz_service_get_healthz_with_http_info(**kwargs)  # noqa: E501
 
-    def get_healthz_with_http_info(self, **kwargs):  # noqa: E501
+    def healthz_service_get_healthz_with_http_info(self, **kwargs):  # noqa: E501
         """Get healthz data.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_healthz_with_http_info(async_req=True)
+        >>> thread = api.healthz_service_get_healthz_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -103,15 +103,15 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_healthz" % key
+                    " to method healthz_service_get_healthz" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/job_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/run_service_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -20,65 +20,65 @@
 from kfp_tekton_server_api.api_client import ApiClient
 from kfp_tekton_server_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class JobServiceApi(object):
+class RunServiceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_job(self, body, **kwargs):  # noqa: E501
-        """Creates a new job.  # noqa: E501
+    def run_service_archive_run(self, id, **kwargs):  # noqa: E501
+        """Archives a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_job(body, async_req=True)
+        >>> thread = api.run_service_archive_run(id, async_req=True)
         >>> result = thread.get()
 
-        :param body: The job to be created (required)
-        :type body: V1Job
+        :param id: The ID of the run to be archived. (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Job
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_job_with_http_info(body, **kwargs)  # noqa: E501
+        return self.run_service_archive_run_with_http_info(id, **kwargs)  # noqa: E501
 
-    def create_job_with_http_info(self, body, **kwargs):  # noqa: E501
-        """Creates a new job.  # noqa: E501
+    def run_service_archive_run_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Archives a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_job_with_http_info(body, async_req=True)
+        >>> thread = api.run_service_archive_run_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param body: The job to be created (required)
-        :type body: V1Job
+        :param id: The ID of the run to be archived. (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -87,95 +87,217 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Job, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'body'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_job" % key
+                    " to method run_service_archive_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'body' is set
-        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
-                                                        local_var_params['body'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `body` when calling `create_job`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `run_service_archive_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in local_var_params:
-            body_params = local_var_params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/apis/v1/runs/{id}:archive', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='object',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def run_service_create_run(self, run, **kwargs):  # noqa: E501
+        """Creates a new run.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_create_run(run, async_req=True)
+        >>> result = thread.get()
+
+        :param run: (required)
+        :type run: V1Run
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1RunDetail
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.run_service_create_run_with_http_info(run, **kwargs)  # noqa: E501
+
+    def run_service_create_run_with_http_info(self, run, **kwargs):  # noqa: E501
+        """Creates a new run.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_create_run_with_http_info(run, async_req=True)
+        >>> result = thread.get()
+
+        :param run: (required)
+        :type run: V1Run
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1RunDetail, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'run'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method run_service_create_run" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'run' is set
+        if self.api_client.client_side_validation and ('run' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run` when calling `run_service_create_run`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'run' in local_var_params:
+            body_params = local_var_params['run']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs', 'POST',
+            '/apis/v1/runs', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1Job',  # noqa: E501
+            response_type='V1RunDetail',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_job(self, id, **kwargs):  # noqa: E501
-        """Deletes a job.  # noqa: E501
+    def run_service_delete_run(self, id, **kwargs):  # noqa: E501
+        """Deletes a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_job(id, async_req=True)
+        >>> thread = api.run_service_delete_run(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be deleted (required)
+        :param id: The ID of the run to be deleted. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -184,26 +306,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_job_with_http_info(id, **kwargs)  # noqa: E501
+        return self.run_service_delete_run_with_http_info(id, **kwargs)  # noqa: E501
 
-    def delete_job_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Deletes a job.  # noqa: E501
+    def run_service_delete_run_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Deletes a run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_job_with_http_info(id, async_req=True)
+        >>> thread = api.run_service_delete_run_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be deleted (required)
+        :param id: The ID of the run to be deleted. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -234,22 +356,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_job" % key
+                    " to method run_service_delete_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `delete_job`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `run_service_delete_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -265,68 +387,68 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs/{id}', 'DELETE',
+            '/apis/v1/runs/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def disable_job(self, id, **kwargs):  # noqa: E501
-        """Stops a job and all its associated runs. The job is not deleted.  # noqa: E501
+    def run_service_get_run(self, run_id, **kwargs):  # noqa: E501
+        """Finds a specific run by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.disable_job(id, async_req=True)
+        >>> thread = api.run_service_get_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be disabled (required)
-        :type id: str
+        :param run_id: The ID of the run to be retrieved. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: V1RunDetail
         """
         kwargs['_return_http_data_only'] = True
-        return self.disable_job_with_http_info(id, **kwargs)  # noqa: E501
+        return self.run_service_get_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def disable_job_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Stops a job and all its associated runs. The job is not deleted.  # noqa: E501
+    def run_service_get_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
+        """Finds a specific run by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.disable_job_with_http_info(id, async_req=True)
+        >>> thread = api.run_service_get_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be disabled (required)
-        :type id: str
+        :param run_id: The ID of the run to be retrieved. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -335,49 +457,49 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1RunDetail, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method disable_job" % key
+                    " to method run_service_get_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `disable_job`")  # noqa: E501
+        # verify the required parameter 'run_id' is set
+        if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_id` when calling `run_service_get_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'run_id' in local_var_params:
+            path_params['runId'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -387,40 +509,474 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs/{id}/disable', 'POST',
+            '/apis/v1/runs/{runId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='object',  # noqa: E501
+            response_type='V1RunDetail',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def enable_job(self, id, **kwargs):  # noqa: E501
-        """Restarts a job that was previously stopped. All runs associated with the job will continue.  # noqa: E501
+    def run_service_list_runs(self, **kwargs):  # noqa: E501
+        """Finds all runs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.enable_job(id, async_req=True)
+        >>> thread = api.run_service_list_runs(async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be enabled (required)
-        :type id: str
+        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListRuns call or can be omitted when fetching the first page.
+        :type page_token: str
+        :param page_size: The number of runs to be listed per page. If there are more runs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
+        :type page_size: int
+        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" (Example, \"name asc\" or \"id desc\"). Ascending by default.
+        :type sort_by: str
+        :param resource_reference_key_type: The type of the resource that referred to.
+        :type resource_reference_key_type: str
+        :param resource_reference_key_id: The ID of the resource that referred to.
+        :type resource_reference_key_id: str
+        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
+        :type filter: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1ListRunsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.run_service_list_runs_with_http_info(**kwargs)  # noqa: E501
+
+    def run_service_list_runs_with_http_info(self, **kwargs):  # noqa: E501
+        """Finds all runs.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_list_runs_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListRuns call or can be omitted when fetching the first page.
+        :type page_token: str
+        :param page_size: The number of runs to be listed per page. If there are more runs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
+        :type page_size: int
+        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" (Example, \"name asc\" or \"id desc\"). Ascending by default.
+        :type sort_by: str
+        :param resource_reference_key_type: The type of the resource that referred to.
+        :type resource_reference_key_type: str
+        :param resource_reference_key_id: The ID of the resource that referred to.
+        :type resource_reference_key_id: str
+        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
+        :type filter: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1ListRunsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'page_token',
+            'page_size',
+            'sort_by',
+            'resource_reference_key_type',
+            'resource_reference_key_id',
+            'filter'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method run_service_list_runs" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
+            query_params.append(('pageToken', local_var_params['page_token']))  # noqa: E501
+        if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
+            query_params.append(('pageSize', local_var_params['page_size']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sortBy', local_var_params['sort_by']))  # noqa: E501
+        if 'resource_reference_key_type' in local_var_params and local_var_params['resource_reference_key_type'] is not None:  # noqa: E501
+            query_params.append(('resourceReferenceKey.type', local_var_params['resource_reference_key_type']))  # noqa: E501
+        if 'resource_reference_key_id' in local_var_params and local_var_params['resource_reference_key_id'] is not None:  # noqa: E501
+            query_params.append(('resourceReferenceKey.id', local_var_params['resource_reference_key_id']))  # noqa: E501
+        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
+            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/apis/v1/runs', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='V1ListRunsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def run_service_read_artifact(self, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
+        """Finds a run's artifact data.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_read_artifact(run_id, node_id, artifact_name, async_req=True)
+        >>> result = thread.get()
+
+        :param run_id: The ID of the run. (required)
+        :type run_id: str
+        :param node_id: The ID of the running node. (required)
+        :type node_id: str
+        :param artifact_name: The name of the artifact. (required)
+        :type artifact_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1ReadArtifactResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.run_service_read_artifact_with_http_info(run_id, node_id, artifact_name, **kwargs)  # noqa: E501
+
+    def run_service_read_artifact_with_http_info(self, run_id, node_id, artifact_name, **kwargs):  # noqa: E501
+        """Finds a run's artifact data.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_read_artifact_with_http_info(run_id, node_id, artifact_name, async_req=True)
+        >>> result = thread.get()
+
+        :param run_id: The ID of the run. (required)
+        :type run_id: str
+        :param node_id: The ID of the running node. (required)
+        :type node_id: str
+        :param artifact_name: The name of the artifact. (required)
+        :type artifact_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1ReadArtifactResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'run_id',
+            'node_id',
+            'artifact_name'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method run_service_read_artifact" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'run_id' is set
+        if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_id` when calling `run_service_read_artifact`")  # noqa: E501
+        # verify the required parameter 'node_id' is set
+        if self.api_client.client_side_validation and ('node_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['node_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `node_id` when calling `run_service_read_artifact`")  # noqa: E501
+        # verify the required parameter 'artifact_name' is set
+        if self.api_client.client_side_validation and ('artifact_name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['artifact_name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `artifact_name` when calling `run_service_read_artifact`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'run_id' in local_var_params:
+            path_params['runId'] = local_var_params['run_id']  # noqa: E501
+        if 'node_id' in local_var_params:
+            path_params['nodeId'] = local_var_params['node_id']  # noqa: E501
+        if 'artifact_name' in local_var_params:
+            path_params['artifactName'] = local_var_params['artifact_name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/apis/v1/runs/{runId}/nodes/{nodeId}/artifacts/{artifactName}:read', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='V1ReadArtifactResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def run_service_report_run_metrics(self, run_id, body, **kwargs):  # noqa: E501
+        """ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_report_run_metrics(run_id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param run_id: Required. The parent run ID of the metric. (required)
+        :type run_id: str
+        :param body: (required)
+        :type body: InlineObject
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1ReportRunMetricsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.run_service_report_run_metrics_with_http_info(run_id, body, **kwargs)  # noqa: E501
+
+    def run_service_report_run_metrics_with_http_info(self, run_id, body, **kwargs):  # noqa: E501
+        """ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_report_run_metrics_with_http_info(run_id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param run_id: Required. The parent run ID of the metric. (required)
+        :type run_id: str
+        :param body: (required)
+        :type body: InlineObject
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1ReportRunMetricsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'run_id',
+            'body'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method run_service_report_run_metrics" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'run_id' is set
+        if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_id` when calling `run_service_report_run_metrics`")  # noqa: E501
+        # verify the required parameter 'body' is set
+        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
+                                                        local_var_params['body'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `body` when calling `run_service_report_run_metrics`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'run_id' in local_var_params:
+            path_params['runId'] = local_var_params['run_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/apis/v1/runs/{runId}:reportMetrics', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='V1ReportRunMetricsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def run_service_retry_run(self, run_id, **kwargs):  # noqa: E501
+        """Re-initiates a failed or terminated run.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.run_service_retry_run(run_id, async_req=True)
+        >>> result = thread.get()
+
+        :param run_id: The ID of the run to be retried. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -428,27 +984,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.enable_job_with_http_info(id, **kwargs)  # noqa: E501
+        return self.run_service_retry_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def enable_job_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Restarts a job that was previously stopped. All runs associated with the job will continue.  # noqa: E501
+    def run_service_retry_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
+        """Re-initiates a failed or terminated run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.enable_job_with_http_info(id, async_req=True)
+        >>> thread = api.run_service_retry_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be enabled (required)
-        :type id: str
+        :param run_id: The ID of the run to be retried. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -463,43 +1019,43 @@
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method enable_job" % key
+                    " to method run_service_retry_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `enable_job`")  # noqa: E501
+        # verify the required parameter 'run_id' is set
+        if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_id` when calling `run_service_retry_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'run_id' in local_var_params:
+            path_params['runId'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -509,68 +1065,68 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs/{id}/enable', 'POST',
+            '/apis/v1/runs/{runId}/retry', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_job(self, id, **kwargs):  # noqa: E501
-        """Finds a specific job by ID.  # noqa: E501
+    def run_service_terminate_run(self, run_id, **kwargs):  # noqa: E501
+        """Terminates an active run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_job(id, async_req=True)
+        >>> thread = api.run_service_terminate_run(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be retrieved (required)
-        :type id: str
+        :param run_id: The ID of the run to be terminated. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1Job
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_job_with_http_info(id, **kwargs)  # noqa: E501
+        return self.run_service_terminate_run_with_http_info(run_id, **kwargs)  # noqa: E501
 
-    def get_job_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Finds a specific job by ID.  # noqa: E501
+    def run_service_terminate_run_with_http_info(self, run_id, **kwargs):  # noqa: E501
+        """Terminates an active run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_job_with_http_info(id, async_req=True)
+        >>> thread = api.run_service_terminate_run_with_http_info(run_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The ID of the job to be retrieved (required)
-        :type id: str
+        :param run_id: The ID of the run to be terminated. (required)
+        :type run_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -579,49 +1135,49 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1Job, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'run_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_job" % key
+                    " to method run_service_terminate_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_job`")  # noqa: E501
+        # verify the required parameter 'run_id' is set
+        if self.api_client.client_side_validation and ('run_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_id` when calling `run_service_terminate_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'run_id' in local_var_params:
+            path_params['runId'] = local_var_params['run_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -631,88 +1187,68 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs/{id}', 'GET',
+            '/apis/v1/runs/{runId}/terminate', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1Job',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_jobs(self, **kwargs):  # noqa: E501
-        """Finds all jobs.  # noqa: E501
+    def run_service_unarchive_run(self, id, **kwargs):  # noqa: E501
+        """Restores an archived run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_jobs(async_req=True)
+        >>> thread = api.run_service_unarchive_run(id, async_req=True)
         >>> result = thread.get()
 
-        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListJobs call or can be omitted when fetching the first page.
-        :type page_token: str
-        :param page_size: The number of jobs to be listed per page. If there are more jobs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
-        :type page_size: int
-        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\". Ascending by default.
-        :type sort_by: str
-        :param resource_reference_key_type: The type of the resource that referred to.
-        :type resource_reference_key_type: str
-        :param resource_reference_key_id: The ID of the resource that referred to.
-        :type resource_reference_key_id: str
-        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
-        :type filter: str
+        :param id: The ID of the run to be restored. (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListJobsResponse
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_jobs_with_http_info(**kwargs)  # noqa: E501
+        return self.run_service_unarchive_run_with_http_info(id, **kwargs)  # noqa: E501
 
-    def list_jobs_with_http_info(self, **kwargs):  # noqa: E501
-        """Finds all jobs.  # noqa: E501
+    def run_service_unarchive_run_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Restores an archived run.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_jobs_with_http_info(async_req=True)
+        >>> thread = api.run_service_unarchive_run_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListJobs call or can be omitted when fetching the first page.
-        :type page_token: str
-        :param page_size: The number of jobs to be listed per page. If there are more jobs than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
-        :type page_size: int
-        :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\". Ascending by default.
-        :type sort_by: str
-        :param resource_reference_key_type: The type of the resource that referred to.
-        :type resource_reference_key_type: str
-        :param resource_reference_key_id: The ID of the resource that referred to.
-        :type resource_reference_key_id: str
-        :param filter: A url-encoded, JSON-serialized Filter protocol buffer (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/v1/filter.proto)).
-        :type filter: str
+        :param id: The ID of the run to be restored. (required)
+        :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -721,62 +1257,51 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListJobsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'page_token',
-            'page_size',
-            'sort_by',
-            'resource_reference_key_type',
-            'resource_reference_key_id',
-            'filter'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_jobs" % key
+                    " to method run_service_unarchive_run" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `run_service_unarchive_run`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
-            query_params.append(('page_token', local_var_params['page_token']))  # noqa: E501
-        if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
-            query_params.append(('page_size', local_var_params['page_size']))  # noqa: E501
-        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
-            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
-        if 'resource_reference_key_type' in local_var_params and local_var_params['resource_reference_key_type'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.type', local_var_params['resource_reference_key_type']))  # noqa: E501
-        if 'resource_reference_key_id' in local_var_params and local_var_params['resource_reference_key_id'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.id', local_var_params['resource_reference_key_id']))  # noqa: E501
-        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
-            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -784,21 +1309,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/jobs', 'GET',
+            '/apis/v1/runs/{id}:unarchive', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='V1ListJobsResponse',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_service_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -32,25 +32,25 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_pipeline(self, body, **kwargs):  # noqa: E501
+    def pipeline_service_create_pipeline(self, pipeline, **kwargs):  # noqa: E501
         """Creates a pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline(body, async_req=True)
+        >>> thread = api.pipeline_service_create_pipeline(pipeline, async_req=True)
         >>> result = thread.get()
 
-        :param body: (required)
-        :type body: V1Pipeline
+        :param pipeline: (required)
+        :type pipeline: V1Pipeline
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -58,27 +58,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1Pipeline
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_pipeline_with_http_info(body, **kwargs)  # noqa: E501
+        return self.pipeline_service_create_pipeline_with_http_info(pipeline, **kwargs)  # noqa: E501
 
-    def create_pipeline_with_http_info(self, body, **kwargs):  # noqa: E501
+    def pipeline_service_create_pipeline_with_http_info(self, pipeline, **kwargs):  # noqa: E501
         """Creates a pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline_with_http_info(body, async_req=True)
+        >>> thread = api.pipeline_service_create_pipeline_with_http_info(pipeline, async_req=True)
         >>> result = thread.get()
 
-        :param body: (required)
-        :type body: V1Pipeline
+        :param pipeline: (required)
+        :type pipeline: V1Pipeline
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -93,52 +93,52 @@
                  returns the request thread.
         :rtype: tuple(V1Pipeline, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'body'
+            'pipeline'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_pipeline" % key
+                    " to method pipeline_service_create_pipeline" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'body' is set
-        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
-                                                        local_var_params['body'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `body` when calling `create_pipeline`")  # noqa: E501
+        # verify the required parameter 'pipeline' is set
+        if self.api_client.client_side_validation and ('pipeline' not in local_var_params or  # noqa: E501
+                                                        local_var_params['pipeline'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `pipeline` when calling `pipeline_service_create_pipeline`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in local_var_params:
-            body_params = local_var_params['body']
+        if 'pipeline' in local_var_params:
+            body_params = local_var_params['pipeline']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
@@ -158,25 +158,25 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_pipeline_version(self, body, **kwargs):  # noqa: E501
+    def pipeline_service_create_pipeline_version(self, version, **kwargs):  # noqa: E501
         """Adds a pipeline version to the specified pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline_version(body, async_req=True)
+        >>> thread = api.pipeline_service_create_pipeline_version(version, async_req=True)
         >>> result = thread.get()
 
-        :param body: ResourceReference inside PipelineVersion specifies the pipeline that this version belongs to. (required)
-        :type body: V1PipelineVersion
+        :param version: ResourceReference inside PipelineVersion specifies the pipeline that this version belongs to. (required)
+        :type version: V1PipelineVersion
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -184,27 +184,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1PipelineVersion
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_pipeline_version_with_http_info(body, **kwargs)  # noqa: E501
+        return self.pipeline_service_create_pipeline_version_with_http_info(version, **kwargs)  # noqa: E501
 
-    def create_pipeline_version_with_http_info(self, body, **kwargs):  # noqa: E501
+    def pipeline_service_create_pipeline_version_with_http_info(self, version, **kwargs):  # noqa: E501
         """Adds a pipeline version to the specified pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_pipeline_version_with_http_info(body, async_req=True)
+        >>> thread = api.pipeline_service_create_pipeline_version_with_http_info(version, async_req=True)
         >>> result = thread.get()
 
-        :param body: ResourceReference inside PipelineVersion specifies the pipeline that this version belongs to. (required)
-        :type body: V1PipelineVersion
+        :param version: ResourceReference inside PipelineVersion specifies the pipeline that this version belongs to. (required)
+        :type version: V1PipelineVersion
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -219,52 +219,52 @@
                  returns the request thread.
         :rtype: tuple(V1PipelineVersion, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'body'
+            'version'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_pipeline_version" % key
+                    " to method pipeline_service_create_pipeline_version" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'body' is set
-        if self.api_client.client_side_validation and ('body' not in local_var_params or  # noqa: E501
-                                                        local_var_params['body'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `body` when calling `create_pipeline_version`")  # noqa: E501
+        # verify the required parameter 'version' is set
+        if self.api_client.client_side_validation and ('version' not in local_var_params or  # noqa: E501
+                                                        local_var_params['version'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version` when calling `pipeline_service_create_pipeline_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in local_var_params:
-            body_params = local_var_params['body']
+        if 'version' in local_var_params:
+            body_params = local_var_params['version']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
@@ -284,21 +284,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_pipeline(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_delete_pipeline(self, id, **kwargs):  # noqa: E501
         """Deletes a pipeline and its pipeline versions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_pipeline(id, async_req=True)
+        >>> thread = api.pipeline_service_delete_pipeline(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline to be deleted. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -310,23 +310,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_pipeline_with_http_info(id, **kwargs)  # noqa: E501
+        return self.pipeline_service_delete_pipeline_with_http_info(id, **kwargs)  # noqa: E501
 
-    def delete_pipeline_with_http_info(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_delete_pipeline_with_http_info(self, id, **kwargs):  # noqa: E501
         """Deletes a pipeline and its pipeline versions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_pipeline_with_http_info(id, async_req=True)
+        >>> thread = api.pipeline_service_delete_pipeline_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline to be deleted. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -360,22 +360,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_pipeline" % key
+                    " to method pipeline_service_delete_pipeline" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `delete_pipeline`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `pipeline_service_delete_pipeline`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -406,21 +406,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_pipeline_version(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_delete_pipeline_version(self, version_id, **kwargs):  # noqa: E501
         """Deletes a pipeline version by pipeline version ID. If the deleted pipeline version is the default pipeline version, the pipeline's default version changes to the pipeline's most recent pipeline version. If there are no remaining pipeline versions, the pipeline will have no default version. Examines the run_service_api.ipynb notebook to learn more about creating a run using a pipeline version (https://github.com/kubeflow/pipelines/blob/master/tools/benchmarks/run_service_api.ipynb).  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_pipeline_version(version_id, async_req=True)
+        >>> thread = api.pipeline_service_delete_pipeline_version(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version to be deleted. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -432,23 +432,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_pipeline_version_with_http_info(version_id, **kwargs)  # noqa: E501
+        return self.pipeline_service_delete_pipeline_version_with_http_info(version_id, **kwargs)  # noqa: E501
 
-    def delete_pipeline_version_with_http_info(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_delete_pipeline_version_with_http_info(self, version_id, **kwargs):  # noqa: E501
         """Deletes a pipeline version by pipeline version ID. If the deleted pipeline version is the default pipeline version, the pipeline's default version changes to the pipeline's most recent pipeline version. If there are no remaining pipeline versions, the pipeline will have no default version. Examines the run_service_api.ipynb notebook to learn more about creating a run using a pipeline version (https://github.com/kubeflow/pipelines/blob/master/tools/benchmarks/run_service_api.ipynb).  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_pipeline_version_with_http_info(version_id, async_req=True)
+        >>> thread = api.pipeline_service_delete_pipeline_version_with_http_info(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version to be deleted. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -482,28 +482,28 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_pipeline_version" % key
+                    " to method pipeline_service_delete_pipeline_version" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'version_id' is set
         if self.api_client.client_side_validation and ('version_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['version_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `version_id` when calling `delete_pipeline_version`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version_id` when calling `pipeline_service_delete_pipeline_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'version_id' in local_var_params:
-            path_params['version_id'] = local_var_params['version_id']  # noqa: E501
+            path_params['versionId'] = local_var_params['version_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -513,36 +513,36 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/pipeline_versions/{version_id}', 'DELETE',
+            '/apis/v1/pipeline_versions/{versionId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_pipeline(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline(self, id, **kwargs):  # noqa: E501
         """Finds a specific pipeline by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline(id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline to be retrieved. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -554,23 +554,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1Pipeline
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_pipeline_with_http_info(id, **kwargs)  # noqa: E501
+        return self.pipeline_service_get_pipeline_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_pipeline_with_http_info(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline_with_http_info(self, id, **kwargs):  # noqa: E501
         """Finds a specific pipeline by ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline_with_http_info(id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline to be retrieved. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -604,22 +604,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_pipeline" % key
+                    " to method pipeline_service_get_pipeline" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_pipeline`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `pipeline_service_get_pipeline`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -650,21 +650,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_pipeline_version(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline_version(self, version_id, **kwargs):  # noqa: E501
         """Gets a pipeline version by pipeline version ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline_version(version_id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline_version(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version to be retrieved. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -676,23 +676,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1PipelineVersion
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_pipeline_version_with_http_info(version_id, **kwargs)  # noqa: E501
+        return self.pipeline_service_get_pipeline_version_with_http_info(version_id, **kwargs)  # noqa: E501
 
-    def get_pipeline_version_with_http_info(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline_version_with_http_info(self, version_id, **kwargs):  # noqa: E501
         """Gets a pipeline version by pipeline version ID.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline_version_with_http_info(version_id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline_version_with_http_info(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version to be retrieved. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -726,28 +726,28 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_pipeline_version" % key
+                    " to method pipeline_service_get_pipeline_version" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'version_id' is set
         if self.api_client.client_side_validation and ('version_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['version_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `version_id` when calling `get_pipeline_version`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version_id` when calling `pipeline_service_get_pipeline_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'version_id' in local_var_params:
-            path_params['version_id'] = local_var_params['version_id']  # noqa: E501
+            path_params['versionId'] = local_var_params['version_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -757,36 +757,36 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/pipeline_versions/{version_id}', 'GET',
+            '/apis/v1/pipeline_versions/{versionId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V1PipelineVersion',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_pipeline_version_template(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline_version_template(self, version_id, **kwargs):  # noqa: E501
         """Returns a YAML template that contains the specified pipeline version's description, parameters and metadata.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline_version_template(version_id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline_version_template(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version whose template is to be retrieved. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -798,23 +798,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1GetTemplateResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_pipeline_version_template_with_http_info(version_id, **kwargs)  # noqa: E501
+        return self.pipeline_service_get_pipeline_version_template_with_http_info(version_id, **kwargs)  # noqa: E501
 
-    def get_pipeline_version_template_with_http_info(self, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_get_pipeline_version_template_with_http_info(self, version_id, **kwargs):  # noqa: E501
         """Returns a YAML template that contains the specified pipeline version's description, parameters and metadata.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_pipeline_version_template_with_http_info(version_id, async_req=True)
+        >>> thread = api.pipeline_service_get_pipeline_version_template_with_http_info(version_id, async_req=True)
         >>> result = thread.get()
 
         :param version_id: The ID of the pipeline version whose template is to be retrieved. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -848,28 +848,28 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_pipeline_version_template" % key
+                    " to method pipeline_service_get_pipeline_version_template" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'version_id' is set
         if self.api_client.client_side_validation and ('version_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['version_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `version_id` when calling `get_pipeline_version_template`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version_id` when calling `pipeline_service_get_pipeline_version_template`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'version_id' in local_var_params:
-            path_params['version_id'] = local_var_params['version_id']  # noqa: E501
+            path_params['versionId'] = local_var_params['version_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -879,36 +879,36 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/pipeline_versions/{version_id}/templates', 'GET',
+            '/apis/v1/pipeline_versions/{versionId}/templates', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='V1GetTemplateResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_template(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_get_template(self, id, **kwargs):  # noqa: E501
         """Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_template(id, async_req=True)
+        >>> thread = api.pipeline_service_get_template(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline whose template is to be retrieved. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -920,23 +920,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1GetTemplateResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_template_with_http_info(id, **kwargs)  # noqa: E501
+        return self.pipeline_service_get_template_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_template_with_http_info(self, id, **kwargs):  # noqa: E501
+    def pipeline_service_get_template_with_http_info(self, id, **kwargs):  # noqa: E501
         """Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_template_with_http_info(id, async_req=True)
+        >>> thread = api.pipeline_service_get_template_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: The ID of the pipeline whose template is to be retrieved. (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -970,22 +970,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_template" % key
+                    " to method pipeline_service_get_template" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_template`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `pipeline_service_get_template`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -1016,21 +1016,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_pipeline_versions(self, **kwargs):  # noqa: E501
+    def pipeline_service_list_pipeline_versions(self, **kwargs):  # noqa: E501
         """Lists all pipeline versions of a given pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_pipeline_versions(async_req=True)
+        >>> thread = api.pipeline_service_list_pipeline_versions(async_req=True)
         >>> result = thread.get()
 
         :param resource_key_type: The type of the resource that referred to.
         :type resource_key_type: str
         :param resource_key_id: The ID of the resource that referred to.
         :type resource_key_id: str
         :param page_size: The number of pipeline versions to be listed per page. If there are more pipeline versions than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
@@ -1052,23 +1052,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1ListPipelineVersionsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_pipeline_versions_with_http_info(**kwargs)  # noqa: E501
+        return self.pipeline_service_list_pipeline_versions_with_http_info(**kwargs)  # noqa: E501
 
-    def list_pipeline_versions_with_http_info(self, **kwargs):  # noqa: E501
+    def pipeline_service_list_pipeline_versions_with_http_info(self, **kwargs):  # noqa: E501
         """Lists all pipeline versions of a given pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_pipeline_versions_with_http_info(async_req=True)
+        >>> thread = api.pipeline_service_list_pipeline_versions_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param resource_key_type: The type of the resource that referred to.
         :type resource_key_type: str
         :param resource_key_id: The ID of the resource that referred to.
         :type resource_key_id: str
         :param page_size: The number of pipeline versions to be listed per page. If there are more pipeline versions than this number, the response message will contain a nextPageToken field you can use to fetch the next page.
@@ -1117,34 +1117,34 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_pipeline_versions" % key
+                    " to method pipeline_service_list_pipeline_versions" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'resource_key_type' in local_var_params and local_var_params['resource_key_type'] is not None:  # noqa: E501
-            query_params.append(('resource_key.type', local_var_params['resource_key_type']))  # noqa: E501
+            query_params.append(('resourceKey.type', local_var_params['resource_key_type']))  # noqa: E501
         if 'resource_key_id' in local_var_params and local_var_params['resource_key_id'] is not None:  # noqa: E501
-            query_params.append(('resource_key.id', local_var_params['resource_key_id']))  # noqa: E501
+            query_params.append(('resourceKey.id', local_var_params['resource_key_id']))  # noqa: E501
         if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
-            query_params.append(('page_size', local_var_params['page_size']))  # noqa: E501
+            query_params.append(('pageSize', local_var_params['page_size']))  # noqa: E501
         if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
-            query_params.append(('page_token', local_var_params['page_token']))  # noqa: E501
+            query_params.append(('pageToken', local_var_params['page_token']))  # noqa: E501
         if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
-            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            query_params.append(('sortBy', local_var_params['sort_by']))  # noqa: E501
         if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
             query_params.append(('filter', local_var_params['filter']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -1169,21 +1169,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_pipelines(self, **kwargs):  # noqa: E501
+    def pipeline_service_list_pipelines(self, **kwargs):  # noqa: E501
         """Finds all pipelines.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_pipelines(async_req=True)
+        >>> thread = api.pipeline_service_list_pipelines(async_req=True)
         >>> result = thread.get()
 
         :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListPipelines call.
         :type page_token: str
         :param page_size: The number of pipelines to be listed per page. If there are more pipelines than this number, the response message will contain a valid value in the nextPageToken field.
         :type page_size: int
         :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" Ascending by default.
@@ -1205,23 +1205,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1ListPipelinesResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_pipelines_with_http_info(**kwargs)  # noqa: E501
+        return self.pipeline_service_list_pipelines_with_http_info(**kwargs)  # noqa: E501
 
-    def list_pipelines_with_http_info(self, **kwargs):  # noqa: E501
+    def pipeline_service_list_pipelines_with_http_info(self, **kwargs):  # noqa: E501
         """Finds all pipelines.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_pipelines_with_http_info(async_req=True)
+        >>> thread = api.pipeline_service_list_pipelines_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param page_token: A page token to request the next page of results. The token is acquried from the nextPageToken field of the response from the previous ListPipelines call.
         :type page_token: str
         :param page_size: The number of pipelines to be listed per page. If there are more pipelines than this number, the response message will contain a valid value in the nextPageToken field.
         :type page_size: int
         :param sort_by: Can be format of \"field_name\", \"field_name asc\" or \"field_name desc\" Ascending by default.
@@ -1270,36 +1270,36 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_pipelines" % key
+                    " to method pipeline_service_list_pipelines" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'page_token' in local_var_params and local_var_params['page_token'] is not None:  # noqa: E501
-            query_params.append(('page_token', local_var_params['page_token']))  # noqa: E501
+            query_params.append(('pageToken', local_var_params['page_token']))  # noqa: E501
         if 'page_size' in local_var_params and local_var_params['page_size'] is not None:  # noqa: E501
-            query_params.append(('page_size', local_var_params['page_size']))  # noqa: E501
+            query_params.append(('pageSize', local_var_params['page_size']))  # noqa: E501
         if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
-            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            query_params.append(('sortBy', local_var_params['sort_by']))  # noqa: E501
         if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
             query_params.append(('filter', local_var_params['filter']))  # noqa: E501
         if 'resource_reference_key_type' in local_var_params and local_var_params['resource_reference_key_type'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.type', local_var_params['resource_reference_key_type']))  # noqa: E501
+            query_params.append(('resourceReferenceKey.type', local_var_params['resource_reference_key_type']))  # noqa: E501
         if 'resource_reference_key_id' in local_var_params and local_var_params['resource_reference_key_id'] is not None:  # noqa: E501
-            query_params.append(('resource_reference_key.id', local_var_params['resource_reference_key_id']))  # noqa: E501
+            query_params.append(('resourceReferenceKey.id', local_var_params['resource_reference_key_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1322,21 +1322,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_pipeline_default_version(self, pipeline_id, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_update_pipeline_default_version(self, pipeline_id, version_id, **kwargs):  # noqa: E501
         """Update the default pipeline version of a specific pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_pipeline_default_version(pipeline_id, version_id, async_req=True)
+        >>> thread = api.pipeline_service_update_pipeline_default_version(pipeline_id, version_id, async_req=True)
         >>> result = thread.get()
 
         :param pipeline_id: The ID of the pipeline to be updated. (required)
         :type pipeline_id: str
         :param version_id: The ID of the default version. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
@@ -1350,23 +1350,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_pipeline_default_version_with_http_info(pipeline_id, version_id, **kwargs)  # noqa: E501
+        return self.pipeline_service_update_pipeline_default_version_with_http_info(pipeline_id, version_id, **kwargs)  # noqa: E501
 
-    def update_pipeline_default_version_with_http_info(self, pipeline_id, version_id, **kwargs):  # noqa: E501
+    def pipeline_service_update_pipeline_default_version_with_http_info(self, pipeline_id, version_id, **kwargs):  # noqa: E501
         """Update the default pipeline version of a specific pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_pipeline_default_version_with_http_info(pipeline_id, version_id, async_req=True)
+        >>> thread = api.pipeline_service_update_pipeline_default_version_with_http_info(pipeline_id, version_id, async_req=True)
         >>> result = thread.get()
 
         :param pipeline_id: The ID of the pipeline to be updated. (required)
         :type pipeline_id: str
         :param version_id: The ID of the default version. (required)
         :type version_id: str
         :param async_req: Whether to execute the request asynchronously.
@@ -1403,34 +1403,34 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_pipeline_default_version" % key
+                    " to method pipeline_service_update_pipeline_default_version" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'pipeline_id' is set
         if self.api_client.client_side_validation and ('pipeline_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['pipeline_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `pipeline_id` when calling `update_pipeline_default_version`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `pipeline_id` when calling `pipeline_service_update_pipeline_default_version`")  # noqa: E501
         # verify the required parameter 'version_id' is set
         if self.api_client.client_side_validation and ('version_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['version_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `version_id` when calling `update_pipeline_default_version`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `version_id` when calling `pipeline_service_update_pipeline_default_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'pipeline_id' in local_var_params:
-            path_params['pipeline_id'] = local_var_params['pipeline_id']  # noqa: E501
+            path_params['pipelineId'] = local_var_params['pipeline_id']  # noqa: E501
         if 'version_id' in local_var_params:
-            path_params['version_id'] = local_var_params['version_id']  # noqa: E501
+            path_params['versionId'] = local_var_params['version_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -1440,15 +1440,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['Bearer']  # noqa: E501
 
         return self.api_client.call_api(
-            '/apis/v1/pipelines/{pipeline_id}/default_version/{version_id}', 'POST',
+            '/apis/v1/pipelines/{pipelineId}/default_version/{versionId}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='object',  # noqa: E501
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api/pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_upload_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/api_client.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/configuration.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.5.0\n"\
-               "SDK Package Version: 1.5.0".\
+               "Version of the API: 1.7.0\n"\
+               "SDK Package Version: 1.8.0rc1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/exceptions.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/__init__.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
+from kfp_tekton_server_api.models.googlerpc_status import GooglerpcStatus
+from kfp_tekton_server_api.models.inline_object import InlineObject
 from kfp_tekton_server_api.models.job_mode import JobMode
 from kfp_tekton_server_api.models.pipeline_spec_runtime_config import PipelineSpecRuntimeConfig
 from kfp_tekton_server_api.models.protobuf_any import ProtobufAny
 from kfp_tekton_server_api.models.report_run_metrics_response_report_run_metric_result import ReportRunMetricsResponseReportRunMetricResult
 from kfp_tekton_server_api.models.report_run_metrics_response_report_run_metric_result_status import ReportRunMetricsResponseReportRunMetricResultStatus
 from kfp_tekton_server_api.models.run_metric_format import RunMetricFormat
 from kfp_tekton_server_api.models.v1_cron_schedule import V1CronSchedule
@@ -35,15 +37,14 @@
 from kfp_tekton_server_api.models.v1_periodic_schedule import V1PeriodicSchedule
 from kfp_tekton_server_api.models.v1_pipeline import V1Pipeline
 from kfp_tekton_server_api.models.v1_pipeline_runtime import V1PipelineRuntime
 from kfp_tekton_server_api.models.v1_pipeline_spec import V1PipelineSpec
 from kfp_tekton_server_api.models.v1_pipeline_version import V1PipelineVersion
 from kfp_tekton_server_api.models.v1_read_artifact_response import V1ReadArtifactResponse
 from kfp_tekton_server_api.models.v1_relationship import V1Relationship
-from kfp_tekton_server_api.models.v1_report_run_metrics_request import V1ReportRunMetricsRequest
 from kfp_tekton_server_api.models.v1_report_run_metrics_response import V1ReportRunMetricsResponse
 from kfp_tekton_server_api.models.v1_resource_key import V1ResourceKey
 from kfp_tekton_server_api.models.v1_resource_reference import V1ResourceReference
 from kfp_tekton_server_api.models.v1_resource_type import V1ResourceType
 from kfp_tekton_server_api.models.v1_run import V1Run
 from kfp_tekton_server_api.models.v1_run_detail import V1RunDetail
 from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/job_mode.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/job_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,15 +35,15 @@
     openapi_types = {
         'parameters': 'dict(str, V1Value)',
         'pipeline_root': 'str'
     }
 
     attribute_map = {
         'parameters': 'parameters',
-        'pipeline_root': 'pipeline_root'
+        'pipeline_root': 'pipelineRoot'
     }
 
     def __init__(self, parameters=None, pipeline_root=None, local_vars_configuration=None):  # noqa: E501
         """PipelineSpecRuntimeConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/protobuf_any.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,54 +29,82 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'type': 'str',
         'type_url': 'str',
         'value': 'str'
     }
 
     attribute_map = {
+        'type': '@type',
         'type_url': 'type_url',
         'value': 'value'
     }
 
-    def __init__(self, type_url=None, value=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, type_url=None, value=None, local_vars_configuration=None):  # noqa: E501
         """ProtobufAny - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._type_url = None
         self._value = None
         self.discriminator = None
 
+        if type is not None:
+            self.type = type
         if type_url is not None:
             self.type_url = type_url
         if value is not None:
             self.value = value
 
     @property
+    def type(self):
+        """Gets the type of this ProtobufAny.  # noqa: E501
+
+        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. This string must contain at least one \"/\" character. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
+
+        :return: The type of this ProtobufAny.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ProtobufAny.
+
+        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. This string must contain at least one \"/\" character. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
+
+        :param type: The type of this ProtobufAny.  # noqa: E501
+        :type type: str
+        """
+
+        self._type = type
+
+    @property
     def type_url(self):
         """Gets the type_url of this ProtobufAny.  # noqa: E501
 
-        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. This string must contain at least one \"/\" character. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
+        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
 
         :return: The type_url of this ProtobufAny.  # noqa: E501
         :rtype: str
         """
         return self._type_url
 
     @type_url.setter
     def type_url(self, type_url):
         """Sets the type_url of this ProtobufAny.
 
-        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. This string must contain at least one \"/\" character. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
+        A URL/resource name that uniquely identifies the type of the serialized protocol buffer message. The last segment of the URL's path must represent the fully qualified name of the type (as in `path/google.protobuf.Duration`). The name should be in a canonical form (e.g., leading \".\" is not accepted).  In practice, teams usually precompile into the binary all types that they expect it to use in the context of Any. However, for URLs which use the scheme `http`, `https`, or no scheme, one can optionally set up a type server that maps type URLs to message definitions as follows:  * If no scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield a [google.protobuf.Type][]   value in binary format, or produce an error. * Applications are allowed to cache lookup results based on the   URL, or have them precompiled into a binary to avoid any   lookup. Therefore, binary compatibility needs to be preserved   on changes to types. (Use versioned type names to manage   breaking changes.)  Note: this functionality is not currently available in the official protobuf release, and it is not used for type URLs beginning with type.googleapis.com.  Schemes other than `http`, `https` (or the empty scheme) might be used with implementation specific semantics.  # noqa: E501
 
         :param type_url: The type_url of this ProtobufAny.  # noqa: E501
         :type type_url: str
         """
 
         self._type_url = type_url
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'metric_name': 'str',
         'metric_node_id': 'str',
         'status': 'ReportRunMetricsResponseReportRunMetricResultStatus',
         'message': 'str'
     }
 
     attribute_map = {
-        'metric_name': 'metric_name',
-        'metric_node_id': 'metric_node_id',
+        'metric_name': 'metricName',
+        'metric_node_id': 'metricNodeId',
         'status': 'status',
         'message': 'message'
     }
 
     def __init__(self, metric_name=None, metric_node_id=None, status=None, message=None, local_vars_configuration=None):  # noqa: E501
         """ReportRunMetricsResponseReportRunMetricResult - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/run_metric_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_cron_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,16 +35,16 @@
     openapi_types = {
         'start_time': 'datetime',
         'end_time': 'datetime',
         'cron': 'str'
     }
 
     attribute_map = {
-        'start_time': 'start_time',
-        'end_time': 'end_time',
+        'start_time': 'startTime',
+        'end_time': 'endTime',
         'cron': 'cron'
     }
 
     def __init__(self, start_time=None, end_time=None, cron=None, local_vars_configuration=None):  # noqa: E501
         """V1CronSchedule - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -41,17 +41,17 @@
         'storage_state': 'V1ExperimentStorageState'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'description': 'description',
-        'created_at': 'created_at',
-        'resource_references': 'resource_references',
-        'storage_state': 'storage_state'
+        'created_at': 'createdAt',
+        'resource_references': 'resourceReferences',
+        'storage_state': 'storageState'
     }
 
     def __init__(self, id=None, name=None, description=None, created_at=None, resource_references=None, storage_state=None, local_vars_configuration=None):  # noqa: E501
         """V1Experiment - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_relationship.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kfp_tekton_server_api.configuration import Configuration
 
 
-class V1ExperimentStorageState(object):
+class V1Relationship(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "STORAGESTATE_UNSPECIFIED"
-    AVAILABLE = "STORAGESTATE_AVAILABLE"
-    ARCHIVED = "STORAGESTATE_ARCHIVED"
+    UNKNOWN_RELATIONSHIP = "UNKNOWN_RELATIONSHIP"
+    OWNER = "OWNER"
+    CREATOR = "CREATOR"
 
-    allowable_values = [UNSPECIFIED, AVAILABLE, ARCHIVED]  # noqa: E501
+    allowable_values = [UNKNOWN_RELATIONSHIP, OWNER, CREATOR]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V1ExperimentStorageState - a model defined in OpenAPI"""  # noqa: E501
+        """V1Relationship - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1ExperimentStorageState):
+        if not isinstance(other, V1Relationship):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1ExperimentStorageState):
+        if not isinstance(other, V1Relationship):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_healthz_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'multi_user': 'bool'
     }
 
     attribute_map = {
-        'multi_user': 'multi_user'
+        'multi_user': 'multiUser'
     }
 
     def __init__(self, multi_user=None, local_vars_configuration=None):  # noqa: E501
         """V1GetHealthzResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_template_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_job.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -50,26 +50,26 @@
         'no_catchup': 'bool'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'description': 'description',
-        'pipeline_spec': 'pipeline_spec',
-        'resource_references': 'resource_references',
-        'service_account': 'service_account',
-        'max_concurrency': 'max_concurrency',
+        'pipeline_spec': 'pipelineSpec',
+        'resource_references': 'resourceReferences',
+        'service_account': 'serviceAccount',
+        'max_concurrency': 'maxConcurrency',
         'trigger': 'trigger',
         'mode': 'mode',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
         'status': 'status',
         'error': 'error',
         'enabled': 'enabled',
-        'no_catchup': 'no_catchup'
+        'no_catchup': 'noCatchup'
     }
 
     def __init__(self, id=None, name=None, description=None, pipeline_spec=None, resource_references=None, service_account=None, max_concurrency=None, trigger=None, mode=None, created_at=None, updated_at=None, status=None, error=None, enabled=None, no_catchup=None, local_vars_configuration=None):  # noqa: E501
         """V1Job - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_experiments_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'experiments': 'list[V1Experiment]',
         'total_size': 'int',
         'next_page_token': 'str'
     }
 
     attribute_map = {
         'experiments': 'experiments',
-        'total_size': 'total_size',
-        'next_page_token': 'next_page_token'
+        'total_size': 'totalSize',
+        'next_page_token': 'nextPageToken'
     }
 
     def __init__(self, experiments=None, total_size=None, next_page_token=None, local_vars_configuration=None):  # noqa: E501
         """V1ListExperimentsResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_jobs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'jobs': 'list[V1Job]',
         'total_size': 'int',
         'next_page_token': 'str'
     }
 
     attribute_map = {
         'jobs': 'jobs',
-        'total_size': 'total_size',
-        'next_page_token': 'next_page_token'
+        'total_size': 'totalSize',
+        'next_page_token': 'nextPageToken'
     }
 
     def __init__(self, jobs=None, total_size=None, next_page_token=None, local_vars_configuration=None):  # noqa: E501
         """V1ListJobsResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'versions': 'list[V1PipelineVersion]',
         'next_page_token': 'str',
         'total_size': 'int'
     }
 
     attribute_map = {
         'versions': 'versions',
-        'next_page_token': 'next_page_token',
-        'total_size': 'total_size'
+        'next_page_token': 'nextPageToken',
+        'total_size': 'totalSize'
     }
 
     def __init__(self, versions=None, next_page_token=None, total_size=None, local_vars_configuration=None):  # noqa: E501
         """V1ListPipelineVersionsResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipelines_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'pipelines': 'list[V1Pipeline]',
         'total_size': 'int',
         'next_page_token': 'str'
     }
 
     attribute_map = {
         'pipelines': 'pipelines',
-        'total_size': 'total_size',
-        'next_page_token': 'next_page_token'
+        'total_size': 'totalSize',
+        'next_page_token': 'nextPageToken'
     }
 
     def __init__(self, pipelines=None, total_size=None, next_page_token=None, local_vars_configuration=None):  # noqa: E501
         """V1ListPipelinesResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_runs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,16 +36,16 @@
         'runs': 'list[V1Run]',
         'total_size': 'int',
         'next_page_token': 'str'
     }
 
     attribute_map = {
         'runs': 'runs',
-        'total_size': 'total_size',
-        'next_page_token': 'next_page_token'
+        'total_size': 'totalSize',
+        'next_page_token': 'nextPageToken'
     }
 
     def __init__(self, runs=None, total_size=None, next_page_token=None, local_vars_configuration=None):  # noqa: E501
         """V1ListRunsResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_periodic_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,17 +35,17 @@
     openapi_types = {
         'start_time': 'datetime',
         'end_time': 'datetime',
         'interval_second': 'str'
     }
 
     attribute_map = {
-        'start_time': 'start_time',
-        'end_time': 'end_time',
-        'interval_second': 'interval_second'
+        'start_time': 'startTime',
+        'end_time': 'endTime',
+        'interval_second': 'intervalSecond'
     }
 
     def __init__(self, start_time=None, end_time=None, interval_second=None, local_vars_configuration=None):  # noqa: E501
         """V1PeriodicSchedule - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -37,44 +37,47 @@
         'created_at': 'datetime',
         'name': 'str',
         'description': 'str',
         'parameters': 'list[V1Parameter]',
         'url': 'V1Url',
         'error': 'str',
         'default_version': 'V1PipelineVersion',
-        'resource_references': 'list[V1ResourceReference]'
+        'resource_references': 'list[V1ResourceReference]',
+        'created_at': 'datetime'
     }
 
     attribute_map = {
         'id': 'id',
-        'created_at': 'created_at',
+        'created_at': 'createdAt',
         'name': 'name',
         'description': 'description',
         'parameters': 'parameters',
         'url': 'url',
         'error': 'error',
-        'default_version': 'default_version',
-        'resource_references': 'resource_references'
+        'default_version': 'defaultVersion',
+        'resource_references': 'resourceReferences',
+        'created_at': 'created_at'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, created_at=None, local_vars_configuration=None):  # noqa: E501
         """V1Pipeline - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._parameters = None
         self._url = None
         self._error = None
         self._default_version = None
         self._resource_references = None
+        self._created_at = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if name is not None:
@@ -87,14 +90,16 @@
             self.url = url
         if error is not None:
             self.error = error
         if default_version is not None:
             self.default_version = default_version
         if resource_references is not None:
             self.resource_references = resource_references
+        if created_at is not None:
+            self.created_at = created_at
 
     @property
     def id(self):
         """Gets the id of this V1Pipeline.  # noqa: E501
 
         Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
@@ -291,14 +296,35 @@
 
         :param resource_references: The resource_references of this V1Pipeline.  # noqa: E501
         :type resource_references: list[V1ResourceReference]
         """
 
         self._resource_references = resource_references
 
+    @property
+    def created_at(self):
+        """Gets the created_at of this V1Pipeline.  # noqa: E501
+
+
+        :return: The created_at of this V1Pipeline.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._created_at
+
+    @created_at.setter
+    def created_at(self, created_at):
+        """Sets the created_at of this V1Pipeline.
+
+
+        :param created_at: The created_at of this V1Pipeline.  # noqa: E501
+        :type created_at: datetime
+        """
+
+        self._created_at = created_at
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -34,16 +34,16 @@
     """
     openapi_types = {
         'pipeline_manifest': 'str',
         'workflow_manifest': 'str'
     }
 
     attribute_map = {
-        'pipeline_manifest': 'pipeline_manifest',
-        'workflow_manifest': 'workflow_manifest'
+        'pipeline_manifest': 'pipelineManifest',
+        'workflow_manifest': 'workflowManifest'
     }
 
     def __init__(self, pipeline_manifest=None, workflow_manifest=None, local_vars_configuration=None):  # noqa: E501
         """V1PipelineRuntime - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -38,20 +38,20 @@
         'workflow_manifest': 'str',
         'pipeline_manifest': 'str',
         'parameters': 'list[V1Parameter]',
         'runtime_config': 'PipelineSpecRuntimeConfig'
     }
 
     attribute_map = {
-        'pipeline_id': 'pipeline_id',
-        'pipeline_name': 'pipeline_name',
-        'workflow_manifest': 'workflow_manifest',
-        'pipeline_manifest': 'pipeline_manifest',
+        'pipeline_id': 'pipelineId',
+        'pipeline_name': 'pipelineName',
+        'workflow_manifest': 'workflowManifest',
+        'pipeline_manifest': 'pipelineManifest',
         'parameters': 'parameters',
-        'runtime_config': 'runtime_config'
+        'runtime_config': 'runtimeConfig'
     }
 
     def __init__(self, pipeline_id=None, pipeline_name=None, workflow_manifest=None, pipeline_manifest=None, parameters=None, runtime_config=None, local_vars_configuration=None):  # noqa: E501
         """V1PipelineSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_read_artifact_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment_storage_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kfp_tekton_server_api.configuration import Configuration
 
 
-class V1Relationship(object):
+class V1ExperimentStorageState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN_RELATIONSHIP = "UNKNOWN_RELATIONSHIP"
-    OWNER = "OWNER"
-    CREATOR = "CREATOR"
+    UNSPECIFIED = "STORAGESTATE_UNSPECIFIED"
+    AVAILABLE = "STORAGESTATE_AVAILABLE"
+    ARCHIVED = "STORAGESTATE_ARCHIVED"
 
-    allowable_values = [UNKNOWN_RELATIONSHIP, OWNER, CREATOR]  # noqa: E501
+    allowable_values = [UNSPECIFIED, AVAILABLE, ARCHIVED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """V1Relationship - a model defined in OpenAPI"""  # noqa: E501
+        """V1ExperimentStorageState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1Relationship):
+        if not isinstance(other, V1ExperimentStorageState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1Relationship):
+        if not isinstance(other, V1ExperimentStorageState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_report_run_metrics_request.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/inline_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,79 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kfp_tekton_server_api.configuration import Configuration
 
 
-class V1ReportRunMetricsRequest(object):
+class InlineObject(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'run_id': 'str',
         'metrics': 'list[V1RunMetric]'
     }
 
     attribute_map = {
-        'run_id': 'run_id',
         'metrics': 'metrics'
     }
 
-    def __init__(self, run_id=None, metrics=None, local_vars_configuration=None):  # noqa: E501
-        """V1ReportRunMetricsRequest - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, metrics=None, local_vars_configuration=None):  # noqa: E501
+        """InlineObject - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._run_id = None
         self._metrics = None
         self.discriminator = None
 
-        if run_id is not None:
-            self.run_id = run_id
         if metrics is not None:
             self.metrics = metrics
 
     @property
-    def run_id(self):
-        """Gets the run_id of this V1ReportRunMetricsRequest.  # noqa: E501
-
-        Required. The parent run ID of the metric.  # noqa: E501
-
-        :return: The run_id of this V1ReportRunMetricsRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._run_id
-
-    @run_id.setter
-    def run_id(self, run_id):
-        """Sets the run_id of this V1ReportRunMetricsRequest.
-
-        Required. The parent run ID of the metric.  # noqa: E501
-
-        :param run_id: The run_id of this V1ReportRunMetricsRequest.  # noqa: E501
-        :type run_id: str
-        """
-
-        self._run_id = run_id
-
-    @property
     def metrics(self):
-        """Gets the metrics of this V1ReportRunMetricsRequest.  # noqa: E501
+        """Gets the metrics of this InlineObject.  # noqa: E501
 
         List of metrics to report.  # noqa: E501
 
-        :return: The metrics of this V1ReportRunMetricsRequest.  # noqa: E501
+        :return: The metrics of this InlineObject.  # noqa: E501
         :rtype: list[V1RunMetric]
         """
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics):
-        """Sets the metrics of this V1ReportRunMetricsRequest.
+        """Sets the metrics of this InlineObject.
 
         List of metrics to report.  # noqa: E501
 
-        :param metrics: The metrics of this V1ReportRunMetricsRequest.  # noqa: E501
+        :param metrics: The metrics of this InlineObject.  # noqa: E501
         :type metrics: list[V1RunMetric]
         """
 
         self._metrics = metrics
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -133,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1ReportRunMetricsRequest):
+        if not isinstance(other, InlineObject):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1ReportRunMetricsRequest):
+        if not isinstance(other, InlineObject):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_report_run_metrics_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -47,22 +47,22 @@
         'error': 'str',
         'metrics': 'list[V1RunMetric]'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        'storage_state': 'storage_state',
+        'storage_state': 'storageState',
         'description': 'description',
-        'pipeline_spec': 'pipeline_spec',
-        'resource_references': 'resource_references',
-        'service_account': 'service_account',
-        'created_at': 'created_at',
-        'scheduled_at': 'scheduled_at',
-        'finished_at': 'finished_at',
+        'pipeline_spec': 'pipelineSpec',
+        'resource_references': 'resourceReferences',
+        'service_account': 'serviceAccount',
+        'created_at': 'createdAt',
+        'scheduled_at': 'scheduledAt',
+        'finished_at': 'finishedAt',
         'status': 'status',
         'error': 'error',
         'metrics': 'metrics'
     }
 
     def __init__(self, id=None, name=None, storage_state=None, description=None, pipeline_spec=None, resource_references=None, service_account=None, created_at=None, scheduled_at=None, finished_at=None, status=None, error=None, metrics=None, local_vars_configuration=None):  # noqa: E501
         """V1Run - a model defined in OpenAPI"""  # noqa: E501
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,15 +35,15 @@
     openapi_types = {
         'run': 'V1Run',
         'pipeline_runtime': 'V1PipelineRuntime'
     }
 
     attribute_map = {
         'run': 'run',
-        'pipeline_runtime': 'pipeline_runtime'
+        'pipeline_runtime': 'pipelineRuntime'
     }
 
     def __init__(self, run=None, pipeline_runtime=None, local_vars_configuration=None):  # noqa: E501
         """V1RunDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -37,16 +37,16 @@
         'node_id': 'str',
         'number_value': 'float',
         'format': 'RunMetricFormat'
     }
 
     attribute_map = {
         'name': 'name',
-        'node_id': 'node_id',
-        'number_value': 'number_value',
+        'node_id': 'nodeId',
+        'number_value': 'numberValue',
         'format': 'format'
     }
 
     def __init__(self, name=None, node_id=None, number_value=None, format=None, local_vars_configuration=None):  # noqa: E501
         """V1RunMetric - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_storage_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_status.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -34,16 +34,16 @@
     """
     openapi_types = {
         'cron_schedule': 'V1CronSchedule',
         'periodic_schedule': 'V1PeriodicSchedule'
     }
 
     attribute_map = {
-        'cron_schedule': 'cron_schedule',
-        'periodic_schedule': 'periodic_schedule'
+        'cron_schedule': 'cronSchedule',
+        'periodic_schedule': 'periodicSchedule'
     }
 
     def __init__(self, cron_schedule=None, periodic_schedule=None, local_vars_configuration=None):  # noqa: E501
         """V1Trigger - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_url.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,32 +29,37 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'pipeline_url': 'str',
         'pipeline_url': 'str'
     }
 
     attribute_map = {
+        'pipeline_url': 'pipelineUrl',
         'pipeline_url': 'pipeline_url'
     }
 
-    def __init__(self, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pipeline_url=None, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
         """V1Url - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pipeline_url = None
+        self._pipeline_url = None
         self.discriminator = None
 
         if pipeline_url is not None:
             self.pipeline_url = pipeline_url
+        if pipeline_url is not None:
+            self.pipeline_url = pipeline_url
 
     @property
     def pipeline_url(self):
         """Gets the pipeline_url of this V1Url.  # noqa: E501
 
         URL of the pipeline definition or the pipeline version definition.  # noqa: E501
 
@@ -71,14 +76,35 @@
 
         :param pipeline_url: The pipeline_url of this V1Url.  # noqa: E501
         :type pipeline_url: str
         """
 
         self._pipeline_url = pipeline_url
 
+    @property
+    def pipeline_url(self):
+        """Gets the pipeline_url of this V1Url.  # noqa: E501
+
+
+        :return: The pipeline_url of this V1Url.  # noqa: E501
+        :rtype: str
+        """
+        return self._pipeline_url
+
+    @pipeline_url.setter
+    def pipeline_url(self, pipeline_url):
+        """Sets the pipeline_url of this V1Url.
+
+
+        :param pipeline_url: The pipeline_url of this V1Url.  # noqa: E501
+        :type pipeline_url: str
+        """
+
+        self._pipeline_url = pipeline_url
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/models/v1_value.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,17 +35,17 @@
     openapi_types = {
         'int_value': 'str',
         'double_value': 'float',
         'string_value': 'str'
     }
 
     attribute_map = {
-        'int_value': 'int_value',
-        'double_value': 'double_value',
-        'string_value': 'string_value'
+        'int_value': 'intValue',
+        'double_value': 'doubleValue',
+        'string_value': 'stringValue'
     }
 
     def __init__(self, int_value=None, double_value=None, string_value=None, local_vars_configuration=None):  # noqa: E501
         """V1Value - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api/rest.py` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `kfp-tekton-server-api-1.5.0/kfp_tekton_server_api.egg-info/SOURCES.txt` & `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 kfp_tekton_server_api/api/experiment_service_api.py
 kfp_tekton_server_api/api/healthz_service_api.py
 kfp_tekton_server_api/api/job_service_api.py
 kfp_tekton_server_api/api/pipeline_service_api.py
 kfp_tekton_server_api/api/pipeline_upload_service_api.py
 kfp_tekton_server_api/api/run_service_api.py
 kfp_tekton_server_api/models/__init__.py
+kfp_tekton_server_api/models/googlerpc_status.py
+kfp_tekton_server_api/models/inline_object.py
 kfp_tekton_server_api/models/job_mode.py
 kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
 kfp_tekton_server_api/models/protobuf_any.py
 kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
 kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
 kfp_tekton_server_api/models/run_metric_format.py
 kfp_tekton_server_api/models/v1_cron_schedule.py
@@ -41,29 +43,30 @@
 kfp_tekton_server_api/models/v1_periodic_schedule.py
 kfp_tekton_server_api/models/v1_pipeline.py
 kfp_tekton_server_api/models/v1_pipeline_runtime.py
 kfp_tekton_server_api/models/v1_pipeline_spec.py
 kfp_tekton_server_api/models/v1_pipeline_version.py
 kfp_tekton_server_api/models/v1_read_artifact_response.py
 kfp_tekton_server_api/models/v1_relationship.py
-kfp_tekton_server_api/models/v1_report_run_metrics_request.py
 kfp_tekton_server_api/models/v1_report_run_metrics_response.py
 kfp_tekton_server_api/models/v1_resource_key.py
 kfp_tekton_server_api/models/v1_resource_reference.py
 kfp_tekton_server_api/models/v1_resource_type.py
 kfp_tekton_server_api/models/v1_run.py
 kfp_tekton_server_api/models/v1_run_detail.py
 kfp_tekton_server_api/models/v1_run_metric.py
 kfp_tekton_server_api/models/v1_run_storage_state.py
 kfp_tekton_server_api/models/v1_status.py
 kfp_tekton_server_api/models/v1_trigger.py
 kfp_tekton_server_api/models/v1_url.py
 kfp_tekton_server_api/models/v1_value.py
 test/test_experiment_service_api.py
+test/test_googlerpc_status.py
 test/test_healthz_service_api.py
+test/test_inline_object.py
 test/test_job_mode.py
 test/test_job_service_api.py
 test/test_pipeline_service_api.py
 test/test_pipeline_spec_runtime_config.py
 test/test_pipeline_upload_service_api.py
 test/test_protobuf_any.py
 test/test_report_run_metrics_response_report_run_metric_result.py
@@ -85,15 +88,14 @@
 test/test_v1_periodic_schedule.py
 test/test_v1_pipeline.py
 test/test_v1_pipeline_runtime.py
 test/test_v1_pipeline_spec.py
 test/test_v1_pipeline_version.py
 test/test_v1_read_artifact_response.py
 test/test_v1_relationship.py
-test/test_v1_report_run_metrics_request.py
 test/test_v1_report_run_metrics_response.py
 test/test_v1_resource_key.py
 test/test_v1_resource_reference.py
 test/test_v1_resource_type.py
 test/test_v1_run.py
 test/test_v1_run_detail.py
 test/test_v1_run_metric.py
```

### Comparing `kfp-tekton-server-api-1.5.0/setup.py` & `kfp-tekton-server-api-1.8.0rc1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-tekton-server-api"
-VERSION = "1.5.0"
+VERSION = "1.8.0rc1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Kubeflow Pipelines on Tekton API",
-    author="kfp-tekton",
-    author_email="prashsh1@in.ibm.com",
+    description="Kubeflow Pipelines API",
+    author="google",
+    author_email="kubeflow-pipelines@google.com",
     url="https://github.com/kubeflow/kfp-tekton",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Kubeflow Pipelines on Tekton API"],
+    keywords=["OpenAPI", "OpenAPI-Generator", "Kubeflow Pipelines API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
     long_description="""\
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.  # noqa: E501
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.  # noqa: E501
     """
 )
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_experiment_service_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -24,51 +24,51 @@
 
     def setUp(self):
         self.api = kfp_tekton_server_api.api.experiment_service_api.ExperimentServiceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_archive_experiment(self):
-        """Test case for archive_experiment
+    def test_experiment_service_archive_experiment(self):
+        """Test case for experiment_service_archive_experiment
 
         Archives an experiment and the experiment's runs and jobs.  # noqa: E501
         """
         pass
 
-    def test_create_experiment(self):
-        """Test case for create_experiment
+    def test_experiment_service_create_experiment(self):
+        """Test case for experiment_service_create_experiment
 
         Creates a new experiment.  # noqa: E501
         """
         pass
 
-    def test_delete_experiment(self):
-        """Test case for delete_experiment
+    def test_experiment_service_delete_experiment(self):
+        """Test case for experiment_service_delete_experiment
 
         Deletes an experiment without deleting the experiment's runs and jobs. To avoid unexpected behaviors, delete an experiment's runs and jobs before deleting the experiment.  # noqa: E501
         """
         pass
 
-    def test_get_experiment(self):
-        """Test case for get_experiment
+    def test_experiment_service_get_experiment(self):
+        """Test case for experiment_service_get_experiment
 
         Finds a specific experiment by ID.  # noqa: E501
         """
         pass
 
-    def test_list_experiment(self):
-        """Test case for list_experiment
+    def test_experiment_service_list_experiment(self):
+        """Test case for experiment_service_list_experiment
 
         Finds all experiments. Supports pagination, and sorting on certain fields.  # noqa: E501
         """
         pass
 
-    def test_unarchive_experiment(self):
-        """Test case for unarchive_experiment
+    def test_experiment_service_unarchive_experiment(self):
+        """Test case for experiment_service_unarchive_experiment
 
         Restores an archived experiment. The experiment's archived runs and jobs will stay archived.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_healthz_service_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -24,16 +24,16 @@
 
     def setUp(self):
         self.api = kfp_tekton_server_api.api.healthz_service_api.HealthzServiceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_healthz(self):
-        """Test case for get_healthz
+    def test_healthz_service_get_healthz(self):
+        """Test case for healthz_service_get_healthz
 
         Get healthz data.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_job_mode.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_job_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_service_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -24,86 +24,86 @@
 
     def setUp(self):
         self.api = kfp_tekton_server_api.api.pipeline_service_api.PipelineServiceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_create_pipeline(self):
-        """Test case for create_pipeline
+    def test_pipeline_service_create_pipeline(self):
+        """Test case for pipeline_service_create_pipeline
 
         Creates a pipeline.  # noqa: E501
         """
         pass
 
-    def test_create_pipeline_version(self):
-        """Test case for create_pipeline_version
+    def test_pipeline_service_create_pipeline_version(self):
+        """Test case for pipeline_service_create_pipeline_version
 
         Adds a pipeline version to the specified pipeline.  # noqa: E501
         """
         pass
 
-    def test_delete_pipeline(self):
-        """Test case for delete_pipeline
+    def test_pipeline_service_delete_pipeline(self):
+        """Test case for pipeline_service_delete_pipeline
 
         Deletes a pipeline and its pipeline versions.  # noqa: E501
         """
         pass
 
-    def test_delete_pipeline_version(self):
-        """Test case for delete_pipeline_version
+    def test_pipeline_service_delete_pipeline_version(self):
+        """Test case for pipeline_service_delete_pipeline_version
 
         Deletes a pipeline version by pipeline version ID. If the deleted pipeline version is the default pipeline version, the pipeline's default version changes to the pipeline's most recent pipeline version. If there are no remaining pipeline versions, the pipeline will have no default version. Examines the run_service_api.ipynb notebook to learn more about creating a run using a pipeline version (https://github.com/kubeflow/pipelines/blob/master/tools/benchmarks/run_service_api.ipynb).  # noqa: E501
         """
         pass
 
-    def test_get_pipeline(self):
-        """Test case for get_pipeline
+    def test_pipeline_service_get_pipeline(self):
+        """Test case for pipeline_service_get_pipeline
 
         Finds a specific pipeline by ID.  # noqa: E501
         """
         pass
 
-    def test_get_pipeline_version(self):
-        """Test case for get_pipeline_version
+    def test_pipeline_service_get_pipeline_version(self):
+        """Test case for pipeline_service_get_pipeline_version
 
         Gets a pipeline version by pipeline version ID.  # noqa: E501
         """
         pass
 
-    def test_get_pipeline_version_template(self):
-        """Test case for get_pipeline_version_template
+    def test_pipeline_service_get_pipeline_version_template(self):
+        """Test case for pipeline_service_get_pipeline_version_template
 
         Returns a YAML template that contains the specified pipeline version's description, parameters and metadata.  # noqa: E501
         """
         pass
 
-    def test_get_template(self):
-        """Test case for get_template
+    def test_pipeline_service_get_template(self):
+        """Test case for pipeline_service_get_template
 
         Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.  # noqa: E501
         """
         pass
 
-    def test_list_pipeline_versions(self):
-        """Test case for list_pipeline_versions
+    def test_pipeline_service_list_pipeline_versions(self):
+        """Test case for pipeline_service_list_pipeline_versions
 
         Lists all pipeline versions of a given pipeline.  # noqa: E501
         """
         pass
 
-    def test_list_pipelines(self):
-        """Test case for list_pipelines
+    def test_pipeline_service_list_pipelines(self):
+        """Test case for pipeline_service_list_pipelines
 
         Finds all pipelines.  # noqa: E501
         """
         pass
 
-    def test_update_pipeline_default_version(self):
-        """Test case for update_pipeline_default_version
+    def test_pipeline_service_update_pipeline_default_version(self):
+        """Test case for pipeline_service_update_pipeline_default_version
 
         Update the default pipeline version of a specific pipeline.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_spec_runtime_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_upload_service_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_protobuf_any.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -32,14 +32,15 @@
         """Test ProtobufAny
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kfp_tekton_server_api.models.protobuf_any.ProtobufAny()  # noqa: E501
         if include_optional :
             return ProtobufAny(
+                type = '0', 
                 type_url = '0', 
                 value = 'YQ=='
             )
         else :
             return ProtobufAny(
         )
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_run_metric_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_run_service_api.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_run_service_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -24,79 +24,79 @@
 
     def setUp(self):
         self.api = kfp_tekton_server_api.api.run_service_api.RunServiceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_archive_run(self):
-        """Test case for archive_run
+    def test_run_service_archive_run(self):
+        """Test case for run_service_archive_run
 
         Archives a run.  # noqa: E501
         """
         pass
 
-    def test_create_run(self):
-        """Test case for create_run
+    def test_run_service_create_run(self):
+        """Test case for run_service_create_run
 
         Creates a new run.  # noqa: E501
         """
         pass
 
-    def test_delete_run(self):
-        """Test case for delete_run
+    def test_run_service_delete_run(self):
+        """Test case for run_service_delete_run
 
         Deletes a run.  # noqa: E501
         """
         pass
 
-    def test_get_run(self):
-        """Test case for get_run
+    def test_run_service_get_run(self):
+        """Test case for run_service_get_run
 
         Finds a specific run by ID.  # noqa: E501
         """
         pass
 
-    def test_list_runs(self):
-        """Test case for list_runs
+    def test_run_service_list_runs(self):
+        """Test case for run_service_list_runs
 
         Finds all runs.  # noqa: E501
         """
         pass
 
-    def test_read_artifact(self):
-        """Test case for read_artifact
+    def test_run_service_read_artifact(self):
+        """Test case for run_service_read_artifact
 
         Finds a run's artifact data.  # noqa: E501
         """
         pass
 
-    def test_report_run_metrics(self):
-        """Test case for report_run_metrics
+    def test_run_service_report_run_metrics(self):
+        """Test case for run_service_report_run_metrics
 
         ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.  # noqa: E501
         """
         pass
 
-    def test_retry_run(self):
-        """Test case for retry_run
+    def test_run_service_retry_run(self):
+        """Test case for run_service_retry_run
 
         Re-initiates a failed or terminated run.  # noqa: E501
         """
         pass
 
-    def test_terminate_run(self):
-        """Test case for terminate_run
+    def test_run_service_terminate_run(self):
+        """Test case for run_service_terminate_run
 
         Terminates an active run.  # noqa: E501
         """
         pass
 
-    def test_unarchive_run(self):
-        """Test case for unarchive_run
+    def test_run_service_unarchive_run(self):
+        """Test case for run_service_unarchive_run
 
         Restores an archived run.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_cron_schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment_storage_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_healthz_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_template_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_job.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_experiments_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_jobs_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_list_pipeline_versions_response import V1ListPipelineVersionsResponse  # noqa: E501
+from kfp_tekton_server_api.models.v1_pipeline_version import V1PipelineVersion  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1ListPipelineVersionsResponse(unittest.TestCase):
-    """V1ListPipelineVersionsResponse unit test stubs"""
+class TestV1PipelineVersion(unittest.TestCase):
+    """V1PipelineVersion unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ListPipelineVersionsResponse
+        """Test V1PipelineVersion
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_list_pipeline_versions_response.V1ListPipelineVersionsResponse()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_pipeline_version.V1PipelineVersion()  # noqa: E501
         if include_optional :
-            return V1ListPipelineVersionsResponse(
-                versions = [
-                    kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
-                        id = '0', 
+            return V1PipelineVersion(
+                id = '0', 
+                name = '0', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                parameters = [
+                    kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                         name = '0', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        parameters = [
-                            kfp_tekton_server_api.models.v1_parameter.v1Parameter(
-                                name = '0', 
-                                value = '0', )
-                            ], 
-                        code_source_url = '0', 
-                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                            pipeline_url = '0', ), 
-                        resource_references = [
-                            kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                                    type = 'UNKNOWN_RESOURCE_TYPE', 
-                                    id = '0', ), 
-                                name = '0', 
-                                relationship = 'UNKNOWN_RELATIONSHIP', )
-                            ], 
-                        description = '0', )
+                        value = '0', )
                     ], 
-                next_page_token = '0', 
-                total_size = 56
+                code_source_url = '0', 
+                package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                    pipeline_url = '0', 
+                    pipeline_url = '0', ), 
+                resource_references = [
+                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                            type = 'UNKNOWN_RESOURCE_TYPE', 
+                            id = '0', ), 
+                        name = '0', 
+                        relationship = 'UNKNOWN_RELATIONSHIP', )
+                    ], 
+                description = '0', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                code_source_url = '0', 
+                package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                    pipeline_url = '0', 
+                    pipeline_url = '0', ), 
+                resource_references = [
+                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                            type = 'UNKNOWN_RESOURCE_TYPE', 
+                            id = '0', ), 
+                        name = '0', 
+                        relationship = 'UNKNOWN_RELATIONSHIP', )
+                    ]
             )
         else :
-            return V1ListPipelineVersionsResponse(
+            return V1PipelineVersion(
         )
 
-    def testV1ListPipelineVersionsResponse(self):
-        """Test V1ListPipelineVersionsResponse"""
+    def testV1PipelineVersion(self):
+        """Test V1PipelineVersion"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipeline_versions_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_list_pipelines_response import V1ListPipelinesResponse  # noqa: E501
+from kfp_tekton_server_api.models.v1_list_pipeline_versions_response import V1ListPipelineVersionsResponse  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1ListPipelinesResponse(unittest.TestCase):
-    """V1ListPipelinesResponse unit test stubs"""
+class TestV1ListPipelineVersionsResponse(unittest.TestCase):
+    """V1ListPipelineVersionsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ListPipelinesResponse
+        """Test V1ListPipelineVersionsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_list_pipelines_response.V1ListPipelinesResponse()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_list_pipeline_versions_response.V1ListPipelineVersionsResponse()  # noqa: E501
         if include_optional :
-            return V1ListPipelinesResponse(
-                pipelines = [
-                    kfp_tekton_server_api.models.v1_pipeline.v1Pipeline(
+            return V1ListPipelineVersionsResponse(
+                versions = [
+                    kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
                         id = '0', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         name = '0', 
-                        description = '0', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         parameters = [
                             kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                                 name = '0', 
                                 value = '0', )
                             ], 
-                        url = kfp_tekton_server_api.models.v1_url.v1Url(
+                        code_source_url = '0', 
+                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                            pipeline_url = '0', 
+                            pipeline_url = '0', ), 
+                        resource_references = [
+                            kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                                key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                                    type = 'UNKNOWN_RESOURCE_TYPE', 
+                                    id = '0', ), 
+                                name = '0', 
+                                relationship = 'UNKNOWN_RELATIONSHIP', )
+                            ], 
+                        description = '0', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        code_source_url = '0', 
+                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                            pipeline_url = '0', 
                             pipeline_url = '0', ), 
-                        error = '0', 
-                        default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
-                            id = '0', 
-                            name = '0', 
-                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            code_source_url = '0', 
-                            package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                                pipeline_url = '0', ), 
-                            resource_references = [
-                                kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                    key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                                        type = 'UNKNOWN_RESOURCE_TYPE', 
-                                        id = '0', ), 
-                                    name = '0', 
-                                    relationship = 'UNKNOWN_RELATIONSHIP', )
-                                ], 
-                            description = '0', ), 
                         resource_references = [
                             kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
                                 name = '0', )
                             ], )
                     ], 
-                total_size = 56, 
-                next_page_token = '0'
+                next_page_token = '0', 
+                total_size = 56
             )
         else :
-            return V1ListPipelinesResponse(
+            return V1ListPipelineVersionsResponse(
         )
 
-    def testV1ListPipelinesResponse(self):
-        """Test V1ListPipelinesResponse"""
+    def testV1ListPipelineVersionsResponse(self):
+        """Test V1ListPipelineVersionsResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_runs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_periodic_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -42,45 +42,57 @@
                 description = '0', 
                 parameters = [
                     kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                         name = '0', 
                         value = '0', )
                     ], 
                 url = kfp_tekton_server_api.models.v1_url.v1Url(
+                    pipeline_url = '0', 
                     pipeline_url = '0', ), 
                 error = '0', 
                 default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
                     id = '0', 
                     name = '0', 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     parameters = [
                         kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                             name = '0', 
                             value = '0', )
                         ], 
                     code_source_url = '0', 
                     package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                        pipeline_url = '0', 
                         pipeline_url = '0', ), 
                     resource_references = [
                         kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
                             key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
                                 type = 'UNKNOWN_RESOURCE_TYPE', 
                                 id = '0', ), 
                             name = '0', 
                             relationship = 'UNKNOWN_RELATIONSHIP', )
                         ], 
-                    description = '0', ), 
+                    description = '0', 
+                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    code_source_url = '0', 
+                    package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                        pipeline_url = '0', 
+                        pipeline_url = '0', ), 
+                    resource_references = [
+                        kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                            name = '0', )
+                        ], ), 
                 resource_references = [
                     kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
                         key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
                             type = 'UNKNOWN_RESOURCE_TYPE', 
                             id = '0', ), 
                         name = '0', 
                         relationship = 'UNKNOWN_RELATIONSHIP', )
-                    ]
+                    ], 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
             return V1Pipeline(
         )
 
     def testV1Pipeline(self):
         """Test V1Pipeline"""
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_read_artifact_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_report_run_metrics_request.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_metric.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_report_run_metrics_request import V1ReportRunMetricsRequest  # noqa: E501
+from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1ReportRunMetricsRequest(unittest.TestCase):
-    """V1ReportRunMetricsRequest unit test stubs"""
+class TestV1RunMetric(unittest.TestCase):
+    """V1RunMetric unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ReportRunMetricsRequest
+        """Test V1RunMetric
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_report_run_metrics_request.V1ReportRunMetricsRequest()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_run_metric.V1RunMetric()  # noqa: E501
         if include_optional :
-            return V1ReportRunMetricsRequest(
-                run_id = '0', 
-                metrics = [
-                    kfp_tekton_server_api.models.v1_run_metric.v1RunMetric(
-                        name = '0', 
-                        node_id = '0', 
-                        number_value = 1.337, 
-                        format = 'UNSPECIFIED', )
-                    ]
+            return V1RunMetric(
+                name = '0', 
+                node_id = '0', 
+                number_value = 1.337, 
+                format = 'UNSPECIFIED'
             )
         else :
-            return V1ReportRunMetricsRequest(
+            return V1RunMetric(
         )
 
-    def testV1ReportRunMetricsRequest(self):
-        """Test V1ReportRunMetricsRequest"""
+    def testV1RunMetric(self):
+        """Test V1RunMetric"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_report_run_metrics_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_run.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_inline_object.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric  # noqa: E501
+from kfp_tekton_server_api.models.inline_object import InlineObject  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1RunMetric(unittest.TestCase):
-    """V1RunMetric unit test stubs"""
+class TestInlineObject(unittest.TestCase):
+    """InlineObject unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1RunMetric
+        """Test InlineObject
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_run_metric.V1RunMetric()  # noqa: E501
+        # model = kfp_tekton_server_api.models.inline_object.InlineObject()  # noqa: E501
         if include_optional :
-            return V1RunMetric(
-                name = '0', 
-                node_id = '0', 
-                number_value = 1.337, 
-                format = 'UNSPECIFIED'
+            return InlineObject(
+                metrics = [
+                    kfp_tekton_server_api.models.v1_run_metric.v1RunMetric(
+                        name = '0', 
+                        node_id = '0', 
+                        number_value = 1.337, 
+                        format = 'UNSPECIFIED', )
+                    ]
             )
         else :
-            return V1RunMetric(
+            return InlineObject(
         )
 
-    def testV1RunMetric(self):
-        """Test V1RunMetric"""
+    def testInlineObject(self):
+        """Test InlineObject"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_storage_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_status.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -35,17 +35,17 @@
             optional params are included """
         # model = kfp_tekton_server_api.models.v1_status.V1Status()  # noqa: E501
         if include_optional :
             return V1Status(
                 error = '0', 
                 code = 56, 
                 details = [
-                    kfp_tekton_server_api.models.protobuf_any.protobufAny(
-                        type_url = '0', 
-                        value = 'YQ==', )
+                    {
+                        'key' : None
+                        }
                     ]
             )
         else :
             return V1Status(
         )
 
     def testV1Status(self):
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_url.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -32,14 +32,15 @@
         """Test V1Url
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kfp_tekton_server_api.models.v1_url.V1Url()  # noqa: E501
         if include_optional :
             return V1Url(
+                pipeline_url = '0', 
                 pipeline_url = '0'
             )
         else :
             return V1Url(
         )
 
     def testV1Url(self):
```

### Comparing `kfp-tekton-server-api-1.5.0/test/test_v1_value.py` & `kfp-tekton-server-api-1.8.0rc1/test/test_v1_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines on Tekton API
+    Kubeflow Pipelines API
 
-    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
-    Contact: prashsh1@in.ibm.com
+    Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

