# Comparing `tmp/fern_merge-0.0.27.tar.gz` & `tmp/fern_merge-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_merge-0.0.27.tar", max compression
+gzip compressed data, was "fern_merge-0.0.28.tar", max compression
```

## Comparing `fern_merge-0.0.27.tar` & `fern_merge-0.0.28.tar`

### file list

```diff
@@ -1,398 +1,421 @@
--rw-r--r--   0        0        0     2139 2023-07-12 15:28:29.095870 fern_merge-0.0.27/README.md
--rw-r--r--   0        0        0      371 2023-07-12 15:28:29.095870 fern_merge-0.0.27/pyproject.toml
--rw-r--r--   0        0        0      187 2023-07-12 15:28:29.095870 fern_merge-0.0.27/src/merge/__init__.py
--rw-r--r--   0        0        0     1547 2023-07-12 15:28:29.095870 fern_merge-0.0.27/src/merge/client.py
--rw-r--r--   0        0        0      528 2023-07-12 15:28:29.095870 fern_merge-0.0.27/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1101 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      201 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/py.typed
--rw-r--r--   0        0        0      116 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/__init__.py
--rw-r--r--   0        0        0     8148 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2284 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    12088 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    14581 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    11850 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2304 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    16506 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2045 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     5972 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0     8117 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2362 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2537 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    12540 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0     6768 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0     6771 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0     8227 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4774 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5305 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0     8095 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     5900 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4816 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2545 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     6014 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0     8545 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6892 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2644 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     4201 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0     7399 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4191 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    11068 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2681 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0     2087 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0     1109 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0     2473 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-12 15:28:29.099870 fern_merge-0.0.27/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2128 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0     1780 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0     1117 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2290 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0     1478 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0     3803 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1504 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0     1506 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      742 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1336 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      555 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3441 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0     1045 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     1946 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0     2799 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0     1832 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1602 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0     1604 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0     1039 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0     2543 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      723 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3200 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2455 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0     1150 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      893 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2677 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0     1731 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1662 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1664 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0     1451 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      762 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0     8534 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2286 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2306 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0     8705 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0     6633 2023-07-12 15:28:29.103870 fern_merge-0.0.27/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     5928 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0     8024 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    17328 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0     8741 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0     7291 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0     6772 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4776 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5307 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0     7265 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4818 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     5946 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0     8756 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2547 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6898 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2646 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0     6609 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    12810 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0     8364 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4195 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    11775 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2386 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      529 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2290 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0     1478 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2156 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      949 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6740 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0     2796 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6116 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0     1109 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18592 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      770 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2238 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0     1136 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0     1336 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      555 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-12 15:28:29.107870 fern_merge-0.0.27/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11846 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      509 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     1946 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      993 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2773 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      801 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3474 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2485 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0     1272 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3126 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0     1106 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1146 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      495 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-12 15:28:29.111870 fern_merge-0.0.27/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.27/PKG-INFO
+-rw-r--r--   0        0        0     2139 2023-07-12 19:36:44.472510 fern_merge-0.0.28/README.md
+-rw-r--r--   0        0        0      371 2023-07-12 19:36:44.472510 fern_merge-0.0.28/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/client.py
+-rw-r--r--   0        0        0      528 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1101 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      201 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/py.typed
+-rw-r--r--   0        0        0      116 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0     8926 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2284 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    12088 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    14581 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    11850 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2304 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    16506 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2045 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     5972 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0     8117 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2362 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    12540 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0     6768 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0     6771 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     8227 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4774 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5305 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0     8095 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     5900 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4816 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2545 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     6014 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0     8545 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     6892 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2644 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     4201 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0     7399 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4191 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    12298 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2693 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2121 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0     1109 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0     2473 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0     3803 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1336 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      555 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3441 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0     1045 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     1946 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0     2799 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0     1832 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2543 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      723 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3200 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2455 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0     1150 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      893 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2677 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0     1731 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9130 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2286 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2306 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0     8705 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0     6633 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     5928 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8024 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    17328 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0     8741 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0     7291 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0     6772 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4776 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5307 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0     7265 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4818 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     5946 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8756 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2547 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     6898 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2646 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0     6609 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    12810 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0     8364 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4195 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    12720 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6740 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0     2796 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6116 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0     1109 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18610 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      770 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0     1336 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      555 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11858 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      189 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     1946 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      993 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2792 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      171 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3484 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3158 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      184 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0     1106 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1146 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      495 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.28/PKG-INFO
```

### Comparing `fern_merge-0.0.27/README.md` & `fern_merge-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/client.py` & `fern_merge-0.0.28/src/merge/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/core/__init__.py` & `fern_merge-0.0.28/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/core/client_wrapper.py` & `fern_merge-0.0.28/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/core/datetime_utils.py` & `fern_merge-0.0.28/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/core/jsonable_encoder.py` & `fern_merge-0.0.28/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/__init__.py` & `fern_merge-0.0.28/src/merge/resources/ats/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,55 @@
     AccountIntegration,
     AccountToken,
     ActivitiesListRequestRemoteFields,
     ActivitiesListRequestShowEnumOrigins,
     ActivitiesRetrieveRequestRemoteFields,
     ActivitiesRetrieveRequestShowEnumOrigins,
     Activity,
+    ActivityActivityType,
     ActivityRequest,
+    ActivityRequestActivityType,
     ActivityResponse,
     ActivityTypeEnum,
     Application,
     ApplicationRequest,
     ApplicationResponse,
     ApplicationsListRequestExpand,
     ApplicationsRetrieveRequestExpand,
     Attachment,
+    AttachmentAttachmentType,
     AttachmentRequest,
+    AttachmentRequestAttachmentType,
     AttachmentResponse,
     AttachmentTypeEnum,
     AvailableActions,
     Candidate,
     CandidateRequest,
     CandidateResponse,
     CandidatesListRequestExpand,
     CandidatesRetrieveRequestExpand,
     CategoriesEnum,
     CategoryEnum,
     CommonModelScopesBodyRequest,
     ConditionSchema,
+    ConditionSchemaConditionType,
     ConditionTypeEnum,
     DebugModeLog,
     DebugModelLogSummary,
     Department,
     DisabilityStatusEnum,
     Eeoc,
     EeocsListRequestRemoteFields,
     EeocsListRequestShowEnumOrigins,
     EeocsRetrieveRequestRemoteFields,
     EeocsRetrieveRequestShowEnumOrigins,
     EmailAddress,
+    EmailAddressEmailAddressType,
     EmailAddressRequest,
+    EmailAddressRequestEmailAddressType,
     EmailAddressTypeEnum,
     EnabledActionsEnum,
     EncodingEnum,
     ErrorValidationProblem,
     GenderEnum,
     InterviewsListRequestExpand,
     InterviewsRetrieveRequestExpand,
@@ -98,22 +105,25 @@
     PaginatedRemoteUserList,
     PaginatedScheduledInterviewList,
     PaginatedScorecardList,
     PaginatedSyncStatusList,
     PaginatedTagList,
     PatchedCandidateRequest,
     PhoneNumber,
+    PhoneNumberPhoneNumberType,
     PhoneNumberRequest,
+    PhoneNumberRequestPhoneNumberType,
     PhoneNumberTypeEnum,
     RaceEnum,
     ReasonEnum,
     RejectReason,
     RemoteData,
     RemoteKey,
     RemoteResponse,
+    RemoteResponseResponseType,
     RemoteUser,
     RequestFormatEnum,
     ResponseTypeEnum,
     ScheduledInterview,
     ScheduledInterviewRequest,
     ScheduledInterviewResponse,
     ScheduledInterviewStatusEnum,
@@ -122,15 +132,17 @@
     ScorecardsRetrieveRequestExpand,
     SelectiveSyncConfigurationsUsageEnum,
     SyncStatus,
     SyncStatusStatusEnum,
     Tag,
     Url,
     UrlRequest,
+    UrlRequestUrlType,
     UrlTypeEnum,
