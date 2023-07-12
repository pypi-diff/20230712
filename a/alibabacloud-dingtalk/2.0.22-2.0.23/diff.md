# Comparing `tmp/alibabacloud_dingtalk-2.0.22.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.22.tar", last modified: Wed Jul  5 01:54:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.23.tar", last modified: Wed Jul 12 02:54:07 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.22.tar` & `alibabacloud_dingtalk-2.0.23.tar`

### file list

```diff
@@ -1,377 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/
--rw-r--r--   0 root         (0) root         (0)    20077 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202090 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   575598 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19674 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27526 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    71831 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5464 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12452 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/
+-rw-r--r--   0 root         (0) root         (0)    20142 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202090 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   575598 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.22/ChangeLog.md` & `alibabacloud_dingtalk-2.0.23/ChangeLog.md`

 * *Files identical despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-05 Version: 2.0.22
+- Update AddOfficialAccountFollower.
+
 2023-06-16 Version: 2.0.21
 - Update AddOfficialAccountFollower.
 
 2023-06-13 Version: 2.0.20
 - Update AddOfficialAccountFollower.
 
 2023-06-09 Version: 2.0.19
```

### Comparing `alibabacloud_dingtalk-2.0.22/LICENSE` & `alibabacloud_dingtalk-2.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/PKG-INFO` & `alibabacloud_dingtalk-2.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.22
+Version: 2.0.23
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.22/README-CN.md` & `alibabacloud_dingtalk-2.0.23/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/README.md` & `alibabacloud_dingtalk-2.0.23/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -631,14 +631,124 @@
         self,
         request: dingtalkcard__1__0_models.RegisterCallbackRequest,
     ) -> dingtalkcard__1__0_models.RegisterCallbackResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcard__1__0_models.RegisterCallbackHeaders()
         return await self.register_callback_with_options_async(request, headers, runtime)
 
+    def streaming_update_with_options(
+        self,
+        request: dingtalkcard__1__0_models.StreamingUpdateRequest,
+        headers: dingtalkcard__1__0_models.StreamingUpdateHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcard__1__0_models.StreamingUpdateResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.guid):
+            body['guid'] = request.guid
+        if not UtilClient.is_unset(request.is_error):
+            body['isError'] = request.is_error
+        if not UtilClient.is_unset(request.is_finalize):
+            body['isFinalize'] = request.is_finalize
+        if not UtilClient.is_unset(request.is_full):
+            body['isFull'] = request.is_full
+        if not UtilClient.is_unset(request.key):
+            body['key'] = request.key
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='StreamingUpdate',
+            version='card_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/card/streaming',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcard__1__0_models.StreamingUpdateResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def streaming_update_with_options_async(
+        self,
+        request: dingtalkcard__1__0_models.StreamingUpdateRequest,
+        headers: dingtalkcard__1__0_models.StreamingUpdateHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcard__1__0_models.StreamingUpdateResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.guid):
+            body['guid'] = request.guid
+        if not UtilClient.is_unset(request.is_error):
+            body['isError'] = request.is_error
+        if not UtilClient.is_unset(request.is_finalize):
+            body['isFinalize'] = request.is_finalize
+        if not UtilClient.is_unset(request.is_full):
+            body['isFull'] = request.is_full
+        if not UtilClient.is_unset(request.key):
+            body['key'] = request.key
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='StreamingUpdate',
+            version='card_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/card/streaming',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcard__1__0_models.StreamingUpdateResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def streaming_update(
+        self,
+        request: dingtalkcard__1__0_models.StreamingUpdateRequest,
+    ) -> dingtalkcard__1__0_models.StreamingUpdateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcard__1__0_models.StreamingUpdateHeaders()
+        return self.streaming_update_with_options(request, headers, runtime)
+
+    async def streaming_update_async(
+        self,
+        request: dingtalkcard__1__0_models.StreamingUpdateRequest,
+    ) -> dingtalkcard__1__0_models.StreamingUpdateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcard__1__0_models.StreamingUpdateHeaders()
+        return await self.streaming_update_with_options_async(request, headers, runtime)
+
     def update_card_with_options(
         self,
         request: dingtalkcard__1__0_models.UpdateCardRequest,
         headers: dingtalkcard__1__0_models.UpdateCardHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcard__1__0_models.UpdateCardResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2752,14 +2752,187 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RegisterCallbackResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class StreamingUpdateHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class StreamingUpdateRequest(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        guid: str = None,
+        is_error: bool = None,
+        is_finalize: bool = None,
+        is_full: bool = None,
+        key: str = None,
+        out_track_id: str = None,
+    ):
+        self.content = content
+        self.guid = guid
+        self.is_error = is_error
+        self.is_finalize = is_finalize
+        self.is_full = is_full
+        self.key = key
+        self.out_track_id = out_track_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['content'] = self.content
+        if self.guid is not None:
+            result['guid'] = self.guid
+        if self.is_error is not None:
+            result['isError'] = self.is_error
+        if self.is_finalize is not None:
+            result['isFinalize'] = self.is_finalize
+        if self.is_full is not None:
+            result['isFull'] = self.is_full
+        if self.key is not None:
+            result['key'] = self.key
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('guid') is not None:
+            self.guid = m.get('guid')
+        if m.get('isError') is not None:
+            self.is_error = m.get('isError')
+        if m.get('isFinalize') is not None:
+            self.is_finalize = m.get('isFinalize')
+        if m.get('isFull') is not None:
+            self.is_full = m.get('isFull')
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        return self
+
+
+class StreamingUpdateResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class StreamingUpdateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: StreamingUpdateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = StreamingUpdateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateCardHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -315,14 +315,104 @@
         self,
         request: dingtalkcontract__1__0_models.EsignSyncEventRequest,
     ) -> dingtalkcontract__1__0_models.EsignSyncEventResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcontract__1__0_models.EsignSyncEventHeaders()
         return await self.esign_sync_event_with_options_async(request, headers, runtime)
 
