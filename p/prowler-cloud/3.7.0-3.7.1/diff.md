# Comparing `tmp/prowler_cloud-3.7.0.tar.gz` & `tmp/prowler_cloud-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowler_cloud-3.7.0.tar", max compression
+gzip compressed data, was "prowler_cloud-3.7.1.tar", max compression
```

## Comparing `prowler_cloud-3.7.0.tar` & `prowler_cloud-3.7.1.tar`

### file list

```diff
@@ -1,1463 +1,1467 @@
--rw-r--r--   0        0        0    11339 2023-04-19 12:29:23.881015 prowler_cloud-3.7.0/LICENSE
--rw-r--r--   0        0        0    13569 2023-07-06 15:19:45.402712 prowler_cloud-3.7.0/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.914816 prowler_cloud-3.7.0/prowler/__init__.py
--rw-r--r--   0        0        0     8955 2023-07-03 11:01:07.431854 prowler_cloud-3.7.0/prowler/__main__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.915066 prowler_cloud-3.7.0/prowler/compliance/aws/__init__.py
--rw-r--r--   0        0        0     6516 2023-04-19 12:29:23.915167 prowler_cloud-3.7.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
--rw-r--r--   0        0        0    17475 2023-05-05 09:13:27.463166 prowler_cloud-3.7.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
--rw-r--r--   0        0        0     4834 2023-06-30 10:43:24.634853 prowler_cloud-3.7.0/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json
--rw-r--r--   0        0        0   165349 2023-06-20 14:40:34.308345 prowler_cloud-3.7.0/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json
--rw-r--r--   0        0        0   260398 2023-05-05 09:13:27.464116 prowler_cloud-3.7.0/prowler/compliance/aws/cis_1.4_aws.json
--rw-r--r--   0        0        0   287275 2023-05-05 09:13:27.464378 prowler_cloud-3.7.0/prowler/compliance/aws/cis_1.5_aws.json
--rw-r--r--   0        0        0    15458 2023-05-05 09:13:27.464544 prowler_cloud-3.7.0/prowler/compliance/aws/cisa_aws.json
--rw-r--r--   0        0        0   142312 2023-06-27 15:32:11.836451 prowler_cloud-3.7.0/prowler/compliance/aws/ens_rd2022_aws.json
--rw-r--r--   0        0        0    18551 2023-05-05 09:13:27.465542 prowler_cloud-3.7.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json
--rw-r--r--   0        0        0    57257 2023-05-05 09:13:27.465738 prowler_cloud-3.7.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
--rw-r--r--   0        0        0    31059 2023-05-05 09:13:27.465933 prowler_cloud-3.7.0/prowler/compliance/aws/ffiec_aws.json
--rw-r--r--   0        0        0    10166 2023-05-05 09:13:27.466051 prowler_cloud-3.7.0/prowler/compliance/aws/gdpr_aws.json
--rw-r--r--   0        0        0    18763 2023-05-05 09:13:27.466199 prowler_cloud-3.7.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
--rw-r--r--   0        0        0    11774 2023-04-19 12:29:23.917593 prowler_cloud-3.7.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json
--rw-r--r--   0        0        0    31000 2023-05-05 09:13:27.466383 prowler_cloud-3.7.0/prowler/compliance/aws/hipaa_aws.json
--rw-r--r--   0        0        0    41885 2023-06-27 13:53:14.834579 prowler_cloud-3.7.0/prowler/compliance/aws/iso27001_2013_aws.json
--rw-r--r--   0        0        0   132178 2023-06-30 10:43:24.635330 prowler_cloud-3.7.0/prowler/compliance/aws/mitre_attack_aws.json
--rw-r--r--   0        0        0    86208 2023-05-05 09:13:27.466727 prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json
--rw-r--r--   0        0        0    50559 2023-05-05 09:13:27.466907 prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json
--rw-r--r--   0        0        0   243911 2023-05-05 09:13:27.467143 prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json
--rw-r--r--   0        0        0    40042 2023-05-05 09:13:27.467382 prowler_cloud-3.7.0/prowler/compliance/aws/nist_csf_1.1_aws.json
--rw-r--r--   0        0        0     8722 2023-05-05 09:13:27.467518 prowler_cloud-3.7.0/prowler/compliance/aws/pci_3.2.1_aws.json
--rw-r--r--   0        0        0     8563 2023-05-05 09:13:27.467620 prowler_cloud-3.7.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
--rw-r--r--   0        0        0    93913 2023-05-05 09:13:27.467966 prowler_cloud-3.7.0/prowler/compliance/aws/soc2_aws.json
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918830 prowler_cloud-3.7.0/prowler/compliance/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.918896 prowler_cloud-3.7.0/prowler/compliance/gcp/__init__.py
--rw-r--r--   0        0        0   385663 2023-07-06 15:19:45.403878 prowler_cloud-3.7.0/prowler/compliance/gcp/cis_2.0_gcp.json
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919011 prowler_cloud-3.7.0/prowler/config/__init__.py
--rw-r--r--   0        0        0     3459 2023-07-06 13:16:28.765230 prowler_cloud-3.7.0/prowler/config/allowlist.yaml
--rw-r--r--   0        0        0      165 2023-04-19 12:29:23.919158 prowler_cloud-3.7.0/prowler/config/checklist_example.json
--rw-r--r--   0        0        0     3300 2023-07-06 15:35:28.448647 prowler_cloud-3.7.0/prowler/config/config.py
--rw-r--r--   0        0        0     1942 2023-05-08 10:22:47.016010 prowler_cloud-3.7.0/prowler/config/config.yaml
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919791 prowler_cloud-3.7.0/prowler/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-19 12:29:23.919861 prowler_cloud-3.7.0/prowler/lib/banner.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.919915 prowler_cloud-3.7.0/prowler/lib/check/__init__.py
--rw-r--r--   0        0        0    22996 2023-07-03 11:01:07.432313 prowler_cloud-3.7.0/prowler/lib/check/check.py
--rw-r--r--   0        0        0     2973 2023-04-19 12:29:23.920475 prowler_cloud-3.7.0/prowler/lib/check/checks_loader.py
--rw-r--r--   0        0        0     3864 2023-06-30 10:43:24.635796 prowler_cloud-3.7.0/prowler/lib/check/compliance.py
--rw-r--r--   0        0        0     5225 2023-06-30 10:43:24.636203 prowler_cloud-3.7.0/prowler/lib/check/compliance_models.py
--rw-r--r--   0        0        0     3835 2023-04-19 12:29:23.920708 prowler_cloud-3.7.0/prowler/lib/check/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.920774 prowler_cloud-3.7.0/prowler/lib/cli/__init__.py
--rw-r--r--   0        0        0    18411 2023-06-27 13:53:14.835271 prowler_cloud-3.7.0/prowler/lib/cli/parser.py
--rw-r--r--   0        0        0     1885 2023-04-19 12:29:23.921010 prowler_cloud-3.7.0/prowler/lib/logger.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.921073 prowler_cloud-3.7.0/prowler/lib/outputs/__init__.py
--rw-r--r--   0        0        0    34169 2023-07-06 15:19:45.404618 prowler_cloud-3.7.0/prowler/lib/outputs/compliance.py
--rw-r--r--   0        0        0    10181 2023-07-06 15:19:45.404899 prowler_cloud-3.7.0/prowler/lib/outputs/file_descriptors.py
--rw-r--r--   0        0        0    20435 2023-06-20 14:40:34.310197 prowler_cloud-3.7.0/prowler/lib/outputs/html.py
--rw-r--r--   0        0        0    12276 2023-06-27 13:52:23.853550 prowler_cloud-3.7.0/prowler/lib/outputs/json.py
--rw-r--r--   0        0        0    25615 2023-07-06 15:19:45.405141 prowler_cloud-3.7.0/prowler/lib/outputs/models.py
--rw-r--r--   0        0        0    11105 2023-07-06 15:19:45.405362 prowler_cloud-3.7.0/prowler/lib/outputs/outputs.py
--rw-r--r--   0        0        0     5015 2023-06-20 14:40:34.311159 prowler_cloud-3.7.0/prowler/lib/outputs/slack.py
--rw-r--r--   0        0        0     6592 2023-06-20 14:40:34.311418 prowler_cloud-3.7.0/prowler/lib/outputs/summary_table.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923838 prowler_cloud-3.7.0/prowler/lib/scan_filters/__init__.py
--rw-r--r--   0        0        0      552 2023-04-19 12:29:23.923910 prowler_cloud-3.7.0/prowler/lib/scan_filters/scan_filters.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.923974 prowler_cloud-3.7.0/prowler/lib/utils/__init__.py
--rw-r--r--   0        0        0     2539 2023-06-20 14:40:34.311700 prowler_cloud-3.7.0/prowler/lib/utils/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924142 prowler_cloud-3.7.0/prowler/providers/aws/__init__.py
--rw-r--r--   0        0        0    13384 2023-06-27 13:53:14.836012 prowler_cloud-3.7.0/prowler/providers/aws/aws_provider.py
--rw-r--r--   0        0        0   218667 2023-07-06 15:19:42.789198 prowler_cloud-3.7.0/prowler/providers/aws/aws_regions_by_service.json
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924651 prowler_cloud-3.7.0/prowler/providers/aws/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924735 prowler_cloud-3.7.0/prowler/providers/aws/lib/allowlist/__init__.py
--rw-r--r--   0        0        0    10757 2023-07-06 15:19:45.405631 prowler_cloud-3.7.0/prowler/providers/aws/lib/allowlist/allowlist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.924868 prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/__init__.py
--rw-r--r--   0        0        0     1871 2023-06-20 14:40:34.312925 prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/arn.py
--rw-r--r--   0        0        0     2193 2023-05-18 14:27:54.553794 prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/error.py
--rw-r--r--   0        0        0     1957 2023-05-18 14:27:54.554158 prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/models.py
--rw-r--r--   0        0        0     1152 2023-06-20 14:40:34.313217 prowler_cloud-3.7.0/prowler/providers/aws/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0     1251 2023-06-20 14:40:34.313501 prowler_cloud-3.7.0/prowler/providers/aws/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-05-18 14:27:54.554201 prowler_cloud-3.7.0/prowler/providers/aws/lib/credentials/__init__.py
--rw-r--r--   0        0        0     2459 2023-05-18 14:27:54.554464 prowler_cloud-3.7.0/prowler/providers/aws/lib/credentials/credentials.py
--rw-r--r--   0        0        0        0 2023-05-18 14:27:54.554501 prowler_cloud-3.7.0/prowler/providers/aws/lib/organizations/__init__.py
--rw-r--r--   0        0        0     1657 2023-05-18 14:27:54.554590 prowler_cloud-3.7.0/prowler/providers/aws/lib/organizations/organizations.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925231 prowler_cloud-3.7.0/prowler/providers/aws/lib/quick_inventory/__init__.py
--rw-r--r--   0        0        0    15534 2023-06-20 14:40:34.313864 prowler_cloud-3.7.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925429 prowler_cloud-3.7.0/prowler/providers/aws/lib/resource_api_tagging/__init__.py
--rw-r--r--   0        0        0     1585 2023-04-19 12:29:23.925524 prowler_cloud-3.7.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925602 prowler_cloud-3.7.0/prowler/providers/aws/lib/security_hub/__init__.py
--rw-r--r--   0        0        0     5867 2023-04-19 12:29:23.925704 prowler_cloud-3.7.0/prowler/providers/aws/lib/security_hub/security_hub.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925777 prowler_cloud-3.7.0/prowler/providers/aws/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925856 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.925925 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.925983 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
--rw-r--r--   0        0        0     1584 2023-04-19 12:29:23.926072 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
--rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.926147 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926226 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
--rw-r--r--   0        0        0     1635 2023-04-19 12:29:23.926328 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
--rw-r--r--   0        0        0     2184 2023-04-19 12:29:23.926396 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
--rw-r--r--   0        0        0     5375 2023-05-10 14:15:16.406939 prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926555 prowler_cloud-3.7.0/prowler/providers/aws/services/account/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.926641 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926710 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-19 12:29:23.926813 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
--rw-r--r--   0        0        0      717 2023-06-20 14:40:34.314180 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.926987 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.927076 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
--rw-r--r--   0        0        0      746 2023-06-20 14:40:34.314421 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927235 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-19 12:29:23.927318 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
--rw-r--r--   0        0        0      764 2023-06-20 14:40:34.314619 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
--rw-r--r--   0        0        0      706 2023-06-27 13:53:14.837050 prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927558 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927642 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:29:23.927732 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:23.927811 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.927881 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.927960 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
--rw-r--r--   0        0        0     1636 2023-04-19 12:29:23.928023 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.928090 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_client.py
--rw-r--r--   0        0        0     4752 2023-04-19 12:29:23.928187 prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928261 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928350 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-19 12:29:23.928450 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      976 2023-04-19 12:29:23.928524 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.928590 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928660 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-19 12:29:23.928751 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
--rw-r--r--   0        0        0     1126 2023-04-19 12:29:23.928823 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.928899 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-19 12:29:23.928989 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
--rw-r--r--   0        0        0      994 2023-04-19 12:29:23.929063 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929128 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1676 2023-04-19 12:29:23.929219 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-04-19 12:29:23.929284 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
--rw-r--r--   0        0        0     5320 2023-06-20 14:40:34.315084 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929405 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1181 2023-04-19 12:29:23.929484 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1093 2023-04-19 12:29:23.929553 prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929624 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929711 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1504 2023-06-20 14:40:34.315355 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.929864 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.929939 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0      995 2023-06-20 14:40:34.315632 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-06-20 14:40:34.315868 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
--rw-r--r--   0        0        0      234 2023-04-19 12:29:23.930163 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
--rw-r--r--   0        0        0     4018 2023-06-20 14:40:34.316132 prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930354 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.930444 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930518 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
--rw-r--r--   0        0        0     1346 2023-04-19 12:29:23.930597 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
--rw-r--r--   0        0        0     1273 2023-04-19 12:29:23.930659 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930725 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-19 12:29:23.930807 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
--rw-r--r--   0        0        0     1408 2023-04-19 12:29:23.930874 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.930944 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.931029 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1420 2023-04-19 12:29:23.931102 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931165 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-19 12:29:23.931240 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:23.931295 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
--rw-r--r--   0        0        0     3619 2023-04-19 12:29:23.931383 prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931448 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/__init__.py
--rw-r--r--   0        0        0      220 2023-04-19 12:29:23.931525 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931592 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-05 09:13:27.472031 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
--rw-r--r--   0        0        0     1902 2023-04-19 12:29:23.931745 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
--rw-r--r--   0        0        0       78 2023-04-19 12:29:23.931828 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.472076 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-05 09:13:27.472334 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json
--rw-r--r--   0        0        0     1002 2023-05-05 09:13:27.472880 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py
--rw-r--r--   0        0        0     4192 2023-05-05 09:13:27.473076 prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.931954 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/__init__.py
--rw-r--r--   0        0        0      204 2023-04-19 12:29:23.932016 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932077 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-19 12:29:23.932164 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2548 2023-04-19 12:29:23.932234 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932304 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.932378 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
--rw-r--r--   0        0        0     3352 2023-04-19 12:29:23.932441 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932505 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
--rw-r--r--   0        0        0     1536 2023-04-19 12:29:23.932592 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
--rw-r--r--   0        0        0     2209 2023-04-19 12:29:23.932663 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932740 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-19 12:29:23.932821 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1823 2023-04-19 12:29:23.932902 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.932963 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-19 12:29:23.933034 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.933094 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933149 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
--rw-r--r--   0        0        0     1120 2023-04-19 12:29:23.933215 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
--rw-r--r--   0        0        0     1144 2023-04-19 12:29:23.933278 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933349 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-19 12:29:23.933433 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.933505 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
--rw-r--r--   0        0        0     8137 2023-06-20 14:40:34.316418 prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933644 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/__init__.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.933747 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.933815 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-20 14:40:34.316728 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
--rw-r--r--   0        0        0      999 2023-06-20 14:40:34.316916 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934091 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
--rw-r--r--   0        0        0     1339 2023-06-20 14:40:34.317196 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
--rw-r--r--   0        0        0     1189 2023-06-20 14:40:34.317353 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
--rw-r--r--   0        0        0     6981 2023-06-27 13:53:14.837233 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934489 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-20 14:40:34.317685 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
--rw-r--r--   0        0        0     1096 2023-04-19 12:29:23.934711 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.934779 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
--rw-r--r--   0        0        0     1264 2023-06-20 14:40:34.317878 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
--rw-r--r--   0        0        0      976 2023-06-20 14:40:34.318069 prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935269 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.935355 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_client.py
--rw-r--r--   0        0        0     4466 2023-06-12 09:47:29.460240 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935540 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.935635 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
--rw-r--r--   0        0        0     1992 2023-04-19 12:29:23.935711 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.935787 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1286 2023-04-19 12:29:23.935877 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.935948 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936018 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/__init__.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.936101 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936165 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-27 13:52:23.853748 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:23.936308 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936374 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
--rw-r--r--   0        0        0     1311 2023-06-27 13:52:23.853892 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.936530 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936609 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
--rw-r--r--   0        0        0     1385 2023-06-27 13:52:23.854019 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
--rw-r--r--   0        0        0     1721 2023-05-10 11:50:34.104587 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.936817 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-27 13:52:23.854126 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1230 2023-04-19 12:29:23.936947 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937022 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
--rw-r--r--   0        0        0     1375 2023-06-27 13:52:23.854244 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
--rw-r--r--   0        0        0     1781 2023-04-19 12:29:23.937196 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937272 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.937369 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
--rw-r--r--   0        0        0     1031 2023-04-19 12:29:23.937430 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
--rw-r--r--   0        0        0     6218 2023-06-20 14:40:34.318328 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937579 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937669 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.937759 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
--rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.937826 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.937892 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.937965 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1575 2023-04-19 12:29:23.938067 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2245 2023-04-19 12:29:23.938153 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938212 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
--rw-r--r--   0        0        0     1287 2023-04-19 12:29:23.938333 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
--rw-r--r--   0        0        0     1073 2023-04-19 12:29:23.938697 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938764 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1951 2023-04-19 12:29:23.938841 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.938890 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.938948 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.939027 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
--rw-r--r--   0        0        0     1457 2023-04-19 12:29:23.939086 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939144 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-19 12:29:23.939214 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2232 2023-04-19 12:29:23.939277 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939341 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1393 2023-04-19 12:29:23.939412 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2755 2023-04-19 12:29:23.939471 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939529 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
--rw-r--r--   0        0        0     1730 2023-04-19 12:29:23.939601 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
--rw-r--r--   0        0        0     2004 2023-06-20 14:40:34.318580 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939720 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-19 12:29:23.939796 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
--rw-r--r--   0        0        0     3014 2023-06-20 14:40:34.318828 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.939922 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-19 12:29:23.939984 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
--rw-r--r--   0        0        0     3016 2023-06-20 14:40:34.319110 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
--rw-r--r--   0        0        0     9527 2023-06-27 13:53:14.837417 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940199 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940267 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.940345 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2519 2023-06-20 14:40:34.319488 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940466 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1462 2023-04-19 12:29:23.940535 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2525 2023-06-20 14:40:34.319654 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940649 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-19 12:29:23.940721 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2543 2023-06-20 14:40:34.319839 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.940837 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-19 12:29:23.940906 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2728 2023-06-20 14:40:34.320143 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:23.941012 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941070 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.941158 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
--rw-r--r--   0        0        0      922 2023-06-20 14:40:34.320335 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941280 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-19 12:29:23.941353 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1002 2023-04-19 12:29:23.941409 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941464 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
--rw-r--r--   0        0        0     1345 2023-04-19 12:29:23.941540 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
--rw-r--r--   0        0        0     5022 2023-07-03 11:01:07.433610 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941667 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
--rw-r--r--   0        0        0     1365 2023-04-19 12:29:23.941749 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
--rw-r--r--   0        0        0     1569 2023-05-05 09:13:27.476087 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.941872 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.941939 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2519 2023-06-20 14:40:34.320541 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942073 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-19 12:29:23.942161 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2465 2023-06-20 14:40:34.320747 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942293 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
--rw-r--r--   0        0        0     1495 2023-04-19 12:29:23.942381 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
--rw-r--r--   0        0        0     2336 2023-06-20 14:40:34.320931 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942526 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.942602 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
--rw-r--r--   0        0        0     3174 2023-06-20 14:40:34.321135 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942746 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
--rw-r--r--   0        0        0     1560 2023-04-19 12:29:23.942838 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
--rw-r--r--   0        0        0     2389 2023-06-20 14:40:34.321317 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.942969 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-19 12:29:23.943038 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
--rw-r--r--   0        0        0     2671 2023-06-20 14:40:34.321486 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943156 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-19 12:29:23.943233 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
--rw-r--r--   0        0        0     2876 2023-06-20 14:40:34.321688 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943362 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-19 12:29:23.943440 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
--rw-r--r--   0        0        0     2356 2023-06-20 14:40:34.321873 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943561 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
--rw-r--r--   0        0        0     1448 2023-04-19 12:29:23.943632 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
--rw-r--r--   0        0        0     2541 2023-06-20 14:40:34.322060 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943748 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-19 12:29:23.943818 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
--rw-r--r--   0        0        0     2331 2023-06-20 14:40:34.322248 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.943942 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
--rw-r--r--   0        0        0     1446 2023-04-19 12:29:23.944012 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
--rw-r--r--   0        0        0     2336 2023-06-20 14:40:34.322448 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
--rw-r--r--   0        0        0    11386 2023-06-20 14:40:34.322761 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:23.944212 prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/logs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944273 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/__init__.py
--rw-r--r--   0        0        0      234 2023-04-19 12:29:23.944347 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944416 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-19 12:29:23.944500 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
--rw-r--r--   0        0        0     1665 2023-04-19 12:29:23.944568 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
--rw-r--r--   0        0        0    10588 2023-05-24 12:24:26.331323 prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944765 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.944830 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.944884 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.944969 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
--rw-r--r--   0        0        0     1250 2023-06-20 14:40:34.323030 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945096 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.945184 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
--rw-r--r--   0        0        0     1060 2023-06-20 14:40:34.323243 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
--rw-r--r--   0        0        0     3858 2023-06-20 14:40:34.323405 prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945694 prowler_cloud-3.7.0/prowler/providers/aws/services/config/__init__.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.945780 prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.945850 prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-19 12:29:23.945945 prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
--rw-r--r--   0        0        0     1682 2023-06-20 14:40:34.323686 prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
--rw-r--r--   0        0        0     3295 2023-06-20 14:40:34.323941 prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946178 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/__init__.py
--rw-r--r--   0        0        0      254 2023-04-19 12:29:23.946265 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946353 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-19 12:29:23.946439 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
--rw-r--r--   0        0        0      997 2023-04-19 12:29:23.946510 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946579 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-19 12:29:23.946679 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
--rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.946756 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.946833 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
--rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.946921 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
--rw-r--r--   0        0        0     1872 2023-04-19 12:29:23.946998 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947066 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-19 12:29:23.947152 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
--rw-r--r--   0        0        0     1660 2023-04-19 12:29:23.947219 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947291 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
--rw-r--r--   0        0        0     1533 2023-05-23 15:26:48.800169 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
--rw-r--r--   0        0        0     1373 2023-04-19 12:29:23.947451 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
--rw-r--r--   0        0        0    13316 2023-05-24 12:24:26.331507 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947590 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-19 12:29:23.947677 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
--rw-r--r--   0        0        0     1269 2023-04-19 12:29:23.947755 prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.476586 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/__init__.py
--rw-r--r--   0        0        0      180 2023-05-05 09:13:27.476701 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.476741 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
--rw-r--r--   0        0        0      888 2023-05-24 12:24:26.331852 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
--rw-r--r--   0        0        0      967 2023-06-20 14:40:34.324165 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
--rw-r--r--   0        0        0     3504 2023-06-27 13:53:14.837593 prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947825 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.947904 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dax_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.947975 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-19 12:29:23.948080 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      957 2023-04-19 12:29:23.948147 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:23.948205 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_client.py
--rw-r--r--   0        0        0     8906 2023-06-20 14:40:34.324628 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948358 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1497 2023-04-19 12:29:23.948440 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      988 2023-04-19 12:29:23.948503 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948563 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-19 12:29:23.948637 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
--rw-r--r--   0        0        0      933 2023-04-19 12:29:23.948691 prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948749 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.948833 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.948914 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
--rw-r--r--   0        0        0      843 2023-04-19 12:29:23.948970 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.949029 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949092 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-19 12:29:23.949180 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
--rw-r--r--   0        0        0      850 2023-06-20 14:40:34.324803 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949304 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-19 12:29:23.949464 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
--rw-r--r--   0        0        0      965 2023-04-19 12:29:23.949557 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949630 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
--rw-r--r--   0        0        0     1530 2023-04-19 12:29:23.949725 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
--rw-r--r--   0        0        0      922 2023-04-19 12:29:23.949801 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.949868 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-19 12:29:23.949957 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
--rw-r--r--   0        0        0      849 2023-04-19 12:29:23.950030 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950097 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-19 12:29:23.950180 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
--rw-r--r--   0        0        0     2037 2023-04-19 12:29:23.950242 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950302 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
--rw-r--r--   0        0        0     1107 2023-04-19 12:29:23.950384 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
--rw-r--r--   0        0        0      971 2023-04-19 12:29:23.950439 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950496 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
--rw-r--r--   0        0        0     1461 2023-04-19 12:29:23.950579 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.950656 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950724 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-19 12:29:23.950816 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
--rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.950882 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.950943 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-19 12:29:23.951025 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
--rw-r--r--   0        0        0     1253 2023-04-19 12:29:23.951080 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951148 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-19 12:29:23.951220 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
--rw-r--r--   0        0        0     1491 2023-04-19 12:29:23.951290 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951360 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
--rw-r--r--   0        0        0     1543 2023-04-19 12:29:23.951437 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
--rw-r--r--   0        0        0     1034 2023-04-19 12:29:23.951499 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951556 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-19 12:29:23.951627 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
--rw-r--r--   0        0        0     1118 2023-04-19 12:29:23.951691 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.951757 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
--rw-r--r--   0        0        0     1292 2023-04-19 12:29:23.951839 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
--rw-r--r--   0        0        0     2348 2023-04-19 12:29:23.951906 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
--rw-r--r--   0        0        0       78 2023-04-19 12:29:23.951997 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952059 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-19 12:29:23.952133 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
--rw-r--r--   0        0        0     1247 2023-04-19 12:29:23.952190 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952247 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1483 2023-04-19 12:29:23.952329 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.952407 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952471 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-19 12:29:23.952556 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.952633 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952700 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-19 12:29:23.952777 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
--rw-r--r--   0        0        0     1028 2023-06-27 13:53:14.837813 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.952917 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-19 12:29:23.953015 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
--rw-r--r--   0        0        0     1548 2023-06-27 13:53:14.837977 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953177 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:23.953258 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
--rw-r--r--   0        0        0     1516 2023-06-27 13:53:14.838114 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953390 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1429 2023-04-19 12:29:23.953489 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1489 2023-06-27 13:53:14.838245 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953618 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-19 12:29:23.953692 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1517 2023-06-27 13:53:14.838395 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.953865 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-19 12:29:23.953950 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
--rw-r--r--   0        0        0     1577 2023-06-27 13:53:14.838558 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954078 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-29 08:01:20.093372 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
--rw-r--r--   0        0        0     1612 2023-06-27 13:53:14.838704 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954310 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.954387 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
--rw-r--r--   0        0        0     1507 2023-06-27 13:53:14.838837 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954527 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.954613 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
--rw-r--r--   0        0        0     1523 2023-06-27 13:53:14.838968 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.954805 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-19 12:29:23.954886 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
--rw-r--r--   0        0        0     1570 2023-06-27 13:53:14.839138 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955027 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.955101 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
--rw-r--r--   0        0        0     1541 2023-06-27 13:53:14.839307 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955225 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.955470 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
--rw-r--r--   0        0        0     1516 2023-06-27 13:53:14.839465 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955701 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-19 12:29:23.955778 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
--rw-r--r--   0        0        0     1507 2023-06-27 13:53:14.839605 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.955937 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
--rw-r--r--   0        0        0     1218 2023-04-19 12:29:23.956030 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
--rw-r--r--   0        0        0     1579 2023-06-27 13:53:14.839765 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956187 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-19 12:29:23.956261 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
--rw-r--r--   0        0        0     1502 2023-06-27 13:53:14.839899 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956378 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-19 12:29:23.956461 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
--rw-r--r--   0        0        0     2440 2023-06-15 08:15:26.965365 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956612 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.956694 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
--rw-r--r--   0        0        0     1305 2023-06-15 08:15:26.965509 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.956843 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.956915 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
--rw-r--r--   0        0        0     1029 2023-06-15 08:15:26.965644 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957038 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
--rw-r--r--   0        0        0     1043 2023-04-19 12:29:23.957111 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
--rw-r--r--   0        0        0     1144 2023-06-15 08:15:26.965757 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957238 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.957327 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
--rw-r--r--   0        0        0     1219 2023-06-15 08:15:26.965882 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
--rw-r--r--   0        0        0    21389 2023-06-27 13:53:14.840071 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957595 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/lib/__init__.py
--rw-r--r--   0        0        0     2581 2023-04-19 12:29:23.957667 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/lib/network_acls.py
--rw-r--r--   0        0        0     3966 2023-06-20 14:40:34.325312 prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/lib/security_groups.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.957793 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.957867 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.478427 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1375 2023-05-05 09:13:27.478526 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1568 2023-05-10 11:50:34.106496 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958564 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.958647 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
--rw-r--r--   0        0        0     1030 2023-05-10 11:50:34.106819 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.958786 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1213 2023-04-19 12:29:23.958874 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1506 2023-05-10 11:50:34.107125 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959014 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-05 09:13:27.478749 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1108 2023-05-10 11:50:34.107376 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959276 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-19 12:29:23.959354 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
--rw-r--r--   0        0        0     2377 2023-05-10 11:50:34.107690 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
--rw-r--r--   0        0        0    13675 2023-05-30 08:44:47.534809 prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959623 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.959708 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_client.py
--rw-r--r--   0        0        0     3857 2023-04-19 12:29:23.959800 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.959863 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
--rw-r--r--   0        0        0     1625 2023-04-19 12:29:23.959946 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
--rw-r--r--   0        0        0     2328 2023-04-19 12:29:23.960011 prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960125 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.960222 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960305 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1366 2023-04-19 12:29:23.960396 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      857 2023-06-20 14:40:34.325577 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960528 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1099 2023-04-19 12:29:23.960600 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
--rw-r--r--   0        0        0      847 2023-06-20 14:40:34.325832 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.960737 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0      981 2023-04-19 12:29:23.960839 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1861 2023-06-20 14:40:34.326100 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
--rw-r--r--   0        0        0     4240 2023-06-20 14:40:34.326355 prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961116 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.961185 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961253 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.961335 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
--rw-r--r--   0        0        0      992 2023-04-19 12:29:23.961410 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961481 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
--rw-r--r--   0        0        0     1559 2023-04-19 12:29:23.961578 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
--rw-r--r--   0        0        0     1215 2023-04-19 12:29:23.961639 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961713 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-19 12:29:23.961815 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
--rw-r--r--   0        0        0     1489 2023-04-19 12:29:23.961889 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.961959 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.962044 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.962138 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
--rw-r--r--   0        0        0     4792 2023-06-20 14:40:34.326562 prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962323 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.962401 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962478 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-19 12:29:23.962564 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1115 2023-06-22 10:47:51.095598 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.962724 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-19 12:29:23.962884 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
--rw-r--r--   0        0        0      823 2023-04-19 12:29:23.963014 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963091 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.963168 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
--rw-r--r--   0        0        0      817 2023-04-19 12:29:23.963238 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
--rw-r--r--   0        0        0     4592 2023-06-23 11:43:10.292336 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963437 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-19 12:29:23.963512 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
--rw-r--r--   0        0        0      937 2023-04-19 12:29:23.963596 prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963667 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.963732 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.963789 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-19 12:29:23.963879 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
--rw-r--r--   0        0        0      892 2023-04-19 12:29:23.963953 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964013 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
--rw-r--r--   0        0        0     1718 2023-04-19 12:29:23.964087 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.964151 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964211 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-19 12:29:23.964275 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1646 2023-04-19 12:29:23.964347 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964420 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-19 12:29:23.964495 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
--rw-r--r--   0        0        0      888 2023-04-19 12:29:23.964568 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964639 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
--rw-r--r--   0        0        0      996 2023-04-19 12:29:23.964720 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
--rw-r--r--   0        0        0      836 2023-04-19 12:29:23.964781 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.964855 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1435 2023-04-19 12:29:23.964939 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
--rw-r--r--   0        0        0      924 2023-04-19 12:29:23.965007 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
--rw-r--r--   0        0        0     7882 2023-06-23 11:43:10.292512 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965174 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1325 2023-04-19 12:29:23.965247 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
--rw-r--r--   0        0        0     1664 2023-04-19 12:29:23.965315 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965389 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-19 12:29:23.965478 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1439 2023-04-19 12:29:23.965558 prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965631 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.965708 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.965783 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-19 12:29:23.965875 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
--rw-r--r--   0        0        0      981 2023-06-20 14:40:34.326737 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966035 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
--rw-r--r--   0        0        0      897 2023-04-19 12:29:23.966124 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
--rw-r--r--   0        0        0     1200 2023-04-19 12:29:23.966202 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966274 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-19 12:29:23.966359 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
--rw-r--r--   0        0        0     4444 2023-04-19 12:29:23.966445 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
--rw-r--r--   0        0        0     8372 2023-06-20 14:40:34.326930 prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_service.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.478942 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/__init__.py
--rw-r--r--   0        0        0      180 2023-05-05 09:13:27.479267 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.479335 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-20 14:40:34.327185 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json
--rw-r--r--   0        0        0     1328 2023-06-20 14:40:34.327370 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py
--rw-r--r--   0        0        0     4604 2023-06-20 14:40:34.327546 prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966618 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.966702 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_client.py
--rw-r--r--   0        0        0     4080 2023-05-24 12:24:26.332213 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.966878 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
--rw-r--r--   0        0        0     1219 2023-04-19 12:29:23.966963 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
--rw-r--r--   0        0        0     1940 2023-04-19 12:29:23.967043 prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967105 prowler_cloud-3.7.0/prowler/providers/aws/services/globalaccelerator/__init__.py
--rw-r--r--   0        0        0      259 2023-04-19 12:29:23.967180 prowler_cloud-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
--rw-r--r--   0        0        0     2455 2023-05-24 12:24:26.332349 prowler_cloud-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967325 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/__init__.py
--rw-r--r--   0        0        0      185 2023-04-19 12:29:23.967397 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967474 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1464 2023-04-19 12:29:23.967574 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      994 2023-06-20 14:40:34.327741 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967737 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-19 12:29:23.967812 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      986 2023-06-20 14:40:34.327927 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.967951 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
--rw-r--r--   0        0        0     1222 2023-04-19 12:29:23.968034 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
--rw-r--r--   0        0        0      927 2023-06-20 14:40:34.328159 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968182 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1632 2023-04-19 12:29:23.968257 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1408 2023-06-20 14:40:34.328388 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968383 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1623 2023-04-19 12:29:23.968454 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1399 2023-06-20 14:40:34.328597 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968592 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1644 2023-04-19 12:29:23.968667 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1369 2023-06-20 14:40:34.328853 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.968797 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1574 2023-04-19 12:29:23.968878 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1664 2023-06-20 14:40:34.329147 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969022 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1600 2023-04-19 12:29:23.969110 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1335 2023-06-20 14:40:34.329375 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969240 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-19 12:29:23.969311 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1326 2023-06-20 14:40:34.329584 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0    10529 2023-06-20 14:40:34.329786 prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969509 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969576 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.969697 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
--rw-r--r--   0        0        0     1221 2023-04-19 12:29:23.969805 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.969867 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.969929 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
--rw-r--r--   0        0        0     1282 2023-04-19 12:29:23.970039 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
--rw-r--r--   0        0        0     1130 2023-04-19 12:29:23.970105 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970169 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.970275 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
--rw-r--r--   0        0        0      961 2023-04-19 12:29:23.970332 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
--rw-r--r--   0        0        0     7243 2023-06-20 14:40:34.329969 prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970527 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970612 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
--rw-r--r--   0        0        0     1010 2023-04-19 12:29:23.970708 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.970784 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.970861 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-19 12:29:23.970944 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
--rw-r--r--   0        0        0     2805 2023-04-19 12:29:23.971012 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.480199 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2073 2023-05-05 09:13:27.480314 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2227 2023-05-05 09:13:27.480403 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971078 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-19 12:29:23.971163 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
--rw-r--r--   0        0        0      802 2023-04-19 12:29:23.971231 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.971296 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.480457 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2088 2023-05-05 09:13:27.480562 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2238 2023-05-05 09:13:27.480625 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.480662 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2118 2023-05-05 09:13:27.480741 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2251 2023-05-05 09:13:27.480806 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971377 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971535 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.971628 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971705 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-19 12:29:23.971792 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
--rw-r--r--   0        0        0     4146 2023-04-19 12:29:23.971858 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.971926 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
--rw-r--r--   0        0        0     1417 2023-04-19 12:29:23.972003 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-19 12:29:23.972081 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972166 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
--rw-r--r--   0        0        0     1089 2023-04-19 12:29:23.972256 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
--rw-r--r--   0        0        0     2665 2023-05-05 09:13:27.480952 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972389 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
--rw-r--r--   0        0        0     1707 2023-04-19 12:29:23.972482 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
--rw-r--r--   0        0        0     1090 2023-04-19 12:29:23.972558 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972624 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-19 12:29:23.972706 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
--rw-r--r--   0        0        0     1541 2023-04-19 12:29:23.972769 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.972838 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-19 12:29:23.972940 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
--rw-r--r--   0        0        0     1414 2023-06-20 14:40:34.330192 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973071 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973150 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
--rw-r--r--   0        0        0     1140 2023-06-20 14:40:34.330361 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973285 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-19 12:29:23.973378 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
--rw-r--r--   0        0        0     1239 2023-06-20 14:40:34.330555 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973504 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-19 12:29:23.973578 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
--rw-r--r--   0        0        0     1149 2023-06-20 14:40:34.330731 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973709 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-19 12:29:23.973792 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
--rw-r--r--   0        0        0     1285 2023-06-20 14:40:34.330905 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.973931 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.974020 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
--rw-r--r--   0        0        0     1149 2023-06-20 14:40:34.331060 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974151 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-19 12:29:23.974224 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
--rw-r--r--   0        0        0     1137 2023-06-20 14:40:34.331221 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974357 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-19 12:29:23.974457 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
--rw-r--r--   0        0        0     6229 2023-05-25 11:43:16.014146 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.974606 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-19 12:29:23.974689 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
--rw-r--r--   0        0        0     1925 2023-04-19 12:29:23.974757 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975046 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.975177 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
--rw-r--r--   0        0        0     1967 2023-05-10 11:50:34.108549 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975347 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-19 12:29:23.975454 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
--rw-r--r--   0        0        0     1954 2023-05-10 11:50:34.108760 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
--rw-r--r--   0        0        0        0 2023-05-10 11:50:34.108806 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-10 11:50:34.109073 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json
--rw-r--r--   0        0        0     4380 2023-05-10 11:50:34.109308 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975766 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
--rw-r--r--   0        0        0     1172 2023-05-10 11:50:34.109555 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
--rw-r--r--   0        0        0     4097 2023-06-27 13:53:14.840573 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.975982 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976060 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-06-20 14:40:34.331377 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976178 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1738 2023-04-19 12:29:23.976255 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.976311 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976377 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-19 12:29:23.976446 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
--rw-r--r--   0        0        0     2832 2023-04-19 12:29:23.976523 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.976606 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
--rw-r--r--   0        0        0     1335 2023-04-19 12:29:23.976734 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
--rw-r--r--   0        0        0      901 2023-04-19 12:29:23.976840 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
--rw-r--r--   0        0        0    23893 2023-06-20 14:40:34.331688 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977064 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-19 12:29:23.977144 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
--rw-r--r--   0        0        0      940 2023-04-19 12:29:23.977241 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977300 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-19 12:29:23.977369 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.977431 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977490 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.977576 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
--rw-r--r--   0        0        0     1698 2023-04-19 12:29:23.977650 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977716 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-19 12:29:23.977798 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
--rw-r--r--   0        0        0     2671 2023-04-19 12:29:23.977863 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.977919 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.977991 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.978054 prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.482853 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/__init__.py
--rw-r--r--   0        0        0      215 2023-05-05 09:13:27.483189 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.483228 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
--rw-r--r--   0        0        0     1158 2023-05-05 09:13:27.483319 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
--rw-r--r--   0        0        0     1498 2023-06-20 14:40:34.331896 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
--rw-r--r--   0        0        0     4084 2023-06-27 13:53:14.840770 prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978113 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.978191 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978250 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-19 12:29:23.978323 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
--rw-r--r--   0        0        0     1194 2023-04-19 12:29:23.978399 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978466 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.978546 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.978604 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978665 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-19 12:29:23.978738 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2525 2023-04-19 12:29:23.978835 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0     5417 2023-06-20 14:40:34.332355 prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.978985 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:23.979068 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979172 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-19 12:29:23.979278 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
--rw-r--r--   0        0        0      982 2023-06-20 14:40:34.332540 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
--rw-r--r--   0        0        0     1913 2023-06-20 14:40:34.332711 prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_service.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.483555 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/__init__.py
--rw-r--r--   0        0        0      249 2023-05-05 09:13:27.484082 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.484137 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-05 09:13:27.484448 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json
--rw-r--r--   0        0        0     1143 2023-06-20 14:40:34.333004 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py
--rw-r--r--   0        0        0     3581 2023-06-27 13:53:14.840947 prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979538 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/__init__.py
--rw-r--r--   0        0        0      238 2023-04-19 12:29:23.979628 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_client.py
--rw-r--r--   0        0        0     7580 2023-06-20 14:40:34.333302 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.979801 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-19 12:29:23.979914 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1102 2023-04-19 12:29:23.979989 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980060 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-19 12:29:23.980138 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1871 2023-04-19 12:29:23.980196 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980261 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-19 12:29:23.980344 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0     1003 2023-04-19 12:29:23.980412 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980494 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.980571 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
--rw-r--r--   0        0        0      991 2023-04-19 12:29:23.980633 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980699 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-19 12:29:23.980766 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-04-19 12:29:23.980826 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.980887 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-19 12:29:23.980964 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981024 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981096 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-19 12:29:23.981163 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2655 2023-04-19 12:29:23.981223 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981286 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
--rw-r--r--   0        0        0     1736 2023-04-19 12:29:23.981364 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.981430 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981492 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-19 12:29:23.981574 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.981643 prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981710 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.981781 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-19 12:29:23.981880 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
--rw-r--r--   0        0        0      984 2023-04-19 12:29:23.981978 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
--rw-r--r--   0        0        0      239 2023-04-19 12:29:23.982039 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982100 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-19 12:29:23.982181 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
--rw-r--r--   0        0        0     1816 2023-04-19 12:29:23.982292 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982372 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
--rw-r--r--   0        0        0     1548 2023-04-19 12:29:23.982458 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
--rw-r--r--   0        0        0     5769 2023-05-05 09:13:27.485334 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
--rw-r--r--   0        0        0     8762 2023-05-05 09:13:27.485618 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_service.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.485668 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/__init__.py
--rw-r--r--   0        0        0     1047 2023-05-05 09:13:27.486014 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json
--rw-r--r--   0        0        0     1432 2023-05-05 09:13:27.486234 prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982747 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.982808 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.982868 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1473 2023-04-19 12:29:23.982939 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
--rw-r--r--   0        0        0     1034 2023-05-24 12:24:26.332853 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983065 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-19 12:29:23.983129 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
--rw-r--r--   0        0        0     1789 2023-06-20 14:40:34.333610 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-05-10 12:51:51.349122 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/__init__.py
--rw-r--r--   0        0        0     1111 2023-06-27 13:52:23.854354 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json
--rw-r--r--   0        0        0     1215 2023-05-24 12:24:26.333114 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983243 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983318 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
--rw-r--r--   0        0        0     1010 2023-05-24 12:24:26.333266 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983450 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
--rw-r--r--   0        0        0     1488 2023-04-19 12:29:23.983528 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
--rw-r--r--   0        0        0      997 2023-05-24 12:24:26.333389 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983654 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-19 12:29:23.983734 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
--rw-r--r--   0        0        0     1019 2023-05-24 12:24:26.333504 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.983846 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-19 12:29:23.983913 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
--rw-r--r--   0        0        0     1730 2023-06-20 14:40:34.334159 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984024 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
--rw-r--r--   0        0        0     1426 2023-06-19 12:53:21.105800 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
--rw-r--r--   0        0        0     1009 2023-05-24 12:24:26.333759 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984238 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
--rw-r--r--   0        0        0     1370 2023-04-19 12:29:23.984322 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
--rw-r--r--   0        0        0      942 2023-05-24 12:24:26.333897 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984438 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
--rw-r--r--   0        0        0     1510 2023-04-19 12:29:23.984507 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
--rw-r--r--   0        0        0     1469 2023-05-24 12:24:26.334160 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
--rw-r--r--   0        0        0    16516 2023-06-20 14:40:34.334408 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984675 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-19 12:29:23.984750 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
--rw-r--r--   0        0        0     1635 2023-05-24 12:24:26.334484 prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.984870 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/__init__.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:23.984935 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985000 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-19 12:29:23.985070 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
--rw-r--r--   0        0        0      973 2023-04-19 12:29:23.985129 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985188 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-19 12:29:23.985268 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
--rw-r--r--   0        0        0      984 2023-04-19 12:29:23.985335 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985415 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-05 09:13:27.487422 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
--rw-r--r--   0        0        0      996 2023-04-19 12:29:23.985566 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985646 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
--rw-r--r--   0        0        0     1297 2023-04-19 12:29:23.985733 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
--rw-r--r--   0        0        0      992 2023-04-19 12:29:23.985798 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
--rw-r--r--   0        0        0     5144 2023-06-20 14:40:34.334645 prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.985981 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/__init__.py
--rw-r--r--   0        0        0      261 2023-04-19 12:29:23.986103 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986181 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
--rw-r--r--   0        0        0      973 2023-04-19 12:29:23.986311 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
--rw-r--r--   0        0        0     1089 2023-06-20 14:40:34.334863 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
--rw-r--r--   0        0        0     2339 2023-06-27 13:53:14.841112 prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986621 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/__init__.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:23.986702 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_client.py
--rw-r--r--   0        0        0        0 2023-05-10 11:50:34.110681 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/__init__.py
--rw-r--r--   0        0        0     1426 2023-05-10 11:50:34.111008 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json
--rw-r--r--   0        0        0     2927 2023-06-20 14:40:34.335451 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.986785 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-19 12:29:23.986873 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-19 12:29:23.986944 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987014 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
--rw-r--r--   0        0        0      998 2023-04-19 12:29:23.987103 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-19 12:29:23.987177 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987269 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-19 12:29:23.987366 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1303 2023-05-10 11:50:34.111420 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0     8575 2023-06-20 14:40:34.335723 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_service.py
--rw-r--r--   0        0        0      221 2023-04-19 12:29:23.987613 prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53domains_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987693 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.987787 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-19 12:29:23.987884 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
--rw-r--r--   0        0        0     1128 2023-06-20 14:40:34.335916 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988015 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
--rw-r--r--   0        0        0     1266 2023-04-19 12:29:23.988088 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
--rw-r--r--   0        0        0      957 2023-04-19 12:29:23.988152 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988226 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-19 12:29:23.988319 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
--rw-r--r--   0        0        0      917 2023-04-19 12:29:23.988387 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988462 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:23.988553 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-19 12:29:23.988658 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988729 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1426 2023-04-19 12:29:23.988821 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
--rw-r--r--   0        0        0      943 2023-04-19 12:29:23.988889 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.488949 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/__init__.py
--rw-r--r--   0        0        0     1399 2023-05-05 09:13:27.489275 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json
--rw-r--r--   0        0        0      944 2023-05-05 09:13:27.489501 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.988968 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:23.989059 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
--rw-r--r--   0        0        0      947 2023-04-19 12:29:23.989147 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989246 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-19 12:29:23.989355 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
--rw-r--r--   0        0        0     1716 2023-04-19 12:29:23.989421 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989491 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-19 12:29:23.989572 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
--rw-r--r--   0        0        0     4078 2023-06-20 14:40:34.336095 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989751 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-19 12:29:23.989835 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
--rw-r--r--   0        0        0     2099 2023-04-19 12:29:23.989900 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.989969 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1372 2023-04-19 12:29:23.990050 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0      978 2023-04-19 12:29:23.990109 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
--rw-r--r--   0        0        0      175 2023-04-19 12:29:23.990183 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_client.py
--rw-r--r--   0        0        0    17497 2023-06-20 14:40:34.336286 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_service.py
--rw-r--r--   0        0        0      196 2023-04-19 12:29:23.990316 prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3control_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990374 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/__init__.py
--rw-r--r--   0        0        0      210 2023-04-19 12:29:23.990438 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990496 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.990579 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0      945 2023-04-19 12:29:23.990641 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990707 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.990791 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0      966 2023-04-19 12:29:23.990864 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.990928 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1412 2023-04-19 12:29:23.991009 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-19 12:29:23.991068 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991133 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-19 12:29:23.991201 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-04-19 12:29:23.991261 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991361 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1361 2023-04-19 12:29:23.991468 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1063 2023-04-19 12:29:23.991540 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991611 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
--rw-r--r--   0        0        0     1524 2023-04-19 12:29:23.991699 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
--rw-r--r--   0        0        0     1091 2023-04-19 12:29:23.991760 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
--rw-r--r--   0        0        0    11611 2023-05-10 11:50:34.112091 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.991885 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-19 12:29:23.991978 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1040 2023-04-19 12:29:23.992040 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992106 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1106 2023-04-19 12:29:23.992184 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-04-19 12:29:23.992243 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992305 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:23.992378 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1042 2023-04-19 12:29:23.992438 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992502 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-19 12:29:23.992573 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1072 2023-04-19 12:29:23.992638 prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992702 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.992781 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-19 12:29:23.992866 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1054 2023-04-19 12:29:23.992929 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.992979 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
--rw-r--r--   0        0        0     2529 2023-05-24 12:24:26.334783 prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993113 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/__init__.py
--rw-r--r--   0        0        0      220 2023-04-19 12:29:23.993184 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993254 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-19 12:29:23.993329 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-19 12:29:23.993393 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
--rw-r--r--   0        0        0     4490 2023-04-19 12:29:23.993473 prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993540 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993616 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
--rw-r--r--   0        0        0     1051 2023-04-19 12:29:23.993699 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
--rw-r--r--   0        0        0     1259 2023-04-19 12:29:23.993773 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.993837 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-19 12:29:23.993917 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
--rw-r--r--   0        0        0     1267 2023-04-19 12:29:23.993973 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994037 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
--rw-r--r--   0        0        0     1041 2023-04-19 12:29:23.994115 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
--rw-r--r--   0        0        0     1316 2023-04-19 12:29:23.994182 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994249 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-19 12:29:23.994335 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
--rw-r--r--   0        0        0     1271 2023-04-19 12:29:23.994405 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994473 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-19 12:29:23.994548 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
--rw-r--r--   0        0        0     1353 2023-04-19 12:29:23.994604 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994667 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
--rw-r--r--   0        0        0     1020 2023-04-19 12:29:23.994734 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
--rw-r--r--   0        0        0     1275 2023-06-15 07:48:57.732866 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
--rw-r--r--   0        0        0      195 2023-04-19 12:29:23.994856 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_client.py
--rw-r--r--   0        0        0     2527 2023-04-19 12:29:23.994929 prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.994989 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995057 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_client.py
--rw-r--r--   0        0        0     3814 2023-04-19 12:29:23.995137 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995195 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-19 12:29:23.995275 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      841 2023-04-19 12:29:23.995345 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995410 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-19 12:29:23.995514 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1938 2023-05-05 09:13:27.490249 prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995633 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.995710 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995775 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1396 2023-04-19 12:29:23.995846 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-19 12:29:23.995899 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.995957 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-19 12:29:23.996042 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      939 2023-04-19 12:29:23.996103 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
--rw-r--r--   0        0        0     4417 2023-06-20 14:40:34.336573 prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996219 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.996281 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996339 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-19 12:29:23.996410 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
--rw-r--r--   0        0        0     1974 2023-04-19 12:29:23.996483 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996550 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-19 12:29:23.996637 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
--rw-r--r--   0        0        0      884 2023-04-19 12:29:23.996701 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.996767 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
--rw-r--r--   0        0        0     1557 2023-04-19 12:29:23.996859 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
--rw-r--r--   0        0        0      993 2023-06-12 09:23:17.889693 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
--rw-r--r--   0        0        0     7698 2023-06-20 14:40:34.336832 prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_service.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.490291 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/__init__.py
--rw-r--r--   0        0        0      234 2023-05-05 09:13:27.490362 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.490401 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
--rw-r--r--   0        0        0     1144 2023-06-20 14:40:34.337062 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
--rw-r--r--   0        0        0     1487 2023-06-20 14:40:34.337237 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
--rw-r--r--   0        0        0     6856 2023-06-27 13:53:14.841291 prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998014 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 12:29:23.998077 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998144 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-19 12:29:23.998228 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
--rw-r--r--   0        0        0     1478 2023-05-10 11:50:34.112695 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
--rw-r--r--   0        0        0     3575 2023-06-27 13:53:14.841494 prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998427 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:23.998500 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_client.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.490829 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
--rw-r--r--   0        0        0      945 2023-06-20 14:40:34.337901 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
--rw-r--r--   0        0        0     1010 2023-06-20 14:40:34.338057 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.998838 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-19 12:29:23.998922 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     3410 2023-06-20 14:40:34.338302 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999058 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-19 12:29:23.999134 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     2222 2023-06-20 14:40:34.338555 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999264 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1214 2023-04-19 12:29:23.999341 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      800 2023-06-20 14:40:34.338723 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:23.999459 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-19 12:29:23.999536 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
--rw-r--r--   0        0        0     1497 2023-06-20 14:40:34.338992 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
--rw-r--r--   0        0        0    16958 2023-06-27 13:53:14.841703 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_service.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.491137 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
--rw-r--r--   0        0        0      988 2023-06-20 14:40:34.339589 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
--rw-r--r--   0        0        0     1327 2023-06-20 14:40:34.339821 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.339856 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/__init__.py
--rw-r--r--   0        0        0     1370 2023-06-20 14:40:34.340103 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json
--rw-r--r--   0        0        0     1086 2023-06-20 14:40:34.340227 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py
--rw-r--r--   0        0        0        0 2023-05-05 09:13:27.491317 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
--rw-r--r--   0        0        0      967 2023-06-20 14:40:34.340500 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
--rw-r--r--   0        0        0     1483 2023-06-20 14:40:34.340781 prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000473 prowler_cloud-3.7.0/prowler/providers/aws/services/waf/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:24.000539 prowler_cloud-3.7.0/prowler/providers/aws/services/waf/waf_client.py
--rw-r--r--   0        0        0     2645 2023-04-19 12:29:24.000622 prowler_cloud-3.7.0/prowler/providers/aws/services/waf/waf_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000680 prowler_cloud-3.7.0/prowler/providers/aws/services/wafv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-19 12:29:24.000748 prowler_cloud-3.7.0/prowler/providers/aws/services/wafv2/wafv2_client.py
--rw-r--r--   0        0        0     2724 2023-04-19 12:29:24.000842 prowler_cloud-3.7.0/prowler/providers/aws/services/wafv2/wafv2_service.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.340824 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/__init__.py
--rw-r--r--   0        0        0      249 2023-06-20 14:40:34.341050 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_client.py
--rw-r--r--   0        0        0     2972 2023-06-20 14:40:34.341214 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.341248 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/__init__.py
--rw-r--r--   0        0        0     1680 2023-06-20 14:40:34.341472 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json
--rw-r--r--   0        0        0     1090 2023-06-20 14:40:34.341638 prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.000903 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/__init__.py
--rw-r--r--   0        0        0      215 2023-04-19 12:29:24.000979 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_client.py
--rw-r--r--   0        0        0     3821 2023-06-20 14:40:34.341840 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001108 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     2073 2023-04-19 12:29:24.001196 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-04-19 12:29:24.001258 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-05-10 14:15:16.408052 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/__init__.py
--rw-r--r--   0        0        0     1371 2023-05-10 14:15:16.408188 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json
--rw-r--r--   0        0        0     2344 2023-05-10 14:15:16.408290 prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001325 prowler_cloud-3.7.0/prowler/providers/azure/__init__.py
--rw-r--r--   0        0        0     8818 2023-06-20 14:40:34.342129 prowler_cloud-3.7.0/prowler/providers/azure/azure_provider.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001546 prowler_cloud-3.7.0/prowler/providers/azure/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      258 2023-04-19 12:29:24.001624 prowler_cloud-3.7.0/prowler/providers/azure/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      796 2023-04-19 12:29:24.001856 prowler_cloud-3.7.0/prowler/providers/azure/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.001965 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/__init__.py
--rw-r--r--   0        0        0      205 2023-04-19 12:29:24.002041 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002107 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-19 12:29:24.002201 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
--rw-r--r--   0        0        0     1182 2023-04-19 12:29:24.002300 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002370 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
--rw-r--r--   0        0        0      926 2023-04-19 12:29:24.002447 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
--rw-r--r--   0        0        0     1121 2023-04-19 12:29:24.002545 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002609 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-19 12:29:24.002689 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1210 2023-04-19 12:29:24.002792 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.002856 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
--rw-r--r--   0        0        0     1561 2023-04-19 12:29:24.002928 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
--rw-r--r--   0        0        0     1181 2023-04-19 12:29:24.003026 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003101 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
--rw-r--r--   0        0        0     1306 2023-04-19 12:29:24.003180 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.003285 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003354 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
--rw-r--r--   0        0        0      906 2023-04-19 12:29:24.003441 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1638 2023-04-19 12:29:24.003543 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003612 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-19 12:29:24.003699 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
--rw-r--r--   0        0        0     1122 2023-04-19 12:29:24.003798 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.003875 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
--rw-r--r--   0        0        0     1590 2023-04-19 12:29:24.003965 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-19 12:29:24.004069 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004143 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-19 12:29:24.004227 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1346 2023-04-19 12:29:24.004336 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004406 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-19 12:29:24.004481 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
--rw-r--r--   0        0        0     1170 2023-04-19 12:29:24.004577 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004642 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-19 12:29:24.004717 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
--rw-r--r--   0        0        0     1227 2023-04-19 12:29:24.004839 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.004910 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
--rw-r--r--   0        0        0     1693 2023-04-19 12:29:24.005006 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
--rw-r--r--   0        0        0     1202 2023-04-19 12:29:24.005103 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
--rw-r--r--   0        0        0     2326 2023-04-19 12:29:24.005198 prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005261 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/__init__.py
--rw-r--r--   0        0        0      180 2023-04-19 12:29:24.005325 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_client.py
--rw-r--r--   0        0        0     2696 2023-04-19 12:29:24.005421 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005484 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
--rw-r--r--   0        0        0      996 2023-04-19 12:29:24.005565 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
--rw-r--r--   0        0        0     1330 2023-04-19 12:29:24.005639 prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005701 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.005772 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-19 12:29:24.005850 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.005926 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
--rw-r--r--   0        0        0      200 2023-04-19 12:29:24.005980 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006041 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-19 12:29:24.006117 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-19 12:29:24.006185 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006249 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
--rw-r--r--   0        0        0     1765 2023-04-19 12:29:24.006334 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
--rw-r--r--   0        0        0     1265 2023-04-19 12:29:24.006399 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006465 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-19 12:29:24.006543 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
--rw-r--r--   0        0        0     1156 2023-04-19 12:29:24.006608 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006669 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
--rw-r--r--   0        0        0     1246 2023-04-19 12:29:24.006748 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
--rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.006809 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.006877 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-19 12:29:24.006957 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-19 12:29:24.007018 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007076 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-19 12:29:24.007155 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-19 12:29:24.007210 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
--rw-r--r--   0        0        0     3651 2023-04-19 12:29:24.007316 prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.007373 prowler_cloud-3.7.0/prowler/providers/common/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.007448 prowler_cloud-3.7.0/prowler/providers/common/allowlist.py
--rw-r--r--   0        0        0    15670 2023-06-20 14:40:34.342410 prowler_cloud-3.7.0/prowler/providers/common/audit_info.py
--rw-r--r--   0        0        0      251 2023-04-19 12:29:24.008002 prowler_cloud-3.7.0/prowler/providers/common/models.py
--rw-r--r--   0        0        0     4669 2023-06-20 14:40:34.342520 prowler_cloud-3.7.0/prowler/providers/common/outputs.py
--rw-r--r--   0        0        0      837 2023-05-24 12:24:26.335676 prowler_cloud-3.7.0/prowler/providers/common/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008430 prowler_cloud-3.7.0/prowler/providers/gcp/__init__.py
--rw-r--r--   0        0        0     3468 2023-06-20 14:40:34.342628 prowler_cloud-3.7.0/prowler/providers/gcp/gcp_provider.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008639 prowler_cloud-3.7.0/prowler/providers/gcp/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      229 2023-06-20 14:40:34.342738 prowler_cloud-3.7.0/prowler/providers/gcp/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      683 2023-06-20 14:40:34.342822 prowler_cloud-3.7.0/prowler/providers/gcp/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.342883 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.342952 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/__init__.py
--rw-r--r--   0        0        0     1751 2023-07-05 08:16:44.915667 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json
--rw-r--r--   0        0        0     1135 2023-07-06 15:19:45.405871 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py
--rw-r--r--   0        0        0      192 2023-06-20 14:40:34.343460 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.405928 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-06 15:19:45.406112 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json
--rw-r--r--   0        0        0      912 2023-07-06 15:19:45.406250 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.343538 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/__init__.py
--rw-r--r--   0        0        0     1700 2023-06-20 14:40:34.343783 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json
--rw-r--r--   0        0        0     1103 2023-07-06 15:19:45.406424 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py
--rw-r--r--   0        0        0     2054 2023-07-06 15:19:45.406571 prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.008869 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/__init__.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:24.008942 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009000 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-19 12:29:24.009076 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      988 2023-06-20 14:40:34.344295 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009202 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-19 12:29:24.009314 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
--rw-r--r--   0        0        0      968 2023-07-03 11:25:22.479079 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
--rw-r--r--   0        0        0     4484 2023-06-20 14:40:34.344561 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009566 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-19 12:29:24.009671 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      964 2023-06-20 14:40:34.344674 prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.009835 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
--rw-r--r--   0        0        0      266 2023-04-19 12:29:24.009910 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
--rw-r--r--   0        0        0     2408 2023-07-06 15:19:45.406727 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010050 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/__init__.py
--rw-r--r--   0        0        0      197 2023-04-19 12:29:24.010112 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010172 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
--rw-r--r--   0        0        0     1408 2023-04-19 12:29:24.010282 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
--rw-r--r--   0        0        0     1004 2023-06-20 14:40:34.344882 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010443 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-19 12:29:24.010556 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
--rw-r--r--   0        0        0     1175 2023-06-20 14:40:34.344998 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.010712 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
--rw-r--r--   0        0        0     1216 2023-04-19 12:29:24.011215 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
--rw-r--r--   0        0        0     1196 2023-06-20 14:40:34.345097 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011633 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
--rw-r--r--   0        0        0     2058 2023-04-19 12:29:24.011749 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
--rw-r--r--   0        0        0     1295 2023-06-20 14:40:34.345199 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.011912 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-19 12:29:24.012026 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
--rw-r--r--   0        0        0     1200 2023-06-20 14:40:34.345299 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012183 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-19 12:29:24.012289 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
--rw-r--r--   0        0        0     1212 2023-06-20 14:40:34.345415 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.012642 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
--rw-r--r--   0        0        0     1618 2023-04-19 12:29:24.012759 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
--rw-r--r--   0        0        0     1303 2023-06-20 14:40:34.345533 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013002 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-06 15:19:45.406892 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
--rw-r--r--   0        0        0     1316 2023-06-20 14:40:34.345664 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013261 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
--rw-r--r--   0        0        0     1955 2023-04-19 12:29:24.013390 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
--rw-r--r--   0        0        0     1459 2023-06-20 14:40:34.345819 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013695 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
--rw-r--r--   0        0        0     1745 2023-04-19 12:29:24.013803 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
--rw-r--r--   0        0        0     1403 2023-06-20 14:40:34.345930 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.013964 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-19 12:29:24.014087 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
--rw-r--r--   0        0        0     1361 2023-06-20 14:40:34.346045 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014331 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-19 12:29:24.014469 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
--rw-r--r--   0        0        0     1097 2023-06-20 14:40:34.346167 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014636 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
--rw-r--r--   0        0        0     1492 2023-04-19 12:29:24.014749 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
--rw-r--r--   0        0        0     1039 2023-06-20 14:40:34.346286 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.014903 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-19 12:29:24.014985 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      984 2023-06-20 14:40:34.346407 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015134 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
--rw-r--r--   0        0        0     2153 2023-04-19 12:29:24.015262 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
--rw-r--r--   0        0        0     1343 2023-06-20 14:40:34.346536 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015435 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
--rw-r--r--   0        0        0     1702 2023-04-19 12:29:24.015548 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
--rw-r--r--   0        0        0     1225 2023-06-20 14:40:34.346651 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.015707 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.015828 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
--rw-r--r--   0        0        0     1312 2023-06-20 14:40:34.346767 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016272 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
--rw-r--r--   0        0        0     1860 2023-04-19 12:29:24.016436 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
--rw-r--r--   0        0        0     1194 2023-06-20 14:40:34.346888 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016651 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
--rw-r--r--   0        0        0     2002 2023-04-19 12:29:24.016785 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
--rw-r--r--   0        0        0     1183 2023-06-20 14:40:34.347008 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.016981 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-19 12:29:24.017114 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
--rw-r--r--   0        0        0     1203 2023-06-20 14:40:34.347118 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.017311 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-19 12:29:24.017749 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
--rw-r--r--   0        0        0     1172 2023-06-20 14:40:34.347240 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018063 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
--rw-r--r--   0        0        0     1428 2023-04-19 12:29:24.018178 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
--rw-r--r--   0        0        0      970 2023-06-20 14:40:34.347359 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
--rw-r--r--   0        0        0     2723 2023-06-20 14:40:34.347475 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018443 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.406949 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/__init__.py
--rw-r--r--   0        0        0     1719 2023-07-06 15:19:45.407065 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json
--rw-r--r--   0        0        0     1638 2023-07-06 15:19:45.407140 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018527 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-19 12:29:24.018636 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
--rw-r--r--   0        0        0      913 2023-06-20 14:40:34.347594 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.018787 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
--rw-r--r--   0        0        0     1270 2023-04-19 12:29:24.018893 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
--rw-r--r--   0        0        0     1054 2023-06-20 14:40:34.347696 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
--rw-r--r--   0        0        0      226 2023-04-19 12:29:24.019016 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
--rw-r--r--   0        0        0     2493 2023-07-06 15:19:45.407271 prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019173 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/__init__.py
--rw-r--r--   0        0        0      192 2023-04-19 12:29:24.019237 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.407323 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/__init__.py
--rw-r--r--   0        0        0     2313 2023-07-06 15:19:45.407440 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json
--rw-r--r--   0        0        0     1987 2023-07-06 15:19:45.407537 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.407597 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/__init__.py
--rw-r--r--   0        0        0     2451 2023-07-06 15:19:45.407701 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json
--rw-r--r--   0        0        0     1977 2023-07-06 15:19:45.407785 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.407827 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-06 15:19:45.407919 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json
--rw-r--r--   0        0        0     1284 2023-07-06 15:19:45.407989 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.408067 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/__init__.py
--rw-r--r--   0        0        0     2383 2023-07-06 15:19:45.408221 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-07-06 15:19:45.408324 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.408370 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-06 15:19:45.408485 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json
--rw-r--r--   0        0        0     1266 2023-07-06 15:19:45.408579 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.408624 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/__init__.py
--rw-r--r--   0        0        0     2091 2023-07-06 15:19:45.408729 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json
--rw-r--r--   0        0        0     1443 2023-07-06 15:19:45.409079 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.409132 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-06 15:19:45.409254 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json
--rw-r--r--   0        0        0     1082 2023-07-06 15:19:45.409340 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.409388 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/__init__.py
--rw-r--r--   0        0        0     2358 2023-07-06 15:19:45.409498 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json
--rw-r--r--   0        0        0     1043 2023-07-06 15:19:45.409575 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019294 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-19 12:29:24.019382 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      891 2023-06-20 14:40:34.349360 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.409613 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-06 15:19:45.409709 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json
--rw-r--r--   0        0        0     1267 2023-07-06 15:19:45.409783 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.409829 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-06 15:19:45.409939 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-07-06 15:19:45.410023 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.410075 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1508 2023-07-06 15:19:45.410186 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json
--rw-r--r--   0        0        0      930 2023-07-06 15:19:45.410277 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019505 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-19 12:29:24.019597 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
--rw-r--r--   0        0        0     1551 2023-06-20 14:40:34.349828 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.410328 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1749 2023-07-06 15:19:45.410433 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1181 2023-07-06 15:19:45.410512 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.410572 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/__init__.py
--rw-r--r--   0        0        0     2085 2023-07-06 15:19:45.410680 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json
--rw-r--r--   0        0        0      889 2023-07-06 15:19:45.410745 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.410789 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/__init__.py
--rw-r--r--   0        0        0     1897 2023-07-06 15:19:45.410889 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json
--rw-r--r--   0        0        0      881 2023-07-06 15:19:45.410974 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py
--rw-r--r--   0        0        0    12640 2023-07-06 15:19:45.411185 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.411234 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     2121 2023-07-06 15:19:45.411341 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      949 2023-07-06 15:19:45.411441 prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.351490 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/__init__.py
--rw-r--r--   0        0        0      197 2023-06-20 14:40:34.351564 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_client.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.351627 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/__init__.py
--rw-r--r--   0        0        0     2301 2023-06-20 14:40:34.351776 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json
--rw-r--r--   0        0        0      975 2023-06-20 14:40:34.351899 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py
--rw-r--r--   0        0        0     2316 2023-06-20 14:40:34.352069 prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_service.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.352134 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/__init__.py
--rw-r--r--   0        0        0      172 2023-06-20 14:40:34.352209 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_client.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.352275 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/__init__.py
--rw-r--r--   0        0        0     1818 2023-06-20 14:40:34.352426 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json
--rw-r--r--   0        0        0      938 2023-07-06 15:19:45.411621 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.352614 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/__init__.py
--rw-r--r--   0        0        0     1826 2023-06-20 14:40:34.352758 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json
--rw-r--r--   0        0        0     1117 2023-06-20 14:40:34.352890 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.352968 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/__init__.py
--rw-r--r--   0        0        0     1829 2023-06-20 14:40:34.353125 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json
--rw-r--r--   0        0        0     1121 2023-06-20 14:40:34.353256 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py
--rw-r--r--   0        0        0     3394 2023-07-06 15:19:45.411759 prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019781 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/__init__.py
--rw-r--r--   0        0        0      205 2023-07-06 15:19:45.411860 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/accessapproval_client.py
--rw-r--r--   0        0        0      214 2023-07-06 15:19:45.411925 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/essentialcontacts_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.411974 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/__init__.py
--rw-r--r--   0        0        0     2590 2023-07-06 15:19:45.412082 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json
--rw-r--r--   0        0        0      972 2023-07-06 15:19:45.412159 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.412204 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1997 2023-07-06 15:19:45.412307 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json
--rw-r--r--   0        0        0      963 2023-07-06 15:19:45.412394 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py
--rw-r--r--   0        0        0      172 2023-04-19 12:29:24.019858 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-06-20 14:40:34.353462 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-20 14:40:34.353607 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json
--rw-r--r--   0        0        0     1605 2023-07-06 15:19:45.412557 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.412600 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-06 15:19:45.412711 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json
--rw-r--r--   0        0        0     1040 2023-07-06 15:19:45.412797 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.412839 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/__init__.py
--rw-r--r--   0        0        0     2135 2023-07-06 15:19:45.412971 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json
--rw-r--r--   0        0        0     1857 2023-07-06 15:19:45.413070 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.413119 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/__init__.py
--rw-r--r--   0        0        0     2235 2023-07-06 15:19:45.413212 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json
--rw-r--r--   0        0        0     1469 2023-07-06 15:19:45.413306 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.019919 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-19 12:29:24.019998 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     1392 2023-06-20 14:40:34.353952 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020509 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-19 12:29:24.020619 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
--rw-r--r--   0        0        0     1035 2023-06-20 14:40:34.354067 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.020931 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-19 12:29:24.021052 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
--rw-r--r--   0        0        0     1314 2023-06-20 14:40:34.354178 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
--rw-r--r--   0        0        0     6222 2023-07-06 15:19:45.413471 prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021333 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/__init__.py
--rw-r--r--   0        0        0      172 2023-04-19 12:29:24.021401 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021465 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1195 2023-04-19 12:29:24.021537 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0      993 2023-06-20 14:40:34.354396 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021662 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.021737 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1128 2023-06-20 14:40:34.354509 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
--rw-r--r--   0        0        0     5395 2023-06-20 14:40:34.354608 prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.021915 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/__init__.py
--rw-r--r--   0        0        0      192 2023-04-19 12:29:24.021981 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_client.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022046 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1438 2023-04-19 12:29:24.022174 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2234 2023-06-20 14:40:34.354760 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022510 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-19 12:29:24.022758 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2209 2023-06-20 14:40:34.354869 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.022918 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-19 12:29:24.023029 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2328 2023-06-20 14:40:34.354983 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023196 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1589 2023-06-20 14:40:34.355280 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2526 2023-06-20 14:40:34.355376 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023535 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 12:29:24.023657 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2145 2023-06-20 14:40:34.355491 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.023843 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-19 12:29:24.023959 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2324 2023-06-20 14:40:34.355649 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024131 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:29:24.024268 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2426 2023-06-20 14:40:34.355792 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024464 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1157 2023-04-19 12:29:24.024600 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2257 2023-06-20 14:40:34.355914 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
--rw-r--r--   0        0        0     3047 2023-06-20 14:40:34.356037 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_service.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.024897 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-19 12:29:24.024987 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
--rw-r--r--   0        0        0     1633 2023-06-20 14:40:34.356162 prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
--rw-r--r--   0        0        0        0 2023-04-19 12:29:24.025173 prowler_cloud-3.7.0/prowler/providers/gcp/services/monitoring/__init__.py
--rw-r--r--   0        0        0      207 2023-04-19 12:29:24.025294 prowler_cloud-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_client.py
--rw-r--r--   0        0        0     2125 2023-06-20 14:40:34.356292 prowler_cloud-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.413519 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/__init__.py
--rw-r--r--   0        0        0      226 2023-07-06 15:19:45.413617 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:45.413669 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/__init__.py
--rw-r--r--   0        0        0     1904 2023-07-06 15:19:45.413774 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json
--rw-r--r--   0        0        0     1266 2023-07-06 15:19:45.413851 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py
--rw-r--r--   0        0        0     1821 2023-07-06 15:19:45.413945 prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_service.py
--rw-r--r--   0        0        0     2496 2023-07-06 16:00:02.388404 prowler_cloud-3.7.0/pyproject.toml
--rw-r--r--   0        0        0    15578 1970-01-01 00:00:00.000000 prowler_cloud-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-01-13 11:57:05.921517 prowler_cloud-3.7.1/LICENSE
+-rw-r--r--   0        0        0    13569 2023-07-12 15:05:25.684973 prowler_cloud-3.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-16 16:13:03.525738 prowler_cloud-3.7.1/prowler/__init__.py
+-rw-r--r--   0        0        0     8955 2023-07-12 15:05:15.021561 prowler_cloud-3.7.1/prowler/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.951734 prowler_cloud-3.7.1/prowler/compliance/aws/__init__.py
+-rw-r--r--   0        0        0     6516 2023-03-06 20:22:13.679854 prowler_cloud-3.7.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
+-rw-r--r--   0        0        0    17475 2023-07-03 09:05:20.345724 prowler_cloud-3.7.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
+-rw-r--r--   0        0        0     4834 2023-07-12 15:05:15.021848 prowler_cloud-3.7.1/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json
+-rw-r--r--   0        0        0   165349 2023-07-03 09:08:09.573800 prowler_cloud-3.7.1/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json
+-rw-r--r--   0        0        0   260398 2023-07-03 09:05:20.346459 prowler_cloud-3.7.1/prowler/compliance/aws/cis_1.4_aws.json
+-rw-r--r--   0        0        0   287275 2023-07-03 09:05:20.346701 prowler_cloud-3.7.1/prowler/compliance/aws/cis_1.5_aws.json
+-rw-r--r--   0        0        0   292304 2023-07-12 15:05:25.687044 prowler_cloud-3.7.1/prowler/compliance/aws/cis_2.0_aws.json
+-rw-r--r--   0        0        0    15458 2023-07-03 09:05:20.346863 prowler_cloud-3.7.1/prowler/compliance/aws/cisa_aws.json
+-rw-r--r--   0        0        0   142312 2023-07-12 15:05:15.023167 prowler_cloud-3.7.1/prowler/compliance/aws/ens_rd2022_aws.json
+-rw-r--r--   0        0        0    18551 2023-07-03 09:05:20.347612 prowler_cloud-3.7.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json
+-rw-r--r--   0        0        0    57257 2023-07-03 09:05:20.347747 prowler_cloud-3.7.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
+-rw-r--r--   0        0        0    31059 2023-07-03 09:05:20.347911 prowler_cloud-3.7.1/prowler/compliance/aws/ffiec_aws.json
+-rw-r--r--   0        0        0    10166 2023-07-03 09:05:20.348018 prowler_cloud-3.7.1/prowler/compliance/aws/gdpr_aws.json
+-rw-r--r--   0        0        0    18763 2023-07-03 09:05:20.348157 prowler_cloud-3.7.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
+-rw-r--r--   0        0        0    11774 2023-03-06 20:22:13.684290 prowler_cloud-3.7.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json
+-rw-r--r--   0        0        0    31000 2023-07-03 09:05:20.348317 prowler_cloud-3.7.1/prowler/compliance/aws/hipaa_aws.json
+-rw-r--r--   0        0        0    41885 2023-07-12 15:05:15.023337 prowler_cloud-3.7.1/prowler/compliance/aws/iso27001_2013_aws.json
+-rw-r--r--   0        0        0   132178 2023-07-12 15:05:15.024220 prowler_cloud-3.7.1/prowler/compliance/aws/mitre_attack_aws.json
+-rw-r--r--   0        0        0    86208 2023-07-03 09:05:20.348622 prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json
+-rw-r--r--   0        0        0    50559 2023-07-03 09:05:20.348794 prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json
+-rw-r--r--   0        0        0   243911 2023-07-03 09:05:20.349006 prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json
+-rw-r--r--   0        0        0    40042 2023-07-03 09:05:20.349181 prowler_cloud-3.7.1/prowler/compliance/aws/nist_csf_1.1_aws.json
+-rw-r--r--   0        0        0     8722 2023-07-03 09:05:20.349314 prowler_cloud-3.7.1/prowler/compliance/aws/pci_3.2.1_aws.json
+-rw-r--r--   0        0        0     8563 2023-07-03 09:05:20.349404 prowler_cloud-3.7.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
+-rw-r--r--   0        0        0    93913 2023-07-03 09:05:20.349686 prowler_cloud-3.7.1/prowler/compliance/aws/soc2_aws.json
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.953374 prowler_cloud-3.7.1/prowler/compliance/azure/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.778755 prowler_cloud-3.7.1/prowler/compliance/gcp/__init__.py
+-rw-r--r--   0        0        0   385663 2023-07-12 15:05:15.026045 prowler_cloud-3.7.1/prowler/compliance/gcp/cis_2.0_gcp.json
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.953497 prowler_cloud-3.7.1/prowler/config/__init__.py
+-rw-r--r--   0        0        0     3459 2023-07-12 15:05:15.026418 prowler_cloud-3.7.1/prowler/config/allowlist.yaml
+-rw-r--r--   0        0        0      165 2023-01-13 11:57:05.953701 prowler_cloud-3.7.1/prowler/config/checklist_example.json
+-rw-r--r--   0        0        0     3300 2023-07-12 15:13:03.129220 prowler_cloud-3.7.1/prowler/config/config.py
+-rw-r--r--   0        0        0     1942 2023-07-03 09:04:44.779107 prowler_cloud-3.7.1/prowler/config/config.yaml
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.955549 prowler_cloud-3.7.1/prowler/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-01-13 11:57:05.955634 prowler_cloud-3.7.1/prowler/lib/banner.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.955700 prowler_cloud-3.7.1/prowler/lib/check/__init__.py
+-rw-r--r--   0        0        0    22996 2023-07-12 15:05:15.026817 prowler_cloud-3.7.1/prowler/lib/check/check.py
+-rw-r--r--   0        0        0     2973 2023-03-06 20:22:13.687423 prowler_cloud-3.7.1/prowler/lib/check/checks_loader.py
+-rw-r--r--   0        0        0     3864 2023-07-12 15:05:15.027175 prowler_cloud-3.7.1/prowler/lib/check/compliance.py
+-rw-r--r--   0        0        0     5225 2023-07-12 15:05:15.027524 prowler_cloud-3.7.1/prowler/lib/check/compliance_models.py
+-rw-r--r--   0        0        0     3835 2023-07-03 09:04:44.779220 prowler_cloud-3.7.1/prowler/lib/check/models.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.957104 prowler_cloud-3.7.1/prowler/lib/cli/__init__.py
+-rw-r--r--   0        0        0    18411 2023-07-12 15:05:15.027741 prowler_cloud-3.7.1/prowler/lib/cli/parser.py
+-rw-r--r--   0        0        0     1885 2023-03-06 20:22:13.688295 prowler_cloud-3.7.1/prowler/lib/logger.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.957591 prowler_cloud-3.7.1/prowler/lib/outputs/__init__.py
+-rw-r--r--   0        0        0    34169 2023-07-12 15:05:15.028194 prowler_cloud-3.7.1/prowler/lib/outputs/compliance.py
+-rw-r--r--   0        0        0    10181 2023-07-12 15:05:15.028443 prowler_cloud-3.7.1/prowler/lib/outputs/file_descriptors.py
+-rw-r--r--   0        0        0    20435 2023-07-03 09:08:09.577790 prowler_cloud-3.7.1/prowler/lib/outputs/html.py
+-rw-r--r--   0        0        0    12276 2023-07-12 15:05:15.028602 prowler_cloud-3.7.1/prowler/lib/outputs/json.py
+-rw-r--r--   0        0        0    25615 2023-07-12 15:05:15.029032 prowler_cloud-3.7.1/prowler/lib/outputs/models.py
+-rw-r--r--   0        0        0    11105 2023-07-12 15:05:15.029310 prowler_cloud-3.7.1/prowler/lib/outputs/outputs.py
+-rw-r--r--   0        0        0     5015 2023-07-03 09:08:09.578743 prowler_cloud-3.7.1/prowler/lib/outputs/slack.py
+-rw-r--r--   0        0        0     6592 2023-07-03 09:08:09.578891 prowler_cloud-3.7.1/prowler/lib/outputs/summary_table.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:22:13.689353 prowler_cloud-3.7.1/prowler/lib/scan_filters/__init__.py
+-rw-r--r--   0        0        0      552 2023-03-06 20:22:13.689438 prowler_cloud-3.7.1/prowler/lib/scan_filters/scan_filters.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.959299 prowler_cloud-3.7.1/prowler/lib/utils/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-03 09:08:09.579016 prowler_cloud-3.7.1/prowler/lib/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.959512 prowler_cloud-3.7.1/prowler/providers/aws/__init__.py
+-rw-r--r--   0        0        0    13384 2023-07-12 15:05:15.029492 prowler_cloud-3.7.1/prowler/providers/aws/aws_provider.py
+-rw-r--r--   0        0        0   219041 2023-07-12 15:05:25.687564 prowler_cloud-3.7.1/prowler/providers/aws/aws_regions_by_service.json
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.960542 prowler_cloud-3.7.1/prowler/providers/aws/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.960609 prowler_cloud-3.7.1/prowler/providers/aws/lib/allowlist/__init__.py
+-rw-r--r--   0        0        0    11103 2023-07-12 15:05:25.687801 prowler_cloud-3.7.1/prowler/providers/aws/lib/allowlist/allowlist.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.960754 prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/__init__.py
+-rw-r--r--   0        0        0     1871 2023-07-03 09:08:09.579764 prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/arn.py
+-rw-r--r--   0        0        0     2193 2023-07-03 09:08:09.579867 prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/error.py
+-rw-r--r--   0        0        0     1957 2023-07-03 09:08:09.579931 prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/models.py
+-rw-r--r--   0        0        0     1152 2023-07-03 09:08:09.580057 prowler_cloud-3.7.1/prowler/providers/aws/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0     1251 2023-07-03 09:08:09.580168 prowler_cloud-3.7.1/prowler/providers/aws/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.580210 prowler_cloud-3.7.1/prowler/providers/aws/lib/credentials/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-03 09:08:09.580303 prowler_cloud-3.7.1/prowler/providers/aws/lib/credentials/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.580340 prowler_cloud-3.7.1/prowler/providers/aws/lib/organizations/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-03 09:08:09.580417 prowler_cloud-3.7.1/prowler/providers/aws/lib/organizations/organizations.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:25.687881 prowler_cloud-3.7.1/prowler/providers/aws/lib/policy_condition_parser/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-12 15:05:25.688308 prowler_cloud-3.7.1/prowler/providers/aws/lib/policy_condition_parser/policy_condition_parser.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.961181 prowler_cloud-3.7.1/prowler/providers/aws/lib/quick_inventory/__init__.py
+-rw-r--r--   0        0        0    15534 2023-07-03 09:08:09.580574 prowler_cloud-3.7.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:03:25.023680 prowler_cloud-3.7.1/prowler/providers/aws/lib/resource_api_tagging/__init__.py
+-rw-r--r--   0        0        0     1585 2023-07-03 09:03:25.023778 prowler_cloud-3.7.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.961407 prowler_cloud-3.7.1/prowler/providers/aws/lib/security_hub/__init__.py
+-rw-r--r--   0        0        0     5867 2023-03-06 20:22:13.692076 prowler_cloud-3.7.1/prowler/providers/aws/lib/security_hub/security_hub.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.961792 prowler_cloud-3.7.1/prowler/providers/aws/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.961867 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-18 13:29:18.042815 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:22:13.692138 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
+-rw-r--r--   0        0        0     1584 2023-07-03 09:03:25.023929 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
+-rw-r--r--   0        0        0     1478 2023-07-03 09:03:25.024039 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.962013 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
+-rw-r--r--   0        0        0     1635 2023-07-03 09:03:25.024166 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
+-rw-r--r--   0        0        0     2184 2023-07-03 09:03:25.024276 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
+-rw-r--r--   0        0        0     5375 2023-07-03 09:08:09.580768 prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.962381 prowler_cloud-3.7.1/prowler/providers/aws/services/account/__init__.py
+-rw-r--r--   0        0        0      200 2023-01-13 11:57:05.962472 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.962557 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-03 09:03:25.024594 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
+-rw-r--r--   0        0        0      717 2023-07-03 09:08:09.580916 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.962905 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-03 09:03:25.024705 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
+-rw-r--r--   0        0        0      746 2023-07-03 09:08:09.581051 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.963226 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
+-rw-r--r--   0        0        0     1674 2023-07-03 09:03:25.024819 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
+-rw-r--r--   0        0        0      764 2023-07-03 09:08:09.581169 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
+-rw-r--r--   0        0        0      706 2023-07-12 15:05:15.030255 prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.963532 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.963612 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
+-rw-r--r--   0        0        0     1368 2023-07-03 09:03:25.024949 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
+-rw-r--r--   0        0        0     1233 2023-07-03 09:03:25.025050 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.963844 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-03 09:03:25.025158 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
+-rw-r--r--   0        0        0     1636 2023-07-03 09:03:25.025266 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
+-rw-r--r--   0        0        0      180 2023-02-03 08:49:54.272601 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_client.py
+-rw-r--r--   0        0        0     4752 2023-07-03 09:03:25.025377 prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.964233 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.964311 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-03 09:03:25.025502 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      976 2023-07-03 09:03:25.025601 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
+-rw-r--r--   0        0        0      215 2023-01-13 11:57:05.964569 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.964640 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-03 09:03:25.025721 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
+-rw-r--r--   0        0        0     1126 2023-07-03 09:03:25.025823 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.964844 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-03 09:03:25.025947 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
+-rw-r--r--   0        0        0      994 2023-07-03 09:03:25.026043 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.965129 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-03 09:03:25.026159 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-07-03 09:03:25.026271 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
+-rw-r--r--   0        0        0     5320 2023-07-03 09:08:09.581400 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.965448 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-03 09:03:25.026505 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1093 2023-07-03 09:03:25.026605 prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.965656 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.965729 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1504 2023-07-12 15:05:15.030423 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1123 2023-07-03 09:03:25.026817 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.965930 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0      995 2023-07-12 15:05:15.030570 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-07-03 09:08:09.581758 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
+-rw-r--r--   0        0        0      234 2023-01-13 11:57:05.966163 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
+-rw-r--r--   0        0        0     4018 2023-07-03 09:08:09.581927 prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.966348 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/__init__.py
+-rw-r--r--   0        0        0      210 2023-01-13 11:57:05.966422 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.966494 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1346 2023-07-03 09:03:25.027300 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1273 2023-07-03 09:03:25.027406 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.966742 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
+-rw-r--r--   0        0        0     1257 2023-07-03 09:03:25.027521 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
+-rw-r--r--   0        0        0     1408 2023-07-03 09:03:25.027636 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.966960 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1269 2023-07-03 09:03:25.027784 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1420 2023-07-03 09:03:25.027887 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.967252 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-03 09:03:25.028007 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1583 2023-07-03 09:03:25.028113 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
+-rw-r--r--   0        0        0     3619 2023-07-03 09:03:25.028231 prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.967550 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/__init__.py
+-rw-r--r--   0        0        0      220 2023-01-13 11:57:05.967738 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.967838 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-03 09:08:09.582064 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
+-rw-r--r--   0        0        0     1902 2023-01-13 11:57:05.968068 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
+-rw-r--r--   0        0        0       78 2023-01-13 11:57:05.968194 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.582105 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-03 09:08:09.582195 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json
+-rw-r--r--   0        0        0     1002 2023-07-03 09:08:09.582286 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py
+-rw-r--r--   0        0        0     4192 2023-07-03 09:08:09.582474 prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.968359 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/__init__.py
+-rw-r--r--   0        0        0      204 2023-01-13 11:57:05.968437 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.968512 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-03 09:03:25.028617 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2548 2023-07-03 09:03:25.028785 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.968788 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-03 09:03:25.028936 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
+-rw-r--r--   0        0        0     3352 2023-07-03 09:03:25.029047 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.969041 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
+-rw-r--r--   0        0        0     1536 2023-07-03 09:03:25.029168 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
+-rw-r--r--   0        0        0     2209 2023-07-03 09:03:25.029277 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.969297 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-03 09:03:25.029386 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1823 2023-07-03 09:03:25.029492 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.969606 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-03 09:03:25.029596 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
+-rw-r--r--   0        0        0     1058 2023-07-03 09:03:25.029704 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.969925 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
+-rw-r--r--   0        0        0     1120 2023-07-03 09:03:25.029825 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
+-rw-r--r--   0        0        0     1144 2023-07-03 09:03:25.029931 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.970351 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
+-rw-r--r--   0        0        0     1619 2023-07-03 09:03:25.030052 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
+-rw-r--r--   0        0        0     1169 2023-07-03 09:03:25.030157 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
+-rw-r--r--   0        0        0     8137 2023-07-03 09:08:09.582683 prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.067918 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-03 09:04:49.068053 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.068102 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
+-rw-r--r--   0        0        0     1350 2023-07-03 09:08:09.582850 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
+-rw-r--r--   0        0        0      999 2023-07-03 09:08:09.582980 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.068332 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-03 09:08:09.583109 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
+-rw-r--r--   0        0        0     1189 2023-07-03 09:08:09.583209 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
+-rw-r--r--   0        0        0     6981 2023-07-12 15:05:15.030736 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.068680 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
+-rw-r--r--   0        0        0     1397 2023-07-03 09:08:09.583399 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
+-rw-r--r--   0        0        0     1096 2023-07-03 09:04:49.068871 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.068909 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
+-rw-r--r--   0        0        0     1264 2023-07-03 09:08:09.583506 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
+-rw-r--r--   0        0        0      976 2023-07-03 09:08:09.583605 prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.970905 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/__init__.py
+-rw-r--r--   0        0        0      244 2023-01-13 11:57:05.971060 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_client.py
+-rw-r--r--   0        0        0     4466 2023-07-03 09:08:09.583761 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:03:25.030448 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-03 09:03:25.030682 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
+-rw-r--r--   0        0        0     1992 2023-07-03 09:03:25.030756 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.971707 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1286 2023-07-03 09:03:25.030878 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1249 2023-07-03 09:03:25.031007 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.972139 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/__init__.py
+-rw-r--r--   0        0        0      215 2023-01-13 11:57:05.972260 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.972405 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1422 2023-07-12 15:05:15.030885 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-07-03 09:03:25.031227 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.972797 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
+-rw-r--r--   0        0        0     1311 2023-07-12 15:05:15.031023 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
+-rw-r--r--   0        0        0     1164 2023-07-03 09:03:25.031442 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.973212 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
+-rw-r--r--   0        0        0     1385 2023-07-12 15:05:15.031151 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
+-rw-r--r--   0        0        0     1721 2023-07-03 09:08:09.584260 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.973664 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1491 2023-07-12 15:05:15.031261 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1230 2023-07-03 09:03:25.031888 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.974064 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-12 15:05:15.031411 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
+-rw-r--r--   0        0        0     1781 2023-07-03 09:03:25.032119 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.974487 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-03 09:03:25.032252 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
+-rw-r--r--   0        0        0     1031 2023-07-03 09:03:25.032355 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
+-rw-r--r--   0        0        0     6218 2023-07-03 09:08:09.584587 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.974972 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.069124 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-03 09:04:49.069222 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
+-rw-r--r--   0        0        0     1707 2023-07-03 09:04:49.069302 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
+-rw-r--r--   0        0        0      215 2023-01-13 11:57:05.975069 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.975161 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1575 2023-07-03 09:03:25.032632 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2245 2023-07-03 09:03:25.032786 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.069339 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-03 09:04:49.069440 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
+-rw-r--r--   0        0        0     1073 2023-07-03 09:04:49.069528 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.975474 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-03 09:03:25.032904 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1524 2023-07-03 09:03:25.033001 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.975962 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-03 09:03:25.033121 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
+-rw-r--r--   0        0        0     1457 2023-07-03 09:03:25.033223 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.976385 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-03 09:03:25.033336 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2232 2023-07-03 09:03:25.033439 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.976657 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1393 2023-07-03 09:03:25.033562 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2755 2023-07-03 09:03:25.033680 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.976929 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-03 09:03:25.033813 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
+-rw-r--r--   0        0        0     2004 2023-07-03 09:08:09.584728 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.977224 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
+-rw-r--r--   0        0        0     1537 2023-07-03 09:03:25.034127 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
+-rw-r--r--   0        0        0     3014 2023-07-03 09:08:09.584863 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.977477 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
+-rw-r--r--   0        0        0     1565 2023-07-03 09:03:25.034397 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
+-rw-r--r--   0        0        0     3016 2023-07-03 09:08:09.584966 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
+-rw-r--r--   0        0        0     9527 2023-07-12 15:05:15.031638 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.977811 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.977899 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-03 09:03:25.034831 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2519 2023-07-03 09:08:09.585256 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.978168 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1462 2023-07-03 09:03:25.035081 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2525 2023-07-03 09:08:09.585365 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.978383 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1450 2023-07-03 09:03:25.035323 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2543 2023-07-03 09:08:09.585495 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.978608 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1418 2023-07-03 09:03:25.035588 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2728 2023-07-03 09:08:09.585604 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
+-rw-r--r--   0        0        0      215 2023-01-13 11:57:05.978813 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.978880 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-03 09:03:25.035814 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
+-rw-r--r--   0        0        0      922 2023-07-03 09:08:09.585725 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.979167 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1249 2023-07-03 09:03:25.035922 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1002 2023-07-03 09:03:25.036036 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:03:25.036076 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
+-rw-r--r--   0        0        0     1345 2023-07-03 09:03:25.036166 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
+-rw-r--r--   0        0        0     5022 2023-07-12 15:05:15.031804 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.979462 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-03 09:03:25.036356 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
+-rw-r--r--   0        0        0     1569 2023-07-03 09:08:09.585839 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.979810 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-07-03 09:03:25.036552 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2519 2023-07-03 09:08:09.585973 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.980131 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-07-03 09:03:25.036751 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2465 2023-07-03 09:08:09.586086 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.980475 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
+-rw-r--r--   0        0        0     1495 2023-07-03 09:03:25.036966 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
+-rw-r--r--   0        0        0     2336 2023-07-03 09:08:09.586207 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.980814 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-03 09:03:25.037151 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
+-rw-r--r--   0        0        0     3174 2023-07-03 09:08:09.586341 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.981155 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
+-rw-r--r--   0        0        0     1560 2023-07-03 09:03:25.037336 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
+-rw-r--r--   0        0        0     2389 2023-07-03 09:08:09.586476 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.981424 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1456 2023-07-03 09:03:25.037528 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2671 2023-07-03 09:08:09.586600 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.981670 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-03 09:03:25.037726 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2876 2023-07-03 09:08:09.586701 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.981866 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-03 09:03:25.037938 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
+-rw-r--r--   0        0        0     2356 2023-07-03 09:08:09.586814 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.982056 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-03 09:03:25.038155 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
+-rw-r--r--   0        0        0     2541 2023-07-03 09:08:09.586936 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.982251 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-03 09:03:25.039298 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
+-rw-r--r--   0        0        0     2331 2023-07-03 09:08:09.587079 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.982447 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
+-rw-r--r--   0        0        0     1446 2023-07-03 09:03:25.039502 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
+-rw-r--r--   0        0        0     2336 2023-07-03 09:08:09.587198 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
+-rw-r--r--   0        0        0    11386 2023-07-03 09:08:09.587291 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
+-rw-r--r--   0        0        0      197 2023-01-13 11:57:05.982694 prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/logs_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.982758 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/__init__.py
+-rw-r--r--   0        0        0      234 2023-01-13 11:57:05.982822 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.982887 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-03 09:03:25.039853 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
+-rw-r--r--   0        0        0     1665 2023-07-03 09:03:25.039955 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
+-rw-r--r--   0        0        0    10588 2023-07-03 09:08:09.587413 prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.983759 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/__init__.py
+-rw-r--r--   0        0        0      210 2023-01-13 11:57:05.983839 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.983905 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-03 09:03:25.040212 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
+-rw-r--r--   0        0        0     1250 2023-07-03 09:08:09.587574 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.984147 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-03 09:03:25.040355 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
+-rw-r--r--   0        0        0     1060 2023-07-03 09:08:09.587694 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
+-rw-r--r--   0        0        0     3858 2023-07-03 09:08:09.587805 prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.984483 prowler_cloud-3.7.1/prowler/providers/aws/services/config/__init__.py
+-rw-r--r--   0        0        0      195 2023-01-13 11:57:05.984584 prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.984661 prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-03 09:03:25.040581 prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
+-rw-r--r--   0        0        0     1682 2023-07-03 09:08:09.587933 prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
+-rw-r--r--   0        0        0     3295 2023-07-03 09:08:09.588042 prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.985003 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/__init__.py
+-rw-r--r--   0        0        0      254 2023-01-13 11:57:05.985083 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.985154 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
+-rw-r--r--   0        0        0     1191 2023-07-03 09:03:25.040800 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
+-rw-r--r--   0        0        0      997 2023-07-03 09:03:25.040904 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.985394 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
+-rw-r--r--   0        0        0     1187 2023-07-03 09:03:25.041011 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
+-rw-r--r--   0        0        0     1041 2023-07-03 09:03:25.041105 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.985635 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
+-rw-r--r--   0        0        0     1042 2023-07-03 09:03:25.041209 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
+-rw-r--r--   0        0        0     1872 2023-07-03 09:03:25.041303 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.985897 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
+-rw-r--r--   0        0        0     1098 2023-07-03 09:03:25.041416 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
+-rw-r--r--   0        0        0     1660 2023-07-03 09:03:25.041525 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.986146 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-03 09:03:25.041657 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
+-rw-r--r--   0        0        0     1373 2023-07-03 09:03:25.041758 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
+-rw-r--r--   0        0        0    13316 2023-07-03 09:08:09.588177 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.986478 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
+-rw-r--r--   0        0        0     1265 2023-07-03 09:03:25.041978 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
+-rw-r--r--   0        0        0     1269 2023-07-03 09:03:25.042070 prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.588212 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-03 09:08:09.588351 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.588389 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-03 09:08:09.588497 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
+-rw-r--r--   0        0        0      967 2023-07-03 09:08:09.588576 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
+-rw-r--r--   0        0        0     3504 2023-07-12 15:05:15.031948 prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.986707 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/__init__.py
+-rw-r--r--   0        0        0      190 2023-01-13 11:57:05.986792 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dax_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.986871 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1594 2023-07-03 09:03:25.042204 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      957 2023-07-03 09:03:25.042314 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
+-rw-r--r--   0        0        0      205 2023-01-13 11:57:05.987136 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_client.py
+-rw-r--r--   0        0        0     8906 2023-07-03 09:08:09.588950 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.987279 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1497 2023-07-03 09:03:25.042972 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      988 2023-07-03 09:03:25.043071 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.987508 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
+-rw-r--r--   0        0        0     1529 2023-07-03 09:03:25.043161 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
+-rw-r--r--   0        0        0      933 2023-07-03 09:03:25.043249 prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.987721 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.987809 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-03 09:03:25.043351 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
+-rw-r--r--   0        0        0      843 2023-07-03 09:03:25.043457 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:05.988097 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.988200 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1192 2023-07-03 09:03:25.043576 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
+-rw-r--r--   0        0        0      850 2023-07-03 09:08:09.589120 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.988549 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
+-rw-r--r--   0        0        0     1176 2023-07-03 09:03:25.043672 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
+-rw-r--r--   0        0        0      965 2023-07-03 09:03:25.043790 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.988819 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
+-rw-r--r--   0        0        0     1530 2023-07-03 09:03:25.043914 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
+-rw-r--r--   0        0        0      922 2023-07-03 09:03:25.044025 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.989080 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-03 09:03:25.044150 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
+-rw-r--r--   0        0        0      849 2023-07-03 09:03:25.044267 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.989598 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
+-rw-r--r--   0        0        0     1057 2023-07-03 09:03:25.044389 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
+-rw-r--r--   0        0        0     2037 2023-07-03 09:03:25.044507 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.989982 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
+-rw-r--r--   0        0        0     1107 2023-07-03 09:03:25.044638 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
+-rw-r--r--   0        0        0      971 2023-07-03 09:03:25.044754 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.990358 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
+-rw-r--r--   0        0        0     1461 2023-07-03 09:03:25.044869 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
+-rw-r--r--   0        0        0     1179 2023-07-03 09:03:25.044979 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.990653 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
+-rw-r--r--   0        0        0     1067 2023-07-03 09:03:25.045104 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
+-rw-r--r--   0        0        0     1111 2023-07-03 09:03:25.045208 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.991049 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
+-rw-r--r--   0        0        0     1174 2023-07-03 09:03:25.045338 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
+-rw-r--r--   0        0        0     1253 2023-07-03 09:03:25.045452 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.991409 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
+-rw-r--r--   0        0        0     1201 2023-07-03 09:03:25.045570 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
+-rw-r--r--   0        0        0     1491 2023-07-03 09:03:25.045677 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.991745 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-03 09:03:25.045812 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
+-rw-r--r--   0        0        0     1034 2023-07-03 09:03:25.045924 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.992105 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-03 09:03:25.046073 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0     1118 2023-07-03 09:03:25.046206 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.992454 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
+-rw-r--r--   0        0        0     1292 2023-07-03 09:03:25.046370 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
+-rw-r--r--   0        0        0     2348 2023-07-03 09:03:25.046483 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
+-rw-r--r--   0        0        0       78 2023-01-13 11:57:05.992828 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.992928 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
+-rw-r--r--   0        0        0     1378 2023-07-03 09:03:25.046604 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
+-rw-r--r--   0        0        0     1247 2023-07-03 09:03:25.046718 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.993215 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-03 09:03:25.046882 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1268 2023-07-03 09:03:25.047070 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.993533 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-03 09:03:25.047231 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1296 2023-07-03 09:03:25.047360 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.993866 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
+-rw-r--r--   0        0        0     1139 2023-07-03 09:03:25.047524 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
+-rw-r--r--   0        0        0     1028 2023-07-12 15:05:15.032095 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.994172 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-03 09:03:25.047849 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
+-rw-r--r--   0        0        0     1548 2023-07-12 15:05:15.032238 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.994488 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
+-rw-r--r--   0        0        0     1169 2023-07-03 09:03:25.048106 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
+-rw-r--r--   0        0        0     1516 2023-07-12 15:05:15.032349 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.994761 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1429 2023-07-03 09:03:25.048362 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1489 2023-07-12 15:05:15.032494 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.994982 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1371 2023-07-03 09:03:25.048593 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1517 2023-07-12 15:05:15.032623 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.995196 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-03 09:03:25.048793 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
+-rw-r--r--   0        0        0     1577 2023-07-12 15:05:15.032767 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.995419 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-03 09:03:25.049018 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
+-rw-r--r--   0        0        0     1612 2023-07-12 15:05:15.032913 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.995639 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-03 09:03:25.049241 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
+-rw-r--r--   0        0        0     1507 2023-07-12 15:05:15.033064 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.995880 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-03 09:03:25.049438 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
+-rw-r--r--   0        0        0     1523 2023-07-12 15:05:15.033215 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.996118 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-03 09:03:25.049649 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
+-rw-r--r--   0        0        0     1570 2023-07-12 15:05:15.033332 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.996335 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
+-rw-r--r--   0        0        0     1190 2023-07-03 09:03:25.049880 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
+-rw-r--r--   0        0        0     1541 2023-07-12 15:05:15.033465 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.996898 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-03 09:03:25.050105 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
+-rw-r--r--   0        0        0     1516 2023-07-12 15:05:15.033588 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.997135 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-03 09:03:25.050363 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
+-rw-r--r--   0        0        0     1507 2023-07-12 15:05:15.033707 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.997351 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
+-rw-r--r--   0        0        0     1218 2023-07-03 09:03:25.050620 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
+-rw-r--r--   0        0        0     1579 2023-07-12 15:05:15.033824 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.997573 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-03 09:03:25.050875 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
+-rw-r--r--   0        0        0     1502 2023-07-12 15:05:15.033969 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.997783 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-03 09:03:25.051136 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
+-rw-r--r--   0        0        0     2440 2023-07-03 09:03:25.051257 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.997999 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-03 09:03:25.051397 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
+-rw-r--r--   0        0        0     1305 2023-07-03 09:03:25.051493 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.998202 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
+-rw-r--r--   0        0        0     1221 2023-07-03 09:03:25.051597 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
+-rw-r--r--   0        0        0     1029 2023-07-03 09:03:25.051697 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.998745 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
+-rw-r--r--   0        0        0     1043 2023-07-03 09:03:25.052015 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
+-rw-r--r--   0        0        0     1144 2023-07-03 09:03:25.052105 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.998935 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-03 09:03:25.052228 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
+-rw-r--r--   0        0        0     1219 2023-07-03 09:03:25.052320 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
+-rw-r--r--   0        0        0    21389 2023-07-12 15:05:15.034148 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.999276 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/lib/__init__.py
+-rw-r--r--   0        0        0     2581 2023-01-13 11:57:05.999365 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/lib/network_acls.py
+-rw-r--r--   0        0        0     3966 2023-07-03 09:08:09.591974 prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/lib/security_groups.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.999534 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:05.999632 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.313158 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-03 09:05:11.313332 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1568 2023-07-03 09:08:09.592132 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:05.999741 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
+-rw-r--r--   0        0        0     1123 2023-07-03 09:03:25.052581 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
+-rw-r--r--   0        0        0     1030 2023-07-03 09:08:09.592300 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.000077 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1213 2023-07-03 09:03:25.052833 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1506 2023-07-03 09:08:09.592460 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.000394 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-03 09:05:11.313516 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1108 2023-07-03 09:08:09.592588 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.000724 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-03 09:03:25.053270 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
+-rw-r--r--   0        0        0     2377 2023-07-03 09:08:09.592782 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
+-rw-r--r--   0        0        0    13675 2023-07-03 09:08:09.592908 prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.001084 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.001188 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_client.py
+-rw-r--r--   0        0        0     3857 2023-07-03 09:03:25.053625 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.001633 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
+-rw-r--r--   0        0        0     1625 2023-07-03 09:03:25.053729 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
+-rw-r--r--   0        0        0     2328 2023-07-03 09:03:25.053821 prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.002287 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.002364 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.002447 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1366 2023-07-03 09:03:25.053929 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      857 2023-07-03 09:08:09.593054 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.002702 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-03 09:03:25.054113 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      847 2023-07-03 09:08:09.593184 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.002950 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-03 09:03:25.054312 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1861 2023-07-03 09:08:09.593332 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4240 2023-07-03 09:08:09.593469 prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.003291 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.003361 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.003436 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-03 09:03:25.054611 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
+-rw-r--r--   0        0        0      992 2023-07-03 09:03:25.054705 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.003683 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-03 09:03:25.054815 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
+-rw-r--r--   0        0        0     1215 2023-07-03 09:03:25.054899 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.003930 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-03 09:03:25.055014 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
+-rw-r--r--   0        0        0     1489 2023-07-03 09:03:25.055110 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.004169 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-03 09:03:25.055207 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1020 2023-07-03 09:03:25.055294 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4792 2023-07-03 09:08:09.593593 prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.004490 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.004559 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.004624 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-03 09:03:25.055518 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1115 2023-07-03 09:03:25.055609 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.004848 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1111 2023-07-03 09:03:25.055708 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
+-rw-r--r--   0        0        0      823 2023-07-03 09:03:25.055812 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.005063 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-03 09:03:25.055908 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      817 2023-07-03 09:03:25.056006 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
+-rw-r--r--   0        0        0     4592 2023-07-03 09:03:25.056141 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.005329 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1360 2023-07-03 09:03:25.056268 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0      937 2023-07-03 09:03:25.056366 prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.005573 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-01-13 11:57:06.005675 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.005753 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-03 09:03:25.056488 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
+-rw-r--r--   0        0        0      892 2023-07-03 09:03:25.056582 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.005983 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-03 09:04:44.781437 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
+-rw-r--r--   0        0        0     1367 2023-07-03 09:04:44.781536 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.006247 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-03 09:03:25.056889 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1646 2023-07-03 09:03:25.056989 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.006511 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-03 09:03:25.057081 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
+-rw-r--r--   0        0        0      888 2023-07-03 09:03:25.057160 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.006772 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-03 09:03:25.057251 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
+-rw-r--r--   0        0        0      836 2023-07-03 09:03:25.057344 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.007033 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1435 2023-07-03 09:03:25.057464 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      924 2023-07-03 09:03:25.057554 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
+-rw-r--r--   0        0        0     7882 2023-07-03 09:03:25.057884 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.007653 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1325 2023-07-03 09:03:25.057996 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0     1664 2023-07-03 09:03:25.058097 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.007940 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1004 2023-07-03 09:03:25.058220 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1439 2023-07-03 09:03:25.058316 prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.008231 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.008324 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.008417 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-03 09:03:25.058633 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
+-rw-r--r--   0        0        0      981 2023-07-03 09:08:09.593722 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.008712 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-03 09:03:25.058747 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
+-rw-r--r--   0        0        0     1200 2023-07-03 09:03:25.058854 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.008995 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-03 09:03:25.058953 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
+-rw-r--r--   0        0        0     4444 2023-07-03 09:03:25.059054 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
+-rw-r--r--   0        0        0     8372 2023-07-03 09:08:09.593855 prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.593892 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-03 09:08:09.593959 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.593992 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-03 09:08:09.594066 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json
+-rw-r--r--   0        0        0     1328 2023-07-03 09:08:09.594134 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py
+-rw-r--r--   0        0        0     4604 2023-07-03 09:08:09.594229 prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.009341 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/__init__.py
+-rw-r--r--   0        0        0      200 2023-01-13 11:57:06.009419 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_client.py
+-rw-r--r--   0        0        0     4080 2023-07-03 09:08:09.594345 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.009798 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-03 09:03:25.059459 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
+-rw-r--r--   0        0        0     1940 2023-07-03 09:03:25.059564 prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.010308 prowler_cloud-3.7.1/prowler/providers/aws/services/globalaccelerator/__init__.py
+-rw-r--r--   0        0        0      259 2023-01-13 11:57:06.010414 prowler_cloud-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
+-rw-r--r--   0        0        0     2455 2023-07-03 09:08:09.594472 prowler_cloud-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.010615 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/__init__.py
+-rw-r--r--   0        0        0      185 2023-01-13 11:57:06.010711 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.010811 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-03 09:03:25.059701 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      994 2023-07-03 09:08:09.594606 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.011129 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-03 09:03:25.059819 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      986 2023-07-03 09:08:09.594710 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.011436 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-03 09:03:25.059929 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
+-rw-r--r--   0        0        0      927 2023-07-03 09:08:09.594838 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.011731 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-03 09:03:25.060034 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1408 2023-07-03 09:08:09.594977 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.012003 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1623 2023-07-03 09:03:25.060155 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1399 2023-07-03 09:08:09.595084 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.012296 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1644 2023-07-03 09:03:25.060265 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1369 2023-07-03 09:08:09.595204 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.012552 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1574 2023-07-03 09:03:25.060363 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1664 2023-07-03 09:08:09.595334 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.012802 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-03 09:03:25.060464 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1335 2023-07-03 09:08:09.595546 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013005 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-03 09:03:25.060573 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1326 2023-07-03 09:08:09.595661 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0    10529 2023-07-03 09:08:09.596034 prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013303 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:01.832226 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-03 09:05:01.832316 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
+-rw-r--r--   0        0        0     1221 2023-07-03 09:05:01.832383 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
+-rw-r--r--   0        0        0      210 2023-01-13 11:57:06.013365 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013426 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-03 09:05:01.832500 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1130 2023-07-03 09:03:25.060781 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013652 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-03 09:05:01.832623 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
+-rw-r--r--   0        0        0      961 2023-07-03 09:03:25.060987 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
+-rw-r--r--   0        0        0     7243 2023-07-03 09:08:09.596198 prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013916 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.013993 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-03 09:03:25.061201 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
+-rw-r--r--   0        0        0     1933 2023-01-13 11:57:06.014145 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.014203 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-03 09:03:25.061301 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
+-rw-r--r--   0        0        0     2805 2023-03-06 20:22:13.708943 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:20.350846 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-03 09:05:20.351041 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2227 2023-07-03 09:05:20.351121 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.014401 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
+-rw-r--r--   0        0        0     1494 2023-07-03 09:03:25.061408 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
+-rw-r--r--   0        0        0      802 2023-07-03 09:03:25.061513 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
+-rw-r--r--   0        0        0      180 2023-05-18 13:25:12.964429 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:20.351153 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2088 2023-07-03 09:05:20.351227 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2238 2023-07-03 09:05:20.351288 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:20.351319 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2118 2023-07-03 09:05:20.351411 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2251 2023-07-03 09:05:20.351470 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.014685 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-07-03 09:03:25.061627 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-07-03 09:03:25.061742 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.014906 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-07-03 09:03:25.061841 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4146 2023-07-03 09:03:25.061950 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.015136 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1417 2023-07-03 09:03:25.062065 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-07-03 09:03:25.062167 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.015350 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-03 09:03:25.062308 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
+-rw-r--r--   0        0        0     2665 2023-07-03 09:05:20.351592 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.015601 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
+-rw-r--r--   0        0        0     1707 2023-07-03 09:03:25.062558 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
+-rw-r--r--   0        0        0     1090 2023-01-13 11:57:06.015822 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.015907 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-03 09:03:25.062656 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
+-rw-r--r--   0        0        0     1541 2023-03-06 20:22:13.709581 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.016132 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-03 09:03:25.062777 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
+-rw-r--r--   0        0        0     1414 2023-07-03 09:08:09.596335 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.016350 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-03 09:03:25.062982 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
+-rw-r--r--   0        0        0     1140 2023-07-03 09:08:09.596466 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.016547 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-03 09:03:25.063086 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
+-rw-r--r--   0        0        0     1239 2023-07-03 09:08:09.596604 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.016743 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-03 09:03:25.063184 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
+-rw-r--r--   0        0        0     1149 2023-07-03 09:08:09.596728 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.016927 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
+-rw-r--r--   0        0        0     1280 2023-07-03 09:03:25.063286 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
+-rw-r--r--   0        0        0     1285 2023-07-03 09:08:09.596866 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.017114 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-03 09:03:25.063376 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
+-rw-r--r--   0        0        0     1149 2023-07-03 09:08:09.596992 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.017304 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
+-rw-r--r--   0        0        0     1300 2023-07-03 09:03:25.063484 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
+-rw-r--r--   0        0        0     1137 2023-07-03 09:08:09.597125 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.017492 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-03 09:03:25.063646 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
+-rw-r--r--   0        0        0     6229 2023-07-03 09:05:20.351718 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.017697 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-03 09:03:25.063761 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
+-rw-r--r--   0        0        0     1925 2023-01-13 11:57:06.017860 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.069895 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-03 09:04:49.069999 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
+-rw-r--r--   0        0        0     1967 2023-07-03 09:08:09.597284 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.070121 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-03 09:04:49.070218 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
+-rw-r--r--   0        0        0     1954 2023-07-03 09:08:09.597403 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.597456 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-03 09:08:09.597555 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json
+-rw-r--r--   0        0        0     4380 2023-07-03 09:08:09.597638 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:22:13.710861 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-03 09:08:09.597764 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
+-rw-r--r--   0        0        0     4097 2023-07-12 15:05:15.034320 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.018132 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-03 09:03:25.064263 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-07-03 09:08:09.598024 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.018355 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1738 2023-07-03 09:03:25.064474 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1020 2023-07-03 09:03:25.064579 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.018558 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-03 09:03:25.064698 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
+-rw-r--r--   0        0        0     2832 2023-07-03 09:03:25.064803 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.070324 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
+-rw-r--r--   0        0        0     1335 2023-07-03 09:04:49.070424 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
+-rw-r--r--   0        0        0      901 2023-07-03 09:04:49.070500 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
+-rw-r--r--   0        0        0    24265 2023-07-12 15:05:25.689068 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.018868 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
+-rw-r--r--   0        0        0     1256 2023-07-03 09:03:25.065089 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
+-rw-r--r--   0        0        0      940 2023-07-03 09:04:49.070805 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.019053 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1061 2023-07-03 09:03:25.065220 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1341 2023-07-03 09:03:25.065329 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.019296 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-03 09:03:25.065452 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
+-rw-r--r--   0        0        0     1698 2023-03-06 20:22:13.711919 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.020027 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-03 09:03:25.065583 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
+-rw-r--r--   0        0        0     2671 2023-01-13 11:57:06.020248 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.020370 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-03 09:03:25.065706 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
+-rw-r--r--   0        0        0     1341 2023-03-06 20:22:13.712056 prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.598255 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-03 09:08:09.598420 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.598453 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-03 09:08:09.598539 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
+-rw-r--r--   0        0        0     1498 2023-07-03 09:08:09.598619 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
+-rw-r--r--   0        0        0     4084 2023-07-12 15:05:15.034500 prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.020698 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.020815 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.020913 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-03 09:03:25.065828 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
+-rw-r--r--   0        0        0     1194 2023-07-03 09:03:25.065939 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.021224 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-03 09:03:25.066099 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1294 2023-07-03 09:03:25.066206 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.021544 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-03 09:03:25.066334 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2525 2023-07-03 09:04:49.070954 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0     5417 2023-07-03 09:08:09.598878 prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.022026 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/__init__.py
+-rw-r--r--   0        0        0      190 2023-01-13 11:57:06.022142 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.022257 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-03 09:03:25.066807 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
+-rw-r--r--   0        0        0      982 2023-07-03 09:08:09.599038 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
+-rw-r--r--   0        0        0     1913 2023-07-03 09:08:09.599151 prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.599187 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-03 09:08:09.599264 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.599301 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-03 09:08:09.599386 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json
+-rw-r--r--   0        0        0     1143 2023-07-03 09:08:09.599467 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py
+-rw-r--r--   0        0        0     3581 2023-07-12 15:05:15.034655 prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.022710 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/__init__.py
+-rw-r--r--   0        0        0      238 2023-01-13 11:57:06.022819 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_client.py
+-rw-r--r--   0        0        0     7580 2023-07-03 09:08:09.599685 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.023018 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1124 2023-07-03 09:03:25.067192 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1102 2023-07-03 09:03:25.067291 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.023373 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1478 2023-07-03 09:03:25.067409 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1871 2023-07-03 09:03:25.067522 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.023665 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1555 2023-07-03 09:03:25.067662 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0     1003 2023-07-03 09:03:25.067773 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.023952 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-03 09:03:25.067901 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
+-rw-r--r--   0        0        0      991 2023-07-03 09:03:25.068010 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.024280 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
+-rw-r--r--   0        0        0     1128 2023-07-03 09:03:25.068122 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-07-03 09:03:25.068252 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.024590 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1766 2023-07-03 09:03:25.068366 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-03 09:03:25.068470 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.024901 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-03 09:03:25.068573 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2655 2023-07-03 09:03:25.068679 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.025164 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
+-rw-r--r--   0        0        0     1736 2023-07-03 09:03:25.068793 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
+-rw-r--r--   0        0        0     1046 2023-07-03 09:03:25.068892 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.025381 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
+-rw-r--r--   0        0        0     1242 2023-07-03 09:03:25.069019 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-03 09:03:25.069122 prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.781970 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.782025 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-03 09:04:44.782134 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-03 09:04:49.071107 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
+-rw-r--r--   0        0        0      239 2023-07-03 09:04:44.782293 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.782333 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
+-rw-r--r--   0        0        0     1579 2023-07-03 09:04:44.782434 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
+-rw-r--r--   0        0        0     1816 2023-07-03 09:04:49.071260 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.782548 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-03 09:04:44.782648 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
+-rw-r--r--   0        0        0     5769 2023-07-03 09:08:09.599854 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
+-rw-r--r--   0        0        0     8762 2023-07-03 09:08:09.600053 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.600100 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/__init__.py
+-rw-r--r--   0        0        0     1047 2023-07-03 09:08:09.600204 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json
+-rw-r--r--   0        0        0     1432 2023-07-03 09:08:09.600288 prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.025609 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.025678 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.025751 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-03 09:03:25.069234 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
+-rw-r--r--   0        0        0     1034 2023-07-03 09:08:09.600464 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.025961 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-03 09:03:25.069415 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
+-rw-r--r--   0        0        0     1789 2023-07-03 09:08:09.600604 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.600658 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/__init__.py
+-rw-r--r--   0        0        0     1111 2023-07-12 15:05:15.034798 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json
+-rw-r--r--   0        0        0     1215 2023-07-03 09:08:09.600816 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.026166 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-03 09:03:25.069601 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
+-rw-r--r--   0        0        0     1010 2023-07-03 09:08:09.600928 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.026403 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
+-rw-r--r--   0        0        0     1488 2023-07-03 09:03:25.069821 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
+-rw-r--r--   0        0        0      997 2023-07-03 09:08:09.601046 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.026778 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
+-rw-r--r--   0        0        0     1732 2023-07-03 09:03:25.070029 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
+-rw-r--r--   0        0        0     1019 2023-07-03 09:08:09.601170 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.027012 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-03 09:03:25.070234 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
+-rw-r--r--   0        0        0     1730 2023-07-03 09:08:09.601295 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.027247 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-03 09:03:25.070444 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
+-rw-r--r--   0        0        0     1009 2023-07-03 09:08:09.601423 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.027480 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-03 09:03:25.070690 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
+-rw-r--r--   0        0        0      942 2023-07-03 09:08:09.601590 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:03:25.070880 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-03 09:03:25.070971 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
+-rw-r--r--   0        0        0     1469 2023-07-03 09:08:09.601726 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
+-rw-r--r--   0        0        0    16516 2023-07-03 09:08:09.601873 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.027811 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-03 09:03:25.071503 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
+-rw-r--r--   0        0        0     1635 2023-07-03 09:08:09.602006 prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.028032 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/__init__.py
+-rw-r--r--   0        0        0      205 2023-01-13 11:57:06.028116 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.028186 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-03 09:03:25.071765 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
+-rw-r--r--   0        0        0      973 2023-07-03 09:03:25.071864 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.028441 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
+-rw-r--r--   0        0        0     1204 2023-07-03 09:03:25.071981 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-03 09:03:25.072092 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.028689 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-03 09:08:09.602150 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
+-rw-r--r--   0        0        0      996 2023-07-03 09:03:25.072333 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.028927 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
+-rw-r--r--   0        0        0     1297 2023-07-03 09:03:25.072487 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
+-rw-r--r--   0        0        0      992 2023-07-03 09:03:25.072640 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
+-rw-r--r--   0        0        0     5144 2023-07-03 09:08:09.602272 prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.071414 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-03 09:04:49.071489 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:49.071520 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-03 09:04:49.071604 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
+-rw-r--r--   0        0        0     1089 2023-07-03 09:08:09.602417 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
+-rw-r--r--   0        0        0     2339 2023-07-12 15:05:15.034929 prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.029220 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/__init__.py
+-rw-r--r--   0        0        0      200 2023-01-13 11:57:06.029290 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.602629 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-03 09:08:09.602726 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json
+-rw-r--r--   0        0        0     2927 2023-07-03 09:08:09.602815 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.029374 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-03 09:03:25.072883 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-03 09:03:25.072986 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.029636 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-03 09:03:25.073105 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
+-rw-r--r--   0        0        0     1058 2023-07-03 09:03:25.073201 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.029862 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-03 09:03:25.073323 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1303 2023-07-03 09:08:09.602946 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0     8575 2023-07-03 09:08:09.603081 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_service.py
+-rw-r--r--   0        0        0      221 2023-01-13 11:57:06.030245 prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53domains_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.030316 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.030411 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-03 09:03:25.073706 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
+-rw-r--r--   0        0        0     1128 2023-07-03 09:08:09.603232 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.030639 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-03 09:03:25.073830 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
+-rw-r--r--   0        0        0      957 2023-07-03 09:03:25.073934 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.031224 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-03 09:03:25.074056 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
+-rw-r--r--   0        0        0      917 2023-07-03 09:03:25.074167 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:03:25.074223 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-03 09:03:25.074330 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
+-rw-r--r--   0        0        0     1123 2023-07-03 09:04:44.783107 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.031639 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-03 09:03:25.074522 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
+-rw-r--r--   0        0        0      943 2023-07-03 09:03:25.074620 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.603273 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-03 09:08:09.603356 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json
+-rw-r--r--   0        0        0      944 2023-07-03 09:08:09.604158 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.032078 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-03 09:03:25.074737 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
+-rw-r--r--   0        0        0      947 2023-07-03 09:03:25.074830 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.032575 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-03 09:03:25.074939 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
+-rw-r--r--   0        0        0     1716 2023-07-03 09:03:25.075038 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.032908 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1939 2023-07-03 09:03:25.075142 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0     4078 2023-07-03 09:08:09.604291 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.033201 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
+-rw-r--r--   0        0        0     1190 2023-07-03 09:03:25.075342 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
+-rw-r--r--   0        0        0     2099 2023-07-03 09:03:25.075434 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.033620 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1372 2023-07-03 09:03:25.075534 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      978 2023-07-03 09:03:25.075637 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
+-rw-r--r--   0        0        0      175 2023-01-13 11:57:06.033910 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_client.py
+-rw-r--r--   0        0        0    17497 2023-07-03 09:08:09.604442 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_service.py
+-rw-r--r--   0        0        0      196 2023-01-13 11:57:06.034147 prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3control_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.034211 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/__init__.py
+-rw-r--r--   0        0        0      210 2023-01-13 11:57:06.034277 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.034342 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-03 09:03:25.075877 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0      945 2023-07-03 09:03:25.075975 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.034554 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-03 09:03:25.076110 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0      966 2023-07-03 09:03:25.076227 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.034769 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1412 2023-07-03 09:03:25.076356 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1046 2023-07-03 09:03:25.076450 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.035011 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-03 09:03:25.076551 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-07-03 09:03:25.076660 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.035240 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1361 2023-07-03 09:03:25.076788 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1063 2023-07-03 09:03:25.076898 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.035492 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
+-rw-r--r--   0        0        0     1524 2023-07-03 09:03:25.077021 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
+-rw-r--r--   0        0        0     1091 2023-07-03 09:03:25.077109 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
+-rw-r--r--   0        0        0    11611 2023-07-03 09:08:09.604604 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.035801 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1119 2023-07-03 09:03:25.077333 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1040 2023-07-03 09:03:25.077425 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.036016 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-03 09:03:25.077529 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-07-03 09:03:25.077621 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.036223 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-03 09:03:25.077720 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1042 2023-07-03 09:03:25.077806 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.036491 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-03 09:03:25.077902 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1072 2023-07-03 09:03:25.077997 prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.036744 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.036825 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-03 09:04:44.783359 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1054 2023-07-03 09:03:25.078224 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
+-rw-r--r--   0        0        0      244 2023-01-13 11:57:06.037033 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
+-rw-r--r--   0        0        0     2529 2023-07-03 09:08:09.604744 prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.037186 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/__init__.py
+-rw-r--r--   0        0        0      220 2023-01-13 11:57:06.037261 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.037333 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-03 09:03:25.078425 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
+-rw-r--r--   0        0        0     1296 2023-03-06 20:22:13.715546 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
+-rw-r--r--   0        0        0     4490 2023-03-06 20:22:13.715680 prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.037616 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.037713 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-03 09:03:25.078537 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
+-rw-r--r--   0        0        0     1259 2023-07-03 09:03:25.078649 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.037981 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1045 2023-07-03 09:03:25.078746 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1267 2023-07-03 09:03:25.078848 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.038259 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
+-rw-r--r--   0        0        0     1041 2023-07-03 09:03:25.078955 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
+-rw-r--r--   0        0        0     1316 2023-07-03 09:03:25.079054 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.038469 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
+-rw-r--r--   0        0        0     1021 2023-07-03 09:03:25.079156 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
+-rw-r--r--   0        0        0     1271 2023-01-13 11:57:06.038627 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.038703 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-03 09:03:25.079250 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1353 2023-07-03 09:03:25.079345 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.038960 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-03 09:03:25.079445 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
+-rw-r--r--   0        0        0     1275 2023-07-03 09:03:25.079540 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
+-rw-r--r--   0        0        0      195 2023-01-13 11:57:06.039175 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_client.py
+-rw-r--r--   0        0        0     2527 2023-03-06 20:22:13.715805 prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.039319 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.039393 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_client.py
+-rw-r--r--   0        0        0     3814 2023-07-03 09:03:25.079668 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.039544 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-03 09:03:25.079776 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-07-03 09:03:25.079877 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.039780 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1340 2023-07-03 09:03:25.079991 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1938 2023-07-03 09:08:09.604874 prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.040032 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.040107 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.040185 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1396 2023-07-03 09:03:25.080175 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2245 2023-07-12 15:05:25.689886 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.040516 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-03 09:03:25.080380 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      939 2023-07-03 09:03:25.080470 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
+-rw-r--r--   0        0        0     4417 2023-07-03 09:08:09.605001 prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.040905 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-24 12:09:01.660799 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.041088 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-03 09:03:25.080668 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
+-rw-r--r--   0        0        0     1974 2023-07-03 09:03:25.080790 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.041349 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
+-rw-r--r--   0        0        0     1142 2023-07-03 09:03:25.080916 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
+-rw-r--r--   0        0        0      884 2023-07-03 09:03:25.081024 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.041620 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-03 09:03:25.081143 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
+-rw-r--r--   0        0        0      993 2023-07-03 09:03:25.081251 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
+-rw-r--r--   0        0        0     7698 2023-07-03 09:08:09.605125 prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.313735 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-03 09:05:11.313804 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.313834 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-03 09:08:09.605263 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
+-rw-r--r--   0        0        0     1487 2023-07-03 09:08:09.605382 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
+-rw-r--r--   0        0        0     6856 2023-07-12 15:05:15.035066 prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.042019 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/__init__.py
+-rw-r--r--   0        0        0      244 2023-01-13 11:57:06.042118 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.042204 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
+-rw-r--r--   0        0        0     1132 2023-07-03 09:03:25.081520 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
+-rw-r--r--   0        0        0     1478 2023-07-03 09:08:09.605644 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
+-rw-r--r--   0        0        0     3575 2023-07-12 15:05:15.035197 prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.042656 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.042739 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.314117 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
+-rw-r--r--   0        0        0      945 2023-07-03 09:08:09.605922 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
+-rw-r--r--   0        0        0     1010 2023-07-03 09:08:09.606027 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.042814 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-03 09:03:25.081658 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     3410 2023-07-03 09:08:09.606182 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.043059 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-03 09:03:25.081920 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     2222 2023-07-03 09:08:09.606304 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.043266 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-03 09:03:25.082197 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      800 2023-07-03 09:08:09.606425 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.043476 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-03 09:03:25.082427 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
+-rw-r--r--   0        0        0     1497 2023-07-03 09:08:09.606545 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
+-rw-r--r--   0        0        0    16958 2023-07-12 15:05:15.035332 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.314491 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
+-rw-r--r--   0        0        0      988 2023-07-03 09:08:09.606801 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
+-rw-r--r--   0        0        0     1327 2023-07-03 09:08:09.606905 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.606951 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-03 09:08:09.607047 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json
+-rw-r--r--   0        0        0     1086 2023-07-03 09:08:09.607112 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:05:11.314758 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
+-rw-r--r--   0        0        0      967 2023-07-03 09:08:09.607252 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
+-rw-r--r--   0        0        0     1483 2023-07-03 09:08:09.607364 prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.043779 prowler_cloud-3.7.1/prowler/providers/aws/services/waf/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.043840 prowler_cloud-3.7.1/prowler/providers/aws/services/waf/waf_client.py
+-rw-r--r--   0        0        0     2645 2023-03-06 20:22:13.717290 prowler_cloud-3.7.1/prowler/providers/aws/services/waf/waf_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.043965 prowler_cloud-3.7.1/prowler/providers/aws/services/wafv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-01-13 11:57:06.044033 prowler_cloud-3.7.1/prowler/providers/aws/services/wafv2/wafv2_client.py
+-rw-r--r--   0        0        0     2724 2023-03-06 20:22:13.717476 prowler_cloud-3.7.1/prowler/providers/aws/services/wafv2/wafv2_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.607415 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-03 09:08:09.607547 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_client.py
+-rw-r--r--   0        0        0     2972 2023-07-03 09:08:09.607647 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.607702 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-03 09:08:09.607805 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json
+-rw-r--r--   0        0        0     1090 2023-07-03 09:08:09.607884 prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.044201 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-24 10:37:33.271310 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_client.py
+-rw-r--r--   0        0        0     3821 2023-07-03 09:08:09.608006 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.044403 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-03 09:03:25.082902 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-07-03 09:03:25.083015 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.608047 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/__init__.py
+-rw-r--r--   0        0        0     1371 2023-07-03 09:08:09.608127 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json
+-rw-r--r--   0        0        0     2344 2023-07-03 09:08:09.608204 prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.044616 prowler_cloud-3.7.1/prowler/providers/azure/__init__.py
+-rw-r--r--   0        0        0     8818 2023-07-03 09:08:09.608350 prowler_cloud-3.7.1/prowler/providers/azure/azure_provider.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.044810 prowler_cloud-3.7.1/prowler/providers/azure/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      258 2023-03-06 20:22:13.718157 prowler_cloud-3.7.1/prowler/providers/azure/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      796 2023-07-03 09:04:49.072042 prowler_cloud-3.7.1/prowler/providers/azure/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.045058 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/__init__.py
+-rw-r--r--   0        0        0      205 2023-01-13 11:57:06.045122 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.045185 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-03 09:03:25.083188 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
+-rw-r--r--   0        0        0     1182 2023-07-03 09:04:44.783769 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.045433 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
+-rw-r--r--   0        0        0      926 2023-07-03 09:03:25.083307 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
+-rw-r--r--   0        0        0     1121 2023-07-03 09:04:44.783897 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.045640 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1654 2023-07-03 09:03:25.083428 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1210 2023-07-03 09:04:44.784019 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.045846 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-03 09:03:25.083543 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
+-rw-r--r--   0        0        0     1181 2023-07-03 09:04:44.784132 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.046090 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
+-rw-r--r--   0        0        0     1306 2023-07-03 09:03:25.083660 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-07-03 09:04:44.784231 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.046313 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-03 09:03:25.083786 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1638 2023-07-03 09:04:44.784326 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.046517 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-03 09:03:25.083907 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
+-rw-r--r--   0        0        0     1122 2023-07-03 09:04:44.784423 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.046771 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
+-rw-r--r--   0        0        0     1590 2023-07-03 09:03:25.084029 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-07-03 09:04:44.784535 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.046995 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1187 2023-07-03 09:03:25.084193 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1346 2023-07-03 09:04:44.784665 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.047329 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
+-rw-r--r--   0        0        0     1509 2023-07-03 09:03:25.084316 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
+-rw-r--r--   0        0        0     1170 2023-07-03 09:04:44.784802 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.047565 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
+-rw-r--r--   0        0        0     1751 2023-07-03 09:03:25.084460 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
+-rw-r--r--   0        0        0     1227 2023-07-03 09:04:44.785154 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.047787 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
+-rw-r--r--   0        0        0     1693 2023-07-03 09:03:25.084596 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
+-rw-r--r--   0        0        0     1202 2023-07-03 09:04:44.785262 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
+-rw-r--r--   0        0        0     2326 2023-07-03 09:04:49.072155 prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.048061 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/__init__.py
+-rw-r--r--   0        0        0      180 2023-01-13 11:57:06.048123 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_client.py
+-rw-r--r--   0        0        0     2696 2023-07-03 09:04:49.072269 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.048253 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-03 09:03:25.084733 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
+-rw-r--r--   0        0        0     1330 2023-01-13 11:57:06.048389 prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.048452 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.048538 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
+-rw-r--r--   0        0        0     1470 2023-07-03 09:03:25.084876 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-01-13 11:57:06.048703 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
+-rw-r--r--   0        0        0      200 2023-01-13 11:57:06.048764 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_client.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.048833 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-03 09:03:25.084988 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
+-rw-r--r--   0        0        0     1179 2023-01-13 11:57:06.048984 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.049053 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1765 2023-07-03 09:03:25.085111 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1265 2023-01-13 11:57:06.049182 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.049254 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-03 09:03:25.085246 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1156 2023-01-13 11:57:06.049424 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.049513 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
+-rw-r--r--   0        0        0     1246 2023-07-03 09:03:25.085379 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
+-rw-r--r--   0        0        0     1151 2023-01-13 11:57:06.049679 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.049761 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-03 09:03:25.085508 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1169 2023-01-13 11:57:06.049954 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.050038 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-03 09:03:25.085666 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-01-13 11:57:06.050222 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
+-rw-r--r--   0        0        0     3651 2023-07-03 09:04:49.072386 prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_service.py
+-rw-r--r--   0        0        0        0 2023-01-13 11:57:06.050386 prowler_cloud-3.7.1/prowler/providers/common/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-03 09:03:25.085739 prowler_cloud-3.7.1/prowler/providers/common/allowlist.py
+-rw-r--r--   0        0        0    15670 2023-07-03 09:08:09.608524 prowler_cloud-3.7.1/prowler/providers/common/audit_info.py
+-rw-r--r--   0        0        0      251 2023-03-06 20:22:13.718850 prowler_cloud-3.7.1/prowler/providers/common/models.py
+-rw-r--r--   0        0        0     4669 2023-07-03 09:08:09.608636 prowler_cloud-3.7.1/prowler/providers/common/outputs.py
+-rw-r--r--   0        0        0      837 2023-07-03 09:08:09.608746 prowler_cloud-3.7.1/prowler/providers/common/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.785531 prowler_cloud-3.7.1/prowler/providers/gcp/__init__.py
+-rw-r--r--   0        0        0     3468 2023-07-03 09:08:09.608881 prowler_cloud-3.7.1/prowler/providers/gcp/gcp_provider.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.785650 prowler_cloud-3.7.1/prowler/providers/gcp/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-03 09:08:09.609007 prowler_cloud-3.7.1/prowler/providers/gcp/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      683 2023-07-03 09:08:09.609104 prowler_cloud-3.7.1/prowler/providers/gcp/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.609152 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.609207 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/__init__.py
+-rw-r--r--   0        0        0     1751 2023-07-03 09:08:09.609301 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json
+-rw-r--r--   0        0        0     1135 2023-07-12 15:05:15.036045 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py
+-rw-r--r--   0        0        0      192 2023-07-03 09:08:09.609478 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.036091 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/__init__.py
+-rw-r--r--   0        0        0     1446 2023-07-12 15:05:15.036193 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json
+-rw-r--r--   0        0        0      912 2023-07-12 15:05:15.036315 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.609516 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/__init__.py
+-rw-r--r--   0        0        0     1700 2023-07-03 09:08:09.609602 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json
+-rw-r--r--   0        0        0     1103 2023-07-12 15:05:15.036611 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py
+-rw-r--r--   0        0        0     2054 2023-07-12 15:05:15.036831 prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.785853 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-03 09:04:44.785916 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.785974 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-03 09:04:44.786054 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      988 2023-07-03 09:08:09.609906 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.786177 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-03 09:04:44.786262 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
+-rw-r--r--   0        0        0      968 2023-07-12 15:05:15.037000 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
+-rw-r--r--   0        0        0     4484 2023-07-03 09:08:09.610147 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.786453 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-03 09:04:44.786555 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      964 2023-07-03 09:08:09.610257 prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.786647 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-03 09:04:44.786724 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
+-rw-r--r--   0        0        0     2408 2023-07-12 15:05:15.037142 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.786859 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-03 09:04:44.786928 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.786984 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-03 09:04:44.787058 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
+-rw-r--r--   0        0        0     1004 2023-07-03 09:08:09.610547 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.787167 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-03 09:04:44.787260 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
+-rw-r--r--   0        0        0     1175 2023-07-03 09:08:09.610707 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.787407 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
+-rw-r--r--   0        0        0     1216 2023-07-03 09:04:44.787493 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
+-rw-r--r--   0        0        0     1196 2023-07-03 09:08:09.610831 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.787612 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
+-rw-r--r--   0        0        0     2058 2023-07-03 09:04:44.787694 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
+-rw-r--r--   0        0        0     1295 2023-07-03 09:08:09.610963 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.787812 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-03 09:04:44.787884 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1200 2023-07-03 09:08:09.611105 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788003 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
+-rw-r--r--   0        0        0     1447 2023-07-03 09:04:44.788084 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
+-rw-r--r--   0        0        0     1212 2023-07-03 09:08:09.611222 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788202 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-03 09:04:44.788287 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
+-rw-r--r--   0        0        0     1303 2023-07-03 09:08:09.611350 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788399 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-12 15:05:15.037477 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1316 2023-07-03 09:08:09.611474 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788590 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1955 2023-07-03 09:04:44.788673 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1459 2023-07-03 09:08:09.611595 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788783 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-03 09:04:44.788871 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
+-rw-r--r--   0        0        0     1403 2023-07-03 09:08:09.611713 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.788987 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-03 09:04:44.789065 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1361 2023-07-03 09:08:09.611836 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.789184 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
+-rw-r--r--   0        0        0     1151 2023-07-03 09:04:44.789270 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
+-rw-r--r--   0        0        0     1097 2023-07-03 09:08:09.611955 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.789405 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
+-rw-r--r--   0        0        0     1492 2023-07-03 09:04:44.789488 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
+-rw-r--r--   0        0        0     1039 2023-07-03 09:08:09.612088 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.789616 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1319 2023-07-03 09:04:44.789708 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-03 09:08:09.612194 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.790982 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-03 09:04:44.791064 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
+-rw-r--r--   0        0        0     1343 2023-07-03 09:08:09.612309 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.791187 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
+-rw-r--r--   0        0        0     1702 2023-07-03 09:04:44.791276 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
+-rw-r--r--   0        0        0     1225 2023-07-03 09:08:09.612409 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.791390 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-03 09:04:44.791467 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
+-rw-r--r--   0        0        0     1312 2023-07-03 09:08:09.612515 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.791584 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
+-rw-r--r--   0        0        0     1860 2023-07-03 09:04:44.791664 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
+-rw-r--r--   0        0        0     1194 2023-07-03 09:08:09.612625 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.791776 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
+-rw-r--r--   0        0        0     2002 2023-07-03 09:04:44.791857 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
+-rw-r--r--   0        0        0     1183 2023-07-03 09:08:09.612733 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.791970 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-03 09:04:44.792047 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1203 2023-07-03 09:08:09.612857 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.792164 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-03 09:04:44.792242 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
+-rw-r--r--   0        0        0     1172 2023-07-03 09:08:09.612952 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.792358 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
+-rw-r--r--   0        0        0     1428 2023-07-03 09:04:44.792439 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
+-rw-r--r--   0        0        0      970 2023-07-03 09:08:09.613059 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
+-rw-r--r--   0        0        0     2723 2023-07-03 09:08:09.613164 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.792660 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.037527 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-12 15:05:15.037785 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json
+-rw-r--r--   0        0        0     1638 2023-07-12 15:05:15.038039 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.792756 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-03 09:04:44.792833 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0      913 2023-07-03 09:08:09.613270 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.792972 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
+-rw-r--r--   0        0        0     1270 2023-07-03 09:04:44.793061 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
+-rw-r--r--   0        0        0     1054 2023-07-03 09:08:09.613423 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
+-rw-r--r--   0        0        0      226 2023-07-03 09:04:44.793200 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
+-rw-r--r--   0        0        0     2493 2023-07-12 15:05:15.038265 prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.793332 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-03 09:04:44.793418 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.038315 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-12 15:05:15.038436 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json
+-rw-r--r--   0        0        0     1987 2023-07-12 15:05:15.038560 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.038607 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/__init__.py
+-rw-r--r--   0        0        0     2451 2023-07-12 15:05:15.038704 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json
+-rw-r--r--   0        0        0     1977 2023-07-12 15:05:15.038828 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.038866 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-12 15:05:15.038970 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json
+-rw-r--r--   0        0        0     1284 2023-07-12 15:05:15.039044 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.039078 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/__init__.py
+-rw-r--r--   0        0        0     2383 2023-07-12 15:05:15.039176 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-07-12 15:05:15.039261 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.039305 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-12 15:05:15.039404 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json
+-rw-r--r--   0        0        0     1266 2023-07-12 15:05:15.039491 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.039533 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/__init__.py
+-rw-r--r--   0        0        0     2091 2023-07-12 15:05:15.039647 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json
+-rw-r--r--   0        0        0     1443 2023-07-12 15:05:15.039717 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.039751 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-12 15:05:15.039838 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json
+-rw-r--r--   0        0        0     1082 2023-07-12 15:05:15.039903 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.039937 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/__init__.py
+-rw-r--r--   0        0        0     2358 2023-07-12 15:05:15.040029 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1043 2023-07-12 15:05:15.040090 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.793517 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-03 09:04:44.793588 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      891 2023-07-03 09:08:09.614844 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.040126 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-12 15:05:15.040223 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json
+-rw-r--r--   0        0        0     1267 2023-07-12 15:05:15.040347 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.040390 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-12 15:05:15.040494 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-07-12 15:05:15.040573 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.040611 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1508 2023-07-12 15:05:15.040712 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      930 2023-07-12 15:05:15.040801 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.793730 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
+-rw-r--r--   0        0        0     1132 2023-07-03 09:04:44.793815 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
+-rw-r--r--   0        0        0     1551 2023-07-03 09:08:09.615174 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.040840 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-12 15:05:15.040942 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1181 2023-07-12 15:05:15.041017 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.041053 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/__init__.py
+-rw-r--r--   0        0        0     2085 2023-07-12 15:05:15.041148 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json
+-rw-r--r--   0        0        0      889 2023-07-12 15:05:15.041218 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.041254 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/__init__.py
+-rw-r--r--   0        0        0     1897 2023-07-12 15:05:15.041345 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json
+-rw-r--r--   0        0        0      881 2023-07-12 15:05:15.041408 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py
+-rw-r--r--   0        0        0    12640 2023-07-12 15:05:15.041601 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.041639 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     2121 2023-07-12 15:05:15.041730 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      949 2023-07-12 15:05:15.041801 prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616102 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-03 09:08:09.616187 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616219 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/__init__.py
+-rw-r--r--   0        0        0     2301 2023-07-03 09:08:09.616315 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json
+-rw-r--r--   0        0        0      975 2023-07-03 09:08:09.616397 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py
+-rw-r--r--   0        0        0     2316 2023-07-03 09:08:09.616459 prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616488 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-03 09:08:09.616550 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616581 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/__init__.py
+-rw-r--r--   0        0        0     1818 2023-07-03 09:08:09.616657 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json
+-rw-r--r--   0        0        0      938 2023-07-12 15:05:15.041964 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616757 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/__init__.py
+-rw-r--r--   0        0        0     1826 2023-07-03 09:08:09.616837 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json
+-rw-r--r--   0        0        0     1117 2023-07-03 09:08:09.616898 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.616930 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/__init__.py
+-rw-r--r--   0        0        0     1829 2023-07-03 09:08:09.617001 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json
+-rw-r--r--   0        0        0     1121 2023-07-03 09:08:09.617055 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py
+-rw-r--r--   0        0        0     3394 2023-07-12 15:05:15.042086 prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.794002 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-12 15:05:15.042166 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/accessapproval_client.py
+-rw-r--r--   0        0        0      214 2023-07-12 15:05:15.042231 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/essentialcontacts_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.042268 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/__init__.py
+-rw-r--r--   0        0        0     2590 2023-07-12 15:05:15.042364 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json
+-rw-r--r--   0        0        0      972 2023-07-12 15:05:15.042456 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.042501 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1997 2023-07-12 15:05:15.042607 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      963 2023-07-12 15:05:15.042684 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py
+-rw-r--r--   0        0        0      172 2023-07-03 09:04:44.794083 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:08:09.617154 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/__init__.py
+-rw-r--r--   0        0        0     2294 2023-07-03 09:08:09.617248 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json
+-rw-r--r--   0        0        0     1674 2023-07-12 15:05:25.690397 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.042938 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-12 15:05:15.043032 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json
+-rw-r--r--   0        0        0     1040 2023-07-12 15:05:15.043102 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.043139 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/__init__.py
+-rw-r--r--   0        0        0     2135 2023-07-12 15:05:15.043249 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json
+-rw-r--r--   0        0        0     1857 2023-07-12 15:05:15.043318 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.043353 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/__init__.py
+-rw-r--r--   0        0        0     2235 2023-07-12 15:05:15.043437 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json
+-rw-r--r--   0        0        0     1469 2023-07-12 15:05:15.043512 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.794152 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-03 09:04:44.794232 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     1392 2023-07-03 09:08:09.617459 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.794348 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-03 09:04:44.794437 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1035 2023-07-03 09:08:09.617561 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.794586 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-03 09:04:44.794688 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
+-rw-r--r--   0        0        0     1314 2023-07-03 09:08:09.617661 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
+-rw-r--r--   0        0        0     6222 2023-07-12 15:05:15.043651 prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.794915 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-03 09:04:44.794995 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.795067 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1195 2023-07-03 09:04:44.795202 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0      993 2023-07-03 09:08:09.617866 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.795362 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-07-03 09:04:44.795466 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1128 2023-07-03 09:08:09.617967 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
+-rw-r--r--   0        0        0     5395 2023-07-03 09:08:09.618056 prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.795690 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-03 09:04:44.795776 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.795851 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1438 2023-07-03 09:04:44.795970 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2234 2023-07-03 09:08:09.618192 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.796147 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1243 2023-07-03 09:04:44.796256 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2209 2023-07-03 09:08:09.618299 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.796460 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-03 09:04:44.796553 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2328 2023-07-03 09:08:09.618416 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.796712 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1589 2023-07-12 15:05:15.043807 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2526 2023-07-03 09:08:09.618639 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.796963 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-03 09:04:44.797056 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2145 2023-07-03 09:08:09.618743 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.797248 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-07-03 09:04:44.797329 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2324 2023-07-03 09:08:09.618841 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.797475 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1113 2023-07-03 09:04:44.797576 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2426 2023-07-03 09:08:09.618939 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.797749 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1157 2023-07-03 09:04:44.797832 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2257 2023-07-03 09:08:09.619044 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
+-rw-r--r--   0        0        0     3047 2023-07-03 09:08:09.619142 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.798054 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-03 09:04:44.798126 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
+-rw-r--r--   0        0        0     1633 2023-07-03 09:08:09.619254 prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:04:44.798269 prowler_cloud-3.7.1/prowler/providers/gcp/services/monitoring/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-03 09:04:44.798338 prowler_cloud-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_client.py
+-rw-r--r--   0        0        0     2125 2023-07-03 09:08:09.619365 prowler_cloud-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.043848 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-12 15:05:15.043938 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:05:15.043981 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/__init__.py
+-rw-r--r--   0        0        0     1904 2023-07-12 15:05:15.044083 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json
+-rw-r--r--   0        0        0     1266 2023-07-12 15:05:15.044151 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py
+-rw-r--r--   0        0        0     1821 2023-07-12 15:05:15.044257 prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_service.py
+-rw-r--r--   0        0        0     2497 2023-07-12 15:15:05.071387 prowler_cloud-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0    51589 1970-01-01 00:00:00.000000 prowler_cloud-3.7.1/setup.py
+-rw-r--r--   0        0        0    15677 1970-01-01 00:00:00.000000 prowler_cloud-3.7.1/PKG-INFO
```

### Comparing `prowler_cloud-3.7.0/LICENSE` & `prowler_cloud-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/README.md` & `prowler_cloud-3.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 `Prowler` is an Open Source security tool to perform AWS, GCP and Azure security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness.
 
 It contains hundreds of controls covering CIS, NIST 800, NIST CSF, CISA, RBI, FedRAMP, PCI-DSS, GDPR, HIPAA, FFIEC, SOC2, GXP, AWS Well-Architected Framework Security Pillar, AWS Foundational Technical Review (FTR), ENS (Spainish National Security Schema) and your custom security frameworks.
 
 | Provider | Checks | Services | [Compliance Frameworks](https://docs.prowler.cloud/en/latest/tutorials/compliance/) | [Categories](https://docs.prowler.cloud/en/latest/tutorials/misc/#categories) |
 |---|---|---|---|---|
-| AWS | 283 | 55 -> `prowler aws --list-services` | 21 -> `prowler aws --list-compliance` | 5 -> `prowler aws --list-categories` |
+| AWS | 283 | 55 -> `prowler aws --list-services` | 25 -> `prowler aws --list-compliance` | 5 -> `prowler aws --list-categories` |
 | GCP | 73 | 11 -> `prowler gcp --list-services` | 1 -> `prowler gcp --list-compliance` | 0 -> `prowler gcp --list-categories`|
 | Azure | 20 | 3 -> `prowler azure --list-services` | CIS soon | 1 -> `prowler azure --list-categories` |
 | Kubernetes | Planned | - | - | - |
 
 # 📖 Documentation
 
 The full documentation can now be found at [https://docs.prowler.cloud](https://docs.prowler.cloud)
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 of controls covering CIS, NIST 800, NIST CSF, CISA, RBI, FedRAMP, PCI-DSS,
 GDPR, HIPAA, FFIEC, SOC2, GXP, AWS Well-Architected Framework Security Pillar,
 AWS Foundational Technical Review (FTR), ENS (Spainish National Security
 Schema) and your custom security frameworks. | Provider | Checks | Services |
 [Compliance Frameworks](https://docs.prowler.cloud/en/latest/tutorials/
 compliance/) | [Categories](https://docs.prowler.cloud/en/latest/tutorials/
 misc/#categories) | |---|---|---|---|---| | AWS | 283 | 55 -> `prowler aws --
-list-services` | 21 -> `prowler aws --list-compliance` | 5 -> `prowler aws --
+list-services` | 25 -> `prowler aws --list-compliance` | 5 -> `prowler aws --
 list-categories` | | GCP | 73 | 11 -> `prowler gcp --list-services` | 1 -
 > `prowler gcp --list-compliance` | 0 -> `prowler gcp --list-categories`| |
 Azure | 20 | 3 -> `prowler azure --list-services` | CIS soon | 1 -> `prowler
 azure --list-categories` | | Kubernetes | Planned | - | - | - | # ð
 Documentation The full documentation can now be found at [https://
 docs.prowler.cloud](https://docs.prowler.cloud) ## Looking for Prowler v2
 documentation? For Prowler v2 Documentation, please go to https://github.com/
```

### Comparing `prowler_cloud-3.7.0/prowler/__main__.py` & `prowler_cloud-3.7.1/prowler/__main__.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/cis_1.4_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/cis_1.4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/cis_1.5_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/cis_1.5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/cisa_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/cisa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/ens_rd2022_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/ens_rd2022_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/ffiec_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/ffiec_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/gdpr_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/gdpr_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/hipaa_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/hipaa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/iso27001_2013_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/iso27001_2013_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/mitre_attack_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/mitre_attack_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/nist_csf_1.1_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/nist_csf_1.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/pci_3.2.1_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/pci_3.2.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/aws/soc2_aws.json` & `prowler_cloud-3.7.1/prowler/compliance/aws/soc2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/compliance/gcp/cis_2.0_gcp.json` & `prowler_cloud-3.7.1/prowler/compliance/gcp/cis_2.0_gcp.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/config/allowlist.yaml` & `prowler_cloud-3.7.1/prowler/config/allowlist.yaml`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/config/config.py` & `prowler_cloud-3.7.1/prowler/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 import yaml
 
 from prowler.lib.logger import logger
 
 timestamp = datetime.today()
 timestamp_utc = datetime.now(timezone.utc).replace(tzinfo=timezone.utc)
-prowler_version = "3.7.0"
+prowler_version = "3.7.1"
 boto3_user_agent_extra = "APN_1826889"
 html_logo_url = "https://github.com/prowler-cloud/prowler/"
 html_logo_img = "https://user-images.githubusercontent.com/3985464/113734260-7ba06900-96fb-11eb-82bc-d4f68a1e2710.png"
 square_logo_img = "https://user-images.githubusercontent.com/38561120/235905862-9ece5bd7-9aa3-4e48-807a-3a9035eb8bfb.png"
 aws_logo = "https://user-images.githubusercontent.com/38561120/235953920-3e3fba08-0795-41dc-b480-9bea57db9f2e.png"
 azure_logo = "https://user-images.githubusercontent.com/38561120/235927375-b23e2e0f-8932-49ec-b59c-d89f61c8041d.png"
 gcp_logo = "https://user-images.githubusercontent.com/38561120/235928332-eb4accdc-c226-4391-8e97-6ca86a91cf50.png"
```

### Comparing `prowler_cloud-3.7.0/prowler/config/config.yaml` & `prowler_cloud-3.7.1/prowler/config/config.yaml`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/banner.py` & `prowler_cloud-3.7.1/prowler/lib/banner.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/check/check.py` & `prowler_cloud-3.7.1/prowler/lib/check/check.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/check/checks_loader.py` & `prowler_cloud-3.7.1/prowler/lib/check/checks_loader.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/check/compliance.py` & `prowler_cloud-3.7.1/prowler/lib/check/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/check/compliance_models.py` & `prowler_cloud-3.7.1/prowler/lib/check/compliance_models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/check/models.py` & `prowler_cloud-3.7.1/prowler/lib/check/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/cli/parser.py` & `prowler_cloud-3.7.1/prowler/lib/cli/parser.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/logger.py` & `prowler_cloud-3.7.1/prowler/lib/logger.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/compliance.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/file_descriptors.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/file_descriptors.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/html.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/html.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/json.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/json.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/models.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/outputs.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/slack.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/slack.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/outputs/summary_table.py` & `prowler_cloud-3.7.1/prowler/lib/outputs/summary_table.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/scan_filters/scan_filters.py` & `prowler_cloud-3.7.1/prowler/lib/scan_filters/scan_filters.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/lib/utils/utils.py` & `prowler_cloud-3.7.1/prowler/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/aws_provider.py` & `prowler_cloud-3.7.1/prowler/providers/aws/aws_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/aws_regions_by_service.json` & `prowler_cloud-3.7.1/prowler/providers/aws/aws_regions_by_service.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999173280423279%*

 * *Differences: {"'services'": "{'internetmonitor': {'regions': {'aws': {insert: [(4, 'ap-northeast-3'), (6, "*

 * *               "'ap-south-2'), (9, 'ap-southeast-3'), (10, 'ap-southeast-4'), (13, "*

 * *               "'eu-central-2'), (16, 'eu-south-2'), (20, 'me-central-1')]}}}, 'network-firewall': "*

 * *               "{'regions': {'aws': {insert: [(6, 'ap-south-2'), (10, 'ap-southeast-4'), (13, "*

 * *               "'eu-central-2'), (16, 'eu-south-2')]}}}, 'savingsplans': {'regions': {'aws-cn': "*

 * *               "['cn-north-1', 'cn-no […]*

```diff
@@ -4625,24 +4625,31 @@
         "internetmonitor": {
             "regions": {
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
+                    "ap-northeast-3",
                     "ap-south-1",
+                    "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
+                    "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
+                    "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
+                    "eu-south-2",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
+                    "me-central-1",
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
@@ -6460,21 +6467,25 @@
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
+                    "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
+                    "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
+                    "eu-south-2",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
                     "me-central-1",
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
@@ -8089,15 +8100,18 @@
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
-                "aws-cn": [],
+                "aws-cn": [
+                    "cn-north-1",
+                    "cn-northwest-1"
+                ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
         "scheduler": {
@@ -9321,14 +9335,15 @@
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-south-2",
                     "eu-west-1",
```

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/allowlist/allowlist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/allowlist/allowlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,26 +111,35 @@
             f"{error.__class__.__name__} -- {error}[{error.__traceback__.tb_lineno}]"
         )
         sys.exit(1)
 
 
 def is_allowlisted(allowlist, audited_account, check, region, resource, tags):
     try:
+        allowlisted_checks = {}
         # By default is not allowlisted
         is_finding_allowlisted = False
         # First set account key from allowlist dict
         if audited_account in allowlist["Accounts"]:
-            account = audited_account
+            allowlisted_checks = allowlist["Accounts"][audited_account]["Checks"]
         # If there is a *, it affects to all accounts
-        elif "*" in allowlist["Accounts"]:
-            account = "*"
+        # This cannot be elif since in the case of * and single accounts we
+        # want to merge allowlisted checks from * to the other accounts check list
+        if "*" in allowlist["Accounts"]:
+            checks_multi_account = allowlist["Accounts"]["*"]["Checks"]
         # Test if it is allowlisted
-        allowlisted_checks = allowlist["Accounts"][account]["Checks"]
+        allowlisted_checks.update(checks_multi_account)
         if is_allowlisted_in_check(
-            allowlisted_checks, audited_account, account, check, region, resource, tags
+            allowlisted_checks,
+            audited_account,
+            audited_account,
+            check,
+            region,
+            resource,
+            tags,
         ):
             is_finding_allowlisted = True
 
         return is_finding_allowlisted
     except Exception as error:
         logger.critical(
             f"{error.__class__.__name__} -- {error}[{error.__traceback__.tb_lineno}]"
```

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/arn.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/arn.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/error.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/error.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/arn/models.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/arn/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/audit_info/audit_info.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/audit_info/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/audit_info/models.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/credentials/credentials.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/organizations/organizations.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/organizations/organizations.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/lib/security_hub/security_hub.py` & `prowler_cloud-3.7.1/prowler/providers/aws/lib/security_hub/security_hub.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/account/account_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/account/account_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/acm/acm_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/acm/acm_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/appstream/appstream_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/appstream/appstream_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/awslambda/awslambda_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/awslambda/awslambda_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/codebuild/codebuild_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/codebuild/codebuild_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/config/config_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/config/config_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/drs/drs_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/drs/drs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/ec2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/ec2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/lib/network_acls.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/lib/network_acls.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ec2/lib/security_groups.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ec2/lib/security_groups.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecr/ecr_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecr/ecr_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/efs/efs_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/efs/efs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/eks/eks_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/eks/eks_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/emr/emr_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/fms/fms_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/fms/fms_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/glue/glue_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/guardduty/guardduty_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/guardduty/guardduty_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,25 +359,31 @@
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __list_attached_role_policies__(self):
         logger.info("IAM - List Attached User Policies...")
         try:
             for role in self.roles:
-                attached_role_policies = []
-                list_attached_role_policies_paginator = self.client.get_paginator(
-                    "list_attached_role_policies"
-                )
-                for page in list_attached_role_policies_paginator.paginate(
-                    RoleName=role.name
-                ):
-                    for policy in page["AttachedPolicies"]:
-                        attached_role_policies.append(policy)
+                try:
+                    attached_role_policies = []
+                    list_attached_role_policies_paginator = self.client.get_paginator(
+                        "list_attached_role_policies"
+                    )
+                    for page in list_attached_role_policies_paginator.paginate(
+                        RoleName=role.name
+                    ):
+                        for policy in page["AttachedPolicies"]:
+                            attached_role_policies.append(policy)
 
-                role.attached_policies = attached_role_policies
+                    role.attached_policies = attached_role_policies
+                except ClientError as error:
+                    if error.response["Error"]["Code"] == "NoSuchEntityException":
+                        logger.warning(
+                            f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                        )
 
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __list_inline_user_policies__(self):
```

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/inspector2/inspector2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/inspector2/inspector2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/kms/kms_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/macie/macie_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/macie/macie_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/redshift/redshift_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/route53/route53_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/route53/route53_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/s3/s3_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/securityhub/securityhub_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/securityhub/securityhub_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/shield/shield_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/shield/shield_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
+from prowler.providers.aws.lib.policy_condition_parser.policy_condition_parser import (
+    is_account_only_allowed_in_condition,
+)
 from prowler.providers.aws.services.sqs.sqs_client import sqs_client
 
 
 class sqs_queues_not_publicly_accessible(Check):
     def execute(self):
         findings = []
         for queue in sqs_client.queues:
@@ -24,18 +27,20 @@
                                 and "*" in statement["Principal"]["AWS"]
                             )
                             or (
                                 "CanonicalUser" in statement["Principal"]
                                 and "*" in statement["Principal"]["CanonicalUser"]
                             )
                         ):
-                            if "Condition" not in statement:
-                                report.status = "FAIL"
-                                report.status_extended = (
-                                    f"SQS queue {queue.id} policy with public access"
+                            if (
+                                "Condition" in statement
+                                and is_account_only_allowed_in_condition(
+                                    statement["Condition"], sqs_client.audited_account
                                 )
+                            ):
+                                report.status_extended = f"SQS queue {queue.id} is not public because its policy only allows access from the same account"
                             else:
                                 report.status = "FAIL"
-                                report.status_extended = f"SQS queue {queue.id} policy with public access but has a Condition"
+                                report.status_extended = f"SQS queue {queue.id} is public because its policy allows public access"
             findings.append(report)
 
         return findings
```

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/sqs/sqs_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssm/ssm_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssm/ssm_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/waf/waf_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/waf/waf_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/wafv2/wafv2_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/wafv2/wafv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_service.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py` & `prowler_cloud-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/azure_provider.py` & `prowler_cloud-3.7.1/prowler/providers/azure/azure_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/lib/audit_info/models.py` & `prowler_cloud-3.7.1/prowler/providers/azure/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/defender/defender_service.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/defender/defender_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_service.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/azure/services/storage/storage_service.py` & `prowler_cloud-3.7.1/prowler/providers/azure/services/storage/storage_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/common/allowlist.py` & `prowler_cloud-3.7.1/prowler/providers/common/allowlist.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/common/audit_info.py` & `prowler_cloud-3.7.1/prowler/providers/common/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/common/outputs.py` & `prowler_cloud-3.7.1/prowler/providers/common/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/common/quick_inventory.py` & `prowler_cloud-3.7.1/prowler/providers/common/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/gcp_provider.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/gcp_provider.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/lib/audit_info/models.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/dns/dns_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/dns/dns_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,10 +26,11 @@
         for project in cloudresourcemanager_client.project_ids:
             if project not in failed_projects:
                 report = Check_Report_GCP(self.metadata())
                 report.project_id = project
                 report.resource_id = project
                 report.resource_name = ""
                 report.status = "PASS"
+                report.location = cloudresourcemanager_client.region
                 report.status_extended = f"No IAM Users assigned to service roles at project level {project}."
                 findings.append(report)
         return findings
```

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/iam/iam_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/kms/kms_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_service.py` & `prowler_cloud-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_service.py`

 * *Files identical despite different names*

### Comparing `prowler_cloud-3.7.0/pyproject.toml` & `prowler_cloud-3.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,34 @@
   "Pepe Fagoaga <pepe@verica.io>"
 ]
 name = "prowler-cloud"
 packages = [
   {include = "prowler"}
 ]
 readme = "README.md"
-version = "3.7.0"
+version = "3.7.1"
 
 [tool.poetry.dependencies]
 alive-progress = "3.1.4"
 awsipranges = "0.3.3"
 azure-identity = "1.13.0"
 azure-mgmt-authorization = "3.0.0"
 azure-mgmt-security = "5.0.0"
 azure-mgmt-storage = "21.0.0"
 azure-mgmt-subscription = "3.1.1"
 azure-storage-blob = "12.16.0"
-boto3 = "1.26.161"
+boto3 = "1.26.165"
 botocore = "1.29.165"
 colorama = "0.4.6"
 detect-secrets = "1.4.0"
-google-api-python-client = "2.91.0"
+google-api-python-client = "2.92.0"
 mkdocs = {version = "1.4.3", optional = true}
 mkdocs-material = {version = "9.1.18", optional = true}
 msgraph-core = "0.2.2"
-pydantic = "1.10.9"
+pydantic = "1.10.11"
 python = "^3.9"
 schema = "0.7.5"
 shodan = "1.29.1"
 slack-sdk = "3.21.3"
 tabulate = "0.9.0"
 
 [tool.poetry.extras]
@@ -55,18 +55,18 @@
 bandit = "1.7.5"
 black = "22.12.0"
 coverage = "7.2.7"
 docker = "6.1.3"
 flake8 = "6.0.0"
 freezegun = "1.2.2"
 moto = "4.1.12"
-openapi-spec-validator = "0.5.7"
+openapi-spec-validator = "0.6.0"
 pylint = "2.17.4"
 pytest = "7.4.0"
-pytest-randomly = "3.12.0"
+pytest-randomly = "3.13.0"
 pytest-xdist = "3.3.1"
 safety = "2.3.5"
 sure = "2.0.1"
 vulture = "2.7"
 
 [tool.poetry.scripts]
 prowler = "prowler.__main__:prowler"
```

### Comparing `prowler_cloud-3.7.0/PKG-INFO` & `prowler_cloud-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: prowler-cloud
-Version: 3.7.0
+Version: 3.7.1
 Summary: Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.
 License: Apache-2.0
 Author: Toni de la Fuente
 Author-email: toni@blyx.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@verica.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: alive-progress (==3.1.4)
 Requires-Dist: awsipranges (==0.3.3)
 Requires-Dist: azure-identity (==1.13.0)
 Requires-Dist: azure-mgmt-authorization (==3.0.0)
 Requires-Dist: azure-mgmt-security (==5.0.0)
 Requires-Dist: azure-mgmt-storage (==21.0.0)
 Requires-Dist: azure-mgmt-subscription (==3.1.1)
 Requires-Dist: azure-storage-blob (==12.16.0)
-Requires-Dist: boto3 (==1.26.161)
+Requires-Dist: boto3 (==1.26.165)
 Requires-Dist: botocore (==1.29.165)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: detect-secrets (==1.4.0)
-Requires-Dist: google-api-python-client (==2.91.0)
+Requires-Dist: google-api-python-client (==2.92.0)
 Requires-Dist: mkdocs (==1.4.3) ; extra == "docs"
 Requires-Dist: mkdocs-material (==9.1.18) ; extra == "docs"
 Requires-Dist: msgraph-core (==0.2.2)
-Requires-Dist: pydantic (==1.10.9)
+Requires-Dist: pydantic (==1.10.11)
 Requires-Dist: schema (==0.7.5)
 Requires-Dist: shodan (==1.29.1)
 Requires-Dist: slack-sdk (==3.21.3)
 Requires-Dist: tabulate (==0.9.0)
 Project-URL: Changelog, https://github.com/prowler-cloud/prowler/releases
 Project-URL: Documentation, https://docs.prowler.cloud
 Project-URL: Homepage, https://github.com/prowler-cloud/prowler
@@ -78,15 +80,15 @@
 
 `Prowler` is an Open Source security tool to perform AWS, GCP and Azure security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness.
 
 It contains hundreds of controls covering CIS, NIST 800, NIST CSF, CISA, RBI, FedRAMP, PCI-DSS, GDPR, HIPAA, FFIEC, SOC2, GXP, AWS Well-Architected Framework Security Pillar, AWS Foundational Technical Review (FTR), ENS (Spainish National Security Schema) and your custom security frameworks.
 
 | Provider | Checks | Services | [Compliance Frameworks](https://docs.prowler.cloud/en/latest/tutorials/compliance/) | [Categories](https://docs.prowler.cloud/en/latest/tutorials/misc/#categories) |
 |---|---|---|---|---|
-| AWS | 283 | 55 -> `prowler aws --list-services` | 21 -> `prowler aws --list-compliance` | 5 -> `prowler aws --list-categories` |
+| AWS | 283 | 55 -> `prowler aws --list-services` | 25 -> `prowler aws --list-compliance` | 5 -> `prowler aws --list-categories` |
 | GCP | 73 | 11 -> `prowler gcp --list-services` | 1 -> `prowler gcp --list-compliance` | 0 -> `prowler gcp --list-categories`|
 | Azure | 20 | 3 -> `prowler azure --list-services` | CIS soon | 1 -> `prowler azure --list-categories` |
 | Kubernetes | Planned | - | - | - |
 
 # 📖 Documentation
 
 The full documentation can now be found at [https://docs.prowler.cloud](https://docs.prowler.cloud)
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: prowler-cloud Version: 3.7.0 Summary: Prowler is an
+Metadata-Version: 2.1 Name: prowler-cloud Version: 3.7.1 Summary: Prowler is an
 Open Source security tool to perform Cloud Security best practices assessments,
 audits, incident response, continuous monitoring, hardening and forensics
 readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001,
 GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks. License:
 Apache-2.0 Author: Toni de la Fuente Author-email: toni@blyx.com Maintainer:
 Sergio Garcia Maintainer-email: sergio@verica.io Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist:
-alive-progress (==3.1.4) Requires-Dist: awsipranges (==0.3.3) Requires-Dist:
-azure-identity (==1.13.0) Requires-Dist: azure-mgmt-authorization (==3.0.0)
-Requires-Dist: azure-mgmt-security (==5.0.0) Requires-Dist: azure-mgmt-storage
-(==21.0.0) Requires-Dist: azure-mgmt-subscription (==3.1.1) Requires-Dist:
-azure-storage-blob (==12.16.0) Requires-Dist: boto3 (==1.26.161) Requires-Dist:
-botocore (==1.29.165) Requires-Dist: colorama (==0.4.6) Requires-Dist: detect-
-secrets (==1.4.0) Requires-Dist: google-api-python-client (==2.91.0) Requires-
-Dist: mkdocs (==1.4.3) ; extra == "docs" Requires-Dist: mkdocs-material
-(==9.1.18) ; extra == "docs" Requires-Dist: msgraph-core (==0.2.2) Requires-
-Dist: pydantic (==1.10.9) Requires-Dist: schema (==0.7.5) Requires-Dist: shodan
-(==1.29.1) Requires-Dist: slack-sdk (==3.21.3) Requires-Dist: tabulate
-(==0.9.0) Project-URL: Changelog, https://github.com/prowler-cloud/prowler/
-releases Project-URL: Documentation, https://docs.prowler.cloud Project-URL:
-Homepage, https://github.com/prowler-cloud/prowler Project-URL: Issue tracker,
-https://github.com/prowler-cloud/prowler/issues Description-Content-Type: text/
-markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Provides-Extra:
+docs Requires-Dist: alive-progress (==3.1.4) Requires-Dist: awsipranges
+(==0.3.3) Requires-Dist: azure-identity (==1.13.0) Requires-Dist: azure-mgmt-
+authorization (==3.0.0) Requires-Dist: azure-mgmt-security (==5.0.0) Requires-
+Dist: azure-mgmt-storage (==21.0.0) Requires-Dist: azure-mgmt-subscription
+(==3.1.1) Requires-Dist: azure-storage-blob (==12.16.0) Requires-Dist: boto3
+(==1.26.165) Requires-Dist: botocore (==1.29.165) Requires-Dist: colorama
+(==0.4.6) Requires-Dist: detect-secrets (==1.4.0) Requires-Dist: google-api-
+python-client (==2.92.0) Requires-Dist: mkdocs (==1.4.3) ; extra == "docs"
+Requires-Dist: mkdocs-material (==9.1.18) ; extra == "docs" Requires-Dist:
+msgraph-core (==0.2.2) Requires-Dist: pydantic (==1.10.11) Requires-Dist:
+schema (==0.7.5) Requires-Dist: shodan (==1.29.1) Requires-Dist: slack-sdk
+(==3.21.3) Requires-Dist: tabulate (==0.9.0) Project-URL: Changelog, https://
+github.com/prowler-cloud/prowler/releases Project-URL: Documentation, https://
+docs.prowler.cloud Project-URL: Homepage, https://github.com/prowler-cloud/
+prowler Project-URL: Issue tracker, https://github.com/prowler-cloud/prowler/
+issues Description-Content-Type: text/markdown
                 [https://github.com/prowler-cloud/prowler/blob/
         62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-
 dark.png?raw=True#gh-dark-mode-only] [https://github.com/prowler-cloud/prowler/
       blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-
                     light.png?raw=True#gh-light-mode-only]
   See all the things you and your team can do with ProwlerPro at prowler.pro
 ===============================================================================
@@ -44,15 +45,15 @@
 of controls covering CIS, NIST 800, NIST CSF, CISA, RBI, FedRAMP, PCI-DSS,
 GDPR, HIPAA, FFIEC, SOC2, GXP, AWS Well-Architected Framework Security Pillar,
 AWS Foundational Technical Review (FTR), ENS (Spainish National Security
 Schema) and your custom security frameworks. | Provider | Checks | Services |
 [Compliance Frameworks](https://docs.prowler.cloud/en/latest/tutorials/
 compliance/) | [Categories](https://docs.prowler.cloud/en/latest/tutorials/
 misc/#categories) | |---|---|---|---|---| | AWS | 283 | 55 -> `prowler aws --
-list-services` | 21 -> `prowler aws --list-compliance` | 5 -> `prowler aws --
+list-services` | 25 -> `prowler aws --list-compliance` | 5 -> `prowler aws --
 list-categories` | | GCP | 73 | 11 -> `prowler gcp --list-services` | 1 -
 > `prowler gcp --list-compliance` | 0 -> `prowler gcp --list-categories`| |
 Azure | 20 | 3 -> `prowler azure --list-services` | CIS soon | 1 -> `prowler
 azure --list-categories` | | Kubernetes | Planned | - | - | - | # ð
 Documentation The full documentation can now be found at [https://
 docs.prowler.cloud](https://docs.prowler.cloud) ## Looking for Prowler v2
 documentation? For Prowler v2 Documentation, please go to https://github.com/
```