+    UrlUrlType,
     ValidationProblemSource,
     VeteranStatusEnum,
     VisibilityEnum,
     WarningValidationProblem,
     WebhookReceiver,
 )
 from .resources import (
@@ -174,48 +186,55 @@
     "AccountIntegration",
     "AccountToken",
     "ActivitiesListRequestRemoteFields",
     "ActivitiesListRequestShowEnumOrigins",
     "ActivitiesRetrieveRequestRemoteFields",
     "ActivitiesRetrieveRequestShowEnumOrigins",
     "Activity",
+    "ActivityActivityType",
     "ActivityRequest",
+    "ActivityRequestActivityType",
     "ActivityResponse",
     "ActivityTypeEnum",
     "Application",
     "ApplicationRequest",
     "ApplicationResponse",
     "ApplicationsListRequestExpand",
     "ApplicationsRetrieveRequestExpand",
     "Attachment",
+    "AttachmentAttachmentType",
     "AttachmentRequest",
+    "AttachmentRequestAttachmentType",
     "AttachmentResponse",
     "AttachmentTypeEnum",
     "AvailableActions",
     "Candidate",
     "CandidateRequest",
     "CandidateResponse",
     "CandidatesListRequestExpand",
     "CandidatesRetrieveRequestExpand",
     "CategoriesEnum",
     "CategoryEnum",
     "CommonModelScopesBodyRequest",
     "ConditionSchema",
+    "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Department",
     "DisabilityStatusEnum",
     "Eeoc",
     "EeocsListRequestRemoteFields",
     "EeocsListRequestShowEnumOrigins",
     "EeocsRetrieveRequestRemoteFields",
     "EeocsRetrieveRequestShowEnumOrigins",
     "EmailAddress",
+    "EmailAddressEmailAddressType",
     "EmailAddressRequest",
+    "EmailAddressRequestEmailAddressType",
     "EmailAddressTypeEnum",
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "GenderEnum",
     "InterviewsListRequestExpand",
     "InterviewsRetrieveRequestExpand",
@@ -263,22 +282,25 @@
     "PaginatedRemoteUserList",
     "PaginatedScheduledInterviewList",
     "PaginatedScorecardList",
     "PaginatedSyncStatusList",
     "PaginatedTagList",
     "PatchedCandidateRequest",
     "PhoneNumber",
+    "PhoneNumberPhoneNumberType",
     "PhoneNumberRequest",
+    "PhoneNumberRequestPhoneNumberType",
     "PhoneNumberTypeEnum",
     "RaceEnum",
     "ReasonEnum",
     "RejectReason",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
+    "RemoteResponseResponseType",
     "RemoteUser",
     "RequestFormatEnum",
     "ResponseTypeEnum",
     "ScheduledInterview",
     "ScheduledInterviewRequest",
     "ScheduledInterviewResponse",
     "ScheduledInterviewStatusEnum",
@@ -287,15 +309,17 @@
     "ScorecardsRetrieveRequestExpand",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tag",
     "Url",
     "UrlRequest",
+    "UrlRequestUrlType",
     "UrlTypeEnum",
+    "UrlUrlType",
     "ValidationProblemSource",
     "VeteranStatusEnum",
     "VisibilityEnum",
     "WarningValidationProblem",
     "WebhookReceiver",
     "account_details",
     "account_token",
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/__init__.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/account_details/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/account_token/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/activities/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/applications/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/attachments/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/available_actions/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/candidates/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/delete_account/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/departments/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/eeocs/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/force_resync/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/generate_key/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/interviews/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/issues/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/job_interview_stages/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/jobs/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/link_token/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/linked_accounts/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/offers/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/offices/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/passthrough/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/regenerate_key/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/reject_reasons/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/scorecards/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/selective_sync/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/sync_status/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/tags/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/users/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/resources/webhook_receivers/client.py` & `fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/__init__.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,48 +8,55 @@
 from .account_integration import AccountIntegration
 from .account_token import AccountToken
 from .activities_list_request_remote_fields import ActivitiesListRequestRemoteFields
 from .activities_list_request_show_enum_origins import ActivitiesListRequestShowEnumOrigins
 from .activities_retrieve_request_remote_fields import ActivitiesRetrieveRequestRemoteFields
 from .activities_retrieve_request_show_enum_origins import ActivitiesRetrieveRequestShowEnumOrigins
 from .activity import Activity
+from .activity_activity_type import ActivityActivityType
 from .activity_request import ActivityRequest
+from .activity_request_activity_type import ActivityRequestActivityType
 from .activity_response import ActivityResponse
 from .activity_type_enum import ActivityTypeEnum
 from .application import Application
 from .application_request import ApplicationRequest
 from .application_response import ApplicationResponse
 from .applications_list_request_expand import ApplicationsListRequestExpand
 from .applications_retrieve_request_expand import ApplicationsRetrieveRequestExpand
 from .attachment import Attachment
+from .attachment_attachment_type import AttachmentAttachmentType
 from .attachment_request import AttachmentRequest
+from .attachment_request_attachment_type import AttachmentRequestAttachmentType
 from .attachment_response import AttachmentResponse
 from .attachment_type_enum import AttachmentTypeEnum
 from .available_actions import AvailableActions
 from .candidate import Candidate
 from .candidate_request import CandidateRequest
 from .candidate_response import CandidateResponse
 from .candidates_list_request_expand import CandidatesListRequestExpand
 from .candidates_retrieve_request_expand import CandidatesRetrieveRequestExpand
 from .categories_enum import CategoriesEnum
 from .category_enum import CategoryEnum
 from .common_model_scopes_body_request import CommonModelScopesBodyRequest
 from .condition_schema import ConditionSchema
+from .condition_schema_condition_type import ConditionSchemaConditionType
 from .condition_type_enum import ConditionTypeEnum
 from .debug_mode_log import DebugModeLog
 from .debug_model_log_summary import DebugModelLogSummary
 from .department import Department
 from .disability_status_enum import DisabilityStatusEnum
 from .eeoc import Eeoc
 from .eeocs_list_request_remote_fields import EeocsListRequestRemoteFields
 from .eeocs_list_request_show_enum_origins import EeocsListRequestShowEnumOrigins
 from .eeocs_retrieve_request_remote_fields import EeocsRetrieveRequestRemoteFields
 from .eeocs_retrieve_request_show_enum_origins import EeocsRetrieveRequestShowEnumOrigins
 from .email_address import EmailAddress
+from .email_address_email_address_type import EmailAddressEmailAddressType
 from .email_address_request import EmailAddressRequest
+from .email_address_request_email_address_type import EmailAddressRequestEmailAddressType
 from .email_address_type_enum import EmailAddressTypeEnum
 from .enabled_actions_enum import EnabledActionsEnum
 from .encoding_enum import EncodingEnum
 from .error_validation_problem import ErrorValidationProblem
 from .gender_enum import GenderEnum
 from .interviews_list_request_expand import InterviewsListRequestExpand
 from .interviews_retrieve_request_expand import InterviewsRetrieveRequestExpand
@@ -97,22 +104,25 @@
 from .paginated_remote_user_list import PaginatedRemoteUserList
 from .paginated_scheduled_interview_list import PaginatedScheduledInterviewList
 from .paginated_scorecard_list import PaginatedScorecardList
 from .paginated_sync_status_list import PaginatedSyncStatusList
 from .paginated_tag_list import PaginatedTagList
 from .patched_candidate_request import PatchedCandidateRequest
 from .phone_number import PhoneNumber
+from .phone_number_phone_number_type import PhoneNumberPhoneNumberType
 from .phone_number_request import PhoneNumberRequest
+from .phone_number_request_phone_number_type import PhoneNumberRequestPhoneNumberType
 from .phone_number_type_enum import PhoneNumberTypeEnum
 from .race_enum import RaceEnum
 from .reason_enum import ReasonEnum
 from .reject_reason import RejectReason
 from .remote_data import RemoteData
 from .remote_key import RemoteKey
 from .remote_response import RemoteResponse
+from .remote_response_response_type import RemoteResponseResponseType
 from .remote_user import RemoteUser
 from .request_format_enum import RequestFormatEnum
 from .response_type_enum import ResponseTypeEnum
 from .scheduled_interview import ScheduledInterview
 from .scheduled_interview_request import ScheduledInterviewRequest
 from .scheduled_interview_response import ScheduledInterviewResponse
 from .scheduled_interview_status_enum import ScheduledInterviewStatusEnum
@@ -121,15 +131,17 @@
 from .scorecards_retrieve_request_expand import ScorecardsRetrieveRequestExpand
 from .selective_sync_configurations_usage_enum import SelectiveSyncConfigurationsUsageEnum
 from .sync_status import SyncStatus
 from .sync_status_status_enum import SyncStatusStatusEnum
 from .tag import Tag
 from .url import Url
 from .url_request import UrlRequest
+from .url_request_url_type import UrlRequestUrlType
 from .url_type_enum import UrlTypeEnum
+from .url_url_type import UrlUrlType
 from .validation_problem_source import ValidationProblemSource
 from .veteran_status_enum import VeteranStatusEnum
 from .visibility_enum import VisibilityEnum
 from .warning_validation_problem import WarningValidationProblem
 from .webhook_receiver import WebhookReceiver
 
 __all__ = [
@@ -141,48 +153,55 @@
     "AccountIntegration",
     "AccountToken",
     "ActivitiesListRequestRemoteFields",
     "ActivitiesListRequestShowEnumOrigins",
     "ActivitiesRetrieveRequestRemoteFields",
     "ActivitiesRetrieveRequestShowEnumOrigins",
     "Activity",
+    "ActivityActivityType",
     "ActivityRequest",
+    "ActivityRequestActivityType",
     "ActivityResponse",
     "ActivityTypeEnum",
     "Application",
     "ApplicationRequest",
     "ApplicationResponse",
     "ApplicationsListRequestExpand",
     "ApplicationsRetrieveRequestExpand",
     "Attachment",
+    "AttachmentAttachmentType",
     "AttachmentRequest",
+    "AttachmentRequestAttachmentType",
     "AttachmentResponse",
     "AttachmentTypeEnum",
     "AvailableActions",
     "Candidate",
     "CandidateRequest",
     "CandidateResponse",
     "CandidatesListRequestExpand",
     "CandidatesRetrieveRequestExpand",
     "CategoriesEnum",
     "CategoryEnum",
     "CommonModelScopesBodyRequest",
     "ConditionSchema",
+    "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Department",
     "DisabilityStatusEnum",
     "Eeoc",
     "EeocsListRequestRemoteFields",
     "EeocsListRequestShowEnumOrigins",
     "EeocsRetrieveRequestRemoteFields",
     "EeocsRetrieveRequestShowEnumOrigins",
     "EmailAddress",
+    "EmailAddressEmailAddressType",
     "EmailAddressRequest",
+    "EmailAddressRequestEmailAddressType",
     "EmailAddressTypeEnum",
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "GenderEnum",
     "InterviewsListRequestExpand",
     "InterviewsRetrieveRequestExpand",
@@ -230,22 +249,25 @@
     "PaginatedRemoteUserList",
     "PaginatedScheduledInterviewList",
     "PaginatedScorecardList",
     "PaginatedSyncStatusList",
     "PaginatedTagList",
     "PatchedCandidateRequest",
     "PhoneNumber",
+    "PhoneNumberPhoneNumberType",
     "PhoneNumberRequest",
+    "PhoneNumberRequestPhoneNumberType",
     "PhoneNumberTypeEnum",
     "RaceEnum",
     "ReasonEnum",
     "RejectReason",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
+    "RemoteResponseResponseType",
     "RemoteUser",
     "RequestFormatEnum",
     "ResponseTypeEnum",
     "ScheduledInterview",
     "ScheduledInterviewRequest",
     "ScheduledInterviewResponse",
     "ScheduledInterviewStatusEnum",
@@ -254,14 +276,16 @@
     "ScorecardsRetrieveRequestExpand",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tag",
     "Url",
     "UrlRequest",
+    "UrlRequestUrlType",
     "UrlTypeEnum",
+    "UrlUrlType",
     "ValidationProblemSource",
     "VeteranStatusEnum",
     "VisibilityEnum",
     "WarningValidationProblem",
     "WebhookReceiver",
 ]
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/access_role_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_details.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_integration.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/account_token.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activity.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .activity_type_enum import ActivityTypeEnum
+from .activity_activity_type import ActivityActivityType
 from .remote_data import RemoteData
 from .visibility_enum import VisibilityEnum
 
 
 class Activity(pydantic.BaseModel):
     """
     # The Activity Object
@@ -20,15 +20,15 @@
     Fetch from the `LIST Activities` endpoint and filter by `ID` to show all activities.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     user: typing.Optional[str] = pydantic.Field(description="The user that performed the action.")
     remote_created_at: typing.Optional[str] = pydantic.Field(description="When the third party's activity was created.")
-    activity_type: typing.Optional[ActivityTypeEnum] = pydantic.Field(
+    activity_type: typing.Optional[ActivityActivityType] = pydantic.Field(
         description=("The activity's type.\n" "\n" "* `NOTE` - NOTE\n" "* `EMAIL` - EMAIL\n" "* `OTHER` - OTHER\n")
     )
     subject: typing.Optional[str] = pydantic.Field(description="The activity's subject.")
     body: typing.Optional[str] = pydantic.Field(description="The activity's body.")
     visibility: typing.Optional[VisibilityEnum] = pydantic.Field(
         description=(
             "The activity's visibility.\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activity_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activity_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .activity_type_enum import ActivityTypeEnum
+from .activity_request_activity_type import ActivityRequestActivityType
 from .visibility_enum import VisibilityEnum
 
 
 class ActivityRequest(pydantic.BaseModel):
     """
     # The Activity Object
     ### Description
     The `Activity` object is used to represent an activity for a candidate performed by a user.
     ### Usage Example
     Fetch from the `LIST Activities` endpoint and filter by `ID` to show all activities.
     """
 
     user: typing.Optional[str] = pydantic.Field(description="The user that performed the action.")
-    activity_type: typing.Optional[ActivityTypeEnum] = pydantic.Field(
+    activity_type: typing.Optional[ActivityRequestActivityType] = pydantic.Field(
         description=("The activity's type.\n" "\n" "* `NOTE` - NOTE\n" "* `EMAIL` - EMAIL\n" "* `OTHER` - OTHER\n")
     )
     subject: typing.Optional[str] = pydantic.Field(description="The activity's subject.")
     body: typing.Optional[str] = pydantic.Field(description="The activity's body.")
     visibility: typing.Optional[VisibilityEnum] = pydantic.Field(
         description=(
             "The activity's visibility.\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activity_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/activity_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/application.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/application_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/application_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/applications_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/attachment.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .attachment_type_enum import AttachmentTypeEnum
+from .attachment_attachment_type import AttachmentAttachmentType
 from .remote_data import RemoteData
 
 
 class Attachment(pydantic.BaseModel):
     """
     # The Attachment Object
     ### Description
@@ -20,15 +20,15 @@
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     file_name: typing.Optional[str] = pydantic.Field(description="The attachment's name.")
     file_url: typing.Optional[str] = pydantic.Field(description="The attachment's url.")
     candidate: typing.Optional[str] = pydantic.Field(description="")
-    attachment_type: typing.Optional[AttachmentTypeEnum] = pydantic.Field(
+    attachment_type: typing.Optional[AttachmentAttachmentType] = pydantic.Field(
         description=(
             "The attachment's type.\n"
             "\n"
             "* `RESUME` - RESUME\n"
             "* `COVER_LETTER` - COVER_LETTER\n"
             "* `OFFER_LETTER` - OFFER_LETTER\n"
             "* `OTHER` - OTHER\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/attachment_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .attachment_type_enum import AttachmentTypeEnum
+from .attachment_request_attachment_type import AttachmentRequestAttachmentType
 
 
 class AttachmentRequest(pydantic.BaseModel):
     """
     # The Attachment Object
     ### Description
     The `Attachment` object is used to represent a file attached to a candidate.
     ### Usage Example
     Fetch from the `LIST Attachments` endpoint and view attachments accessible by a company.
     """
 
     file_name: typing.Optional[str] = pydantic.Field(description="The attachment's name.")
     file_url: typing.Optional[str] = pydantic.Field(description="The attachment's url.")
     candidate: typing.Optional[str] = pydantic.Field(description="")
-    attachment_type: typing.Optional[AttachmentTypeEnum] = pydantic.Field(
+    attachment_type: typing.Optional[AttachmentRequestAttachmentType] = pydantic.Field(
         description=(
             "The attachment's type.\n"
             "\n"
             "* `RESUME` - RESUME\n"
             "* `COVER_LETTER` - COVER_LETTER\n"
             "* `OFFER_LETTER` - OFFER_LETTER\n"
             "* `OTHER` - OTHER\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/attachment_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/attachment_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/available_actions.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/candidate.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/candidate_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/candidate_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/candidates_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/categories_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/category_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/condition_schema.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .condition_type_enum import ConditionTypeEnum
+from .condition_schema_condition_type import ConditionSchemaConditionType
 from .operator_schema import OperatorSchema
 
 
 class ConditionSchema(pydantic.BaseModel):
     id: str = pydantic.Field(
         description="The ID of the condition schema. This ID is used when updating selective syncs for a linked account."
     )
@@ -22,15 +22,15 @@
     )
     field_name: typing.Optional[str] = pydantic.Field(
         description='The name of the field on the common model that this condition corresponds to, if they conceptually match. e.g. "location_type".'
     )
     is_unique: typing.Optional[bool] = pydantic.Field(
         description="Whether this condition can only be applied once. If false, the condition can be AND'd together multiple times."
     )
-    condition_type: ConditionTypeEnum = pydantic.Field(
+    condition_type: ConditionSchemaConditionType = pydantic.Field(
         description=(
             "The type of value(s) that can be set for this condition.\n"
             "\n"
             "* `BOOLEAN` - BOOLEAN\n"
             "* `DATE` - DATE\n"
             "* `DATE_TIME` - DATE_TIME\n"
             "* `INTEGER` - INTEGER\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/condition_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/debug_mode_log.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/debug_model_log_summary.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/department.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/disability_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/eeoc.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/email_address.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/email_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_address_type_enum import EmailAddressTypeEnum
+from .email_address_email_address_type import EmailAddressEmailAddressType
 
 
 class EmailAddress(pydantic.BaseModel):
     """
     # The EmailAddress Object
     ### Description
     The `EmailAddress` object is used to represent a candidate's email address.
     ### Usage Example
     Fetch from the `GET Candidate` endpoint and view their email addresses.
     """
 
     value: typing.Optional[str] = pydantic.Field(description="The email address.")
-    email_address_type: typing.Optional[EmailAddressTypeEnum] = pydantic.Field(
+    email_address_type: typing.Optional[EmailAddressEmailAddressType] = pydantic.Field(
         description=(
             "The type of email address.\n" "\n" "* `PERSONAL` - PERSONAL\n" "* `WORK` - WORK\n" "* `OTHER` - OTHER\n"
         )
     )
     modified_at: typing.Optional[str] = pydantic.Field(
         description="This is the datetime that this object was last updated by Merge"
     )
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/email_address_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_address_type_enum import EmailAddressTypeEnum
+from .email_address_request_email_address_type import EmailAddressRequestEmailAddressType
 
 
 class EmailAddressRequest(pydantic.BaseModel):
     """
     # The EmailAddress Object
     ### Description
     The `EmailAddress` object is used to represent a candidate's email address.
     ### Usage Example
     Fetch from the `GET Candidate` endpoint and view their email addresses.
     """
 
     value: typing.Optional[str] = pydantic.Field(description="The email address.")
-    email_address_type: typing.Optional[EmailAddressTypeEnum] = pydantic.Field(
+    email_address_type: typing.Optional[EmailAddressRequestEmailAddressType] = pydantic.Field(
         description=(
             "The type of email address.\n" "\n" "* `PERSONAL` - PERSONAL\n" "* `WORK` - WORK\n" "* `OTHER` - OTHER\n"
         )
     )
     integration_params: typing.Optional[typing.Dict[str, typing.Any]]
     linked_account_params: typing.Optional[typing.Dict[str, typing.Any]]
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/email_address_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/enabled_actions_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/encoding_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/error_validation_problem.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/gender_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/interviews_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/issue.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/issue_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/job.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/job_interview_stage.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/job_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/jobs_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/jobs_list_request_status.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/link_token.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_condition.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_condition_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_account_status.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/meta_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/method_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/model_operation.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/multipart_form_field_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/offer.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/offer_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/offers_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/office.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/operator_schema.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/overall_recommendation_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_activity_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_application_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_attachment_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_candidate_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_department_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_eeoc_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_issue_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_job_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_offer_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_office_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_remote_user_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_scorecard_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_sync_status_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/paginated_tag_list.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/patched_candidate_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/phone_number.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/phone_number.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .phone_number_type_enum import PhoneNumberTypeEnum
+from .phone_number_phone_number_type import PhoneNumberPhoneNumberType
 
 
 class PhoneNumber(pydantic.BaseModel):
     """
     # The PhoneNumber Object
     ### Description
     The `PhoneNumber` object is used to represent a candidate's phone number.
     ### Usage Example
     Fetch from the `GET Candidate` endpoint and view their phone numbers.
     """
 
     value: typing.Optional[str] = pydantic.Field(description="The phone number.")
-    phone_number_type: typing.Optional[PhoneNumberTypeEnum] = pydantic.Field(
+    phone_number_type: typing.Optional[PhoneNumberPhoneNumberType] = pydantic.Field(
         description=(
             "The type of phone number.\n"
             "\n"
             "* `HOME` - HOME\n"
             "* `WORK` - WORK\n"
             "* `MOBILE` - MOBILE\n"
             "* `SKYPE` - SKYPE\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/phone_number_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/url_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .phone_number_type_enum import PhoneNumberTypeEnum
+from .url_request_url_type import UrlRequestUrlType
 
 
-class PhoneNumberRequest(pydantic.BaseModel):
+class UrlRequest(pydantic.BaseModel):
     """
-    # The PhoneNumber Object
+    # The Url Object
     ### Description
-    The `PhoneNumber` object is used to represent a candidate's phone number.
+    The `Url` object is used to represent hyperlinks associated with the parent model.
     ### Usage Example
-    Fetch from the `GET Candidate` endpoint and view their phone numbers.
+    Fetch from the `GET Candidate` endpoint and view their website urls.
     """
 
-    value: typing.Optional[str] = pydantic.Field(description="The phone number.")
-    phone_number_type: typing.Optional[PhoneNumberTypeEnum] = pydantic.Field(
+    value: typing.Optional[str] = pydantic.Field(description="The site's url.")
+    url_type: typing.Optional[UrlRequestUrlType] = pydantic.Field(
         description=(
-            "The type of phone number.\n"
+            "The type of site.\n"
             "\n"
-            "* `HOME` - HOME\n"
-            "* `WORK` - WORK\n"
-            "* `MOBILE` - MOBILE\n"
-            "* `SKYPE` - SKYPE\n"
+            "* `PERSONAL` - PERSONAL\n"
+            "* `COMPANY` - COMPANY\n"
+            "* `PORTFOLIO` - PORTFOLIO\n"
+            "* `BLOG` - BLOG\n"
+            "* `SOCIAL_MEDIA` - SOCIAL_MEDIA\n"
             "* `OTHER` - OTHER\n"
+            "* `JOB_POSTING` - JOB_POSTING\n"
         )
     )
     integration_params: typing.Optional[typing.Dict[str, typing.Any]]
     linked_account_params: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/phone_number_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/race_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/reason_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/reject_reason.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/remote_data.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/remote_key.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/remote_response.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/model_operation.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,34 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .response_type_enum import ResponseTypeEnum
 
 
-class RemoteResponse(pydantic.BaseModel):
+class ModelOperation(pydantic.BaseModel):
     """
-    # The RemoteResponse Object
+    # The ModelOperation Object
     ### Description
-    The `RemoteResponse` object is used to represent information returned from a third-party endpoint.
+    The `ModelOperation` object is used to represent the operations that are currently supported for a given model.
 
     ### Usage Example
-    View the `RemoteResponse` returned from your `DataPassthrough`.
+    View what operations are supported for the `Candidate` endpoint.
     """
 
-    method: str
-    path: str
-    status: int
-    response: typing.Any
-    response_headers: typing.Optional[typing.Dict[str, typing.Any]]
-    response_type: typing.Optional[ResponseTypeEnum]
-    headers: typing.Optional[typing.Dict[str, typing.Any]]
+    model_name: str
+    available_operations: typing.List[str]
+    required_post_parameters: typing.List[str]
+    supported_fields: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/remote_user.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/request_format_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/response_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_request.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scorecard.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/sync_status.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/sync_status_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/tag.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/url.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/url.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .url_type_enum import UrlTypeEnum
+from .url_url_type import UrlUrlType
 
 
 class Url(pydantic.BaseModel):
     """
     # The Url Object
     ### Description
     The `Url` object is used to represent hyperlinks associated with the parent model.
     ### Usage Example
     Fetch from the `GET Candidate` endpoint and view their website urls.
     """
 
     value: typing.Optional[str] = pydantic.Field(description="The site's url.")
-    url_type: typing.Optional[UrlTypeEnum] = pydantic.Field(
+    url_type: typing.Optional[UrlUrlType] = pydantic.Field(
         description=(
             "The type of site.\n"
             "\n"
             "* `PERSONAL` - PERSONAL\n"
             "* `COMPANY` - COMPANY\n"
             "* `PORTFOLIO` - PORTFOLIO\n"
             "* `BLOG` - BLOG\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/url_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/earning.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,42 +2,50 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .url_type_enum import UrlTypeEnum
+from .earning_type import EarningType
+from .remote_data import RemoteData
 
 
-class UrlRequest(pydantic.BaseModel):
+class Earning(pydantic.BaseModel):
     """
-    # The Url Object
+    # The Earning Object
     ### Description
-    The `Url` object is used to represent hyperlinks associated with the parent model.
+    The `Earning` object is used to represent an array of different compensations that an employee receives within specific wage categories.
+
     ### Usage Example
-    Fetch from the `GET Candidate` endpoint and view their website urls.
+    Fetch from the `LIST Earnings` endpoint and filter by `ID` to show all earnings.
     """
 
-    value: typing.Optional[str] = pydantic.Field(description="The site's url.")
-    url_type: typing.Optional[UrlTypeEnum] = pydantic.Field(
+    id: typing.Optional[str]
+    remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
+    employee_payroll_run: typing.Optional[str]
+    amount: typing.Optional[float] = pydantic.Field(description="The amount earned.")
+    type: typing.Optional[EarningType] = pydantic.Field(
         description=(
-            "The type of site.\n"
+            "The type of earning.\n"
             "\n"
-            "* `PERSONAL` - PERSONAL\n"
-            "* `COMPANY` - COMPANY\n"
-            "* `PORTFOLIO` - PORTFOLIO\n"
-            "* `BLOG` - BLOG\n"
-            "* `SOCIAL_MEDIA` - SOCIAL_MEDIA\n"
-            "* `OTHER` - OTHER\n"
-            "* `JOB_POSTING` - JOB_POSTING\n"
+            "* `SALARY` - SALARY\n"
+            "* `REIMBURSEMENT` - REIMBURSEMENT\n"
+            "* `OVERTIME` - OVERTIME\n"
+            "* `BONUS` - BONUS\n"
         )
     )
-    integration_params: typing.Optional[typing.Dict[str, typing.Any]]
-    linked_account_params: typing.Optional[typing.Dict[str, typing.Any]]
+    remote_was_deleted: typing.Optional[bool] = pydantic.Field(
+        description="Indicates whether or not this object has been deleted by third party webhooks."
+    )
+    modified_at: typing.Optional[str] = pydantic.Field(
+        description="This is the datetime that this object was last updated by Merge"
+    )
+    field_mappings: typing.Optional[typing.Dict[str, typing.Any]]
+    remote_data: typing.Optional[typing.List[RemoteData]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/url_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/validation_problem_source.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/veteran_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/visibility_enum.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/warning_validation_problem.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/ats/types/webhook_receiver.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/__init__.py` & `fern_merge-0.0.28/src/merge/resources/hris/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,31 @@
     AccountDetailsAndActionsIntegration,
     AccountDetailsAndActionsStatusEnum,
     AccountIntegration,
     AccountToken,
     AccountTypeEnum,
     AvailableActions,
     BankInfo,
+    BankInfoAccountType,
     BankInfoListRequestAccountType,
     BankInfoListRequestOrderBy,
     Benefit,
     CategoriesEnum,
     CategoryEnum,
     CommonModelScopesBodyRequest,
     Company,
     ConditionSchema,
+    ConditionSchemaConditionType,
     ConditionTypeEnum,
     CountryEnum,
     DebugModeLog,
     DebugModelLogSummary,
     Deduction,
     Earning,
+    EarningType,
     EarningTypeEnum,
     Employee,
     EmployeePayrollRun,
     EmployeePayrollRunsListRequestExpand,
     EmployeePayrollRunsRetrieveRequestExpand,
     EmployeeRequest,
     EmployeeResponse,
@@ -35,14 +38,15 @@
     EmployeesListRequestExpand,
     EmployeesListRequestRemoteFields,
     EmployeesListRequestShowEnumOrigins,
     EmployeesRetrieveRequestExpand,
     EmployeesRetrieveRequestRemoteFields,
     EmployeesRetrieveRequestShowEnumOrigins,
     Employment,
+    EmploymentEmploymentType,
     EmploymentStatusEnum,
     EmploymentTypeEnum,
     EmploymentsListRequestExpand,
     EmploymentsListRequestOrderBy,
     EmploymentsListRequestRemoteFields,
     EmploymentsListRequestShowEnumOrigins,
     EmploymentsRetrieveRequestExpand,
@@ -51,26 +55,28 @@
     EnabledActionsEnum,
     EncodingEnum,
     ErrorValidationProblem,
     EthnicityEnum,
     FlsaStatusEnum,
     GenderEnum,
     Group,
+    GroupType,
     GroupTypeEnum,
     Issue,
     IssueStatusEnum,
     IssuesListRequestStatus,
     LinkToken,
     LinkedAccountCondition,
     LinkedAccountConditionRequest,
     LinkedAccountSelectiveSyncConfiguration,
     LinkedAccountSelectiveSyncConfigurationRequest,
     LinkedAccountStatus,
     LinkedAccountsListRequestCategory,
     Location,
+    LocationLocationType,
     LocationTypeEnum,
     MaritalStatusEnum,
     MetaResponse,
     MethodEnum,
     ModelOperation,
     MultipartFormFieldRequest,
     OperatorSchema,
@@ -92,43 +98,48 @@
     PaginatedTimeOffBalanceList,
     PaginatedTimeOffList,
     PayCurrencyEnum,
     PayFrequencyEnum,
     PayGroup,
     PayPeriodEnum,
     PayrollRun,
+    PayrollRunRunType,
     PayrollRunsListRequestRemoteFields,
     PayrollRunsListRequestRunType,
     PayrollRunsListRequestShowEnumOrigins,
     PayrollRunsRetrieveRequestRemoteFields,
     PayrollRunsRetrieveRequestShowEnumOrigins,
     PolicyTypeEnum,
     ReasonEnum,
     RemoteData,
     RemoteKey,
     RemoteResponse,
+    RemoteResponseResponseType,
     RequestFormatEnum,
     RequestTypeEnum,
     ResponseTypeEnum,
     RunStateEnum,
     RunTypeEnum,
     SelectiveSyncConfigurationsUsageEnum,
     SyncStatus,
     SyncStatusStatusEnum,
     Tax,
     Team,
     TimeOff,
     TimeOffBalance,
+    TimeOffBalancePolicyType,
     TimeOffBalancesListRequestPolicyType,
     TimeOffListRequestExpand,
     TimeOffListRequestRemoteFields,
     TimeOffListRequestRequestType,
     TimeOffListRequestShowEnumOrigins,
     TimeOffListRequestStatus,
     TimeOffRequest,
+    TimeOffRequestRequestType,
+    TimeOffRequestType,
     TimeOffResponse,
     TimeOffRetrieveRequestExpand,
     TimeOffRetrieveRequestRemoteFields,
     TimeOffRetrieveRequestShowEnumOrigins,
     TimeOffStatusEnum,
     UnitsEnum,
     ValidationProblemSource,
@@ -171,28 +182,31 @@
     "AccountDetailsAndActionsIntegration",
     "AccountDetailsAndActionsStatusEnum",
     "AccountIntegration",
     "AccountToken",
     "AccountTypeEnum",
     "AvailableActions",
     "BankInfo",
+    "BankInfoAccountType",
     "BankInfoListRequestAccountType",
     "BankInfoListRequestOrderBy",
     "Benefit",
     "CategoriesEnum",
     "CategoryEnum",
     "CommonModelScopesBodyRequest",
     "Company",
     "ConditionSchema",
+    "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "CountryEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Deduction",
     "Earning",
+    "EarningType",
     "EarningTypeEnum",
     "Employee",
     "EmployeePayrollRun",
     "EmployeePayrollRunsListRequestExpand",
     "EmployeePayrollRunsRetrieveRequestExpand",
     "EmployeeRequest",
     "EmployeeResponse",
@@ -200,14 +214,15 @@
     "EmployeesListRequestExpand",
     "EmployeesListRequestRemoteFields",
     "EmployeesListRequestShowEnumOrigins",
     "EmployeesRetrieveRequestExpand",
     "EmployeesRetrieveRequestRemoteFields",
     "EmployeesRetrieveRequestShowEnumOrigins",
     "Employment",
+    "EmploymentEmploymentType",
     "EmploymentStatusEnum",
     "EmploymentTypeEnum",
     "EmploymentsListRequestExpand",
     "EmploymentsListRequestOrderBy",
     "EmploymentsListRequestRemoteFields",
     "EmploymentsListRequestShowEnumOrigins",
     "EmploymentsRetrieveRequestExpand",
@@ -216,26 +231,28 @@
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "EthnicityEnum",
     "FlsaStatusEnum",
     "GenderEnum",
     "Group",
+    "GroupType",
     "GroupTypeEnum",
     "Issue",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
     "LinkedAccountSelectiveSyncConfiguration",
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "Location",
+    "LocationLocationType",
     "LocationTypeEnum",
     "MaritalStatusEnum",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
     "OperatorSchema",
@@ -257,43 +274,48 @@
     "PaginatedTimeOffBalanceList",
     "PaginatedTimeOffList",
     "PayCurrencyEnum",
     "PayFrequencyEnum",
     "PayGroup",
     "PayPeriodEnum",
     "PayrollRun",
+    "PayrollRunRunType",
     "PayrollRunsListRequestRemoteFields",
     "PayrollRunsListRequestRunType",
     "PayrollRunsListRequestShowEnumOrigins",
     "PayrollRunsRetrieveRequestRemoteFields",
     "PayrollRunsRetrieveRequestShowEnumOrigins",
     "PolicyTypeEnum",
     "ReasonEnum",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
+    "RemoteResponseResponseType",
     "RequestFormatEnum",
     "RequestTypeEnum",
     "ResponseTypeEnum",
     "RunStateEnum",
     "RunTypeEnum",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tax",
     "Team",
     "TimeOff",
     "TimeOffBalance",
+    "TimeOffBalancePolicyType",
     "TimeOffBalancesListRequestPolicyType",
     "TimeOffListRequestExpand",
     "TimeOffListRequestRemoteFields",
     "TimeOffListRequestRequestType",
     "TimeOffListRequestShowEnumOrigins",
     "TimeOffListRequestStatus",
     "TimeOffRequest",
+    "TimeOffRequestRequestType",
+    "TimeOffRequestType",
     "TimeOffResponse",
     "TimeOffRetrieveRequestExpand",
     "TimeOffRetrieveRequestRemoteFields",
     "TimeOffRetrieveRequestShowEnumOrigins",
     "TimeOffStatusEnum",
     "UnitsEnum",
     "ValidationProblemSource",
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/__init__.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/account_details/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/account_token/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/available_actions/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/bank_info/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/benefits/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/companies/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/delete_account/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/employees/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/employments/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/force_resync/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/generate_key/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/groups/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/issues/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/link_token/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/linked_accounts/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/locations/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/passthrough/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/pay_groups/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/payroll_runs/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/regenerate_key/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/selective_sync/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/sync_status/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/teams/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/time_off/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/time_off_balances/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/resources/webhook_receivers/client.py` & `fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/__init__.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 from .account_details_and_actions_integration import AccountDetailsAndActionsIntegration
 from .account_details_and_actions_status_enum import AccountDetailsAndActionsStatusEnum
 from .account_integration import AccountIntegration
 from .account_token import AccountToken
 from .account_type_enum import AccountTypeEnum
 from .available_actions import AvailableActions
 from .bank_info import BankInfo
+from .bank_info_account_type import BankInfoAccountType
 from .bank_info_list_request_account_type import BankInfoListRequestAccountType
 from .bank_info_list_request_order_by import BankInfoListRequestOrderBy
 from .benefit import Benefit
 from .categories_enum import CategoriesEnum
 from .category_enum import CategoryEnum
 from .common_model_scopes_body_request import CommonModelScopesBodyRequest
 from .company import Company
 from .condition_schema import ConditionSchema
+from .condition_schema_condition_type import ConditionSchemaConditionType
 from .condition_type_enum import ConditionTypeEnum
 from .country_enum import CountryEnum
 from .debug_mode_log import DebugModeLog
 from .debug_model_log_summary import DebugModelLogSummary
 from .deduction import Deduction
 from .earning import Earning
+from .earning_type import EarningType
 from .earning_type_enum import EarningTypeEnum
 from .employee import Employee
 from .employee_payroll_run import EmployeePayrollRun
 from .employee_payroll_runs_list_request_expand import EmployeePayrollRunsListRequestExpand
 from .employee_payroll_runs_retrieve_request_expand import EmployeePayrollRunsRetrieveRequestExpand
 from .employee_request import EmployeeRequest
 from .employee_response import EmployeeResponse
@@ -34,14 +37,15 @@
 from .employees_list_request_expand import EmployeesListRequestExpand
 from .employees_list_request_remote_fields import EmployeesListRequestRemoteFields
 from .employees_list_request_show_enum_origins import EmployeesListRequestShowEnumOrigins
 from .employees_retrieve_request_expand import EmployeesRetrieveRequestExpand
 from .employees_retrieve_request_remote_fields import EmployeesRetrieveRequestRemoteFields
 from .employees_retrieve_request_show_enum_origins import EmployeesRetrieveRequestShowEnumOrigins
 from .employment import Employment
+from .employment_employment_type import EmploymentEmploymentType
 from .employment_status_enum import EmploymentStatusEnum
 from .employment_type_enum import EmploymentTypeEnum
 from .employments_list_request_expand import EmploymentsListRequestExpand
 from .employments_list_request_order_by import EmploymentsListRequestOrderBy
 from .employments_list_request_remote_fields import EmploymentsListRequestRemoteFields
 from .employments_list_request_show_enum_origins import EmploymentsListRequestShowEnumOrigins
 from .employments_retrieve_request_expand import EmploymentsRetrieveRequestExpand
@@ -50,26 +54,28 @@
 from .enabled_actions_enum import EnabledActionsEnum
 from .encoding_enum import EncodingEnum
 from .error_validation_problem import ErrorValidationProblem
 from .ethnicity_enum import EthnicityEnum
 from .flsa_status_enum import FlsaStatusEnum
 from .gender_enum import GenderEnum
 from .group import Group
+from .group_type import GroupType
 from .group_type_enum import GroupTypeEnum
 from .issue import Issue
 from .issue_status_enum import IssueStatusEnum
 from .issues_list_request_status import IssuesListRequestStatus
 from .link_token import LinkToken
 from .linked_account_condition import LinkedAccountCondition
 from .linked_account_condition_request import LinkedAccountConditionRequest
 from .linked_account_selective_sync_configuration import LinkedAccountSelectiveSyncConfiguration
 from .linked_account_selective_sync_configuration_request import LinkedAccountSelectiveSyncConfigurationRequest
 from .linked_account_status import LinkedAccountStatus
 from .linked_accounts_list_request_category import LinkedAccountsListRequestCategory
 from .location import Location
+from .location_location_type import LocationLocationType
 from .location_type_enum import LocationTypeEnum
 from .marital_status_enum import MaritalStatusEnum
 from .meta_response import MetaResponse
 from .method_enum import MethodEnum
 from .model_operation import ModelOperation
 from .multipart_form_field_request import MultipartFormFieldRequest
 from .operator_schema import OperatorSchema
@@ -91,43 +97,48 @@
 from .paginated_time_off_balance_list import PaginatedTimeOffBalanceList
 from .paginated_time_off_list import PaginatedTimeOffList
 from .pay_currency_enum import PayCurrencyEnum
 from .pay_frequency_enum import PayFrequencyEnum
 from .pay_group import PayGroup
 from .pay_period_enum import PayPeriodEnum
 from .payroll_run import PayrollRun
+from .payroll_run_run_type import PayrollRunRunType
 from .payroll_runs_list_request_remote_fields import PayrollRunsListRequestRemoteFields
 from .payroll_runs_list_request_run_type import PayrollRunsListRequestRunType
 from .payroll_runs_list_request_show_enum_origins import PayrollRunsListRequestShowEnumOrigins
 from .payroll_runs_retrieve_request_remote_fields import PayrollRunsRetrieveRequestRemoteFields
 from .payroll_runs_retrieve_request_show_enum_origins import PayrollRunsRetrieveRequestShowEnumOrigins
 from .policy_type_enum import PolicyTypeEnum
 from .reason_enum import ReasonEnum
 from .remote_data import RemoteData
 from .remote_key import RemoteKey
 from .remote_response import RemoteResponse
+from .remote_response_response_type import RemoteResponseResponseType
 from .request_format_enum import RequestFormatEnum
 from .request_type_enum import RequestTypeEnum
 from .response_type_enum import ResponseTypeEnum
 from .run_state_enum import RunStateEnum
 from .run_type_enum import RunTypeEnum
 from .selective_sync_configurations_usage_enum import SelectiveSyncConfigurationsUsageEnum
 from .sync_status import SyncStatus
 from .sync_status_status_enum import SyncStatusStatusEnum
 from .tax import Tax
 from .team import Team
 from .time_off import TimeOff
 from .time_off_balance import TimeOffBalance
+from .time_off_balance_policy_type import TimeOffBalancePolicyType
 from .time_off_balances_list_request_policy_type import TimeOffBalancesListRequestPolicyType
 from .time_off_list_request_expand import TimeOffListRequestExpand
 from .time_off_list_request_remote_fields import TimeOffListRequestRemoteFields
 from .time_off_list_request_request_type import TimeOffListRequestRequestType
 from .time_off_list_request_show_enum_origins import TimeOffListRequestShowEnumOrigins
 from .time_off_list_request_status import TimeOffListRequestStatus
 from .time_off_request import TimeOffRequest
+from .time_off_request_request_type import TimeOffRequestRequestType
+from .time_off_request_type import TimeOffRequestType
 from .time_off_response import TimeOffResponse
 from .time_off_retrieve_request_expand import TimeOffRetrieveRequestExpand
 from .time_off_retrieve_request_remote_fields import TimeOffRetrieveRequestRemoteFields
 from .time_off_retrieve_request_show_enum_origins import TimeOffRetrieveRequestShowEnumOrigins
 from .time_off_status_enum import TimeOffStatusEnum
 from .units_enum import UnitsEnum
 from .validation_problem_source import ValidationProblemSource
@@ -140,28 +151,31 @@
     "AccountDetailsAndActionsIntegration",
     "AccountDetailsAndActionsStatusEnum",
     "AccountIntegration",
     "AccountToken",
     "AccountTypeEnum",
     "AvailableActions",
     "BankInfo",
+    "BankInfoAccountType",
     "BankInfoListRequestAccountType",
     "BankInfoListRequestOrderBy",
     "Benefit",
     "CategoriesEnum",
     "CategoryEnum",
     "CommonModelScopesBodyRequest",
     "Company",
     "ConditionSchema",
+    "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "CountryEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Deduction",
     "Earning",
+    "EarningType",
     "EarningTypeEnum",
     "Employee",
     "EmployeePayrollRun",
     "EmployeePayrollRunsListRequestExpand",
     "EmployeePayrollRunsRetrieveRequestExpand",
     "EmployeeRequest",
     "EmployeeResponse",
@@ -169,14 +183,15 @@
     "EmployeesListRequestExpand",
     "EmployeesListRequestRemoteFields",
     "EmployeesListRequestShowEnumOrigins",
     "EmployeesRetrieveRequestExpand",
     "EmployeesRetrieveRequestRemoteFields",
     "EmployeesRetrieveRequestShowEnumOrigins",
     "Employment",
+    "EmploymentEmploymentType",
     "EmploymentStatusEnum",
     "EmploymentTypeEnum",
     "EmploymentsListRequestExpand",
     "EmploymentsListRequestOrderBy",
     "EmploymentsListRequestRemoteFields",
     "EmploymentsListRequestShowEnumOrigins",
     "EmploymentsRetrieveRequestExpand",
@@ -185,26 +200,28 @@
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "EthnicityEnum",
     "FlsaStatusEnum",
     "GenderEnum",
     "Group",
+    "GroupType",
     "GroupTypeEnum",
     "Issue",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
     "LinkedAccountSelectiveSyncConfiguration",
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "Location",
+    "LocationLocationType",
     "LocationTypeEnum",
     "MaritalStatusEnum",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
     "OperatorSchema",
@@ -226,43 +243,48 @@
     "PaginatedTimeOffBalanceList",
     "PaginatedTimeOffList",
     "PayCurrencyEnum",
     "PayFrequencyEnum",
     "PayGroup",
     "PayPeriodEnum",
     "PayrollRun",
+    "PayrollRunRunType",
     "PayrollRunsListRequestRemoteFields",
     "PayrollRunsListRequestRunType",
     "PayrollRunsListRequestShowEnumOrigins",
     "PayrollRunsRetrieveRequestRemoteFields",
     "PayrollRunsRetrieveRequestShowEnumOrigins",
     "PolicyTypeEnum",
     "ReasonEnum",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
+    "RemoteResponseResponseType",
     "RequestFormatEnum",
     "RequestTypeEnum",
     "ResponseTypeEnum",
     "RunStateEnum",
     "RunTypeEnum",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tax",
     "Team",
     "TimeOff",
     "TimeOffBalance",
+    "TimeOffBalancePolicyType",
     "TimeOffBalancesListRequestPolicyType",
     "TimeOffListRequestExpand",
     "TimeOffListRequestRemoteFields",
     "TimeOffListRequestRequestType",
     "TimeOffListRequestShowEnumOrigins",
     "TimeOffListRequestStatus",
     "TimeOffRequest",
+    "TimeOffRequestRequestType",
+    "TimeOffRequestType",
     "TimeOffResponse",
     "TimeOffRetrieveRequestExpand",
     "TimeOffRetrieveRequestRemoteFields",
     "TimeOffRetrieveRequestShowEnumOrigins",
     "TimeOffStatusEnum",
     "UnitsEnum",
     "ValidationProblemSource",
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_details.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_integration.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_token.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/account_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/available_actions.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/bank_info.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .account_type_enum import AccountTypeEnum
+from .bank_info_account_type import BankInfoAccountType
 from .remote_data import RemoteData
 
 
 class BankInfo(pydantic.BaseModel):
     """
     # The BankInfo Object
     ### Description
@@ -22,15 +22,15 @@
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     employee: typing.Optional[str] = pydantic.Field(description="The employee with this bank account.")
     account_number: typing.Optional[str] = pydantic.Field(description="The account number.")
     routing_number: typing.Optional[str] = pydantic.Field(description="The routing number.")
     bank_name: typing.Optional[str] = pydantic.Field(description="The bank name.")
-    account_type: typing.Optional[AccountTypeEnum] = pydantic.Field(
+    account_type: typing.Optional[BankInfoAccountType] = pydantic.Field(
         description=("The bank account type\n" "\n" "* `SAVINGS` - SAVINGS\n" "* `CHECKING` - CHECKING\n")
     )
     remote_created_at: typing.Optional[str] = pydantic.Field(
         description="When the matching bank object was created in the third party system."
     )
     remote_was_deleted: typing.Optional[bool] = pydantic.Field(
         description="Indicates whether or not this object has been deleted by third party webhooks."
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/benefit.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/categories_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/category_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/company.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/condition_schema.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .condition_type_enum import ConditionTypeEnum
+from .condition_schema_condition_type import ConditionSchemaConditionType
 from .operator_schema import OperatorSchema
 
 
 class ConditionSchema(pydantic.BaseModel):
     id: str = pydantic.Field(
         description="The ID of the condition schema. This ID is used when updating selective syncs for a linked account."
     )
@@ -22,15 +22,15 @@
     )
     field_name: typing.Optional[str] = pydantic.Field(
         description='The name of the field on the common model that this condition corresponds to, if they conceptually match. e.g. "location_type".'
     )
     is_unique: typing.Optional[bool] = pydantic.Field(
         description="Whether this condition can only be applied once. If false, the condition can be AND'd together multiple times."
     )
-    condition_type: ConditionTypeEnum = pydantic.Field(
+    condition_type: ConditionSchemaConditionType = pydantic.Field(
         description=(
             "The type of value(s) that can be set for this condition.\n"
             "\n"
             "* `BOOLEAN` - BOOLEAN\n"
             "* `DATE` - DATE\n"
             "* `DATE_TIME` - DATE_TIME\n"
             "* `INTEGER` - INTEGER\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/condition_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/country_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/debug_mode_log.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/debug_model_log_summary.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/deduction.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/earning.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/group.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .earning_type_enum import EarningTypeEnum
+from .group_type import GroupType
 from .remote_data import RemoteData
 
 
-class Earning(pydantic.BaseModel):
+class Group(pydantic.BaseModel):
     """
-    # The Earning Object
+    # The Group Object
     ### Description
-    The `Earning` object is used to represent an array of different compensations that an employee receives within specific wage categories.
+    The `Group` object is used to represent any subset of employees, such as `PayGroup` or `Team`. Employees can be in multiple Groups.
 
     ### Usage Example
-    Fetch from the `LIST Earnings` endpoint and filter by `ID` to show all earnings.
+    Fetch from the `LIST Employee` endpoint and expand groups to view an employee's groups.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
-    employee_payroll_run: typing.Optional[str]
-    amount: typing.Optional[float] = pydantic.Field(description="The amount earned.")
-    type: typing.Optional[EarningTypeEnum] = pydantic.Field(
+    parent_group: typing.Optional[str] = pydantic.Field(description="The parent group for this group.")
+    name: typing.Optional[str] = pydantic.Field(description="The group name.")
+    type: typing.Optional[GroupType] = pydantic.Field(
         description=(
-            "The type of earning.\n"
+            "The group type\n"
             "\n"
-            "* `SALARY` - SALARY\n"
-            "* `REIMBURSEMENT` - REIMBURSEMENT\n"
-            "* `OVERTIME` - OVERTIME\n"
-            "* `BONUS` - BONUS\n"
+            "* `TEAM` - TEAM\n"
+            "* `DEPARTMENT` - DEPARTMENT\n"
+            "* `COST_CENTER` - COST_CENTER\n"
+            "* `BUSINESS_UNIT` - BUSINESS_UNIT\n"
+            "* `GROUP` - GROUP\n"
         )
     )
     remote_was_deleted: typing.Optional[bool] = pydantic.Field(
         description="Indicates whether or not this object has been deleted by third party webhooks."
     )
     modified_at: typing.Optional[str] = pydantic.Field(
         description="This is the datetime that this object was last updated by Merge"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/earning_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_run.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employee_response.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employment.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employment.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .employment_type_enum import EmploymentTypeEnum
+from .employment_employment_type import EmploymentEmploymentType
 from .flsa_status_enum import FlsaStatusEnum
 from .pay_currency_enum import PayCurrencyEnum
 from .pay_frequency_enum import PayFrequencyEnum
 from .pay_period_enum import PayPeriodEnum
 from .remote_data import RemoteData
 
 
@@ -381,15 +381,15 @@
             "* `EXEMPT` - EXEMPT\n"
             "* `SALARIED_NONEXEMPT` - SALARIED_NONEXEMPT\n"
             "* `NONEXEMPT` - NONEXEMPT\n"
             "* `OWNER` - OWNER\n"
         )
     )
     effective_date: typing.Optional[str] = pydantic.Field(description="The position's effective date.")
-    employment_type: typing.Optional[EmploymentTypeEnum] = pydantic.Field(
+    employment_type: typing.Optional[EmploymentEmploymentType] = pydantic.Field(
         description=(
             "The position's type of employment.\n"
             "\n"
             "* `FULL_TIME` - FULL_TIME\n"
             "* `PART_TIME` - PART_TIME\n"
             "* `INTERN` - INTERN\n"
             "* `CONTRACTOR` - CONTRACTOR\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employment_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employment_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_order_by.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/enabled_actions_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/encoding_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/error_validation_problem.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/ethnicity_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/flsa_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/gender_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/group.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/tax.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,42 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .group_type_enum import GroupTypeEnum
 from .remote_data import RemoteData
 
 
-class Group(pydantic.BaseModel):
+class Tax(pydantic.BaseModel):
     """
-    # The Group Object
+    # The Tax Object
     ### Description
-    The `Group` object is used to represent any subset of employees, such as `PayGroup` or `Team`. Employees can be in multiple Groups.
+    The `Tax` object is used to represent an array of the tax deductions for a given employee's payroll run.
 
     ### Usage Example
-    Fetch from the `LIST Employee` endpoint and expand groups to view an employee's groups.
+    Fetch from the `LIST Taxes` endpoint and filter by `ID` to show all taxes.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
-    parent_group: typing.Optional[str] = pydantic.Field(description="The parent group for this group.")
-    name: typing.Optional[str] = pydantic.Field(description="The group name.")
-    type: typing.Optional[GroupTypeEnum] = pydantic.Field(
-        description=(
-            "The group type\n"
-            "\n"
-            "* `TEAM` - TEAM\n"
-            "* `DEPARTMENT` - DEPARTMENT\n"
-            "* `COST_CENTER` - COST_CENTER\n"
-            "* `BUSINESS_UNIT` - BUSINESS_UNIT\n"
-            "* `GROUP` - GROUP\n"
-        )
+    employee_payroll_run: typing.Optional[str]
+    name: typing.Optional[str] = pydantic.Field(description="The tax's name.")
+    amount: typing.Optional[float] = pydantic.Field(description="The tax amount.")
+    employer_tax: typing.Optional[bool] = pydantic.Field(
+        description="Whether or not the employer is responsible for paying the tax."
     )
     remote_was_deleted: typing.Optional[bool] = pydantic.Field(
         description="Indicates whether or not this object has been deleted by third party webhooks."
     )
     modified_at: typing.Optional[str] = pydantic.Field(
         description="This is the datetime that this object was last updated by Merge"
     )
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/group_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/issue.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/issue_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/link_token.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_condition.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_condition_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_account_status.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/location.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .country_enum import CountryEnum
-from .location_type_enum import LocationTypeEnum
+from .location_location_type import LocationLocationType
 from .remote_data import RemoteData
 
 
 class Location(pydantic.BaseModel):
     """
     # The Location Object
     ### Description
@@ -283,15 +283,15 @@
             "* `WF` - Wallis and Futuna\n"
             "* `EH` - Western Sahara\n"
             "* `YE` - Yemen\n"
             "* `ZM` - Zambia\n"
             "* `ZW` - Zimbabwe\n"
         )
     )
-    location_type: typing.Optional[LocationTypeEnum] = pydantic.Field(
+    location_type: typing.Optional[LocationLocationType] = pydantic.Field(
         description=("The location's type. Can be either WORK or HOME\n" "\n" "* `HOME` - HOME\n" "* `WORK` - WORK\n")
     )
     remote_was_deleted: typing.Optional[bool] = pydantic.Field(
         description="Indicates whether or not this object has been deleted by third party webhooks."
     )
     modified_at: typing.Optional[str] = pydantic.Field(
         description="This is the datetime that this object was last updated by Merge"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/marital_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/meta_response.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/method_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/model_operation.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/sync_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .selective_sync_configurations_usage_enum import SelectiveSyncConfigurationsUsageEnum
+from .sync_status_status_enum import SyncStatusStatusEnum
 
 
-class ModelOperation(pydantic.BaseModel):
+class SyncStatus(pydantic.BaseModel):
     """
-    # The ModelOperation Object
+    # The SyncStatus Object
     ### Description
-    The `ModelOperation` object is used to represent the operations that are currently supported for a given model.
+    The `SyncStatus` object is used to represent the syncing state of an account
 
     ### Usage Example
-    View what operations are supported for the `Candidate` endpoint.
+    View the `SyncStatus` for an account to see how recently its models were synced.
     """
 
     model_name: str
-    available_operations: typing.List[str]
-    required_post_parameters: typing.List[str]
-    supported_fields: typing.List[str]
+    model_id: str
+    last_sync_start: typing.Optional[str]
+    next_sync_start: typing.Optional[str]
+    status: SyncStatusStatusEnum
+    is_initial_sync: bool
+    selective_sync_configurations_usage: typing.Optional[SelectiveSyncConfigurationsUsageEnum]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/multipart_form_field_request.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/operator_schema.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_bank_info_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_benefit_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_company_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employee_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_employment_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_group_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_issue_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_location_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_pay_group_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_sync_status_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_team_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/paginated_time_off_list.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/pay_currency_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/pay_frequency_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/pay_group.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/pay_period_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_run.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .payroll_run_run_type import PayrollRunRunType
 from .remote_data import RemoteData
 from .run_state_enum import RunStateEnum
-from .run_type_enum import RunTypeEnum
 
 
 class PayrollRun(pydantic.BaseModel):
     """
     # The PayrollRun Object
     ### Description
     The `PayrollRun` object is used to represent a group of pay statements for a specific pay schedule.
@@ -30,15 +30,15 @@
             "* `PAID` - PAID\n"
             "* `DRAFT` - DRAFT\n"
             "* `APPROVED` - APPROVED\n"
             "* `FAILED` - FAILED\n"
             "* `CLOSED` - CLOSED\n"
         )
     )
-    run_type: typing.Optional[RunTypeEnum] = pydantic.Field(
+    run_type: typing.Optional[PayrollRunRunType] = pydantic.Field(
         description=(
             "The type of the payroll run\n"
             "\n"
             "* `REGULAR` - REGULAR\n"
             "* `OFF_CYCLE` - OFF_CYCLE\n"
             "* `CORRECTION` - CORRECTION\n"
             "* `TERMINATION` - TERMINATION\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/policy_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/reason_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/remote_data.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/remote_key.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/remote_response.py` & `fern_merge-0.0.28/src/merge/resources/ats/types/remote_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .response_type_enum import ResponseTypeEnum
+from .remote_response_response_type import RemoteResponseResponseType
 
 
 class RemoteResponse(pydantic.BaseModel):
     """
     # The RemoteResponse Object
     ### Description
     The `RemoteResponse` object is used to represent information returned from a third-party endpoint.
@@ -20,15 +20,15 @@
     """
 
     method: str
     path: str
     status: int
     response: typing.Any
     response_headers: typing.Optional[typing.Dict[str, typing.Any]]
-    response_type: typing.Optional[ResponseTypeEnum]
+    response_type: typing.Optional[RemoteResponseResponseType]
     headers: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/request_format_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/request_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/response_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/run_state_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/run_type_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/sync_status_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/tax.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,45 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .remote_data import RemoteData
+from .time_off_balance_policy_type import TimeOffBalancePolicyType
 
 
-class Tax(pydantic.BaseModel):
+class TimeOffBalance(pydantic.BaseModel):
     """
-    # The Tax Object
+    # The TimeOffBalance Object
     ### Description
-    The `Tax` object is used to represent an array of the tax deductions for a given employee's payroll run.
+    The `TimeOffBalance` object is used to represent current balances for an employee's Time Off plan.
 
     ### Usage Example
-    Fetch from the `LIST Taxes` endpoint and filter by `ID` to show all taxes.
+    Fetch from the `LIST TimeOffBalances` endpoint and filter by `ID` to show all time off balances.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
-    employee_payroll_run: typing.Optional[str]
-    name: typing.Optional[str] = pydantic.Field(description="The tax's name.")
-    amount: typing.Optional[float] = pydantic.Field(description="The tax amount.")
-    employer_tax: typing.Optional[bool] = pydantic.Field(
-        description="Whether or not the employer is responsible for paying the tax."
+    employee: typing.Optional[str] = pydantic.Field(description="The employee the balance belongs to.")
+    balance: typing.Optional[float] = pydantic.Field(
+        description="The current remaining PTO balance, always measured in terms of hours."
+    )
+    used: typing.Optional[float] = pydantic.Field(description="The amount of PTO used in terms of hours.")
+    policy_type: typing.Optional[TimeOffBalancePolicyType] = pydantic.Field(
+        description=(
+            "The policy type of this time off balance.\n"
+            "\n"
+            "* `VACATION` - VACATION\n"
+            "* `SICK` - SICK\n"
+            "* `PERSONAL` - PERSONAL\n"
+            "* `JURY_DUTY` - JURY_DUTY\n"
+            "* `VOLUNTEER` - VOLUNTEER\n"
+            "* `BEREAVEMENT` - BEREAVEMENT\n"
+        )
     )
     remote_was_deleted: typing.Optional[bool] = pydantic.Field(
         description="Indicates whether or not this object has been deleted by third party webhooks."
     )
     modified_at: typing.Optional[str] = pydantic.Field(
         description="This is the datetime that this object was last updated by Merge"
     )
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/team.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .remote_data import RemoteData
-from .request_type_enum import RequestTypeEnum
+from .time_off_request_type import TimeOffRequestType
 from .time_off_status_enum import TimeOffStatusEnum
 from .units_enum import UnitsEnum
 
 
 class TimeOff(pydantic.BaseModel):
     """
     # The TimeOff Object
@@ -47,15 +47,15 @@
             "* `HOURS` - HOURS\n"
             "* `DAYS` - DAYS\n"
         )
     )
     amount: typing.Optional[float] = pydantic.Field(
         description="The time off quantity measured by the prescribed “units”."
     )
-    request_type: typing.Optional[RequestTypeEnum] = pydantic.Field(
+    request_type: typing.Optional[TimeOffRequestType] = pydantic.Field(
         description=(
             "The type of time off request.\n"
             "\n"
             "* `VACATION` - VACATION\n"
             "* `SICK` - SICK\n"
             "* `PERSONAL` - PERSONAL\n"
             "* `JURY_DUTY` - JURY_DUTY\n"
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_balance.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,55 +2,76 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .policy_type_enum import PolicyTypeEnum
-from .remote_data import RemoteData
+from .time_off_request_request_type import TimeOffRequestRequestType
+from .time_off_status_enum import TimeOffStatusEnum
+from .units_enum import UnitsEnum
 
 
-class TimeOffBalance(pydantic.BaseModel):
+class TimeOffRequest(pydantic.BaseModel):
     """
-    # The TimeOffBalance Object
+    # The TimeOff Object
     ### Description
-    The `TimeOffBalance` object is used to represent current balances for an employee's Time Off plan.
+    The `TimeOff` object is used to represent all employees' Time Off entries.
 
     ### Usage Example
-    Fetch from the `LIST TimeOffBalances` endpoint and filter by `ID` to show all time off balances.
+    Fetch from the `LIST TimeOffs` endpoint and filter by `ID` to show all time off requests.
     """
 
-    id: typing.Optional[str]
-    remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
-    employee: typing.Optional[str] = pydantic.Field(description="The employee the balance belongs to.")
-    balance: typing.Optional[float] = pydantic.Field(
-        description="The current remaining PTO balance, always measured in terms of hours."
+    employee: typing.Optional[str] = pydantic.Field(description="The employee requesting time off.")
+    approver: typing.Optional[str] = pydantic.Field(
+        description="The Merge ID of the employee with the ability to approve the time off request."
     )
-    used: typing.Optional[float] = pydantic.Field(description="The amount of PTO used in terms of hours.")
-    policy_type: typing.Optional[PolicyTypeEnum] = pydantic.Field(
+    status: typing.Optional[TimeOffStatusEnum] = pydantic.Field(
         description=(
-            "The policy type of this time off balance.\n"
+            "The status of this time off request.\n"
+            "\n"
+            "* `REQUESTED` - REQUESTED\n"
+            "* `APPROVED` - APPROVED\n"
+            "* `DECLINED` - DECLINED\n"
+            "* `CANCELLED` - CANCELLED\n"
+            "* `DELETED` - DELETED\n"
+        )
+    )
+    employee_note: typing.Optional[str] = pydantic.Field(description="The employee note for this time off request.")
+    units: typing.Optional[UnitsEnum] = pydantic.Field(
+        description=(
+            "The measurement that the third-party integration uses to count time requested.\n"
+            "\n"
+            "* `HOURS` - HOURS\n"
+            "* `DAYS` - DAYS\n"
+        )
+    )
+    amount: typing.Optional[float] = pydantic.Field(
+        description="The time off quantity measured by the prescribed “units”."
+    )
+    request_type: typing.Optional[TimeOffRequestRequestType] = pydantic.Field(
+        description=(
+            "The type of time off request.\n"
             "\n"
             "* `VACATION` - VACATION\n"
             "* `SICK` - SICK\n"
             "* `PERSONAL` - PERSONAL\n"
             "* `JURY_DUTY` - JURY_DUTY\n"
             "* `VOLUNTEER` - VOLUNTEER\n"
             "* `BEREAVEMENT` - BEREAVEMENT\n"
         )
     )
-    remote_was_deleted: typing.Optional[bool] = pydantic.Field(
-        description="Indicates whether or not this object has been deleted by third party webhooks."
+    start_time: typing.Optional[str] = pydantic.Field(
+        description="The day and time of the start of the time requested off."
     )
-    modified_at: typing.Optional[str] = pydantic.Field(
-        description="This is the datetime that this object was last updated by Merge"
+    end_time: typing.Optional[str] = pydantic.Field(
+        description="The day and time of the end of the time requested off."
     )
-    field_mappings: typing.Optional[typing.Dict[str, typing.Any]]
-    remote_data: typing.Optional[typing.List[RemoteData]]
+    integration_params: typing.Optional[typing.Dict[str, typing.Any]]
+    linked_account_params: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_list_request_status.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_response.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/time_off_status_enum.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/validation_problem_source.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/warning_validation_problem.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/src/merge/resources/hris/types/webhook_receiver.py` & `fern_merge-0.0.28/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.27/PKG-INFO` & `fern_merge-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-merge
-Version: 0.0.27
+Version: 0.0.28
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