+    def query_advanced_contract_version_with_options(
+        self,
+        request: dingtalkcontract__1__0_models.QueryAdvancedContractVersionRequest,
+        headers: dingtalkcontract__1__0_models.QueryAdvancedContractVersionHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.extension):
+            body['extension'] = request.extension
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryAdvancedContractVersion',
+            version='contract_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contract/versions/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_advanced_contract_version_with_options_async(
+        self,
+        request: dingtalkcontract__1__0_models.QueryAdvancedContractVersionRequest,
+        headers: dingtalkcontract__1__0_models.QueryAdvancedContractVersionHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.extension):
+            body['extension'] = request.extension
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryAdvancedContractVersion',
+            version='contract_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contract/versions/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_advanced_contract_version(
+        self,
+        request: dingtalkcontract__1__0_models.QueryAdvancedContractVersionRequest,
+    ) -> dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontract__1__0_models.QueryAdvancedContractVersionHeaders()
+        return self.query_advanced_contract_version_with_options(request, headers, runtime)
+
+    async def query_advanced_contract_version_async(
+        self,
+        request: dingtalkcontract__1__0_models.QueryAdvancedContractVersionRequest,
+    ) -> dingtalkcontract__1__0_models.QueryAdvancedContractVersionResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontract__1__0_models.QueryAdvancedContractVersionHeaders()
+        return await self.query_advanced_contract_version_with_options_async(request, headers, runtime)
+
     def send_contract_card_with_options(
         self,
         request: dingtalkcontract__1__0_models.SendContractCardRequest,
         headers: dingtalkcontract__1__0_models.SendContractCardHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcontract__1__0_models.SendContractCardResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class EsignQueryGrantInfoHeaders(TeaModel):
+class AddDeviceVideoConferenceMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,151 +33,174 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class EsignQueryGrantInfoRequest(TeaModel):
+class AddDeviceVideoConferenceMembersRequest(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        extension: Dict[str, str] = None,
-        union_id: str = None,
+        user_ids: List[str] = None,
     ):
-        self.corp_id = corp_id
-        self.extension = extension
-        self.union_id = union_id
+        self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
         return self
 
 
-class EsignQueryGrantInfoResponseBodyResult(TeaModel):
+class AddDeviceVideoConferenceMembersResponse(TeaModel):
     def __init__(
         self,
-        legal_person: str = None,
-        mobile_phone_number: str = None,
-        org_name: str = None,
-        state_code: str = None,
-        unified_social_credit: str = None,
-        user_name: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class CreateDeviceVideoConferenceHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.legal_person = legal_person
-        self.mobile_phone_number = mobile_phone_number
-        self.org_name = org_name
-        self.state_code = state_code
-        self.unified_social_credit = unified_social_credit
-        self.user_name = user_name
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.legal_person is not None:
-            result['legalPerson'] = self.legal_person
-        if self.mobile_phone_number is not None:
-            result['mobilePhoneNumber'] = self.mobile_phone_number
-        if self.org_name is not None:
-            result['orgName'] = self.org_name
-        if self.state_code is not None:
-            result['stateCode'] = self.state_code
-        if self.unified_social_credit is not None:
-            result['unifiedSocialCredit'] = self.unified_social_credit
-        if self.user_name is not None:
-            result['userName'] = self.user_name
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('legalPerson') is not None:
-            self.legal_person = m.get('legalPerson')
-        if m.get('mobilePhoneNumber') is not None:
-            self.mobile_phone_number = m.get('mobilePhoneNumber')
-        if m.get('orgName') is not None:
-            self.org_name = m.get('orgName')
-        if m.get('stateCode') is not None:
-            self.state_code = m.get('stateCode')
-        if m.get('unifiedSocialCredit') is not None:
-            self.unified_social_credit = m.get('unifiedSocialCredit')
-        if m.get('userName') is not None:
-            self.user_name = m.get('userName')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class EsignQueryGrantInfoResponseBody(TeaModel):
+class CreateDeviceVideoConferenceRequest(TeaModel):
     def __init__(
         self,
-        result: EsignQueryGrantInfoResponseBodyResult = None,
-        success: bool = None,
+        user_ids: List[str] = None,
     ):
-        self.result = result
-        self.success = success
+        self.user_ids = user_ids
 
     def validate(self):
-        if self.result:
-            self.result.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.result is not None:
-            result['result'] = self.result.to_map()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('result') is not None:
-            temp_model = EsignQueryGrantInfoResponseBodyResult()
-            self.result = temp_model.from_map(m['result'])
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
         return self
 
 
-class EsignQueryGrantInfoResponse(TeaModel):
+class CreateDeviceVideoConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        conference_id: str = None,
+    ):
+        self.code = code
+        self.conference_id = conference_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['code'] = self.code
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        return self
+
+
+class CreateDeviceVideoConferenceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: EsignQueryGrantInfoResponseBody = None,
+        body: CreateDeviceVideoConferenceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -203,20 +226,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = EsignQueryGrantInfoResponseBody()
+            temp_model = CreateDeviceVideoConferenceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class EsignQueryIdentityByTicketHeaders(TeaModel):
+class ExtractFacialFeatureHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -241,121 +264,80 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class EsignQueryIdentityByTicketRequest(TeaModel):
+class ExtractFacialFeatureRequest(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        extension: Dict[str, str] = None,
-        ticket: str = None,
+        media_id: str = None,
+        userid: str = None,
     ):
-        self.corp_id = corp_id
-        self.extension = extension
-        self.ticket = ticket
+        self.media_id = media_id
+        self.userid = userid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.ticket is not None:
-            result['ticket'] = self.ticket
+        if self.media_id is not None:
+            result['mediaId'] = self.media_id
+        if self.userid is not None:
+            result['userid'] = self.userid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('ticket') is not None:
-            self.ticket = m.get('ticket')
+        if m.get('mediaId') is not None:
+            self.media_id = m.get('mediaId')
+        if m.get('userid') is not None:
+            self.userid = m.get('userid')
         return self
 
 
-class EsignQueryIdentityByTicketResponseBodyResult(TeaModel):
+class ExtractFacialFeatureResponseBody(TeaModel):
     def __init__(
         self,
-        union_id: str = None,
-    ):
-        self.union_id = union_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
-        return self
-
-
-class EsignQueryIdentityByTicketResponseBody(TeaModel):
-    def __init__(
-        self,
-        result: EsignQueryIdentityByTicketResponseBodyResult = None,
-        success: bool = None,
+        result: bool = None,
     ):
         self.result = result
-        self.success = success
 
     def validate(self):
-        if self.result:
-            self.result.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.result is not None:
-            result['result'] = self.result.to_map()
-        if self.success is not None:
-            result['success'] = self.success
+            result['result'] = self.result
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('result') is not None:
-            temp_model = EsignQueryIdentityByTicketResponseBodyResult()
-            self.result = temp_model.from_map(m['result'])
-        if m.get('success') is not None:
-            self.success = m.get('success')
+            self.result = m.get('result')
         return self
 
 
-class EsignQueryIdentityByTicketResponse(TeaModel):
+class ExtractFacialFeatureResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: EsignQueryIdentityByTicketResponseBody = None,
+        body: ExtractFacialFeatureResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -381,20 +363,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = EsignQueryIdentityByTicketResponseBody()
+            temp_model = ExtractFacialFeatureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class EsignSyncEventHeaders(TeaModel):
+class KickDeviceVideoConferenceMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -419,172 +401,247 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class EsignSyncEventRequest(TeaModel):
+class KickDeviceVideoConferenceMembersRequest(TeaModel):
+    def __init__(
+        self,
+        user_ids: List[str] = None,
+    ):
+        self.user_ids = user_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
+        return self
+
+
+class KickDeviceVideoConferenceMembersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class MachineManagerUpdateHeaders(TeaModel):
     def __init__(
         self,
-        action: str = None,
-        corp_id: str = None,
-        esign_data: str = None,
-        extension: Dict[str, str] = None,
-        union_id: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.action = action
-        self.corp_id = corp_id
-        self.esign_data = esign_data
-        self.extension = extension
-        self.union_id = union_id
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.esign_data is not None:
-            result['esignData'] = self.esign_data
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('esignData') is not None:
-            self.esign_data = m.get('esignData')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class EsignSyncEventResponseBodyResult(TeaModel):
+class MachineManagerUpdateRequestAtmManagerRightMap(TeaModel):
     def __init__(
         self,
-        message: str = None,
+        attendance_person_manage: bool = None,
+        bluetooth_punch_manage: bool = None,
+        device_reset: bool = None,
+        device_settings: bool = None,
+        face_punch_manage: bool = None,
+        finger_punch_manage: bool = None,
     ):
-        self.message = message
+        self.attendance_person_manage = attendance_person_manage
+        self.bluetooth_punch_manage = bluetooth_punch_manage
+        self.device_reset = device_reset
+        self.device_settings = device_settings
+        self.face_punch_manage = face_punch_manage
+        self.finger_punch_manage = finger_punch_manage
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.message is not None:
-            result['message'] = self.message
+        if self.attendance_person_manage is not None:
+            result['attendancePersonManage'] = self.attendance_person_manage
+        if self.bluetooth_punch_manage is not None:
+            result['bluetoothPunchManage'] = self.bluetooth_punch_manage
+        if self.device_reset is not None:
+            result['deviceReset'] = self.device_reset
+        if self.device_settings is not None:
+            result['deviceSettings'] = self.device_settings
+        if self.face_punch_manage is not None:
+            result['facePunchManage'] = self.face_punch_manage
+        if self.finger_punch_manage is not None:
+            result['fingerPunchManage'] = self.finger_punch_manage
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('message') is not None:
-            self.message = m.get('message')
+        if m.get('attendancePersonManage') is not None:
+            self.attendance_person_manage = m.get('attendancePersonManage')
+        if m.get('bluetoothPunchManage') is not None:
+            self.bluetooth_punch_manage = m.get('bluetoothPunchManage')
+        if m.get('deviceReset') is not None:
+            self.device_reset = m.get('deviceReset')
+        if m.get('deviceSettings') is not None:
+            self.device_settings = m.get('deviceSettings')
+        if m.get('facePunchManage') is not None:
+            self.face_punch_manage = m.get('facePunchManage')
+        if m.get('fingerPunchManage') is not None:
+            self.finger_punch_manage = m.get('fingerPunchManage')
         return self
 
 
-class EsignSyncEventResponseBody(TeaModel):
+class MachineManagerUpdateRequest(TeaModel):
     def __init__(
         self,
-        result: EsignSyncEventResponseBodyResult = None,
-        success: bool = None,
+        atm_manager_right_map: MachineManagerUpdateRequestAtmManagerRightMap = None,
+        device_id: int = None,
+        scope_dept_ids: List[int] = None,
+        user_id: str = None,
     ):
-        self.result = result
-        self.success = success
+        self.atm_manager_right_map = atm_manager_right_map
+        self.device_id = device_id
+        self.scope_dept_ids = scope_dept_ids
+        self.user_id = user_id
 
     def validate(self):
-        if self.result:
-            self.result.validate()
+        if self.atm_manager_right_map:
+            self.atm_manager_right_map.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.result is not None:
-            result['result'] = self.result.to_map()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.atm_manager_right_map is not None:
+            result['atmManagerRightMap'] = self.atm_manager_right_map.to_map()
+        if self.device_id is not None:
+            result['deviceId'] = self.device_id
+        if self.scope_dept_ids is not None:
+            result['scopeDeptIds'] = self.scope_dept_ids
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('result') is not None:
-            temp_model = EsignSyncEventResponseBodyResult()
-            self.result = temp_model.from_map(m['result'])
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('atmManagerRightMap') is not None:
+            temp_model = MachineManagerUpdateRequestAtmManagerRightMap()
+            self.atm_manager_right_map = temp_model.from_map(m['atmManagerRightMap'])
+        if m.get('deviceId') is not None:
+            self.device_id = m.get('deviceId')
+        if m.get('scopeDeptIds') is not None:
+            self.scope_dept_ids = m.get('scopeDeptIds')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class EsignSyncEventResponse(TeaModel):
+class MachineManagerUpdateResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: EsignSyncEventResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
-        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = EsignSyncEventResponseBody()
-            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class SendContractCardHeaders(TeaModel):
+class MachineUsersUpdateHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -609,259 +666,177 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class SendContractCardRequestContractInfo(TeaModel):
+class MachineUsersUpdateRequest(TeaModel):
     def __init__(
         self,
-        contract_code: str = None,
-        contract_name: str = None,
-        create_time: int = None,
-        sign_user_name: str = None,
+        add_dept_ids: List[int] = None,
+        add_user_ids: List[str] = None,
+        del_dept_ids: List[int] = None,
+        del_user_ids: List[str] = None,
+        dev_ids: List[int] = None,
+        device_ids: List[str] = None,
     ):
-        self.contract_code = contract_code
-        self.contract_name = contract_name
-        self.create_time = create_time
-        self.sign_user_name = sign_user_name
+        self.add_dept_ids = add_dept_ids
+        self.add_user_ids = add_user_ids
+        self.del_dept_ids = del_dept_ids
+        self.del_user_ids = del_user_ids
+        self.dev_ids = dev_ids
+        self.device_ids = device_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contract_code is not None:
-            result['contractCode'] = self.contract_code
-        if self.contract_name is not None:
-            result['contractName'] = self.contract_name
-        if self.create_time is not None:
-            result['createTime'] = self.create_time
-        if self.sign_user_name is not None:
-            result['signUserName'] = self.sign_user_name
+        if self.add_dept_ids is not None:
+            result['addDeptIds'] = self.add_dept_ids
+        if self.add_user_ids is not None:
+            result['addUserIds'] = self.add_user_ids
+        if self.del_dept_ids is not None:
+            result['delDeptIds'] = self.del_dept_ids
+        if self.del_user_ids is not None:
+            result['delUserIds'] = self.del_user_ids
+        if self.dev_ids is not None:
+            result['devIds'] = self.dev_ids
+        if self.device_ids is not None:
+            result['deviceIds'] = self.device_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('contractCode') is not None:
-            self.contract_code = m.get('contractCode')
-        if m.get('contractName') is not None:
-            self.contract_name = m.get('contractName')
-        if m.get('createTime') is not None:
-            self.create_time = m.get('createTime')
-        if m.get('signUserName') is not None:
-            self.sign_user_name = m.get('signUserName')
+        if m.get('addDeptIds') is not None:
+            self.add_dept_ids = m.get('addDeptIds')
+        if m.get('addUserIds') is not None:
+            self.add_user_ids = m.get('addUserIds')
+        if m.get('delDeptIds') is not None:
+            self.del_dept_ids = m.get('delDeptIds')
+        if m.get('delUserIds') is not None:
+            self.del_user_ids = m.get('delUserIds')
+        if m.get('devIds') is not None:
+            self.dev_ids = m.get('devIds')
+        if m.get('deviceIds') is not None:
+            self.device_ids = m.get('deviceIds')
         return self
 
 
-class SendContractCardRequestReceivers(TeaModel):
+class MachineUsersUpdateResponse(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        user_id: str = None,
-        user_type: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
     ):
-        self.corp_id = corp_id
-        self.user_id = user_id
-        self.user_type = user_type
+        self.headers = headers
+        self.status_code = status_code
 
     def validate(self):
-        pass
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.user_type is not None:
-            result['userType'] = self.user_type
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('userType') is not None:
-            self.user_type = m.get('userType')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         return self
 
 
-class SendContractCardRequestSender(TeaModel):
+class QueryDeviceVideoConferenceBookHeaders(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        user_id: str = None,
-        user_type: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.corp_id = corp_id
-        self.user_id = user_id
-        self.user_type = user_type
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.user_type is not None:
-            result['userType'] = self.user_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('userType') is not None:
-            self.user_type = m.get('userType')
-        return self
-
-
-class SendContractCardRequest(TeaModel):
-    def __init__(
-        self,
-        card_type: str = None,
-        contract_info: SendContractCardRequestContractInfo = None,
-        corp_id: str = None,
-        extension: Dict[str, str] = None,
-        process_instance_id: str = None,
-        receive_groups: List[str] = None,
-        receivers: List[SendContractCardRequestReceivers] = None,
-        sender: SendContractCardRequestSender = None,
-        sync_single_chat: bool = None,
-    ):
-        self.card_type = card_type
-        self.contract_info = contract_info
-        self.corp_id = corp_id
-        self.extension = extension
-        self.process_instance_id = process_instance_id
-        self.receive_groups = receive_groups
-        self.receivers = receivers
-        self.sender = sender
-        self.sync_single_chat = sync_single_chat
-
-    def validate(self):
-        if self.contract_info:
-            self.contract_info.validate()
-        if self.receivers:
-            for k in self.receivers:
-                if k:
-                    k.validate()
-        if self.sender:
-            self.sender.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.card_type is not None:
-            result['cardType'] = self.card_type
-        if self.contract_info is not None:
-            result['contractInfo'] = self.contract_info.to_map()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.process_instance_id is not None:
-            result['processInstanceId'] = self.process_instance_id
-        if self.receive_groups is not None:
-            result['receiveGroups'] = self.receive_groups
-        result['receivers'] = []
-        if self.receivers is not None:
-            for k in self.receivers:
-                result['receivers'].append(k.to_map() if k else None)
-        if self.sender is not None:
-            result['sender'] = self.sender.to_map()
-        if self.sync_single_chat is not None:
-            result['syncSingleChat'] = self.sync_single_chat
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cardType') is not None:
-            self.card_type = m.get('cardType')
-        if m.get('contractInfo') is not None:
-            temp_model = SendContractCardRequestContractInfo()
-            self.contract_info = temp_model.from_map(m['contractInfo'])
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('processInstanceId') is not None:
-            self.process_instance_id = m.get('processInstanceId')
-        if m.get('receiveGroups') is not None:
-            self.receive_groups = m.get('receiveGroups')
-        self.receivers = []
-        if m.get('receivers') is not None:
-            for k in m.get('receivers'):
-                temp_model = SendContractCardRequestReceivers()
-                self.receivers.append(temp_model.from_map(k))
-        if m.get('sender') is not None:
-            temp_model = SendContractCardRequestSender()
-            self.sender = temp_model.from_map(m['sender'])
-        if m.get('syncSingleChat') is not None:
-            self.sync_single_chat = m.get('syncSingleChat')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class SendContractCardResponseBody(TeaModel):
+class QueryDeviceVideoConferenceBookResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        code: str = None,
+        conference_id: str = None,
     ):
-        self.success = success
+        self.code = code
+        self.conference_id = conference_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
         return self
 
 
-class SendContractCardResponse(TeaModel):
+class QueryDeviceVideoConferenceBookResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: SendContractCardResponseBody = None,
+        body: QueryDeviceVideoConferenceBookResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -887,12 +862,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = SendContractCardResponseBody()
+            temp_model = QueryDeviceVideoConferenceBookResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -721,14 +721,72 @@
         return self.diot_system_mark_test_with_options(headers, runtime)
 
     async def diot_system_mark_test_async(self) -> dingtalkdiot__1__0_models.DiotSystemMarkTestResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.diot_system_mark_test_with_options_async(headers, runtime)
 
+    def diot__market__manager_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.DiotMarketManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='Diot_Market_Manager',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.DiotMarketManagerResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def diot__market__manager_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.DiotMarketManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='Diot_Market_Manager',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.DiotMarketManagerResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def diot__market__manager(self) -> dingtalkdiot__1__0_models.DiotMarketManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.diot__market__manager_with_options(headers, runtime)
+
+    async def diot__market__manager_async(self) -> dingtalkdiot__1__0_models.DiotMarketManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.diot__market__manager_with_options_async(headers, runtime)
+
     def push_event_with_options(
         self,
         request: dingtalkdiot__1__0_models.PushEventRequest,
         headers: dingtalkdiot__1__0_models.PushEventHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdiot__1__0_models.PushEventResponse:
         UtilClient.validate_model(request)
@@ -1181,14 +1239,72 @@
         self,
         request: dingtalkdiot__1__0_models.RegisterDeviceRequest,
     ) -> dingtalkdiot__1__0_models.RegisterDeviceResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkdiot__1__0_models.RegisterDeviceHeaders()
         return await self.register_device_with_options_async(request, headers, runtime)
 
+    def upgrade_device_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.UpgradeDeviceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='UpgradeDevice',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/upgrade/device',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.UpgradeDeviceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def upgrade_device_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.UpgradeDeviceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='UpgradeDevice',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/upgrade/device',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.UpgradeDeviceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def upgrade_device(self) -> dingtalkdiot__1__0_models.UpgradeDeviceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upgrade_device_with_options(headers, runtime)
+
+    async def upgrade_device_async(self) -> dingtalkdiot__1__0_models.UpgradeDeviceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upgrade_device_with_options_async(headers, runtime)
+
     def workbench_transform_info_with_options(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse:
         req = open_api_models.OpenApiRequest(
             headers=headers
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1304,14 +1304,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DiotSystemMarkTestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DiotMarketManagerResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class DiotMarketManagerResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DiotMarketManagerResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DiotMarketManagerResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PushEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -2274,14 +2345,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RegisterDeviceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpgradeDeviceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class UpgradeDeviceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpgradeDeviceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpgradeDeviceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class WorkbenchTransformInfoResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
         self.request_id = request_id
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,108 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def push_live_activity_with_options(
+        self,
+        request: dingtalklive_activities__1__0_models.PushLiveActivityRequest,
+        headers: dingtalklive_activities__1__0_models.PushLiveActivityHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalklive_activities__1__0_models.PushLiveActivityResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.activity_event_data):
+            body['activityEventData'] = request.activity_event_data
+        if not UtilClient.is_unset(request.activity_event_option):
+            body['activityEventOption'] = request.activity_event_option
+        if not UtilClient.is_unset(request.activity_id):
+            body['activityId'] = request.activity_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PushLiveActivity',
+            version='liveActivities_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/liveActivities/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalklive_activities__1__0_models.PushLiveActivityResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def push_live_activity_with_options_async(
+        self,
+        request: dingtalklive_activities__1__0_models.PushLiveActivityRequest,
+        headers: dingtalklive_activities__1__0_models.PushLiveActivityHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalklive_activities__1__0_models.PushLiveActivityResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.activity_event_data):
+            body['activityEventData'] = request.activity_event_data
+        if not UtilClient.is_unset(request.activity_event_option):
+            body['activityEventOption'] = request.activity_event_option
+        if not UtilClient.is_unset(request.activity_id):
+            body['activityId'] = request.activity_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PushLiveActivity',
+            version='liveActivities_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/liveActivities/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalklive_activities__1__0_models.PushLiveActivityResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def push_live_activity(
+        self,
+        request: dingtalklive_activities__1__0_models.PushLiveActivityRequest,
+    ) -> dingtalklive_activities__1__0_models.PushLiveActivityResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalklive_activities__1__0_models.PushLiveActivityHeaders()
+        return self.push_live_activity_with_options(request, headers, runtime)
+
+    async def push_live_activity_async(
+        self,
+        request: dingtalklive_activities__1__0_models.PushLiveActivityRequest,
+    ) -> dingtalklive_activities__1__0_models.PushLiveActivityResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalklive_activities__1__0_models.PushLiveActivityHeaders()
+        return await self.push_live_activity_with_options_async(request, headers, runtime)
+
     def send_live_activity_with_options(
         self,
         request: dingtalklive_activities__1__0_models.SendLiveActivityRequest,
         headers: dingtalklive_activities__1__0_models.SendLiveActivityHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalklive_activities__1__0_models.SendLiveActivityResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, Any
+from typing import Dict, List
 
 
-class SendLiveActivityHeaders(TeaModel):
+class QueryGoodsListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,169 +33,204 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class SendLiveActivityRequestActivityEventData(TeaModel):
+class QueryGoodsListRequest(TeaModel):
     def __init__(
         self,
-        i_18n_content_state: Any = None,
-        template_id: str = None,
+        end_time_in_mills: int = None,
+        max_results: int = None,
+        next_token: int = None,
+        start_time_in_mills: int = None,
     ):
-        self.i_18n_content_state = i_18n_content_state
-        self.template_id = template_id
+        self.end_time_in_mills = end_time_in_mills
+        self.max_results = max_results
+        self.next_token = next_token
+        self.start_time_in_mills = start_time_in_mills
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.i_18n_content_state is not None:
-            result['i18nContentState'] = self.i_18n_content_state
-        if self.template_id is not None:
-            result['templateId'] = self.template_id
+        if self.end_time_in_mills is not None:
+            result['endTimeInMills'] = self.end_time_in_mills
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.start_time_in_mills is not None:
+            result['startTimeInMills'] = self.start_time_in_mills
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('i18nContentState') is not None:
-            self.i_18n_content_state = m.get('i18nContentState')
-        if m.get('templateId') is not None:
-            self.template_id = m.get('templateId')
+        if m.get('endTimeInMills') is not None:
+            self.end_time_in_mills = m.get('endTimeInMills')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('startTimeInMills') is not None:
+            self.start_time_in_mills = m.get('startTimeInMills')
         return self
 
 
-class SendLiveActivityRequestActivityEventOption(TeaModel):
+class QueryGoodsListResponseBodyResultList(TeaModel):
     def __init__(
         self,
-        dismissal_date: int = None,
-        push_type: str = None,
-        send_date: int = None,
-        stale_date: int = None,
+        goods_name: str = None,
+        goods_no: str = None,
+        instance_id: str = None,
+        product_specs: str = None,
+        unit: str = None,
     ):
-        self.dismissal_date = dismissal_date
-        self.push_type = push_type
-        self.send_date = send_date
-        self.stale_date = stale_date
+        self.goods_name = goods_name
+        self.goods_no = goods_no
+        self.instance_id = instance_id
+        self.product_specs = product_specs
+        self.unit = unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.dismissal_date is not None:
-            result['dismissalDate'] = self.dismissal_date
-        if self.push_type is not None:
-            result['pushType'] = self.push_type
-        if self.send_date is not None:
-            result['sendDate'] = self.send_date
-        if self.stale_date is not None:
-            result['staleDate'] = self.stale_date
+        if self.goods_name is not None:
+            result['goodsName'] = self.goods_name
+        if self.goods_no is not None:
+            result['goodsNo'] = self.goods_no
+        if self.instance_id is not None:
+            result['instanceId'] = self.instance_id
+        if self.product_specs is not None:
+            result['productSpecs'] = self.product_specs
+        if self.unit is not None:
+            result['unit'] = self.unit
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('dismissalDate') is not None:
-            self.dismissal_date = m.get('dismissalDate')
-        if m.get('pushType') is not None:
-            self.push_type = m.get('pushType')
-        if m.get('sendDate') is not None:
-            self.send_date = m.get('sendDate')
-        if m.get('staleDate') is not None:
-            self.stale_date = m.get('staleDate')
+        if m.get('goodsName') is not None:
+            self.goods_name = m.get('goodsName')
+        if m.get('goodsNo') is not None:
+            self.goods_no = m.get('goodsNo')
+        if m.get('instanceId') is not None:
+            self.instance_id = m.get('instanceId')
+        if m.get('productSpecs') is not None:
+            self.product_specs = m.get('productSpecs')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
         return self
 
 
-class SendLiveActivityRequest(TeaModel):
+class QueryGoodsListResponseBodyResult(TeaModel):
     def __init__(
         self,
-        activity_event_data: SendLiveActivityRequestActivityEventData = None,
-        activity_event_option: SendLiveActivityRequestActivityEventOption = None,
-        activity_id: str = None,
+        has_more: bool = None,
+        list: List[QueryGoodsListResponseBodyResultList] = None,
+        max_results: int = None,
+        next_token: str = None,
     ):
-        self.activity_event_data = activity_event_data
-        self.activity_event_option = activity_event_option
-        self.activity_id = activity_id
+        self.has_more = has_more
+        self.list = list
+        self.max_results = max_results
+        self.next_token = next_token
 
     def validate(self):
-        if self.activity_event_data:
-            self.activity_event_data.validate()
-        if self.activity_event_option:
-            self.activity_event_option.validate()
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.activity_event_data is not None:
-            result['activityEventData'] = self.activity_event_data.to_map()
-        if self.activity_event_option is not None:
-            result['activityEventOption'] = self.activity_event_option.to_map()
-        if self.activity_id is not None:
-            result['activityId'] = self.activity_id
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('activityEventData') is not None:
-            temp_model = SendLiveActivityRequestActivityEventData()
-            self.activity_event_data = temp_model.from_map(m['activityEventData'])
-        if m.get('activityEventOption') is not None:
-            temp_model = SendLiveActivityRequestActivityEventOption()
-            self.activity_event_option = temp_model.from_map(m['activityEventOption'])
-        if m.get('activityId') is not None:
-            self.activity_id = m.get('activityId')
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryGoodsListResponseBodyResultList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class SendLiveActivityResponseBody(TeaModel):
+class QueryGoodsListResponseBody(TeaModel):
     def __init__(
         self,
-        result: str = None,
+        result: QueryGoodsListResponseBodyResult = None,
+        success: bool = None,
     ):
         self.result = result
+        self.success = success
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.result is not None:
-            result['result'] = self.result
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('result') is not None:
-            self.result = m.get('result')
+            temp_model = QueryGoodsListResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class SendLiveActivityResponse(TeaModel):
+class QueryGoodsListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: SendLiveActivityResponseBody = None,
+        body: QueryGoodsListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -221,12 +256,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = SendLiveActivityResponseBody()
+            temp_model = QueryGoodsListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class AddDeviceVideoConferenceMembersHeaders(TeaModel):
+class AddRecentUserAppListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,76 +33,160 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class AddDeviceVideoConferenceMembersRequest(TeaModel):
+class AddRecentUserAppListRequestUsedAppDetailList(TeaModel):
     def __init__(
         self,
-        user_ids: List[str] = None,
+        agent_id: str = None,
     ):
-        self.user_ids = user_ids
+        self.agent_id = agent_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_ids is not None:
-            result['userIds'] = self.user_ids
+        if self.agent_id is not None:
+            result['agentId'] = self.agent_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userIds') is not None:
-            self.user_ids = m.get('userIds')
+        if m.get('agentId') is not None:
+            self.agent_id = m.get('agentId')
         return self
 
 
-class AddDeviceVideoConferenceMembersResponse(TeaModel):
+class AddRecentUserAppListRequest(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        used_app_detail_list: List[AddRecentUserAppListRequestUsedAppDetailList] = None,
+        user_id: str = None,
+    ):
+        self.corp_id = corp_id
+        self.used_app_detail_list = used_app_detail_list
+        self.user_id = user_id
+
+    def validate(self):
+        if self.used_app_detail_list:
+            for k in self.used_app_detail_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        result['usedAppDetailList'] = []
+        if self.used_app_detail_list is not None:
+            for k in self.used_app_detail_list:
+                result['usedAppDetailList'].append(k.to_map() if k else None)
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        self.used_app_detail_list = []
+        if m.get('usedAppDetailList') is not None:
+            for k in m.get('usedAppDetailList'):
+                temp_model = AddRecentUserAppListRequestUsedAppDetailList()
+                self.used_app_detail_list.append(temp_model.from_map(k))
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class AddRecentUserAppListResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class AddRecentUserAppListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
+        body: AddRecentUserAppListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
+        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AddRecentUserAppListResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateDeviceVideoConferenceHeaders(TeaModel):
+class GetDingPortalDetailHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -127,80 +211,124 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateDeviceVideoConferenceRequest(TeaModel):
+class GetDingPortalDetailResponseBodyPages(TeaModel):
     def __init__(
         self,
-        user_ids: List[str] = None,
-    ):
-        self.user_ids = user_ids
+        all_visible: bool = None,
+        dept_ids: List[int] = None,
+        page_name: str = None,
+        page_uuid: str = None,
+        role_ids: List[int] = None,
+        userids: List[str] = None,
+    ):
+        self.all_visible = all_visible
+        self.dept_ids = dept_ids
+        self.page_name = page_name
+        self.page_uuid = page_uuid
+        self.role_ids = role_ids
+        self.userids = userids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_ids is not None:
-            result['userIds'] = self.user_ids
+        if self.all_visible is not None:
+            result['allVisible'] = self.all_visible
+        if self.dept_ids is not None:
+            result['deptIds'] = self.dept_ids
+        if self.page_name is not None:
+            result['pageName'] = self.page_name
+        if self.page_uuid is not None:
+            result['pageUuid'] = self.page_uuid
+        if self.role_ids is not None:
+            result['roleIds'] = self.role_ids
+        if self.userids is not None:
+            result['userids'] = self.userids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userIds') is not None:
-            self.user_ids = m.get('userIds')
+        if m.get('allVisible') is not None:
+            self.all_visible = m.get('allVisible')
+        if m.get('deptIds') is not None:
+            self.dept_ids = m.get('deptIds')
+        if m.get('pageName') is not None:
+            self.page_name = m.get('pageName')
+        if m.get('pageUuid') is not None:
+            self.page_uuid = m.get('pageUuid')
+        if m.get('roleIds') is not None:
+            self.role_ids = m.get('roleIds')
+        if m.get('userids') is not None:
+            self.userids = m.get('userids')
         return self
 
 
-class CreateDeviceVideoConferenceResponseBody(TeaModel):
+class GetDingPortalDetailResponseBody(TeaModel):
     def __init__(
         self,
-        code: str = None,
-        conference_id: str = None,
+        app_uuid: str = None,
+        ding_portal_name: str = None,
+        pages: List[GetDingPortalDetailResponseBodyPages] = None,
     ):
-        self.code = code
-        self.conference_id = conference_id
+        self.app_uuid = app_uuid
+        self.ding_portal_name = ding_portal_name
+        self.pages = pages
 
     def validate(self):
-        pass
+        if self.pages:
+            for k in self.pages:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['code'] = self.code
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
+        if self.app_uuid is not None:
+            result['appUuid'] = self.app_uuid
+        if self.ding_portal_name is not None:
+            result['dingPortalName'] = self.ding_portal_name
+        result['pages'] = []
+        if self.pages is not None:
+            for k in self.pages:
+                result['pages'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
+        if m.get('appUuid') is not None:
+            self.app_uuid = m.get('appUuid')
+        if m.get('dingPortalName') is not None:
+            self.ding_portal_name = m.get('dingPortalName')
+        self.pages = []
+        if m.get('pages') is not None:
+            for k in m.get('pages'):
+                temp_model = GetDingPortalDetailResponseBodyPages()
+                self.pages.append(temp_model.from_map(k))
         return self
 
 
-class CreateDeviceVideoConferenceResponse(TeaModel):
+class GetDingPortalDetailResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateDeviceVideoConferenceResponseBody = None,
+        body: GetDingPortalDetailResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -226,20 +354,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateDeviceVideoConferenceResponseBody()
+            temp_model = GetDingPortalDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ExtractFacialFeatureHeaders(TeaModel):
+class GetPluginPermissionPointHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -264,80 +392,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ExtractFacialFeatureRequest(TeaModel):
+class GetPluginPermissionPointRequest(TeaModel):
     def __init__(
         self,
-        media_id: str = None,
-        userid: str = None,
+        mini_app_id: str = None,
     ):
-        self.media_id = media_id
-        self.userid = userid
+        self.mini_app_id = mini_app_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.media_id is not None:
-            result['mediaId'] = self.media_id
-        if self.userid is not None:
-            result['userid'] = self.userid
+        if self.mini_app_id is not None:
+            result['miniAppId'] = self.mini_app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('mediaId') is not None:
-            self.media_id = m.get('mediaId')
-        if m.get('userid') is not None:
-            self.userid = m.get('userid')
+        if m.get('miniAppId') is not None:
+            self.mini_app_id = m.get('miniAppId')
         return self
 
 
-class ExtractFacialFeatureResponseBody(TeaModel):
+class GetPluginPermissionPointResponseBody(TeaModel):
     def __init__(
         self,
-        result: bool = None,
+        permission_point_list: List[str] = None,
     ):
-        self.result = result
+        self.permission_point_list = permission_point_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.result is not None:
-            result['result'] = self.result
+        if self.permission_point_list is not None:
+            result['permissionPointList'] = self.permission_point_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('result') is not None:
-            self.result = m.get('result')
+        if m.get('permissionPointList') is not None:
+            self.permission_point_list = m.get('permissionPointList')
         return self
 
 
-class ExtractFacialFeatureResponse(TeaModel):
+class GetPluginPermissionPointResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ExtractFacialFeatureResponseBody = None,
+        body: GetPluginPermissionPointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -363,20 +485,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ExtractFacialFeatureResponseBody()
+            temp_model = GetPluginPermissionPointResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class KickDeviceVideoConferenceMembersHeaders(TeaModel):
+class GetPluginRuleCheckInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -401,76 +523,119 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class KickDeviceVideoConferenceMembersRequest(TeaModel):
+class GetPluginRuleCheckInfoRequest(TeaModel):
     def __init__(
         self,
-        user_ids: List[str] = None,
+        mini_app_id: str = None,
     ):
-        self.user_ids = user_ids
+        self.mini_app_id = mini_app_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_ids is not None:
-            result['userIds'] = self.user_ids
+        if self.mini_app_id is not None:
+            result['miniAppId'] = self.mini_app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userIds') is not None:
-            self.user_ids = m.get('userIds')
+        if m.get('miniAppId') is not None:
+            self.mini_app_id = m.get('miniAppId')
         return self
 
 
-class KickDeviceVideoConferenceMembersResponse(TeaModel):
+class GetPluginRuleCheckInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        pack_code: str = None,
+        plugin_rule_check_detail: str = None,
+    ):
+        self.pack_code = pack_code
+        self.plugin_rule_check_detail = plugin_rule_check_detail
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.pack_code is not None:
+            result['packCode'] = self.pack_code
+        if self.plugin_rule_check_detail is not None:
+            result['pluginRuleCheckDetail'] = self.plugin_rule_check_detail
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('packCode') is not None:
+            self.pack_code = m.get('packCode')
+        if m.get('pluginRuleCheckDetail') is not None:
+            self.plugin_rule_check_detail = m.get('pluginRuleCheckDetail')
+        return self
+
+
+class GetPluginRuleCheckInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
+        body: GetPluginRuleCheckInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
+        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPluginRuleCheckInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class MachineManagerUpdateHeaders(TeaModel):
+class ListWorkBenchGroupHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -495,153 +660,166 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class MachineManagerUpdateRequestAtmManagerRightMap(TeaModel):
+class ListWorkBenchGroupRequest(TeaModel):
     def __init__(
         self,
-        attendance_person_manage: bool = None,
-        bluetooth_punch_manage: bool = None,
-        device_reset: bool = None,
-        device_settings: bool = None,
-        face_punch_manage: bool = None,
-        finger_punch_manage: bool = None,
+        ecological_corp_id: str = None,
+        group_type: str = None,
+        op_union_id: str = None,
     ):
-        self.attendance_person_manage = attendance_person_manage
-        self.bluetooth_punch_manage = bluetooth_punch_manage
-        self.device_reset = device_reset
-        self.device_settings = device_settings
-        self.face_punch_manage = face_punch_manage
-        self.finger_punch_manage = finger_punch_manage
+        self.ecological_corp_id = ecological_corp_id
+        self.group_type = group_type
+        self.op_union_id = op_union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.attendance_person_manage is not None:
-            result['attendancePersonManage'] = self.attendance_person_manage
-        if self.bluetooth_punch_manage is not None:
-            result['bluetoothPunchManage'] = self.bluetooth_punch_manage
-        if self.device_reset is not None:
-            result['deviceReset'] = self.device_reset
-        if self.device_settings is not None:
-            result['deviceSettings'] = self.device_settings
-        if self.face_punch_manage is not None:
-            result['facePunchManage'] = self.face_punch_manage
-        if self.finger_punch_manage is not None:
-            result['fingerPunchManage'] = self.finger_punch_manage
+        if self.ecological_corp_id is not None:
+            result['ecologicalCorpId'] = self.ecological_corp_id
+        if self.group_type is not None:
+            result['groupType'] = self.group_type
+        if self.op_union_id is not None:
+            result['opUnionId'] = self.op_union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('attendancePersonManage') is not None:
-            self.attendance_person_manage = m.get('attendancePersonManage')
-        if m.get('bluetoothPunchManage') is not None:
-            self.bluetooth_punch_manage = m.get('bluetoothPunchManage')
-        if m.get('deviceReset') is not None:
-            self.device_reset = m.get('deviceReset')
-        if m.get('deviceSettings') is not None:
-            self.device_settings = m.get('deviceSettings')
-        if m.get('facePunchManage') is not None:
-            self.face_punch_manage = m.get('facePunchManage')
-        if m.get('fingerPunchManage') is not None:
-            self.finger_punch_manage = m.get('fingerPunchManage')
+        if m.get('ecologicalCorpId') is not None:
+            self.ecological_corp_id = m.get('ecologicalCorpId')
+        if m.get('groupType') is not None:
+            self.group_type = m.get('groupType')
+        if m.get('opUnionId') is not None:
+            self.op_union_id = m.get('opUnionId')
         return self
 
 
-class MachineManagerUpdateRequest(TeaModel):
+class ListWorkBenchGroupResponseBodyGroupList(TeaModel):
     def __init__(
         self,
-        atm_manager_right_map: MachineManagerUpdateRequestAtmManagerRightMap = None,
-        device_id: int = None,
-        scope_dept_ids: List[int] = None,
-        user_id: str = None,
+        component_id: str = None,
+        name: str = None,
     ):
-        self.atm_manager_right_map = atm_manager_right_map
-        self.device_id = device_id
-        self.scope_dept_ids = scope_dept_ids
-        self.user_id = user_id
+        self.component_id = component_id
+        self.name = name
 
     def validate(self):
-        if self.atm_manager_right_map:
-            self.atm_manager_right_map.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.atm_manager_right_map is not None:
-            result['atmManagerRightMap'] = self.atm_manager_right_map.to_map()
-        if self.device_id is not None:
-            result['deviceId'] = self.device_id
-        if self.scope_dept_ids is not None:
-            result['scopeDeptIds'] = self.scope_dept_ids
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.component_id is not None:
+            result['componentId'] = self.component_id
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('atmManagerRightMap') is not None:
-            temp_model = MachineManagerUpdateRequestAtmManagerRightMap()
-            self.atm_manager_right_map = temp_model.from_map(m['atmManagerRightMap'])
-        if m.get('deviceId') is not None:
-            self.device_id = m.get('deviceId')
-        if m.get('scopeDeptIds') is not None:
-            self.scope_dept_ids = m.get('scopeDeptIds')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('componentId') is not None:
+            self.component_id = m.get('componentId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
-class MachineManagerUpdateResponse(TeaModel):
+class ListWorkBenchGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        group_list: List[ListWorkBenchGroupResponseBodyGroupList] = None,
+    ):
+        self.group_list = group_list
+
+    def validate(self):
+        if self.group_list:
+            for k in self.group_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['groupList'] = []
+        if self.group_list is not None:
+            for k in self.group_list:
+                result['groupList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.group_list = []
+        if m.get('groupList') is not None:
+            for k in m.get('groupList'):
+                temp_model = ListWorkBenchGroupResponseBodyGroupList()
+                self.group_list.append(temp_model.from_map(k))
+        return self
+
+
+class ListWorkBenchGroupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
+        body: ListWorkBenchGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
+        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListWorkBenchGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class MachineUsersUpdateHeaders(TeaModel):
+class QueryComponentScopesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -666,106 +844,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class MachineUsersUpdateRequest(TeaModel):
+class QueryComponentScopesResponseBody(TeaModel):
     def __init__(
         self,
-        add_dept_ids: List[int] = None,
-        add_user_ids: List[str] = None,
-        del_dept_ids: List[int] = None,
-        del_user_ids: List[str] = None,
-        dev_ids: List[int] = None,
-        device_ids: List[str] = None,
+        dept_visible_scopes: List[int] = None,
+        user_visible_scopes: List[str] = None,
     ):
-        self.add_dept_ids = add_dept_ids
-        self.add_user_ids = add_user_ids
-        self.del_dept_ids = del_dept_ids
-        self.del_user_ids = del_user_ids
-        self.dev_ids = dev_ids
-        self.device_ids = device_ids
+        self.dept_visible_scopes = dept_visible_scopes
+        self.user_visible_scopes = user_visible_scopes
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.add_dept_ids is not None:
-            result['addDeptIds'] = self.add_dept_ids
-        if self.add_user_ids is not None:
-            result['addUserIds'] = self.add_user_ids
-        if self.del_dept_ids is not None:
-            result['delDeptIds'] = self.del_dept_ids
-        if self.del_user_ids is not None:
-            result['delUserIds'] = self.del_user_ids
-        if self.dev_ids is not None:
-            result['devIds'] = self.dev_ids
-        if self.device_ids is not None:
-            result['deviceIds'] = self.device_ids
+        if self.dept_visible_scopes is not None:
+            result['deptVisibleScopes'] = self.dept_visible_scopes
+        if self.user_visible_scopes is not None:
+            result['userVisibleScopes'] = self.user_visible_scopes
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('addDeptIds') is not None:
-            self.add_dept_ids = m.get('addDeptIds')
-        if m.get('addUserIds') is not None:
-            self.add_user_ids = m.get('addUserIds')
-        if m.get('delDeptIds') is not None:
-            self.del_dept_ids = m.get('delDeptIds')
-        if m.get('delUserIds') is not None:
-            self.del_user_ids = m.get('delUserIds')
-        if m.get('devIds') is not None:
-            self.dev_ids = m.get('devIds')
-        if m.get('deviceIds') is not None:
-            self.device_ids = m.get('deviceIds')
+        if m.get('deptVisibleScopes') is not None:
+            self.dept_visible_scopes = m.get('deptVisibleScopes')
+        if m.get('userVisibleScopes') is not None:
+            self.user_visible_scopes = m.get('userVisibleScopes')
         return self
 
 
-class MachineUsersUpdateResponse(TeaModel):
+class QueryComponentScopesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
+        body: QueryComponentScopesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
+        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryComponentScopesResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryDeviceVideoConferenceBookHeaders(TeaModel):
+class QueryShortcutScopesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -790,53 +954,53 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryDeviceVideoConferenceBookResponseBody(TeaModel):
+class QueryShortcutScopesResponseBody(TeaModel):
     def __init__(
         self,
-        code: str = None,
-        conference_id: str = None,
+        dept_visible_scopes: List[int] = None,
+        user_visible_scopes: List[str] = None,
     ):
-        self.code = code
-        self.conference_id = conference_id
+        self.dept_visible_scopes = dept_visible_scopes
+        self.user_visible_scopes = user_visible_scopes
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['code'] = self.code
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
+        if self.dept_visible_scopes is not None:
+            result['deptVisibleScopes'] = self.dept_visible_scopes
+        if self.user_visible_scopes is not None:
+            result['userVisibleScopes'] = self.user_visible_scopes
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
+        if m.get('deptVisibleScopes') is not None:
+            self.dept_visible_scopes = m.get('deptVisibleScopes')
+        if m.get('userVisibleScopes') is not None:
+            self.user_visible_scopes = m.get('userVisibleScopes')
         return self
 
 
-class QueryDeviceVideoConferenceBookResponse(TeaModel):
+class QueryShortcutScopesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryDeviceVideoConferenceBookResponseBody = None,
+        body: QueryShortcutScopesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -862,12 +1026,124 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryDeviceVideoConferenceBookResponseBody()
+            temp_model = QueryShortcutScopesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateDingPortalPageScopeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateDingPortalPageScopeRequest(TeaModel):
+    def __init__(
+        self,
+        all_visible: bool = None,
+        dept_ids: List[int] = None,
+        role_ids: List[int] = None,
+        userids: List[str] = None,
+    ):
+        self.all_visible = all_visible
+        self.dept_ids = dept_ids
+        self.role_ids = role_ids
+        self.userids = userids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all_visible is not None:
+            result['allVisible'] = self.all_visible
+        if self.dept_ids is not None:
+            result['deptIds'] = self.dept_ids
+        if self.role_ids is not None:
+            result['roleIds'] = self.role_ids
+        if self.userids is not None:
+            result['userids'] = self.userids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('allVisible') is not None:
+            self.all_visible = m.get('allVisible')
+        if m.get('deptIds') is not None:
+            self.dept_ids = m.get('deptIds')
+        if m.get('roleIds') is not None:
+            self.role_ids = m.get('roleIds')
+        if m.get('userids') is not None:
+            self.userids = m.get('userids')
+        return self
+
+
+class UpdateDingPortalPageScopeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,18 @@
             body['realAmount'] = request.real_amount
         if not UtilClient.is_unset(request.refund_amount):
             body['refundAmount'] = request.refund_amount
         if not UtilClient.is_unset(request.relative_order_no):
             body['relativeOrderNo'] = request.relative_order_no
         if not UtilClient.is_unset(request.source):
             body['source'] = request.source
+        if not UtilClient.is_unset(request.supply_logo):
+            body['supplyLogo'] = request.supply_logo
+        if not UtilClient.is_unset(request.supply_name):
+            body['supplyName'] = request.supply_name
         if not UtilClient.is_unset(request.target_corp_id):
             body['targetCorpId'] = request.target_corp_id
         if not UtilClient.is_unset(request.total_amount):
             body['totalAmount'] = request.total_amount
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
         real_headers = {}
@@ -356,14 +360,18 @@
             body['realAmount'] = request.real_amount
         if not UtilClient.is_unset(request.refund_amount):
             body['refundAmount'] = request.refund_amount
         if not UtilClient.is_unset(request.relative_order_no):
             body['relativeOrderNo'] = request.relative_order_no
         if not UtilClient.is_unset(request.source):
             body['source'] = request.source
+        if not UtilClient.is_unset(request.supply_logo):
+            body['supplyLogo'] = request.supply_logo
+        if not UtilClient.is_unset(request.supply_name):
+            body['supplyName'] = request.supply_name
         if not UtilClient.is_unset(request.target_corp_id):
             body['targetCorpId'] = request.target_corp_id
         if not UtilClient.is_unset(request.total_amount):
             body['totalAmount'] = request.total_amount
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
         real_headers = {}
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -704,14 +704,16 @@
         order_details: List[SyncTripOrderRequestOrderDetails] = None,
         order_no: str = None,
         order_url: str = None,
         real_amount: str = None,
         refund_amount: str = None,
         relative_order_no: str = None,
         source: str = None,
+        supply_logo: str = None,
+        supply_name: str = None,
         target_corp_id: str = None,
         total_amount: str = None,
         type: str = None,
     ):
         self.channel_type = channel_type
         self.currency = currency
         self.ding_user_id = ding_user_id
@@ -726,14 +728,16 @@
         self.order_details = order_details
         self.order_no = order_no
         self.order_url = order_url
         self.real_amount = real_amount
         self.refund_amount = refund_amount
         self.relative_order_no = relative_order_no
         self.source = source
+        self.supply_logo = supply_logo
+        self.supply_name = supply_name
         self.target_corp_id = target_corp_id
         self.total_amount = total_amount
         self.type = type
 
     def validate(self):
         if self.event:
             self.event.validate()
@@ -782,14 +786,18 @@
             result['realAmount'] = self.real_amount
         if self.refund_amount is not None:
             result['refundAmount'] = self.refund_amount
         if self.relative_order_no is not None:
             result['relativeOrderNo'] = self.relative_order_no
         if self.source is not None:
             result['source'] = self.source
+        if self.supply_logo is not None:
+            result['supplyLogo'] = self.supply_logo
+        if self.supply_name is not None:
+            result['supplyName'] = self.supply_name
         if self.target_corp_id is not None:
             result['targetCorpId'] = self.target_corp_id
         if self.total_amount is not None:
             result['totalAmount'] = self.total_amount
         if self.type is not None:
             result['type'] = self.type
         return result
@@ -832,14 +840,18 @@
             self.real_amount = m.get('realAmount')
         if m.get('refundAmount') is not None:
             self.refund_amount = m.get('refundAmount')
         if m.get('relativeOrderNo') is not None:
             self.relative_order_no = m.get('relativeOrderNo')
         if m.get('source') is not None:
             self.source = m.get('source')
+        if m.get('supplyLogo') is not None:
+            self.supply_logo = m.get('supplyLogo')
+        if m.get('supplyName') is not None:
+            self.supply_name = m.get('supplyName')
         if m.get('targetCorpId') is not None:
             self.target_corp_id = m.get('targetCorpId')
         if m.get('totalAmount') is not None:
             self.total_amount = m.get('totalAmount')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class AddRecentUserAppListHeaders(TeaModel):
+class EsignQueryGrantInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,121 +33,151 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class AddRecentUserAppListRequestUsedAppDetailList(TeaModel):
+class EsignQueryGrantInfoRequest(TeaModel):
     def __init__(
         self,
-        agent_id: str = None,
+        corp_id: str = None,
+        extension: Dict[str, str] = None,
+        union_id: str = None,
     ):
-        self.agent_id = agent_id
+        self.corp_id = corp_id
+        self.extension = extension
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.agent_id is not None:
-            result['agentId'] = self.agent_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('agentId') is not None:
-            self.agent_id = m.get('agentId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class AddRecentUserAppListRequest(TeaModel):
+class EsignQueryGrantInfoResponseBodyResult(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        used_app_detail_list: List[AddRecentUserAppListRequestUsedAppDetailList] = None,
-        user_id: str = None,
+        legal_person: str = None,
+        mobile_phone_number: str = None,
+        org_name: str = None,
+        state_code: str = None,
+        unified_social_credit: str = None,
+        user_name: str = None,
     ):
-        self.corp_id = corp_id
-        self.used_app_detail_list = used_app_detail_list
-        self.user_id = user_id
+        self.legal_person = legal_person
+        self.mobile_phone_number = mobile_phone_number
+        self.org_name = org_name
+        self.state_code = state_code
+        self.unified_social_credit = unified_social_credit
+        self.user_name = user_name
 
     def validate(self):
-        if self.used_app_detail_list:
-            for k in self.used_app_detail_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        result['usedAppDetailList'] = []
-        if self.used_app_detail_list is not None:
-            for k in self.used_app_detail_list:
-                result['usedAppDetailList'].append(k.to_map() if k else None)
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.legal_person is not None:
+            result['legalPerson'] = self.legal_person
+        if self.mobile_phone_number is not None:
+            result['mobilePhoneNumber'] = self.mobile_phone_number
+        if self.org_name is not None:
+            result['orgName'] = self.org_name
+        if self.state_code is not None:
+            result['stateCode'] = self.state_code
+        if self.unified_social_credit is not None:
+            result['unifiedSocialCredit'] = self.unified_social_credit
+        if self.user_name is not None:
+            result['userName'] = self.user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        self.used_app_detail_list = []
-        if m.get('usedAppDetailList') is not None:
-            for k in m.get('usedAppDetailList'):
-                temp_model = AddRecentUserAppListRequestUsedAppDetailList()
-                self.used_app_detail_list.append(temp_model.from_map(k))
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('legalPerson') is not None:
+            self.legal_person = m.get('legalPerson')
+        if m.get('mobilePhoneNumber') is not None:
+            self.mobile_phone_number = m.get('mobilePhoneNumber')
+        if m.get('orgName') is not None:
+            self.org_name = m.get('orgName')
+        if m.get('stateCode') is not None:
+            self.state_code = m.get('stateCode')
+        if m.get('unifiedSocialCredit') is not None:
+            self.unified_social_credit = m.get('unifiedSocialCredit')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
         return self
 
 
-class AddRecentUserAppListResponseBody(TeaModel):
+class EsignQueryGrantInfoResponseBody(TeaModel):
     def __init__(
         self,
-        result: bool = None,
+        result: EsignQueryGrantInfoResponseBodyResult = None,
+        success: bool = None,
     ):
         self.result = result
+        self.success = success
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.result is not None:
-            result['result'] = self.result
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('result') is not None:
-            self.result = m.get('result')
+            temp_model = EsignQueryGrantInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class AddRecentUserAppListResponse(TeaModel):
+class EsignQueryGrantInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: AddRecentUserAppListResponseBody = None,
+        body: EsignQueryGrantInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -173,20 +203,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = AddRecentUserAppListResponseBody()
+            temp_model = EsignQueryGrantInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetDingPortalDetailHeaders(TeaModel):
+class EsignQueryIdentityByTicketHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -211,255 +241,121 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetDingPortalDetailResponseBodyPages(TeaModel):
-    def __init__(
-        self,
-        all_visible: bool = None,
-        dept_ids: List[int] = None,
-        page_name: str = None,
-        page_uuid: str = None,
-        role_ids: List[int] = None,
-        userids: List[str] = None,
-    ):
-        self.all_visible = all_visible
-        self.dept_ids = dept_ids
-        self.page_name = page_name
-        self.page_uuid = page_uuid
-        self.role_ids = role_ids
-        self.userids = userids
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.all_visible is not None:
-            result['allVisible'] = self.all_visible
-        if self.dept_ids is not None:
-            result['deptIds'] = self.dept_ids
-        if self.page_name is not None:
-            result['pageName'] = self.page_name
-        if self.page_uuid is not None:
-            result['pageUuid'] = self.page_uuid
-        if self.role_ids is not None:
-            result['roleIds'] = self.role_ids
-        if self.userids is not None:
-            result['userids'] = self.userids
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('allVisible') is not None:
-            self.all_visible = m.get('allVisible')
-        if m.get('deptIds') is not None:
-            self.dept_ids = m.get('deptIds')
-        if m.get('pageName') is not None:
-            self.page_name = m.get('pageName')
-        if m.get('pageUuid') is not None:
-            self.page_uuid = m.get('pageUuid')
-        if m.get('roleIds') is not None:
-            self.role_ids = m.get('roleIds')
-        if m.get('userids') is not None:
-            self.userids = m.get('userids')
-        return self
-
-
-class GetDingPortalDetailResponseBody(TeaModel):
-    def __init__(
-        self,
-        app_uuid: str = None,
-        ding_portal_name: str = None,
-        pages: List[GetDingPortalDetailResponseBodyPages] = None,
-    ):
-        self.app_uuid = app_uuid
-        self.ding_portal_name = ding_portal_name
-        self.pages = pages
-
-    def validate(self):
-        if self.pages:
-            for k in self.pages:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.app_uuid is not None:
-            result['appUuid'] = self.app_uuid
-        if self.ding_portal_name is not None:
-            result['dingPortalName'] = self.ding_portal_name
-        result['pages'] = []
-        if self.pages is not None:
-            for k in self.pages:
-                result['pages'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('appUuid') is not None:
-            self.app_uuid = m.get('appUuid')
-        if m.get('dingPortalName') is not None:
-            self.ding_portal_name = m.get('dingPortalName')
-        self.pages = []
-        if m.get('pages') is not None:
-            for k in m.get('pages'):
-                temp_model = GetDingPortalDetailResponseBodyPages()
-                self.pages.append(temp_model.from_map(k))
-        return self
-
-
-class GetDingPortalDetailResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: GetDingPortalDetailResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = GetDingPortalDetailResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class GetPluginPermissionPointHeaders(TeaModel):
+class EsignQueryIdentityByTicketRequest(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
+        corp_id: str = None,
+        extension: Dict[str, str] = None,
+        ticket: str = None,
     ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+        self.corp_id = corp_id
+        self.extension = extension
+        self.ticket = ticket
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.ticket is not None:
+            result['ticket'] = self.ticket
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('ticket') is not None:
+            self.ticket = m.get('ticket')
         return self
 
 
-class GetPluginPermissionPointRequest(TeaModel):
+class EsignQueryIdentityByTicketResponseBodyResult(TeaModel):
     def __init__(
         self,
-        mini_app_id: str = None,
+        union_id: str = None,
     ):
-        self.mini_app_id = mini_app_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.mini_app_id is not None:
-            result['miniAppId'] = self.mini_app_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('miniAppId') is not None:
-            self.mini_app_id = m.get('miniAppId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class GetPluginPermissionPointResponseBody(TeaModel):
+class EsignQueryIdentityByTicketResponseBody(TeaModel):
     def __init__(
         self,
-        permission_point_list: List[str] = None,
+        result: EsignQueryIdentityByTicketResponseBodyResult = None,
+        success: bool = None,
     ):
-        self.permission_point_list = permission_point_list
+        self.result = result
+        self.success = success
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.permission_point_list is not None:
-            result['permissionPointList'] = self.permission_point_list
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('permissionPointList') is not None:
-            self.permission_point_list = m.get('permissionPointList')
+        if m.get('result') is not None:
+            temp_model = EsignQueryIdentityByTicketResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class GetPluginPermissionPointResponse(TeaModel):
+class EsignQueryIdentityByTicketResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetPluginPermissionPointResponseBody = None,
+        body: EsignQueryIdentityByTicketResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -485,20 +381,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetPluginPermissionPointResponseBody()
+            temp_model = EsignQueryIdentityByTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetPluginRuleCheckInfoHeaders(TeaModel):
+class EsignSyncEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -523,80 +419,133 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetPluginRuleCheckInfoRequest(TeaModel):
+class EsignSyncEventRequest(TeaModel):
     def __init__(
         self,
-        mini_app_id: str = None,
+        action: str = None,
+        corp_id: str = None,
+        esign_data: str = None,
+        extension: Dict[str, str] = None,
+        union_id: str = None,
     ):
-        self.mini_app_id = mini_app_id
+        self.action = action
+        self.corp_id = corp_id
+        self.esign_data = esign_data
+        self.extension = extension
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.mini_app_id is not None:
-            result['miniAppId'] = self.mini_app_id
+        if self.action is not None:
+            result['action'] = self.action
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.esign_data is not None:
+            result['esignData'] = self.esign_data
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('miniAppId') is not None:
-            self.mini_app_id = m.get('miniAppId')
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('esignData') is not None:
+            self.esign_data = m.get('esignData')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class GetPluginRuleCheckInfoResponseBody(TeaModel):
+class EsignSyncEventResponseBodyResult(TeaModel):
     def __init__(
         self,
-        pack_code: str = None,
-        plugin_rule_check_detail: str = None,
+        message: str = None,
     ):
-        self.pack_code = pack_code
-        self.plugin_rule_check_detail = plugin_rule_check_detail
+        self.message = message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.pack_code is not None:
-            result['packCode'] = self.pack_code
-        if self.plugin_rule_check_detail is not None:
-            result['pluginRuleCheckDetail'] = self.plugin_rule_check_detail
+        if self.message is not None:
+            result['message'] = self.message
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('packCode') is not None:
-            self.pack_code = m.get('packCode')
-        if m.get('pluginRuleCheckDetail') is not None:
-            self.plugin_rule_check_detail = m.get('pluginRuleCheckDetail')
+        if m.get('message') is not None:
+            self.message = m.get('message')
         return self
 
 
-class GetPluginRuleCheckInfoResponse(TeaModel):
+class EsignSyncEventResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: EsignSyncEventResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = EsignSyncEventResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class EsignSyncEventResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetPluginRuleCheckInfoResponseBody = None,
+        body: EsignSyncEventResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -622,20 +571,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetPluginRuleCheckInfoResponseBody()
+            temp_model = EsignSyncEventResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListWorkBenchGroupHeaders(TeaModel):
+class QueryAdvancedContractVersionHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -660,127 +609,127 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListWorkBenchGroupRequest(TeaModel):
+class QueryAdvancedContractVersionRequest(TeaModel):
     def __init__(
         self,
-        ecological_corp_id: str = None,
-        group_type: str = None,
-        op_union_id: str = None,
+        corp_id: str = None,
+        extension: Dict[str, str] = None,
     ):
-        self.ecological_corp_id = ecological_corp_id
-        self.group_type = group_type
-        self.op_union_id = op_union_id
+        self.corp_id = corp_id
+        self.extension = extension
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.ecological_corp_id is not None:
-            result['ecologicalCorpId'] = self.ecological_corp_id
-        if self.group_type is not None:
-            result['groupType'] = self.group_type
-        if self.op_union_id is not None:
-            result['opUnionId'] = self.op_union_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.extension is not None:
+            result['extension'] = self.extension
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ecologicalCorpId') is not None:
-            self.ecological_corp_id = m.get('ecologicalCorpId')
-        if m.get('groupType') is not None:
-            self.group_type = m.get('groupType')
-        if m.get('opUnionId') is not None:
-            self.op_union_id = m.get('opUnionId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
         return self
 
 
-class ListWorkBenchGroupResponseBodyGroupList(TeaModel):
+class QueryAdvancedContractVersionResponseBodyResult(TeaModel):
     def __init__(
         self,
-        component_id: str = None,
-        name: str = None,
+        enable_esign_attachment_sign: bool = None,
+        extension: Dict[str, str] = None,
+        version: str = None,
     ):
-        self.component_id = component_id
-        self.name = name
+        self.enable_esign_attachment_sign = enable_esign_attachment_sign
+        self.extension = extension
+        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.component_id is not None:
-            result['componentId'] = self.component_id
-        if self.name is not None:
-            result['name'] = self.name
+        if self.enable_esign_attachment_sign is not None:
+            result['enableEsignAttachmentSign'] = self.enable_esign_attachment_sign
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.version is not None:
+            result['version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('componentId') is not None:
-            self.component_id = m.get('componentId')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('enableEsignAttachmentSign') is not None:
+            self.enable_esign_attachment_sign = m.get('enableEsignAttachmentSign')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('version') is not None:
+            self.version = m.get('version')
         return self
 
 
-class ListWorkBenchGroupResponseBody(TeaModel):
+class QueryAdvancedContractVersionResponseBody(TeaModel):
     def __init__(
         self,
-        group_list: List[ListWorkBenchGroupResponseBodyGroupList] = None,
+        result: QueryAdvancedContractVersionResponseBodyResult = None,
+        success: bool = None,
     ):
-        self.group_list = group_list
+        self.result = result
+        self.success = success
 
     def validate(self):
-        if self.group_list:
-            for k in self.group_list:
-                if k:
-                    k.validate()
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['groupList'] = []
-        if self.group_list is not None:
-            for k in self.group_list:
-                result['groupList'].append(k.to_map() if k else None)
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.group_list = []
-        if m.get('groupList') is not None:
-            for k in m.get('groupList'):
-                temp_model = ListWorkBenchGroupResponseBodyGroupList()
-                self.group_list.append(temp_model.from_map(k))
+        if m.get('result') is not None:
+            temp_model = QueryAdvancedContractVersionResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class ListWorkBenchGroupResponse(TeaModel):
+class QueryAdvancedContractVersionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListWorkBenchGroupResponseBody = None,
+        body: QueryAdvancedContractVersionResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -806,20 +755,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListWorkBenchGroupResponseBody()
+            temp_model = QueryAdvancedContractVersionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryComponentScopesHeaders(TeaModel):
+class SendContractCardHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -844,306 +793,290 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryComponentScopesResponseBody(TeaModel):
+class SendContractCardRequestContractInfo(TeaModel):
     def __init__(
         self,
-        dept_visible_scopes: List[int] = None,
-        user_visible_scopes: List[str] = None,
-    ):
-        self.dept_visible_scopes = dept_visible_scopes
-        self.user_visible_scopes = user_visible_scopes
+        contract_code: str = None,
+        contract_name: str = None,
+        create_time: int = None,
+        sign_user_name: str = None,
+    ):
+        self.contract_code = contract_code
+        self.contract_name = contract_name
+        self.create_time = create_time
+        self.sign_user_name = sign_user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.dept_visible_scopes is not None:
-            result['deptVisibleScopes'] = self.dept_visible_scopes
-        if self.user_visible_scopes is not None:
-            result['userVisibleScopes'] = self.user_visible_scopes
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('deptVisibleScopes') is not None:
-            self.dept_visible_scopes = m.get('deptVisibleScopes')
-        if m.get('userVisibleScopes') is not None:
-            self.user_visible_scopes = m.get('userVisibleScopes')
-        return self
-
-
-class QueryComponentScopesResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: QueryComponentScopesResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.contract_code is not None:
+            result['contractCode'] = self.contract_code
+        if self.contract_name is not None:
+            result['contractName'] = self.contract_name
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.sign_user_name is not None:
+            result['signUserName'] = self.sign_user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = QueryComponentScopesResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('contractCode') is not None:
+            self.contract_code = m.get('contractCode')
+        if m.get('contractName') is not None:
+            self.contract_name = m.get('contractName')
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('signUserName') is not None:
+            self.sign_user_name = m.get('signUserName')
         return self
 
 
-class QueryShortcutScopesHeaders(TeaModel):
+class SendContractCardRequestReceivers(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
+        corp_id: str = None,
+        user_id: str = None,
+        user_type: str = None,
     ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+        self.corp_id = corp_id
+        self.user_id = user_id
+        self.user_type = user_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_type is not None:
+            result['userType'] = self.user_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userType') is not None:
+            self.user_type = m.get('userType')
         return self
 
 
-class QueryShortcutScopesResponseBody(TeaModel):
+class SendContractCardRequestSender(TeaModel):
     def __init__(
         self,
-        dept_visible_scopes: List[int] = None,
-        user_visible_scopes: List[str] = None,
+        corp_id: str = None,
+        user_id: str = None,
+        user_type: str = None,
     ):
-        self.dept_visible_scopes = dept_visible_scopes
-        self.user_visible_scopes = user_visible_scopes
+        self.corp_id = corp_id
+        self.user_id = user_id
+        self.user_type = user_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.dept_visible_scopes is not None:
-            result['deptVisibleScopes'] = self.dept_visible_scopes
-        if self.user_visible_scopes is not None:
-            result['userVisibleScopes'] = self.user_visible_scopes
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_type is not None:
+            result['userType'] = self.user_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('deptVisibleScopes') is not None:
-            self.dept_visible_scopes = m.get('deptVisibleScopes')
-        if m.get('userVisibleScopes') is not None:
-            self.user_visible_scopes = m.get('userVisibleScopes')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userType') is not None:
+            self.user_type = m.get('userType')
         return self
 
 
-class QueryShortcutScopesResponse(TeaModel):
+class SendContractCardRequest(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: QueryShortcutScopesResponseBody = None,
+        card_type: str = None,
+        contract_info: SendContractCardRequestContractInfo = None,
+        corp_id: str = None,
+        extension: Dict[str, str] = None,
+        process_instance_id: str = None,
+        receive_groups: List[str] = None,
+        receivers: List[SendContractCardRequestReceivers] = None,
+        sender: SendContractCardRequestSender = None,
+        sync_single_chat: bool = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.card_type = card_type
+        self.contract_info = contract_info
+        self.corp_id = corp_id
+        self.extension = extension
+        self.process_instance_id = process_instance_id
+        self.receive_groups = receive_groups
+        self.receivers = receivers
+        self.sender = sender
+        self.sync_single_chat = sync_single_chat
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.contract_info:
+            self.contract_info.validate()
+        if self.receivers:
+            for k in self.receivers:
+                if k:
+                    k.validate()
+        if self.sender:
+            self.sender.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.card_type is not None:
+            result['cardType'] = self.card_type
+        if self.contract_info is not None:
+            result['contractInfo'] = self.contract_info.to_map()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        if self.receive_groups is not None:
+            result['receiveGroups'] = self.receive_groups
+        result['receivers'] = []
+        if self.receivers is not None:
+            for k in self.receivers:
+                result['receivers'].append(k.to_map() if k else None)
+        if self.sender is not None:
+            result['sender'] = self.sender.to_map()
+        if self.sync_single_chat is not None:
+            result['syncSingleChat'] = self.sync_single_chat
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = QueryShortcutScopesResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('cardType') is not None:
+            self.card_type = m.get('cardType')
+        if m.get('contractInfo') is not None:
+            temp_model = SendContractCardRequestContractInfo()
+            self.contract_info = temp_model.from_map(m['contractInfo'])
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        if m.get('receiveGroups') is not None:
+            self.receive_groups = m.get('receiveGroups')
+        self.receivers = []
+        if m.get('receivers') is not None:
+            for k in m.get('receivers'):
+                temp_model = SendContractCardRequestReceivers()
+                self.receivers.append(temp_model.from_map(k))
+        if m.get('sender') is not None:
+            temp_model = SendContractCardRequestSender()
+            self.sender = temp_model.from_map(m['sender'])
+        if m.get('syncSingleChat') is not None:
+            self.sync_single_chat = m.get('syncSingleChat')
         return self
 
 
-class UpdateDingPortalPageScopeHeaders(TeaModel):
+class SendContractCardResponseBody(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
+        success: bool = None,
     ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
-        return self
-
-
-class UpdateDingPortalPageScopeRequest(TeaModel):
-    def __init__(
-        self,
-        all_visible: bool = None,
-        dept_ids: List[int] = None,
-        role_ids: List[int] = None,
-        userids: List[str] = None,
-    ):
-        self.all_visible = all_visible
-        self.dept_ids = dept_ids
-        self.role_ids = role_ids
-        self.userids = userids
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.all_visible is not None:
-            result['allVisible'] = self.all_visible
-        if self.dept_ids is not None:
-            result['deptIds'] = self.dept_ids
-        if self.role_ids is not None:
-            result['roleIds'] = self.role_ids
-        if self.userids is not None:
-            result['userids'] = self.userids
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('allVisible') is not None:
-            self.all_visible = m.get('allVisible')
-        if m.get('deptIds') is not None:
-            self.dept_ids = m.get('deptIds')
-        if m.get('roleIds') is not None:
-            self.role_ids = m.get('roleIds')
-        if m.get('userids') is not None:
-            self.userids = m.get('userids')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class UpdateDingPortalPageScopeResponse(TeaModel):
+class SendContractCardResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
+        body: SendContractCardResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
+        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SendContractCardResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.22
+Version: 2.0.23
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,17 @@
 alibabacloud_dingtalk/project_1_0/models.py
 alibabacloud_dingtalk/project_integration_1_0/__init__.py
 alibabacloud_dingtalk/project_integration_1_0/client.py
 alibabacloud_dingtalk/project_integration_1_0/models.py
 alibabacloud_dingtalk/rcs_call_1_0/__init__.py
 alibabacloud_dingtalk/rcs_call_1_0/client.py
 alibabacloud_dingtalk/rcs_call_1_0/models.py
+alibabacloud_dingtalk/report_1_0/__init__.py
+alibabacloud_dingtalk/report_1_0/client.py
+alibabacloud_dingtalk/report_1_0/models.py
 alibabacloud_dingtalk/resident_1_0/__init__.py
 alibabacloud_dingtalk/resident_1_0/client.py
 alibabacloud_dingtalk/resident_1_0/models.py
 alibabacloud_dingtalk/robot_1_0/__init__.py
 alibabacloud_dingtalk/robot_1_0/client.py
 alibabacloud_dingtalk/robot_1_0/models.py
 alibabacloud_dingtalk/rooms_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.22/setup.py` & `alibabacloud_dingtalk-2.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 05/07/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

