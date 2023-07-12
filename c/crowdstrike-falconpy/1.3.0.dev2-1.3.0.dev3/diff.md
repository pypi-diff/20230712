# Comparing `tmp/crowdstrike-falconpy-1.3.0.dev2.tar.gz` & `tmp/crowdstrike-falconpy-1.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-1.3.0.dev2.tar", last modified: Tue Jul 11 08:19:37 2023, max compression
+gzip compressed data, was "crowdstrike-falconpy-1.3.0.dev3.tar", last modified: Wed Jul 12 02:22:09 2023, max compression
```

## Comparing `crowdstrike-falconpy-1.3.0.dev2.tar` & `crowdstrike-falconpy-1.3.0.dev3.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.210667 crowdstrike-falconpy-1.3.0.dev2/
--rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/AUTHORS.md
--rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/LICENSE
--rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-11 08:19:37.210346 crowdstrike-falconpy-1.3.0.dev2/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/README.md
--rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-11 08:19:37.210788 crowdstrike-falconpy-1.3.0.dev2/setup.cfg
--rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/setup.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.110289 crowdstrike-falconpy-1.3.0.dev2/src/
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.116383 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/
--rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-11 08:19:37.000000 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)     7615 2023-07-11 08:19:37.000000 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/SOURCES.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-11 08:19:37.000000 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/dependency_links.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-11 08:19:37.000000 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/requires.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        9 2023-07-11 08:19:37.000000 crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/top_level.txt
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.146481 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/
--rw-r--r--   0 jhiller    (501) staff       (20)    12031 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.149265 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/
--rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_behavior.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_connection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_payloads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_validator.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.152023 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/
--rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_base_falcon_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_bearer_token.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20032 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_falcon_interface.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_interface_config.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_uber_interface.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.152492 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_constant/
--rw-r--r--   0 jhiller    (501) staff       (20)     2915 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_constant/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.173920 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/
--rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_prevention_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.180650 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/
--rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.182035 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/
--rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_container_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_token_fail_reason.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.183369 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/
--rw-r--r--   0 jhiller    (501) staff       (20)     2606 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5837 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/_exceptions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/_warnings.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.184078 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_log/
--rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_log/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_log/_facility.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.203359 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/
--rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_device_control_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_falconx.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_firewall.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_generic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_response_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_sensor_update_policy.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.207148 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/
--rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/__base_resource.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_base_dictionary.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_errors.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_expanded_result.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_headers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_resources.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_response_component.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15675 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_result.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.208357 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/
--rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/_base_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11024 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/_service_class.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-11 08:19:37.209804 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/
--rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_functions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2120 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_version.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/api_complete.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/debug.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-11 08:19:35.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-11 08:19:36.000000 crowdstrike-falconpy-1.3.0.dev2/src/falconpy/zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.283789 crowdstrike-falconpy-1.3.0.dev3/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/AUTHORS.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/LICENSE
+-rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-12 02:22:09.283476 crowdstrike-falconpy-1.3.0.dev3/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/README.md
+-rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-12 02:22:09.283907 crowdstrike-falconpy-1.3.0.dev3/setup.cfg
+-rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/setup.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.151796 crowdstrike-falconpy-1.3.0.dev3/src/
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.169059 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/
+-rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-12 02:22:09.000000 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)     7615 2023-07-12 02:22:09.000000 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-12 02:22:09.000000 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-12 02:22:09.000000 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/requires.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        9 2023-07-12 02:22:09.000000 crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/top_level.txt
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.209835 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/
+-rw-r--r--   0 jhiller    (501) staff       (20)    12031 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.213167 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_behavior.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_connection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_payloads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_validator.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.216045 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_base_falcon_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_bearer_token.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20032 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_falcon_interface.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_interface_config.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_uber_interface.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.216621 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_constant/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2915 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_constant/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.242850 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/
+-rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_prevention_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.251037 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.252505 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_container_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_token_fail_reason.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.253656 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2606 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5837 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/_exceptions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/_warnings.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.254428 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_log/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_log/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_log/_facility.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.275459 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/
+-rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_device_control_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_falconx.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_firewall.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_generic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_response_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_sensor_update_policy.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.279722 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/__base_resource.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_base_dictionary.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_errors.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_expanded_result.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_headers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_resources.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_response_component.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16223 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_result.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.280873 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/_base_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11024 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/_service_class.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-12 02:22:09.282879 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_functions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2120 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_version.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/api_complete.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/debug.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-12 02:22:07.000000 crowdstrike-falconpy-1.3.0.dev3/src/falconpy/zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-1.3.0.dev2/AUTHORS.md` & `crowdstrike-falconpy-1.3.0.dev3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/LICENSE` & `crowdstrike-falconpy-1.3.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/PKG-INFO` & `crowdstrike-falconpy-1.3.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.3.0.dev2
+Version: 1.3.0.dev3
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.3.0.dev2/README.md` & `crowdstrike-falconpy-1.3.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/setup.py` & `crowdstrike-falconpy-1.3.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/PKG-INFO` & `crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.3.0.dev2
+Version: 1.3.0.dev3
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/crowdstrike_falconpy.egg-info/SOURCES.txt` & `crowdstrike-falconpy-1.3.0.dev3/src/crowdstrike_falconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_behavior.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_behavior.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_connection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_connection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_meta.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_payloads.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_payloads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_api_request/_request_validator.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_api_request/_request_validator.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_base_falcon_auth.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_base_falcon_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_bearer_token.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_bearer_token.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_falcon_interface.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_falcon_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_interface_config.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_interface_config.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_auth_object/_uber_interface.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_auth_object/_uber_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_constant/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_constant/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_alerts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_detects.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_discover.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_event_streams.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_fdr.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_filevantage.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_host_group.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_hosts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_incidents.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_intel.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_iocs.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_malquery.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_message_center.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_mssp.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_oauth2.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_ods.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_quarantine.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_recon.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_report_executions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_response_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_update_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_user_management.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_fdr.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_base_url.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_container_base_url.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_enum/_token_fail_reason.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_enum/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/_exceptions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/_exceptions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_error/_warnings.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_error/_warnings.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_log/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_log/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_log/_facility.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_log/_facility.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_alerts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_container.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_detects.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_device_control_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_device_control_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_falconx.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_firewall.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_firewall.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_generic.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_generic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_host_group.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_incidents.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ioa.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_malquery.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_message_center.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_mssp.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_ods.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_prevention_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_recon.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_reports.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_response_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_response_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_payload/_sensor_update_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_payload/_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/__base_resource.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/__base_resource.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_base_dictionary.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_base_dictionary.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_errors.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_errors.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_expanded_result.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_expanded_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_headers.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_headers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_meta.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_resources.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_resources.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_response_component.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_response_component.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_result/_result.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_result/_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,29 @@
             elif body.get("access_token", None):
                 # Authentication response
                 self.raw = RawBody(body)
                 self.meta = Meta()
                 self.resources = Resources()
                 self.errors = Errors()
             else:
-                # Standard response
+                # Standard responses and RTR
                 self.meta = Meta(body.get("meta", {}))
-                self.resources = Resources(body.get("resources", []))
                 self.errors = Errors(body.get("errors", []))
+                # RTR Batch responses
+                if body.get("batch_id", {}):
+                    # Batch session init
+                    self.raw = RawBody(body)
+                    self.resources = Resources(body.get("resources", []))
+                elif body.get("combined", {}):
+                    # Batch session results have to be handled as RawBody
+                    # due to the combined response format.
+                    self.raw = RawBody(body)
+                else:
+                    # Standard API responses
+                    self.resources = Resources(body.get("resources", []))
 
     # Iteration handlers
     def __iter__(self):
         """Return this object for iteration handling."""
         _returned = self
         if self.data:
             _returned = self.resources.data.__iter__()
```

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/_base_service_class.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/_base_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_service_class/_service_class.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_service_class/_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/__init__.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_auth.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_functions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_functions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_util/_uber.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_util/_uber.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/_version.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-_VERSION = '1.3.0.dev2'
+_VERSION = '1.3.0.dev3'
 _MAINTAINER = 'Joshua Hiller'
 _AUTHOR = 'CrowdStrike'
 _AUTHOR_EMAIL = 'falconpy@crowdstrike.com'
 _CREDITS = 'CrowdStrike'
 _DESCRIPTION = "The CrowdStrike Falcon SDK for Python 3"
 _TITLE = "crowdstrike-falconpy"
 _PROJECT_URL = "https://github.com/CrowdStrike/falconpy"
```

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/alerts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/api_complete.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/debug.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/detects.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/device_control_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/discover.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/event_streams.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falcon_container.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/falconx_sandbox.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/fdr.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/filevantage.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/firewall_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/host_group.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/hosts.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/incidents.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/intel.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ioa_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ioc.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/iocs.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/kubernetes_protection.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/malquery.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/message_center.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ml_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/mobile_enrollment.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/mssp.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/oauth2.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/ods.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/overwatch_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/prevention_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/quarantine.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/quick_scan.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/recon.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/report_executions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/response_policies.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_download.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_update_policy.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/tailored_intelligence.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/user_management.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev2/src/falconpy/zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev3/src/falconpy/zero_trust_assessment.py`

 * *Files identical despite different names*

